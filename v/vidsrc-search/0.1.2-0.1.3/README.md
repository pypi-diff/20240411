# Comparing `tmp/vidsrc-search-0.1.2.tar.gz` & `tmp/vidsrc-search-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidsrc-search-0.1.2.tar", last modified: Tue Feb 13 22:03:35 2024, max compression
+gzip compressed data, was "vidsrc-search-0.1.3.tar", last modified: Wed Apr 10 16:53:09 2024, max compression
```

## Comparing `vidsrc-search-0.1.2.tar` & `vidsrc-search-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-02-13 22:03:35.648473 vidsrc-search-0.1.2/
--rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-02-07 23:52:12.000000 vidsrc-search-0.1.2/LICENSE
--rw-r--r--   0 Dev        (502) staff       (20)     1439 2024-02-13 22:03:35.648251 vidsrc-search-0.1.2/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)      668 2024-02-12 01:10:39.000000 vidsrc-search-0.1.2/README.md
--rw-r--r--   0 Dev        (502) staff       (20)        4 2024-02-13 22:03:19.000000 vidsrc-search-0.1.2/a.txt
--rw-r--r--   0 Dev        (502) staff       (20)      883 2024-02-13 22:03:25.000000 vidsrc-search-0.1.2/pyproject.toml
--rw-r--r--   0 Dev        (502) staff       (20)       38 2024-02-13 22:03:35.648515 vidsrc-search-0.1.2/setup.cfg
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-02-13 22:03:35.644172 vidsrc-search-0.1.2/src/
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-02-13 22:03:35.647101 vidsrc-search-0.1.2/src/vidsrc_search/
--rw-r--r--   0 Dev        (502) staff       (20)     1235 2024-02-13 21:51:50.000000 vidsrc-search-0.1.2/src/vidsrc_search/__main__.py
--rw-r--r--   0 Dev        (502) staff       (20)     3154 2024-02-12 19:56:03.000000 vidsrc-search-0.1.2/src/vidsrc_search/argparsing.py
--rw-r--r--   0 Dev        (502) staff       (20)     2752 2024-02-13 01:09:37.000000 vidsrc-search-0.1.2/src/vidsrc_search/download.py
--rw-r--r--   0 Dev        (502) staff       (20)     1234 2024-02-12 00:30:50.000000 vidsrc-search-0.1.2/src/vidsrc_search/json_utils.py
--rw-r--r--   0 Dev        (502) staff       (20)     4134 2024-02-13 21:59:23.000000 vidsrc-search-0.1.2/src/vidsrc_search/search.py
--rw-r--r--   0 Dev        (502) staff       (20)      885 2024-02-12 00:41:51.000000 vidsrc-search-0.1.2/src/vidsrc_search/uninstall.py
--rw-r--r--   0 Dev        (502) staff       (20)     4907 2024-02-13 21:13:42.000000 vidsrc-search-0.1.2/src/vidsrc_search/utils.py
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-02-13 22:03:35.648046 vidsrc-search-0.1.2/src/vidsrc_search.egg-info/
--rw-r--r--   0 Dev        (502) staff       (20)     1439 2024-02-13 22:03:35.000000 vidsrc-search-0.1.2/src/vidsrc_search.egg-info/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)      496 2024-02-13 22:03:35.000000 vidsrc-search-0.1.2/src/vidsrc_search.egg-info/SOURCES.txt
--rw-r--r--   0 Dev        (502) staff       (20)        1 2024-02-13 22:03:35.000000 vidsrc-search-0.1.2/src/vidsrc_search.egg-info/dependency_links.txt
--rw-r--r--   0 Dev        (502) staff       (20)       62 2024-02-13 22:03:35.000000 vidsrc-search-0.1.2/src/vidsrc_search.egg-info/entry_points.txt
--rw-r--r--   0 Dev        (502) staff       (20)       44 2024-02-13 22:03:35.000000 vidsrc-search-0.1.2/src/vidsrc_search.egg-info/requires.txt
--rw-r--r--   0 Dev        (502) staff       (20)       14 2024-02-13 22:03:35.000000 vidsrc-search-0.1.2/src/vidsrc_search.egg-info/top_level.txt
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-10 16:53:09.067613 vidsrc-search-0.1.3/
+-rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-04-10 15:45:52.000000 vidsrc-search-0.1.3/LICENSE
+-rw-r--r--   0 Dev        (502) staff       (20)       12 2024-04-10 16:52:29.000000 vidsrc-search-0.1.3/LICENSE.txt
+-rw-r--r--   0 Dev        (502) staff       (20)     1473 2024-04-10 16:53:09.067318 vidsrc-search-0.1.3/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)      668 2024-04-10 15:45:52.000000 vidsrc-search-0.1.3/README.md
+-rw-r--r--   0 Dev        (502) staff       (20)      889 2024-04-10 16:52:38.000000 vidsrc-search-0.1.3/pyproject.toml
+-rw-r--r--   0 Dev        (502) staff       (20)       38 2024-04-10 16:53:09.067683 vidsrc-search-0.1.3/setup.cfg
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-10 16:53:09.061916 vidsrc-search-0.1.3/src/
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-10 16:53:09.065415 vidsrc-search-0.1.3/src/vidsrc_search/
+-rw-r--r--   0 Dev        (502) staff       (20)     1240 2024-04-10 15:48:15.000000 vidsrc-search-0.1.3/src/vidsrc_search/__main__.py
+-rw-r--r--   0 Dev        (502) staff       (20)     3154 2024-04-10 16:31:20.000000 vidsrc-search-0.1.3/src/vidsrc_search/argparsing.py
+-rw-r--r--   0 Dev        (502) staff       (20)     2752 2024-04-10 15:49:47.000000 vidsrc-search-0.1.3/src/vidsrc_search/download.py
+-rw-r--r--   0 Dev        (502) staff       (20)     1234 2024-04-10 15:45:52.000000 vidsrc-search-0.1.3/src/vidsrc_search/json_utils.py
+-rw-r--r--   0 Dev        (502) staff       (20)     4158 2024-04-10 15:51:08.000000 vidsrc-search-0.1.3/src/vidsrc_search/search.py
+-rw-r--r--   0 Dev        (502) staff       (20)      885 2024-04-10 15:45:52.000000 vidsrc-search-0.1.3/src/vidsrc_search/uninstall.py
+-rw-r--r--   0 Dev        (502) staff       (20)     6195 2024-04-10 16:47:31.000000 vidsrc-search-0.1.3/src/vidsrc_search/utils.py
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-10 16:53:09.066998 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/
+-rw-r--r--   0 Dev        (502) staff       (20)     1473 2024-04-10 16:53:09.000000 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)      502 2024-04-10 16:53:09.000000 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/SOURCES.txt
+-rw-r--r--   0 Dev        (502) staff       (20)        1 2024-04-10 16:53:09.000000 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/dependency_links.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       62 2024-04-10 16:53:09.000000 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/entry_points.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       44 2024-04-10 16:53:09.000000 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/requires.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       14 2024-04-10 16:53:09.000000 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/top_level.txt
```

### Comparing `vidsrc-search-0.1.2/LICENSE` & `vidsrc-search-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vidsrc-search-0.1.2/PKG-INFO` & `vidsrc-search-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: vidsrc-search
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pirate movie watcher written in Python
-License: MIT
+License: MIT License
         
 Project-URL: Homepage, https://github.com/SomedudeX/vidsrc-search
 Keywords: movie,video,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE.txt
 Requires-Dist: aiohttp
 Requires-Dist: thefuzz
 Requires-Dist: tabulate
 Requires-Dist: requests
 Requires-Dist: pywebview
 
 ## Overview
