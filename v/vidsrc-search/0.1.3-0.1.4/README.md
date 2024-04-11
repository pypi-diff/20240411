# Comparing `tmp/vidsrc-search-0.1.3.tar.gz` & `tmp/vidsrc-search-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidsrc-search-0.1.3.tar", last modified: Wed Apr 10 16:53:09 2024, max compression
+gzip compressed data, was "vidsrc-search-0.1.4.tar", last modified: Thu Apr 11 00:00:33 2024, max compression
```

## Comparing `vidsrc-search-0.1.3.tar` & `vidsrc-search-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-10 16:53:09.067613 vidsrc-search-0.1.3/
--rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-04-10 15:45:52.000000 vidsrc-search-0.1.3/LICENSE
--rw-r--r--   0 Dev        (502) staff       (20)       12 2024-04-10 16:52:29.000000 vidsrc-search-0.1.3/LICENSE.txt
--rw-r--r--   0 Dev        (502) staff       (20)     1473 2024-04-10 16:53:09.067318 vidsrc-search-0.1.3/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)      668 2024-04-10 15:45:52.000000 vidsrc-search-0.1.3/README.md
--rw-r--r--   0 Dev        (502) staff       (20)      889 2024-04-10 16:52:38.000000 vidsrc-search-0.1.3/pyproject.toml
--rw-r--r--   0 Dev        (502) staff       (20)       38 2024-04-10 16:53:09.067683 vidsrc-search-0.1.3/setup.cfg
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-10 16:53:09.061916 vidsrc-search-0.1.3/src/
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-10 16:53:09.065415 vidsrc-search-0.1.3/src/vidsrc_search/
--rw-r--r--   0 Dev        (502) staff       (20)     1240 2024-04-10 15:48:15.000000 vidsrc-search-0.1.3/src/vidsrc_search/__main__.py
--rw-r--r--   0 Dev        (502) staff       (20)     3154 2024-04-10 16:31:20.000000 vidsrc-search-0.1.3/src/vidsrc_search/argparsing.py
--rw-r--r--   0 Dev        (502) staff       (20)     2752 2024-04-10 15:49:47.000000 vidsrc-search-0.1.3/src/vidsrc_search/download.py
--rw-r--r--   0 Dev        (502) staff       (20)     1234 2024-04-10 15:45:52.000000 vidsrc-search-0.1.3/src/vidsrc_search/json_utils.py
--rw-r--r--   0 Dev        (502) staff       (20)     4158 2024-04-10 15:51:08.000000 vidsrc-search-0.1.3/src/vidsrc_search/search.py
--rw-r--r--   0 Dev        (502) staff       (20)      885 2024-04-10 15:45:52.000000 vidsrc-search-0.1.3/src/vidsrc_search/uninstall.py
--rw-r--r--   0 Dev        (502) staff       (20)     6195 2024-04-10 16:47:31.000000 vidsrc-search-0.1.3/src/vidsrc_search/utils.py
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-10 16:53:09.066998 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/
--rw-r--r--   0 Dev        (502) staff       (20)     1473 2024-04-10 16:53:09.000000 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)      502 2024-04-10 16:53:09.000000 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/SOURCES.txt
--rw-r--r--   0 Dev        (502) staff       (20)        1 2024-04-10 16:53:09.000000 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/dependency_links.txt
--rw-r--r--   0 Dev        (502) staff       (20)       62 2024-04-10 16:53:09.000000 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/entry_points.txt
--rw-r--r--   0 Dev        (502) staff       (20)       44 2024-04-10 16:53:09.000000 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/requires.txt
--rw-r--r--   0 Dev        (502) staff       (20)       14 2024-04-10 16:53:09.000000 vidsrc-search-0.1.3/src/vidsrc_search.egg-info/top_level.txt
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-11 00:00:33.050706 vidsrc-search-0.1.4/
+-rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-04-10 17:32:10.000000 vidsrc-search-0.1.4/LICENSE
+-rw-r--r--   0 Dev        (502) staff       (20)        1 2024-04-10 23:53:27.000000 vidsrc-search-0.1.4/LICENSE.txt
+-rw-r--r--   0 Dev        (502) staff       (20)     1462 2024-04-11 00:00:33.050423 vidsrc-search-0.1.4/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)      668 2024-04-10 17:32:10.000000 vidsrc-search-0.1.4/README.md
+-rw-r--r--   0 Dev        (502) staff       (20)      889 2024-04-10 23:53:39.000000 vidsrc-search-0.1.4/pyproject.toml
+-rw-r--r--   0 Dev        (502) staff       (20)       38 2024-04-11 00:00:33.050749 vidsrc-search-0.1.4/setup.cfg
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-11 00:00:33.040283 vidsrc-search-0.1.4/src/
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-11 00:00:33.047779 vidsrc-search-0.1.4/src/vidsrc_search/
+-rw-r--r--   0 Dev        (502) staff       (20)     1235 2024-04-10 22:54:38.000000 vidsrc-search-0.1.4/src/vidsrc_search/__main__.py
+-rw-r--r--   0 Dev        (502) staff       (20)     4739 2024-04-10 23:33:40.000000 vidsrc-search-0.1.4/src/vidsrc_search/argparsing.py
+-rw-r--r--   0 Dev        (502) staff       (20)     2762 2024-04-10 22:52:18.000000 vidsrc-search-0.1.4/src/vidsrc_search/download.py
+-rw-r--r--   0 Dev        (502) staff       (20)     1249 2024-04-10 22:39:47.000000 vidsrc-search-0.1.4/src/vidsrc_search/json_utils.py
+-rw-r--r--   0 Dev        (502) staff       (20)     5322 2024-04-10 23:53:05.000000 vidsrc-search-0.1.4/src/vidsrc_search/search.py
+-rw-r--r--   0 Dev        (502) staff       (20)      884 2024-04-10 22:37:50.000000 vidsrc-search-0.1.4/src/vidsrc_search/uninstall.py
+-rw-r--r--   0 Dev        (502) staff       (20)     6599 2024-04-10 23:59:44.000000 vidsrc-search-0.1.4/src/vidsrc_search/utils.py
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-11 00:00:33.049956 vidsrc-search-0.1.4/src/vidsrc_search.egg-info/
+-rw-r--r--   0 Dev        (502) staff       (20)     1462 2024-04-11 00:00:33.000000 vidsrc-search-0.1.4/src/vidsrc_search.egg-info/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)      502 2024-04-11 00:00:33.000000 vidsrc-search-0.1.4/src/vidsrc_search.egg-info/SOURCES.txt
+-rw-r--r--   0 Dev        (502) staff       (20)        1 2024-04-11 00:00:33.000000 vidsrc-search-0.1.4/src/vidsrc_search.egg-info/dependency_links.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       62 2024-04-11 00:00:33.000000 vidsrc-search-0.1.4/src/vidsrc_search.egg-info/entry_points.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       44 2024-04-11 00:00:33.000000 vidsrc-search-0.1.4/src/vidsrc_search.egg-info/requires.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       14 2024-04-11 00:00:33.000000 vidsrc-search-0.1.4/src/vidsrc_search.egg-info/top_level.txt
```

### Comparing `vidsrc-search-0.1.3/LICENSE` & `vidsrc-search-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vidsrc-search-0.1.3/PKG-INFO` & `vidsrc-search-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vidsrc-search
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pirate movie watcher written in Python
-License: MIT License
+License: 
         
 Project-URL: Homepage, https://github.com/SomedudeX/vidsrc-search
 Keywords: movie,video,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `vidsrc-search-0.1.3/README.md` & `vidsrc-search-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vidsrc-search-0.1.3/pyproject.toml` & `vidsrc-search-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vidsrc-search"
-version = "0.1.3"
+version = "0.1.4"
 description = "A pirate movie watcher written in Python"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
```

