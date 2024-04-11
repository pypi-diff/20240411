# Comparing `tmp/spydir-0.1.1.tar.gz` & `tmp/spydir-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spydir-0.1.1.tar", last modified: Wed Apr 10 00:46:38 2024, max compression
+gzip compressed data, was "spydir-0.1.2.tar", last modified: Thu Apr 11 07:31:17 2024, max compression
```

## Comparing `spydir-0.1.1.tar` & `spydir-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-10 00:46:38.156617 spydir-0.1.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       70 2024-04-10 00:17:14.000000 spydir-0.1.1/.gitignore
--rw-r--r--   0 sergey    (1000) sergey    (1000)      122 2024-04-08 22:52:28.000000 spydir-0.1.1/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      810 2024-04-10 00:46:38.156617 spydir-0.1.1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      226 2024-04-10 00:17:37.000000 spydir-0.1.1/README.md
--rw-r--r--   0 sergey    (1000) sergey    (1000)      663 2024-04-08 22:56:10.000000 spydir-0.1.1/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-04-10 00:46:38.156617 spydir-0.1.1/setup.cfg
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-10 00:46:38.156617 spydir-0.1.1/spydir.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      810 2024-04-10 00:46:38.000000 spydir-0.1.1/spydir.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      235 2024-04-10 00:46:38.000000 spydir-0.1.1/spydir.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-10 00:46:38.000000 spydir-0.1.1/spydir.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2024-04-10 00:46:38.000000 spydir-0.1.1/spydir.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       44 2024-04-10 00:46:38.000000 spydir-0.1.1/spydir.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        7 2024-04-10 00:46:38.000000 spydir-0.1.1/spydir.egg-info/top_level.txt
--rwxr-xr-x   0 sergey    (1000) sergey    (1000)     8967 2024-04-10 00:25:34.000000 spydir-0.1.1/spydir.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-11 07:31:17.619607 spydir-0.1.2/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       83 2024-04-11 07:26:00.000000 spydir-0.1.2/.gitignore
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      122 2024-04-08 22:52:28.000000 spydir-0.1.2/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      808 2024-04-11 07:31:17.619607 spydir-0.1.2/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      224 2024-04-10 23:29:40.000000 spydir-0.1.2/README.md
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      663 2024-04-08 22:56:10.000000 spydir-0.1.2/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-04-11 07:31:17.619607 spydir-0.1.2/setup.cfg
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-11 07:31:17.619607 spydir-0.1.2/spydir.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      808 2024-04-11 07:31:17.000000 spydir-0.1.2/spydir.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      235 2024-04-11 07:31:17.000000 spydir-0.1.2/spydir.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-11 07:31:17.000000 spydir-0.1.2/spydir.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2024-04-11 07:31:17.000000 spydir-0.1.2/spydir.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       44 2024-04-11 07:31:17.000000 spydir-0.1.2/spydir.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        7 2024-04-11 07:31:17.000000 spydir-0.1.2/spydir.egg-info/top_level.txt
+-rwxr-xr-x   0 sergey    (1000) sergey    (1000)     9648 2024-04-10 23:24:06.000000 spydir-0.1.2/spydir.py
```

### Comparing `spydir-0.1.1/PKG-INFO` & `spydir-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spydir
-Version: 0.1.1
+Version: 0.1.2
 Author: Sergey M
 License: FUCK LICENSE
         
         Author attribution is required. Commercial use permitted. If you don't like Russians then go fuck yourself.
         
 Project-URL: Repository, https://github.com/s3rgeym/spydir.git
 Classifier: Topic :: Internet
@@ -22,13 +22,13 @@
 
 Directory listing scanner to search for downloadable archives and other files
 
 ```bash
 # you can use pip instead
 pipx install spydir
 
-# scan list of hosts
-spydir -i hosts.txt -o results.txt
+# scan list of urls
+spydir -i urls.txt -o results.txt
 
 # see help
 spydir -h
 ```
```

### Comparing `spydir-0.1.1/pyproject.toml` & `spydir-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spydir-0.1.1/spydir.egg-info/PKG-INFO` & `spydir-0.1.2/spydir.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spydir
-Version: 0.1.1
+Version: 0.1.2
 Author: Sergey M
 License: FUCK LICENSE
         
         Author attribution is required. Commercial use permitted. If you don't like Russians then go fuck yourself.
         
 Project-URL: Repository, https://github.com/s3rgeym/spydir.git
 Classifier: Topic :: Internet
