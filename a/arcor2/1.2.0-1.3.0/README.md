# Comparing `tmp/arcor2-1.2.0.tar.gz` & `tmp/arcor2-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2-1.2.0.tar", last modified: Fri Jan 26 07:55:06 2024, max compression
+gzip compressed data, was "arcor2-1.3.0.tar", last modified: Thu Apr 11 09:47:28 2024, max compression
```

## Comparing `arcor2-1.2.0.tar` & `arcor2-1.3.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.611744 arcor2-1.2.0/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-01-26 07:55:06.000000 arcor2-1.2.0/MANIFEST.in
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)    19277 2024-01-26 07:55:06.611744 arcor2-1.2.0/PKG-INFO
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.607744 arcor2-1.2.0/arcor2/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        5 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/VERSION
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      732 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    25186 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/cached.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.611744 arcor2-1.2.0/arcor2/clients/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/clients/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      508 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/clients/aio_asset.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2743 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/clients/aio_project_service.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1409 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/clients/aio_scene_service.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2039 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/clients/asset.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     8731 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/clients/project_service.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5495 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/clients/scene_service.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.611744 arcor2-1.2.0/arcor2/data/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2304 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/data/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      752 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/data/camera.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    21507 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/data/common.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4026 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/data/events.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      267 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/data/execution.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4043 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/data/object_type.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      194 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/data/robot.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.611744 arcor2-1.2.0/arcor2/data/rpc/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      212 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/data/rpc/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2019 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/data/rpc/common.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      690 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/data/scene.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3469 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/docstring.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      969 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/env.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.611744 arcor2-1.2.0/arcor2/exceptions/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      152 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/exceptions/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      910 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/exceptions/helpers.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     7081 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/flask.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6720 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/helpers.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1176 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/image.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      814 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/json.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1223 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/logging.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1472 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/logic.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.611744 arcor2-1.2.0/arcor2/object_types/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/object_types/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    14792 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/object_types/abstract.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      716 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/object_types/flow_actions.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1037 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/object_types/logic_actions.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1492 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/object_types/random_actions.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1391 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/object_types/time_actions.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4355 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/object_types/upload.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6810 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/object_types/utils.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.611744 arcor2-1.2.0/arcor2/parameter_plugins/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      193 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3752 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/base.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1702 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/boolean.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2220 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/double.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1305 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/image.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3875 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/integer.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3810 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/integer_enum.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2393 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/joints.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1299 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/list.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4531 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/pose.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2184 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/position.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1481 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/string.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      320 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/string_enum.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3163 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/parameter_plugins/utils.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/py.typed
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    11124 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/rest.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.611744 arcor2-1.2.0/arcor2/scripts/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/scripts/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      485 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/scripts/upload_builtin_objects.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.611744 arcor2-1.2.0/arcor2/source/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      171 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/source/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5482 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/source/utils.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.611744 arcor2-1.2.0/arcor2/test_objects/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      165 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/test_objects/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      624 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/test_objects/box.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       64 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/test_objects/box2.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6599 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/test_objects/dummy_multiarm_robot.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      620 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/test_objects/param_to_return.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      449 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/test_objects/position_param.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1982 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/test_objects/tester.py
--rwxr-xr-x   0 zdenekm   (1000) zdenekm   (1000)      770 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/test_objects/upload.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     7129 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/transformations.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1879 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/urdf.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6181 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2/ws_server.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-26 07:55:06.611744 arcor2-1.2.0/arcor2.egg-info/
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)    19277 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2.egg-info/PKG-INFO
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     2203 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       93 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2.egg-info/entry_points.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      513 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2.egg-info/requires.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        7 2024-01-26 07:55:06.000000 arcor2-1.2.0/arcor2.egg-info/top_level.txt
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      822 2024-01-26 07:55:06.000000 arcor2-1.2.0/backend_shim.py
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-01-26 07:55:06.611744 arcor2-1.2.0/setup.cfg
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    20919 2024-01-26 07:55:06.000000 arcor2-1.2.0/setup.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.673376 arcor2-1.3.0/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-04-11 09:47:26.000000 arcor2-1.3.0/MANIFEST.in
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)    19365 2024-04-11 09:47:28.673376 arcor2-1.3.0/PKG-INFO
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.645378 arcor2-1.3.0/arcor2/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        5 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/VERSION
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      704 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    25186 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/cached.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.653377 arcor2-1.3.0/arcor2/clients/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/clients/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      508 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/clients/aio_asset.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2743 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/clients/aio_project_service.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1409 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/clients/aio_scene_service.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2039 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/clients/asset.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     8731 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/clients/project_service.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5495 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/clients/scene_service.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.657377 arcor2-1.3.0/arcor2/data/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1589 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/data/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      752 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/data/camera.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    21571 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/data/common.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4026 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/data/events.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      267 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/data/execution.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4043 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/data/object_type.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      194 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/data/robot.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.657377 arcor2-1.3.0/arcor2/data/rpc/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      212 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/data/rpc/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2019 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/data/rpc/common.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      690 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/data/scene.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3469 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/docstring.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      969 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/env.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.657377 arcor2-1.3.0/arcor2/exceptions/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      152 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/exceptions/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      910 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/exceptions/helpers.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     7081 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/flask.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6720 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/helpers.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1176 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/image.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      814 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/json.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1223 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/logging.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1472 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/logic.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.661377 arcor2-1.3.0/arcor2/object_types/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/object_types/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    14792 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/object_types/abstract.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      716 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/object_types/flow_actions.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1037 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/object_types/logic_actions.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1492 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/object_types/random_actions.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1391 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/object_types/time_actions.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4355 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/object_types/upload.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6826 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/object_types/utils.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.669377 arcor2-1.3.0/arcor2/parameter_plugins/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      193 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3752 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/base.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1702 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/boolean.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2220 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/double.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1305 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/image.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3875 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/integer.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3810 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/integer_enum.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2393 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/joints.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1299 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/list.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4531 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/pose.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2184 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/position.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1481 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/string.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      320 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/string_enum.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3163 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/parameter_plugins/utils.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/py.typed
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    11124 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/rest.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.669377 arcor2-1.3.0/arcor2/scripts/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/scripts/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      485 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/scripts/upload_builtin_objects.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.669377 arcor2-1.3.0/arcor2/source/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      171 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/source/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5482 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/source/utils.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.673376 arcor2-1.3.0/arcor2/test_objects/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      165 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/test_objects/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      624 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/test_objects/box.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       64 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/test_objects/box2.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6599 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/test_objects/dummy_multiarm_robot.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      620 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/test_objects/param_to_return.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      449 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/test_objects/position_param.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1982 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/test_objects/tester.py
+-rwxr-xr-x   0 zdenekm   (1000) zdenekm   (1000)      770 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/test_objects/upload.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     7129 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/transformations.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2022 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/urdf.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6181 2024-04-11 09:47:27.000000 arcor2-1.3.0/arcor2/ws_server.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.649377 arcor2-1.3.0/arcor2.egg-info/
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)    19365 2024-04-11 09:47:28.000000 arcor2-1.3.0/arcor2.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     2203 2024-04-11 09:47:28.000000 arcor2-1.3.0/arcor2.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-11 09:47:28.000000 arcor2-1.3.0/arcor2.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       93 2024-04-11 09:47:28.000000 arcor2-1.3.0/arcor2.egg-info/entry_points.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-11 09:47:28.000000 arcor2-1.3.0/arcor2.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      600 2024-04-11 09:47:28.000000 arcor2-1.3.0/arcor2.egg-info/requires.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        7 2024-04-11 09:47:28.000000 arcor2-1.3.0/arcor2.egg-info/top_level.txt
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      835 2024-04-11 09:47:26.000000 arcor2-1.3.0/backend_shim.py
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-04-11 09:47:28.673376 arcor2-1.3.0/setup.cfg
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    21127 2024-04-11 09:47:26.000000 arcor2-1.3.0/setup.py
```

### Comparing `arcor2-1.2.0/PKG-INFO` & `arcor2-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: arcor2
-Version: 1.2.0
+Version: 1.3.0
 Summary: ARCOR2 base library
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: ==3.10.*
+Requires-Python: ==3.11.*
 Description-Content-Type: text/markdown
 
 # arcor2
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.3.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
 ## [1.2.0] - 2024-01-26
 
 ### Added
 
 - `save_type_def` helper function.
 
 ## [1.1.0] - 2023-07-20
