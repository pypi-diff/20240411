# Comparing `tmp/pyvispr-2023.9.tar.gz` & `tmp/pyvispr-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvispr-2023.9.tar", last modified: Tue Dec 19 10:39:44 2023, max compression
+gzip compressed data, was "pyvispr-2024.1.tar", last modified: Thu Apr 11 11:30:13 2024, max compression
```

## Comparing `pyvispr-2023.9.tar` & `pyvispr-2024.1.tar`

### file list

```diff
@@ -1,68 +1,96 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/
--rw-r--r--   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 pyvispr-2023.9/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     5479 2023-12-19 10:39:44.082937 pyvispr-2023.9/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2023-11-17 11:04:31.000000 pyvispr-2023.9/README-COPYRIGHT-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pyvispr-2023.9/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     4650 2023-11-17 11:29:18.000000 pyvispr-2023.9/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.079604 pyvispr-2023.9/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.079604 pyvispr-2023.9/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1863 2023-11-17 11:29:18.000000 pyvispr-2023.9/documentation/wiki/description.asciidoc
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 pyvispr-2023.9/pyproject.toml
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/pyvispr/
--rw-r--r--   0 eric      (1000) users      (984)     1594 2023-11-17 11:20:29.000000 pyvispr-2023.9/pyvispr/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/pyvispr/catalog/
--rw-r--r--   0 eric      (1000) users      (984)     2467 2023-12-14 13:25:36.000000 pyvispr-2023.9/pyvispr/catalog/constants.py
--rw-r--r--   0 eric      (1000) users      (984)     2263 2023-12-14 13:26:16.000000 pyvispr-2023.9/pyvispr/catalog/main.py
--rw-r--r--   0 eric      (1000) users      (984)     8393 2023-12-19 10:13:34.000000 pyvispr-2023.9/pyvispr/catalog/parser.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/pyvispr/config/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/pyvispr/config/appearance/
--rw-r--r--   0 eric      (1000) users      (984)     1678 2023-11-24 19:22:48.000000 pyvispr-2023.9/pyvispr/config/appearance/backend.py
--rw-r--r--   0 eric      (1000) users      (984)     2511 2023-12-11 10:42:45.000000 pyvispr-2023.9/pyvispr/config/appearance/color.py
--rw-r--r--   0 eric      (1000) users      (984)     1711 2023-12-13 13:08:28.000000 pyvispr-2023.9/pyvispr/config/appearance/geometry.py
--rw-r--r--   0 eric      (1000) users      (984)     1762 2023-12-14 13:26:22.000000 pyvispr-2023.9/pyvispr/config/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/pyvispr/extension/
--rw-r--r--   0 eric      (1000) users      (984)     1858 2023-11-17 10:40:01.000000 pyvispr-2023.9/pyvispr/extension/module.py
--rw-r--r--   0 eric      (1000) users      (984)     1723 2023-12-14 14:25:13.000000 pyvispr-2023.9/pyvispr/extension/string_.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/pyvispr/flow/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/pyvispr/flow/descriptive/
--rw-r--r--   0 eric      (1000) users      (984)     9059 2023-12-19 10:13:34.000000 pyvispr-2023.9/pyvispr/flow/descriptive/node.py
--rw-r--r--   0 eric      (1000) users      (984)     2488 2023-12-18 16:18:57.000000 pyvispr-2023.9/pyvispr/flow/descriptive/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/pyvispr/flow/functional/
--rw-r--r--   0 eric      (1000) users      (984)     7350 2023-12-18 08:58:13.000000 pyvispr-2023.9/pyvispr/flow/functional/graph.py
--rw-r--r--   0 eric      (1000) users      (984)     4509 2023-12-12 21:43:02.000000 pyvispr-2023.9/pyvispr/flow/functional/link.py
--rw-r--r--   0 eric      (1000) users      (984)    10166 2023-12-18 16:41:27.000000 pyvispr-2023.9/pyvispr/flow/functional/node_isolated.py
--rw-r--r--   0 eric      (1000) users      (984)     3304 2023-12-13 13:44:24.000000 pyvispr-2023.9/pyvispr/flow/functional/node_linked.py
--rw-r--r--   0 eric      (1000) users      (984)     2558 2023-12-06 08:54:33.000000 pyvispr-2023.9/pyvispr/flow/functional/socket.py
--rw-r--r--   0 eric      (1000) users      (984)     2210 2023-12-08 14:41:05.000000 pyvispr-2023.9/pyvispr/flow/messenger.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/pyvispr/flow/visual/
--rw-r--r--   0 eric      (1000) users      (984)    18887 2023-12-19 10:13:34.000000 pyvispr-2023.9/pyvispr/flow/visual/graph.py
--rw-r--r--   0 eric      (1000) users      (984)     6168 2023-12-19 10:13:34.000000 pyvispr-2023.9/pyvispr/flow/visual/link.py
--rw-r--r--   0 eric      (1000) users      (984)    12092 2023-12-19 10:13:34.000000 pyvispr-2023.9/pyvispr/flow/visual/node.py
--rw-r--r--   0 eric      (1000) users      (984)     1880 2023-12-07 16:16:52.000000 pyvispr-2023.9/pyvispr/flow/visual/socket.py
--rw-r--r--   0 eric      (1000) users      (984)     7968 2023-12-19 10:13:34.000000 pyvispr-2023.9/pyvispr/flow/visual/whiteboard.py
--rw-r--r--   0 eric      (1000) users      (984)     1914 2023-12-18 19:37:25.000000 pyvispr-2023.9/pyvispr/install.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.079604 pyvispr-2023.9/pyvispr/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/pyvispr/interface/storage/
--rw-r--r--   0 eric      (1000) users      (984)     3006 2023-12-18 18:41:16.000000 pyvispr-2023.9/pyvispr/interface/storage/loading.py
--rw-r--r--   0 eric      (1000) users      (984)     3533 2023-12-19 07:56:09.000000 pyvispr-2023.9/pyvispr/interface/storage/stowing.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/pyvispr/interface/window/
--rw-r--r--   0 eric      (1000) users      (984)     4200 2023-12-19 10:35:37.000000 pyvispr-2023.9/pyvispr/interface/window/installer.py
--rw-r--r--   0 eric      (1000) users      (984)     1841 2023-12-13 13:55:15.000000 pyvispr-2023.9/pyvispr/interface/window/messenger.py
--rw-r--r--   0 eric      (1000) users      (984)     7367 2023-12-19 10:13:34.000000 pyvispr-2023.9/pyvispr/interface/window/runner.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/pyvispr/interface/window/widget/
--rw-r--r--   0 eric      (1000) users      (984)     1844 2023-12-19 10:13:31.000000 pyvispr-2023.9/pyvispr/interface/window/widget/function_list.py
--rw-r--r--   0 eric      (1000) users      (984)     3416 2023-12-19 10:13:34.000000 pyvispr-2023.9/pyvispr/interface/window/widget/list.py
--rw-r--r--   0 eric      (1000) users      (984)     2413 2023-12-18 18:40:08.000000 pyvispr-2023.9/pyvispr/interface/window/widget/menu.py
--rw-r--r--   0 eric      (1000) users      (984)     1926 2023-12-19 10:13:31.000000 pyvispr-2023.9/pyvispr/interface/window/widget/module_list.py
--rw-r--r--   0 eric      (1000) users      (984)     3713 2023-12-19 10:13:31.000000 pyvispr-2023.9/pyvispr/interface/window/widget/node_list.py
--rwxr-xr-x   0 eric      (1000) users      (984)     1905 2023-12-19 07:56:37.000000 pyvispr-2023.9/pyvispr/run.py
--rw-r--r--   0 eric      (1000) users      (984)     1577 2023-12-19 10:38:40.000000 pyvispr-2023.9/pyvispr/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-12-19 10:39:44.082937 pyvispr-2023.9/pyvispr.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     5479 2023-12-19 10:39:44.000000 pyvispr-2023.9/pyvispr.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     1494 2023-12-19 10:39:44.000000 pyvispr-2023.9/pyvispr.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-12-19 10:39:44.000000 pyvispr-2023.9/pyvispr.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       91 2023-12-19 10:39:44.000000 pyvispr-2023.9/pyvispr.egg-info/entry_points.txt
--rw-r--r--   0 eric      (1000) users      (984)       19 2023-12-19 10:39:44.000000 pyvispr-2023.9/pyvispr.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)        8 2023-12-19 10:39:44.000000 pyvispr-2023.9/pyvispr.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-12-19 10:39:44.082937 pyvispr-2023.9/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     6254 2023-12-19 10:39:37.000000 pyvispr-2023.9/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.859575 pyvispr-2024.1/
+-rwx------   0 eric      (1000) users      (984)      139 2024-04-05 18:00:47.000000 pyvispr-2024.1/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     5681 2024-04-11 11:30:13.859575 pyvispr-2024.1/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      642 2024-02-07 09:03:58.000000 pyvispr-2024.1/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pyvispr-2024.1/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     4652 2024-02-07 09:03:58.000000 pyvispr-2024.1/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.849575 pyvispr-2024.1/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.852908 pyvispr-2024.1/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     2421 2024-02-07 09:22:47.000000 pyvispr-2024.1/documentation/wiki/description.asciidoc
+-rwx------   0 eric      (1000) users      (984)      112 2024-02-07 08:56:45.000000 pyvispr-2024.1/pyproject.toml
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.852908 pyvispr-2024.1/pyvispr/
+-rwx------   0 eric      (1000) users      (984)     1594 2023-11-17 11:20:29.000000 pyvispr-2024.1/pyvispr/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.852908 pyvispr-2024.1/pyvispr/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.852908 pyvispr-2024.1/pyvispr/catalog/factory/
+-rwx------   0 eric      (1000) users      (984)     1804 2024-01-19 10:13:27.000000 pyvispr-2024.1/pyvispr/catalog/factory/image_loader.py
+-rwx------   0 eric      (1000) users      (984)    12213 2024-04-11 08:05:54.000000 pyvispr-2024.1/pyvispr/catalog/factory/image_viewer.py
+-rwx------   0 eric      (1000) users      (984)     1975 2024-01-19 10:13:27.000000 pyvispr-2024.1/pyvispr/catalog/factory/numexpr_calculator.py
+-rwx------   0 eric      (1000) users      (984)     1818 2024-01-19 10:18:15.000000 pyvispr-2024.1/pyvispr/catalog/factory/value.py
+-rwx------   0 eric      (1000) users      (984)     2506 2024-04-10 14:04:53.000000 pyvispr-2024.1/pyvispr/catalog/factory/value_viewer.py
+-rwx------   0 eric      (1000) users      (984)     7691 2024-04-11 08:05:54.000000 pyvispr-2024.1/pyvispr/catalog/installer.py
+-rwx------   0 eric      (1000) users      (984)     4114 2024-04-10 13:36:40.000000 pyvispr-2024.1/pyvispr/catalog/parser.py
+-rwx------   0 eric      (1000) users      (984)     2226 2024-04-10 14:04:29.000000 pyvispr-2024.1/pyvispr/catalog/type.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.852908 pyvispr-2024.1/pyvispr/config/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.852908 pyvispr-2024.1/pyvispr/config/appearance/
+-rwx------   0 eric      (1000) users      (984)     1584 2024-04-10 13:34:33.000000 pyvispr-2024.1/pyvispr/config/appearance/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)     1611 2024-04-10 13:52:01.000000 pyvispr-2024.1/pyvispr/config/appearance/behavior.py
+-rwx------   0 eric      (1000) users      (984)     2586 2024-01-19 18:43:09.000000 pyvispr-2024.1/pyvispr/config/appearance/color.py
+-rwx------   0 eric      (1000) users      (984)     1711 2023-12-13 13:08:28.000000 pyvispr-2024.1/pyvispr/config/appearance/geometry.py
+-rwx------   0 eric      (1000) users      (984)     1788 2024-04-10 14:04:53.000000 pyvispr-2024.1/pyvispr/config/path.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.856242 pyvispr-2024.1/pyvispr/constant/
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 14:04:29.000000 pyvispr-2024.1/pyvispr/constant/app.py
+-rwx------   0 eric      (1000) users      (984)     1961 2024-01-22 14:35:46.000000 pyvispr-2024.1/pyvispr/constant/catalog.py
+-rw-r--r--   0 eric      (1000) users      (984)     1654 2024-04-10 13:34:03.000000 pyvispr-2024.1/pyvispr/constant/function.py
+-rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-10 13:51:28.000000 pyvispr-2024.1/pyvispr/constant/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     1610 2024-04-10 15:59:22.000000 pyvispr-2024.1/pyvispr/constant/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.856242 pyvispr-2024.1/pyvispr/constant/widget/
+-rw-r--r--   0 eric      (1000) users      (984)     1873 2024-04-10 14:04:53.000000 pyvispr-2024.1/pyvispr/constant/widget/function_header.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 13:59:48.000000 pyvispr-2024.1/pyvispr/constant/widget/list.py
+-rw-r--r--   0 eric      (1000) users      (984)     1936 2024-04-10 14:44:36.000000 pyvispr-2024.1/pyvispr/constant/widget/node.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.856242 pyvispr-2024.1/pyvispr/extension/
+-rwx------   0 eric      (1000) users      (984)    11628 2024-04-11 08:06:24.000000 pyvispr-2024.1/pyvispr/extension/function.py
+-rwx------   0 eric      (1000) users      (984)     2907 2024-04-11 10:11:11.000000 pyvispr-2024.1/pyvispr/extension/module.py
+-rwx------   0 eric      (1000) users      (984)     1986 2024-01-19 10:18:15.000000 pyvispr-2024.1/pyvispr/extension/qt6.py
+-rwx------   0 eric      (1000) users      (984)     1723 2023-12-14 14:25:13.000000 pyvispr-2024.1/pyvispr/extension/string_.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.856242 pyvispr-2024.1/pyvispr/flow/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.856242 pyvispr-2024.1/pyvispr/flow/descriptive/
+-rwx------   0 eric      (1000) users      (984)     7992 2024-04-11 11:25:22.000000 pyvispr-2024.1/pyvispr/flow/descriptive/node.py
+-rwx------   0 eric      (1000) users      (984)     4481 2024-04-10 14:44:36.000000 pyvispr-2024.1/pyvispr/flow/descriptive/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.856242 pyvispr-2024.1/pyvispr/flow/functional/
+-rwx------   0 eric      (1000) users      (984)     6827 2024-04-11 08:16:26.000000 pyvispr-2024.1/pyvispr/flow/functional/graph.py
+-rwx------   0 eric      (1000) users      (984)     4509 2023-12-12 21:43:02.000000 pyvispr-2024.1/pyvispr/flow/functional/link.py
+-rwx------   0 eric      (1000) users      (984)    10835 2024-04-11 08:05:14.000000 pyvispr-2024.1/pyvispr/flow/functional/node_isolated.py
+-rwx------   0 eric      (1000) users      (984)     3546 2024-04-11 08:19:29.000000 pyvispr-2024.1/pyvispr/flow/functional/node_linked.py
+-rwx------   0 eric      (1000) users      (984)     2549 2024-04-10 14:37:49.000000 pyvispr-2024.1/pyvispr/flow/functional/socket.py
+-rwx------   0 eric      (1000) users      (984)     2169 2024-04-10 16:31:30.000000 pyvispr-2024.1/pyvispr/flow/messenger.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.856242 pyvispr-2024.1/pyvispr/flow/visual/
+-rwx------   0 eric      (1000) users      (984)    18732 2024-04-11 08:03:57.000000 pyvispr-2024.1/pyvispr/flow/visual/graph.py
+-rw-r--r--   0 eric      (1000) users      (984)     1858 2024-04-10 15:51:00.000000 pyvispr-2024.1/pyvispr/flow/visual/ii_value.py
+-rwx------   0 eric      (1000) users      (984)     6200 2024-04-11 08:06:24.000000 pyvispr-2024.1/pyvispr/flow/visual/link.py
+-rwx------   0 eric      (1000) users      (984)    13012 2024-04-10 15:39:21.000000 pyvispr-2024.1/pyvispr/flow/visual/node.py
+-rwx------   0 eric      (1000) users      (984)     1879 2024-04-10 14:04:53.000000 pyvispr-2024.1/pyvispr/flow/visual/socket.py
+-rwx------   0 eric      (1000) users      (984)     7968 2024-04-10 14:04:53.000000 pyvispr-2024.1/pyvispr/flow/visual/whiteboard.py
+-rwx------   0 eric      (1000) users      (984)     1917 2024-04-10 14:04:53.000000 pyvispr-2024.1/pyvispr/install.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.849575 pyvispr-2024.1/pyvispr/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.856242 pyvispr-2024.1/pyvispr/interface/storage/
+-rwx------   0 eric      (1000) users      (984)     2993 2024-04-10 14:07:15.000000 pyvispr-2024.1/pyvispr/interface/storage/loading.py
+-rwx------   0 eric      (1000) users      (984)     3550 2024-04-10 14:07:15.000000 pyvispr-2024.1/pyvispr/interface/storage/stowing.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.856242 pyvispr-2024.1/pyvispr/interface/window/
+-rwx------   0 eric      (1000) users      (984)    15752 2024-04-10 14:04:53.000000 pyvispr-2024.1/pyvispr/interface/window/installer.py
+-rwx------   0 eric      (1000) users      (984)     1841 2023-12-13 13:55:15.000000 pyvispr-2024.1/pyvispr/interface/window/messenger.py
+-rwx------   0 eric      (1000) users      (984)     7880 2024-04-11 10:10:11.000000 pyvispr-2024.1/pyvispr/interface/window/runner.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.856242 pyvispr-2024.1/pyvispr/interface/window/widget/
+-rwx------   0 eric      (1000) users      (984)    16038 2024-04-10 14:04:53.000000 pyvispr-2024.1/pyvispr/interface/window/widget/function_header.py
+-rwx------   0 eric      (1000) users      (984)     4147 2024-04-10 14:04:53.000000 pyvispr-2024.1/pyvispr/interface/window/widget/list.py
+-rwx------   0 eric      (1000) users      (984)     2533 2024-01-16 14:25:32.000000 pyvispr-2024.1/pyvispr/interface/window/widget/list_file.py
+-rwx------   0 eric      (1000) users      (984)     2458 2024-01-19 20:05:03.000000 pyvispr-2024.1/pyvispr/interface/window/widget/list_function.py
+-rwx------   0 eric      (1000) users      (984)     1925 2024-04-10 14:04:53.000000 pyvispr-2024.1/pyvispr/interface/window/widget/list_module.py
+-rwx------   0 eric      (1000) users      (984)     3818 2024-04-10 14:04:53.000000 pyvispr-2024.1/pyvispr/interface/window/widget/list_node.py
+-rwx------   0 eric      (1000) users      (984)     2412 2024-04-10 14:04:53.000000 pyvispr-2024.1/pyvispr/interface/window/widget/menu.py
+-rwx------   0 eric      (1000) users      (984)     1908 2024-04-11 10:07:56.000000 pyvispr-2024.1/pyvispr/run.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.856242 pyvispr-2024.1/pyvispr/runtime/
+-rw-r--r--   0 eric      (1000) users      (984)     1713 2024-04-10 14:04:53.000000 pyvispr-2024.1/pyvispr/runtime/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)     1625 2024-04-10 13:44:05.000000 pyvispr-2024.1/pyvispr/runtime/catalog.py
+-rw-r--r--   0 eric      (1000) users      (984)     1628 2024-04-10 14:44:17.000000 pyvispr-2024.1/pyvispr/runtime/messenger.py
+-rw-r--r--   0 eric      (1000) users      (984)     1718 2024-04-10 14:44:38.000000 pyvispr-2024.1/pyvispr/runtime/socket.py
+-rwx------   0 eric      (1000) users      (984)     1577 2024-04-11 08:07:41.000000 pyvispr-2024.1/pyvispr/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 11:30:13.856242 pyvispr-2024.1/pyvispr.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     5681 2024-04-11 11:30:13.000000 pyvispr-2024.1/pyvispr.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     2280 2024-04-11 11:30:13.000000 pyvispr-2024.1/pyvispr.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-11 11:30:13.000000 pyvispr-2024.1/pyvispr.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       87 2024-04-11 11:30:13.000000 pyvispr-2024.1/pyvispr.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) users      (984)       99 2024-04-11 11:30:13.000000 pyvispr-2024.1/pyvispr.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)        8 2024-04-11 11:30:13.000000 pyvispr-2024.1/pyvispr.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)       99 2024-04-10 14:52:27.000000 pyvispr-2024.1/requirements.txt
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-11 11:30:13.859575 pyvispr-2024.1/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     8530 2024-04-11 11:30:02.000000 pyvispr-2024.1/setup.py
```

### Comparing `pyvispr-2023.9/PKG-INFO` & `pyvispr-2024.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvispr
-Version: 2023.9
+Version: 2024.1
 Summary: Visual Programming App for Python
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyVispr//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
@@ -12,19 +12,27 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
-Requires-Dist: PyQt6
+Requires-Dist: babelwidget
+Requires-Dist: conf_ini_g
+Requires-Dist: json_any
+Requires-Dist: logger_36
+Requires-Dist: numexpr
+Requires-Dist: numpy
 Requires-Dist: platformdirs