### Comparing `vidsrc-search-0.1.3/src/vidsrc_search/__main__.py` & `vidsrc-search-0.1.4/src/vidsrc_search/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import os
 import sys
-import warnings
 
 from . import utils
 from . import argparsing
 
 
 def main():
     try:
@@ -30,14 +29,14 @@
         print()
         print(f" [Fatal] An unknown error was encountered during the execution of vidsrc-search")
         print(f" [Fatal] Error message from program: {e}")
         utils.cleanup()
         print()
         print(f" [Info] Note: ")
         print(f" [Info] This might be due to a temporary error in the program")
-        print(f" [Info] The issue might fix itself if you rerun the program")
+        print(f" [Info] The issue might fix itself if wait a bit and rerun the program")
         print(f" [Info] Vidsrc-search terminating with exit code 255")
         sys.exit(255)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `vidsrc-search-0.1.3/src/vidsrc_search/argparsing.py` & `vidsrc-search-0.1.4/src/vidsrc_search/argparsing.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,41 @@
 
 from . import utils
 from . import search
 from . import download
 from . import uninstall
 
 
+def parse_command_opt_flag() -> None:
+    _argv = sys.argv
+
+    if _argv[1] == "help":
+        print(f" [Fatal] Too many arguments provided for command 'help'")
+        print(f" [Fatal] Use 'vidsrc-search help help' for usage info")
+        print(f" [Fatal] Vidsrc-search terminating with exit code 1")
+        sys.exit(1)
+    elif _argv[1] == "search":
+        if _argv[3] != "--fallback":
+            print(f" [Fatal] Invalid flag '{_argv[3]}' for command 'search'")
+            print(f" [Fatal] Use 'vidsrc-search help search' for usage info")
+            print(f" [Fatal] Vidsrc-search terminating with exit code 1")
+            sys.exit(1)
+        search.handle_search(_argv[2], fallback=True)
+        return
+    elif _argv[1] == "library":
+        print(f" [Fatal] Too many arguments provided for command 'libary'")
+        print(f" [Fatal] Use 'vidsrc-search help library' for usage info")
+        print(f" [Fatal] Vidsrc-search terminating with exit code 1")
+        sys.exit(1)
+    else:
+        print(f" [Fatal] Invalid argument: '{_argv[1]}'")
+        print(f" [Fatal] Use 'vidsrc-search help' for usage info")
+        print(f" [Fatal] Vidsrc-search terminating with exit code 1")
+        sys.exit(1)
+
 def parse_command_opt() -> None:
     _argv = sys.argv
     
     if _argv[1] == "help":
         if _argv[2] == "help":
             utils.show_help_help()
             return
@@ -17,20 +44,25 @@
             utils.show_help_search()
             return
         elif _argv[2] == "library":
             utils.show_help_lib()
             return
         else:
             print(f" [Fatal] Invalid argument for help: '{_argv[2]}'")
-            print(f" [Fatal] Use 'vidsrc-search help' for usage info")
+            print(f" [Fatal] Use 'vidsrc-search help help' for usage info")
             print(f" [Fatal] Vidsrc-search terminating with exit code 1")
             sys.exit(1)
             
     if _argv[1] == "search":
-        search.handle_search(_argv[2])
+        if _argv[2] == "--fallback":
+            print(f" [Fatal] No search query were provided to vidsrc-search")
+            print(f" [Fatal] Use 'vidsrc-search help' for usage info")
+            print(f" [Fatal] Vidsrc-search terminating with exit code 1")
+            sys.exit(1)
+        search.handle_search(_argv[2], fallback=False)
         return
          
     if _argv[1] == "library":
         if _argv[2] == "download":
             download.handle_download()
             return
         elif _argv[2] == "remove":
@@ -81,15 +113,18 @@
         return
     if _argc == 2:
         parse_command()
         return
     if _argc == 3:
         parse_command_opt()
         return
-    if _argc > 3:
+    if _argc == 4:
+        parse_command_opt_flag()
+        return
+    if _argc > 4:
         print(f" [Fatal] Too many arguments provided")
         print(f" [Fatal] Use 'vidsrc-search help' for usage info")
         print(f" [Fatal] Vidsrc-search terminating with exit code 1")
         sys.exit(1)
     
     print(f" [Fatal] An unknown error occured")
     print(f" [Info] Locals:")
```

