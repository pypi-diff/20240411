# Comparing `tmp/domolibrary_extensions-0.0.8.tar.gz` & `tmp/domolibrary_extensions-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary_extensions-0.0.8.tar", last modified: Thu Feb 29 00:02:02 2024, max compression
+gzip compressed data, was "domolibrary_extensions-0.0.9.tar", last modified: Thu Feb 29 00:44:51 2024, max compression
```

## Comparing `domolibrary_extensions-0.0.8.tar` & `domolibrary_extensions-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:02:02.030045 domolibrary_extensions-0.0.8/
--rw-r--r--   0 root         (0) root         (0)    11337 2024-02-28 21:44:42.000000 domolibrary_extensions-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2024-02-28 21:44:42.000000 domolibrary_extensions-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1038 2024-02-29 00:02:02.030045 domolibrary_extensions-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      314 2024-02-28 21:44:42.000000 domolibrary_extensions-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:02:02.030045 domolibrary_extensions-0.0.8/domolibrary_extensions/
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-28 23:59:17.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31942 2024-02-28 23:59:17.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/_modidx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:02:02.030045 domolibrary_extensions-0.0.8/domolibrary_extensions/asana/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 23:59:17.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/asana/__init__.py
--rw-r--r--   0 root         (0) root         (0)      812 2024-02-28 23:59:16.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/asana/auth.py
--rw-r--r--   0 root         (0) root         (0)     3237 2024-02-28 23:59:16.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/asana/project.py
--rw-r--r--   0 root         (0) root         (0)     8337 2024-02-28 23:59:16.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/asana/task.py
--rw-r--r--   0 root         (0) root         (0)     1314 2024-02-28 23:59:16.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/asana/user.py
--rw-r--r--   0 root         (0) root         (0)     7990 2024-02-28 23:59:16.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:02:02.030045 domolibrary_extensions-0.0.8/domolibrary_extensions/google/
--rw-r--r--   0 root         (0) root         (0)     5059 2024-02-28 23:59:16.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/google/GDoc_File.py
--rw-r--r--   0 root         (0) root         (0)     2827 2024-02-28 23:59:16.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/google/GDoc_Files.py
--rw-r--r--   0 root         (0) root         (0)     1779 2024-02-28 23:59:16.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/google/GSearch.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 23:59:17.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5753 2024-02-28 23:59:16.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/google/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:02:02.030045 domolibrary_extensions-0.0.8/domolibrary_extensions/integrations/
--rw-r--r--   0 root         (0) root         (0)     3475 2024-02-28 23:59:16.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/integrations/ProxyCurl.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 23:59:17.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:02:02.030045 domolibrary_extensions-0.0.8/domolibrary_extensions/jira/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 23:59:17.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/jira/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1624 2024-02-28 23:59:16.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/jira/auth.py
--rw-r--r--   0 root         (0) root         (0)     1138 2024-02-28 23:59:16.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/jira/routes.py
--rw-r--r--   0 root         (0) root         (0)     8859 2024-02-28 23:59:17.000000 domolibrary_extensions-0.0.8/domolibrary_extensions/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:02:02.030045 domolibrary_extensions-0.0.8/domolibrary_extensions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1038 2024-02-29 00:02:02.000000 domolibrary_extensions-0.0.8/domolibrary_extensions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1119 2024-02-29 00:02:02.000000 domolibrary_extensions-0.0.8/domolibrary_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-29 00:02:02.000000 domolibrary_extensions-0.0.8/domolibrary_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2024-02-29 00:02:02.000000 domolibrary_extensions-0.0.8/domolibrary_extensions.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 22:02:13.000000 domolibrary_extensions-0.0.8/domolibrary_extensions.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      213 2024-02-29 00:02:02.000000 domolibrary_extensions-0.0.8/domolibrary_extensions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-02-29 00:02:02.000000 domolibrary_extensions-0.0.8/domolibrary_extensions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1186 2024-02-29 00:01:56.000000 domolibrary_extensions-0.0.8/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-29 00:02:02.030045 domolibrary_extensions-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2669 2024-02-28 21:44:43.000000 domolibrary_extensions-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:44:51.109798 domolibrary_extensions-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)    11337 2024-02-28 21:44:42.000000 domolibrary_extensions-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2024-02-28 21:44:42.000000 domolibrary_extensions-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1038 2024-02-29 00:44:51.109798 domolibrary_extensions-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      314 2024-02-28 21:44:42.000000 domolibrary_extensions-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:44:51.109798 domolibrary_extensions-0.0.9/domolibrary_extensions/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32456 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/_modidx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:44:51.109798 domolibrary_extensions-0.0.9/domolibrary_extensions/asana/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/asana/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      812 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/asana/auth.py
+-rw-r--r--   0 root         (0) root         (0)     3237 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/asana/project.py
+-rw-r--r--   0 root         (0) root         (0)     8337 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/asana/task.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/asana/user.py
+-rw-r--r--   0 root         (0) root         (0)     9899 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:44:51.109798 domolibrary_extensions-0.0.9/domolibrary_extensions/google/
+-rw-r--r--   0 root         (0) root         (0)     5059 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/google/GDoc_File.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/google/GDoc_Files.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/google/GSearch.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5753 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/google/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:44:51.109798 domolibrary_extensions-0.0.9/domolibrary_extensions/integrations/
+-rw-r--r--   0 root         (0) root         (0)     3475 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/integrations/ProxyCurl.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:44:51.109798 domolibrary_extensions-0.0.9/domolibrary_extensions/jira/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/jira/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/jira/auth.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/jira/routes.py
+-rw-r--r--   0 root         (0) root         (0)    11833 2024-02-29 00:43:36.000000 domolibrary_extensions-0.0.9/domolibrary_extensions/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 00:44:51.109798 domolibrary_extensions-0.0.9/domolibrary_extensions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1038 2024-02-29 00:44:51.000000 domolibrary_extensions-0.0.9/domolibrary_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-02-29 00:44:51.000000 domolibrary_extensions-0.0.9/domolibrary_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-29 00:44:51.000000 domolibrary_extensions-0.0.9/domolibrary_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2024-02-29 00:44:51.000000 domolibrary_extensions-0.0.9/domolibrary_extensions.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 22:02:13.000000 domolibrary_extensions-0.0.9/domolibrary_extensions.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      213 2024-02-29 00:44:51.000000 domolibrary_extensions-0.0.9/domolibrary_extensions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-02-29 00:44:51.000000 domolibrary_extensions-0.0.9/domolibrary_extensions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-02-29 00:43:31.000000 domolibrary_extensions-0.0.9/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-29 00:44:51.109798 domolibrary_extensions-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2669 2024-02-28 21:44:43.000000 domolibrary_extensions-0.0.9/setup.py
```

### Comparing `domolibrary_extensions-0.0.8/LICENSE` & `domolibrary_extensions-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary_extensions-0.0.8/PKG-INFO` & `domolibrary_extensions-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary_extensions
-Version: 0.0.8
+Version: 0.0.9
 Summary: integrate google docs with github
 Home-page: https://github.com/jaewilson07/domolibrary_extensions
 Author: jaewilson07
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/_modidx.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,16 @@
                                                                                                               'domolibrary_extensions/client.py'),
                                                'domolibrary_extensions.client._generate_cache_name': ( 'client/client.html#_generate_cache_name',
                                                                                                        'domolibrary_extensions/client.py'),
                                                'domolibrary_extensions.client.get_cache': ( 'client/client.html#get_cache',
                                                                                             'domolibrary_extensions/client.py'),
                                                'domolibrary_extensions.client.get_data': ( 'client/client.html#get_data',
                                                                                            'domolibrary_extensions/client.py'),
