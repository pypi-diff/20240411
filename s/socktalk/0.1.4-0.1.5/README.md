# Comparing `tmp/socktalk-0.1.4.tar.gz` & `tmp/socktalk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socktalk-0.1.4.tar", last modified: Wed Apr 10 11:15:01 2024, max compression
+gzip compressed data, was "socktalk-0.1.5.tar", last modified: Thu Apr 11 11:56:02 2024, max compression
```

## Comparing `socktalk-0.1.4.tar` & `socktalk-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 11:15:01.589890 socktalk-0.1.4/
--rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.1.4/LICENSE
--rw-r--r--   0 mike      (1000) mike      (1000)     3853 2024-04-10 11:15:01.589890 socktalk-0.1.4/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     3362 2024-04-10 11:05:16.000000 socktalk-0.1.4/README.md
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 11:15:01.589890 socktalk-0.1.4/server_client/
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.1.4/server_client/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     5408 2024-04-09 11:09:29.000000 socktalk-0.1.4/server_client/ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.1.4/server_client/client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3984 2024-04-10 09:06:22.000000 socktalk-0.1.4/server_client/server.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2527 2024-04-10 09:05:25.000000 socktalk-0.1.4/server_client/start_server_with_ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-10 11:15:01.589890 socktalk-0.1.4/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     1005 2024-04-10 11:14:19.000000 socktalk-0.1.4/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 11:15:01.589890 socktalk-0.1.4/socktalk.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)     3853 2024-04-10 11:15:01.000000 socktalk-0.1.4/socktalk.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      366 2024-04-10 11:15:01.000000 socktalk-0.1.4/socktalk.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-10 11:15:01.000000 socktalk-0.1.4/socktalk.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      157 2024-04-10 11:15:01.000000 socktalk-0.1.4/socktalk.egg-info/entry_points.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       30 2024-04-10 11:15:01.000000 socktalk-0.1.4/socktalk.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-10 11:15:01.000000 socktalk-0.1.4/socktalk.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 11:56:02.409703 socktalk-0.1.5/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.1.5/LICENSE
+-rw-r--r--   0 mike      (1000) mike      (1000)     4129 2024-04-11 11:56:02.409703 socktalk-0.1.5/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3638 2024-04-11 11:54:10.000000 socktalk-0.1.5/README.md
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 11:56:02.405703 socktalk-0.1.5/server_client/
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.1.5/server_client/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5390 2024-04-11 11:39:20.000000 socktalk-0.1.5/server_client/ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.1.5/server_client/client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3984 2024-04-10 09:06:22.000000 socktalk-0.1.5/server_client/server.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3456 2024-04-11 11:27:09.000000 socktalk-0.1.5/server_client/start_server_with_ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-11 11:56:02.409703 socktalk-0.1.5/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1005 2024-04-11 11:50:34.000000 socktalk-0.1.5/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 11:56:02.409703 socktalk-0.1.5/socktalk.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)     4129 2024-04-11 11:56:02.000000 socktalk-0.1.5/socktalk.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      366 2024-04-11 11:56:02.000000 socktalk-0.1.5/socktalk.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-11 11:56:02.000000 socktalk-0.1.5/socktalk.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      157 2024-04-11 11:56:02.000000 socktalk-0.1.5/socktalk.egg-info/entry_points.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       30 2024-04-11 11:56:02.000000 socktalk-0.1.5/socktalk.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-11 11:56:02.000000 socktalk-0.1.5/socktalk.egg-info/top_level.txt
```

### Comparing `socktalk-0.1.4/LICENSE` & `socktalk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.4/PKG-INFO` & `socktalk-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socktalk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Socket-based AI chat server and multi-user chat client
 Project-URL: Source, https://github.com/mdkmk/chat_server
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -15,39 +15,45 @@
 # "socktalk" Socket-based AI chat server and multi-user chat client
 
 If running the code from the github repository:
 Please install the requirements into a virtual environment, then launch "start_server_with_ai_client.py" after adjusting the settings (send full chat history, ai client api key, enabling ai mode 1 or ai mode 2, editing mode1 or mode2 intervals), then launch "client.py" (can be launched multiple times, for multiple users)
 
 If running the code using the python library "socktalk" (pip install socktalk):
 You can use the following terminal commands:
-1) "ai_server": Runs the chat server with a connected AI client. Currently uses gpt-3.5-turbo model.
+1) "ai_server": Runs the chat server with a connected AI client. Uses gpt-3.5-turbo model by default.
     You should create an environment file named ".env" in the working directory from which you execute the python
     commands for the library, in order to adjust the AI modes and chat server settings.
 
     Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key to function you will need to load at least 5$ of credit on your OpenAI account.
