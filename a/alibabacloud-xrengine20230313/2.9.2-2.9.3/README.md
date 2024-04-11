# Comparing `tmp/alibabacloud_xrengine20230313-2.9.2.tar.gz` & `tmp/alibabacloud_xrengine20230313-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_xrengine20230313-2.9.2.tar", last modified: Tue Mar 26 08:31:38 2024, max compression
+gzip compressed data, was "dist/alibabacloud_xrengine20230313-2.9.3.tar", last modified: Thu Apr 11 03:03:45 2024, max compression
```

## Comparing `alibabacloud_xrengine20230313-2.9.2.tar` & `alibabacloud_xrengine20230313-2.9.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:31:38.000000 alibabacloud_xrengine20230313-2.9.2/
--rw-r--r--   0 root         (0) root         (0)     1553 2024-03-26 08:31:37.000000 alibabacloud_xrengine20230313-2.9.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-26 08:31:37.000000 alibabacloud_xrengine20230313-2.9.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-26 08:31:37.000000 alibabacloud_xrengine20230313-2.9.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-03-26 08:31:38.000000 alibabacloud_xrengine20230313-2.9.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-03-26 08:31:37.000000 alibabacloud_xrengine20230313-2.9.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-03-26 08:31:37.000000 alibabacloud_xrengine20230313-2.9.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:31:38.000000 alibabacloud_xrengine20230313-2.9.2/alibabacloud_xrengine20230313/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-26 08:31:37.000000 alibabacloud_xrengine20230313-2.9.2/alibabacloud_xrengine20230313/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211149 2024-03-26 08:31:37.000000 alibabacloud_xrengine20230313-2.9.2/alibabacloud_xrengine20230313/client.py
--rw-r--r--   0 root         (0) root         (0)   673183 2024-03-26 08:31:37.000000 alibabacloud_xrengine20230313-2.9.2/alibabacloud_xrengine20230313/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:31:38.000000 alibabacloud_xrengine20230313-2.9.2/alibabacloud_xrengine20230313.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-03-26 08:31:38.000000 alibabacloud_xrengine20230313-2.9.2/alibabacloud_xrengine20230313.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-03-26 08:31:38.000000 alibabacloud_xrengine20230313-2.9.2/alibabacloud_xrengine20230313.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 08:31:38.000000 alibabacloud_xrengine20230313-2.9.2/alibabacloud_xrengine20230313.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-26 08:31:38.000000 alibabacloud_xrengine20230313-2.9.2/alibabacloud_xrengine20230313.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-03-26 08:31:38.000000 alibabacloud_xrengine20230313-2.9.2/alibabacloud_xrengine20230313.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-26 08:31:38.000000 alibabacloud_xrengine20230313-2.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2024-03-26 08:31:37.000000 alibabacloud_xrengine20230313-2.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/
+-rw-r--r--   0 root         (0) root         (0)     1773 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/alibabacloud_xrengine20230313/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/alibabacloud_xrengine20230313/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   211409 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/alibabacloud_xrengine20230313/client.py
+-rw-r--r--   0 root         (0) root         (0)   673777 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/alibabacloud_xrengine20230313/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/alibabacloud_xrengine20230313.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/alibabacloud_xrengine20230313.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/alibabacloud_xrengine20230313.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/alibabacloud_xrengine20230313.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/alibabacloud_xrengine20230313.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/alibabacloud_xrengine20230313.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-11 03:03:45.000000 alibabacloud_xrengine20230313-2.9.3/setup.py
```

### Comparing `alibabacloud_xrengine20230313-2.9.2/LICENSE` & `alibabacloud_xrengine20230313-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-2.9.2/PKG-INFO` & `alibabacloud_xrengine20230313-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_xrengine20230313
-Version: 2.9.2
+Version: 2.9.3
 Summary: Alibaba Cloud xrEngine (20230313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_xrengine20230313-2.9.2/README-CN.md` & `alibabacloud_xrengine20230313-2.9.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-2.9.2/README.md` & `alibabacloud_xrengine20230313-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-2.9.2/alibabacloud_xrengine20230313/client.py` & `alibabacloud_xrengine20230313-2.9.3/alibabacloud_xrengine20230313/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5014,14 +5014,16 @@
     ) -> xr_engine_20230313_models.SubmitMotionShopTaskResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.avatar_id):
             body['AvatarId'] = request.avatar_id
         if not UtilClient.is_unset(request.jwt_token):
             body['JwtToken'] = request.jwt_token
