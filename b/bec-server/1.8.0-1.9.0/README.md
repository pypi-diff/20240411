# Comparing `tmp/bec-server-1.8.0.tar.gz` & `tmp/bec-server-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec-server-1.8.0.tar", last modified: Tue Feb 20 20:19:29 2024, max compression
+gzip compressed data, was "bec-server-1.9.0.tar", last modified: Thu Feb 22 19:50:23 2024, max compression
```

## Comparing `bec-server-1.8.0.tar` & `bec-server-1.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:29.243608 bec-server-1.8.0/
--rw-r--r--   0 root         (0) root         (0)      442 2024-02-20 20:19:29.243608 bec-server-1.8.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:29.243608 bec-server-1.8.0/bec_server/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-02-20 11:03:23.000000 bec-server-1.8.0/bec_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2024-02-20 11:03:23.000000 bec-server-1.8.0/bec_server/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2024-02-20 11:03:23.000000 bec-server-1.8.0/bec_server/service_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2024-02-20 11:03:23.000000 bec-server-1.8.0/bec_server/tmux_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:29.243608 bec-server-1.8.0/bec_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      442 2024-02-20 20:19:29.000000 bec-server-1.8.0/bec_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2024-02-20 20:19:29.000000 bec-server-1.8.0/bec_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 20:19:29.000000 bec-server-1.8.0/bec_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-02-20 20:19:29.000000 bec-server-1.8.0/bec_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      192 2024-02-20 20:19:29.000000 bec-server-1.8.0/bec_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-02-20 20:19:29.000000 bec-server-1.8.0/bec_server.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-02-20 20:19:29.244608 bec-server-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2184 2024-02-20 20:19:24.000000 bec-server-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:23.031110 bec-server-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)      442 2024-02-22 19:50:23.031110 bec-server-1.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:23.031110 bec-server-1.9.0/bec_server/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-02-22 18:57:01.000000 bec-server-1.9.0/bec_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2024-02-22 18:57:01.000000 bec-server-1.9.0/bec_server/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2024-02-22 18:57:01.000000 bec-server-1.9.0/bec_server/service_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2024-02-22 18:57:01.000000 bec-server-1.9.0/bec_server/tmux_launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:23.031110 bec-server-1.9.0/bec_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      442 2024-02-22 19:50:23.000000 bec-server-1.9.0/bec_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2024-02-22 19:50:23.000000 bec-server-1.9.0/bec_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 19:50:23.000000 bec-server-1.9.0/bec_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-02-22 19:50:23.000000 bec-server-1.9.0/bec_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2024-02-22 19:50:23.000000 bec-server-1.9.0/bec_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-02-22 19:50:23.000000 bec-server-1.9.0/bec_server.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-02-22 19:50:23.035110 bec-server-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2184 2024-02-22 19:50:16.000000 bec-server-1.9.0/setup.py
```

### Comparing `bec-server-1.8.0/bec_server/launch.py` & `bec-server-1.9.0/bec_server/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-1.8.0/bec_server/service_handler.py` & `bec-server-1.9.0/bec_server/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-1.8.0/bec_server/tmux_launch.py` & `bec-server-1.9.0/bec_server/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-1.8.0/setup.py` & `bec-server-1.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import subprocess
 import sys
 
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
```

