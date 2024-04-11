# Comparing `tmp/alibabacloud_green20220302-2.2.2.tar.gz` & `tmp/alibabacloud_green20220302-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_green20220302-2.2.2.tar", last modified: Tue Mar 26 17:10:26 2024, max compression
+gzip compressed data, was "dist/alibabacloud_green20220302-2.2.3.tar", last modified: Thu Apr 11 11:25:55 2024, max compression
```

## Comparing `alibabacloud_green20220302-2.2.2.tar` & `alibabacloud_green20220302-2.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 17:10:26.000000 alibabacloud_green20220302-2.2.2/
--rw-r--r--   0 root         (0) root         (0)      951 2024-03-26 17:10:25.000000 alibabacloud_green20220302-2.2.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-26 17:10:25.000000 alibabacloud_green20220302-2.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-26 17:10:25.000000 alibabacloud_green20220302-2.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2415 2024-03-26 17:10:26.000000 alibabacloud_green20220302-2.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1103 2024-03-26 17:10:25.000000 alibabacloud_green20220302-2.2.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1188 2024-03-26 17:10:25.000000 alibabacloud_green20220302-2.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 17:10:26.000000 alibabacloud_green20220302-2.2.2/alibabacloud_green20220302/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-26 17:10:25.000000 alibabacloud_green20220302-2.2.2/alibabacloud_green20220302/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50071 2024-03-26 17:10:25.000000 alibabacloud_green20220302-2.2.2/alibabacloud_green20220302/client.py
--rw-r--r--   0 root         (0) root         (0)   117833 2024-03-26 17:10:25.000000 alibabacloud_green20220302-2.2.2/alibabacloud_green20220302/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 17:10:26.000000 alibabacloud_green20220302-2.2.2/alibabacloud_green20220302.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2415 2024-03-26 17:10:26.000000 alibabacloud_green20220302-2.2.2/alibabacloud_green20220302.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2024-03-26 17:10:26.000000 alibabacloud_green20220302-2.2.2/alibabacloud_green20220302.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 17:10:26.000000 alibabacloud_green20220302-2.2.2/alibabacloud_green20220302.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-26 17:10:26.000000 alibabacloud_green20220302-2.2.2/alibabacloud_green20220302.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-03-26 17:10:26.000000 alibabacloud_green20220302-2.2.2/alibabacloud_green20220302.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-26 17:10:26.000000 alibabacloud_green20220302-2.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2621 2024-03-26 17:10:25.000000 alibabacloud_green20220302-2.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50071 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302/client.py
+-rw-r--r--   0 root         (0) root         (0)   119635 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2621 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/setup.py
```

### Comparing `alibabacloud_green20220302-2.2.2/ChangeLog.md` & `alibabacloud_green20220302-2.2.3/ChangeLog.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+2024-03-26 Version: 2.2.2
+- Update API VideoModeration: update response param.
+- Update API VideoModerationResult: update response param.
+- Update API VoiceModeration: update response param.
+- Update API VoiceModerationResult: update response param.
+
+
 2024-02-01 Version: 2.2.1
 - Generated python 2022-03-02 for Green.
 
 2024-01-31 Version: 2.2.0
 - Support API DescribeUrlModerationResult.
 - Support API UrlAsyncModeration.
```

### Comparing `alibabacloud_green20220302-2.2.2/LICENSE` & `alibabacloud_green20220302-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.2/PKG-INFO` & `alibabacloud_green20220302-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_green20220302
-Version: 2.2.2
+Version: 2.2.3
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-2.2.2/README-CN.md` & `alibabacloud_green20220302-2.2.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.2/README.md` & `alibabacloud_green20220302-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.2/alibabacloud_green20220302/client.py` & `alibabacloud_green20220302-2.2.3/alibabacloud_green20220302/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.2/alibabacloud_green20220302/models.py` & `alibabacloud_green20220302-2.2.3/alibabacloud_green20220302/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -750,40 +750,93 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('FigureId') is not None:
             self.figure_id = m.get('FigureId')
         return self
 
 
+class DescribeImageResultExtResponseBodyDataTextInImageCustomTexts(TeaModel):
+    def __init__(
+        self,
+        key_words: str = None,
+        lib_id: str = None,
+        lib_name: str = None,
+    ):
+        self.key_words = key_words
+        self.lib_id = lib_id
+        self.lib_name = lib_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key_words is not None:
+            result['KeyWords'] = self.key_words
+        if self.lib_id is not None:
+            result['LibId'] = self.lib_id
+        if self.lib_name is not None:
+            result['LibName'] = self.lib_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('KeyWords') is not None:
+            self.key_words = m.get('KeyWords')
+        if m.get('LibId') is not None:
+            self.lib_id = m.get('LibId')
+        if m.get('LibName') is not None:
+            self.lib_name = m.get('LibName')
+        return self
+
+
 class DescribeImageResultExtResponseBodyDataTextInImage(TeaModel):
     def __init__(
         self,
+        custom_texts: List[DescribeImageResultExtResponseBodyDataTextInImageCustomTexts] = None,
         ocr_datas: List[str] = None,
         risk_words: List[str] = None,
     ):
+        self.custom_texts = custom_texts
         self.ocr_datas = ocr_datas
         self.risk_words = risk_words
 
     def validate(self):
-        pass
+        if self.custom_texts:
+            for k in self.custom_texts:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        result['CustomTexts'] = []
+        if self.custom_texts is not None:
+            for k in self.custom_texts:
+                result['CustomTexts'].append(k.to_map() if k else None)
         if self.ocr_datas is not None:
             result['OcrDatas'] = self.ocr_datas
         if self.risk_words is not None:
             result['RiskWords'] = self.risk_words
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        self.custom_texts = []
+        if m.get('CustomTexts') is not None:
+            for k in m.get('CustomTexts'):
+                temp_model = DescribeImageResultExtResponseBodyDataTextInImageCustomTexts()
+                self.custom_texts.append(temp_model.from_map(k))
         if m.get('OcrDatas') is not None:
             self.ocr_datas = m.get('OcrDatas')
         if m.get('RiskWords') is not None:
             self.risk_words = m.get('RiskWords')
         return self
```

### Comparing `alibabacloud_green20220302-2.2.2/alibabacloud_green20220302.egg-info/PKG-INFO` & `alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-green20220302
-Version: 2.2.2
+Version: 2.2.3
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-2.2.2/setup.py` & `alibabacloud_green20220302-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_green20220302.
 
-Created on 26/03/2024
+Created on 11/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_green20220302"
 NAME = "alibabacloud_green20220302" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Green (20220302) SDK Library for Python"
```