+Requires-Dist: PyQt6
+Requires-Dist: scikit-image
+Requires-Dist: str_to_obj
 
 ..
-   Copyright CNRS/Inria/UCA
+   Copyright CNRS/Inria/UniCA
    Contributor(s): Eric Debreuve (since 2017)
 
    eric.debreuve@cnrs.fr
 
    This software is governed by the CeCILL  license under French law and
    abiding by the rules of distribution of free software.  You can  use,
    modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `pyvispr-2023.9/README-COPYRIGHT-utf8.txt` & `pyvispr-2024.1/README-COPYRIGHT-utf8.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Copyright CNRS/Inria/UCA
+Copyright CNRS/Inria/UniCA
 Contributor(s): Eric Debreuve (since 2017)
 
 eric.debreuve@cnrs.fr
 
 This software is being developed by Eric Debreuve, a CNRS employee and member of team Morpheme.
-Team Morpheme is a joint team between Inria, CNRS, and UCA.
+Team Morpheme is a joint team between Inria, CNRS, and UniCA.
 It is hosted by the Centre Inria d'Université Côte d'Azur, Laboratory I3S, and Laboratory iBV.
 
 CNRS: https://www.cnrs.fr/index.php/en
 Inria: https://www.inria.fr/en/
-UCA: https://univ-cotedazur.eu/
+UniCA: https://univ-cotedazur.eu/
 Centre Inria d'Université Côte d'Azur: https://www.inria.fr/en/centre/sophia/
 I3S: https://www.i3s.unice.fr/en/
 iBV: http://ibv.unice.fr/
 Team Morpheme: https://team.inria.fr/morpheme/
```

