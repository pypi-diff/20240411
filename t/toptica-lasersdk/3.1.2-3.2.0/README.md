# Comparing `tmp/toptica_lasersdk-3.1.2.tar.gz` & `tmp/toptica_lasersdk-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toptica_lasersdk-3.1.2.tar", last modified: Thu Nov 23 15:57:40 2023, max compression
+gzip compressed data, was "toptica_lasersdk-3.2.0.tar", last modified: Thu Apr 11 08:22:24 2024, max compression
```

## Comparing `toptica_lasersdk-3.1.2.tar` & `toptica_lasersdk-3.2.0.tar`

### file list

```diff
@@ -1,97 +1,114 @@
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:40.535209 toptica_lasersdk-3.1.2/
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     1064 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/LICENSE.txt
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)       42 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/MANIFEST.in
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1259 2023-11-23 15:57:40.535209 toptica_lasersdk-3.1.2/PKG-INFO
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)      187 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/README.rst
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)        6 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/VERSION
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)       67 2023-11-23 15:57:40.539209 toptica_lasersdk-3.1.2/setup.cfg
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     1896 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/setup.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:40.491208 toptica_lasersdk-3.1.2/toptica/
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)       56 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/toptica/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:40.495208 toptica_lasersdk-3.1.2/toptica/lasersdk/
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:40.495208 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)    44822 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/client.py
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)    23646 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/connection.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:40.511208 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:21.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   170620 2023-11-23 15:57:15.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_4_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   171562 2023-11-23 15:57:15.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_5_1.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   232612 2023-11-23 15:57:15.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_6_1.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   233786 2023-11-23 15:57:16.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_6_3.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   246622 2023-11-23 15:57:16.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_7_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   248966 2023-11-23 15:57:16.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_8_1.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   261310 2023-11-23 15:57:17.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_9_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   263226 2023-11-23 15:57:17.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_0_1.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   263226 2023-11-23 15:57:17.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_0_3.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   291029 2023-11-23 15:57:17.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_1_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   299100 2023-11-23 15:57:18.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_2_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   300760 2023-11-23 15:57:18.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_3_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   303631 2023-11-23 15:57:18.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_3_2.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   304057 2023-11-23 15:57:19.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_3_4.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   303276 2023-11-23 15:57:19.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_4_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   321937 2023-11-23 15:57:19.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_5_2.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   321937 2023-11-23 15:57:20.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_5_3.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   321937 2023-11-23 15:57:20.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_5_4.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   332388 2023-11-23 15:57:20.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_6_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   332545 2023-11-23 15:57:21.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_7_2.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   349569 2023-11-23 15:57:21.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v3_0_1.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:40.515208 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_cle/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:22.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_cle/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    40587 2023-11-23 15:57:21.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_cle/v1_0_8.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    40758 2023-11-23 15:57:22.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_cle/v1_1_3.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    42285 2023-11-23 15:57:22.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_cle/v2_2_5.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:40.515208 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_mle/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:22.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_mle/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    51223 2023-11-23 15:57:22.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_mle/v1_8_1.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    51223 2023-11-23 15:57:22.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_mle/v2_2_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    51223 2023-11-23 15:57:23.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_mle/v2_3_1.py
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)    47226 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/client.py
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)    23491 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/decop.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:40.531209 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:13.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   169451 2023-11-23 15:57:07.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_4_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   170417 2023-11-23 15:57:07.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_5_1.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   231311 2023-11-23 15:57:07.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_6_1.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   232485 2023-11-23 15:57:08.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_6_3.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   245153 2023-11-23 15:57:08.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_7_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   247353 2023-11-23 15:57:08.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_8_1.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   259577 2023-11-23 15:57:08.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_9_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   261505 2023-11-23 15:57:09.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_0_1.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   261505 2023-11-23 15:57:09.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_0_3.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   289092 2023-11-23 15:57:09.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_1_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   297139 2023-11-23 15:57:10.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_2_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   298763 2023-11-23 15:57:10.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_3_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   301610 2023-11-23 15:57:10.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_3_2.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   302024 2023-11-23 15:57:11.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_3_4.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   301279 2023-11-23 15:57:11.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_4_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   319772 2023-11-23 15:57:11.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_5_2.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   319772 2023-11-23 15:57:12.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_5_3.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   319772 2023-11-23 15:57:12.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_5_4.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   330187 2023-11-23 15:57:12.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_6_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   330344 2023-11-23 15:57:13.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_7_2.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   347248 2023-11-23 15:57:13.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v3_0_1.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:40.535209 toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_cle/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:14.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_cle/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    39626 2023-11-23 15:57:13.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_cle/v1_0_8.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    39797 2023-11-23 15:57:14.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_cle/v1_1_3.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    41324 2023-11-23 15:57:14.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_cle/v2_2_5.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:40.535209 toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_mle/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:14.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_mle/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    49974 2023-11-23 15:57:14.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_mle/v1_8_1.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    49974 2023-11-23 15:57:14.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_mle/v2_2_0.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    49974 2023-11-23 15:57:15.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_mle/v2_3_1.py
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)    39377 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/lasersdk_gen.py
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/py.typed
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:40.535209 toptica_lasersdk-3.1.2/toptica/lasersdk/utils/
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/utils/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     7705 2023-11-23 15:56:53.000000 toptica_lasersdk-3.1.2/toptica/lasersdk/utils/dlcpro.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-11-23 15:57:40.535209 toptica_lasersdk-3.1.2/toptica_lasersdk.egg-info/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1259 2023-11-23 15:57:40.000000 toptica_lasersdk-3.1.2/toptica_lasersdk.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3064 2023-11-23 15:57:40.000000 toptica_lasersdk-3.1.2/toptica_lasersdk.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2023-11-23 15:57:40.000000 toptica_lasersdk-3.1.2/toptica_lasersdk.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       69 2023-11-23 15:57:40.000000 toptica_lasersdk-3.1.2/toptica_lasersdk.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        8 2023-11-23 15:57:40.000000 toptica_lasersdk-3.1.2/toptica_lasersdk.egg-info/namespace_packages.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       16 2023-11-23 15:57:40.000000 toptica_lasersdk-3.1.2/toptica_lasersdk.egg-info/requires.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        8 2023-11-23 15:57:40.000000 toptica_lasersdk-3.1.2/toptica_lasersdk.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:24.487754 toptica_lasersdk-3.2.0/
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     1064 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/LICENSE.txt
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)       42 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1285 2024-04-11 08:22:24.487754 toptica_lasersdk-3.2.0/PKG-INFO
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)      187 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/README.rst
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)        6 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/VERSION
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)       67 2024-04-11 08:22:24.487754 toptica_lasersdk-3.2.0/setup.cfg
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     1896 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/setup.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:24.435753 toptica_lasersdk-3.2.0/tests/
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)    20746 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/tests/test_async_client.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)    19633 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/tests/test_client.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     3612 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/tests/test_client_subscription.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     4952 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/tests/test_client_subscription_async.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     6498 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/tests/test_client_types.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     6719 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/tests/test_client_types_async.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     8576 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/tests/test_connection.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     5102 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/tests/test_decop.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     9222 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/tests/test_decop_decode_value_inferred.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     2533 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/tests/test_dlcpro.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     1289 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/tests/test_dlcpro_utils.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     2442 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/tests/test_lasersdk_gen_commandline.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:24.435753 toptica_lasersdk-3.2.0/toptica/
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)       56 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/toptica/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:24.435753 toptica_lasersdk-3.2.0/toptica/lasersdk/
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:24.435753 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)    44822 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/client.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)    23646 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/connection.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:24.455754 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:01.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   170620 2024-04-11 08:21:52.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_4_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   171562 2024-04-11 08:21:52.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_5_1.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   232612 2024-04-11 08:21:53.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_6_1.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   233786 2024-04-11 08:21:53.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_6_3.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   246622 2024-04-11 08:21:53.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_7_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   248966 2024-04-11 08:21:54.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_8_1.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   261310 2024-04-11 08:21:54.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_9_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   263226 2024-04-11 08:21:55.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_0_1.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   263226 2024-04-11 08:21:55.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_0_3.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   291029 2024-04-11 08:21:56.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_1_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   299100 2024-04-11 08:21:56.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_2_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   300760 2024-04-11 08:21:57.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_3_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   303631 2024-04-11 08:21:57.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_3_2.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   304057 2024-04-11 08:21:57.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_3_4.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   303276 2024-04-11 08:21:58.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_4_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   321937 2024-04-11 08:21:58.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_5_2.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   321937 2024-04-11 08:21:59.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_5_3.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   321937 2024-04-11 08:21:59.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_5_4.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   332388 2024-04-11 08:22:00.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_6_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   332545 2024-04-11 08:22:00.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_7_2.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   349569 2024-04-11 08:22:01.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v3_0_1.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   352483 2024-04-11 08:22:01.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v3_1_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   363741 2024-04-11 08:22:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v3_2_0.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:24.459754 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_cle/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_cle/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    40587 2024-04-11 08:22:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_cle/v1_0_8.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    40758 2024-04-11 08:22:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_cle/v1_1_3.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    42285 2024-04-11 08:22:03.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_cle/v2_2_5.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:24.459754 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_mle/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:04.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_mle/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    51223 2024-04-11 08:22:03.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_mle/v1_8_1.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    51223 2024-04-11 08:22:04.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_mle/v2_2_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    51223 2024-04-11 08:22:04.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_mle/v2_3_1.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)    47226 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/client.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)    23491 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/decop.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:24.479754 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:21:49.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   169451 2024-04-11 08:21:40.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_4_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   170417 2024-04-11 08:21:40.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_5_1.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   231311 2024-04-11 08:21:40.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_6_1.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   232485 2024-04-11 08:21:41.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_6_3.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   245153 2024-04-11 08:21:41.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_7_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   247353 2024-04-11 08:21:42.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_8_1.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   259577 2024-04-11 08:21:42.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_9_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   261505 2024-04-11 08:21:43.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_0_1.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   261505 2024-04-11 08:21:43.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_0_3.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   289092 2024-04-11 08:21:43.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_1_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   297139 2024-04-11 08:21:44.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_2_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   298763 2024-04-11 08:21:44.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_3_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   301610 2024-04-11 08:21:45.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_3_2.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   302024 2024-04-11 08:21:45.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_3_4.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   301279 2024-04-11 08:21:46.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_4_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   319772 2024-04-11 08:21:46.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_5_2.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   319772 2024-04-11 08:21:46.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_5_3.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   319772 2024-04-11 08:21:47.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_5_4.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   330187 2024-04-11 08:21:47.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_6_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   330344 2024-04-11 08:21:48.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_7_2.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   347248 2024-04-11 08:21:48.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v3_0_1.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   350150 2024-04-11 08:21:49.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v3_1_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   361396 2024-04-11 08:21:49.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v3_2_0.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:24.483754 toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_cle/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:21:50.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_cle/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    39626 2024-04-11 08:21:50.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_cle/v1_0_8.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    39797 2024-04-11 08:21:50.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_cle/v1_1_3.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    41324 2024-04-11 08:21:50.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_cle/v2_2_5.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:24.483754 toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_mle/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:21:51.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_mle/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    49974 2024-04-11 08:21:51.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_mle/v1_8_1.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    49974 2024-04-11 08:21:51.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_mle/v2_2_0.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    49974 2024-04-11 08:21:51.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_mle/v2_3_1.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)    39377 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/lasersdk_gen.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/py.typed
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:24.483754 toptica_lasersdk-3.2.0/toptica/lasersdk/utils/
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/utils/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins   (2000)     7705 2024-04-11 08:21:02.000000 toptica_lasersdk-3.2.0/toptica/lasersdk/utils/dlcpro.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 08:22:24.487754 toptica_lasersdk-3.2.0/toptica_lasersdk.egg-info/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1285 2024-04-11 08:22:24.000000 toptica_lasersdk-3.2.0/toptica_lasersdk.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3572 2024-04-11 08:22:24.000000 toptica_lasersdk-3.2.0/toptica_lasersdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2024-04-11 08:22:24.000000 toptica_lasersdk-3.2.0/toptica_lasersdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       68 2024-04-11 08:22:24.000000 toptica_lasersdk-3.2.0/toptica_lasersdk.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        8 2024-04-11 08:22:24.000000 toptica_lasersdk-3.2.0/toptica_lasersdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       16 2024-04-11 08:22:24.000000 toptica_lasersdk-3.2.0/toptica_lasersdk.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        8 2024-04-11 08:22:24.000000 toptica_lasersdk-3.2.0/toptica_lasersdk.egg-info/top_level.txt
```

### Comparing `toptica_lasersdk-3.1.2/LICENSE.txt` & `toptica_lasersdk-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `toptica_lasersdk-3.1.2/PKG-INFO` & `toptica_lasersdk-3.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: toptica_lasersdk
-Version: 3.1.2
+Version: 3.2.0
 Summary: TOPTICA Python Laser SDK
 Home-page: https://toptica.github.io/python-lasersdk/
 Author: TOPTICA Photonics AG
 Author-email: info@toptica.com
 License: MIT
 Keywords: toptica photonics laser sdk dlcpro ichrome cle mle
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -20,14 +19,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6,<4
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: ifaddr
+Requires-Dist: pyserial
 
 TOPTICA Python Laser SDK
 ========================
 
 The **TOPTICA Python Laser SDK** allows for the easy control of TOPTICA laser products from a PC using the Python programming language.
-
-
```

