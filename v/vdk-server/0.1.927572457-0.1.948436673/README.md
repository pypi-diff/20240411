# Comparing `tmp/vdk-server-0.1.927572457.tar.gz` & `tmp/vdk-server-0.1.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-server-0.1.927572457.tar", last modified: Tue Jul 11 12:43:00 2023, max compression
+gzip compressed data, was "vdk-server-0.1.948436673.tar", last modified: Fri Jul 28 09:43:23 2023, max compression
```

## Comparing `vdk-server-0.1.927572457.tar` & `vdk-server-0.1.948436673.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:43:00.486867 vdk-server-0.1.927572457/
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-11 12:42:44.000000 vdk-server-0.1.927572457/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      992 2023-07-11 12:43:00.486867 vdk-server-0.1.927572457/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      374 2023-07-11 12:42:44.000000 vdk-server-0.1.927572457/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 12:43:00.486867 vdk-server-0.1.927572457/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1147 2023-07-11 12:42:49.000000 vdk-server-0.1.927572457/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:43:00.486867 vdk-server-0.1.927572457/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:43:00.486867 vdk-server-0.1.927572457/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:43:00.486867 vdk-server-0.1.927572457/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:43:00.486867 vdk-server-0.1.927572457/src/vdk/plugin/server/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-11 12:42:44.000000 vdk-server-0.1.927572457/src/vdk/plugin/server/configmap-local-registry-hosting-template.yaml
--rw-rw-rw-   0 root         (0) root         (0)    20085 2023-07-11 12:42:44.000000 vdk-server-0.1.927572457/src/vdk/plugin/server/ingress-nginx-deploy.yaml
--rw-rw-rw-   0 root         (0) root         (0)    33435 2023-07-11 12:42:44.000000 vdk-server-0.1.927572457/src/vdk/plugin/server/installer.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-07-11 12:42:44.000000 vdk-server-0.1.927572457/src/vdk/plugin/server/kind-cluster-config-template.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-11 12:42:44.000000 vdk-server-0.1.927572457/src/vdk/plugin/server/server_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-07-11 12:42:44.000000 vdk-server-0.1.927572457/src/vdk/plugin/server/server_plugin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:43:00.486867 vdk-server-0.1.927572457/src/vdk_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      992 2023-07-11 12:43:00.000000 vdk-server-0.1.927572457/src/vdk_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-11 12:43:00.000000 vdk-server-0.1.927572457/src/vdk_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 12:43:00.000000 vdk-server-0.1.927572457/src/vdk_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-11 12:43:00.000000 vdk-server-0.1.927572457/src/vdk_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-11 12:43:00.000000 vdk-server-0.1.927572457/src/vdk_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-11 12:43:00.000000 vdk-server-0.1.927572457/src/vdk_server.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:43:00.486867 vdk-server-0.1.927572457/tests/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-07-11 12:42:44.000000 vdk-server-0.1.927572457/tests/test_plugin_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:23.410719 vdk-server-0.1.948436673/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-28 09:43:01.000000 vdk-server-0.1.948436673/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      992 2023-07-28 09:43:23.410719 vdk-server-0.1.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      374 2023-07-28 09:43:01.000000 vdk-server-0.1.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:43:23.410719 vdk-server-0.1.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-07-28 09:43:10.000000 vdk-server-0.1.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:23.402719 vdk-server-0.1.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:23.402719 vdk-server-0.1.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:23.402719 vdk-server-0.1.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:23.406720 vdk-server-0.1.948436673/src/vdk/plugin/server/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-28 09:43:01.000000 vdk-server-0.1.948436673/src/vdk/plugin/server/configmap-local-registry-hosting-template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    20085 2023-07-28 09:43:01.000000 vdk-server-0.1.948436673/src/vdk/plugin/server/ingress-nginx-deploy.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    33435 2023-07-28 09:43:01.000000 vdk-server-0.1.948436673/src/vdk/plugin/server/installer.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-07-28 09:43:01.000000 vdk-server-0.1.948436673/src/vdk/plugin/server/kind-cluster-config-template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-28 09:43:01.000000 vdk-server-0.1.948436673/src/vdk/plugin/server/server_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-07-28 09:43:01.000000 vdk-server-0.1.948436673/src/vdk/plugin/server/server_plugin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:23.406720 vdk-server-0.1.948436673/src/vdk_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      992 2023-07-28 09:43:23.000000 vdk-server-0.1.948436673/src/vdk_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-28 09:43:23.000000 vdk-server-0.1.948436673/src/vdk_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:43:23.000000 vdk-server-0.1.948436673/src/vdk_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-28 09:43:23.000000 vdk-server-0.1.948436673/src/vdk_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-28 09:43:23.000000 vdk-server-0.1.948436673/src/vdk_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:43:23.000000 vdk-server-0.1.948436673/src/vdk_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:23.410719 vdk-server-0.1.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-07-28 09:43:01.000000 vdk-server-0.1.948436673/tests/test_plugin_template.py
```

### Comparing `vdk-server-0.1.927572457/PKG-INFO` & `vdk-server-0.1.948436673/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-server
-Version: 0.1.927572457
+Version: 0.1.948436673
 Summary: Versatile Data Kit SDK plugin that facilitates the installation of a local Control Service.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-server-0.1.927572457/setup.py` & `vdk-server-0.1.948436673/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.1.927572457"
+__version__ = "0.1.948436673"
 
 setuptools.setup(
     name="vdk-server",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin that facilitates the installation of a local Control Service.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-server-0.1.927572457/src/vdk/plugin/server/ingress-nginx-deploy.yaml` & `vdk-server-0.1.948436673/src/vdk/plugin/server/ingress-nginx-deploy.yaml`

 * *Files identical despite different names*

### Comparing `vdk-server-0.1.927572457/src/vdk/plugin/server/installer.py` & `vdk-server-0.1.948436673/src/vdk/plugin/server/installer.py`

 * *Files identical despite different names*

### Comparing `vdk-server-0.1.927572457/src/vdk/plugin/server/kind-cluster-config-template.yaml` & `vdk-server-0.1.948436673/src/vdk/plugin/server/kind-cluster-config-template.yaml`

 * *Files identical despite different names*

### Comparing `vdk-server-0.1.927572457/src/vdk/plugin/server/server_plugin.py` & `vdk-server-0.1.948436673/src/vdk/plugin/server/server_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-server-0.1.927572457/src/vdk/plugin/server/server_plugin_utils.py` & `vdk-server-0.1.948436673/src/vdk/plugin/server/server_plugin_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-server-0.1.927572457/src/vdk_server.egg-info/PKG-INFO` & `vdk-server-0.1.948436673/src/vdk_server.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-server
-Version: 0.1.927572457
+Version: 0.1.948436673
 Summary: Versatile Data Kit SDK plugin that facilitates the installation of a local Control Service.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-server-0.1.927572457/src/vdk_server.egg-info/SOURCES.txt` & `vdk-server-0.1.948436673/src/vdk_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

