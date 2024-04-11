# Comparing `tmp/emx-1.0.3-py3-none-any.whl.zip` & `tmp/emx-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7050 bytes, number of entries: 8
--rw-r--r--  2.0 unx    19044 b- defN 24-Apr-10 14:22 emx/__init__.py
+Zip file size: 7143 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    19105 b- defN 24-Apr-10 14:54 emx/__init__.py
 -rw-r--r--  2.0 unx      239 b- defN 24-Apr-10 11:34 emx/__main__.py
 -rw-r--r--  2.0 unx     2320 b- defN 24-Apr-10 08:57 emx/http.py
--rw-r--r--  2.0 unx      310 b- defN 24-Apr-10 14:23 emx-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 14:23 emx-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 24-Apr-10 14:23 emx-1.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-10 14:23 emx-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      583 b- defN 24-Apr-10 14:23 emx-1.0.3.dist-info/RECORD
-8 files, 22659 bytes uncompressed, 6042 bytes compressed:  73.3%
+-rw-r--r--  2.0 unx      310 b- defN 24-Apr-10 15:06 emx-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 15:06 emx-1.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 24-Apr-10 15:06 emx-1.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-10 15:06 emx-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      583 b- defN 24-Apr-10 15:06 emx-1.0.5.dist-info/RECORD
+8 files, 22720 bytes uncompressed, 6135 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: emx/__main__.py
 Comment: 
 
 Filename: emx/http.py
 Comment: 
 
-Filename: emx-1.0.3.dist-info/METADATA
+Filename: emx-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: emx-1.0.3.dist-info/WHEEL
+Filename: emx-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: emx-1.0.3.dist-info/entry_points.txt
+Filename: emx-1.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: emx-1.0.3.dist-info/top_level.txt
+Filename: emx-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: emx-1.0.3.dist-info/RECORD
+Filename: emx-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## emx/__init__.py