### Comparing `pyvispr-2023.9/README-LICENCE-utf8.txt` & `pyvispr-2024.1/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2023.9/README.rst` & `pyvispr-2024.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..
-   Copyright CNRS/Inria/UCA
+   Copyright CNRS/Inria/UniCA
    Contributor(s): Eric Debreuve (since 2017)
 
    eric.debreuve@cnrs.fr
 
    This software is governed by the CeCILL  license under French law and
    abiding by the rules of distribution of free software.  You can  use,
    modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `pyvispr-2023.9/documentation/wiki/description.asciidoc` & `pyvispr-2024.1/documentation/wiki/description.asciidoc`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright CNRS/Inria/UCA
+// Copyright CNRS/Inria/UniCA
 // Contributor(s): Eric Debreuve (since 2017)
 //
 // eric.debreuve@cnrs.fr
 //
 // This software is governed by the CeCILL  license under French law and
 // abiding by the rules of distribution of free software.  You can  use,
 // modify and/ or redistribute the software under the terms of the CeCILL
@@ -35,8 +35,24 @@
 :PROJECT_NAME: pyVispr
 :SHORT_DESCRIPTION: Visual Programming App for Python
 :KEYWORDS: Visual programming, Python
 
 :REPOSITORY_NAME: pyVispr
 :REPOSITORY_USER: eric.debreuve
 :REPOSITORY_SITE: src.koda.cnrs.fr
+:DOCUMENTATION_SITE: -/wikis/home
 :SINCE_YEAR: 2017
+
+:LICENSE_SHORT: CeCILL-2.1
+:LICENCE_LONG: CEA CNRS Inria Logiciel Libre License, version 2.1
+:PY_VERSION: 3.11
+
+// https://pypi.org/classifiers/    Topic::*               # /!\ REMOVE THE PREFIX
+// https://pypi.org/classifiers/    Intended Audience::*   # /!\ REMOVE THE PREFIX
+// https://pypi.org/classifiers/    Development Status::*  # /!\ REMOVE THE PREFIX
+:PYPI_NAME: pyvispr
+:PYPI_TOPIC: Scientific/Engineering
+:PYPI_AUDIENCE: Science/Research
+:PYPI_STATUS: 3 - Alpha
+
+:IMPORT_NAME: pyvispr
+:CONFIG_FOLDER: pyVispr
```

### Comparing `pyvispr-2023.9/pyvispr/__init__.py` & `pyvispr-2024.1/pyvispr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2023.9/pyvispr/catalog/constants.py` & `pyvispr-2024.1/pyvispr/constant/catalog.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,24 +28,15 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 # NODE_NAME: Node name as it will appear in interface.
 # ACTUAL_SOURCE: Where is the node implemented? See node_t.path and node_t.source.
 # FUNCTION_NAME: Node function.
+# INPUT_II_NAMES: Sequence of names with interactive input.
 # OUTPUT_NAMES: Sequence of names.
-# MISSING_IN_INDICATORS: Sequence of booleans indicating the presence of *args and **kwargs arguments.
-# MISSING_IN_HINTS: Sequence of arguments with missing type hint.
-# MISSING_OUT_HINT_INDICATOR: Boolean indicating the presence of output type hint.
-#
-# MISSING_IN_OUT_NAME_PREFIX: With integer postfix, replaces *args and **kwargs in argument list.
-# HINT_PLACEHOLDER: Replaces missing type hints.
 #
 NODE_NAME = "_node_name"
 ACTUAL_SOURCE = "_actual"
 FUNCTION_NAME = "_function_name"
+INPUT_II_NAMES = "_ii_inputs"
 OUTPUT_NAMES = "_outputs"
-MISSING_IN_INDICATORS = "_missing_in"
-MISSING_IN_HINTS = "_missing_in_hint"
-MISSING_OUT_HINT_INDICATOR = "_missing_out_hint"
-MISSING_IN_OUT_NAME_PREFIX = "_missing_"
-HINT_PLACEHOLDER = "no_hint"
```

### Comparing `pyvispr-2023.9/pyvispr/catalog/main.py` & `pyvispr-2024.1/pyvispr/catalog/type.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,31 +27,28 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 
-from pyvispr.config.main import CATALOG_FOLDER
+from pyvispr.config.path import CATALOG_FOLDER
 from pyvispr.flow.descriptive.node import node_t
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
-class _catalog_t(list[node_t]):
+class catalog_t(list[node_t]):
     def __post_init__(self) -> None:
         """"""
-        self.extend(node_t(path=_pth) for _pth in CATALOG_FOLDER.rglob("*.py"))
+        self.extend(map(node_t.NewForPath, CATALOG_FOLDER.rglob("*.py")))
 
     @property
     def node_names(self) -> tuple[str, ...]:
         return tuple(_elm.name for _elm in self)
 
     def NodeDescription(self, node_name: str, /) -> node_t:
         """"""
         for node in self:
             if node.name == node_name:
                 return node
 
         raise ValueError(f"No node with name: {node_name}")
-
-
-NODE_CATALOG = _catalog_t()
```

### Comparing `pyvispr-2023.9/pyvispr/config/appearance/backend.py` & `pyvispr-2024.1/pyvispr/extension/string_.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,12 +25,11 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from babelwidget.main import backend_t
 
-SCREEN_BACKEND_NAME = "pyqt6"
-
-SCREEN_BACKEND = backend_t(name=SCREEN_BACKEND_NAME)
+def SplitAndStriped(text: str, separator: str, /) -> tuple[str, str] | tuple[str, ...]:
+    """"""
+    return tuple(_elm.strip() for _elm in text.split(sep=separator))
```

### Comparing `pyvispr-2023.9/pyvispr/config/appearance/color.py` & `pyvispr-2024.1/pyvispr/config/appearance/color.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,7 +52,10 @@
 INOUT_BRUSH_INACTIVE = QBrush(color_e.dodgerblue)
 
 LINK_PEN_EMPTY = QPen(color_e.dodgerblue, 3, constant_e.PenStyle.DashLine)
 LINK_PEN_FULL = QPen(color_e.dodgerblue, 3, constant_e.PenStyle.SolidLine)
 LINK_BRUSH_ARROW = QBrush(color_e.dodgerblue)
 
 GRID_PEN = QPen(color_e.gainsboro)
+
+ORANGE_BRUSH = QBrush(color_e.orange)
+BLACK_BRUSH = QBrush(color_e.black)
```

### Comparing `pyvispr-2023.9/pyvispr/config/appearance/geometry.py` & `pyvispr-2024.1/pyvispr/config/appearance/geometry.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2023.9/pyvispr/config/main.py` & `pyvispr-2024.1/pyvispr/constant/path.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,10 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import platformdirs as fldr
+from pathlib import Path as path_t
 
-TITLE = "pyVispr"
-
-CONFIG_FOLDER = fldr.user_config_path(appname=TITLE, ensure_exists=True)
-CONFIG_FILE = CONFIG_FOLDER / "config.ini"
-
-CATALOG_FOLDER = CONFIG_FOLDER / "catalog"
+HOME_FOLDER = path_t.home()
```

### Comparing `pyvispr-2023.9/pyvispr/extension/module.py` & `pyvispr-2024.1/pyvispr/config/appearance/behavior.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,10 @@
 # encouraged to load and test the software's suitability as regards their
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
+from __future__ import annotations
 
-from importlib import util
-from pathlib import Path as path_t
-from types import ModuleType as module_t
-
-
-def ModuleForPath(path: path_t, /) -> module_t:
-    """"""
-    path = path_t(path).expanduser()
-    spec = util.spec_from_file_location(path.stem, path)
-    return spec.loader.load_module(spec.name)
+TOO_MANY_SELECTED = 6
```

### Comparing `pyvispr-2023.9/pyvispr/extension/string_.py` & `pyvispr-2024.1/pyvispr/catalog/factory/image_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,11 +25,19 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
+from pathlib import Path as path_t
 
-def SplitAndStriped(text: str, separator: str, /) -> tuple[str, str] | tuple[str, ...]:
-    """"""
-    return tuple(_elm.strip() for _elm in text.split(sep=separator))
+import numpy
+from skimage.io import imread as image_t
+
+
+def pyVisprImageLoader(filename: path_t | str, /) -> numpy.ndarray:
+    """
+    _ii_inputs: filename
+    _outputs: image
+    """
+    return image_t(filename)
```

### Comparing `pyvispr-2023.9/pyvispr/flow/descriptive/socket.py` & `pyvispr-2024.1/pyvispr/flow/messenger.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,53 +25,26 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
-
-import dataclasses as dtcl
+import typing as h
 from enum import Enum as enum_t
-from typing import Any, Sequence
-
-from str_to_obj.type.hint import any_hint_h
-
-
-class assign_when_importing_t:
-    pass
-
-
-class value_not_set_t:
-    pass
-
-
-class invalid_ii_value_t:
-    def __init__(self, issues: Sequence[str], /) -> None:
-        """"""
-        self.issues = issues
-
-
-ASSIGN_WHEN_ACTIVATING = assign_when_importing_t()
-VALUE_NOT_SET = value_not_set_t()
-
-
-class assignment_e(enum_t):
-    """
-    full: link + interactive, user input.
-    """
-
-    link = 0
-    full = 1
 
 
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class input_t:
-    type: any_hint_h | str | assign_when_importing_t = ASSIGN_WHEN_ACTIVATING
-    assignment: assignment_e = assignment_e.link
-    default_value: Any = VALUE_NOT_SET
+class messenger_t(dict[str | enum_t, list[h.Callable]]):
+    def AddCanal(
+        self, name: str | enum_t, AcknowledgeMessage: h.Callable[[...], None]
+    ) -> None:
+        """
+        Canal: From message name to message acknowledgement function.
+        """
+        if name not in self:
+            self[name] = []
+        self[name].append(AcknowledgeMessage)
 
-    @property
-    def has_default(self) -> bool:
+    def TransmitMessage(self, name: str | enum_t, /, *args, **kwargs) -> None:
         """"""
-        return self.default_value is not VALUE_NOT_SET
+        for AcknowledgeMessage in self.get(name, ()):
+            AcknowledgeMessage(*args, **kwargs)
```

### Comparing `pyvispr-2023.9/pyvispr/flow/functional/graph.py` & `pyvispr-2024.1/pyvispr/flow/functional/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,27 +168,16 @@
                             script_accessor.write(
                                 node.UniqueOutputName(output_names[idx]) + ", "
                             )
                     script_accessor.write(
                         node.UniqueOutputName(output_names[-1]) + " = "
                     )
 
-                output_values = node.Run(script_accessor=script_accessor)
-
-                if n_outputs > 1:
-                    for name, value in zip(output_names, output_values):
-                        node.SetOutputValue(name, value)
-                elif n_outputs > 0:
-                    node.SetOutputValue(output_names[0], output_values)
-
-                for output_name, per_out_links in node.links.items():
-                    output_value = node.outputs[output_name].value
-
-                    for next_node, next_in_name in per_out_links:
-                        next_node.SetInputValue(next_in_name, output_value)
+                node.Run(script_accessor=script_accessor)
+                node.SendOutputsToSuccessors()
 
             nodes_to_be_run.difference_update(runnable_nodes)
 
         if (n_to_be_run > 0) and should_save_as_script:
             script_accessor.write(
                 'print("Workflow saving was incomplete due to some nodes not being runnable.")'
             )