@@ -22,13 +22,13 @@
 
 Directory listing scanner to search for downloadable archives and other files
 
 ```bash
 # you can use pip instead
 pipx install spydir
 
-# scan list of hosts
-spydir -i hosts.txt -o results.txt
+# scan list of urls
+spydir -i urls.txt -o results.txt
 
 # see help
 spydir -h
 ```
```

### Comparing `spydir-0.1.1/spydir.py` & `spydir-0.1.2/spydir.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 import itertools
 import logging
 import multiprocessing as mp
 import re
 import sys
 import threading
 from dataclasses import dataclass
+from pathlib import Path
 from typing import Sequence, TextIO, Type
 from urllib.parse import urljoin
 
 import requests
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 __author__ = "Sergey M"
 
 logger = mp.get_logger()
 
 requests.packages.urllib3.disable_warnings()
 
@@ -94,14 +95,20 @@
         ".conf",
         ".cfg",
         ".ini",
         ".yml",
         ".yaml",
         # php
         ".inc",
+        # скрипты. Их часто используют для дампа базы, те они содержат ее креды
+        ".py",
+        ".pl",
+        ".sh",
+        ".ps",
+        ".bat",
         # other
         ".bk",
         ".bak",
         ".Dockerfile",
         ".log",
         ".log.gz",
     )
@@ -182,23 +189,28 @@
 
             # logger.debug("found link: %s", url)
 
             # Не переходим на уровень выше
             if url == top_level_url:
                 continue
 
-            # Все что можно скачать
-            if url.lower().endswith(self.downloadable_exts):
-                logger.info("found: %s", url)
-                self.out_q.put(url)
-                continue
-
             # Проверяем все вложенные папки
             if url.endswith("/"):
                 self.in_q.put(url)
+                continue
+
+            # Ищем все что можно выкачать в тч файлы без расширений
+            if not self.check_has_extension(url) or url.lower().endswith(
+                self.downloadable_exts
+            ):
+                logger.info("found: %s", url)
+                self.out_q.put(url)
+
+    def check_has_extension(self, url: str) -> bool:
+        return "." in Path(url).name
 
 
 def normalize_url(s: str) -> str:
     return ["https://", ""]["://" in s] + s
 
 
 class OutputThread(threading.Thread):
@@ -221,29 +233,32 @@
     "/wordpress/",
     "/backup/",
     "/backups/",
     "/dump/",
     "/dumps/",
     "/database/",
     "/db/",
-    "/sql/",
+    # "/sql/",
     "/data/",
     "/files/",
-    "/upload/",
-    "/uploads/",
     "/include/",
     "/includes/",
     "/inc/",
     "/sys/",
     "/system/",
     "/lib/",
     "/.docker/",
     "/docker/",
     "/logs/",
     "/log/",
+    "/scripts/",
+    "/tools/",
+    "/app/",
+    "/web/",
+    "/private/",
 )
 
 
 @dataclass
 class SpyDir:
     output: TextIO = sys.stdout
     workers_num: int | None = None
@@ -254,14 +269,15 @@
         self.workers_num = self.workers_num or (mp.cpu_count() * 2 - 1)
 
     class NameSpace(argparse.Namespace):
         input: TextIO
         output: TextIO
         workers_num: int
         debug: bool
+        quiet: bool
         timeout: float
         user_agent: str | None
 
     @classmethod
     def parse_args(
         cls: Type[SpyDir],
         argv: Sequence[str] | None,
@@ -271,14 +287,15 @@
             "-i", "--input", type=argparse.FileType(), default="-"
         )
         parser.add_argument(
             "-o", "--output", type=argparse.FileType("w+"), default="-"
         )
         parser.add_argument("-w", "--workers-num", type=int)
         parser.add_argument("-d", "--debug", action="store_true", default=False)
+        parser.add_argument("-q", "--quiet", action="store_true", default=False)
         parser.add_argument("-t", "--timeout", type=float, default=10.0)
         parser.add_argument("-ua", "--user-agent")
         return parser, parser.parse_args(args=argv, namespace=cls.NameSpace())
 
     @classmethod
     def cli(cls: Type[SpyDir], argv: Sequence[str] | None = None) -> int | None:
         parser, args = cls.parse_args(argv)
@@ -336,12 +353,17 @@
         out_t.join()
 
         logger.info("Finished!")
 
     @staticmethod
     def configure_logger(args: NameSpace) -> None:
         logger.addHandler(ColorHandler())
-        logger.setLevel([logging.INFO, logging.DEBUG][args.debug])
+
+        logger.setLevel(
+            logging.CRITICAL
+            if args.quiet
+            else [logging.INFO, logging.DEBUG][args.debug]
+        )
 
 
 if __name__ == "__main__":
     sys.exit(SpyDir.cli())
```