-    The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. See below for more details.
+    The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. AI model can be adjusted. Mode2 content can be adjusted. See below for more details.
 
     ### ".env" file example
-    
+
     OPENAI_API_KEY=<OPENAI_API_KEY_HERE>
 
     SERVER_IP_ADDRESS=127.0.0.1
 
     SERVER_PORT=1234
 
     SEND_FULL_CHAT_HISTORY=True
 
     AI_MODE1_ACTIVE=True
 
     AI_MODE1_INTERVAL=1
 
+    AI_MODE1_MODEL=gpt-3.5-turbo
+
     AI_MODE2_ACTIVE=True
 
     AI_MODE2_INTERVAL=60
 
+    AI_MODE2_MODEL=gpt-3.5-turbo
+
+    AI_MODE2_CONTENT="Say something interesting from a random Wikipedia page and start your response with 'Did you know', but don't mention the source."
+
 
 2) "chat_server": Runs a chat server without a connected AI client. No .env file necessary.
 
 
 3) "chat_client": Runs the user chat client.
```

### Comparing `socktalk-0.1.4/README.md` & `socktalk-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 # "socktalk" Socket-based AI chat server and multi-user chat client
 
 If running the code from the github repository:
 Please install the requirements into a virtual environment, then launch "start_server_with_ai_client.py" after adjusting the settings (send full chat history, ai client api key, enabling ai mode 1 or ai mode 2, editing mode1 or mode2 intervals), then launch "client.py" (can be launched multiple times, for multiple users)
 
 If running the code using the python library "socktalk" (pip install socktalk):
 You can use the following terminal commands:
-1) "ai_server": Runs the chat server with a connected AI client. Currently uses gpt-3.5-turbo model.
+1) "ai_server": Runs the chat server with a connected AI client. Uses gpt-3.5-turbo model by default.
     You should create an environment file named ".env" in the working directory from which you execute the python
     commands for the library, in order to adjust the AI modes and chat server settings.
 
     Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key to function you will need to load at least 5$ of credit on your OpenAI account.
-    The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. See below for more details.
+    The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. AI model can be adjusted. Mode2 content can be adjusted. See below for more details.
 
     ### ".env" file example
-    
+
     OPENAI_API_KEY=<OPENAI_API_KEY_HERE>
 
     SERVER_IP_ADDRESS=127.0.0.1
 
     SERVER_PORT=1234
 
     SEND_FULL_CHAT_HISTORY=True
 
     AI_MODE1_ACTIVE=True
 
     AI_MODE1_INTERVAL=1
 
+    AI_MODE1_MODEL=gpt-3.5-turbo
+
     AI_MODE2_ACTIVE=True
 
     AI_MODE2_INTERVAL=60
 
+    AI_MODE2_MODEL=gpt-3.5-turbo
+
+    AI_MODE2_CONTENT="Say something interesting from a random Wikipedia page and start your response with 'Did you know', but don't mention the source."
+
 
 2) "chat_server": Runs a chat server without a connected AI client. No .env file necessary.
 
 
 3) "chat_client": Runs the user chat client.
```

### Comparing `socktalk-0.1.4/server_client/ai_client.py` & `socktalk-0.1.5/server_client/ai_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,32 +4,36 @@
 import openai
 import errno
 
 
 class AIChatClient:
     HEADER_LENGTH = 10
 
-    def __init__(self, server, ip, port, username, mode1_enabled, mode1_interval, mode2_enabled, mode2_interval, send_full_chat_history):
+    def __init__(self, server, ip, port, username, mode1_enabled, mode1_interval, mode1_model, mode2_enabled,
+                 mode2_interval, mode2_model, send_full_chat_history, mode2_content):
         self.ip = ip
         self.port = port
         self.username = username
         self.mode1_enabled = mode1_enabled
         self.mode1_interval = mode1_interval
+        self.mode1_model = mode1_model
         self.mode2_enabled = mode2_enabled
         self.mode2_interval = mode2_interval
+        self.mode2_model = mode2_model
+        self.conversation_history = []
+        self.send_full_chat_history = send_full_chat_history
+        self.mode2_content = mode2_content
         self.client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.client_socket.connect((self.ip, self.port))
         self.client_socket.setblocking(False)
         self.send_username()
         self.line_count = 0
         self.last_response_time = float('inf')
         self.openai_client = openai.OpenAI(api_key=os.environ.get("OPENAI_API_KEY"))
         self.error_reported = False