### Comparing `toptica_lasersdk-3.1.2/setup.py` & `toptica_lasersdk-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/client.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/connection.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/connection.py`

 * *Files identical despite different names*

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_4_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_4_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_4_0.xml' on 2023-11-23 15:57:15.264594
+# Generated from 'v1_4_0.xml' on 2024-04-11 08:21:52.311719
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_5_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_5_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_5_1.xml' on 2023-11-23 15:57:15.538426
+# Generated from 'v1_5_1.xml' on 2024-04-11 08:21:52.710534
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_6_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_6_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_6_1.xml' on 2023-11-23 15:57:15.822816
+# Generated from 'v1_6_1.xml' on 2024-04-11 08:21:53.105877
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_6_3.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_6_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_6_3.xml' on 2023-11-23 15:57:16.118422
+# Generated from 'v1_6_3.xml' on 2024-04-11 08:21:53.510665
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_7_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_7_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_7_0.xml' on 2023-11-23 15:57:16.441125
+# Generated from 'v1_7_0.xml' on 2024-04-11 08:21:53.948693
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_8_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_8_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_8_1.xml' on 2023-11-23 15:57:16.736819
+# Generated from 'v1_8_1.xml' on 2024-04-11 08:21:54.389704
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v1_9_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v1_9_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_9_0.xml' on 2023-11-23 15:57:17.060208
+# Generated from 'v1_9_0.xml' on 2024-04-11 08:21:54.791471
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_0_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_0_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_0_1.xml' on 2023-11-23 15:57:17.353780
+# Generated from 'v2_0_1.xml' on 2024-04-11 08:21:55.201619
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_0_3.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_0_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_0_3.xml' on 2023-11-23 15:57:17.647804
+# Generated from 'v2_0_3.xml' on 2024-04-11 08:21:55.612741
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_1_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_1_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_1_0.xml' on 2023-11-23 15:57:17.949797
+# Generated from 'v2_1_0.xml' on 2024-04-11 08:21:56.098259
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_2_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_2_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_2_0.xml' on 2023-11-23 15:57:18.257333
+# Generated from 'v2_2_0.xml' on 2024-04-11 08:21:56.567139
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_3_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_3_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_3_0.xml' on 2023-11-23 15:57:18.557964
+# Generated from 'v2_3_0.xml' on 2024-04-11 08:21:57.004372
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_3_2.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_3_4.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_3_2.xml' on 2023-11-23 15:57:18.899226
+# Generated from 'v2_3_4.xml' on 2024-04-11 08:21:57.861493
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
 
@@ -3701,14 +3701,15 @@
         self.__name = name
         self._serial_number = MutableDecopString(client, name + ':serial-number')
         self._status = DecopInteger(client, name + ':status')
         self._status_txt = DecopString(client, name + ':status-txt')
         self._wavelength_before_optimization = DecopReal(client, name + ':wavelength-before-optimization')
         self._wavelength_after_optimization = DecopReal(client, name + ':wavelength-after-optimization')
         self._wavelength_temp_coeff = DecopReal(client, name + ':wavelength-temp-coeff')
+        self._exposure_time = DecopInteger(client, name + ':exposure-time')
 
     @property
     def serial_number(self) -> 'MutableDecopString':
         return self._serial_number
 
     @property
     def status(self) -> 'DecopInteger':
@@ -3726,14 +3727,18 @@
     def wavelength_after_optimization(self) -> 'DecopReal':
         return self._wavelength_after_optimization
 
     @property
     def wavelength_temp_coeff(self) -> 'DecopReal':
         return self._wavelength_temp_coeff
 
+    @property
+    def exposure_time(self) -> 'DecopInteger':
+        return self._exposure_time
+
 
 class Shg:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._tc = TcChannel1(client, name + ':tc')
         self._cavity_tc = TcChannel1(client, name + ':cavity-tc')
@@ -9292,7 +9297,11 @@
         assert isinstance(password, str) or password is None, f"expected type 'str' or 'None' for parameter 'password', got '{type(password)}'"
         return await self.__client.change_ul(ul, password)
 
     async def change_password(self, password: str) -> None:
         assert isinstance(password, str), f"expected type 'str' for parameter 'password', got '{type(password)}'"
         await self.__client.exec('change-password', password)
 
+    async def change_password_service(self, password: str) -> None:
+        assert isinstance(password, str), f"expected type 'str' for parameter 'password', got '{type(password)}'"
+        await self.__client.exec('change-password-service', password)
+
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_3_4.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_4_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_3_4.xml' on 2023-11-23 15:57:19.225697
+# Generated from 'v2_4_0.xml' on 2024-04-11 08:21:58.312345
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
 
@@ -172,14 +172,15 @@
         self._tc = TcChannel1(client, name + ':tc')
         self._pc = PiezoDrv1(client, name + ':pc')
         self._lock = Lock(client, name + ':lock')
         self._pressure_compensation = PressureCompensation(client, name + ':pressure-compensation')
         self._pd = DlPd(client, name + ':pd')
         self._power_optimization = ScbPowerOptimization(client, name + ':power-optimization')
         self._servo = ServoControlServos(client, name + ':servo')