```

### Comparing `arcor2-1.2.0/arcor2/__init__.py` & `arcor2-1.3.0/arcor2/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pkgutil
+import importlib.resources
 import warnings
 from typing import NamedTuple
 
 
 class DynamicParamTuple(NamedTuple):
     method_name: str
     parent_parameters: set[str]
@@ -16,14 +16,12 @@
 
 
 if __debug__:
     warnings.filterwarnings("error", module="dataclasses_jsonschema")  # make warnings fatal because they are
 
 
 def package_version(package: str, file: str = "VERSION") -> str:
-    if res := pkgutil.get_data(package, file):
-        return res.decode().strip()
-    return "unknown"
+    return importlib.resources.read_text(package, file).strip()
 
 
 def version() -> str:
     return package_version(__name__)
```

### Comparing `arcor2-1.2.0/arcor2/cached.py` & `arcor2-1.3.0/arcor2/cached.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/clients/aio_project_service.py` & `arcor2-1.3.0/arcor2/clients/aio_project_service.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/clients/aio_scene_service.py` & `arcor2-1.3.0/arcor2/clients/aio_scene_service.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/clients/asset.py` & `arcor2-1.3.0/arcor2/clients/asset.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/clients/project_service.py` & `arcor2-1.3.0/arcor2/clients/project_service.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/clients/scene_service.py` & `arcor2-1.3.0/arcor2/clients/scene_service.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/data/__init__.py` & `arcor2-1.3.0/arcor2/data/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import importlib
-import inspect
-import pkgutil
 from typing import TYPE_CHECKING
 
 import dataclasses_jsonschema
 import orjson
