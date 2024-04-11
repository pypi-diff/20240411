# Comparing `tmp/luoguapi-0.1.1.tar.gz` & `tmp/luoguapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luoguapi-0.1.1.tar", last modified: Thu Apr 11 13:29:43 2024, max compression
+gzip compressed data, was "luoguapi-0.1.2.tar", last modified: Thu Apr 11 13:37:48 2024, max compression
```

## Comparing `luoguapi-0.1.1.tar` & `luoguapi-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 13:29:43.754102 luoguapi-0.1.1/
--rw-rw-rw-   0        0        0    35757 2024-04-11 13:18:58.000000 luoguapi-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      182 2024-04-11 13:29:43.751537 luoguapi-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      152 2024-04-11 13:18:58.000000 luoguapi-0.1.1/README.rst
--rw-rw-rw-   0        0        0       42 2024-04-11 13:29:43.755102 luoguapi-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      215 2024-04-11 13:29:36.000000 luoguapi-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 13:29:43.718003 luoguapi-0.1.1/src/
--rw-rw-rw-   0        0        0       17 2024-04-11 13:18:58.000000 luoguapi-0.1.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 13:29:43.749537 luoguapi-0.1.1/src/luoguapi.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-11 13:29:43.000000 luoguapi-0.1.1/src/luoguapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-04-11 13:29:43.000000 luoguapi-0.1.1/src/luoguapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 13:29:43.000000 luoguapi-0.1.1/src/luoguapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-11 13:29:43.000000 luoguapi-0.1.1/src/luoguapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8669 2024-04-11 13:28:11.000000 luoguapi-0.1.1/src/luoguapi.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:37:48.068222 luoguapi-0.1.2/
+-rw-rw-rw-   0        0        0    35757 2024-04-11 13:18:58.000000 luoguapi-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      182 2024-04-11 13:37:48.066222 luoguapi-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2024-04-11 13:18:58.000000 luoguapi-0.1.2/README.rst
+-rw-rw-rw-   0        0        0       42 2024-04-11 13:37:48.069223 luoguapi-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      215 2024-04-11 13:37:43.000000 luoguapi-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:37:48.029567 luoguapi-0.1.2/src/
+-rw-rw-rw-   0        0        0       17 2024-04-11 13:18:58.000000 luoguapi-0.1.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:37:48.065224 luoguapi-0.1.2/src/luoguapi.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-11 13:37:47.000000 luoguapi-0.1.2/src/luoguapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-04-11 13:37:47.000000 luoguapi-0.1.2/src/luoguapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 13:37:47.000000 luoguapi-0.1.2/src/luoguapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-11 13:37:47.000000 luoguapi-0.1.2/src/luoguapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8642 2024-04-11 13:37:35.000000 luoguapi-0.1.2/src/luoguapi.py
```

### Comparing `luoguapi-0.1.1/LICENSE.txt` & `luoguapi-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `luoguapi-0.1.1/src/luoguapi.py` & `luoguapi-0.1.2/src/luoguapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
             response = rmd(
                 response.text, 'JSON.parse(decodeURIComponent("', '"));')
             response = urlDecode(response)
             response = json.loads(response)
             if response['code'] == 400:
                 return [False, 'Invalid Arguments']
             else:
-                return [True, response['currentData']['problems']]
+                return [True, response]
 
         def get(self, uid: str):
             '''
             获取指定题目
             @arg uid: 题目编号
             @return 如果成功获取返回 [True, <题目 json 格式数据>], 失败返回原因 [False, <Problem Not Found>]
             '''
```