+        if not UtilClient.is_unset(request.selected_box_index):
+            body['SelectedBoxIndex'] = request.selected_box_index
         if not UtilClient.is_unset(request.title):
             body['Title'] = request.title
         if not UtilClient.is_unset(request.video_id):
             body['VideoId'] = request.video_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -5048,14 +5050,16 @@
     ) -> xr_engine_20230313_models.SubmitMotionShopTaskResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.avatar_id):
             body['AvatarId'] = request.avatar_id
         if not UtilClient.is_unset(request.jwt_token):
             body['JwtToken'] = request.jwt_token
+        if not UtilClient.is_unset(request.selected_box_index):
+            body['SelectedBoxIndex'] = request.selected_box_index
         if not UtilClient.is_unset(request.title):
             body['Title'] = request.title
         if not UtilClient.is_unset(request.video_id):
             body['VideoId'] = request.video_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
```

### Comparing `alibabacloud_xrengine20230313-2.9.2/alibabacloud_xrengine20230313/models.py` & `alibabacloud_xrengine20230313-2.9.3/alibabacloud_xrengine20230313/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -19967,20 +19967,22 @@
 
 class QueryMotionShopVideoDetectResultResponseBodyDataDetectResult(TeaModel):
     def __init__(
         self,
         box: List[float] = None,
         code: int = None,
         cover_url: str = None,
+        human_boxes: List[List[float]] = None,
         message: str = None,
         selected_frame_index: int = None,
     ):
         self.box = box
         self.code = code
         self.cover_url = cover_url
+        self.human_boxes = human_boxes
         self.message = message
         self.selected_frame_index = selected_frame_index
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -19991,28 +19993,32 @@
         result = dict()
         if self.box is not None:
             result['Box'] = self.box
         if self.code is not None:
             result['Code'] = self.code
         if self.cover_url is not None:
             result['CoverUrl'] = self.cover_url
+        if self.human_boxes is not None:
+            result['HumanBoxes'] = self.human_boxes
         if self.message is not None:
             result['Message'] = self.message
         if self.selected_frame_index is not None:
             result['SelectedFrameIndex'] = self.selected_frame_index
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Box') is not None:
             self.box = m.get('Box')
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('CoverUrl') is not None:
             self.cover_url = m.get('CoverUrl')
+        if m.get('HumanBoxes') is not None:
+            self.human_boxes = m.get('HumanBoxes')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('SelectedFrameIndex') is not None:
             self.selected_frame_index = m.get('SelectedFrameIndex')
         return self
 
 
@@ -20283,19 +20289,21 @@
 
 
 class SubmitMotionShopTaskRequest(TeaModel):
     def __init__(
         self,
         avatar_id: str = None,
         jwt_token: str = None,
+        selected_box_index: int = None,
         title: str = None,
         video_id: str = None,
     ):
         self.avatar_id = avatar_id
         self.jwt_token = jwt_token
+        self.selected_box_index = selected_box_index
         self.title = title
         self.video_id = video_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -20304,26 +20312,30 @@
             return _map
 
         result = dict()
         if self.avatar_id is not None:
             result['AvatarId'] = self.avatar_id
         if self.jwt_token is not None:
             result['JwtToken'] = self.jwt_token
+        if self.selected_box_index is not None:
+            result['SelectedBoxIndex'] = self.selected_box_index
         if self.title is not None:
             result['Title'] = self.title
         if self.video_id is not None:
             result['VideoId'] = self.video_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AvatarId') is not None:
             self.avatar_id = m.get('AvatarId')
         if m.get('JwtToken') is not None:
             self.jwt_token = m.get('JwtToken')
+        if m.get('SelectedBoxIndex') is not None:
+            self.selected_box_index = m.get('SelectedBoxIndex')
         if m.get('Title') is not None:
             self.title = m.get('Title')
         if m.get('VideoId') is not None:
             self.video_id = m.get('VideoId')
         return self
```

### Comparing `alibabacloud_xrengine20230313-2.9.2/alibabacloud_xrengine20230313.egg-info/PKG-INFO` & `alibabacloud_xrengine20230313-2.9.3/alibabacloud_xrengine20230313.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-xrengine20230313
-Version: 2.9.2
+Version: 2.9.3
 Summary: Alibaba Cloud xrEngine (20230313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_xrengine20230313-2.9.2/setup.py` & `alibabacloud_xrengine20230313-2.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_xrengine20230313.
 
-Created on 26/03/2024
+Created on 11/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_xrengine20230313"
 NAME = "alibabacloud_xrengine20230313" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud xrEngine (20230313) SDK Library for Python"
```

