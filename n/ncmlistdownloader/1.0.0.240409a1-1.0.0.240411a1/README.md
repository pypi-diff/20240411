# Comparing `tmp/ncmlistdownloader-1.0.0.240409a1.tar.gz` & `tmp/ncmlistdownloader-1.0.0.240411a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.0.240409a1.tar", last modified: Tue Apr  9 14:53:52 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.0.240411a1.tar", last modified: Thu Apr 11 14:57:45 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.0.240409a1.tar` & `ncmlistdownloader-1.0.0.240411a1.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 14:53:52.172753 ncmlistdownloader-1.0.0.240409a1/
--rw-rw-rw-   0        0        0    35181 2024-03-07 09:37:50.000000 ncmlistdownloader-1.0.0.240409a1/LICENSE
--rw-rw-rw-   0        0        0     1399 2024-04-09 14:53:52.170759 ncmlistdownloader-1.0.0.240409a1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-09 14:53:52.130973 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1264 2024-04-08 14:52:37.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:53:52.155817 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2859 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2248 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2137 2024-04-08 14:53:36.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1784 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:53:52.158800 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6526 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:53:52.160786 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     3929 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:53:52.163782 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     1745 2024-04-09 14:52:18.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:53:52.164775 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     7391 2024-04-09 14:52:21.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:53:52.167768 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1399 2024-04-09 14:53:52.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      606 2024-04-09 14:53:52.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 14:53:52.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-09 14:53:52.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-09 14:53:52.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-09 14:53:52.000000 ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 14:53:52.172753 ncmlistdownloader-1.0.0.240409a1/setup.cfg
--rw-rw-rw-   0        0        0     1700 2024-04-09 14:53:07.000000 ncmlistdownloader-1.0.0.240409a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.419854 ncmlistdownloader-1.0.0.240411a1/
+-rw-rw-rw-   0        0        0    35181 2024-03-07 09:37:50.000000 ncmlistdownloader-1.0.0.240411a1/LICENSE
+-rw-rw-rw-   0        0        0     1424 2024-04-11 14:57:45.419854 ncmlistdownloader-1.0.0.240411a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.357376 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1264 2024-04-08 14:52:37.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.372996 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/cmd/
+-rw-rw-rw-   0        0        0     2700 2024-04-11 14:57:18.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/cmd/__init__.py
+-rw-rw-rw-   0        0        0     1182 2024-04-11 14:57:22.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/cmd/module.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.388612 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2859 2024-04-10 14:43:02.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2325 2024-04-10 09:59:47.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2213 2024-04-10 10:20:01.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1784 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.404472 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6526 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.404472 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3929 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.404472 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     1814 2024-04-11 14:57:28.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.404472 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     7424 2024-04-10 10:20:08.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.419854 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1424 2024-04-11 14:57:45.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      672 2024-04-11 14:57:45.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 14:57:45.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-11 14:57:45.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       46 2024-04-11 14:57:45.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-11 14:57:45.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 14:57:45.419854 ncmlistdownloader-1.0.0.240411a1/setup.cfg
+-rw-rw-rw-   0        0        0     1711 2024-04-11 14:56:54.000000 ncmlistdownloader-1.0.0.240411a1/setup.py
```

### Comparing `ncmlistdownloader-1.0.0.240409a1/LICENSE` & `ncmlistdownloader-1.0.0.240411a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240409a1/PKG-INFO` & `ncmlistdownloader-1.0.0.240411a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240409a1
+Version: 1.0.0.240411a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -25,7 +25,8 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 Requires-Dist: pycryptodome
 Requires-Dist: pillow
 Requires-Dist: mutagen
 Requires-Dist: requests
