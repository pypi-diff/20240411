# Comparing `tmp/henryobj-0.2.2.tar.gz` & `tmp/henryobj-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henryobj-0.2.2.tar", last modified: Tue Apr  9 07:09:00 2024, max compression
+gzip compressed data, was "henryobj-0.2.3.tar", last modified: Wed Apr 10 09:35:51 2024, max compression
```

## Comparing `henryobj-0.2.2.tar` & `henryobj-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-09 07:09:00.000698 henryobj-0.2.2/
--rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-09 07:09:00.000568 henryobj-0.2.2/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)     2976 2024-01-24 08:03:39.000000 henryobj-0.2.2/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-09 07:08:59.999588 henryobj-0.2.2/henryobj/
--rw-r--r--   0 henry      (501) staff       (20)      224 2024-04-09 07:08:41.000000 henryobj-0.2.2/henryobj/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)    21017 2024-03-30 16:01:52.000000 henryobj-0.2.2/henryobj/base.py
--rw-r--r--   0 henry      (501) staff       (20)     1475 2024-03-30 15:45:13.000000 henryobj-0.2.2/henryobj/config.py
--rw-r--r--   0 henry      (501) staff       (20)    15087 2024-03-30 15:15:07.000000 henryobj-0.2.2/henryobj/gpt.py
--rw-r--r--   0 henry      (501) staff       (20)    24819 2024-03-30 16:01:22.000000 henryobj-0.2.2/henryobj/oai.py
--rw-r--r--   0 henry      (501) staff       (20)    14268 2024-03-30 15:59:40.000000 henryobj-0.2.2/henryobj/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-09 07:09:00.000399 henryobj-0.2.2/henryobj.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-09 07:08:59.000000 henryobj-0.2.2/henryobj.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      282 2024-04-09 07:08:59.000000 henryobj-0.2.2/henryobj.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-04-09 07:08:59.000000 henryobj-0.2.2/henryobj.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       60 2024-04-09 07:08:59.000000 henryobj-0.2.2/henryobj.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)        9 2024-04-09 07:08:59.000000 henryobj-0.2.2/henryobj.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-04-09 07:09:00.000742 henryobj-0.2.2/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      574 2024-04-09 07:07:08.000000 henryobj-0.2.2/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-10 09:35:51.446456 henryobj-0.2.3/
+-rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-10 09:35:51.446309 henryobj-0.2.3/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)     2976 2024-01-24 08:03:39.000000 henryobj-0.2.3/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-10 09:35:51.445292 henryobj-0.2.3/henryobj/
+-rw-r--r--   0 henry      (501) staff       (20)      224 2024-04-09 07:08:41.000000 henryobj-0.2.3/henryobj/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)    22625 2024-04-10 09:35:29.000000 henryobj-0.2.3/henryobj/base.py
+-rw-r--r--   0 henry      (501) staff       (20)     1543 2024-04-10 09:35:13.000000 henryobj-0.2.3/henryobj/config.py
+-rw-r--r--   0 henry      (501) staff       (20)    15087 2024-03-30 15:15:07.000000 henryobj-0.2.3/henryobj/gpt.py
+-rw-r--r--   0 henry      (501) staff       (20)    28883 2024-04-09 16:04:06.000000 henryobj-0.2.3/henryobj/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)    14268 2024-03-30 15:59:40.000000 henryobj-0.2.3/henryobj/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-10 09:35:51.446083 henryobj-0.2.3/henryobj.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-10 09:35:51.000000 henryobj-0.2.3/henryobj.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      282 2024-04-10 09:35:51.000000 henryobj-0.2.3/henryobj.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-04-10 09:35:51.000000 henryobj-0.2.3/henryobj.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       60 2024-04-10 09:35:51.000000 henryobj-0.2.3/henryobj.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)        9 2024-04-10 09:35:51.000000 henryobj-0.2.3/henryobj.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-04-10 09:35:51.446520 henryobj-0.2.3/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      574 2024-04-10 09:35:42.000000 henryobj-0.2.3/setup.py
```

### Comparing `henryobj-0.2.2/PKG-INFO` & `henryobj-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henryobj
-Version: 0.2.2
+Version: 0.2.3
 Home-page: https://github.com/HenryObj/mypip
 Description-Content-Type: text/markdown
 
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
```

### Comparing `henryobj-0.2.2/README.md` & `henryobj-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.2/henryobj/base.py` & `henryobj-0.2.3/henryobj/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Utility functions
 
 
-from .config import WARNING_UNKNOWN
+from .config import WARNING_UNKNOWN, CODE_ERR_PT, CODE_WARN_PT
 
 
 from typing import Callable, Any, Union, Optional
 from collections import Counter
 import pathspec
 import datetime
 import requests