```

### Comparing `vidsrc-search-0.1.2/README.md` & `vidsrc-search-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vidsrc-search-0.1.2/pyproject.toml` & `vidsrc-search-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vidsrc-search"
-version = "0.1.2"
+version = "0.1.3"
 description = "A pirate movie watcher written in Python"
 readme = "README.md"
-license = { file = "a.txt" }
+license = { file = "LICENSE.txt" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python",
     "Topic :: Multimedia",
```

### Comparing `vidsrc-search-0.1.2/src/vidsrc_search/__main__.py` & `vidsrc-search-0.1.3/src/vidsrc_search/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import os
 import sys
 import warnings
 
-warnings.filterwarnings("ignore")
-
 from . import utils
 from . import argparsing
 
 
 def main():
     try:
         utils.bootstrap()
         argparsing.parse_args()
-    except KeyboardInterrupt:
-        print()
-        print(" [Warning] Vidsrc-search received KeyboardInterrupt")
+    except SystemExit:
+        pass
+    except UserWarning:
+        print(" [Warning] Vidsrc-search received UserWarning")
         print(" [Warning] Program force quitting with os._exit()")
         utils.cleanup()
         os._exit(0)
-    except UserWarning:
-        print(" [Warning] Vidsrc-search received UserWarning")
+    except KeyboardInterrupt:
+        print()
+        print(" [Warning] Vidsrc-search received KeyboardInterrupt")
         print(" [Warning] Program force quitting with os._exit()")
         utils.cleanup()
         os._exit(0)
-    except Exception as e:
+    except BaseException as e:
         print()
         print(f" [Fatal] An unknown error was encountered during the execution of vidsrc-search")
         print(f" [Fatal] Error message from program: {e}")
         utils.cleanup()
         print()
         print(f" [Info] Note: ")
         print(f" [Info] This might be due to a temporary error in the program")
```

### Comparing `vidsrc-search-0.1.2/src/vidsrc_search/argparsing.py` & `vidsrc-search-0.1.3/src/vidsrc_search/argparsing.py`

 * *Files identical despite different names*

### Comparing `vidsrc-search-0.1.2/src/vidsrc_search/download.py` & `vidsrc-search-0.1.3/src/vidsrc_search/download.py`

 * *Files identical despite different names*

### Comparing `vidsrc-search-0.1.2/src/vidsrc_search/json_utils.py` & `vidsrc-search-0.1.3/src/vidsrc_search/json_utils.py`

 * *Files identical despite different names*

### Comparing `vidsrc-search-0.1.2/src/vidsrc_search/search.py` & `vidsrc-search-0.1.3/src/vidsrc_search/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,28 @@
     with open(lib_path, "r") as f: 
         library = f.read()
     library = json.loads(library) 
 
     for entry in library: 
         if similarity(entry["title"], search_query) >= 60:
             ret.append({
-            "Index": None,
-            "Title": entry["title"], 
-            "IMDB ID": entry["imdb_id"], 
-            "Type": entry["type"], 
-            "URL": entry["embed_url_imdb"], 
-            "Match": f"{similarity(entry['title'], search_query):.2f}%",
+                "Index": None,
+                "Title": entry["title"], 
+                "IMDB ID": entry["imdb_id"], 
+                "Type": entry["type"], 
+                "URL": entry["embed_url_imdb"], 
+                "Match": f"{similarity(entry['title'], search_query):.2f}%",
             })
 
-    if len(ret) == 0: return None
-    ret = sort_results(ret)
+    if len(ret) == 0: 
+        return None
 
+    ret = sort_results(ret)
     while len(ret) > 20: 
         del ret[len(ret) - 1]
-        
     index = 1
     for result in ret:
         result["Index"] = f"[{index}]"
         index += 1
     return ret
```

### Comparing `vidsrc-search-0.1.2/src/vidsrc_search/uninstall.py` & `vidsrc-search-0.1.3/src/vidsrc_search/uninstall.py`

 * *Files identical despite different names*

### Comparing `vidsrc-search-0.1.2/src/vidsrc_search/utils.py` & `vidsrc-search-0.1.3/src/vidsrc_search/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -89,43 +89,68 @@
         
 def asyncio_patch() -> None:
     if sys.platform in ["win32", "cygwin", "msys"]:
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
         
 
 def check_internet() -> None:
-    print()
     print(" [Info] Verifying internet connection")
     
     try: 
         print(" [Info] Testing connection by pinging google.com")
-        requests.get("https://google.com")
+        r = requests.get("https://google.com", allow_redirects = False)
+        r.raise_for_status()
+    except requests.exceptions.HTTPError:
+        print() 
+        print(f" [Fatal] An HTTP error was encountered")
+        print(f" [Fatal] This might be due to an issue with the external server")
+        print(f" [Fatal] Vidsrc-search terminating with exit code 127")
+        sys.exit(127)
     except requests.exceptions.SSLError:
         print() 
         print(f" [Fatal] Could not establish secure connection")
         print(f" [Fatal] You might be on a monitored network or using a VPN/Proxy")
         print(f" [Fatal] Vidsrc-search terminating with exit code 127")
         sys.exit(127)
     except requests.exceptions.ConnectionError:
         print()
         print(f" [Fatal] Could not establish internet connection")
         print(f" [Fatal] Make sure you are connected to the internet")
         print(f" [Fatal] Vidsrc-search terminating with exit code 127")
         sys.exit(127)
+    except requests.exceptions.RequestException as e:
+        print()
+        print(f" [Fatal] An unknown network error occured: {e}")
+        print(f" [Fatal] This could be due to an issue with the external server")
+        print(f" [Fatal] Vidsrc-search terminating with exit code 255")
+        sys.exit(255)
+
     try:
         print(" [Info] Testing connection by pinging vidsrc.to")
         requests.get("https://vidsrc.to", allow_redirects = False)
-    except ConnectionError:
+    except requests.exceptions.HTTPError:
+        print() 
+        print(f" [Fatal] An HTTP error was encountered while pinging vidsrc.to")
+        print(f" [Fatal] This might be due to an issue with the external server")
+        print(f" [Fatal] Vidsrc-search terminating with exit code 127")
+        sys.exit(127)
+    except requests.exceptions.ConnectionError:
         print()
         print(f" [Fatal] Could not reach vidsrc.to")
         print(f" [Fatal] This might be because of an issue with the")
         print(f"         external server, or it might be due to")
         print(f"         that the server is blocked in your region. ")
         print(f" [Fatal] Vidsrc-search terminating with exit code -1")
         sys.exit(127)
+    except requests.exceptions.RequestException as e:
+        print()
+        print(f" [Fatal] An unknown network error occured: {e}")
+        print(f" [Fatal] This could be due to an issue with the server")
+        print(f" [Fatal] Vidsrc-search terminating with exit code 255")
+        sys.exit(255)
     return
 
 
 def cleanup() -> None:
     print(" [Info] Performing program cleanup process")
     path_one = os.path.expanduser("~/.config/pymovie/movie_buffer")
     path_two = os.path.expanduser("~/.config/pymovie/tv_buffer")
```

### Comparing `vidsrc-search-0.1.2/src/vidsrc_search.egg-info/PKG-INFO` & `vidsrc-search-0.1.3/src/vidsrc_search.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: vidsrc-search
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pirate movie watcher written in Python
-License: MIT
+License: MIT License
         
 Project-URL: Homepage, https://github.com/SomedudeX/vidsrc-search
 Keywords: movie,video,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE.txt
 Requires-Dist: aiohttp
 Requires-Dist: thefuzz
 Requires-Dist: tabulate
 Requires-Dist: requests
 Requires-Dist: pywebview
 
 ## Overview
```

