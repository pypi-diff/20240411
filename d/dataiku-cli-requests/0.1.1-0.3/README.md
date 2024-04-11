# Comparing `tmp/dataiku-cli-requests-0.1.1.tar.gz` & `tmp/dataiku-cli-requests-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataiku-cli-requests-0.1.1.tar", last modified: Wed Feb 14 17:22:59 2024, max compression
+gzip compressed data, was "dataiku-cli-requests-0.3.tar", last modified: Thu Apr 11 09:37:45 2024, max compression
```

## Comparing `dataiku-cli-requests-0.1.1.tar` & `dataiku-cli-requests-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-02-14 17:22:59.275221 dataiku-cli-requests-0.1.1/
--rw-rw-rw-   0        0        0      364 2024-02-14 17:22:59.274227 dataiku-cli-requests-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6323 2023-11-07 09:34:37.000000 dataiku-cli-requests-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-14 17:22:59.255469 dataiku-cli-requests-0.1.1/dataiku_cli_requests/
--rw-rw-rw-   0        0        0        0 2023-11-07 14:18:58.000000 dataiku-cli-requests-0.1.1/dataiku_cli_requests/__init__.py
--rw-rw-rw-   0        0        0     5063 2024-02-14 17:06:15.000000 dataiku-cli-requests-0.1.1/dataiku_cli_requests/dataiku_cli_requests.py
-drwxrwxrwx   0        0        0        0 2024-02-14 17:22:59.272222 dataiku-cli-requests-0.1.1/dataiku_cli_requests.egg-info/
--rw-rw-rw-   0        0        0      364 2024-02-14 17:22:59.000000 dataiku-cli-requests-0.1.1/dataiku_cli_requests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2024-02-14 17:22:59.000000 dataiku-cli-requests-0.1.1/dataiku_cli_requests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-14 17:22:59.000000 dataiku-cli-requests-0.1.1/dataiku_cli_requests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-02-14 17:22:59.000000 dataiku-cli-requests-0.1.1/dataiku_cli_requests.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2024-02-14 17:22:59.000000 dataiku-cli-requests-0.1.1/dataiku_cli_requests.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-02-14 17:22:59.000000 dataiku-cli-requests-0.1.1/dataiku_cli_requests.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-14 17:22:59.275221 dataiku-cli-requests-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      638 2024-02-14 17:22:52.000000 dataiku-cli-requests-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-14 17:22:59.267276 dataiku-cli-requests-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-11-07 17:24:20.000000 dataiku-cli-requests-0.1.1/tests/test_database.py
--rw-rw-rw-   0        0        0        0 2023-11-07 17:23:53.000000 dataiku-cli-requests-0.1.1/tests/test_dataiku.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:37:45.623389 dataiku-cli-requests-0.3/
+-rw-rw-rw-   0        0        0      362 2024-04-11 09:37:45.622322 dataiku-cli-requests-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2024-03-01 10:42:42.000000 dataiku-cli-requests-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 09:37:45.540860 dataiku-cli-requests-0.3/dataiku_cli_requests/
+-rw-rw-rw-   0        0        0        0 2023-11-07 14:18:58.000000 dataiku-cli-requests-0.3/dataiku_cli_requests/__init__.py
+-rw-rw-rw-   0        0        0     5063 2024-02-14 17:06:15.000000 dataiku-cli-requests-0.3/dataiku_cli_requests/dataiku_cli_requests.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:37:45.618320 dataiku-cli-requests-0.3/dataiku_cli_requests.egg-info/
+-rw-rw-rw-   0        0        0      362 2024-04-11 09:37:45.000000 dataiku-cli-requests-0.3/dataiku_cli_requests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2024-04-11 09:37:45.000000 dataiku-cli-requests-0.3/dataiku_cli_requests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 09:37:45.000000 dataiku-cli-requests-0.3/dataiku_cli_requests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-11 09:37:45.000000 dataiku-cli-requests-0.3/dataiku_cli_requests.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2024-04-11 09:37:45.000000 dataiku-cli-requests-0.3/dataiku_cli_requests.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-11 09:37:45.000000 dataiku-cli-requests-0.3/dataiku_cli_requests.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 09:37:45.623389 dataiku-cli-requests-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      636 2024-04-11 09:37:08.000000 dataiku-cli-requests-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:37:45.603093 dataiku-cli-requests-0.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-11-07 17:24:20.000000 dataiku-cli-requests-0.3/tests/test_database.py
+-rw-rw-rw-   0        0        0        0 2023-11-07 17:23:53.000000 dataiku-cli-requests-0.3/tests/test_dataiku.py
```

### Comparing `dataiku-cli-requests-0.1.1/dataiku_cli_requests/dataiku_cli_requests.py` & `dataiku-cli-requests-0.3/dataiku_cli_requests/dataiku_cli_requests.py`

 * *Files identical despite different names*

### Comparing `dataiku-cli-requests-0.1.1/setup.py` & `dataiku-cli-requests-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dataiku-cli-requests',
-    version='0.1.1',
+    version='0.3',
     url='https://www.funiber.org',
     author='David Grau Martinez',
     author_email='david.grau@funiber.org',
     description='Una herramienta de línea de comandos para interactuar con Dataiku utilizando solicitudes HTTP',
     packages=find_packages(),
     install_requires=[
         'requests',
```