+        self._eom = PiezoDrv1(client, name + ':eom')
         self._factory_settings = LhFactory(client, name + ':factory-settings')
 
     @property
     def legacy(self) -> 'DecopBoolean':
         return self._legacy
 
     @property
@@ -239,14 +240,18 @@
         return self._power_optimization
 
     @property
     def servo(self) -> 'ServoControlServos':
         return self._servo
 
     @property
+    def eom(self) -> 'PiezoDrv1':
+        return self._eom
+
+    @property
     def factory_settings(self) -> 'LhFactory':
         return self._factory_settings
 
     async def store(self) -> None:
         await self.__client.exec(self.__name + ':store')
 
     async def restore(self) -> None:
@@ -1550,14 +1555,15 @@
         self.__name = name
         self._wavelength = MutableDecopReal(client, name + ':wavelength')
         self._threshold_current = MutableDecopReal(client, name + ':threshold-current')
         self._power = MutableDecopReal(client, name + ':power')
         self._cc = LhFactoryCc(client, name + ':cc')
         self._tc = TcFactorySettings(client, name + ':tc')
         self._pc = DlPcFactorySettings(client, name + ':pc')
+        self._eom = PcFactorySettings(client, name + ':eom')
         self._pd = DlPdFactorySettings(client, name + ':pd')
         self._last_modified = DecopString(client, name + ':last-modified')
         self._modified = DecopBoolean(client, name + ':modified')
 
     @property
     def wavelength(self) -> 'MutableDecopReal':
         return self._wavelength
@@ -1579,14 +1585,18 @@
         return self._tc
 
     @property
     def pc(self) -> 'DlPcFactorySettings':
         return self._pc
 
     @property
+    def eom(self) -> 'PcFactorySettings':
+        return self._eom
+
+    @property
     def pd(self) -> 'DlPdFactorySettings':
         return self._pd
 
     @property
     def last_modified(self) -> 'DecopString':
         return self._last_modified
 
@@ -1790,14 +1800,55 @@
         return self._slew_rate_enabled
 
     @property
     def pressure_compensation_factor(self) -> 'MutableDecopReal':
         return self._pressure_compensation_factor
 
 
+class PcFactorySettings:
+    def __init__(self, client: Client, name: str) -> None:
+        self.__client = client
+        self.__name = name
+        self._voltage_min = MutableDecopReal(client, name + ':voltage-min')
+        self._voltage_max = MutableDecopReal(client, name + ':voltage-max')
+        self._feedforward_enabled = MutableDecopBoolean(client, name + ':feedforward-enabled')
+        self._feedforward_factor = MutableDecopReal(client, name + ':feedforward-factor')
+        self._capacitance = MutableDecopReal(client, name + ':capacitance')
+        self._scan_offset = MutableDecopReal(client, name + ':scan-offset')
+        self._scan_amplitude = MutableDecopReal(client, name + ':scan-amplitude')
+
+    @property
+    def voltage_min(self) -> 'MutableDecopReal':
+        return self._voltage_min
+
+    @property
+    def voltage_max(self) -> 'MutableDecopReal':
+        return self._voltage_max
+
+    @property
+    def feedforward_enabled(self) -> 'MutableDecopBoolean':
+        return self._feedforward_enabled
+
+    @property
+    def feedforward_factor(self) -> 'MutableDecopReal':
+        return self._feedforward_factor
+
+    @property
+    def capacitance(self) -> 'MutableDecopReal':
+        return self._capacitance
+
+    @property
+    def scan_offset(self) -> 'MutableDecopReal':
+        return self._scan_offset
+
+    @property
+    def scan_amplitude(self) -> 'MutableDecopReal':
+        return self._scan_amplitude
+
+
 class DlPdFactorySettings:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._seed = PdCalFactorySettings(client, name + ':seed')
 
     @property
@@ -3478,15 +3529,14 @@
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._ongoing = DecopBoolean(client, name + ':ongoing')
         self._progress = DecopInteger(client, name + ':progress')
         self._status = DecopInteger(client, name + ':status')
         self._status_string = DecopString(client, name + ':status-string')
-        self._last_time_optimized = DecopString(client, name + ':last-time-optimized')
         self._shg_advanced = MutableDecopBoolean(client, name + ':shg-advanced')
         self._stage1 = NloStage1(client, name + ':stage1')
         self._stage2 = NloStage1(client, name + ':stage2')
         self._stage3 = NloStage1(client, name + ':stage3')
         self._stage4 = NloStage1(client, name + ':stage4')
         self._stage5 = NloStage1(client, name + ':stage5')
         self._progress_data_amp = DecopBinary(client, name + ':progress-data-amp')
@@ -3508,18 +3558,14 @@
         return self._status
 
     @property
     def status_string(self) -> 'DecopString':
         return self._status_string
 
     @property
-    def last_time_optimized(self) -> 'DecopString':
-        return self._last_time_optimized
-
-    @property
     def shg_advanced(self) -> 'MutableDecopBoolean':
         return self._shg_advanced
 
     @property
     def stage1(self) -> 'NloStage1':
         return self._stage1
 
@@ -3701,15 +3747,14 @@
         self.__name = name
         self._serial_number = MutableDecopString(client, name + ':serial-number')
         self._status = DecopInteger(client, name + ':status')
         self._status_txt = DecopString(client, name + ':status-txt')
         self._wavelength_before_optimization = DecopReal(client, name + ':wavelength-before-optimization')
         self._wavelength_after_optimization = DecopReal(client, name + ':wavelength-after-optimization')
         self._wavelength_temp_coeff = DecopReal(client, name + ':wavelength-temp-coeff')
-        self._exposure_time = DecopInteger(client, name + ':exposure-time')
 
     @property
     def serial_number(self) -> 'MutableDecopString':
         return self._serial_number
 
     @property
     def status(self) -> 'DecopInteger':
@@ -3727,18 +3772,14 @@
     def wavelength_after_optimization(self) -> 'DecopReal':
         return self._wavelength_after_optimization
 
     @property
     def wavelength_temp_coeff(self) -> 'DecopReal':
         return self._wavelength_temp_coeff
 
-    @property
-    def exposure_time(self) -> 'DecopInteger':
-        return self._exposure_time
-
 
 class Shg:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._tc = TcChannel1(client, name + ':tc')
         self._cavity_tc = TcChannel1(client, name + ':cavity-tc')
@@ -4017,57 +4058,37 @@
 class NloLaserHeadWindow1:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._input_channel = MutableDecopInteger(client, name + ':input-channel')
         self._threshold = MutableDecopReal(client, name + ':threshold')
         self._level_hysteresis = MutableDecopReal(client, name + ':level-hysteresis')
-        self._calibration = NloLaserHeadWindowCalibration2(client, name + ':calibration')
+        self._calibration = NloLaserHeadWindowCalibration1(client, name + ':calibration')
 
     @property
     def input_channel(self) -> 'MutableDecopInteger':
         return self._input_channel
 
     @property
     def threshold(self) -> 'MutableDecopReal':
         return self._threshold
 
     @property
     def level_hysteresis(self) -> 'MutableDecopReal':
         return self._level_hysteresis
 
     @property
-    def calibration(self) -> 'NloLaserHeadWindowCalibration2':
+    def calibration(self) -> 'NloLaserHeadWindowCalibration1':
         return self._calibration
 
 
-class NloLaserHeadWindowCalibration2:
+class NloLaserHeadWindowCalibration1:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
-        self._power_min = MutableDecopReal(client, name + ':power-min')
-        self._power_max = MutableDecopReal(client, name + ':power-max')
-        self._threshold_min = MutableDecopReal(client, name + ':threshold-min')
-        self._threshold_max = MutableDecopReal(client, name + ':threshold-max')
-
-    @property
-    def power_min(self) -> 'MutableDecopReal':
-        return self._power_min
-
-    @property
-    def power_max(self) -> 'MutableDecopReal':
-        return self._power_max
-
-    @property
-    def threshold_min(self) -> 'MutableDecopReal':
-        return self._threshold_min
-
-    @property
-    def threshold_max(self) -> 'MutableDecopReal':
-        return self._threshold_max
 
 
 class NloLaserHeadPid1:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._gain = NloLaserHeadGain1(client, name + ':gain')
@@ -6198,57 +6219,37 @@
 class NloLaserHeadWindow2:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._input_channel = DecopInteger(client, name + ':input-channel')
         self._threshold = DecopReal(client, name + ':threshold')
         self._level_hysteresis = DecopReal(client, name + ':level-hysteresis')
-        self._calibration = NloLaserHeadWindowCalibration1(client, name + ':calibration')
+        self._calibration = NloLaserHeadWindowCalibration2(client, name + ':calibration')
 
     @property
     def input_channel(self) -> 'DecopInteger':
         return self._input_channel
 
     @property
     def threshold(self) -> 'DecopReal':
         return self._threshold
 
     @property
     def level_hysteresis(self) -> 'DecopReal':
         return self._level_hysteresis
 
     @property
-    def calibration(self) -> 'NloLaserHeadWindowCalibration1':
+    def calibration(self) -> 'NloLaserHeadWindowCalibration2':
         return self._calibration
 
 
