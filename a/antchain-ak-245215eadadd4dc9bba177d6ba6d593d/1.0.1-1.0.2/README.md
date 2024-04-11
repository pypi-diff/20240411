# Comparing `tmp/antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1.tar.gz` & `tmp/antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1.tar", last modified: Tue Mar 19 09:41:14 2024, max compression
+gzip compressed data, was "dist/antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2.tar", last modified: Thu Apr 11 03:38:57 2024, max compression
```

## Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1.tar` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 09:41:14.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-19 09:41:13.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-19 09:41:13.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2024-03-19 09:41:14.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2024-03-19 09:41:13.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2024-03-19 09:41:13.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 09:41:14.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2024-03-19 09:41:14.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2024-03-19 09:41:14.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 09:41:14.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-03-19 09:41:14.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-03-19 09:41:14.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 09:41:14.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-19 09:41:13.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24398 2024-03-19 09:41:13.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/client.py
--rw-r--r--   0 root         (0) root         (0)    37129 2024-03-19 09:41:13.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-19 09:41:14.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2024-03-19 09:41:13.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24398 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/client.py
+-rw-r--r--   0 root         (0) root         (0)    39483 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/setup.py
```

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/LICENSE` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/PKG-INFO` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_245215eadadd4dc9bba177d6ba6d593d
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ant Chain Ak_245215eadadd4dc9bba177d6ba6d593d SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/README-CN.md` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/README.md` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/PKG-INFO` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-245215eadadd4dc9bba177d6ba6d593d
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ant Chain Ak_245215eadadd4dc9bba177d6ba6d593d SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/SOURCES.txt` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/client.py` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.1',
+                    'sdk_version': '1.0.2',
                     '_prod_code': 'ak_245215eadadd4dc9bba177d6ba6d593d',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.1',