@@ -199,15 +199,15 @@
     additional = f"""
     ****************************************
     Additional Info: 
     {additional_info}
     ****************************************""" if additional_info else ""
     print(f"""
     ----------------------------------------------------------------
-    🚨 ERROR HO144 🚨
+    🚨 ERROR 🚨
     Occurred: {now}
     Module: {module_name} | Function: {function_name}
     Exception: {exception}{additional}
     ----------------------------------------------------------------
     """)
 
 def log_warning(warning:str, func: Callable[..., Any], additional_info: str = "") -> None:
@@ -243,14 +243,48 @@
     👋 Warning 🟠
     Occurred: {now}
     Module: {module_name} | Function: {function_name}
     Warning message: {warning}{additional}
     ----------------------------------------------------------------
     """)
 
+def log_issue_papertrail(exception: Exception, func: Callable[..., Any], additional_info: str = "") -> None:
+    """
+    Same as log_issue but on one line with a special key to find it.
+    """
+    now = datetime.datetime.now().strftime("%d/%m/%y %H:%M:%S")
+    if hasattr(func, '__name__'):
+        function_name = func.__name__
+        module_name = get_module_name(func)
+    else:
+        function_name = func if isinstance(func, str) else WARNING_UNKNOWN
+        try:
+            module_name = get_module_name(func)
+        except:
+            module_name = "Couldn't get the module name"
+    additional = additional_info.replace("\n"," ") if additional_info else ""
+    print(f"🚨 {CODE_ERR_PT} 🚨 ** | {function_name} in {module_name} | {exception} ** {additional} | {now} | END")
+
+def log_warning_papertrail(exception: Exception, func: Callable[..., Any], additional_info: str = "") -> None:
+    """
+    Same as log_issue but on one line with a special key to find it.
+    """
+    now = datetime.datetime.now().strftime("%d/%m/%y %H:%M:%S")
+    if hasattr(func, '__name__'):
+        function_name = func.__name__
+        module_name = get_module_name(func)
+    else:
+        function_name = func if isinstance(func, str) else WARNING_UNKNOWN
+        try:
+            module_name = get_module_name(func)
+        except:
+            module_name = "Couldn't get the module name"
+    additional = additional_info.replace("\n"," ") if additional_info else ""
+    print(f"👋 {CODE_WARN_PT} 🟠 ** | {function_name} in {module_name} | {exception} ** {additional} | {now} | END")
+
 def print_style(message, color="blue", bold=False):
     """
     To print a message in a specific color.
     Check the function for the list of available colors.
     """
     bold_code = "\033[1m" if bold else ""
     colors = {
```

### Comparing `henryobj-0.2.2/henryobj/config.py` & `henryobj-0.2.3/henryobj/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,8 +41,12 @@
 MODEL_OLD = r"text-embedding-ada-002"
 MODEL_EMB_LARGE = r"text-embedding-3-large"
 MODEL_EMB_SMALL = r"text-embedding-3-small"
 
 
 # ******* GPT
 BUFFER_README_INPUT = 30000
-LARGE_INPUT_THRESHOLD = 10000  # Threshold for considering an input as large
+LARGE_INPUT_THRESHOLD = 10000  # Threshold for considering an input as large
+
+# ******* Papertrail
+CODE_ERR_PT = r"HO144"
+CODE_WARN_PT = r"HO69"
```

### Comparing `henryobj-0.2.2/henryobj/gpt.py` & `henryobj-0.2.3/henryobj/gpt.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.2/henryobj/oai.py` & `henryobj-0.2.3/henryobj/oai.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 from typing import Optional
 
 import tiktoken
 import openai
 import time
+import json
 import os
 import re
 
 
 # ****************************************** INIT CLIENT *****************************************
 
 
@@ -266,14 +267,23 @@
 def initialize_role_in_chatTable(role_definition: str) -> list[dict[str, str]]:
     """
     We need to define how we want our model to perform.
     This function takes this definition as a input and returns it into the chat_table_format.
     """
     return [{"role":"system", "content":role_definition}]
 
+def make_string_json_safe(s : str) -> str:
+    """
+    Replace newlines, tabs, and other control characters
+    """
+    s = s.replace('"', "'")
+    s = s.replace("\n", "\\n").replace("\r", "\\r").replace("\t", "\\t")
+    s = s.strip()
+    return s
+
 def print_gpt_models(all:bool=True) -> None:
     """
     To list the gpt models provided by OpenAI.
     
     Args:
         all: If True, will print all the models. Else, only the 'GPT' ones.
         verbose: If False, will only print the name. Else, everything.