-class NloLaserHeadWindowCalibration1:
+class NloLaserHeadWindowCalibration2:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
-        self._power_min = DecopReal(client, name + ':power-min')
-        self._power_max = DecopReal(client, name + ':power-max')
-        self._threshold_min = DecopReal(client, name + ':threshold-min')
-        self._threshold_max = DecopReal(client, name + ':threshold-max')
-
-    @property
-    def power_min(self) -> 'DecopReal':
-        return self._power_min
-
-    @property
-    def power_max(self) -> 'DecopReal':
-        return self._power_max
-
-    @property
-    def threshold_min(self) -> 'DecopReal':
-        return self._threshold_min
-
-    @property
-    def threshold_max(self) -> 'DecopReal':
-        return self._threshold_max
 
 
 class NloLaserHeadPid2:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._gain = NloLaserHeadGain2(client, name + ':gain')
@@ -6718,32 +6719,53 @@
 
 
 class LaserDiagnosis:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._ready = DecopBoolean(client, name + ':ready')
+        self._options = LaserDiagnosisOptions(client, name + ':options')
 
     @property
     def ready(self) -> 'DecopBoolean':
         return self._ready
 
+    @property
+    def options(self) -> 'LaserDiagnosisOptions':
+        return self._options
+
     async def start(self) -> None:
         await self.__client.exec(self.__name + ':start')
 
     async def print_result(self) -> bytes:
         return await self.__client.exec(self.__name + ':print-result', output_type=bytes)
 
     async def execute(self) -> bytes:
         return await self.__client.exec(self.__name + ':execute', output_type=bytes)
 
     async def generate_to_usb(self) -> None:
         await self.__client.exec(self.__name + ':generate-to-usb')
 
 
+class LaserDiagnosisOptions:
+    def __init__(self, client: Client, name: str) -> None:
+        self.__client = client
+        self.__name = name
+        self._servo_test = MutableDecopBoolean(client, name + ':servo-test')
+        self._servo_stepsize = MutableDecopInteger(client, name + ':servo-stepsize')
+
+    @property
+    def servo_test(self) -> 'MutableDecopBoolean':
+        return self._servo_test
+
+    @property
+    def servo_stepsize(self) -> 'MutableDecopInteger':
+        return self._servo_stepsize
+
+
 class LaserComponents:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
 
 
 class LaserCommon:
@@ -6941,17 +6963,14 @@
         self._power_act = DecopReal(client, name + ':power-act')
         self._wavelength = DecopReal(client, name + ':wavelength')
         self._idle_mode = MutableDecopBoolean(client, name + ':idle-mode')
         self._wavemeter = AutoNloWavemeter(client, name + ':wavemeter')
         self._power_stabilization_settings = AutoNloPowerStabilizationSettings(client, name + ':power-stabilization-settings')
         self._optimization_settings = AutoNloOptimizationOptions(client, name + ':optimization-settings')
         self._optimization_progress = DecopInteger(client, name + ':optimization-progress')
-        self._last_time_auto_align = DecopString(client, name + ':last-time-auto-align')
-        self._last_time_single_mode_optimization = DecopString(client, name + ':last-time-single-mode-optimization')
-        self._single_mode_optimization_valid = DecopInteger(client, name + ':single-mode-optimization-valid')
 
     @property
     def automatic_mode(self) -> 'MutableDecopBoolean':
         return self._automatic_mode
 
     @property
     def serial_number(self) -> 'DecopString':
@@ -7109,26 +7128,14 @@
     def optimization_settings(self) -> 'AutoNloOptimizationOptions':
         return self._optimization_settings
 
     @property
     def optimization_progress(self) -> 'DecopInteger':
         return self._optimization_progress
 
-    @property
-    def last_time_auto_align(self) -> 'DecopString':
-        return self._last_time_auto_align
-
-    @property
-    def last_time_single_mode_optimization(self) -> 'DecopString':
-        return self._last_time_single_mode_optimization
-
-    @property
-    def single_mode_optimization_valid(self) -> 'DecopInteger':
-        return self._single_mode_optimization_valid
-
     async def perform_optimization(self) -> None:
         await self.__client.exec(self.__name + ':perform-optimization')
 
     async def reset_operation_time_cavity(self) -> None:
         await self.__client.exec(self.__name + ':reset-operation-time-cavity')
 
     async def clear_errors(self) -> None:
@@ -8035,48 +8042,26 @@
 
 
 class Buzzer:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._welcome = MutableDecopString(client, name + ':welcome')
-        self._sounds = BuzzerSounds(client, name + ':sounds')
 
     @property
     def welcome(self) -> 'MutableDecopString':
         return self._welcome
 
-    @property
-    def sounds(self) -> 'BuzzerSounds':
-        return self._sounds
-
     async def play_welcome(self) -> None:
         await self.__client.exec(self.__name + ':play-welcome')
 
     async def play(self, melody: str) -> None:
         assert isinstance(melody, str), f"expected type 'str' for parameter 'melody', got '{type(melody)}'"
         await self.__client.exec(self.__name + ':play', melody)
 
-    async def save(self) -> None:
-        await self.__client.exec(self.__name + ':save')
-
-    async def load(self) -> None:
-        await self.__client.exec(self.__name + ':load')
-
-
-class BuzzerSounds:
-    def __init__(self, client: Client, name: str) -> None:
-        self.__client = client
-        self.__name = name
-        self._on_connection = MutableDecopBoolean(client, name + ':on-connection')
-
-    @property
-    def on_connection(self) -> 'MutableDecopBoolean':
-        return self._on_connection
-
 
 class Display:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._brightness = MutableDecopReal(client, name + ':brightness')
         self._auto_dark = MutableDecopBoolean(client, name + ':auto-dark')
@@ -8112,35 +8097,35 @@
 
 class Standby:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._enabled = MutableDecopBoolean(client, name + ':enabled')
         self._state = DecopInteger(client, name + ':state')
-        self._laser1 = StandbyLaser(client, name + ':laser1')
+        self._laser1 = StandbyLaser1(client, name + ':laser1')
         self._laser2 = StandbyLaser2(client, name + ':laser2')
 
     @property
     def enabled(self) -> 'MutableDecopBoolean':
         return self._enabled
 
     @property
     def state(self) -> 'DecopInteger':
         return self._state
 
     @property
-    def laser1(self) -> 'StandbyLaser':
+    def laser1(self) -> 'StandbyLaser1':
         return self._laser1
 
     @property
     def laser2(self) -> 'StandbyLaser2':
         return self._laser2
 
 
-class StandbyLaser:
+class StandbyLaser1:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._dl = StandbyDl(client, name + ':dl')
         self._amp = StandbyAmp(client, name + ':amp')
         self._ctl = StandbyCtl(client, name + ':ctl')
         self._nlo = StandbyShg(client, name + ':nlo')
@@ -8242,19 +8227,24 @@
 
 
 class StandbyLaser2:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._dl = StandbyDl(client, name + ':dl')
+        self._amp = StandbyAmp(client, name + ':amp')
 
     @property
     def dl(self) -> 'StandbyDl':
         return self._dl
 
+    @property
+    def amp(self) -> 'StandbyAmp':
+        return self._amp
+
 
 class PdhBoard:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._slot = DecopString(client, name + ':slot')
         self._serial_number = DecopString(client, name + ':serial-number')
@@ -9297,11 +9287,7 @@
         assert isinstance(password, str) or password is None, f"expected type 'str' or 'None' for parameter 'password', got '{type(password)}'"
         return await self.__client.change_ul(ul, password)
 
     async def change_password(self, password: str) -> None:
         assert isinstance(password, str), f"expected type 'str' for parameter 'password', got '{type(password)}'"
         await self.__client.exec('change-password', password)
 
-    async def change_password_service(self, password: str) -> None:
-        assert isinstance(password, str), f"expected type 'str' for parameter 'password', got '{type(password)}'"
-        await self.__client.exec('change-password-service', password)
-
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_4_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_3_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_4_0.xml' on 2023-11-23 15:57:19.529200
+# Generated from 'v2_3_2.xml' on 2024-04-11 08:21:57.430620
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
 
@@ -172,15 +172,14 @@
         self._tc = TcChannel1(client, name + ':tc')
         self._pc = PiezoDrv1(client, name + ':pc')
         self._lock = Lock(client, name + ':lock')
         self._pressure_compensation = PressureCompensation(client, name + ':pressure-compensation')
         self._pd = DlPd(client, name + ':pd')
         self._power_optimization = ScbPowerOptimization(client, name + ':power-optimization')
         self._servo = ServoControlServos(client, name + ':servo')
-        self._eom = PiezoDrv1(client, name + ':eom')
         self._factory_settings = LhFactory(client, name + ':factory-settings')
 
     @property
     def legacy(self) -> 'DecopBoolean':
         return self._legacy
 
     @property
@@ -240,18 +239,14 @@
         return self._power_optimization
 
     @property
     def servo(self) -> 'ServoControlServos':
         return self._servo
 
     @property
-    def eom(self) -> 'PiezoDrv1':
-        return self._eom
-
-    @property
     def factory_settings(self) -> 'LhFactory':
         return self._factory_settings
 
     async def store(self) -> None:
         await self.__client.exec(self.__name + ':store')
 
     async def restore(self) -> None:
@@ -1555,15 +1550,14 @@
         self.__name = name
         self._wavelength = MutableDecopReal(client, name + ':wavelength')
         self._threshold_current = MutableDecopReal(client, name + ':threshold-current')
         self._power = MutableDecopReal(client, name + ':power')
         self._cc = LhFactoryCc(client, name + ':cc')
         self._tc = TcFactorySettings(client, name + ':tc')
         self._pc = DlPcFactorySettings(client, name + ':pc')