```

### Comparing `pyvispr-2023.9/pyvispr/flow/functional/link.py` & `pyvispr-2024.1/pyvispr/flow/functional/link.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2023.9/pyvispr/flow/functional/node_isolated.py` & `pyvispr-2024.1/pyvispr/flow/functional/node_isolated.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,19 @@
 from __future__ import annotations
 
 import dataclasses as dtcl
 import typing as h
 from enum import Enum as enum_t
 
 from json_any import JsonStringOf
-
+from logger_36 import LOGGER
+from pyvispr.constant.socket import OUTPUT_SET, OUTPUT_UNSET
 from pyvispr.flow.descriptive.node import node_t as description_t
 from pyvispr.flow.functional.socket import input_t, output_t
-from pyvispr.flow.messenger import MESSENGER
+from pyvispr.runtime.messenger import MESSENGER
 
 
 class state_e(enum_t):
     disabled = 1
     todo = 2
     running = 3
     done = 4
@@ -102,48 +103,52 @@
                 continue
 
             source, output_name = source_output_name.split(
                 node_t.UNIQUE_OUTPUT_NAME_SEPARATOR
             )
             name, uid = source.split(node_t.UNIQUE_NAME_SEPARATOR)
             uid = int(uid) + offset
-            input_.source_output_name = f"{name}{node_t.UNIQUE_NAME_SEPARATOR}{uid}{node_t.UNIQUE_OUTPUT_NAME_SEPARATOR}{output_name}"
+            input_.source_output_name = (
+                f"{name}{node_t.UNIQUE_NAME_SEPARATOR}"
+                f"{uid}{node_t.UNIQUE_OUTPUT_NAME_SEPARATOR}"
+                f"{output_name}"
+            )
 
     def InvalidateInputValue(self, /, *, name: str | None = None) -> None:
         """"""
         if self.state is state_e.disabled:
             return
 
         if name is None:
             for input_ in self.inputs.values():
                 input_.Invalidate()
         else:
             self.inputs[name].Invalidate()
         self.state = state_e.todo
-        MESSENGER.TransmitMessage(state_e.todo, (self,))
+        MESSENGER.TransmitMessage(state_e.todo, self)
 
     def InvalidateOutputValues(self) -> None:
         """"""
         if self.state is state_e.disabled:
             return
 
         for output in self.outputs.values():
             output.Invalidate()
         self.state = state_e.todo
-        MESSENGER.TransmitMessage(state_e.todo, (self,))
-        MESSENGER.TransmitMessage("output unset", (self,))
+        MESSENGER.TransmitMessage(state_e.todo, self)
+        MESSENGER.TransmitMessage(OUTPUT_UNSET, self)
 
     def ToggleAbility(self) -> None:
         """"""
         if self.state is state_e.disabled:
             self.state = state_e.todo
-            MESSENGER.TransmitMessage(state_e.todo, (self,))
+            MESSENGER.TransmitMessage(state_e.todo, self)
         else:
             self.state = state_e.disabled
-            MESSENGER.TransmitMessage(state_e.disabled, (self,))
+            MESSENGER.TransmitMessage(state_e.disabled, self)
 
     @property
     def can_run(self) -> bool:
         """
         It must have been checked that the state is not disabled.
 
         This method is meant to be called from functional.graph.Run,
@@ -153,20 +158,20 @@
         not "link") and they are not linked to outputs.
         """
         return (self.description.n_inputs == 0) or all(
             self.inputs[_elm].has_value or self.description.inputs[_elm].has_default
             for _elm in self.inputs
         )
 
-    def Run(self, /, *, script_accessor: h.TextIO = None) -> h.Any | None:
+    def Run(self, /, *, script_accessor: h.TextIO = None) -> None:
         """
         It must have been checked that the state is not disabled.
         """
         self.state = state_e.running