### Comparing `vidsrc-search-0.1.3/src/vidsrc_search/download.py` & `vidsrc-search-0.1.4/src/vidsrc_search/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 async def fetch_downloads(session, url):
     async with session.get(url) as response:
         return await response.json()
         
 
 async def download_movies(total: int):
     domain = "https://vidsrc.to/vapi/movie/new/"
-    root   = "~/.config/pymovie/movie_buffer/"
+    root   = "~/.local/vidsrc-search/movie_buffer/"
     urls   = [f"{domain}{i}" for i in range(total)]
     print(f" [Info] Initiated download_movies with {total} pages")
     async with aiohttp.ClientSession() as session:
         tasks = [fetch_downloads(session, url) for url in urls]
         jsons = await asyncio.gather(*tasks)
         root = os.path.expanduser(root)
         for index, file in enumerate(jsons):
@@ -52,15 +52,15 @@
             f.write(json.dumps(file))
             f.close()
     print(f" [Info] {total} pages/{total * 15} links were succesfully downloaded")
 
 
 async def download_shows(total: int):
     domain = "https://vidsrc.to/vapi/tv/new/"
-    root   = "~/.config/pymovie/tv_buffer/"
+    root   = "~/.local/vidsrc-search/tv_buffer/"
     urls   = [f"{domain}{i}" for i in range(total)]
     print(f" [Info] Initiated download_shows with {total} pages")
     async with aiohttp.ClientSession() as session:
         tasks = [fetch_downloads(session, url) for url in urls]
         jsons = await asyncio.gather(*tasks)
         root = os.path.expanduser(root)
         for index, file in enumerate(jsons):