-        self._eom = PcFactorySettings(client, name + ':eom')
         self._pd = DlPdFactorySettings(client, name + ':pd')
         self._last_modified = DecopString(client, name + ':last-modified')
         self._modified = DecopBoolean(client, name + ':modified')
 
     @property
     def wavelength(self) -> 'MutableDecopReal':
         return self._wavelength
@@ -1585,18 +1579,14 @@
         return self._tc
 
     @property
     def pc(self) -> 'DlPcFactorySettings':
         return self._pc
 
     @property
-    def eom(self) -> 'PcFactorySettings':
-        return self._eom
-
-    @property
     def pd(self) -> 'DlPdFactorySettings':
         return self._pd
 
     @property
     def last_modified(self) -> 'DecopString':
         return self._last_modified
 
@@ -1800,55 +1790,14 @@
         return self._slew_rate_enabled
 
     @property
     def pressure_compensation_factor(self) -> 'MutableDecopReal':
         return self._pressure_compensation_factor
 
 
-class PcFactorySettings:
-    def __init__(self, client: Client, name: str) -> None:
-        self.__client = client
-        self.__name = name
-        self._voltage_min = MutableDecopReal(client, name + ':voltage-min')
-        self._voltage_max = MutableDecopReal(client, name + ':voltage-max')
-        self._feedforward_enabled = MutableDecopBoolean(client, name + ':feedforward-enabled')
-        self._feedforward_factor = MutableDecopReal(client, name + ':feedforward-factor')
-        self._capacitance = MutableDecopReal(client, name + ':capacitance')
-        self._scan_offset = MutableDecopReal(client, name + ':scan-offset')
-        self._scan_amplitude = MutableDecopReal(client, name + ':scan-amplitude')
-
-    @property
-    def voltage_min(self) -> 'MutableDecopReal':
-        return self._voltage_min
-
-    @property
-    def voltage_max(self) -> 'MutableDecopReal':
-        return self._voltage_max
-
-    @property
-    def feedforward_enabled(self) -> 'MutableDecopBoolean':
-        return self._feedforward_enabled
-
-    @property
-    def feedforward_factor(self) -> 'MutableDecopReal':
-        return self._feedforward_factor
-
-    @property
-    def capacitance(self) -> 'MutableDecopReal':
-        return self._capacitance
-
-    @property
-    def scan_offset(self) -> 'MutableDecopReal':
-        return self._scan_offset
-
-    @property
-    def scan_amplitude(self) -> 'MutableDecopReal':
-        return self._scan_amplitude
-
-
 class DlPdFactorySettings:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._seed = PdCalFactorySettings(client, name + ':seed')
 
     @property
@@ -3529,14 +3478,15 @@
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._ongoing = DecopBoolean(client, name + ':ongoing')
         self._progress = DecopInteger(client, name + ':progress')
         self._status = DecopInteger(client, name + ':status')
         self._status_string = DecopString(client, name + ':status-string')
+        self._last_time_optimized = DecopString(client, name + ':last-time-optimized')
         self._shg_advanced = MutableDecopBoolean(client, name + ':shg-advanced')
         self._stage1 = NloStage1(client, name + ':stage1')
         self._stage2 = NloStage1(client, name + ':stage2')
         self._stage3 = NloStage1(client, name + ':stage3')
         self._stage4 = NloStage1(client, name + ':stage4')
         self._stage5 = NloStage1(client, name + ':stage5')
         self._progress_data_amp = DecopBinary(client, name + ':progress-data-amp')
@@ -3558,14 +3508,18 @@
         return self._status
 
     @property
     def status_string(self) -> 'DecopString':
         return self._status_string
 
     @property
+    def last_time_optimized(self) -> 'DecopString':
+        return self._last_time_optimized
+
+    @property
     def shg_advanced(self) -> 'MutableDecopBoolean':
         return self._shg_advanced
 
     @property
     def stage1(self) -> 'NloStage1':
         return self._stage1
 
@@ -4058,37 +4012,57 @@
 class NloLaserHeadWindow1:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._input_channel = MutableDecopInteger(client, name + ':input-channel')
         self._threshold = MutableDecopReal(client, name + ':threshold')
         self._level_hysteresis = MutableDecopReal(client, name + ':level-hysteresis')
-        self._calibration = NloLaserHeadWindowCalibration1(client, name + ':calibration')
+        self._calibration = NloLaserHeadWindowCalibration2(client, name + ':calibration')
 
     @property
     def input_channel(self) -> 'MutableDecopInteger':
         return self._input_channel
 
     @property
     def threshold(self) -> 'MutableDecopReal':
         return self._threshold
 
     @property
     def level_hysteresis(self) -> 'MutableDecopReal':
         return self._level_hysteresis
 
     @property
-    def calibration(self) -> 'NloLaserHeadWindowCalibration1':
+    def calibration(self) -> 'NloLaserHeadWindowCalibration2':
         return self._calibration
 
 
-class NloLaserHeadWindowCalibration1:
+class NloLaserHeadWindowCalibration2:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
+        self._power_min = MutableDecopReal(client, name + ':power-min')
+        self._power_max = MutableDecopReal(client, name + ':power-max')
+        self._threshold_min = MutableDecopReal(client, name + ':threshold-min')
+        self._threshold_max = MutableDecopReal(client, name + ':threshold-max')
+
+    @property
+    def power_min(self) -> 'MutableDecopReal':
+        return self._power_min
+
+    @property
+    def power_max(self) -> 'MutableDecopReal':
+        return self._power_max
+
+    @property
+    def threshold_min(self) -> 'MutableDecopReal':
+        return self._threshold_min
+
+    @property
+    def threshold_max(self) -> 'MutableDecopReal':
+        return self._threshold_max
 
 
 class NloLaserHeadPid1:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._gain = NloLaserHeadGain1(client, name + ':gain')
@@ -6219,37 +6193,57 @@
 class NloLaserHeadWindow2:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._input_channel = DecopInteger(client, name + ':input-channel')
         self._threshold = DecopReal(client, name + ':threshold')
         self._level_hysteresis = DecopReal(client, name + ':level-hysteresis')
-        self._calibration = NloLaserHeadWindowCalibration2(client, name + ':calibration')
+        self._calibration = NloLaserHeadWindowCalibration1(client, name + ':calibration')
 
     @property
     def input_channel(self) -> 'DecopInteger':
         return self._input_channel
 
     @property
     def threshold(self) -> 'DecopReal':
         return self._threshold
 
     @property
     def level_hysteresis(self) -> 'DecopReal':
         return self._level_hysteresis
 
     @property
-    def calibration(self) -> 'NloLaserHeadWindowCalibration2':
+    def calibration(self) -> 'NloLaserHeadWindowCalibration1':
         return self._calibration
 
 
-class NloLaserHeadWindowCalibration2:
+class NloLaserHeadWindowCalibration1:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
+        self._power_min = DecopReal(client, name + ':power-min')
+        self._power_max = DecopReal(client, name + ':power-max')
+        self._threshold_min = DecopReal(client, name + ':threshold-min')
+        self._threshold_max = DecopReal(client, name + ':threshold-max')
+
+    @property
+    def power_min(self) -> 'DecopReal':
+        return self._power_min
+
+    @property
+    def power_max(self) -> 'DecopReal':
+        return self._power_max
+
+    @property
+    def threshold_min(self) -> 'DecopReal':
+        return self._threshold_min
+
+    @property
+    def threshold_max(self) -> 'DecopReal':
+        return self._threshold_max
 
 
 class NloLaserHeadPid2:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._gain = NloLaserHeadGain2(client, name + ':gain')
@@ -6719,53 +6713,32 @@
 
 
 class LaserDiagnosis:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._ready = DecopBoolean(client, name + ':ready')
-        self._options = LaserDiagnosisOptions(client, name + ':options')
 
     @property
     def ready(self) -> 'DecopBoolean':
         return self._ready
 
-    @property
-    def options(self) -> 'LaserDiagnosisOptions':
-        return self._options
-
     async def start(self) -> None:
         await self.__client.exec(self.__name + ':start')
 
     async def print_result(self) -> bytes:
         return await self.__client.exec(self.__name + ':print-result', output_type=bytes)
 
     async def execute(self) -> bytes:
         return await self.__client.exec(self.__name + ':execute', output_type=bytes)
 
     async def generate_to_usb(self) -> None:
         await self.__client.exec(self.__name + ':generate-to-usb')
 
 
-class LaserDiagnosisOptions:
-    def __init__(self, client: Client, name: str) -> None:
-        self.__client = client
-        self.__name = name
-        self._servo_test = MutableDecopBoolean(client, name + ':servo-test')
-        self._servo_stepsize = MutableDecopInteger(client, name + ':servo-stepsize')
-
-    @property
-    def servo_test(self) -> 'MutableDecopBoolean':
-        return self._servo_test
-
-    @property
-    def servo_stepsize(self) -> 'MutableDecopInteger':
-        return self._servo_stepsize
-
-
 class LaserComponents:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
 
 
 class LaserCommon:
@@ -6963,14 +6936,17 @@
         self._power_act = DecopReal(client, name + ':power-act')
         self._wavelength = DecopReal(client, name + ':wavelength')
         self._idle_mode = MutableDecopBoolean(client, name + ':idle-mode')
         self._wavemeter = AutoNloWavemeter(client, name + ':wavemeter')
         self._power_stabilization_settings = AutoNloPowerStabilizationSettings(client, name + ':power-stabilization-settings')
         self._optimization_settings = AutoNloOptimizationOptions(client, name + ':optimization-settings')
         self._optimization_progress = DecopInteger(client, name + ':optimization-progress')
+        self._last_time_auto_align = DecopString(client, name + ':last-time-auto-align')
+        self._last_time_single_mode_optimization = DecopString(client, name + ':last-time-single-mode-optimization')
+        self._single_mode_optimization_valid = DecopInteger(client, name + ':single-mode-optimization-valid')
 
     @property
     def automatic_mode(self) -> 'MutableDecopBoolean':
         return self._automatic_mode
 
     @property
     def serial_number(self) -> 'DecopString':
@@ -7128,14 +7104,26 @@
     def optimization_settings(self) -> 'AutoNloOptimizationOptions':
         return self._optimization_settings
 
     @property
     def optimization_progress(self) -> 'DecopInteger':
         return self._optimization_progress
 
+    @property
+    def last_time_auto_align(self) -> 'DecopString':
+        return self._last_time_auto_align
+
+    @property
+    def last_time_single_mode_optimization(self) -> 'DecopString':
+        return self._last_time_single_mode_optimization
+
+    @property
+    def single_mode_optimization_valid(self) -> 'DecopInteger':
+        return self._single_mode_optimization_valid
+
     async def perform_optimization(self) -> None:
         await self.__client.exec(self.__name + ':perform-optimization')
 
     async def reset_operation_time_cavity(self) -> None:
         await self.__client.exec(self.__name + ':reset-operation-time-cavity')
 
     async def clear_errors(self) -> None:
@@ -8042,26 +8030,48 @@
 
 
 class Buzzer:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._welcome = MutableDecopString(client, name + ':welcome')
+        self._sounds = BuzzerSounds(client, name + ':sounds')
 
     @property
     def welcome(self) -> 'MutableDecopString':
         return self._welcome
 
+    @property
+    def sounds(self) -> 'BuzzerSounds':
+        return self._sounds
+
     async def play_welcome(self) -> None:
         await self.__client.exec(self.__name + ':play-welcome')
 
     async def play(self, melody: str) -> None:
         assert isinstance(melody, str), f"expected type 'str' for parameter 'melody', got '{type(melody)}'"
         await self.__client.exec(self.__name + ':play', melody)
 
+    async def save(self) -> None:
+        await self.__client.exec(self.__name + ':save')
+
+    async def load(self) -> None:
+        await self.__client.exec(self.__name + ':load')
+
+
+class BuzzerSounds:
+    def __init__(self, client: Client, name: str) -> None:
+        self.__client = client
+        self.__name = name
+        self._on_connection = MutableDecopBoolean(client, name + ':on-connection')
+
+    @property
+    def on_connection(self) -> 'MutableDecopBoolean':
+        return self._on_connection
+
 
 class Display:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._brightness = MutableDecopReal(client, name + ':brightness')
         self._auto_dark = MutableDecopBoolean(client, name + ':auto-dark')
@@ -8097,35 +8107,35 @@
 
 class Standby:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._enabled = MutableDecopBoolean(client, name + ':enabled')
         self._state = DecopInteger(client, name + ':state')
-        self._laser1 = StandbyLaser1(client, name + ':laser1')
+        self._laser1 = StandbyLaser(client, name + ':laser1')
         self._laser2 = StandbyLaser2(client, name + ':laser2')
 
     @property
     def enabled(self) -> 'MutableDecopBoolean':
         return self._enabled
 
     @property
     def state(self) -> 'DecopInteger':
         return self._state
 
     @property
-    def laser1(self) -> 'StandbyLaser1':
+    def laser1(self) -> 'StandbyLaser':
         return self._laser1
 
     @property
     def laser2(self) -> 'StandbyLaser2':
         return self._laser2
 
 
-class StandbyLaser1:
+class StandbyLaser:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._dl = StandbyDl(client, name + ':dl')
         self._amp = StandbyAmp(client, name + ':amp')
         self._ctl = StandbyCtl(client, name + ':ctl')
         self._nlo = StandbyShg(client, name + ':nlo')
@@ -8227,24 +8237,19 @@
 
 
 class StandbyLaser2:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._dl = StandbyDl(client, name + ':dl')
-        self._amp = StandbyAmp(client, name + ':amp')
 
     @property
     def dl(self) -> 'StandbyDl':
         return self._dl
 
-    @property
-    def amp(self) -> 'StandbyAmp':
-        return self._amp
-
 
 class PdhBoard:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._slot = DecopString(client, name + ':slot')
         self._serial_number = DecopString(client, name + ':serial-number')
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_5_2.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_5_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_5_2.xml' on 2023-11-23 15:57:19.850996
+# Generated from 'v2_5_2.xml' on 2024-04-11 08:21:58.777298
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_5_3.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_5_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_5_3.xml' on 2023-11-23 15:57:20.181139
+# Generated from 'v2_5_3.xml' on 2024-04-11 08:21:59.255780
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_5_4.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_5_4.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_5_4.xml' on 2023-11-23 15:57:20.501688
+# Generated from 'v2_5_4.xml' on 2024-04-11 08:21:59.720559
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_6_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_6_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_6_0.xml' on 2023-11-23 15:57:20.827374
+# Generated from 'v2_6_0.xml' on 2024-04-11 08:22:00.226770
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v2_7_2.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v2_7_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_7_2.xml' on 2023-11-23 15:57:21.171965
+# Generated from 'v2_7_2.xml' on 2024-04-11 08:22:00.692119
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/dlcpro/v3_0_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/dlcpro/v3_0_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v3_0_1.xml' on 2023-11-23 15:57:21.525561
+# Generated from 'v3_0_1.xml' on 2024-04-11 08:22:01.159839
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_cle/v1_0_8.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_cle/v1_0_8.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_0_8.xml' on 2023-11-23 15:57:21.830571
+# Generated from 'v1_0_8.xml' on 2024-04-11 08:22:02.554501
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_cle/v1_1_3.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_cle/v1_1_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_1_3.xml' on 2023-11-23 15:57:22.101904
+# Generated from 'v1_1_3.xml' on 2024-04-11 08:22:02.922455
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_cle/v2_2_5.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_cle/v2_2_5.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_2_5.xml' on 2023-11-23 15:57:22.342266
+# Generated from 'v2_2_5.xml' on 2024-04-11 08:22:03.288006
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_mle/v1_8_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_mle/v1_8_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_8_1.xml' on 2023-11-23 15:57:22.574702
+# Generated from 'v1_8_1.xml' on 2024-04-11 08:22:03.658926
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_mle/v2_2_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_mle/v2_2_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_2_0.xml' on 2023-11-23 15:57:22.805408
+# Generated from 'v2_2_0.xml' on 2024-04-11 08:22:04.015072
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/asyncio/ichrome_mle/v2_3_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/asyncio/ichrome_mle/v2_3_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_3_1.xml' on 2023-11-23 15:57:23.040990
+# Generated from 'v2_3_1.xml' on 2024-04-11 08:22:04.369213
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.asyncio.client import UserLevel
 from toptica.lasersdk.asyncio.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/client.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/client.py`

 * *Files identical despite different names*

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/decop.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/decop.py`

 * *Files identical despite different names*

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_4_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_4_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_4_0.xml' on 2023-11-23 15:57:07.205970
+# Generated from 'v1_4_0.xml' on 2024-04-11 08:21:40.082166
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_5_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_5_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_5_1.xml' on 2023-11-23 15:57:07.482993
+# Generated from 'v1_5_1.xml' on 2024-04-11 08:21:40.514553
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_6_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_6_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_6_1.xml' on 2023-11-23 15:57:07.783050
+# Generated from 'v1_6_3.xml' on 2024-04-11 08:21:41.366348
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
 
@@ -3394,27 +3394,38 @@
 class NloLaserHeadWindow1:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._input_channel = MutableDecopInteger(client, name + ':input-channel')
         self._threshold = MutableDecopReal(client, name + ':threshold')
         self._level_hysteresis = MutableDecopReal(client, name + ':level-hysteresis')
+        self._calibration = NloLaserHeadWindowCalibration1(client, name + ':calibration')
 
     @property
     def input_channel(self) -> 'MutableDecopInteger':
         return self._input_channel
 
     @property
     def threshold(self) -> 'MutableDecopReal':
         return self._threshold
 
     @property
     def level_hysteresis(self) -> 'MutableDecopReal':
         return self._level_hysteresis
 
+    @property
+    def calibration(self) -> 'NloLaserHeadWindowCalibration1':
+        return self._calibration
+
+
+class NloLaserHeadWindowCalibration1:
+    def __init__(self, client: Client, name: str) -> None:
+        self.__client = client
+        self.__name = name
+
 
 class NloLaserHeadPid1:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._gain = NloLaserHeadGain1(client, name + ':gain')
 
@@ -5287,27 +5298,38 @@
 class NloLaserHeadWindow2:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._input_channel = DecopInteger(client, name + ':input-channel')
         self._threshold = DecopReal(client, name + ':threshold')
         self._level_hysteresis = DecopReal(client, name + ':level-hysteresis')
