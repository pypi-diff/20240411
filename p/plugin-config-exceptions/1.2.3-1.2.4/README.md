# Comparing `tmp/plugin_config_exceptions-1.2.3.tar.gz` & `tmp/plugin_config_exceptions-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugin_config_exceptions-1.2.3.tar", last modified: Thu Apr 11 06:45:45 2024, max compression
+gzip compressed data, was "plugin_config_exceptions-1.2.4.tar", last modified: Thu Apr 11 07:16:27 2024, max compression
```

## Comparing `plugin_config_exceptions-1.2.3.tar` & `plugin_config_exceptions-1.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-11 06:45:45.494861 plugin_config_exceptions-1.2.3/
--rw-r--r--   0 james      (501) staff       (20)      414 2024-04-11 06:45:45.494661 plugin_config_exceptions-1.2.3/PKG-INFO
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-11 06:45:45.494448 plugin_config_exceptions-1.2.3/plugin_config_exceptions.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      414 2024-04-11 06:45:45.000000 plugin_config_exceptions-1.2.3/plugin_config_exceptions.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      200 2024-04-11 06:45:45.000000 plugin_config_exceptions-1.2.3/plugin_config_exceptions.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2024-04-11 06:45:45.000000 plugin_config_exceptions-1.2.3/plugin_config_exceptions.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2024-04-11 06:45:45.000000 plugin_config_exceptions-1.2.3/plugin_config_exceptions.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2024-04-11 06:45:45.494906 plugin_config_exceptions-1.2.3/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      477 2024-04-11 06:45:42.000000 plugin_config_exceptions-1.2.3/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-11 07:16:27.368276 plugin_config_exceptions-1.2.4/
+-rw-r--r--   0 james      (501) staff       (20)      414 2024-04-11 07:16:27.368071 plugin_config_exceptions-1.2.4/PKG-INFO
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-11 07:16:27.367880 plugin_config_exceptions-1.2.4/plugin_config_exceptions.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)      414 2024-04-11 07:16:27.000000 plugin_config_exceptions-1.2.4/plugin_config_exceptions.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      200 2024-04-11 07:16:27.000000 plugin_config_exceptions-1.2.4/plugin_config_exceptions.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-04-11 07:16:27.000000 plugin_config_exceptions-1.2.4/plugin_config_exceptions.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-04-11 07:16:27.000000 plugin_config_exceptions-1.2.4/plugin_config_exceptions.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2024-04-11 07:16:27.368318 plugin_config_exceptions-1.2.4/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)      477 2024-04-11 07:15:44.000000 plugin_config_exceptions-1.2.4/setup.py
```

