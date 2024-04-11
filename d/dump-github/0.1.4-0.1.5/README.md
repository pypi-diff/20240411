# Comparing `tmp/dump_github-0.1.4-py3-none-any.whl.zip` & `tmp/dump_github-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4501 bytes, number of entries: 10
+Zip file size: 4600 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx       43 b- defN 24-Apr-10 18:26 dump_github/__init__.py
 -rw-rw-r--  2.0 unx      715 b- defN 24-Apr-10 17:24 dump_github/lib.py
--rw-rw-r--  2.0 unx     1506 b- defN 24-Apr-11 06:23 dump_github/main.py
+-rw-rw-r--  2.0 unx     1639 b- defN 24-Apr-11 10:25 dump_github/main.py
 -rw-rw-r--  2.0 unx      715 b- defN 24-Apr-10 17:24 dump_github/mylib.py
--rw-rw-r--  2.0 unx     1064 b- defN 24-Apr-11 06:27 dump_github-0.1.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1162 b- defN 24-Apr-11 06:27 dump_github-0.1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-11 06:27 dump_github-0.1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       50 b- defN 24-Apr-11 06:27 dump_github-0.1.4.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 24-Apr-11 06:27 dump_github-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      809 b- defN 24-Apr-11 06:27 dump_github-0.1.4.dist-info/RECORD
-10 files, 6168 bytes uncompressed, 3113 bytes compressed:  49.5%
+-rw-rw-r--  2.0 unx     1064 b- defN 24-Apr-11 10:27 dump_github-0.1.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1287 b- defN 24-Apr-11 10:27 dump_github-0.1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-11 10:27 dump_github-0.1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       50 b- defN 24-Apr-11 10:27 dump_github-0.1.5.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 24-Apr-11 10:27 dump_github-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      809 b- defN 24-Apr-11 10:27 dump_github-0.1.5.dist-info/RECORD
+10 files, 6426 bytes uncompressed, 3212 bytes compressed:  50.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: dump_github/main.py
 Comment: 
 
 Filename: dump_github/mylib.py
 Comment: 
 
-Filename: dump_github-0.1.4.dist-info/LICENSE
+Filename: dump_github-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: dump_github-0.1.4.dist-info/METADATA
+Filename: dump_github-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: dump_github-0.1.4.dist-info/WHEEL
+Filename: dump_github-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: dump_github-0.1.4.dist-info/entry_points.txt
+Filename: dump_github-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: dump_github-0.1.4.dist-info/top_level.txt
+Filename: dump_github-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: dump_github-0.1.4.dist-info/RECORD
+Filename: dump_github-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dump_github/main.py

```diff
@@ -1,44 +1,51 @@
 import argparse
 import os
 from .lib import *
 
-# Config_MaxSize = 1_000
-
 parser = argparse.ArgumentParser(
     prog="dump-github",
     description="Backup users github repo.",
     epilog="https://github.com/Core2002/dump_github",
 )
 
 parser.add_argument("username")
 parser.add_argument(
     "-d", "--download_zip", action="store_true", help="only download zip file"
 )
 parser.add_argument("-p", "--print", action="store_true", help="only print urls")
-parser.add_argument("-t", "--token", action="store", default="", help="github token")
+parser.add_argument("--token", action="store", default="", help="github token")
+parser.add_argument(
+    "--limit_size",
+    type=int,
+    default=100,
+    help="limit size(MB) of download zip file, if 0 then no limit(default:100).",
+)
 
 args = parser.parse_args()
 
 
 def clone_repo(repo):
     name = repo["name"]
     url = repo["clone_url"]
     size = repo["size"]
-    # if int(size) > Config_MaxSize:
-    #     print(f"Keep repo [{name}], Becues size is too Big ({int(size)}).")
-    #     return
     print("Clone repo: {}".format(name))
     os.system("git clone {}".format(url))
 
 
 def download_zip(user_name, reop):
     url = f"https://github.com/{user_name}/{reop['name']}/archive/refs/heads/{reop['default_branch']}.zip"
-    print("Downloading repo zip: {}".format(reop["name"]))
-    os.system("wget {} -O ./{}_{}.zip".format(url, user_name, reop["name"]))
+    max_size = args.limit_size * 1000 * 1000
+    cmd = (
+        "curl --retry 3 --retry-delay 3 -L --max-filesize {} {} -o ./{}_{}.zip".format(
+            max_size, url, user_name, reop["name"]
+        )
+    )
+    print(f"Download {reop['name']} : {url}")
+    os.system(cmd)
 
 
 def main():
     # print(args)
     repos = serach_user_repos(args.username, args.token)
     for repo in repos:
         if args.print == True:
```

## Comparing `dump_github-0.1.4.dist-info/LICENSE` & `dump_github-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dump_github-0.1.4.dist-info/METADATA` & `dump_github-0.1.5.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dump-github
-Version: 0.1.4
+Version: 0.1.5
 Summary: This tool can be used to back up users' GitHub repositories in case they need them later.
 Home-page: https://github.com/core2002/dump_github
 Author: core2002
 Author-email: core2002@aliyun.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,25 +17,26 @@
 
 ### Github Dumper
 
 Github Dumper is a Python program designed to search for users' GitHub repositories and download the repositories. This tool can be used to back up users' GitHub repositories in case they need them later.
 
 **Usage:**
 ```
-usage: dump-github [-h] [-d] [-p] [-t TOKEN] username
+usage: dump-github [-h] [-d] [-p] [--token TOKEN] [--limit_size LIMIT_SIZE] username
 
 Backup users github repo.
 
 positional arguments:
   username
 
 options:
   -h, --help            show this help message and exit
   -d, --download_zip    only download zip file
   -p, --print           only print urls
-  -t TOKEN, --token TOKEN
-                        github token
+  --token TOKEN         github token
+  --limit_size LIMIT_SIZE
+                        limit size(MB) of download zip file, if 0 then no limit(default:100).
 
 https://github.com/Core2002/dump_github
 ```
```