-from dataclasses_jsonschema import JsonSchemaMixin, ValidationError
+from dataclasses_jsonschema import JsonSchemaMixin
 from dataclasses_jsonschema.apispec import DataclassesPlugin, _schema_reference
 
 from arcor2.exceptions import Arcor2Exception
 
 
 class DataException(Arcor2Exception):
     pass
@@ -41,28 +38,7 @@
         for key in data:
             if isinstance(data[key], dict):
                 self.resolve_schema_refs(data[key])
 
 
 # monkey patch to solve https://github.com/s-knibbs/dataclasses-jsonschema/issues/126
 DataclassesPlugin.resolve_schema_refs = resolve_schema_refs  # type: ignore
-
-
-def compile_json_schemas() -> None:
-    """
-    Force compilation of json schema (otherwise it might cause troubles later when executed in parallel)
-    :return:
-    """
-
-    from arcor2 import data
-
-    for _, module_name, _ in pkgutil.iter_modules(data.__path__):
-        module = importlib.import_module(f"{data.__name__}.{module_name}")
-
-        for _, obj in inspect.getmembers(module, inspect.isclass):
-            if not issubclass(obj, JsonSchemaMixin) or obj is JsonSchemaMixin or inspect.isabstract(obj):
-                continue
-
-            try:
-                obj.from_dict({})
-            except ValidationError:
-                pass
```

### Comparing `arcor2-1.2.0/arcor2/data/camera.py` & `arcor2-1.3.0/arcor2/data/camera.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/data/common.py` & `arcor2-1.3.0/arcor2/data/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import abc
 import copy
 from dataclasses import dataclass, field
 from datetime import datetime
-from enum import Enum, unique
+from enum import Enum
+from enum import StrEnum as BuiltinStrEnum
+from enum import unique
 from json import JSONEncoder
 from typing import Any, Iterator, NamedTuple, Optional, TypeVar, cast
 
 import fastuuid as uuid
 import numpy as np
 import quaternion
 from dataclasses_jsonschema import DEFAULT_SCHEMA_TYPE, JsonSchemaMixin
@@ -22,15 +24,15 @@
     if not (prefix and prefix[0].isalpha() and prefix[-1] != "_"):
         raise Arcor2Exception(f"{prefix} is a invalid uid prefix.")
 
     return f"{prefix}_{uuid.uuid4().hex}"
 
 
 @unique
