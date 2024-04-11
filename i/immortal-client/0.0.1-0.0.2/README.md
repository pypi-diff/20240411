# Comparing `tmp/immortal-client-0.0.1.tar.gz` & `tmp/immortal-client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immortal-client-0.0.1.tar", last modified: Thu Apr 11 16:27:41 2024, max compression
+gzip compressed data, was "immortal-client-0.0.2.tar", last modified: Thu Apr 11 17:03:37 2024, max compression
```

## Comparing `immortal-client-0.0.1.tar` & `immortal-client-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 16:27:41.807849 immortal-client-0.0.1/
--rw-rw-rw-   0        0        0     1067 2024-04-03 22:08:13.000000 immortal-client-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      287 2024-04-11 16:27:41.806832 immortal-client-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-03 21:46:04.000000 immortal-client-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 16:27:41.799830 immortal-client-0.0.1/immortal_client/
--rw-rw-rw-   0        0        0        0 2024-04-03 21:46:24.000000 immortal-client-0.0.1/immortal_client/__init__.py
--rw-rw-rw-   0        0        0      477 2024-04-04 07:57:04.000000 immortal-client-0.0.1/immortal_client/client.py
-drwxrwxrwx   0        0        0        0 2024-04-11 16:27:41.805848 immortal-client-0.0.1/immortal_client.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-11 16:27:41.000000 immortal-client-0.0.1/immortal_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-04-11 16:27:41.000000 immortal-client-0.0.1/immortal_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 16:27:41.000000 immortal-client-0.0.1/immortal_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 16:27:41.000000 immortal-client-0.0.1/immortal_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-11 16:27:41.000000 immortal-client-0.0.1/immortal_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 16:27:41.807849 immortal-client-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      381 2024-04-11 16:26:23.000000 immortal-client-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:03:37.169850 immortal-client-0.0.2/
+-rw-rw-rw-   0        0        0     1067 2024-04-03 22:08:13.000000 immortal-client-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2022 2024-04-11 17:03:37.167879 immortal-client-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-03 21:46:04.000000 immortal-client-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 17:03:37.157850 immortal-client-0.0.2/immortal_client/
+-rw-rw-rw-   0        0        0        0 2024-04-03 21:46:24.000000 immortal-client-0.0.2/immortal_client/__init__.py
+-rw-rw-rw-   0        0        0      477 2024-04-04 07:57:04.000000 immortal-client-0.0.2/immortal_client/client.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:03:37.166850 immortal-client-0.0.2/immortal_client.egg-info/
+-rw-rw-rw-   0        0        0     2022 2024-04-11 17:03:37.000000 immortal-client-0.0.2/immortal_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-04-11 17:03:37.000000 immortal-client-0.0.2/immortal_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 17:03:37.000000 immortal-client-0.0.2/immortal_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-11 17:03:37.000000 immortal-client-0.0.2/immortal_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-11 17:03:37.000000 immortal-client-0.0.2/immortal_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      809 2024-04-11 17:01:40.000000 immortal-client-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 17:03:37.169850 immortal-client-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      450 2024-04-11 17:03:28.000000 immortal-client-0.0.2/setup.py
```

### Comparing `immortal-client-0.0.1/LICENSE` & `immortal-client-0.0.2/LICENSE`

 * *Files identical despite different names*