-        MESSENGER.TransmitMessage(state_e.running, (self,))
+        MESSENGER.TransmitMessage(state_e.running, self)
 
         should_save_as_script = script_accessor is not None
 
         if should_save_as_script:
             if self.description.n_outputs > 1:
                 output_assignments = (
                     self.UniqueOutputName(_elm) for _elm in self.outputs
@@ -207,60 +212,68 @@
                     anonymous_args.append(value)
                     if should_save_as_script:
                         anonymous_args_script.append(value_script)
 
             if should_save_as_script:
                 arguments = ", ".join(anonymous_args_script + named_args_script)
                 script_accessor.write(
-                    f"{output_assignments}{self.description.function_name}({arguments})\n"
+                    f"{output_assignments}{self.description.module.__name__}_"
+                    f"{self.description.actual.name}({arguments})\n"
                 )
                 output_values = _FakeOutputs(self.description.n_outputs, "Done")
             else:
-                output_values = self._RunSafely(anonymous_args, named_args)
+                output_values = self._SafeOutputValues(anonymous_args, named_args)
         elif should_save_as_script:
             script_accessor.write(
-                f"{output_assignments}{self.description.function_name}()\n"
+                f"{output_assignments}{self.description.module.__name__}_{self.description.actual.name}()\n"
             )
             output_values = _FakeOutputs(self.description.n_outputs, "Done")
         else:
-            output_values = self._RunSafely(None, None)
+            output_values = self._SafeOutputValues(None, None)
 
-        self.state = state_e.done
-        MESSENGER.TransmitMessage(state_e.done, (self,))
+        # Since output values are computed here, it makes more sense to directly set them, as opposed to returning them
+        # and letting the caller doing it. Hence, _SetOutputValue is meant for internal use, whereas SetInputValue is
+        # meant for external use.
+        output_names = self.description.output_names
+        n_outputs = output_names.__len__()
+        if n_outputs > 1:
+            for name, value in zip(output_names, output_values):
+                self._SetOutputValue(name, value)
+        elif n_outputs > 0:
+            self._SetOutputValue(output_names[0], output_values)
 
-        return output_values
+        self.state = state_e.done
+        MESSENGER.TransmitMessage(state_e.done, self)
 
-    def _RunSafely(
+    def _SafeOutputValues(
         self,
         anonymous_args: h.Sequence[h.Any] | None,
         named_args: dict[str, h.Any] | None,
         /,
     ) -> h.Any | None:
         """"""
         try:
             if anonymous_args is None:
                 output = self.description.Function()
             else:
                 output = self.description.Function(*anonymous_args, **named_args)
         except Exception as exception:
             output = _FakeOutputs(self.description.n_outputs, None)
-            print(f"Exception while running {self.unique_name}:", exception)
+            LOGGER.error(f"Error while running {self.unique_name}:\n{exception}")
 
         return output
 
-    # TODO: Re-think the value setting (here hidden, partially explicit in node_linked), maybe with
-    #     a TransmitValue from out to in method.
     def SetInputValue(self, name: str, value: h.Any, /) -> None:
         """"""
         self.inputs[name].value = value
 
-    def SetOutputValue(self, name: str, value: h.Any, /) -> None:
+    def _SetOutputValue(self, name: str, value: h.Any, /) -> None:
         """"""
         self.outputs[name].value = value
-        MESSENGER.TransmitMessage("output set", (self,))
+        MESSENGER.TransmitMessage(OUTPUT_SET, self)
 
 
 def _EncodedValue(value: h.Any, /) -> str:
     """"""
     as_str, issues = JsonStringOf(value)
     if issues is None:
         as_str = as_str.replace('"', '\\"')
```

### Comparing `pyvispr-2023.9/pyvispr/flow/functional/node_linked.py` & `pyvispr-2024.1/pyvispr/flow/functional/node_linked.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,7 +81,13 @@
         if self.description.n_outputs == 0:
             return True
 
         return any(
             self.OutputIsLinked(_nme) and (not _rcd.has_value)
             for _nme, _rcd in self.outputs.items()
         )
+
+    def SendOutputsToSuccessors(self) -> None:
+        """"""
+        for name, output in self.outputs.items():
+            for next_node, next_in_name in self.links[name]:
+                next_node.SetInputValue(next_in_name, output.value)
```

### Comparing `pyvispr-2023.9/pyvispr/flow/functional/socket.py` & `pyvispr-2024.1/pyvispr/flow/functional/socket.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 import typing as h
 
-from pyvispr.flow.descriptive.socket import VALUE_NOT_SET
+from pyvispr.runtime.socket import VALUE_NOT_SET
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
 class _base_t:
     value: h.Any = VALUE_NOT_SET
 
     @property
```

### Comparing `pyvispr-2023.9/pyvispr/flow/messenger.py` & `pyvispr-2024.1/pyvispr/runtime/socket.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,31 +25,20 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import typing as h
-from enum import Enum as enum_t
 
+class assign_when_importing_t:
+    pass
 
-class messenger_t(dict[str | enum_t, list[h.Callable]]):
-    def AddCanal(
-        self, name: str | enum_t, AcknowledgeMessage: h.Callable[[...], None]
-    ) -> None:
-        """
-        Canal: From message to message acknowledgement function.
-        """
-        if name not in self:
-            self[name] = []
-        self[name].append(AcknowledgeMessage)
-
-    def TransmitMessage(
-        self, name: str | enum_t, content: tuple[h.Any, ...], /
-    ) -> None:
-        """"""
-        for AcknowledgeMessage in self.get(name, ()):
-            AcknowledgeMessage(*content)
 
+ASSIGN_WHEN_ACTIVATING = assign_when_importing_t()
 
-MESSENGER = messenger_t()
+
+class value_not_set_t:
+    pass
+
+
+VALUE_NOT_SET = value_not_set_t()
```

### Comparing `pyvispr-2023.9/pyvispr/flow/visual/graph.py` & `pyvispr-2024.1/pyvispr/flow/visual/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,41 +33,43 @@
 
 import dataclasses as dtcl
 import typing as h
 from datetime import datetime as date_time_t
 
 import PyQt6.QtWidgets as wdgt
 from conf_ini_g.phase.specification.parameter.type import type_t
+from logger_36 import LOGGER
 from PyQt6.QtCore import QCoreApplication, QPoint, QRectF
-from str_to_obj.task.comparison import TypesAreCompatible
-
-from pyvispr.catalog.main import NODE_CATALOG
 from pyvispr.config.appearance.color import (
     BUTTON_BRUSH_STATE_DISABLED,
     BUTTON_BRUSH_STATE_DOING,
     BUTTON_BRUSH_STATE_DONE,
     BUTTON_BRUSH_STATE_TODO,
     INOUT_BRUSH_ACTIVE,
     INOUT_BRUSH_INACTIVE,
     LINK_PEN_EMPTY,
     LINK_PEN_FULL,
     NODE_BRUSH_RESTING,
     NODE_BRUSH_RUNNING,
     QBrush,
     QPen,
 )
-from pyvispr.flow.descriptive.socket import VALUE_NOT_SET, invalid_ii_value_t
+from pyvispr.constant.socket import OUTPUT_SET, OUTPUT_UNSET
 from pyvispr.flow.functional.graph import graph_t as graph_functional_t
 from pyvispr.flow.functional.node_isolated import state_e
 from pyvispr.flow.functional.node_linked import node_t as functional_t
-from pyvispr.flow.messenger import MESSENGER
+from pyvispr.flow.visual.ii_value import invalid_ii_value_t
 from pyvispr.flow.visual.link import link_t
 from pyvispr.flow.visual.node import node_t
 from pyvispr.flow.visual.socket import active_socket_t
 from pyvispr.interface.window.messenger import CreateMessageCanal
+from pyvispr.runtime.catalog import NODE_CATALOG
+from pyvispr.runtime.messenger import MESSENGER
+from pyvispr.runtime.socket import VALUE_NOT_SET
+from str_to_obj.task.comparison import TypesAreCompatible
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
 class graph_t(wdgt.QGraphicsScene):
     functional: graph_functional_t = dtcl.field(
         init=False, default_factory=graph_functional_t
     )
@@ -87,16 +89,16 @@
 
         CreateMessageCanal(self, "changed", self.UpdateLinks)
 
         MESSENGER.AddCanal(state_e.disabled, self.AcknowledgeDisabled)
         MESSENGER.AddCanal(state_e.todo, self.AcknowledgeToDo)
         MESSENGER.AddCanal(state_e.running, self.AcknowledgeRunningStarted)
         MESSENGER.AddCanal(state_e.done, self.AcknowledgeRunningEnded)
-        MESSENGER.AddCanal("output set", self.AcknowledgeLinkFull)
-        MESSENGER.AddCanal("output unset", self.AcknowledgeLinkEmpty)
+        MESSENGER.AddCanal(OUTPUT_SET, self.AcknowledgeLinkFull)
+        MESSENGER.AddCanal(OUTPUT_UNSET, self.AcknowledgeLinkEmpty)
 
     @classmethod
     def __NewFromJsonDescription__(cls, description, /) -> graph_t:
         """"""
         output = cls()
 
         for name, unique_name, ii_values, position_x, position_y in description[0]:
@@ -126,16 +128,14 @@
         self,
     ) -> tuple[
         tuple[tuple[str, str, dict[str, h.Any], float, float], ...],
         tuple[tuple, ...],
         int,
     ]:
         """"""
-        # TODO: If _elm.IIValue() contains invalid_ii_value_t instances, then
-        #     jsonization will fail.
         return (
             tuple(
                 (
                     _elm.functional.description.name,
                     _elm.functional.unique_name,
                     _elm.IIValue(),
                     _elm.x(),
@@ -154,19 +154,19 @@
             self.functional.next_node_uid,
         )
 
     def AddNode(self, name: str, /) -> None:
         """"""
         description = NODE_CATALOG.NodeDescription(name)
         if description.requires_completion:
-            print(f"{description.name} : Requires Completion.")
+            LOGGER.warning(f"Node {description.name} requires completion")
         functional = functional_t.NewForDescription(description)
         self.functional.AddNode(functional)
 
-        node = node_t(functional=functional)
+        node = node_t.NewForFunctional(functional)
         self.nodes.append(node)
 
         self.clearSelection()  # Otherwise the newly created visual node replaces the selection.
         self.addItem(node)
         self.addItem(node.ii_dialog)
 
     def AddLinkMaybe(
@@ -189,15 +189,15 @@
                 button = node.in_btn
             if possible_names.__len__() > 1:
                 selected = _SocketSelection(possible_names, position)
             else:
                 selected = possible_names[0]
             if selected is not None:
                 stripe = sockets[selected]
-                if not isinstance(stripe, type_t):
+                if not node_is_source:
                     stripe = stripe.type
                 self._active_socket.node = node
                 self._active_socket.is_source = node_is_source
                 self._active_socket.name = selected
                 self._active_socket.type = stripe
                 button.setBrush(INOUT_BRUSH_ACTIVE)
 
@@ -270,18 +270,22 @@
         input_name: str,
         /,
     ) -> None:
         """"""
         self.functional.AddLink(
             source.functional, output_name, target.functional, input_name
         )
-        if not any(
-            (_lnk.source_node is source) and (_lnk.target_node is target)
-            for _lnk in self.links
-        ):
+        found = None
+        for link in self.links:
+            if (link.source_node is source) and (link.target_node is target):
+                found = link
+                break
+        if found:
+            found.SetTooltip()
+        else:
             link = link_t(
                 source_node=source,
                 source_point=source.output_anchor_coordinates,
                 target_node=target,
                 target_point=target.input_anchor_coordinates,
             )
             self.links.append(link)
@@ -329,30 +333,26 @@
             )
             should_be_actually_removed = link.UnderlyingFunctionals().__len__() == 0
 
         if should_be_actually_removed:
             self.links.remove(link)
             self.removeItem(link)
             self.removeItem(link.arrow)
+        else:
+            link.SetTooltip()
 
     def UpdateLinks(self, _: h.Sequence[QRectF], /) -> None:
         """"""
         for node in self.selectedItems():
             if isinstance(node, node_t) and node.position_has_changed:
                 for link in self.links:
-                    if node is link.source_node:
-                        link.SetPath(
-                            link.source_node.output_anchor_coordinates,
-                            link.target_point,
-                        )
-                    elif node is link.target_node:
-                        link.SetPath(
-                            link.source_point,
-                            link.target_node.input_anchor_coordinates,
-                        )
+                    link.SetPath(
+                        link.source_node.output_anchor_coordinates,
+                        link.target_node.input_anchor_coordinates,
+                    )
                 node.position_has_changed = False
 
     def MergeWith(self, other: graph_t, /) -> None:
         """"""
         offset = self.functional.next_node_uid - 1
         for node in other.nodes:
             node.functional.OffsetUnicity(offset)
@@ -392,28 +392,27 @@
             )
 
         for node in self.nodes:
             functional = node.functional
             if should_save_as_script:
                 description = functional.description
                 script_accessor.write(
-                    f"""path = path_t("{description.path}").expanduser()
+                    f"""path = path_t("{description.actual.path}").expanduser()
 spec = util.spec_from_file_location(path.stem, path)
 module = spec.loader.load_module(spec.name)
-{description.function_name} = getattr(module, "{description.function_name}")\n
+{description.module.__name__}_{description.actual.name} = getattr(module, "{description.actual.name}")\n
 """
                 )
 
             for input_name in functional.inputs:
                 if (value := node.IIValue(input_name)) is VALUE_NOT_SET:
                     continue
 
                 if isinstance(value, invalid_ii_value_t):
-                    # TODO: Replace exception with proper logging.
-                    raise RuntimeError("Log issues for later review.")
+                    pass  # Issues are stored in value.issues.
                 else:
                     functional.SetInputValue(input_name, value)
 
         un_run_nodes = self.functional.Run(script_accessor=script_accessor)
 
         if should_save_as_script:
             self.functional.InvalidateAllNodes()
```

### Comparing `pyvispr-2023.9/pyvispr/flow/visual/link.py` & `pyvispr-2024.1/pyvispr/flow/visual/link.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 
 import PyQt6.QtWidgets as wdgt
 from PyQt6.QtCore import QPoint, QPointF
 from PyQt6.QtGui import QPainterPath, QPolygonF
-
 from pyvispr.config.appearance.color import (
     LINK_BRUSH_ARROW,
     LINK_PEN_EMPTY,
     LINK_PEN_FULL,
 )
 from pyvispr.config.appearance.geometry import LINK_MIN_HORIZONTAL_SHIFT
 from pyvispr.flow.visual.node import node_t
@@ -51,23 +50,23 @@
     path from mouse events: when clicked the scene items are the group (not of interest) and the path (of interest), but
     as a path item instead of a link_t.
     """
 
     source_node: node_t
     target_node: node_t
     arrow: wdgt.QGraphicsPolygonItem | None = None
-    # TODO: Certainly no need to store these, at least target_point.
-    source_point: QPointF | None = None
-    target_point: QPointF | None = None
+    source_point: dtcl.InitVar[QPointF | None] = None
+    target_point: dtcl.InitVar[QPointF | None] = None
 
-    def __post_init__(self) -> None:
+    def __post_init__(
+        self, source_point: QPointF | None, target_point: QPointF | None
+    ) -> None:
         """"""
         # Otherwise, complaint about super-init not having been called.
         wdgt.QGraphicsPathItem.__init__(self)
-        self.setZValue(1)
 
         arrow = QPolygonF()
         arrow.append(QPointF(10, 0))
         arrow.append(QPointF(0, 10))
         arrow.append(QPointF(0, -10))
         arrow.append(QPointF(10, 0))
         self.arrow = wdgt.QGraphicsPolygonItem(arrow)
@@ -77,32 +76,31 @@
 
         if self.source_node.functional.needs_running:
             pen = LINK_PEN_EMPTY
         else:
             pen = LINK_PEN_FULL
         self.setPen(pen)
 
-        self.SetPath(self.source_point, self.target_point, is_creation=True)
-        self.setToolTip(
-            "\n".join(f"{_elm[0]} ⮞ {_elm[1]}" for _elm in self.UnderlyingFunctionals())
-        )
+        self.SetPath(source_point, target_point, is_creation=True)
+        self.SetTooltip()
+        self.setZValue(1)
 
     def SetPath(
         self,
         source_point: QPointF,
         target_point: QPointF,
         /,
         *,
         is_creation: bool = False,
     ) -> None:
         """"""
         if is_creation:
             translation = source_point
         else:
-            translation = source_point - self.source_point
+            translation = source_point - QPointF(self.path().elementAt(0))
         polygon = self.arrow.polygon()
         polygon.translate(translation)
         self.arrow.setPolygon(polygon)
 
         tangent = 0.4 * (target_point - source_point)
         tangent.setY(0)
         if tangent.x() < 0:
@@ -110,16 +108,19 @@
         if tangent.x() < LINK_MIN_HORIZONTAL_SHIFT:
             tangent.setX(LINK_MIN_HORIZONTAL_SHIFT)
 
         path = QPainterPath(source_point)
         path.cubicTo(source_point + tangent, target_point - tangent, target_point)
         self.setPath(path)
 
-        self.source_point = source_point
-        self.target_point = target_point
+    def SetTooltip(self) -> None:
+        """"""
+        self.setToolTip(
+            "\n".join(f"{_elm[0]} ⮞ {_elm[1]}" for _elm in self.UnderlyingFunctionals())
+        )
 
     def UnderlyingFunctionals(self) -> tuple[tuple[str, str], ...]:
         """"""
         output = []
 
         source = self.source_node.functional
         target = self.target_node.functional
@@ -130,15 +131,15 @@
 
         return tuple(output)
 
     def LinksToBeRemoved(
         self, position: QPoint, /
     ) -> tuple[tuple[str, str] | None, bool] | None:
         """
-        /!\ Strange behavior (Qt bug?): Sometimes a mouse press on a different link (or even in the background)
+        /!\\ Strange behavior (Qt bug?): Sometimes a mouse press on a different link (or even in the background)
         calls the mousePressEvent callback of the previously pressed link; and this repeats several times,
         until clicking far away from any link!!!
         """
         menu = wdgt.QMenu()
         cancel_action = menu.addAction("Close Menu")
         no_action = menu.addAction("or Remove Link(s):")
         no_action.setEnabled(False)
```

### Comparing `pyvispr-2023.9/pyvispr/flow/visual/node.py` & `pyvispr-2024.1/pyvispr/flow/visual/node.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,155 +25,185 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
+from __future__ import annotations
+
 import dataclasses as dtcl
 import typing as h
 
 import PyQt6.QtWidgets as wdgt
 from conf_ini_g.interface.window.parameter.main import TypeAndValueWidgetsForType
+from conf_ini_g.phase.specification.parameter.type import type_t
+from logger_36 import LOGGER
 from PyQt6.QtCore import QPointF, QRectF
-
-from pyvispr.config.appearance.backend import SCREEN_BACKEND
 from pyvispr.config.appearance.color import (
     BUTTON_BRUSH_CONFIG,
     BUTTON_BRUSH_REMOVE,
     BUTTON_BRUSH_STATE_TODO,
     INOUT_BRUSH_INACTIVE,
     NODE_BRUSH_RESTING,
     NODE_BRUSH_SELECTED,
     color_e,
 )
 from pyvispr.config.appearance.geometry import (
     BUTTON_WIDTH,
     NODE_HEIGHT_TOTAL,
     NODE_WIDTH_TOTAL,
 )
-from pyvispr.flow.descriptive.socket import (
-    VALUE_NOT_SET,
-    assignment_e,
-    invalid_ii_value_t,
-    value_not_set_t,
+from pyvispr.constant.widget.node import (
+    HEIGHT_OF_BOTTOM_BUTTONS,
+    HEIGHT_OF_LATERAL_BUTTONS,
+    HORIZONTAL_FREE_SPACE,
+    TOP_OF_BOTTOM_BUTTONS,
+    WIDTH_OF_LATERAL_BUTTONS,
 )
+from pyvispr.flow.descriptive.socket import assignment_e
 from pyvispr.flow.functional.node_linked import node_t as functional_t
+from pyvispr.flow.visual.ii_value import invalid_ii_value_t
+from pyvispr.runtime.backend import SCREEN_BACKEND
+from pyvispr.runtime.socket import VALUE_NOT_SET, value_not_set_t
+from str_to_obj import annotation_t
+
+
+class ii_widget_p(wdgt.QWidget):
+    def Assign(
+        self,
+        value: h.Any,
+        stripe: type_t | annotation_t | None,
+    ) -> None: ...
+
+    def Text(self) -> str: ...
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
 class node_t(wdgt.QGraphicsRectItem):
     functional: functional_t
-    label = None
-    in_btn = None
-    out_btn = None
-    config_btn = None
-    state_btn = None
-    remove_btn = None
-
-    position_has_changed: bool = False
-
-    interactive_inputs: dict[str, wdgt.QWidget] | None = None
-    ii_dialog: wdgt.QGraphicsProxyWidget | None = None
+    label: wdgt.QGraphicsTextItem
+    in_btn: wdgt.QGraphicsRectItem | None
+    out_btn: wdgt.QGraphicsRectItem | None
+    config_btn: wdgt.QGraphicsRectItem
+    state_btn: wdgt.QGraphicsRectItem
+    remove_btn: wdgt.QGraphicsRectItem
+    ii_dialog: wdgt.QGraphicsProxyWidget
+
+    interactive_inputs: dict[str, ii_widget_p] | None = dtcl.field(
+        init=False, default=None
+    )
+    position_has_changed: bool = dtcl.field(init=False, default=False)
 
     def __post_init__(self) -> None:
         """"""
-        # If using: self.setRect(QRectF(0, 0, NODE_WIDTH_TOTAL, NODE_HEIGHT_TOTAL)), Python complains about super-init not
-        # having been called.
+        # If using: self.setRect(QRectF(0, 0, NODE_WIDTH_TOTAL, NODE_HEIGHT_TOTAL)), Python complains about super-init
+        # not having been called.
         wdgt.QGraphicsRectItem.__init__(
             self, QRectF(0, 0, NODE_WIDTH_TOTAL, NODE_HEIGHT_TOTAL)
         )
-        self.SetupAndCreateElements()
-        self.setZValue(2)
-        self.setSelected(True)
 
-    def SetupAndCreateElements(self) -> None:
-        """"""
+        for item in (
+            self.label,
+            self.in_btn,
+            self.out_btn,
+            self.config_btn,
+            self.state_btn,
+            self.remove_btn,
+        ):
+            if item is not None:
+                item.setParentItem(self)
+
         self.setFlag(wdgt.QGraphicsItem.GraphicsItemFlag.ItemIsSelectable)
         self.setFlag(wdgt.QGraphicsItem.GraphicsItemFlag.ItemIsMovable)
         self.setFlag(wdgt.QGraphicsItem.GraphicsItemFlag.ItemClipsChildrenToShape)
         self.setFlag(wdgt.QGraphicsItem.GraphicsItemFlag.ItemSendsGeometryChanges)
-        self.setToolTip(self.details)
         self.setBrush(NODE_BRUSH_RESTING)
+        self.setZValue(2)
+
+        self.config_btn.setToolTip(self.details)
 
-        label = wdgt.QGraphicsTextItem(self)
-        label.setHtml(self.functional.unique_name)
+        self.setSelected(True)
+
+    @classmethod
+    def NewForFunctional(cls, functional: functional_t, /) -> node_t:
+        """"""
+        label = wdgt.QGraphicsTextItem()
+        label.setHtml(functional.unique_name)
         label.setPos(BUTTON_WIDTH, 0)
         label.setTextWidth(NODE_WIDTH_TOTAL - 2 * BUTTON_WIDTH)
         # Causes a crash!
         # label.setTextInteractionFlags(constant_e.ItemSelectionMode.TextSelectableByMouse)
-        self.label = label
-
-        width_of_lateral_buttons = BUTTON_WIDTH
-        height_of_lateral_buttons = NODE_HEIGHT_TOTAL
 
-        top_of_bottom_buttons = NODE_HEIGHT_TOTAL - BUTTON_WIDTH
-        height_of_bottom_buttons = BUTTON_WIDTH
-
-        if self.functional.description.n_inputs > 0:
-            self.in_btn = wdgt.QGraphicsRectItem(
-                QRectF(0, 0, width_of_lateral_buttons, height_of_lateral_buttons),
-                self,
+        if functional.description.n_inputs > 0:
+            in_btn = wdgt.QGraphicsRectItem(
+                QRectF(0, 0, WIDTH_OF_LATERAL_BUTTONS, HEIGHT_OF_LATERAL_BUTTONS)
             )
-            self.in_btn.setBrush(INOUT_BRUSH_INACTIVE)
+            in_btn.setBrush(INOUT_BRUSH_INACTIVE)
         else:
-            self.in_btn = None
+            in_btn = None
 
-        if self.functional.description.n_outputs > 0:
-            self.out_btn = wdgt.QGraphicsRectItem(
+        if functional.description.n_outputs > 0:
+            out_btn = wdgt.QGraphicsRectItem(
                 QRectF(
-                    NODE_WIDTH_TOTAL - width_of_lateral_buttons,
+                    NODE_WIDTH_TOTAL - WIDTH_OF_LATERAL_BUTTONS,
                     0,
-                    width_of_lateral_buttons,
-                    height_of_lateral_buttons,
-                ),
-                self,
+                    WIDTH_OF_LATERAL_BUTTONS,
+                    HEIGHT_OF_LATERAL_BUTTONS,
+                )
             )
-            self.out_btn.setBrush(INOUT_BRUSH_INACTIVE)
+            out_btn.setBrush(INOUT_BRUSH_INACTIVE)
         else:
-            self.out_btn = None
+            out_btn = None
 
-        horizontal_free_space = NODE_WIDTH_TOTAL - 2 * width_of_lateral_buttons
-        config_btn_width = int(horizontal_free_space / 2.5)
-        self.config_btn = wdgt.QGraphicsRectItem(
+        config_btn_width = int(HORIZONTAL_FREE_SPACE / 2.5)
+        config_btn = wdgt.QGraphicsRectItem(
             QRectF(
-                width_of_lateral_buttons,
-                top_of_bottom_buttons,
+                WIDTH_OF_LATERAL_BUTTONS,
+                TOP_OF_BOTTOM_BUTTONS,
                 config_btn_width,
-                height_of_bottom_buttons,
-            ),
-            self,
+                HEIGHT_OF_BOTTOM_BUTTONS,
+            )
         )
-        self.config_btn.setBrush(BUTTON_BRUSH_CONFIG)
+        config_btn.setBrush(BUTTON_BRUSH_CONFIG)
 
-        self.state_btn = wdgt.QGraphicsRectItem(
+        state_btn = wdgt.QGraphicsRectItem(
             QRectF(
-                width_of_lateral_buttons + config_btn_width,
-                top_of_bottom_buttons,
+                WIDTH_OF_LATERAL_BUTTONS + config_btn_width,
+                TOP_OF_BOTTOM_BUTTONS,
                 config_btn_width,
-                height_of_bottom_buttons,
-            ),
-            self,
+                HEIGHT_OF_BOTTOM_BUTTONS,
+            )
         )
-        self.state_btn.setToolTip("Needs Running")
-        self.state_btn.setBrush(BUTTON_BRUSH_STATE_TODO)
+        state_btn.setToolTip("Needs Running")
+        state_btn.setBrush(BUTTON_BRUSH_STATE_TODO)
 
-        self.remove_btn = wdgt.QGraphicsRectItem(
+        remove_btn = wdgt.QGraphicsRectItem(
             QRectF(
-                width_of_lateral_buttons + 2 * config_btn_width,
-                top_of_bottom_buttons,
-                horizontal_free_space - 2 * config_btn_width,
-                height_of_bottom_buttons,
-            ),
-            self,
+                WIDTH_OF_LATERAL_BUTTONS + 2 * config_btn_width,
+                TOP_OF_BOTTOM_BUTTONS,
+                HORIZONTAL_FREE_SPACE - 2 * config_btn_width,
+                HEIGHT_OF_BOTTOM_BUTTONS,
+            )
         )
-        self.remove_btn.setBrush(BUTTON_BRUSH_REMOVE)
+        remove_btn.setBrush(BUTTON_BRUSH_REMOVE)
+
+        ii_dialog = wdgt.QGraphicsProxyWidget()
+        ii_dialog.setZValue(2)
 
-        self.ii_dialog = wdgt.QGraphicsProxyWidget()
-        self.ii_dialog.setZValue(2)
+        return cls(
+            functional=functional,
+            label=label,
+            in_btn=in_btn,
+            out_btn=out_btn,
+            config_btn=config_btn,
+            state_btn=state_btn,
+            remove_btn=remove_btn,
+            ii_dialog=ii_dialog,
+        )
 
     def AlignOnGrid(self) -> None:
         """"""
         position_x, position_y = (
             round(self.x() / NODE_WIDTH_TOTAL) * NODE_WIDTH_TOTAL,
             round(self.y() / NODE_HEIGHT_TOTAL) * NODE_HEIGHT_TOTAL,
         )
@@ -200,15 +230,17 @@
         return output
 
     @property
     def details(self) -> str:
         """"""
         functional = self.functional
 
-        output = [f"Function: {functional.description.function_name}"]
+        output = [
+            f"Function: {functional.description.module.__name__}.{functional.description.actual.name}"
+        ]
 
         if functional.description.n_inputs > 0:
             output.append("Input(s):")
             for name, input_ in functional.description.inputs.items():
                 if input_.has_default:
                     default = f" = {input_.default_value}"
                 else:
@@ -304,14 +336,15 @@
                 input_name in interactive_inputs
             ):
                 value_as_str = interactive_inputs[input_name].Text()
                 expected_type = functional.description.inputs[input_name].type
                 value, issues = expected_type.InterpretedValueOf(value_as_str)
                 if issues.__len__() > 0:
                     value = invalid_ii_value_t(issues)
+                    LOGGER.error("\n".join(issues))
             else:
                 value = VALUE_NOT_SET
             output[input_name] = value
 
         if stripe is dict:
             return output
         if stripe is tuple:
```

### Comparing `pyvispr-2023.9/pyvispr/flow/visual/socket.py` & `pyvispr-2024.1/pyvispr/flow/visual/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,16 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 
-from str_to_obj.type.hint import any_hint_h
-
 from pyvispr.flow.visual.node import node_t
+from str_to_obj.type.hint import any_hint_h
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
 class active_socket_t:
     node: node_t | None = None
     is_source: bool | None = None
     name: str | None = None
```

### Comparing `pyvispr-2023.9/pyvispr/flow/visual/whiteboard.py` & `pyvispr-2024.1/pyvispr/flow/visual/whiteboard.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
 import dataclasses as dtcl
 import typing as h
 
 import PyQt6.QtWidgets as wdgt
 from PyQt6.QtCore import Qt as constant_e
 from PyQt6.QtGui import QMouseEvent, QPainter
-
 from pyvispr.config.appearance.color import GRID_PEN
 from pyvispr.config.appearance.geometry import (
     NODE_HEIGHT_TOTAL,
     NODE_WIDTH_TOTAL,
     WHITEBOARD_HEIGHT,
     WHITEBOARD_WIDTH,
 )
@@ -56,14 +55,15 @@
     grid: wdgt.QGraphicsItemGroup = dtcl.field(init=False, default=None)
     graph: graph_t = dtcl.field(init=False, default=None)
 
     def __post_init__(self) -> None:
         """"""
         # Otherwise, complaint about super-init not having been called.
         wdgt.QGraphicsView.__init__(self)
+
         self.setMinimumSize(WHITEBOARD_WIDTH, WHITEBOARD_HEIGHT)
         self.setSizePolicy(
             wdgt.QSizePolicy.Policy.MinimumExpanding,
             wdgt.QSizePolicy.Policy.MinimumExpanding,
         )
         self.setRenderHint(QPainter.RenderHint.Antialiasing)
         # Used to not work in conjunction with selectable RectItems.
```

### Comparing `pyvispr-2023.9/pyvispr/install.py` & `pyvispr-2024.1/pyvispr/install.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,22 +29,21 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from sys import argv as cmd_line_args
 from sys import exit as Exit
 
 from PyQt6.QtWidgets import QApplication
-
 from pyvispr.interface.window.installer import installer_wdw_t
 
 
 def Main() -> None:
     """"""
     app = QApplication(cmd_line_args)
-    window = installer_wdw_t()
+    window = installer_wdw_t.New()
     window.show()
     Exit(app.exec())
 
 
 if __name__ == "__main__":
     #
     Main()
```

### Comparing `pyvispr-2023.9/pyvispr/interface/storage/loading.py` & `pyvispr-2024.1/pyvispr/interface/storage/loading.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,40 +26,39 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from os.path import dirname as ExtractPathPart
-from pathlib import Path as path_t
 
 import PyQt6.QtWidgets as wdgt
 from json_any.task.storage import LoadFromJSON
+from pyvispr.constant.path import HOME_FOLDER
 
 # from pyvispr.interface.window.main import runner_wdw_t
 
-home_folder = path_t.home()
-last_load_location = home_folder
+_last_load_location = HOME_FOLDER
 
 
 def LoadWorkflow(manager, /) -> None:
     """"""
-    global last_load_location
+    global _last_load_location
 
     filename = wdgt.QFileDialog.getOpenFileName(
         manager,
         "Load Workflow",
-        str(last_load_location),
+        str(_last_load_location),
         "pyVispr Workflows (*.json.*)",
     )
     if (filename is None) or (len(filename[0]) == 0):
         return
     filename = filename[0]
 
-    last_load_location = ExtractPathPart(filename)
+    _last_load_location = ExtractPathPart(filename)
 
     if manager.whiteboard.graph.nodes.__len__() > 0:
         loading_mode = wdgt.QMessageBox(manager)
         loading_mode.setWindowTitle("Loading Options")
         loading_mode.setText(
             "About to load a workflow while the current workflow is not empty\n"
             "Loading options:"
```

### Comparing `pyvispr-2023.9/pyvispr/interface/storage/stowing.py` & `pyvispr-2024.1/pyvispr/interface/storage/stowing.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,20 +31,19 @@
 
 # from pyvispr.interface.window.main import runner_wdw_t
 from os.path import dirname as ExtractPathPart
 from pathlib import Path as path_t
 
 import PyQt6.QtWidgets as wdgt
 from json_any.task.storage import StoreAsJSON
-
+from pyvispr.constant.path import HOME_FOLDER
 from pyvispr.flow.visual.graph import graph_t
 
-home_folder = path_t.home()
-last_save_location = home_folder
-last_save_as_script_location = home_folder
+last_save_location = HOME_FOLDER
+last_save_as_script_location = HOME_FOLDER
 
 
 def SaveWorkflow(manager, /) -> None:
     """"""
     global last_save_location
 
     filename = wdgt.QFileDialog.getSaveFileName(
```

### Comparing `pyvispr-2023.9/pyvispr/interface/window/installer.py` & `pyvispr-2024.1/pyvispr/interface/window/widget/list.py`

 * *Files 27% similar despite different names*

```diff
@@ -27,76 +27,88 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 
-import PyQt6.QtCore as qtcr
 import PyQt6.QtWidgets as wdgt
-
-from pyvispr.config.appearance.color import color_e
-from pyvispr.config.main import TITLE
+from PyQt6.QtCore import Qt as constant_e
+from pyvispr.constant.widget.list import COL_SIZE_PADDING
 from pyvispr.interface.window.messenger import CreateMessageCanal
-from pyvispr.interface.window.widget.function_list import function_list_wgt_t
-from pyvispr.interface.window.widget.module_list import module_list_wgt_t
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
-class installer_wdw_t(wdgt.QMainWindow):
-    def __post_init__(self) -> None:
+class list_wgt_t(wdgt.QListWidget):
+    filter_wgt: wdgt.QLineEdit = dtcl.field(init=False)
+    element_name: dtcl.InitVar[str] = ""
+
+    def __post_init__(self, element_name: str) -> None:
+        """"""
+        wdgt.QListWidget.__init__(self)
+        self.setSelectionMode(wdgt.QAbstractItemView.SelectionMode.NoSelection)
+
+        self.filter_wgt = wdgt.QLineEdit()
+        self.filter_wgt.setPlaceholderText(f"Filter {element_name}")
+        self.filter_wgt.setClearButtonEnabled(True)
+        CreateMessageCanal(self.filter_wgt, "textEdited", self.Filter)
+
+        self.Reload()
+
+    def AddDisabledItem(self, text: str, /) -> None:
+        """"""
+        self.addItem(text)
+        _DisableItem(self.item(self.count() - 1))
+
+    def Reload(self) -> None:
+        """"""
+        self.clear()
+        self.ActualReload()
+        self.sortItems()
+
+        width = self.sizeHintForColumn(0) + COL_SIZE_PADDING
+        self.setFixedWidth(width)
+        self.filter_wgt.setFixedWidth(width)
+
+    def ActualReload(self) -> None:
         """"""
-        wdgt.QMainWindow.__init__(self)
-        self.setWindowTitle(f"{TITLE} - Node Installer")
+        raise NotImplementedError
+
+    def Filter(self, new_filter: str, /) -> None:
+        """"""
+        if new_filter.__len__() > 0:
+            matched_items = self.findItems(
+                new_filter, constant_e.MatchFlag.MatchContains
+            )
+
+            for item_idx in range(self.count()):
+                node_item = self.item(item_idx)
+
+                if node_item not in matched_items:
+                    node_item.setHidden(True)
+                else:
+                    node_item.setHidden(False)
+        else:
+            for item_idx in range(self.count()):
+                self.item(item_idx).setHidden(False)
+
+    def SelectedItemsOrAll(self) -> tuple[wdgt.QListWidgetItem, ...]:
+        """"""
+        output = self.selectedItems()
+
+        if output.__len__() == 0:
+            output = (self.item(_row) for _row in range(self.count()))
+            output = filter(ItemIsEnabled, output)
+
+        return tuple(output)
+
+
+def _DisableItem(item: wdgt.QListWidgetItem, /) -> None:
+    """"""
+    item.setFlags(item.flags() & ~constant_e.ItemFlag.ItemIsEnabled)
+
 
-        single = wdgt.QWidget()
-        select = wdgt.QPushButton("Select Python File")
-        drop = wdgt.QLabel("Drop Python File")
-        drop.setAlignment(qtcr.Qt.AlignmentFlag.AlignCenter)
-        drop.setStyleSheet(f"background-color: {color_e.lightgray.name()};")
-        layout = wdgt.QHBoxLayout()
-        layout.addWidget(select)
-        layout.addWidget(drop)
-        single.setLayout(layout)
-
-        multiple = wdgt.QWidget()
-        select = wdgt.QPushButton("Select Base Folder")
-        drop = wdgt.QLabel("Drop Base Folder")
-        drop.setAlignment(qtcr.Qt.AlignmentFlag.AlignCenter)
-        drop.setStyleSheet(f"background-color: {color_e.lightgray.name()};")
-        layout = wdgt.QHBoxLayout()
-        layout.addWidget(select)
-        layout.addWidget(drop)
-        multiple.setLayout(layout)
-
-        system = wdgt.QWidget()
-        module_list = module_list_wgt_t(element_name="Modules")
-        function_list = function_list_wgt_t(element_name="Functions")
-        layout = wdgt.QGridLayout()
-        layout.addWidget(module_list, 1, 1, alignment=qtcr.Qt.AlignmentFlag.AlignLeft)
-        layout.addWidget(
-            module_list.filter_wgt, 2, 1, alignment=qtcr.Qt.AlignmentFlag.AlignLeft
-        )
-        layout.addWidget(function_list, 1, 2, alignment=qtcr.Qt.AlignmentFlag.AlignLeft)
-        layout.addWidget(
-            function_list.filter_wgt, 2, 2, alignment=qtcr.Qt.AlignmentFlag.AlignLeft
-        )
-        system.setLayout(layout)
-
-        tabs = wdgt.QTabWidget(self)
-        for widget, name in (
-            (single, "Single"),
-            (multiple, "Batch (User)"),
-            (system, "Batch (System)"),
-        ):
-            tabs.addTab(widget, name)
-
-        done = wdgt.QPushButton("Done")
-        CreateMessageCanal(done, "clicked", self.close)
-
-        layout = wdgt.QVBoxLayout()
-        layout.addWidget(tabs)
-        layout.addWidget(done)
-
-        central = wdgt.QWidget(self)
-        central.setLayout(layout)
-        self.setCentralWidget(central)
+def ItemIsEnabled(item: wdgt.QListWidgetItem, /) -> bool:
+    """"""
+    return (
+        item.flags() & constant_e.ItemFlag.ItemIsEnabled
+    ) == constant_e.ItemFlag.ItemIsEnabled
```

### Comparing `pyvispr-2023.9/pyvispr/interface/window/messenger.py` & `pyvispr-2024.1/pyvispr/interface/window/messenger.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2023.9/pyvispr/interface/window/runner.py` & `pyvispr-2024.1/pyvispr/interface/window/runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,57 +25,74 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
+from __future__ import annotations
+
 import dataclasses as dtcl
 from typing import cast
 
 import PyQt6.QtWidgets as wdgt
-
+from logger_36 import AddGenericHandler
 from pyvispr import __version__
-from pyvispr.config.main import TITLE
+from pyvispr.constant.app import APP_NAME
 from pyvispr.flow.visual.whiteboard import whiteboard_t
 from pyvispr.interface.storage.loading import LoadWorkflow
 from pyvispr.interface.storage.stowing import SaveWorkflow, SaveWorkflowAsScript
 from pyvispr.interface.window.messenger import CreateMessageCanal
+from pyvispr.interface.window.widget.list_node import node_list_wgt_t
 from pyvispr.interface.window.widget.menu import AddEntryToMenu
-from pyvispr.interface.window.widget.node_list import node_list_wgt_t
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
 class runner_wdw_t(wdgt.QMainWindow):
-    node_list_wgt: node_list_wgt_t = dtcl.field(init=False)
-    whiteboard: whiteboard_t = dtcl.field(init=False)
+    node_list: node_list_wgt_t
+    whiteboard: whiteboard_t
     status_bar: wdgt.QStatusBar = dtcl.field(init=False)
     _ref_keeper: list = dtcl.field(init=False, default_factory=list)
 
     def __post_init__(self) -> None:
         """"""
         wdgt.QMainWindow.__init__(self)
-        self.setWindowTitle(TITLE)
-
-        self.node_list_wgt = node_list_wgt_t(element_name="Nodes")
-        self.whiteboard = whiteboard_t()
+        self.setWindowTitle(APP_NAME)
 
-        CreateMessageCanal(self.node_list_wgt, "itemClicked", self.AddNode)
+        log_area = wdgt.QTextEdit()
+        log_area.setReadOnly(True)
+        log_area.setLineWrapMode(wdgt.QTextEdit.LineWrapMode.NoWrap)
+        AddGenericHandler(log_area.append, supports_html=True)
+
+        tabs = wdgt.QTabWidget()
+        tabs.addTab(self.whiteboard, "Workflow")
+        tabs.addTab(log_area, "Messages")
+        tabs.setStyleSheet("QTabWidget::tab-bar {alignment: center;}")
 
         layout = wdgt.QGridLayout()
-        layout.addWidget(self.node_list_wgt, 1, 1)
-        layout.addWidget(self.node_list_wgt.filter_wgt, 2, 1)
-        layout.addWidget(self.whiteboard, 1, 2, 2, 1)
+        layout.addWidget(self.node_list, 1, 1)
+        layout.addWidget(self.node_list.filter_wgt, 2, 1)
+        layout.addWidget(tabs, 1, 2, 2, 1)
 
-        central = wdgt.QWidget(self)
+        central = wdgt.QWidget()
         central.setLayout(layout)
         self.setCentralWidget(central)
 
-        self.status_bar = self.statusBar()
         self._AddMenuBar()
+        self.status_bar = self.statusBar()
+
+        CreateMessageCanal(self.node_list, "itemClicked", self.AddNode)
+
+    @classmethod
+    def New(cls) -> runner_wdw_t:
+        """"""
+        node_list = node_list_wgt_t(element_name="Nodes")
+        whiteboard = whiteboard_t()
+
+        return cls(node_list=node_list, whiteboard=whiteboard)
 
     def _AddMenuBar(self) -> None:
         """"""
         menu_bar = self.menuBar()
 
         _ = _AddMenu(
             "py&Vispr",
@@ -139,15 +156,15 @@
             ),
             menu_bar,
             self,
         )
 
         _ = _AddMenu(
             "&Catalog",
-            (("Refresh", lambda *_, **__: self.node_list_wgt.Reload()),),
+            (("Refresh", lambda *_, **__: self.node_list.Reload()),),
             menu_bar,
             self,
         )
 
     def AddNode(self, item: wdgt.QListWidgetItem, /) -> None:
         """
         Calling directly on self.whiteboard.graph from the menu will not work if the graph changes.
```

### Comparing `pyvispr-2023.9/pyvispr/interface/window/widget/function_list.py` & `pyvispr-2024.1/pyvispr/interface/window/widget/list_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 
 from logger_36.task.inspection import Modules
-
 from pyvispr.interface.window.widget.list import list_wgt_t
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
-class function_list_wgt_t(list_wgt_t):
+class module_list_wgt_t(list_wgt_t):
     def ActualReload(self) -> None:
         """"""
-        pass
+        for module in Modules(False, False, only_loaded=False):
+            self.addItem(module)
```

### Comparing `pyvispr-2023.9/pyvispr/interface/window/widget/list.py` & `pyvispr-2024.1/pyvispr/interface/window/widget/list_file.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,66 +26,37 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
+from pathlib import Path as path_t
 
-import PyQt6.QtWidgets as wdgt
-from PyQt6.QtCore import Qt as constant_e
-
-from pyvispr.interface.window.messenger import CreateMessageCanal
-
-COL_SIZE_PADDING = 20
+from pyvispr.interface.window.widget.list import list_wgt_t
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
-class list_wgt_t(wdgt.QListWidget):
-    filter_wgt: wdgt.QLineEdit = dtcl.field(init=False)
-    element_name: dtcl.InitVar[str] = ""
-
-    def __post_init__(self, element_name: str, /) -> None:
-        """"""
-        wdgt.QListWidget.__init__(self)
-        self.setSelectionMode(wdgt.QAbstractItemView.SelectionMode.NoSelection)
-
-        self.filter_wgt = wdgt.QLineEdit()
-        self.filter_wgt.setSizePolicy(
-            wdgt.QSizePolicy.Policy.Minimum,
-            wdgt.QSizePolicy.Policy.Fixed,
-        )
-        self.filter_wgt.setPlaceholderText(" ".join(("Filter", element_name)))
-        self.filter_wgt.setClearButtonEnabled(True)
-        CreateMessageCanal(self.filter_wgt, "textEdited", self.Filter)
-
-        self.Reload()
-
-    def Reload(self) -> None:
-        """"""
-        self.clear()
-        self.ActualReload()
-        self.sortItems()
-
-        self.setFixedWidth(self.sizeHintForColumn(0) + COL_SIZE_PADDING)
+class file_list_wgt_t(list_wgt_t):
+    base_folder: path_t | None = None
+    recursive_mode: bool = False
+    files: dict[str, path_t] = dtcl.field(init=False, default_factory=dict)
 
     def ActualReload(self) -> None:
         """"""
-        raise NotImplementedError
+        if self.base_folder is None:
+            self.AddDisabledItem("No Python Files")
+            return
 
-    def Filter(self, new_filter: str, /) -> None:
-        """"""
-        if new_filter.__len__() > 0:
-            matched_items = self.findItems(
-                new_filter, constant_e.MatchFlag.MatchContains
-            )
-
-            for item_idx in range(self.count()):
-                node_item = self.item(item_idx)
-
-                if node_item not in matched_items:
-                    node_item.setHidden(True)
-                else:
-                    node_item.setHidden(False)
+        if self.recursive_mode:
+            FileIterator = self.base_folder.rglob
         else:
-            for item_idx in range(self.count()):
-                self.item(item_idx).setHidden(False)
+            FileIterator = self.base_folder.glob
+        files = tuple(_elm for _elm in FileIterator("*.py") if _elm.is_file())
+        if files.__len__() == 0:
+            self.AddDisabledItem("No Python Files Found")
+            return
+
+        for file_ in files:
+            stem = file_.stem
+            self.addItem(stem)
+            self.files[stem] = file_
```

### Comparing `pyvispr-2023.9/pyvispr/interface/window/widget/menu.py` & `pyvispr-2024.1/pyvispr/interface/window/widget/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from typing import Callable
 
 import PyQt6.QtWidgets as wdgt
 from PyQt6.QtGui import QAction
-
 from pyvispr.interface.window.messenger import CreateMessageCanal
 
 
 def AddEntryToMenu(
     menu: wdgt.QMenu,
     parent: wdgt.QWidget,
     text: str,
```

### Comparing `pyvispr-2023.9/pyvispr/interface/window/widget/module_list.py` & `pyvispr-2024.1/pyvispr/constant/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,20 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import dataclasses as dtcl
-
-from logger_36.task.inspection import Modules
-
-from pyvispr.interface.window.widget.list import list_wgt_t
-
-
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class module_list_wgt_t(list_wgt_t):
-    def ActualReload(self) -> None:
-        """"""
-        for module in Modules(False, False, only_loaded=False):
-            self.addItem(module)
+APP_NAME = "pyVispr"
```

### Comparing `pyvispr-2023.9/pyvispr/interface/window/widget/node_list.py` & `pyvispr-2024.1/pyvispr/interface/window/widget/list_node.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,32 +28,32 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 from re import search as SearchRegEx
 
-import PyQt6.QtGui as gui
 from PyQt6.QtCore import Qt as constant_e
-
-from pyvispr.catalog.main import NODE_CATALOG
-from pyvispr.config.appearance.color import color_e
+from pyvispr.config.appearance.color import ORANGE_BRUSH
+from pyvispr.flow.descriptive.node import node_t
 from pyvispr.interface.window.widget.list import list_wgt_t
-
-ORANGE_BRUSH = gui.QBrush(color_e.orange)
+from pyvispr.runtime.catalog import NODE_CATALOG
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
 class node_list_wgt_t(list_wgt_t):
+    nodes: dict[str, node_t] = dtcl.field(init=False, default_factory=dict)
+
     def ActualReload(self) -> None:
         """"""
         for node in NODE_CATALOG:
             self.addItem(node.name)
             if node.requires_completion:
                 self.item(self.count() - 1).setForeground(ORANGE_BRUSH)
+            self.nodes[node.name] = node
 
     def Filter(self, new_filter: str, /) -> None:
         """"""
         if new_filter.__len__() > 0:
             matched_items = self.findItems(
                 new_filter, constant_e.MatchFlag.MatchContains
             )
```

### Comparing `pyvispr-2023.9/pyvispr/run.py` & `pyvispr-2024.1/pyvispr/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,22 +29,21 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from sys import argv as cmd_line_args
 from sys import exit as Exit
 
 from PyQt6.QtWidgets import QApplication
-
 from pyvispr.interface.window.runner import runner_wdw_t
 
 
 def Main() -> None:
     """"""
     app = QApplication(cmd_line_args)
-    window = runner_wdw_t()
+    window = runner_wdw_t.New()
     window.show()
     Exit(app.exec())
 
 
 if __name__ == "__main__":
     #
     Main()
```

### Comparing `pyvispr-2023.9/pyvispr/version.py` & `pyvispr-2024.1/pyvispr/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.9"
+__version__ = "2024.1"
```

### Comparing `pyvispr-2023.9/pyvispr.egg-info/PKG-INFO` & `pyvispr-2024.1/pyvispr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvispr
-Version: 2023.9
+Version: 2024.1
 Summary: Visual Programming App for Python
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyVispr//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
@@ -12,19 +12,27 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
-Requires-Dist: PyQt6
+Requires-Dist: babelwidget
+Requires-Dist: conf_ini_g
+Requires-Dist: json_any
+Requires-Dist: logger_36
+Requires-Dist: numexpr
+Requires-Dist: numpy
 Requires-Dist: platformdirs
+Requires-Dist: PyQt6
+Requires-Dist: scikit-image
+Requires-Dist: str_to_obj
 
 ..
-   Copyright CNRS/Inria/UCA
+   Copyright CNRS/Inria/UniCA
    Contributor(s): Eric Debreuve (since 2017)
 
    eric.debreuve@cnrs.fr
 
    This software is governed by the CeCILL  license under French law and
    abiding by the rules of distribution of free software.  You can  use,
    modify and/ or redistribute the software under the terms of the CeCILL
```