-class StrEnum(str, Enum):
+class StrEnum(BuiltinStrEnum):
     @classmethod
     def set(cls) -> set[str]:
         return set(map(lambda c: c.value, cls))  # type: ignore
 
 
 @unique
 class IntEnum(int, Enum):
```

### Comparing `arcor2-1.2.0/arcor2/data/events.py` & `arcor2-1.3.0/arcor2/data/events.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/data/object_type.py` & `arcor2-1.3.0/arcor2/data/object_type.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/data/rpc/common.py` & `arcor2-1.3.0/arcor2/data/rpc/common.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/data/scene.py` & `arcor2-1.3.0/arcor2/data/scene.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/docstring.py` & `arcor2-1.3.0/arcor2/docstring.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/env.py` & `arcor2-1.3.0/arcor2/env.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/exceptions/helpers.py` & `arcor2-1.3.0/arcor2/exceptions/helpers.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/flask.py` & `arcor2-1.3.0/arcor2/flask.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/helpers.py` & `arcor2-1.3.0/arcor2/helpers.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/image.py` & `arcor2-1.3.0/arcor2/image.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/json.py` & `arcor2-1.3.0/arcor2/json.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/logging.py` & `arcor2-1.3.0/arcor2/logging.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/logic.py` & `arcor2-1.3.0/arcor2/logic.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/object_types/abstract.py` & `arcor2-1.3.0/arcor2/object_types/abstract.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/object_types/flow_actions.py` & `arcor2-1.3.0/arcor2/object_types/flow_actions.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/object_types/logic_actions.py` & `arcor2-1.3.0/arcor2/object_types/logic_actions.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/object_types/random_actions.py` & `arcor2-1.3.0/arcor2/object_types/random_actions.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/object_types/time_actions.py` & `arcor2-1.3.0/arcor2/object_types/time_actions.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/object_types/upload.py` & `arcor2-1.3.0/arcor2/object_types/upload.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/object_types/utils.py` & `arcor2-1.3.0/arcor2/object_types/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 
 
 def iterate_over_actions(
     type_def: type[Generic],
 ) -> Iterator[tuple[str, Callable[[Any,], Any]]]:
     for method_name, method in inspect.getmembers(type_def, inspect.isroutine):
         try:
-            if not isinstance(method.__action__, ActionMetadata):
+            if not isinstance(method.__action__, ActionMetadata):  # type: ignore
                 continue
         except AttributeError:
             continue
 
         yield method_name, method
```

### Comparing `arcor2-1.2.0/arcor2/parameter_plugins/base.py` & `arcor2-1.3.0/arcor2/parameter_plugins/base.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/parameter_plugins/boolean.py` & `arcor2-1.3.0/arcor2/parameter_plugins/boolean.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/parameter_plugins/double.py` & `arcor2-1.3.0/arcor2/parameter_plugins/double.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/parameter_plugins/image.py` & `arcor2-1.3.0/arcor2/parameter_plugins/image.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/parameter_plugins/integer.py` & `arcor2-1.3.0/arcor2/parameter_plugins/integer.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/parameter_plugins/integer_enum.py` & `arcor2-1.3.0/arcor2/parameter_plugins/integer_enum.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/parameter_plugins/joints.py` & `arcor2-1.3.0/arcor2/parameter_plugins/joints.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/parameter_plugins/list.py` & `arcor2-1.3.0/arcor2/parameter_plugins/list.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/parameter_plugins/pose.py` & `arcor2-1.3.0/arcor2/parameter_plugins/pose.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/parameter_plugins/position.py` & `arcor2-1.3.0/arcor2/parameter_plugins/position.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/parameter_plugins/string.py` & `arcor2-1.3.0/arcor2/parameter_plugins/string.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/parameter_plugins/utils.py` & `arcor2-1.3.0/arcor2/parameter_plugins/utils.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/rest.py` & `arcor2-1.3.0/arcor2/rest.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/source/utils.py` & `arcor2-1.3.0/arcor2/source/utils.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/test_objects/box.py` & `arcor2-1.3.0/arcor2/test_objects/box.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/test_objects/dummy_multiarm_robot.py` & `arcor2-1.3.0/arcor2/test_objects/dummy_multiarm_robot.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/test_objects/param_to_return.py` & `arcor2-1.3.0/arcor2/test_objects/param_to_return.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/test_objects/tester.py` & `arcor2-1.3.0/arcor2/test_objects/tester.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/test_objects/upload.py` & `arcor2-1.3.0/arcor2/test_objects/upload.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/transformations.py` & `arcor2-1.3.0/arcor2/transformations.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2/urdf.py` & `arcor2-1.3.0/arcor2/urdf.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import fractions
 import io
 import math
 import os
 import tempfile
 import zipfile
 
