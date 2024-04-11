# Comparing `tmp/scalifiai-client-1.3.0a7.tar.gz` & `tmp/scalifiai-client-1.3.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalifiai-client-1.3.0a7.tar", last modified: Sat Apr  6 17:51:26 2024, max compression
+gzip compressed data, was "scalifiai-client-1.3.0a8.tar", last modified: Thu Apr 11 12:19:43 2024, max compression
```

## Comparing `scalifiai-client-1.3.0a7.tar` & `scalifiai-client-1.3.0a8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 17:51:26.406289 scalifiai-client-1.3.0a7/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/LICENSE
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1299 2024-04-06 17:51:26.406289 scalifiai-client-1.3.0a7/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/README.md
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1194 2024-04-06 17:51:07.000000 scalifiai-client-1.3.0a7/pyproject.toml
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 17:51:26.390289 scalifiai-client-1.3.0a7/scalifiai/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6439 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/credentials.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 17:51:26.390289 scalifiai-client-1.3.0a7/scalifiai/mcs/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 17:51:26.394289 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-06 12:51:10.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 17:51:26.394289 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/keras/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/keras/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       24 2024-04-06 12:51:24.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/keras/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/keras/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8462 2024-04-06 14:18:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/keras/main.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 17:51:26.394289 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/pytorch/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 12:49:28.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/pytorch/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       26 2024-04-06 12:51:17.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/pytorch/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5657 2024-04-06 12:58:51.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/pytorch/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     7877 2024-04-06 17:51:01.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/pytorch/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/schema.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2576 2024-04-06 14:22:40.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/utils.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/main.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 17:51:26.398289 scalifiai-client-1.3.0a7/scalifiai/mcs/metadata/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/metadata/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/metadata/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/metadata/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13424 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/metadata/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/metadata/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 17:51:26.398289 scalifiai-client-1.3.0a7/scalifiai/mcs/model/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/model/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/model/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/model/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    34065 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/model/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/model/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 17:51:26.398289 scalifiai-client-1.3.0a7/scalifiai/mcs/model_version/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/model_version/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/model_version/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/model_version/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28720 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/model_version/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/mcs/model_version/schemas.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a7/scalifiai/request_manager.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 17:51:26.402289 scalifiai-client-1.3.0a7/scalifiai_client.egg-info/
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1299 2024-04-06 17:51:26.000000 scalifiai-client-1.3.0a7/scalifiai_client.egg-info/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1570 2024-04-06 17:51:26.000000 scalifiai-client-1.3.0a7/scalifiai_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-06 17:51:26.000000 scalifiai-client-1.3.0a7/scalifiai_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      282 2024-04-06 17:51:26.000000 scalifiai-client-1.3.0a7/scalifiai_client.egg-info/requires.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-06 17:51:26.000000 scalifiai-client-1.3.0a7/scalifiai_client.egg-info/top_level.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-06 17:51:26.406289 scalifiai-client-1.3.0a7/setup.cfg
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-11 12:19:43.598804 scalifiai-client-1.3.0a8/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/LICENSE
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1299 2024-04-11 12:19:43.598804 scalifiai-client-1.3.0a8/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/README.md
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1194 2024-04-11 12:19:13.000000 scalifiai-client-1.3.0a8/pyproject.toml
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-11 12:19:43.586804 scalifiai-client-1.3.0a8/scalifiai/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6439 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/credentials.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-11 12:19:43.586804 scalifiai-client-1.3.0a8/scalifiai/mcs/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-11 12:19:43.590804 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       39 2024-04-11 09:53:31.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-11 12:19:43.590804 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/keras/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/keras/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       24 2024-04-06 12:51:24.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/keras/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/keras/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8444 2024-04-11 09:53:31.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/keras/main.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-11 12:19:43.590804 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/pytorch/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 12:49:28.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/pytorch/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       26 2024-04-06 12:51:17.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/pytorch/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5657 2024-04-06 12:58:51.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/pytorch/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8176 2024-04-11 12:19:25.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/pytorch/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/schema.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2577 2024-04-11 09:53:31.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/utils.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/main.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-11 12:19:43.590804 scalifiai-client-1.3.0a8/scalifiai/mcs/metadata/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/metadata/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/metadata/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/metadata/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13424 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/metadata/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/metadata/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-11 12:19:43.594804 scalifiai-client-1.3.0a8/scalifiai/mcs/model/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/model/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/model/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/model/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    34065 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/model/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/model/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-11 12:19:43.594804 scalifiai-client-1.3.0a8/scalifiai/mcs/model_version/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/model_version/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/model_version/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/model_version/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28720 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/model_version/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/mcs/model_version/schemas.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a8/scalifiai/request_manager.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-11 12:19:43.594804 scalifiai-client-1.3.0a8/scalifiai_client.egg-info/
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1299 2024-04-11 12:19:43.000000 scalifiai-client-1.3.0a8/scalifiai_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1570 2024-04-11 12:19:43.000000 scalifiai-client-1.3.0a8/scalifiai_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-11 12:19:43.000000 scalifiai-client-1.3.0a8/scalifiai_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      282 2024-04-11 12:19:43.000000 scalifiai-client-1.3.0a8/scalifiai_client.egg-info/requires.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-11 12:19:43.000000 scalifiai-client-1.3.0a8/scalifiai_client.egg-info/top_level.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-11 12:19:43.598804 scalifiai-client-1.3.0a8/setup.cfg
```

### Comparing `scalifiai-client-1.3.0a7/PKG-INFO` & `scalifiai-client-1.3.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.3.0a7
+Version: 1.3.0a8
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scalifiai-client-1.3.0a7/pyproject.toml` & `scalifiai-client-1.3.0a8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scalifiai-client"
-version = "1.3.0-alpha.7"
+version = "1.3.0-alpha.8"
 description = "SCALIFI AI NO CODE PLATFORM"
 readme = "README.md"
 authors = [{ name = "Scalifi Ai", email = "helpdesk@scalifiai.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `scalifiai-client-1.3.0a7/scalifiai/base.py` & `scalifiai-client-1.3.0a8/scalifiai/base.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/credentials.py` & `scalifiai-client-1.3.0a8/scalifiai/credentials.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/exceptions.py` & `scalifiai-client-1.3.0a8/scalifiai/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/exceptions.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/exceptions.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/keras/exceptions.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/keras/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/keras/main.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/keras/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,17 +52,19 @@
 
     @classmethod
     def check_model_instance(cls, *, model_instance):
 
         try:
             import tensorflow as tf
         except Exception:
-            print("Skipping Tensorflow check as Tensorflow installation is not detected")
+            print(
+                "Skipping Tensorflow check as Tensorflow installation is not detected"
+            )
             return False
-        
+
         return isinstance(model_instance, tf.keras.Model)
 
     def infer_data_type(self, *, dtype):
 
         data_type = self.DATA_TYPE_CONVERSION.get(dtype, None)
 
         if data_type == None:
@@ -158,18 +160,16 @@
                 try:
                     raise KerasInvalidModelException(extra_info=str(ex))
                 except Exception as ex:
                     raise KerasInvalidModelException()
 
             self.signature = self.infer_signature()
 
-            total_files_size, files_relative_paths, files_data = (
-                get_all_files_and_size(
-                    search_dir_path=model_save_file_path, base_path=model_save_file_path
-                )
+            total_files_size, files_relative_paths, files_data = get_all_files_and_size(
+                search_dir_path=model_save_file_path, base_path=model_save_file_path
             )
 
             create_version_request_body = {
                 "framework": self.framework_key,
                 "variation_name": variation,
                 "config": {
                     "total_files_size": total_files_size,
```

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/pytorch/exceptions.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/pytorch/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/pytorch/main.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/pytorch/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,40 +2,45 @@
 from pathlib import Path
 
 from scalifiai.mcs.frameworks.base import ModelWrapper
 from scalifiai.mcs.frameworks.constants import MODEL_SAVE_FOLDER_NAME
 from scalifiai.mcs.model.exceptions import (
     raise_custom_exception as raise_custom_exception__model,
 )
-from .exceptions import PytorchInvalidDataTypeModelException, PytorchInvalidModelException
+from .exceptions import (
+    PytorchInvalidDataTypeModelException,
+    PytorchInvalidModelException,
+)
 from .constants import FRAMEWORK_KEY
 
 
 # TODO[VIMPORTANT] SEGREGATE `ModelWrapper` class into deep learning and machine learning wrapper class and model following function to appropriate model class: [infer_data_type, infer_signature, serialize_signature]
 class PytorchModelWrapper(ModelWrapper):
 
     framework_key = FRAMEWORK_KEY
 
     # TODO[VIMPORTANT] CHECK AND MAKE FUNCTIONS PRIVATE IF THEY SHOULD NOT BE ACCESSIBLE DIRECTLY
 
     def __init__(self, *, model=None) -> None:
         # TODO[VIMPORTANT] MAKE A FUNCTION FOR IMPORTING DEPENDENT LIBRARIES FOR EACH FRAMEWORK IN THEIR CLASS AND USE THAT FUNCTION OR ELSE RAISE ERROR WITH PROPER INSTALLATION MENTIONED VIA OUR LIBRARY ONLY VIA OTHER DEPENDENCIEZS IN project.toml FILE
 
         super().__init__(model=model)
-        self.DATA_TYPE_CONVERSION = {} # TODO[VIMPORTANT] ONCE SIGNATURE CREATION IS COMPLETED, ADD ALL APPROPRIATE DATA TYPES. TAKE REFERENCE FROM KERAS DIR.
+        self.DATA_TYPE_CONVERSION = (
+            {}
+        )  # TODO[VIMPORTANT] ONCE SIGNATURE CREATION IS COMPLETED, ADD ALL APPROPRIATE DATA TYPES. TAKE REFERENCE FROM KERAS DIR.
 
     @classmethod
     def check_model_instance(cls, *, model_instance):
 
         try:
             import torch
         except Exception:
             print("Skipping Pytorch check as Pytorch installation is not detected")
             return False
-        
+
         return isinstance(model_instance, torch.nn.Module)
 
     def infer_data_type(self, *, dtype):
 
         data_type = self.DATA_TYPE_CONVERSION.get(dtype, None)
 
         if data_type == None:
@@ -87,19 +92,27 @@
         return signature
 
     def get_total_params(self):
 
         return {
             "trainable": {
                 "verbose": "Trainable",
-                "value": int(sum(p.numel() for p in self.model.parameters() if p.requires_grad)),
+                "value": int(
+                    sum(p.numel() for p in self.model.parameters() if p.requires_grad)
+                ),
             },
             "non_trainable": {
                 "verbose": "Non-trainable",
-                "value": int(sum(p.numel() for p in self.model.parameters() if not p.requires_grad)),
+                "value": int(
+                    sum(
+                        p.numel()
+                        for p in self.model.parameters()
+                        if not p.requires_grad
+                    )
+                ),
             },
         }
 
     def save_and_upload(
         self,
         *,
         base_dir_path=None,
@@ -119,29 +132,29 @@
             temp_dir_path = Path(temp_dir)
             model_save_file_path = temp_dir_path / Path(MODEL_SAVE_FOLDER_NAME)
 
             if not model_save_file_path.exists():
                 model_save_file_path.mkdir()
 
             try:
-                torch.jit.script(self.model).save(f"{model_save_file_path.absolute()}/model.pt")
+                torch.jit.script(self.model).save(
+                    f"{model_save_file_path.absolute()}/model.pt"
+                )
             except Exception as ex:
                 print(f"type(ex): {type(ex)}")
                 print(f"ex: {ex}")
                 try:
                     raise PytorchInvalidModelException(extra_info=str(ex))
                 except Exception as ex:
                     raise PytorchInvalidModelException()
 
             self.signature = self.infer_signature()
 
-            total_files_size, files_relative_paths, files_data = (
-                get_all_files_and_size(
-                    search_dir_path=model_save_file_path, base_path=model_save_file_path
-                )
+            total_files_size, files_relative_paths, files_data = get_all_files_and_size(
+                search_dir_path=model_save_file_path, base_path=model_save_file_path
             )
 
             create_version_request_body = {
                 "framework": self.framework_key,
                 "variation_name": variation,
                 "config": {
                     "total_files_size": total_files_size,
@@ -196,17 +209,19 @@
 
     # TODO[VIMPORTANT] COMPLETE FUNCTION AFTER TESTING
     @classmethod
     def load_local_model(cls, *, model_path=None):
         # TODO[VIMPORTANT] MAKE A FUNCTION FOR IMPORTING DEPENDENT LIBRARIES FOR EACH FRAMEWORK IN THEIR CLASS AND USE THAT FUNCTION OR ELSE RAISE ERROR WITH PROPER INSTALLATION MENTIONED VIA OUR LIBRARY ONLY VIA OTHER DEPENDENCIEZS IN project.toml FILE
         import torch
 
-        model_file = next((item for item in model_path.iterdir() if item.is_file()), None)
+        model_file = next(
+            (item for item in model_path.iterdir() if item.is_file()), None
+        )
 
         if model_file == None:
             raise PytorchInvalidModelException(extra_info="No valid model file found")
 
         print(f"type(model_file.absolute()): {type(model_file.absolute())}")
         print(f"model_file.absolute(): {model_file.absolute()}")
+        print(f"str(model_file.absolute()): {str(model_file.absolute())}")
 
-        return torch.jit.load(model_file.absolute())
-
+        return torch.jit.load(str(model_file.absolute()))
```

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/schema.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/schema.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/frameworks/utils.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/frameworks/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     framework = Framework.match_key(key)
 
     if framework == None:
         raise ModelFrameworkNotSupportedException()
 
     return framework
 
+
 def get_all_files_and_size(search_dir_path=None, base_path=None):
     files_relative_paths = []
     files_data = []
     total_size = 0
     for dirpath, _, filenames in os.walk(search_dir_path):
         for filename in filenames:
             file_path = os.path.join(dirpath, filename)
```

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/main.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/metadata/exceptions.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/metadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/metadata/main.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/metadata/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/metadata/schemas.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/metadata/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/model/constants.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/model/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/model/exceptions.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/model/main.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/model/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/model/schemas.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/model/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/model_version/constants.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/model_version/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/model_version/exceptions.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/model_version/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/model_version/main.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/model_version/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/mcs/model_version/schemas.py` & `scalifiai-client-1.3.0a8/scalifiai/mcs/model_version/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai/request_manager.py` & `scalifiai-client-1.3.0a8/scalifiai/request_manager.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a7/scalifiai_client.egg-info/PKG-INFO` & `scalifiai-client-1.3.0a8/scalifiai_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.3.0a7
+Version: 1.3.0a8
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scalifiai-client-1.3.0a7/scalifiai_client.egg-info/SOURCES.txt` & `scalifiai-client-1.3.0a8/scalifiai_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

