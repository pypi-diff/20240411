# Comparing `tmp/headline-gen-1.1.tar.gz` & `tmp/headline-gen-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headline-gen-1.1.tar", last modified: Thu Apr 11 05:17:33 2024, max compression
+gzip compressed data, was "headline-gen-2.0.tar", last modified: Thu Apr 11 05:24:46 2024, max compression
```

## Comparing `headline-gen-1.1.tar` & `headline-gen-2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:17:33.412355 headline-gen-1.1/
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-11 05:17:33.412355 headline-gen-1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:17:33.410355 headline-gen-1.1/headline_gen/
--rw-r--r--   0 root         (0) root         (0)    13132 2024-04-11 05:16:26.000000 headline-gen-1.1/headline_gen/Control.py
--rw-r--r--   0 root         (0) root         (0)       86 2024-04-11 04:54:13.000000 headline-gen-1.1/headline_gen/__int__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:17:33.411355 headline-gen-1.1/headline_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-11 05:17:33.000000 headline-gen-1.1/headline_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      235 2024-04-11 05:17:33.000000 headline-gen-1.1/headline_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 05:17:33.000000 headline-gen-1.1/headline_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-11 05:17:33.000000 headline-gen-1.1/headline_gen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-11 05:17:33.000000 headline-gen-1.1/headline_gen.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 05:17:33.412355 headline-gen-1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      427 2024-04-11 05:16:49.000000 headline-gen-1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:24:46.178603 headline-gen-2.0/
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-11 05:24:46.178603 headline-gen-2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:24:46.176603 headline-gen-2.0/headline_gen/
+-rw-r--r--   0 root         (0) root         (0)    13162 2024-04-11 05:24:29.000000 headline-gen-2.0/headline_gen/Control.py
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-11 04:54:13.000000 headline-gen-2.0/headline_gen/__int__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:24:46.178603 headline-gen-2.0/headline_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-11 05:24:46.000000 headline-gen-2.0/headline_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      235 2024-04-11 05:24:46.000000 headline-gen-2.0/headline_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 05:24:46.000000 headline-gen-2.0/headline_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-11 05:24:46.000000 headline-gen-2.0/headline_gen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-11 05:24:46.000000 headline-gen-2.0/headline_gen.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 05:24:46.178603 headline-gen-2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      427 2024-04-11 05:24:11.000000 headline-gen-2.0/setup.py
```

### Comparing `headline-gen-1.1/headline_gen/Control.py` & `headline-gen-2.0/headline_gen/Control.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,16 @@
     else:
       print("Un defined Operation")
   else:
     print("Parser Files Not Found")
     print("Attempting to Install Parser Files (This may take a Min or Two!!)")
     Downloader()
     if Mode == "Start":
-      ServerInit("Start")
+      server = ServerInit("Start")
+      return server
 
 # Key Phrase Extraction
 
 def remove_punctuation(text):
   table = str.maketrans('', '', string.punctuation)
   return text.translate(table)
```