+        self._calibration = NloLaserHeadWindowCalibration2(client, name + ':calibration')
 
     @property
     def input_channel(self) -> 'DecopInteger':
         return self._input_channel
 
     @property
     def threshold(self) -> 'DecopReal':
         return self._threshold
 
     @property
     def level_hysteresis(self) -> 'DecopReal':
         return self._level_hysteresis
 
+    @property
+    def calibration(self) -> 'NloLaserHeadWindowCalibration2':
+        return self._calibration
+
+
+class NloLaserHeadWindowCalibration2:
+    def __init__(self, client: Client, name: str) -> None:
+        self.__client = client
+        self.__name = name
+
 
 class NloLaserHeadPid2:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._gain = NloLaserHeadGain2(client, name + ':gain')
 
@@ -5483,14 +5505,15 @@
         self._power_margin_tolerance_time = DecopInteger(client, name + ':power-margin-tolerance-time')
         self._power_margin_threshold = DecopReal(client, name + ':power-margin-threshold')
         self._cavity_lock_settle_time = DecopInteger(client, name + ':cavity-lock-settle-time')
         self._cavity_lock_tolerance_factor = DecopInteger(client, name + ':cavity-lock-tolerance-factor')
         self._power_lock_settle_time = DecopInteger(client, name + ':power-lock-settle-time')
         self._cavity_scan_duration = DecopInteger(client, name + ':cavity-scan-duration')
         self._power_stabilization_strategy = DecopInteger(client, name + ':power-stabilization-strategy')
+        self._power_stabilization_level_low_factor = DecopReal(client, name + ':power-stabilization-level-low-factor')
         self._power_output_relative_error_max = DecopReal(client, name + ':power-output-relative-error-max')
         self._power_output_relative_deviation_max = DecopReal(client, name + ':power-output-relative-deviation-max')
         self._operational_pump_power = DecopReal(client, name + ':operational-pump-power')
 
     @property
     def baseplate_temperature_limit(self) -> 'DecopReal':
         return self._baseplate_temperature_limit
@@ -5532,14 +5555,18 @@
         return self._cavity_scan_duration
 
     @property
     def power_stabilization_strategy(self) -> 'DecopInteger':
         return self._power_stabilization_strategy
 
     @property
+    def power_stabilization_level_low_factor(self) -> 'DecopReal':
+        return self._power_stabilization_level_low_factor
+
+    @property
     def power_output_relative_error_max(self) -> 'DecopReal':
         return self._power_output_relative_error_max
 
     @property
     def power_output_relative_deviation_max(self) -> 'DecopReal':
         return self._power_output_relative_deviation_max
 
@@ -5703,14 +5730,15 @@
         self._error_txt = DecopString(client, name + ':error-txt')
         self._operation_time_pump = DecopReal(client, name + ':operation-time-pump')
         self._operation_time_uv = DecopReal(client, name + ':operation-time-uv')
         self._pump_power_margin = DecopReal(client, name + ':pump-power-margin')
         self._remaining_optics_spots = DecopInteger(client, name + ':remaining-optics-spots')
         self._power_set = MutableDecopReal(client, name + ':power-set')
         self._power_act = DecopReal(client, name + ':power-act')
+        self._baseplate_temperature = DecopReal(client, name + ':baseplate-temperature')
 
     @property
     def emission(self) -> 'DecopBoolean':
         return self._emission
 
     @property
     def status(self) -> 'DecopInteger':
@@ -5748,14 +5776,18 @@
     def power_set(self) -> 'MutableDecopReal':
         return self._power_set
 
     @property
     def power_act(self) -> 'DecopReal':
         return self._power_act
 
+    @property
+    def baseplate_temperature(self) -> 'DecopReal':
+        return self._baseplate_temperature
+
     def perform_optimization(self) -> None:
         self.__client.exec(self.__name + ':perform-optimization')
 
     def clear_errors(self) -> None:
         self.__client.exec(self.__name + ':clear-errors')
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_6_3.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_6_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_6_3.xml' on 2023-11-23 15:57:08.064508
+# Generated from 'v1_6_1.xml' on 2024-04-11 08:21:40.910087
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
 
@@ -3394,38 +3394,27 @@
 class NloLaserHeadWindow1:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._input_channel = MutableDecopInteger(client, name + ':input-channel')
         self._threshold = MutableDecopReal(client, name + ':threshold')
         self._level_hysteresis = MutableDecopReal(client, name + ':level-hysteresis')
-        self._calibration = NloLaserHeadWindowCalibration1(client, name + ':calibration')
 
     @property
     def input_channel(self) -> 'MutableDecopInteger':
         return self._input_channel
 
     @property
     def threshold(self) -> 'MutableDecopReal':
         return self._threshold
 
     @property
     def level_hysteresis(self) -> 'MutableDecopReal':
         return self._level_hysteresis
 
-    @property
-    def calibration(self) -> 'NloLaserHeadWindowCalibration1':
-        return self._calibration
-
-
-class NloLaserHeadWindowCalibration1:
-    def __init__(self, client: Client, name: str) -> None:
-        self.__client = client
-        self.__name = name
-
 
 class NloLaserHeadPid1:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._gain = NloLaserHeadGain1(client, name + ':gain')
 
@@ -5298,38 +5287,27 @@
 class NloLaserHeadWindow2:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._input_channel = DecopInteger(client, name + ':input-channel')
         self._threshold = DecopReal(client, name + ':threshold')
         self._level_hysteresis = DecopReal(client, name + ':level-hysteresis')
-        self._calibration = NloLaserHeadWindowCalibration2(client, name + ':calibration')
 
     @property
     def input_channel(self) -> 'DecopInteger':
         return self._input_channel
 
     @property
     def threshold(self) -> 'DecopReal':
         return self._threshold
 
     @property
     def level_hysteresis(self) -> 'DecopReal':
         return self._level_hysteresis
 
-    @property
-    def calibration(self) -> 'NloLaserHeadWindowCalibration2':
-        return self._calibration
-
-
-class NloLaserHeadWindowCalibration2:
-    def __init__(self, client: Client, name: str) -> None:
-        self.__client = client
-        self.__name = name
-
 
 class NloLaserHeadPid2:
     def __init__(self, client: Client, name: str) -> None:
         self.__client = client
         self.__name = name
         self._gain = NloLaserHeadGain2(client, name + ':gain')
 
@@ -5505,15 +5483,14 @@
         self._power_margin_tolerance_time = DecopInteger(client, name + ':power-margin-tolerance-time')
         self._power_margin_threshold = DecopReal(client, name + ':power-margin-threshold')
         self._cavity_lock_settle_time = DecopInteger(client, name + ':cavity-lock-settle-time')
         self._cavity_lock_tolerance_factor = DecopInteger(client, name + ':cavity-lock-tolerance-factor')
         self._power_lock_settle_time = DecopInteger(client, name + ':power-lock-settle-time')
         self._cavity_scan_duration = DecopInteger(client, name + ':cavity-scan-duration')
         self._power_stabilization_strategy = DecopInteger(client, name + ':power-stabilization-strategy')
-        self._power_stabilization_level_low_factor = DecopReal(client, name + ':power-stabilization-level-low-factor')
         self._power_output_relative_error_max = DecopReal(client, name + ':power-output-relative-error-max')
         self._power_output_relative_deviation_max = DecopReal(client, name + ':power-output-relative-deviation-max')
         self._operational_pump_power = DecopReal(client, name + ':operational-pump-power')
 
     @property
     def baseplate_temperature_limit(self) -> 'DecopReal':
         return self._baseplate_temperature_limit
@@ -5555,18 +5532,14 @@
         return self._cavity_scan_duration
 
     @property
     def power_stabilization_strategy(self) -> 'DecopInteger':
         return self._power_stabilization_strategy
 
     @property
-    def power_stabilization_level_low_factor(self) -> 'DecopReal':
-        return self._power_stabilization_level_low_factor
-
-    @property
     def power_output_relative_error_max(self) -> 'DecopReal':
         return self._power_output_relative_error_max
 
     @property
     def power_output_relative_deviation_max(self) -> 'DecopReal':
         return self._power_output_relative_deviation_max
 
@@ -5730,15 +5703,14 @@
         self._error_txt = DecopString(client, name + ':error-txt')
         self._operation_time_pump = DecopReal(client, name + ':operation-time-pump')
         self._operation_time_uv = DecopReal(client, name + ':operation-time-uv')
         self._pump_power_margin = DecopReal(client, name + ':pump-power-margin')
         self._remaining_optics_spots = DecopInteger(client, name + ':remaining-optics-spots')
         self._power_set = MutableDecopReal(client, name + ':power-set')
         self._power_act = DecopReal(client, name + ':power-act')
-        self._baseplate_temperature = DecopReal(client, name + ':baseplate-temperature')
 
     @property
     def emission(self) -> 'DecopBoolean':
         return self._emission
 
     @property
     def status(self) -> 'DecopInteger':
@@ -5776,18 +5748,14 @@
     def power_set(self) -> 'MutableDecopReal':
         return self._power_set
 
     @property
     def power_act(self) -> 'DecopReal':
         return self._power_act
 
