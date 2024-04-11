# Comparing `tmp/dgcloud-0.1.1.tar.gz` & `tmp/dgcloud-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgcloud-0.1.1.tar", last modified: Sun Apr  7 17:12:22 2024, max compression
+gzip compressed data, was "dgcloud-0.1.2.tar", last modified: Thu Apr 11 17:39:46 2024, max compression
```

## Comparing `dgcloud-0.1.1.tar` & `dgcloud-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 dhinagaran  (1000) dhinagaran  (1000)        0 2024-04-07 17:12:22.062158 dgcloud-0.1.1/
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)     1067 2024-04-03 18:13:56.000000 dgcloud-0.1.1/LICENSE
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)      249 2024-04-07 17:12:22.062158 dgcloud-0.1.1/PKG-INFO
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)       72 2024-04-03 18:13:56.000000 dgcloud-0.1.1/README.md
-drwxrwxr-x   0 dhinagaran  (1000) dhinagaran  (1000)        0 2024-04-07 17:12:22.062158 dgcloud-0.1.1/dgcloud/
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)        1 2024-04-03 18:20:11.000000 dgcloud-0.1.1/dgcloud/__init__.py
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)     2233 2024-04-07 16:47:01.000000 dgcloud-0.1.1/dgcloud/cli.py
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)     1254 2024-04-07 16:47:07.000000 dgcloud-0.1.1/dgcloud/cloud.py
-drwxrwxr-x   0 dhinagaran  (1000) dhinagaran  (1000)        0 2024-04-07 17:12:22.062158 dgcloud-0.1.1/dgcloud.egg-info/
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)      249 2024-04-07 17:12:22.000000 dgcloud-0.1.1/dgcloud.egg-info/PKG-INFO
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)      266 2024-04-07 17:12:22.000000 dgcloud-0.1.1/dgcloud.egg-info/SOURCES.txt
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)        1 2024-04-07 17:12:22.000000 dgcloud-0.1.1/dgcloud.egg-info/dependency_links.txt
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)       46 2024-04-07 17:12:22.000000 dgcloud-0.1.1/dgcloud.egg-info/entry_points.txt
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)       22 2024-04-07 17:12:22.000000 dgcloud-0.1.1/dgcloud.egg-info/requires.txt
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)        8 2024-04-07 17:12:22.000000 dgcloud-0.1.1/dgcloud.egg-info/top_level.txt
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)       38 2024-04-07 17:12:22.062158 dgcloud-0.1.1/setup.cfg
--rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)      472 2024-04-07 17:10:59.000000 dgcloud-0.1.1/setup.py
+drwxrwxr-x   0 dhinagaran  (1000) dhinagaran  (1000)        0 2024-04-11 17:39:46.446337 dgcloud-0.1.2/
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)     1067 2024-04-03 18:13:56.000000 dgcloud-0.1.2/LICENSE
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)      249 2024-04-11 17:39:46.446337 dgcloud-0.1.2/PKG-INFO
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)       72 2024-04-03 18:13:56.000000 dgcloud-0.1.2/README.md
+drwxrwxr-x   0 dhinagaran  (1000) dhinagaran  (1000)        0 2024-04-11 17:39:46.446337 dgcloud-0.1.2/dgcloud/
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)        1 2024-04-03 18:20:11.000000 dgcloud-0.1.2/dgcloud/__init__.py
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)     3300 2024-04-11 17:38:12.000000 dgcloud-0.1.2/dgcloud/cli.py
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)     3081 2024-04-11 17:26:45.000000 dgcloud-0.1.2/dgcloud/cloud.py
+drwxrwxr-x   0 dhinagaran  (1000) dhinagaran  (1000)        0 2024-04-11 17:39:46.446337 dgcloud-0.1.2/dgcloud.egg-info/
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)      249 2024-04-11 17:39:46.000000 dgcloud-0.1.2/dgcloud.egg-info/PKG-INFO
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)      266 2024-04-11 17:39:46.000000 dgcloud-0.1.2/dgcloud.egg-info/SOURCES.txt
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)        1 2024-04-11 17:39:46.000000 dgcloud-0.1.2/dgcloud.egg-info/dependency_links.txt
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)       46 2024-04-11 17:39:46.000000 dgcloud-0.1.2/dgcloud.egg-info/entry_points.txt
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)       22 2024-04-11 17:39:46.000000 dgcloud-0.1.2/dgcloud.egg-info/requires.txt
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)        8 2024-04-11 17:39:46.000000 dgcloud-0.1.2/dgcloud.egg-info/top_level.txt
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)       38 2024-04-11 17:39:46.446337 dgcloud-0.1.2/setup.cfg
+-rw-rw-r--   0 dhinagaran  (1000) dhinagaran  (1000)      512 2024-04-11 17:37:08.000000 dgcloud-0.1.2/setup.py
```

### Comparing `dgcloud-0.1.1/LICENSE` & `dgcloud-0.1.2/LICENSE`

 * *Files identical despite different names*