+Requires-Dist: keyboard
```

### Comparing `ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/encode_sec_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 网易云WeAPI解码
-Core.Ver.1.0.0.240404b4-2
+Core.Ver.1.0.0.240410a1
 Author: CooooldWind_, 半岛的孤城
 References: 
 1. 网易云解参数（获取网易云歌词，获取评论同理）[https://www.bilibili.com/read/cv12754897/]
 '''
 
 import random
 import json
@@ -25,41 +25,42 @@
         self.encode_data = encode_data
         self.url = url
         self.func_e = "010001"
         self.func_f = FUNC_F
         self.func_g = "0CoJUm6Qyw8W8jud"
         self.func_i = "vlgPRPyGhwA6F4Sq"
         self.encode_sec_key = SEC_KEY
-    def to_hex(self, encode_data):
+    def __to_hex(self, encode_data):
         '''16进制解码'''
         temp = 16 - len(encode_data) % 16
         return encode_data + chr(temp) * temp
-    def encode_params(self, encode_data, encode_key):
+    def __encode_params(self, encode_data, encode_key):
         '''解码的关键函数(1)'''
         func_iv = "0102030405060708"
-        encode_data = self.to_hex(encode_data)
+        encode_data = self.__to_hex(encode_data)
         encode_aes = AES.new(key = encode_key.encode("utf-8"),
                             IV = func_iv.encode("utf-8"),
                             mode = AES.MODE_CBC)
         base64_sec_key = encode_aes.encrypt(encode_data.encode("utf-8"))
         return str(b64encode(base64_sec_key), "utf-8")
-    def get_params(self, encode_data):
+    def __get_params(self, encode_data):
         '''解码的关键函数(2)'''
-        return self.encode_params(
-            self.encode_params(
+        return self.__encode_params(
+            self.__encode_params(
                 encode_data, self.func_g
             ), self.func_i
         )
-    def get_resource(self):
+    def get_resource(self, cookies = None):
         '''获取资源'''
         get_data = {
-            'params': self.get_params(json.dumps(self.encode_data)),
+            'params': self.__get_params(json.dumps(self.encode_data)),
             'encSecKey': self.encode_sec_key
         }
         get_headers = {
             'User-Agent': random.choice(USER_AGENTS)
         }
         response = requests.post(self.url,
                              data = get_data,
                              headers = get_headers,
+                             cookies = cookies,
                              timeout = 10)
         return response.json()
```

### Comparing `ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/global_args.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 list_downloader/global_args.py
-Core.Ver.1.0.0.240408a1
+Core.Ver.1.0.0.240410a1
 Author: CooooldWind_, 是青旨啊
 '''
 FUNC_F_PART = [
   "00e0b509f6259df8642dbc35662901477df22677ec152b5ff68ace615bb7",
   "b725152b3ab17a876aea8a5aa76d2e417629ec4ee341f56135fccf695280",
   "104e0312ecbda92557c93870114af6c9d05c4f7f0c3685b7a46bee255932",
   "575cce10b424d813cfe4875d3e82047b97ddef52741d546b8e289dc6935b",
@@ -35,14 +35,15 @@
 USER_AGENTS = json_file['USER_AGENTS']
 FUNC_F = json_file['FUNC_F']
 SEC_KEY = json_file['SEC_KEY']
 PLAYLIST_API = json_file['PLAYLIST_API']
 SONG_INFO_API = json_file['SONG_INFO_API']
 SONG_FILE_API = json_file['SONG_FILE_API']
 SONG_FILE_API_2 = json_file['SONG_FILE_API_2']
+SEARCH_API = "https://music.163.com/weapi/cloudsearch/get/web?csrf_token="
 LYRIC_API = json_file['LYRIC_API']
 CMD_START_WORDS = [
     "163ListDownloader CMD Ver.",
     "Made by CooooldWind_",
     "Warning: It's an Alpha Version. It may has a lot of bugs.",
     "If you met them, click the links below:",
     "Gitee: https://gitee.com/CooooldWind/163ListDownloader_NexT/issues",
```

### Comparing `ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/playlist/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 ncmlistdownloader/playlist/__init__.py
-Core.Ver.1.0.0.240409a1
+Core.Ver.1.0.0.240411a1
 Author: CooooldWind_
 '''
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.global_args import *
 from ncmlistdownloader.song import *
 import threading
@@ -16,24 +16,26 @@
             self.id = url_split(url = self.id)
         self.track: list[Song] = []
         self.creator_id = ""
         self.raw_info = {}
         self.track_count = int(0)
         self.creator = ""
         self.track_id = []
+        self.title = ""
 
     def get_info(self):
         self.raw_info = NeteaseParams(url = PLAYLIST_API,
                                       encode_data = {
                                           'csrf_token': '',
                                           'id': self.id,
                                       }).get_resource()['playlist']
         self.creator_id = self.raw_info['userId']
         self.track_count = self.raw_info['trackCount']
         self.creator = self.raw_info['creator']['nickname']
+        self.title = self.raw_info['name']
         for i in self.raw_info['trackIds']:
             self.track_id.append(str(i['id']))
         for truck_id in self.track_id:
             self.track.append(Song(id = truck_id))
         return self.raw_info
     
     def get_detail_info(self):
```

### Comparing `ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/song/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 ncmlistdownloader/song/__init__.py
-Core.Ver.1.0.0.240409a1
+Core.Ver.1.0.0.240410a1
 Author: CooooldWind_
 '''
 
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.thread_test import best_thread
 from ncmlistdownloader.downloader import *
@@ -112,15 +112,15 @@
         获取歌曲信息（多线程用）
         ----------
         无参数。
         '''
         with threading.Semaphore(8):
             self.get_info()
 
-    def song_download_enhanced(self, level: str):
+    def song_download_enhanced(self, level: str, cookies = None):
         flag = True
         level_key = [
             'standard',
             'higher',
             'exhigh',
             'lossless'
         ]
@@ -150,15 +150,15 @@
             'encodeType': 'mp3',
             'csrf_token': '',
         }
         if level == 'lossless': enhance_encode_data['encodeType'] = 'aac'
         enhanced_info = NeteaseParams(
             encode_data = enhance_encode_data,
             url = SONG_FILE_API_2
-        ).get_resource()
+        ).get_resource(cookies = cookies)
         return enhanced_info
 
     def song_download(self):
         filename = self.get_formated_filename('mp3')
         file_origin = OriginFile(self.url_info['song_file'])
         if file_origin.total_size <= 0:
             return -1
```

### Comparing `ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240409a1
+Version: 1.0.0.240411a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -25,7 +25,8 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 Requires-Dist: pycryptodome
 Requires-Dist: pillow
 Requires-Dist: mutagen
 Requires-Dist: requests
+Requires-Dist: keyboard
```

### Comparing `ncmlistdownloader-1.0.0.240409a1/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 ncmlistdownloader/__init__.py
 ncmlistdownloader.egg-info/PKG-INFO
 ncmlistdownloader.egg-info/SOURCES.txt
 ncmlistdownloader.egg-info/dependency_links.txt
 ncmlistdownloader.egg-info/entry_points.txt
 ncmlistdownloader.egg-info/requires.txt
 ncmlistdownloader.egg-info/top_level.txt
+ncmlistdownloader/cmd/__init__.py
+ncmlistdownloader/cmd/module.py
 ncmlistdownloader/common/__init__.py
 ncmlistdownloader/common/encode_sec_key.py
 ncmlistdownloader/common/global_args.py
 ncmlistdownloader/common/thread_test.py
 ncmlistdownloader/downloader/__init__.py
 ncmlistdownloader/editer/__init__.py
 ncmlistdownloader/playlist/__init__.py
```

### Comparing `ncmlistdownloader-1.0.0.240409a1/setup.py` & `ncmlistdownloader-1.0.0.240411a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Programming Language :: Python :: 3.12',
     ],
     name = 'ncmlistdownloader',
-    version = "1.0.0.240409a1",
+    version = "1.0.0.240411a1",
     description = '获取网易云音乐歌单数据，下载音乐，主动添加元信息。',
     author = 'CooooldWind_',
     url = 'https://gitee.com/Cooooldwind/163ListDownloader_NexT',
     packages = find_packages(),
-    install_requires = ['pycryptodome','pillow','mutagen','requests',],
+    install_requires = ['pycryptodome','pillow','mutagen','requests','keyboard',],
     entry_points = {'console_scripts': ['ncmlistdownloader = ncmlistdownloader.__init__:main']},
 )
```