@@ -309,14 +319,87 @@
         name = "Input text"
     else:
         return # to avoid error in case of wrong input
     tok = calculate_token(content)
     out = f"{name}: {len(content)} chars  **  ~ {tok} tokens ** ~ ${round(tok/1000 * price,2)}"
     print(out)
 
+def repair_gpt_conversation(conversation_as_string: str) -> Optional[str]:
+    """
+    Repair a GPT conversation to ensure we can then json.loads() it.
+    Returns the fixed conversation. 
+    """
+    result = None
+    try:
+        new_list = []
+        user_ = r'{"role": "user", "content":'
+        assistant_ = r'{"role": "assistant", "content":'
+        len_a = len(assistant_)
+        len_u = len(user_)
+        while True:
+            bal_user = conversation_as_string.find(user_)
+            bal_assistant = conversation_as_string.find(assistant_)
+            # Cases: over-over / user-over / assistant-over THEN:: user-user / assistant-assistant / user-assistant / assistant-user
+            
+            # over-over
+            if bal_user == -1 and bal_assistant == -1: 
+                break
+            
+            next_bala = conversation_as_string.find(assistant_, bal_assistant + len_a)
+            next_balu = conversation_as_string.find(user_, bal_user + len_u)
+            
+            # assistant-over
+            if bal_user == -1 and next_bala == -1:
+                content = make_string_json_safe(conversation_as_string[bal_assistant + len_a: conversation_as_string.rfind("}")])
+                new_list.append({"role": "assistant", "content":content})
+                break
+            # user-over
+            if bal_assistant == -1 and next_balu == -1:
+                content = make_string_json_safe(conversation_as_string[bal_user + len_u: conversation_as_string.rfind("}")])
+                new_list.append({"role": "user", "content":content})
+                break
+            
+            # user-user
+            if (0 < bal_user < next_balu < bal_assistant or 
+                bal_assistant == -1 and 0 < bal_user < next_balu):
+                role = "user"
+                content = make_string_json_safe(conversation_as_string[bal_user + len_u: conversation_as_string.rfind("}", None, next_balu)])
+                conversation_as_string = conversation_as_string[conversation_as_string.rfind("}", None, next_balu):]
+            # assistant-assistant
+            elif (0 < bal_assistant < next_bala < bal_user or 
+                bal_user == -1 and 0 < bal_assistant < next_bala):
+                role = "assistant"
+                content = make_string_json_safe(conversation_as_string[bal_assistant + len_a: conversation_as_string.rfind("}", None, next_bala)])
+                conversation_as_string = conversation_as_string[conversation_as_string.rfind("}", None, next_bala):]
+            # user-assistant
+            elif 0 < bal_user < bal_assistant:
+                role = "user"
+                content = make_string_json_safe(conversation_as_string[bal_user + len_u: conversation_as_string.rfind("}", None, bal_assistant)])
+                conversation_as_string = conversation_as_string[conversation_as_string.rfind("}", None, bal_assistant):]
+            # assistant-user
+            elif 0 < bal_assistant < bal_user:
+                role = "assistant"
+                content = make_string_json_safe(conversation_as_string[bal_assistant + len_a: conversation_as_string.rfind("}", None, bal_user)])
+                conversation_as_string = conversation_as_string[conversation_as_string.rfind("}", None, bal_user):]
+            else:
+                print("issue - weird use case")
+                print(bal_assistant, bal_user, next_bala, next_balu)
+                print(conversation_as_string)
+                return
+            new_list.append({"role": role, "content":content})
+        try:
+            result = json.dumps(new_list)
+            json.loads(result)
+        except Exception as e:
+            log_issue(e, repair_gpt_conversation)
+            return
+    except Exception as e:
+        log_issue(e, repair_gpt_conversation)
+    return result
+
 def retry_if_too_short(func, *args, **kwargs):
     """
     Retry a given function if its output is too short.
     
     Args:
         func (callable): The function to be called.
         *args: Positional arguments passed to the `func`.
```

### Comparing `henryobj-0.2.2/henryobj/web.py` & `henryobj-0.2.3/henryobj/web.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.2/henryobj.egg-info/PKG-INFO` & `henryobj-0.2.3/henryobj.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henryobj
-Version: 0.2.2
+Version: 0.2.3
 Home-page: https://github.com/HenryObj/mypip
 Description-Content-Type: text/markdown
 
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
```

### Comparing `henryobj-0.2.2/setup.py` & `henryobj-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="henryobj",
-    version="0.2.2", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.2.3", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/mypip',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