```diff
@@ -10,17 +10,20 @@
 from . import http
 import zipfile
 import tempfile
 import shutil
 from tqdm import tqdm
 import json
 import re
+import uuid
 
 verbose = False
 
+def gencode():
+    return str(uuid.uuid4()).replace("-", "").upper() + str(uuid.uuid4()).replace("-", "").upper()
 
 def get_python_link_name(pydll_path, os_name):
     if os_name == "linux":
         for so in os.listdir(pydll_path):
             if so.startswith("libpython") and not so.endswith(".so") and so.find(".so") != -1:
                 basename = os.path.basename(so[3:so.find(".so")])
                 full_path = os.path.join(pydll_path, so)
@@ -103,24 +106,26 @@
             try:
                 self.config = json.load(open(self.CACHE_FILE))
                 if not isinstance(self.config, dict):
                     self.config = {}
             except Exception as e:
                 print(f"Failed to load config file: {self.CACHE_FILE}")
 
-        user_name = self.config.get("UserName", None)
+        user_token = self.config.get("UserToken", None)
+        user_name  = self.config.get("UserName", None)
         if user_name is None:
             while True:
                 user_name = input(f"Please input your UserName: ")
                 if not user_name.encode("utf-8").isalnum():
                     print(f"An invalid username is entered. Only [a-zA-Z0-9] can be passed.")
                 else:
                     break
-
-            self.config["UserName"] = user_name
+            
+            self.config["UserToken"] = gencode()
+            self.config["UserName"]  = user_name
             json.dump(self.config, open(self.CACHE_FILE, "w"))
 
         self.SERVER_IP   = self.config.get("SERVER_IP", self.SERVER_IP)
         self.SERVER_PORT = self.config.get("SERVER_PORT", self.SERVER_PORT)
         self.SERVER_IP   = os.environ.get("EMX_SERVER_IP", self.SERVER_IP)
         self.SERVER_PORT = os.environ.get("EMX_SERVER_PORT", self.SERVER_PORT)
         self.SERVER      = f"http://{self.SERVER_IP}:{self.SERVER_PORT}"
@@ -168,15 +173,16 @@
 
         req_args = urlencode({
             "keyword": key, 
             "type": "name" if isname else "path", 
             "show_count": show_count,
             "show_skip": show_skip,
             "ftype": "all",
-            "user_name": self.cfg.get_cfg("UserName")
+            "user_name": self.cfg.get_cfg("UserName"),
+            "user_token": self.cfg.get_cfg("UserToken")
         })
         
         resp = http.request_info(f"{self.cfg.SERVER}/search?{req_args}")
         if resp is None:
             return False
         
         files = resp["files"]
@@ -197,15 +203,16 @@
 
         req_args = urlencode({
             "keyword": key, 
             "type": "name", 
             "show_count": show_count,
             "show_skip": show_skip,
             "ftype": "cmds",
-            "user_name": self.cfg.get_cfg("UserName")
+            "user_name": self.cfg.get_cfg("UserName"),
+            "user_token": self.cfg.get_cfg("UserToken")
         })
         
         resp = http.request_info(f"{self.cfg.SERVER}/search?{req_args}")
         if resp is None:
             return False
         
         files = resp["files"]
@@ -265,34 +272,22 @@
         print(f"  update_time: {update_time}")
         print(f"  user_name:   {user_name}")
         print(f"  descript:    {descript}")
 
 
     def get(self, args : argparse.Namespace):
         name = args.name
-        isid = args.id
         save = args.save
         no_unzip = args.no_unzip
 
-        try:
-            n = int(name)
-            if str(n) == name:
-                isid = True
-        except:
-            pass
-
-        if isid:
-            req_args = urlencode({"name": name, "type": "id"})
-        else:
-            req_args = urlencode({"name": name, "type": "name"})
-
+        req_args = urlencode({"name": name, "type": "name", "user_token": self.cfg.get_cfg("UserToken")})
         resp = http.request_info(f"{self.cfg.SERVER}/detail?{req_args}")
         if resp is None:
             return False
-        
+
         isdir = resp["is_directory"] == "True"
         zipped = resp["zipped"] == "True"
         do_unzip = True
         if not zipped or no_unzip:
             do_unzip = False
 
         local = save
@@ -330,27 +325,15 @@
             print(f"Save to: {local}")
             return True
 
     def run(self, args : argparse.Namespace):
         name = args.name
         remargs_string = " ".join(self.remargs)
 
-        isid = False
-        try:
-            n = int(name)
-            if str(n) == name:
-                isid = True
-        except:
-            pass
-
-        if isid:
-            req_args = urlencode({"name": name, "type": "id"})
-        else:
-            req_args = urlencode({"name": name, "type": "name"})
-
+        req_args = urlencode({"name": name, "type": "name", "user_token": self.cfg.get_cfg("UserToken")})
         resp = http.request_info(f"{self.cfg.SERVER}/detail?{req_args}")
         if resp is None:
             return False
         
         # isdir = resp["is_directory"] == "True"
         # zipped = resp["zipped"] == "True"
         file_type = resp["file_type"]
@@ -470,15 +453,16 @@
                     "file_size": str(new_size),
                     "raw_size": str(raw_size),
                     "descript": desc,
                     "is_directory": str(isdir),
                     "num_files": str(len(files)),
                     "zipped": str(zipped),
                     "file_type": file_type,
-                    "user_name": self.cfg.get_cfg("UserName")
+                    "user_name": self.cfg.get_cfg("UserName"),
+                    "user_token": self.cfg.get_cfg("UserToken")
                 }
                 fp.seek(0)
                 resp = http.upload_file(f"{self.cfg.SERVER}/upload", fp, headers, f"Upload: {remote}")
         else:
             size = os.path.getsize(local)
             if size >= 5 * 1024 * 1024:
                 print(f"Over of limit for uploaded file size: {size / 1024 / 1024:.3f} MB, maximum = 5MB")
@@ -489,15 +473,16 @@
                 "file_size": str(size),
                 "raw_size": str(size),
                 "descript": desc,
                 "is_directory": str(isdir),
                 "num_files": str(len(files)),
                 "zipped": str(zipped),
                 "file_type": file_type,
-                "user_name": self.cfg.get_cfg("UserName")
+                "user_name": self.cfg.get_cfg("UserName"),
+                "user_token": self.cfg.get_cfg("UserToken")
             }
             resp = http.upload_file(f"{self.cfg.SERVER}/upload", local, headers, f"Upload: {remote}")
 
         if resp is not None:
             print(f"Complete to upload and you can use [file name: {remote}] to view this file")
 
 class Application:
```