```

### Comparing `vidsrc-search-0.1.3/src/vidsrc_search/json_utils.py` & `vidsrc-search-0.1.4/src/vidsrc_search/json_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,23 +21,23 @@
 
 def unite_jsons(movie_index: int, tv_index: int) -> None:
     print(f" [Info] Uniting {movie_index + tv_index} json files")
     unparsed_entries = []
     parsed_entries = []
     for i in range(movie_index): 
         unparsed_entries.append(
-            load_json(f"~/.config/pymovie/movie_buffer/{i}.json")
+            load_json(f"~/.local/vidsrc-search/movie_buffer/{i}.json")
         )
     for i in range(tv_index): 
         unparsed_entries.append(
-            load_json(f"~/.config/pymovie/tv_buffer/{i}.json")
+            load_json(f"~/.local/vidsrc-search/tv_buffer/{i}.json")
         )
 
     print(f" [Info] Parsing {movie_index + tv_index} json files")
     for page in unparsed_entries:
         parsed_entries += parse_entry(page[0])
 
     print(" [Info] Dumping parsed json")
-    path = os.path.expanduser("~/.config/pymovie/lib.json")
+    path = os.path.expanduser("~/.local/vidsrc-search/lib.json")
     with open(path, "w") as f:
         json.dump(parsed_entries, f, indent=4)
     return
```

### Comparing `vidsrc-search-0.1.3/src/vidsrc_search/search.py` & `vidsrc-search-0.1.4/src/vidsrc_search/search.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
 import sys
 import json
 import webview
+import requests
+import webbrowser
 
 from . import utils
 
 from tabulate import tabulate
 from thefuzz.fuzz import partial_ratio, ratio
 
 
@@ -20,15 +22,15 @@
 def sort_results(result: list) -> list:
     result.sort(key = relevance_key, reverse = True)
     return result
 
 
 def search_library(search_query: str):
     ret = []
-    lib_path = os.path.expanduser("~/.config/pymovie/lib.json")
+    lib_path = os.path.expanduser("~/.local/vidsrc-search/lib.json")
     if not os.path.exists(lib_path):
         print(" [Fatal] Library does not exist")
         print(" [Fatal] Please download the library first by using 'vidsrc-search libary download'")
         print(" [Fatal] Vidsrc-search terminating with exit code 2")
         sys.exit(2)
 
     with open(lib_path, "r") as f: 
@@ -78,42 +80,69 @@
     print("           site is not endorsed by the author or checked for its quality, ")
     print("           content, or authenticity. The author of vidsrc-search disclaims")
     print("           any responsibility, express or implied, of the consequences ")
     print("           as a result your usage or dependence on the website provided ")
     print("           through this tool. ")
     print(" [Warning] The following window shown will be the contents of vidsrc.to\n")
     affirm = input(" > I have read and understood the conditions above (Y/n) ")
+    print()
     if not affirm == "Y":
         print()
         print(" [Info] Terminating per user request")
         raise UserWarning
     return
 
 
-def show_movie(index: int, results: list):
+def show_movie(index: int, results: list, fallback: bool = False):
     print_warning()