+import numpy as np
+
 from arcor2 import rest
 from arcor2.exceptions import Arcor2Exception
 
 # this is a workaround to make urdfpy/networkx happy under Python 3.9/3.10
 # TODO not sure if it really works in runtime, the best would be to solve https://github.com/mmatl/urdfpy/issues/4
 # or to switch to another package as proposed here https://github.com/robofit/arcor2/issues/706
 fractions.gcd = math.gcd  # type: ignore
@@ -17,14 +19,17 @@
 # another workaround related to urdfpy/networkx and Python 3.10
 from collections.abc import Iterable, Mapping, Set  # noqa:E402
 
 collections.Mapping = Mapping  # type: ignore
 collections.Set = Set  # type: ignore
 collections.Iterable = Iterable  # type: ignore
 
+np.int = int  # type: ignore  # TODO workaround for urdfpy
+np.float = float  # type: ignore  # TODO workaround for urdfpy
+
 from urdfpy import URDF  # noqa
 
 
 class Arcor2UrdfException(Arcor2Exception):
     pass
```

### Comparing `arcor2-1.2.0/arcor2/ws_server.py` & `arcor2-1.3.0/arcor2/ws_server.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2.egg-info/PKG-INFO` & `arcor2-1.3.0/arcor2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: arcor2
-Version: 1.2.0
+Version: 1.3.0
 Summary: ARCOR2 base library
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: ==3.10.*
+Requires-Python: ==3.11.*
 Description-Content-Type: text/markdown
 
 # arcor2
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.3.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
 ## [1.2.0] - 2024-01-26
 
 ### Added
 
 - `save_type_def` helper function.
 
 ## [1.1.0] - 2023-07-20
```

### Comparing `arcor2-1.2.0/arcor2.egg-info/SOURCES.txt` & `arcor2-1.3.0/arcor2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcor2-1.2.0/arcor2.egg-info/requires.txt` & `arcor2-1.3.0/arcor2.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-Flask~=2.2.3
-Pillow~=9.4.0
+Flask~=3.0.2
+Pillow~=10.2.0
 aiologger~=0.7.0
-apispec-webframeworks~=0.5.2
-apispec[yaml]~=6.3.0
-autopep8~=2.0.2
-colorlog~=6.7.0
-dataclasses-jsonschema[apispec,fast-dateparsing,fast-uuid,fast-validation]~=2.16.0
+apispec-webframeworks~=1.1.0
+apispec[yaml]~=6.6.0
+autopep8~=2.1.0
+colorlog~=6.8.2
+dataclasses-jsonschema[apispec,fast-dateparsing,fast-validation]~=2.16.0
 fastuuid~=0.8.0
 flask-swagger-ui~=4.11.1
-flask_cors~=3.0.10
-numpy-quaternion[numba,scipy]~=2022.4.3
-numpy~=1.23.5
-opencv-contrib-python~=4.7.0.72
-orjson~=3.8.8
-packaging~=21.3
+flask_cors~=4.0.0
+numpy-quaternion[numba,scipy]~=2023.0.3
+numpy~=1.26.4
+opencv-contrib-python~=4.9.0.80
+orjson~=3.9.15
+packaging~=24.0
 pyhumps==3.8.0
-python-dateutil~=2.8.2
-requests~=2.28.2
-setuptools~=66.0.0
-typing-inspect~=0.8.0
+python-dateutil~=2.9.0.post0
+requests~=2.31.0
+setuptools~=69.2.0
+types-orjson==3.6.2
+types-python-dateutil==2.9.0.20240316
+types-requests==2.31.0.20240311
+typing-inspect~=0.9.0
 urdfpy~=0.0.22