-        self.conversation_history = []
-        self.send_full_chat_history = send_full_chat_history
         self.running = True
         self.server = server
 
     def shutdown(self):
         self.running = False
         try:
             self.client_socket.close()
@@ -87,35 +91,34 @@
         if not self.error_reported:
             print(error_message)
             self.send_message(error_message)
             self.error_reported = True
 
     def respond_to_message(self):
         try:
-            messages_to_send = self.conversation_history if self.send_full_chat_history else self.conversation_history[-self.mode1_interval:]
+            messages_to_send = self.conversation_history if self.send_full_chat_history else\
+                self.conversation_history[-self.mode1_interval:]
             print("Sending messages to OpenAI:", messages_to_send)
             chat_completion = self.openai_client.chat.completions.create(
                 messages=messages_to_send,
-                model="gpt-3.5-turbo",
+                model=self.mode1_model,
             )
             response_text = chat_completion.choices[0].message.content
             self.send_message(response_text)
             self.conversation_history.append({"role": "assistant", "content": response_text})
         except Exception as e:
             self.handle_error(f"Error calling OpenAI API: {e}")
 
     def respond_with_new_message(self):
         try:
             chat_completion = self.openai_client.chat.completions.create(
                 messages=[
-                    {"role": "user", "content": "Say something interesting from a random Wikipedia page,"
-                                                " and start your response with 'Did you know', but don't mention"
-                                                " the source."}
+                    {"role": "user", "content": self.mode2_content}
                 ],
-                model="gpt-3.5-turbo",
+                model=self.mode2_model,
             )
             response_text = chat_completion.choices[0].message.content
             self.conversation_history.append({"role": "system", "content": response_text})
             self.send_message(response_text)
         except Exception as e:
             self.handle_error(f"Error calling OpenAI API: {e}")
```

### Comparing `socktalk-0.1.4/server_client/client.py` & `socktalk-0.1.5/server_client/client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.4/server_client/server.py` & `socktalk-0.1.5/server_client/server.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.4/setup.py` & `socktalk-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='socktalk',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     project_urls={
         'Source': 'https://github.com/mdkmk/chat_server'
     },
     install_requires=[
         'PyQt5==5.15.10',
         'openai==1.14.2'
```

### Comparing `socktalk-0.1.4/socktalk.egg-info/PKG-INFO` & `socktalk-0.1.5/socktalk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socktalk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Socket-based AI chat server and multi-user chat client
 Project-URL: Source, https://github.com/mdkmk/chat_server
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -15,39 +15,45 @@
 # "socktalk" Socket-based AI chat server and multi-user chat client
 
 If running the code from the github repository:
 Please install the requirements into a virtual environment, then launch "start_server_with_ai_client.py" after adjusting the settings (send full chat history, ai client api key, enabling ai mode 1 or ai mode 2, editing mode1 or mode2 intervals), then launch "client.py" (can be launched multiple times, for multiple users)
 
 If running the code using the python library "socktalk" (pip install socktalk):
 You can use the following terminal commands:
-1) "ai_server": Runs the chat server with a connected AI client. Currently uses gpt-3.5-turbo model.
+1) "ai_server": Runs the chat server with a connected AI client. Uses gpt-3.5-turbo model by default.
     You should create an environment file named ".env" in the working directory from which you execute the python
     commands for the library, in order to adjust the AI modes and chat server settings.
 
     Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key to function you will need to load at least 5$ of credit on your OpenAI account.
-    The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. See below for more details.
+    The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. AI model can be adjusted. Mode2 content can be adjusted. See below for more details.
 
     ### ".env" file example
-    
+
     OPENAI_API_KEY=<OPENAI_API_KEY_HERE>
 
     SERVER_IP_ADDRESS=127.0.0.1
 
     SERVER_PORT=1234
 
     SEND_FULL_CHAT_HISTORY=True
 
     AI_MODE1_ACTIVE=True
 
     AI_MODE1_INTERVAL=1
 
+    AI_MODE1_MODEL=gpt-3.5-turbo
+
     AI_MODE2_ACTIVE=True
 
     AI_MODE2_INTERVAL=60
 
+    AI_MODE2_MODEL=gpt-3.5-turbo
+
+    AI_MODE2_CONTENT="Say something interesting from a random Wikipedia page and start your response with 'Did you know', but don't mention the source."
+
 
 2) "chat_server": Runs a chat server without a connected AI client. No .env file necessary.
 
 
 3) "chat_client": Runs the user chat client.
```