-    utils.check_internet()    
-    
-    print(f" [Info] Opening index #{index + 1} ({results[index]['Title']}) in external window")
+    utils.check_internet()
+
+    number = index + 1
+    title = results[index]["Title"]
+    url = results[index]["URL"]
+    id = results[index]["IMDB ID"]
+
+    print()
+    print(f" [Info] Checking for local cache")
+
+    if not os.path.exists(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html")):
+        print(f" [Info] Local cache not found: Getting remote html")
+        response = requests.get(url)
+        print(f" [Info] Remote html request status code is {response.status_code}")
+        with open(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"), "w") as f:
+            print(f" [Info] Writing remote html content to local cache")
+            f.write(response.content.decode())
+
+    if not fallback:
+        print(f" [Info] Opening #{number} '{title}' in new browser window")
+        webbrowser.open("file://" + os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"))
+        return
+
+    print(f" [Info] Using fallback mode for movie launching")
+    print(f" [Info] Opening #{number} '{title}' in new window")
     
     window = webview.create_window(
-        f"External - {results[index]['Title']}", 
-        results[index]['URL'],
+        f"External - {title}",
+        os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"),
         maximized = True,
         on_top = True,
     )
-    
+
     window.events.closing += on_closing
     window.events.loaded += on_loaded
-    
-    webview.start(http_server = True)
+
+    webview.start(
+        http_server=True,
+        storage_path=os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}"),
+        private_mode=False
+    )
     return
     
 
-def handle_search(query: str) -> None:
+def handle_search(query: str, fallback: bool = False) -> None:
     print(f" [Info] Searching json libary for '{query}'")
     results = search_library(query)
     if results == None:
         print(f" [Info] '{query}' not found in movies library")
         print(f" [Info] Vidsrc-search terminating due to entry not found")
         return
         
@@ -135,9 +164,9 @@
                 raise ValueError()
             break
         except ValueError:
             print(" [Error] Please enter a valid value")
             continue
     
     open_index -= 1
-    show_movie(open_index, results)
+    show_movie(open_index, results, fallback=fallback)
     return
```

### Comparing `vidsrc-search-0.1.3/src/vidsrc_search/uninstall.py` & `vidsrc-search-0.1.4/src/vidsrc_search/uninstall.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 import json
 
 
 def handle_remove() -> None:
-    lib_path = os.path.expanduser("~/.config/pymovie/lib.json")
+    lib_path = os.path.expanduser("~/.cache/pymovie/lib.json")
     if not os.path.exists(lib_path):
         print(" [Fatal] Library does not exist")
         print(" [Fatal] Please download the library first by using 'vidsrc-search libary download'")
         print(" [Fatal] Vidsrc-search terminating with exit code 2")
         sys.exit(2)
     with open(lib_path, "r") as f:
         jsons = json.load(f)
```

### Comparing `vidsrc-search-0.1.3/src/vidsrc_search/utils.py` & `vidsrc-search-0.1.4/src/vidsrc_search/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,14 +34,20 @@
 HELP_SEARCH = ("\
 Usage: vidsrc-search search <option>                \n\
                                                     \n\
 Required option:                                    \n\
     <str>       a movie title that you would like   \n\
                 vidsrc-search to search for         \n\
                                                     \n\
+Optional flags:                                     \n\
+    --fallback  launch a movie through a custom     \n\
+                python window                       \n\
+                                                    \n\
+                                                    \n\
+                                                    \n\
 Example:                                            \n\
     vidsrc-search search 'oppenheimer'              \n\
     vidsrc-search search 'avatar'                   \
 ")
 
 HELP_LIB = ("\
 Usage: vidsrc-search library <option>               \n\
@@ -73,17 +79,15 @@
     
 def show_help_lib():
     print(HELP_LIB)
     return
 
 
 def make_directory(path: str) -> None:
-    if os.path.exists(path):
-        return
-    os.makedirs(path)
+    os.makedirs(path, exist_ok=True)
     
 
 def delete_directory_recursive(path: str) -> None:
     if os.path.exists(path):
         shutil.rmtree(path)
         
         
@@ -148,24 +152,23 @@
         print(f" [Fatal] Vidsrc-search terminating with exit code 255")
         sys.exit(255)
     return
 
 
 def cleanup() -> None:
     print(" [Info] Performing program cleanup process")
-    path_one = os.path.expanduser("~/.config/pymovie/movie_buffer")
-    path_two = os.path.expanduser("~/.config/pymovie/tv_buffer")
+    path_one = os.path.expanduser("~/.local/vidsrc-search/movie_buffer")
+    path_two = os.path.expanduser("~/.local/vidsrc-search/tv_buffer")
     delete_directory_recursive(path_one)
     delete_directory_recursive(path_two)
+    delete_directory_recursive(os.path.expanduser("~/.config/pymovie"))
     return
 
 
 def bootstrap() -> None:
-    required_path_one = os.path.expanduser("~/.config/pymovie")
-    required_path_two = os.path.expanduser("~/.config/pymovie/movie_buffer")
-    required_path_three = os.path.expanduser("~/.config/pymovie/tv_buffer")
-    
+    required_path_one = os.path.expanduser("~/.local/vidsrc-search/movie_buffer")
+    required_path_two = os.path.expanduser("~/.local/vidsrc-search/tv_buffer")
+    required_path_three = os.path.expanduser("~/.local/vidsrc-search/cache")
     make_directory(required_path_one)
     make_directory(required_path_two)
     make_directory(required_path_three)
-
     return
```

### Comparing `vidsrc-search-0.1.3/src/vidsrc_search.egg-info/PKG-INFO` & `vidsrc-search-0.1.4/src/vidsrc_search.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vidsrc-search
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pirate movie watcher written in Python
-License: MIT License
+License: 
         
 Project-URL: Homepage, https://github.com/SomedudeX/vidsrc-search
 Keywords: movie,video,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