-websockets~=10.4
+websockets~=12.0
```

### Comparing `arcor2-1.2.0/backend_shim.py` & `arcor2-1.3.0/backend_shim.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 
 # DO NOT EDIT THIS FILE -- AUTOGENERATED BY PANTS
 
+import errno
 import os
 import setuptools.build_meta
 
 backend = setuptools.build_meta.__legacy__
 
 dist_dir = "dist/"
 build_wheel = True
 build_sdist = True
 wheel_config_settings = {
     '--global-option': [
         '--python-tag',
-        'py310',
+        'py311',
     ],
 }
 sdist_config_settings = {
 }
 
 # Python 2.7 doesn't have the exist_ok arg on os.makedirs().
 try:
```

### Comparing `arcor2-1.2.0/setup.py` & `arcor2-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,55 +8,64 @@
     'author': 'Robo@FIT',
     'author_email': 'imaterna@fit.vut.cz',
     'classifiers': [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
-        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Natural Language :: English',
         'Topic :: Scientific/Engineering',
     ],
     'description': 'ARCOR2 base library',
     'entry_points': {
         'console_scripts': [
             'arcor2_upload_builtin_objects = arcor2.scripts.upload_builtin_objects:main',
         ],
     },
     'install_requires': (
-        'Flask~=2.2.3',
-        'Pillow~=9.4.0',
+        'Flask~=3.0.2',
+        'Pillow~=10.2.0',
         'aiologger~=0.7.0',
-        'apispec-webframeworks~=0.5.2',
-        'apispec[yaml]~=6.3.0',
-        'autopep8~=2.0.2',
-        'colorlog~=6.7.0',
-        'dataclasses-jsonschema[apispec,fast-dateparsing,fast-uuid,fast-validation]~=2.16.0',
+        'apispec-webframeworks~=1.1.0',
+        'apispec[yaml]~=6.6.0',
+        'autopep8~=2.1.0',
+        'colorlog~=6.8.2',
+        'dataclasses-jsonschema[apispec,fast-dateparsing,fast-validation]~=2.16.0',
         'fastuuid~=0.8.0',
         'flask-swagger-ui~=4.11.1',
-        'flask_cors~=3.0.10',
-        'numpy-quaternion[numba,scipy]~=2022.4.3',
-        'numpy~=1.23.5',
-        'opencv-contrib-python~=4.7.0.72',
-        'orjson~=3.8.8',
-        'packaging~=21.3',
+        'flask_cors~=4.0.0',
+        'numpy-quaternion[numba,scipy]~=2023.0.3',
+        'numpy~=1.26.4',
+        'opencv-contrib-python~=4.9.0.80',
+        'orjson~=3.9.15',
+        'packaging~=24.0',
         'pyhumps==3.8.0',
-        'python-dateutil~=2.8.2',
-        'requests~=2.28.2',
-        'setuptools~=66.0.0',
-        'typing-inspect~=0.8.0',
+        'python-dateutil~=2.9.0.post0',
+        'requests~=2.31.0',
+        'setuptools~=69.2.0',
+        'types-orjson==3.6.2',
+        'types-python-dateutil==2.9.0.20240316',
+        'types-requests==2.31.0.20240311',
+        'typing-inspect~=0.9.0',
         'urdfpy~=0.0.22',
-        'websockets~=10.4',
+        'websockets~=12.0',
     ),
     'license': 'LGPL',
     'long_description': """# arcor2
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.3.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
 ## [1.2.0] - 2024-01-26
 
 ### Added
 
 - `save_type_def` helper function.
 
 ## [1.1.0] - 2023-07-20
@@ -593,10 +602,10 @@
         'arcor2.exceptions',
         'arcor2.object_types',
         'arcor2.parameter_plugins',
         'arcor2.scripts',
         'arcor2.source',
         'arcor2.test_objects',
     ),
-    'python_requires': '==3.10.*',
-    'version': '1.2.0',
+    'python_requires': '==3.11.*',
+    'version': '1.3.0',
 })
```

