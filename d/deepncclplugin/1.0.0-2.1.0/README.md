# Comparing `tmp/deepncclplugin-1.0.0.tar.gz` & `tmp/deepncclplugin-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepncclplugin-1.0.0.tar", last modified: Thu Oct 19 07:25:11 2023, max compression
+gzip compressed data, was "deepncclplugin-2.1.0.tar", last modified: Thu Apr 11 02:05:54 2024, max compression
```

## Comparing `deepncclplugin-1.0.0.tar` & `deepncclplugin-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 07:25:11.985056 deepncclplugin-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1920 2023-10-19 07:25:11.982077 deepncclplugin-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1105 2023-10-19 07:08:17.000000 deepncclplugin-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 07:25:11.906945 deepncclplugin-1.0.0/deepncclplugin/
--rw-r--r--   0 root         (0) root         (0)      769 2023-09-08 09:07:18.000000 deepncclplugin-1.0.0/deepncclplugin/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)  4138600 2023-10-19 07:25:10.000000 deepncclplugin-1.0.0/deepncclplugin/libnccl-net.so.0.0.0
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 07:25:11.972356 deepncclplugin-1.0.0/deepncclplugin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1920 2023-10-19 07:25:11.000000 deepncclplugin-1.0.0/deepncclplugin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      270 2023-10-19 07:25:11.000000 deepncclplugin-1.0.0/deepncclplugin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-19 07:25:11.000000 deepncclplugin-1.0.0/deepncclplugin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-10-19 07:25:11.000000 deepncclplugin-1.0.0/deepncclplugin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-10-19 07:25:11.000000 deepncclplugin-1.0.0/deepncclplugin.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-19 07:25:11.987041 deepncclplugin-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3523 2023-10-19 07:24:48.000000 deepncclplugin-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:05:54.028218 deepncclplugin-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)      531 2024-04-11 02:05:54.024150 deepncclplugin-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-04-07 06:30:01.000000 deepncclplugin-2.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:05:53.934682 deepncclplugin-2.1.0/deepncclplugin/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:26:14.000000 deepncclplugin-2.1.0/deepncclplugin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:05:54.004841 deepncclplugin-2.1.0/deepncclplugin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      531 2024-04-11 02:05:53.000000 deepncclplugin-2.1.0/deepncclplugin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2024-04-11 02:05:53.000000 deepncclplugin-2.1.0/deepncclplugin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 02:05:53.000000 deepncclplugin-2.1.0/deepncclplugin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-11 02:05:53.000000 deepncclplugin-2.1.0/deepncclplugin.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 02:05:54.030819 deepncclplugin-2.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3133 2024-04-11 02:05:38.000000 deepncclplugin-2.1.0/setup.py
```

### Comparing `deepncclplugin-1.0.0/README.md` & `deepncclplugin-2.1.0/README.md`

 * *Files identical despite different names*