-    @property
-    def baseplate_temperature(self) -> 'DecopReal':
-        return self._baseplate_temperature
-
     def perform_optimization(self) -> None:
         self.__client.exec(self.__name + ':perform-optimization')
 
     def clear_errors(self) -> None:
         self.__client.exec(self.__name + ':clear-errors')
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_7_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_7_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_7_0.xml' on 2023-11-23 15:57:08.349426
+# Generated from 'v1_7_0.xml' on 2024-04-11 08:21:41.773476
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_8_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_8_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_8_1.xml' on 2023-11-23 15:57:08.639429
+# Generated from 'v1_8_1.xml' on 2024-04-11 08:21:42.200573
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v1_9_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v1_9_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_9_0.xml' on 2023-11-23 15:57:08.934535
+# Generated from 'v1_9_0.xml' on 2024-04-11 08:21:42.600867
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_0_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_0_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_0_1.xml' on 2023-11-23 15:57:09.261236
+# Generated from 'v2_0_3.xml' on 2024-04-11 08:21:43.472875
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_0_3.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_0_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_0_3.xml' on 2023-11-23 15:57:09.573341
+# Generated from 'v2_0_1.xml' on 2024-04-11 08:21:43.047892
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_1_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_1_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_1_0.xml' on 2023-11-23 15:57:09.880179
+# Generated from 'v2_1_0.xml' on 2024-04-11 08:21:43.896639
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_2_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_2_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_2_0.xml' on 2023-11-23 15:57:10.184848
+# Generated from 'v2_2_0.xml' on 2024-04-11 08:21:44.323794
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_3_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_3_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_3_0.xml' on 2023-11-23 15:57:10.529403
+# Generated from 'v2_3_0.xml' on 2024-04-11 08:21:44.755470
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_3_2.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_3_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_3_2.xml' on 2023-11-23 15:57:10.830984
+# Generated from 'v2_3_2.xml' on 2024-04-11 08:21:45.181508
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_3_4.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_3_4.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_3_4.xml' on 2023-11-23 15:57:11.143843
+# Generated from 'v2_3_4.xml' on 2024-04-11 08:21:45.625741
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_4_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_4_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_4_0.xml' on 2023-11-23 15:57:11.467880
+# Generated from 'v2_4_0.xml' on 2024-04-11 08:21:46.049066
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_5_2.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_5_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_5_2.xml' on 2023-11-23 15:57:11.798771
+# Generated from 'v2_5_2.xml' on 2024-04-11 08:21:46.494617
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_5_3.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_5_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_5_3.xml' on 2023-11-23 15:57:12.125157
+# Generated from 'v2_5_3.xml' on 2024-04-11 08:21:46.957101
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_5_4.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_5_4.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_5_4.xml' on 2023-11-23 15:57:12.452407
+# Generated from 'v2_5_4.xml' on 2024-04-11 08:21:47.406825
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_6_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_6_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_6_0.xml' on 2023-11-23 15:57:12.805796
+# Generated from 'v2_6_0.xml' on 2024-04-11 08:21:47.857944
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v2_7_2.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v2_7_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_7_2.xml' on 2023-11-23 15:57:13.132892
+# Generated from 'v2_7_2.xml' on 2024-04-11 08:21:48.316142
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/dlcpro/v3_0_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/dlcpro/v3_0_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v3_0_1.xml' on 2023-11-23 15:57:13.505786
+# Generated from 'v3_0_1.xml' on 2024-04-11 08:21:48.775964
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_cle/v1_0_8.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_cle/v1_0_8.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_0_8.xml' on 2023-11-23 15:57:13.779483
+# Generated from 'v1_0_8.xml' on 2024-04-11 08:21:50.156752
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_cle/v1_1_3.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_cle/v1_1_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_1_3.xml' on 2023-11-23 15:57:14.021565
+# Generated from 'v1_1_3.xml' on 2024-04-11 08:21:50.514905
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_cle/v2_2_5.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_cle/v2_2_5.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_2_5.xml' on 2023-11-23 15:57:14.261874
+# Generated from 'v2_2_5.xml' on 2024-04-11 08:21:50.855547
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_mle/v1_8_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_mle/v1_8_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v1_8_1.xml' on 2023-11-23 15:57:14.524251
+# Generated from 'v1_8_1.xml' on 2024-04-11 08:21:51.222621
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_mle/v2_2_0.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_mle/v2_2_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_2_0.xml' on 2023-11-23 15:57:14.756943
+# Generated from 'v2_2_0.xml' on 2024-04-11 08:21:51.576845
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/ichrome_mle/v2_3_1.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/ichrome_mle/v2_3_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from 'v2_3_1.xml' on 2023-11-23 15:57:15.000934
+# Generated from 'v2_3_1.xml' on 2024-04-11 08:21:51.932747
 
 from typing import Tuple
 from typing import Optional
 
 from toptica.lasersdk.client import UserLevel
 from toptica.lasersdk.client import Client
```

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/lasersdk_gen.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/lasersdk_gen.py`

 * *Files identical despite different names*

### Comparing `toptica_lasersdk-3.1.2/toptica/lasersdk/utils/dlcpro.py` & `toptica_lasersdk-3.2.0/toptica/lasersdk/utils/dlcpro.py`

 * *Files identical despite different names*

### Comparing `toptica_lasersdk-3.1.2/toptica_lasersdk.egg-info/PKG-INFO` & `toptica_lasersdk-3.2.0/toptica_lasersdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: toptica-lasersdk
-Version: 3.1.2
+Version: 3.2.0
 Summary: TOPTICA Python Laser SDK
 Home-page: https://toptica.github.io/python-lasersdk/
 Author: TOPTICA Photonics AG
 Author-email: info@toptica.com
 License: MIT
 Keywords: toptica photonics laser sdk dlcpro ichrome cle mle
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -20,14 +19,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6,<4
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: ifaddr
+Requires-Dist: pyserial
 
 TOPTICA Python Laser SDK
 ========================
 
 The **TOPTICA Python Laser SDK** allows for the easy control of TOPTICA laser products from a PC using the Python programming language.
-
-
```

### Comparing `toptica_lasersdk-3.1.2/toptica_lasersdk.egg-info/SOURCES.txt` & `toptica_lasersdk-3.2.0/toptica_lasersdk.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
 VERSION
 setup.cfg
 setup.py
+tests/test_async_client.py
+tests/test_client.py
+tests/test_client_subscription.py
+tests/test_client_subscription_async.py
+tests/test_client_types.py
+tests/test_client_types_async.py
+tests/test_connection.py
+tests/test_decop.py
+tests/test_decop_decode_value_inferred.py
+tests/test_dlcpro.py
+tests/test_dlcpro_utils.py
+tests/test_lasersdk_gen_commandline.py
 toptica/__init__.py
 toptica/lasersdk/__init__.py
 toptica/lasersdk/client.py
 toptica/lasersdk/decop.py
 toptica/lasersdk/lasersdk_gen.py
 toptica/lasersdk/py.typed
 toptica/lasersdk/asyncio/__init__.py
@@ -31,14 +43,16 @@
 toptica/lasersdk/asyncio/dlcpro/v2_4_0.py
 toptica/lasersdk/asyncio/dlcpro/v2_5_2.py
 toptica/lasersdk/asyncio/dlcpro/v2_5_3.py
 toptica/lasersdk/asyncio/dlcpro/v2_5_4.py
 toptica/lasersdk/asyncio/dlcpro/v2_6_0.py
 toptica/lasersdk/asyncio/dlcpro/v2_7_2.py
 toptica/lasersdk/asyncio/dlcpro/v3_0_1.py
+toptica/lasersdk/asyncio/dlcpro/v3_1_0.py
+toptica/lasersdk/asyncio/dlcpro/v3_2_0.py
 toptica/lasersdk/asyncio/ichrome_cle/__init__.py
 toptica/lasersdk/asyncio/ichrome_cle/v1_0_8.py
 toptica/lasersdk/asyncio/ichrome_cle/v1_1_3.py
 toptica/lasersdk/asyncio/ichrome_cle/v2_2_5.py
 toptica/lasersdk/asyncio/ichrome_mle/__init__.py
 toptica/lasersdk/asyncio/ichrome_mle/v1_8_1.py
 toptica/lasersdk/asyncio/ichrome_mle/v2_2_0.py
@@ -61,14 +75,16 @@
 toptica/lasersdk/dlcpro/v2_4_0.py
 toptica/lasersdk/dlcpro/v2_5_2.py
 toptica/lasersdk/dlcpro/v2_5_3.py
 toptica/lasersdk/dlcpro/v2_5_4.py
 toptica/lasersdk/dlcpro/v2_6_0.py
 toptica/lasersdk/dlcpro/v2_7_2.py
 toptica/lasersdk/dlcpro/v3_0_1.py
+toptica/lasersdk/dlcpro/v3_1_0.py
+toptica/lasersdk/dlcpro/v3_2_0.py
 toptica/lasersdk/ichrome_cle/__init__.py
 toptica/lasersdk/ichrome_cle/v1_0_8.py
 toptica/lasersdk/ichrome_cle/v1_1_3.py
 toptica/lasersdk/ichrome_cle/v2_2_5.py
 toptica/lasersdk/ichrome_mle/__init__.py
 toptica/lasersdk/ichrome_mle/v1_8_1.py
 toptica/lasersdk/ichrome_mle/v2_2_0.py
```