+                    'sdk_version': '1.0.2',
                     '_prod_code': 'ak_245215eadadd4dc9bba177d6ba6d593d',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/models.py` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 
 class Paster(TeaModel):
     def __init__(
         self,
         x: int = None,
         y: int = None,
         src_url: str = None,
-        scale: int = None,
+        scale: str = None,
     ):
         # 贴片元素离画面位置x坐标
         self.x = x
         # 贴片元素离画面位置y坐标
         self.y = y
         # 贴片元素 url,支持 gif png jpg等图片格式
         self.src_url = src_url
@@ -318,15 +318,15 @@
 
 
 class ScriptVoiceConfig(TeaModel):
     def __init__(
         self,
         voice_id: str = None,
         text: str = None,
-        speed: int = None,
+        speed: str = None,
         audio_url: str = None,
     ):
         # 音色id，合成驱动选择text时必填
         self.voice_id = voice_id
         # 话术脚本内容，合成驱动选择text时必填
         self.text = text
         # 0.5～2，语速，合成驱动选择text时必填
@@ -552,14 +552,75 @@
         if m.get('item_list') is not None:
             for k in m.get('item_list'):
                 temp_model = AvatarProfile()
                 self.item_list.append(temp_model.from_map(k))
         return self
 
 
+class ProfileInfo(TeaModel):
+    def __init__(
+        self,
+        x: int = None,
+        y: int = None,
+        w: int = None,
+        h: int = None,
+        scale: str = None,
+    ):
+        # 数字人离画面位置坐标,可以为负数或者出画
+        # 数字人在视频生成中的位置
+        self.x = x
+        # 数字人离画面位置坐标,可以为负数或者出画
+        # 数字人在视频生成中的位置
+        self.y = y
+        # 数字人视频大小,初始大小为训练素材整体大小非数字人在框选大小
+        self.w = w
+        # 数字人视频大小,初始大小为训练素材整体大小非数字人在框选大小
+        self.h = h
+        # 数字人视频大小缩放,实际大小为  scale*w   scale*h
+        self.scale = scale
+
+    def validate(self):
+        self.validate_required(self.x, 'x')
+        self.validate_required(self.y, 'y')
+        self.validate_required(self.w, 'w')
+        self.validate_required(self.h, 'h')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.x is not None:
+            result['x'] = self.x
+        if self.y is not None:
+            result['y'] = self.y
+        if self.w is not None:
+            result['w'] = self.w
+        if self.h is not None:
+            result['h'] = self.h
+        if self.scale is not None:
+            result['scale'] = self.scale
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('x') is not None:
+            self.x = m.get('x')
+        if m.get('y') is not None:
+            self.y = m.get('y')
+        if m.get('w') is not None:
+            self.w = m.get('w')
+        if m.get('h') is not None:
+            self.h = m.get('h')
+        if m.get('scale') is not None:
+            self.scale = m.get('scale')
+        return self
+
+
 class VideoTask(TeaModel):
     def __init__(
         self,
         state: str = None,
         video_url: str = None,
     ):
         # RUNNING, COMPLETE,FAIL
@@ -591,15 +652,15 @@
         return self
 
 
 class Background(TeaModel):
     def __init__(
         self,
         src_url: str = None,
-        scale: int = None,
+        scale: str = None,
         x: int = None,
         y: int = None,
     ):
         # 背景元素，支持 gif png jpg mp4等格式
         self.src_url = src_url
         # 背景缩放比例
         self.scale = scale
@@ -862,28 +923,31 @@
 class CreateUniversalsaasDigitalhumanVideoTaskRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         avatar_id: str = None,
         driver_type: str = None,
+        profile_info: ProfileInfo = None,
         script_voice_config: ScriptVoiceConfig = None,
         open_captions: bool = None,
         captions_info: CaptionsInfo = None,
         replace_sensitive: bool = None,
         background: Background = None,
         pasters: List[Paster] = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 数字人id
         self.avatar_id = avatar_id
         # text/audio, 合成驱动--文本/音频
         self.driver_type = driver_type
+        # 形象设置
+        self.profile_info = profile_info
         # 话术脚本语音配置
         self.script_voice_config = script_voice_config
         # 是否开启字幕
         self.open_captions = open_captions
         # 字幕配置
         self.captions_info = captions_info
         # 是否替换字幕敏感词
@@ -892,14 +956,16 @@
         self.background = background
         # 贴片元素信息
         self.pasters = pasters
 
     def validate(self):
         self.validate_required(self.avatar_id, 'avatar_id')
         self.validate_required(self.driver_type, 'driver_type')
+        if self.profile_info:
+            self.profile_info.validate()
         self.validate_required(self.script_voice_config, 'script_voice_config')
         if self.script_voice_config:
             self.script_voice_config.validate()
         self.validate_required(self.open_captions, 'open_captions')
         if self.captions_info:
             self.captions_info.validate()
         if self.background:
@@ -919,14 +985,16 @@
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.avatar_id is not None:
             result['avatar_id'] = self.avatar_id
         if self.driver_type is not None:
             result['driver_type'] = self.driver_type
+        if self.profile_info is not None:
+            result['profile_info'] = self.profile_info.to_map()
         if self.script_voice_config is not None:
             result['script_voice_config'] = self.script_voice_config.to_map()
         if self.open_captions is not None:
             result['open_captions'] = self.open_captions
         if self.captions_info is not None:
             result['captions_info'] = self.captions_info.to_map()
         if self.replace_sensitive is not None:
@@ -945,14 +1013,17 @@
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('avatar_id') is not None:
             self.avatar_id = m.get('avatar_id')
         if m.get('driver_type') is not None:
             self.driver_type = m.get('driver_type')
+        if m.get('profile_info') is not None:
+            temp_model = ProfileInfo()
+            self.profile_info = temp_model.from_map(m['profile_info'])
         if m.get('script_voice_config') is not None:
             temp_model = ScriptVoiceConfig()
             self.script_voice_config = temp_model.from_map(m['script_voice_config'])
         if m.get('open_captions') is not None:
             self.open_captions = m.get('open_captions')
         if m.get('captions_info') is not None:
             temp_model = CaptionsInfo()
```

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.1/setup.py` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_245215eadadd4dc9bba177d6ba6d593d.
 
-Created on 19/03/2024
+Created on 11/04/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d"
 NAME = "antchain_ak_245215eadadd4dc9bba177d6ba6d593d" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_245215eadadd4dc9bba177d6ba6d593d SDK Library for Python"
```

