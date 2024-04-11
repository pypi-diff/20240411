# Comparing `tmp/luoguapi-0.1.2.tar.gz` & `tmp/luoguapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luoguapi-0.1.2.tar", last modified: Thu Apr 11 13:37:48 2024, max compression
+gzip compressed data, was "luoguapi-0.1.3.tar", last modified: Thu Apr 11 13:43:55 2024, max compression
```

## Comparing `luoguapi-0.1.2.tar` & `luoguapi-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 13:37:48.068222 luoguapi-0.1.2/
--rw-rw-rw-   0        0        0    35757 2024-04-11 13:18:58.000000 luoguapi-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      182 2024-04-11 13:37:48.066222 luoguapi-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      152 2024-04-11 13:18:58.000000 luoguapi-0.1.2/README.rst
--rw-rw-rw-   0        0        0       42 2024-04-11 13:37:48.069223 luoguapi-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      215 2024-04-11 13:37:43.000000 luoguapi-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 13:37:48.029567 luoguapi-0.1.2/src/
--rw-rw-rw-   0        0        0       17 2024-04-11 13:18:58.000000 luoguapi-0.1.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 13:37:48.065224 luoguapi-0.1.2/src/luoguapi.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-11 13:37:47.000000 luoguapi-0.1.2/src/luoguapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-04-11 13:37:47.000000 luoguapi-0.1.2/src/luoguapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 13:37:47.000000 luoguapi-0.1.2/src/luoguapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-11 13:37:47.000000 luoguapi-0.1.2/src/luoguapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8642 2024-04-11 13:37:35.000000 luoguapi-0.1.2/src/luoguapi.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:43:55.920549 luoguapi-0.1.3/
+-rw-rw-rw-   0        0        0    35757 2024-04-11 13:18:58.000000 luoguapi-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      182 2024-04-11 13:43:55.917548 luoguapi-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2024-04-11 13:18:58.000000 luoguapi-0.1.3/README.rst
+-rw-rw-rw-   0        0        0       42 2024-04-11 13:43:55.920549 luoguapi-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      215 2024-04-11 13:43:43.000000 luoguapi-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:43:55.899310 luoguapi-0.1.3/src/
+-rw-rw-rw-   0        0        0       17 2024-04-11 13:18:58.000000 luoguapi-0.1.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:43:55.916036 luoguapi-0.1.3/src/luoguapi.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-11 13:43:55.000000 luoguapi-0.1.3/src/luoguapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-04-11 13:43:55.000000 luoguapi-0.1.3/src/luoguapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 13:43:55.000000 luoguapi-0.1.3/src/luoguapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-11 13:43:55.000000 luoguapi-0.1.3/src/luoguapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8654 2024-04-11 13:43:39.000000 luoguapi-0.1.3/src/luoguapi.py
```

### Comparing `luoguapi-0.1.2/LICENSE.txt` & `luoguapi-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `luoguapi-0.1.2/src/luoguapi.py` & `luoguapi-0.1.3/src/luoguapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,8 +236,8 @@
             response = requests.get(
                 url=url, headers=self.session.getHeaders(url))
             if response.status_code == 404:
                 return [False, 'Problem Not Found']
             response = rmd(
                 response.text, 'JSON.parse(decodeURIComponent("', '"));')
             response = urlDecode(response)
-            return [True, response]
+            return [True, json.dumps(response)]
```