+                                               'domolibrary_extensions.client.get_data_stream': ( 'client/client.html#get_data_stream',
+                                                                                                  'domolibrary_extensions/client.py'),
                                                'domolibrary_extensions.client.looper': ( 'client/client.html#looper',
                                                                                          'domolibrary_extensions/client.py'),
                                                'domolibrary_extensions.client.prepare_fetch': ( 'client/client.html#prepare_fetch',
                                                                                                 'domolibrary_extensions/client.py'),
                                                'domolibrary_extensions.client.update_cache': ( 'client/client.html#update_cache',
                                                                                                'domolibrary_extensions/client.py')},
             'domolibrary_extensions.google.GDoc_File': { 'domolibrary_extensions.google.GDoc_File.GDocFile_DownloadError': ( 'google/gdoc_file.html#gdocfile_downloaderror',
@@ -195,14 +197,16 @@
                                                                                                           'domolibrary_extensions/utils.py'),
                                               'domolibrary_extensions.utils.detect_encoding': ( 'utils.html#detect_encoding',
                                                                                                 'domolibrary_extensions/utils.py'),
                                               'domolibrary_extensions.utils.download_pptx': ( 'utils.html#download_pptx',
                                                                                               'domolibrary_extensions/utils.py'),
                                               'domolibrary_extensions.utils.download_zip': ( 'utils.html#download_zip',
                                                                                              'domolibrary_extensions/utils.py'),
+                                              'domolibrary_extensions.utils.export_env': ( 'utils.html#export_env',
+                                                                                           'domolibrary_extensions/utils.py'),
                                               'domolibrary_extensions.utils.get_all_files_and_folders': ( 'utils.html#get_all_files_and_folders',
                                                                                                           'domolibrary_extensions/utils.py'),
                                               'domolibrary_extensions.utils.md': ('utils.html#md', 'domolibrary_extensions/utils.py'),
                                               'domolibrary_extensions.utils.read_html_file': ( 'utils.html#read_html_file',
                                                                                                'domolibrary_extensions/utils.py'),
                                               'domolibrary_extensions.utils.remove_query_params_from_url': ( 'utils.html#remove_query_params_from_url',
                                                                                                              'domolibrary_extensions/utils.py'),
```

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/asana/auth.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/asana/auth.py`

 * *Files identical despite different names*

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/asana/project.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/asana/project.py`

 * *Files identical despite different names*

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/asana/task.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/asana/task.py`

 * *Files identical despite different names*

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/asana/user.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/asana/user.py`

 * *Files identical despite different names*

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/client.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 from urllib.parse import urlparse
 
 import httpx
 import json
 
 from pprint import pprint
-
 import domolibrary_extensions.utils as ut
 
 # %% auto 0
-__all__ = ['Auth', 'ResponseGetData', 'get_cache', 'update_cache', 'get_data', 'looper', 'BaseError_Validation', 'BaseError']
+__all__ = ['Auth', 'ResponseGetData', 'get_cache', 'update_cache', 'get_data', 'get_data_stream', 'looper',
+           'BaseError_Validation', 'BaseError']
 
 # %% ../nbs/client/client.ipynb 6
 @dataclass
 class Auth(ABC):
     """Base class for authentication"""
 
     @abstractmethod
@@ -206,14 +206,86 @@
     rgd = ResponseGetData._from_httpx(res, auth=auth)
 
     if rgd.is_success:
         update_cache(cache_path=cache_path, data=rgd.response, debug_prn=debug_prn)
 
     return rgd
 
+# %% ../nbs/client/client.ipynb 22
+async def get_data_stream(
+    url: str,
+    cache_path: str = None,
+    is_ignore_cache: bool = False,
+    headers: dict = None,
+    params: dict = None,
+    body=None,
+    auth: Auth = None,
+    parent_class: str = None,
+    debug_api: bool = False,
+    debug_prn: bool = False,
+    client: httpx.AsyncClient = None,
+    is_verify_ssl: bool = False,
+) -> ResponseGetData:
+    """wrapper for httpx Request library, always use with jiralibrary class"""
+
+    cache_path = cache_path or _generate_cache_name(url)
+
+    if not is_ignore_cache and cache_path:
+        json_data = get_cache(cache_path=cache_path, debug_prn=debug_prn)
+
+        if json_data:
+            return ResponseGetData._from_cache(data=json_data, auth=auth)
+
+    is_close_session = False if client else True
+
+    client = client or httpx.AsyncClient(verify=is_verify_ssl)
+
+    headers, url, params, body = prepare_fetch(
+        url=url,
+        params=params,
+        auth=auth,
+        headers=headers,
+        body=body,
+    )
+
+    if debug_api:
+        pprint(
+            {
+                "headers": headers,
+                "url": url,
+                "params": params,
+                "body": body,
+                "cache_file_path": cache_path,
+                "debug_api": debug_api,
+                "parent_class": parent_class,
+            }
+        )
+
+    content = bytearray()
+
+    async with client.stream(
+        method="GET",
+        url=url,
+        headers=headers,
+        params=params,
+        follow_redirects=True,
+    ) as res:
+        async for chunk in res.aiter_bytes():
+            content += chunk
+
+    if is_close_session:
+        await client.aclose()
+
+    rgd = ResponseGetData._from_httpx(res, auth=auth, content=content)
+
+    if rgd.is_success:
+        update_cache(cache_path=cache_path, data=rgd.response, debug_prn=debug_prn)
+
+    return rgd
+
 # %% ../nbs/client/client.ipynb 24
 async def looper(
     url,
     client: httpx.AsyncClient,
     auth: Auth,
     arr_fn,
     params: dict = None,
@@ -267,15 +339,15 @@
 
         final_array += new_array
         offset += limit
 
     res.response = final_array
 
     if res.is_success:
-        update_cache(cache_path=cache_path, json_data=res.response, debug_prn=debug_prn)
+        update_cache(cache_path=cache_path, data=res.response, debug_prn=debug_prn)
 
     return res
 
 # %% ../nbs/client/client.ipynb 25
 class BaseError_Validation(Exception):
     def __init__(self, message):
         super().__init__(message)
```

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/google/GDoc_File.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/google/GDoc_File.py`

 * *Files identical despite different names*

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/google/GDoc_Files.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/google/GDoc_Files.py`

 * *Files identical despite different names*

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/google/GSearch.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/google/GSearch.py`

 * *Files identical despite different names*

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/google/auth.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/google/auth.py`

 * *Files identical despite different names*

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/integrations/ProxyCurl.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/integrations/ProxyCurl.py`

 * *Files identical despite different names*

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/jira/auth.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/jira/auth.py`

 * *Files identical despite different names*

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/jira/routes.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/jira/routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions/utils.py` & `domolibrary_extensions-0.0.9/domolibrary_extensions/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/utils.ipynb.
 
 # %% auto 0
-__all__ = ['rename_filepath_to_match_datatype', 'detect_encoding', 'read_html_file', 'remove_query_params_from_url', 'update_env',
-           'upsert_folder', 'get_all_files_and_folders', 'ImageBlockConverter', 'md', 'convert_html_to_markdown',
-           'download_zip', 'download_pptx', 'convert_str_to_snake_case', 'convert_str_remove_accents',
-           'convert_str_keep_alphanumeric', 'convert_str_file_name', 'convert_str_to_date']
+__all__ = ['default_keys', 'export_env', 'rename_filepath_to_match_datatype', 'detect_encoding', 'read_html_file',
+           'remove_query_params_from_url', 'update_env', 'upsert_folder', 'get_all_files_and_folders',
+           'ImageBlockConverter', 'md', 'convert_html_to_markdown', 'download_zip', 'download_pptx',
+           'convert_str_to_snake_case', 'convert_str_remove_accents', 'convert_str_keep_alphanumeric',
+           'convert_str_file_name', 'convert_str_to_date']
 
 # %% ../nbs/utils.ipynb 3
 import os
 from typing import List, Tuple, Union
 
 import re
+import pathlib
 import unicodedata
 import json
 import chardet
 from urllib.parse import urljoin, urlparse
 from bs4 import BeautifulSoup
 from markdownify import MarkdownConverter
 
-import pathlib
+import datetime as dt
 
 
 from PIL import Image
 
 import pptx2md
 
 import zipfile
@@ -31,14 +33,146 @@
 
 import datetime as dt
 from dateutil.parser import parse as dtu_parse
 
 from dotenv import set_key, load_dotenv
 
 # %% ../nbs/utils.ipynb 6
+default_keys = [
+    "DOCKER_BUILDKIT",
+    "ENABLE_DYNAMIC_INSTALL",
+    "LESSOPEN",
+    "GIT_COMMITTER_NAME",
+    "PYTHONIOENCODING",
+    "GITHUB_CODESPACE_TOKEN",
+    "USER",
+    "RVM_PATH",
+    "NVS_ROOT",
+    "HOSTNAME",
+    "DOTNET_USE_POLLING_FILE_WATCHER",
+    "CONDA_SCRIPT",
+    "PIPX_HOME",
+    "SHLVL",
+    "GITHUB_CODESPACES_PORT_FORWARDING_DOMAIN",
+    "GCP_KEY",
+    "HUGO_ROOT",
+    "HOME",
+    "OLDPWD",
+    "ORYX_ENV_TYPE",
+    "NVM_BIN",
+    "CODESPACES",
+    "DOTNET_RUNNING_IN_CONTAINER",
+    "NVM_SYMLINK_CURRENT",
+    "DYNAMIC_INSTALL_ROOT_DIR",
+    "PIPX_BIN_DIR",
+    "NVM_INC",
+    "rvm_stored_umask",
+    "ORYX_DIR",
+    "GRADLE_HOME",
+    "rvm_user_install_flag",
+    "MAVEN_HOME",
+    "GOROOT",
+    "NODE_ROOT",
+    "GITHUB_GRAPHQL_URL",
+    "GITHUB_USER",
+    "NVM_DIR",
+    "PYTHON_PATH",
+    "DOTNET_SKIP_FIRST_TIME_EXPERIENCE",
+    "ContainerVersion",
+    "NVS_HOME",
+    "GITHUB_API_URL",
+    "rvm_bin_path",
+    "SDKMAN_CANDIDATES_API",
+    "_",
+    "RUBY_VERSION",
+    "PROMPT_DIRTRIM",
+    "IRBRC",
+    "CLOUDENV_ENVIRONMENT_ID",
+    "DOTNET_ROOT",
+    "NVS_DIR",
+    "PHP_ROOT",
+    "PATH",
+    "JAVA_ROOT",
+    "VSCODE_AGENT_FOLDER",
+    "SDKMAN_CANDIDATES_DIR",
+    "HUGO_DIR",
+    "NPM_GLOBAL",
+    "SHELL_LOGGED_IN",
+    "MY_RUBY_HOME",
+    "LANG",
+    "SDKMAN_DIR",
+    "RUBY_ROOT",
+    "LS_COLORS",
+    "SDKMAN_PLATFORM",
+    "GITHUB_REPOSITORY",
+    "SHELL",
+    "GOPATH",
+    "rvm_prefix",
+    "rvm_loaded_flag",
+    "GEM_HOME",
+    "ORYX_PREFER_USER_INSTALLED_SDKS",
+    "LESSCLOSE",
+    "ORYX_SDK_STORAGE_BASE_URL",
+    "CONDA_DIR",
+    "rvm_version",
+    "DEBIAN_FLAVOR",
+    "GIT_COMMITTER_EMAIL",
+    "GEM_PATH",
+    "JAVA_HOME",
+    "NVS_USE_XZ",
+    "INTERNAL_VSCS_TARGET_URL",
+    "PWD",
+    "NVM_CD_FLAGS",
+    "GITHUB_SERVER_URL",
+    "PHP_PATH",
+    "PYTHON_ROOT",
+    "RAILS_DEVELOPMENT_HOSTS",
+    "NVS_OS",
+    "CODESPACE_NAME",
+    "RUBY_HOME",
+    "MAVEN_ROOT",
+    "rvm_path",
+    "NUGET_XMLDOC_MODE",
+    "VSCODE_HANDLES_SIGPIPE",
+    "VSCODE_AMD_ENTRYPOINT",
+    "VSCODE_HANDLES_UNCAUGHT_ERRORS",
+    "VSCODE_NLS_CONFIG",
+    "BROWSER",
+    "VSCODE_CWD",
+    "ELECTRON_RUN_AS_NODE",
+    "VSCODE_IPC_HOOK_CLI",
+    "VSCODE_L10N_BUNDLE_LOCATION",
+    "DEBUG",
+    "PYDEVD_IPYTHON_COMPATIBLE_DEBUGGING",
+    "PYTHONUNBUFFERED",
+    "PYDEVD_USE_FRAME_EVAL",
+    "TERM",
+    "CLICOLOR",
+    "FORCE_COLOR",
+    "CLICOLOR_FORCE",
+    "PAGER",
+    "GIT_PAGER",
+    "MPLBACKEND",
+]
+
+
+def export_env(default_keys, output_file_path):
+    keep_keys = [key for key in os.environ.keys() if key not in default_keys]
+
+    with open(output_file_path, "w+") as f:
+        f.writelines(
+            [
+                f"{key} = '{value}'\n"
+                for key, value in os.environ.items()
+                if key in keep_keys
+            ]
+        )
+        f.write(f"_OUTPUT_DATE = '{dt.datetime.now().strftime('%Y-%m-%d %H:%M')}'")
+
+# %% ../nbs/utils.ipynb 9
 def rename_filepath_to_match_datatype(data, file_path):
 
     is_path_ext = os.path.splitext(file_path)[-1].lower()
 
     old_suffix = pathlib.Path(file_path).suffix if is_path_ext else None
 
     new_suffix = ""
@@ -53,49 +187,49 @@
     file_path = file_path + new_suffix
 
     if old_suffix:
         file_path = file_path.replace(old_suffix, "")
 
     return file_path
 
-# %% ../nbs/utils.ipynb 8
+# %% ../nbs/utils.ipynb 11
 def detect_encoding(file_path, debug_prn: bool = False):
     detector = chardet.universaldetector.UniversalDetector()
     with open(file_path, "rb") as f:
         for line in f:
             detector.feed(line)
             if detector.done:
                 break
     detector.close()
 
     encoding = detector.result
 
     return encoding
 
-# %% ../nbs/utils.ipynb 10
+# %% ../nbs/utils.ipynb 13
 def read_html_file(
     file_path, is_convert_to_soup: bool = True
 ) -> Union[str, BeautifulSoup]:
     if not os.path.exists(file_path):
         raise FileNotFoundError(file_path)
 
     page_encoding = detect_encoding(file_path)
 
     with open(file_path, encoding=page_encoding["encoding"]) as fp:
         if is_convert_to_soup:
             return BeautifulSoup(fp, "lxml")
 
         return fp.read()
 
-# %% ../nbs/utils.ipynb 12
+# %% ../nbs/utils.ipynb 15
 def remove_query_params_from_url(url):
     u = urlparse(url)
     return urljoin(url, urlparse(url).path)
 
-# %% ../nbs/utils.ipynb 14
+# %% ../nbs/utils.ipynb 17
 def update_env(env_path: str, key: str, value: str, debug_prn: bool = False) -> dict:
     """
     updates a .env file with a key value pair
     then reloads the env_file
     """
 
     if not os.path.exists(env_path):
@@ -125,30 +259,30 @@
 
     set_key(env_path, "env_last_modified", f"updated - {dt.date.today()}")
 
     load_dotenv(env_path, override=True)
 
     return {key: os.getenv(key)}
 
-# %% ../nbs/utils.ipynb 15
+# %% ../nbs/utils.ipynb 18
 def upsert_folder(folder_path: str, debug_prn: bool = False):
     folder_path = os.path.dirname(folder_path)
 
     if debug_prn:
         print(
             {
                 "upsert_folder": os.path.abspath(folder_path),
                 "is_exist": os.path.exists(folder_path),
             }
         )
 
     if not os.path.exists(folder_path):
         os.makedirs(folder_path)
 
-# %% ../nbs/utils.ipynb 16
+# %% ../nbs/utils.ipynb 19
 def get_all_files_and_folders(
     directory, file_type=None  # to only retrieve a specific file type
 ) -> Union[Tuple, List]:
     """walk a directory and retrieve a list of files and a list of directory
     returns Tuple of file_ls , dir_ls OR file_ls if file_type supplied
     """
     if not os.path.exists(directory):
@@ -170,15 +304,15 @@
             dir_ls.append(os.path.join(root, name))
 
     if file_type:
         return file_ls
 
     return file_ls, dir_ls
 
-# %% ../nbs/utils.ipynb 19
+# %% ../nbs/utils.ipynb 22
 class ImageBlockConverter(MarkdownConverter):
     """
     Create a custom MarkdownConverter that adds two newlines after an image
     """
 
     def convert_img(self, el, text, convert_as_inline, is_resize: bool = True):
         """
@@ -211,15 +345,15 @@
         return super().convert_img(el, text, convert_as_inline)
 
 
 def md(html, **options):
     """Create shorthand method for handling conversion"""
     return ImageBlockConverter(**options).convert(html)
 
-# %% ../nbs/utils.ipynb 20
+# %% ../nbs/utils.ipynb 23
 def convert_html_to_markdown(file_path):
     """converts html file to markdown in place"""
 
     with open(file_path, encoding="utf-8") as f:
         html = f.read()
 
     markdown_content = md(
@@ -232,15 +366,15 @@
     md_path = file_path.replace(".html", ".md")
 
     with open(md_path, "w+", encoding="utf-8") as f:
         f.write(markdown_content)
 
     return
 
-# %% ../nbs/utils.ipynb 21
+# %% ../nbs/utils.ipynb 24
 def download_zip(zip_bytes_content, output_folder, is_convert_to_markdown: bool = True):
     """save bytes content to a zip file then convert html to markdown"""
 
     zip = zipfile.ZipFile(io.BytesIO(zip_bytes_content), "r")
     zip.extractall(output_folder)
 
     file_ls = os.listdir(output_folder)
@@ -252,15 +386,15 @@
             os.replace(os.path.join(output_folder, file_name), output_index)
 
             if is_convert_to_markdown:
                 convert_html_to_markdown(os.path.join(output_folder, "index.html"))
 
     return f"successfully downloaded zip to {output_folder}"
 
-# %% ../nbs/utils.ipynb 24
+# %% ../nbs/utils.ipynb 27
 def download_pptx(
     pptx_bytes_content, output_folder, is_convert_to_markdown: bool = True
 ):
     """save bytes content to a pptx file then converts to markdown"""
 
     upsert_folder(output_folder)
 
@@ -275,39 +409,39 @@
             output_ppt_index,
             output=os.path.join(output_folder, "index.md"),
             image_dir=os.path.join(output_folder, "images"),
         )
 
     return f"successfully downloaded content to {output_folder}"
 
-# %% ../nbs/utils.ipynb 28
+# %% ../nbs/utils.ipynb 31
 def convert_str_to_snake_case(text_str):
     """converts 'snake_case_str' to 'snakeCaseStr'"""
 
     return text_str.replace(" ", "_").lower()
 
-# %% ../nbs/utils.ipynb 29
+# %% ../nbs/utils.ipynb 32
 def convert_str_remove_accents(text_str: str) -> str:
     return "".join(
         c
         for c in unicodedata.normalize("NFD", text_str)
         if unicodedata.category(c) != "Mn"
     )
 
-# %% ../nbs/utils.ipynb 31
+# %% ../nbs/utils.ipynb 34
 def convert_str_keep_alphanumeric(text_str) -> str:
     pattern = "[^0-9a-zA-Z_\s]+"
 
     return re.sub(pattern, "", text_str)
 
-# %% ../nbs/utils.ipynb 32
+# %% ../nbs/utils.ipynb 35
 def convert_str_file_name(text_str: str) -> str:
     """convert strings to clean file name or url"""
 
     return convert_str_keep_alphanumeric(
         convert_str_to_snake_case(convert_str_remove_accents(text_str))
     )
 
-# %% ../nbs/utils.ipynb 35
+# %% ../nbs/utils.ipynb 38
 def convert_str_to_date(datefield: str) -> dt.datetime:
     """converts string date to datetime object"""
     return dtu_parse(datefield) if datefield else None
```

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions.egg-info/PKG-INFO` & `domolibrary_extensions-0.0.9/domolibrary_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary-extensions
-Version: 0.0.8
+Version: 0.0.9
 Summary: integrate google docs with github
 Home-page: https://github.com/jaewilson07/domolibrary_extensions
 Author: jaewilson07
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary_extensions-0.0.8/domolibrary_extensions.egg-info/SOURCES.txt` & `domolibrary_extensions-0.0.9/domolibrary_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domolibrary_extensions-0.0.8/settings.ini` & `domolibrary_extensions-0.0.9/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domolibrary_extensions
 lib_name = domolibrary_extensions
-version = 0.0.8
+version = 0.0.9
 min_python = 3.9
 license = apache2
 black_formatting = True
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary_extensions
```

### Comparing `domolibrary_extensions-0.0.8/setup.py` & `domolibrary_extensions-0.0.9/setup.py`

 * *Files identical despite different names*

