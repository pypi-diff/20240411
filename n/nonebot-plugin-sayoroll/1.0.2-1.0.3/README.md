# Comparing `tmp/nonebot-plugin-sayoroll-1.0.2.tar.gz` & `tmp/nonebot-plugin-sayoroll-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sayoroll-1.0.2.tar", last modified: Tue Mar 26 02:06:46 2024, max compression
+gzip compressed data, was "nonebot-plugin-sayoroll-1.0.3.tar", last modified: Thu Apr 11 09:30:36 2024, max compression
```

## Comparing `nonebot-plugin-sayoroll-1.0.2.tar` & `nonebot-plugin-sayoroll-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:06:46.851084 nonebot-plugin-sayoroll-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-26 02:06:43.000000 nonebot-plugin-sayoroll-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-03-26 02:06:46.851084 nonebot-plugin-sayoroll-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-03-26 02:06:43.000000 nonebot-plugin-sayoroll-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:06:46.851084 nonebot-plugin-sayoroll-1.0.2/nonebot_plugin_sayoroll/
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-03-26 02:06:43.000000 nonebot-plugin-sayoroll-1.0.2/nonebot_plugin_sayoroll/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:06:46.851084 nonebot-plugin-sayoroll-1.0.2/nonebot_plugin_sayoroll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-03-26 02:06:46.000000 nonebot-plugin-sayoroll-1.0.2/nonebot_plugin_sayoroll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-26 02:06:46.000000 nonebot-plugin-sayoroll-1.0.2/nonebot_plugin_sayoroll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 02:06:46.000000 nonebot-plugin-sayoroll-1.0.2/nonebot_plugin_sayoroll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-26 02:06:46.000000 nonebot-plugin-sayoroll-1.0.2/nonebot_plugin_sayoroll.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 02:06:46.000000 nonebot-plugin-sayoroll-1.0.2/nonebot_plugin_sayoroll.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 02:06:46.851084 nonebot-plugin-sayoroll-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-26 02:06:43.000000 nonebot-plugin-sayoroll-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:30:36.769732 nonebot-plugin-sayoroll-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 09:30:33.000000 nonebot-plugin-sayoroll-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-11 09:30:36.769732 nonebot-plugin-sayoroll-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-11 09:30:33.000000 nonebot-plugin-sayoroll-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:30:36.769732 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll/
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-11 09:30:33.000000 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:30:36.769732 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-11 09:30:36.000000 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-11 09:30:36.000000 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:30:36.000000 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 09:30:36.000000 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 09:30:36.000000 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:30:36.769732 nonebot-plugin-sayoroll-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-11 09:30:33.000000 nonebot-plugin-sayoroll-1.0.3/setup.py
```

### Comparing `nonebot-plugin-sayoroll-1.0.2/LICENSE` & `nonebot-plugin-sayoroll-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sayoroll-1.0.2/PKG-INFO` & `nonebot-plugin-sayoroll-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sayoroll
-Version: 1.0.2
+Version: 1.0.3
 Summary: 基于NoneBot的高仿以前小夜bot的roll功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 1.0.3 Summary:
 åºäºNoneBotçé«ä»¿ä»¥åå°å¤botçrollåè½ Home-page: https://
 github.com/mas-alone/nonebot-plugin-sayoroll Author: A M D Author-email:
 mas_alone@qq.com Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-
 adapter-onebot>=2.0.0b1 Requires-Dist: nonebot-plugin-alconna>=0.38.2
```

### Comparing `nonebot-plugin-sayoroll-1.0.2/README.md` & `nonebot-plugin-sayoroll-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sayoroll-1.0.2/nonebot_plugin_sayoroll/__init__.py` & `nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import difflib
 from typing import List
 import unicodedata
 import string
 import json
 from pathlib import Path
 
-from nonebot import on_command, require, on_regex
+from nonebot import on_command, require, on_endswith
 from nonebot.internal.adapter import Message
 from nonebot.params import CommandArg
 from nonebot.plugin import PluginMetadata, inherit_supported_adapters
 
 require('nonebot_plugin_alconna')
 from nonebot_plugin_alconna import UniMessage
 
@@ -28,15 +28,15 @@
 
 roll = on_command(
     'roll',
     priority=2,
     block=True
 )
 
-roll_suffix = on_regex(r'[!！/]roll.*概率$', priority=1, block=True)
+roll_suffix = on_endswith(("概率"))
 
 
 def normalize_str(s):
     return unicodedata.normalize('NFKC', s)
 
 
 def get_blocked_words() -> List:
@@ -50,29 +50,27 @@
             data = json.load(f)
         return data
 
 
 @roll_suffix.handle()
 async def _(args: Message = CommandArg()):
     user_input = args.extract_plain_text()
-    user_input = user_input.replace('我', '你').replace('!roll', '').replace('！roll', '').replace('/roll', '')
+    user_input = user_input.replace('我', '你')
     blocked = re.findall('|'.join(get_blocked_words()), user_input, re.IGNORECASE)
     if len(blocked) > 0:
         await UniMessage.text('[{}] 为屏蔽词'.format('] ['.join(blocked))).send(reply_to=True)
         return
     probability = random.uniform(0.01, 100.00)
     msg = '{}为：{:.2f}%'.format(user_input, probability)
     await UniMessage.text(msg).send(reply_to=True)
 
 
 @roll.handle()
 async def _(args: Message = CommandArg()):
     user_input = args.extract_plain_text().strip()
-    if user_input.endswith('概率'):
-        return
     args = args.extract_plain_text().strip()
 
     blocked = re.findall('|'.join(get_blocked_words()), user_input, re.IGNORECASE)
     if len(blocked) > 0:
         await UniMessage.text('[{}] 为屏蔽词'.format('] ['.join(blocked))).send(reply_to=True)
         return
     if not args:
```

### Comparing `nonebot-plugin-sayoroll-1.0.2/nonebot_plugin_sayoroll.egg-info/PKG-INFO` & `nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sayoroll
-Version: 1.0.2
+Version: 1.0.3
 Summary: 基于NoneBot的高仿以前小夜bot的roll功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 1.0.3 Summary:
 åºäºNoneBotçé«ä»¿ä»¥åå°å¤botçrollåè½ Home-page: https://
 github.com/mas-alone/nonebot-plugin-sayoroll Author: A M D Author-email:
 mas_alone@qq.com Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-
 adapter-onebot>=2.0.0b1 Requires-Dist: nonebot-plugin-alconna>=0.38.2
```

### Comparing `nonebot-plugin-sayoroll-1.0.2/setup.py` & `nonebot-plugin-sayoroll-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-sayoroll",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.0.2",  # 程序版本
+    version="1.0.3",  # 程序版本
     author="A M D",  # 项目作者
     author_email="mas_alone@qq.com",  # 作者邮件
     description="基于NoneBot的高仿以前小夜bot的roll功能",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/mas-alone/nonebot-plugin-sayoroll",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

