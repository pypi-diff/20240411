# Comparing `tmp/headline-gen-1.0.tar.gz` & `tmp/headline-gen-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headline-gen-1.0.tar", last modified: Thu Apr 11 05:06:47 2024, max compression
+gzip compressed data, was "headline-gen-1.1.tar", last modified: Thu Apr 11 05:17:33 2024, max compression
```

## Comparing `headline-gen-1.0.tar` & `headline-gen-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:06:47.372288 headline-gen-1.0/
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-11 05:06:47.371287 headline-gen-1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:06:47.370287 headline-gen-1.0/headline_gen/
--rw-r--r--   0 root         (0) root         (0)    13088 2024-04-11 05:06:11.000000 headline-gen-1.0/headline_gen/Control.py
--rw-r--r--   0 root         (0) root         (0)       86 2024-04-11 04:54:13.000000 headline-gen-1.0/headline_gen/__int__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:06:47.371287 headline-gen-1.0/headline_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-11 05:06:47.000000 headline-gen-1.0/headline_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      235 2024-04-11 05:06:47.000000 headline-gen-1.0/headline_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 05:06:47.000000 headline-gen-1.0/headline_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-11 05:06:47.000000 headline-gen-1.0/headline_gen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-11 05:06:47.000000 headline-gen-1.0/headline_gen.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 05:06:47.372288 headline-gen-1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      427 2024-04-11 05:06:25.000000 headline-gen-1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:17:33.412355 headline-gen-1.1/
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-11 05:17:33.412355 headline-gen-1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:17:33.410355 headline-gen-1.1/headline_gen/
+-rw-r--r--   0 root         (0) root         (0)    13132 2024-04-11 05:16:26.000000 headline-gen-1.1/headline_gen/Control.py
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-11 04:54:13.000000 headline-gen-1.1/headline_gen/__int__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:17:33.411355 headline-gen-1.1/headline_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-11 05:17:33.000000 headline-gen-1.1/headline_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      235 2024-04-11 05:17:33.000000 headline-gen-1.1/headline_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 05:17:33.000000 headline-gen-1.1/headline_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-11 05:17:33.000000 headline-gen-1.1/headline_gen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-11 05:17:33.000000 headline-gen-1.1/headline_gen.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 05:17:33.412355 headline-gen-1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      427 2024-04-11 05:16:49.000000 headline-gen-1.1/setup.py
```

### Comparing `headline-gen-1.0/headline_gen/Control.py` & `headline-gen-1.1/headline_gen/Control.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,18 @@
         print("No Server Object Provided")
       else:
         Server.stop()
     else:
       print("Un defined Operation")
   else:
     print("Parser Files Not Found")
-    print("Attempting to Install Parser Files")
+    print("Attempting to Install Parser Files (This may take a Min or Two!!)")
     Downloader()
-    ServerInit(Mode, Server = Server)
+    if Mode == "Start":
+      ServerInit("Start")
 
 # Key Phrase Extraction
 
 def remove_punctuation(text):
   table = str.maketrans('', '', string.punctuation)
   return text.translate(table)
```

