# Comparing `tmp/ffmpeg_media_type-0.0.8.tar.gz` & `tmp/ffmpeg_media_type-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_media_type-0.0.8.tar", max compression
+gzip compressed data, was "ffmpeg_media_type-0.0.9.tar", max compression
```

## Comparing `ffmpeg_media_type-0.0.8.tar` & `ffmpeg_media_type-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1066 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/LICENSE
--rw-r--r--   0        0        0     4904 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/README.md
--rw-r--r--   0        0        0     1589 2023-10-16 06:26:25.089655 ffmpeg_media_type-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      186 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/__init__.py
--rw-r--r--   0        0        0      763 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/conftest.py
--rw-r--r--   0        0        0        0 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/__init__.py
--rw-r--r--   0        0        0    89367 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-3.2.json
--rw-r--r--   0        0        0    91003 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-3.3.json
--rw-r--r--   0        0        0    92339 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-3.4.json
--rw-r--r--   0        0        0    94852 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-4.0.json
--rw-r--r--   0        0        0    95951 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-4.1.json
--rw-r--r--   0        0        0    97292 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-4.2.json
--rw-r--r--   0        0        0   100111 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-4.3.json
--rw-r--r--   0        0        0   106316 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-4.4.json
--rw-r--r--   0        0        0   107177 2023-10-16 06:26:01.929521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-5.0.json
--rw-r--r--   0        0        0   109161 2023-10-16 06:26:01.933521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-5.1.json
--rw-r--r--   0        0        0   120284 2023-10-16 06:26:01.933521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-6.0.json
--rw-r--r--   0        0        0     3689 2023-10-16 06:26:01.933521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/info.py
--rw-r--r--   0        0        0      378 2023-10-16 06:26:01.933521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/main.py
--rw-r--r--   0        0        0        0 2023-10-16 06:26:01.933521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/py.typed
--rw-r--r--   0        0        0        0 2023-10-16 06:26:01.933521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/utils/__init__.py
--rw-r--r--   0        0        0     6977 2023-10-16 06:26:01.933521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/utils/ffmpeg.py
--rw-r--r--   0        0        0      431 2023-10-16 06:26:01.933521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/utils/shell.py
--rw-r--r--   0        0        0     2977 2023-10-16 06:26:01.933521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/utils/table.py
--rw-r--r--   0        0        0     1790 2023-10-16 06:26:02.049521 ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/utils/wiki_ext.py
--rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 ffmpeg_media_type-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4904 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/README.md
+-rw-r--r--   0        0        0     1589 2023-10-17 04:08:52.482603 ffmpeg_media_type-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      186 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/__init__.py
+-rw-r--r--   0        0        0      763 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/conftest.py
+-rw-r--r--   0        0        0        0 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/__init__.py
+-rw-r--r--   0        0        0    89367 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-3.2.json
+-rw-r--r--   0        0        0    91003 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-3.3.json
+-rw-r--r--   0        0        0    92339 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-3.4.json
+-rw-r--r--   0        0        0    94852 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.0.json
+-rw-r--r--   0        0        0    95951 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.1.json
+-rw-r--r--   0        0        0    97292 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.2.json
+-rw-r--r--   0        0        0   100111 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.3.json
+-rw-r--r--   0        0        0   106316 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.4.json
+-rw-r--r--   0        0        0   107177 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-5.0.json
+-rw-r--r--   0        0        0   109161 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-5.1.json
+-rw-r--r--   0        0        0   120284 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-6.0.json
+-rw-r--r--   0        0        0       47 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/exceptions.py
+-rw-r--r--   0        0        0     3689 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/info.py
+-rw-r--r--   0        0        0      378 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/main.py
+-rw-r--r--   0        0        0        0 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/py.typed
+-rw-r--r--   0        0        0        0 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/utils/__init__.py
+-rw-r--r--   0        0        0     6977 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/utils/ffmpeg.py
+-rw-r--r--   0        0        0      514 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/utils/shell.py
+-rw-r--r--   0        0        0     2977 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/utils/table.py
+-rw-r--r--   0        0        0     1790 2023-10-17 04:08:32.074320 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/utils/wiki_ext.py
+-rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 ffmpeg_media_type-0.0.9/PKG-INFO
```

### Comparing `ffmpeg_media_type-0.0.8/LICENSE` & `ffmpeg_media_type-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/README.md` & `ffmpeg_media_type-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/pyproject.toml` & `ffmpeg_media_type-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ffmpeg-media-type"
-version = "0.0.8"
+version = "0.0.9"
 description = "ffmpeg-media-type is a Python library that utilizes FFmpeg to extract crucial details from media files, such as duration, width, and height. With seamless integration of 100% typehint support, it offers a user-friendly interface for easy access to media file information."
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "ffmpeg_media_type", from = "src" }]
 include = ["ffmpeg_media_type/py.typed", "ffmpeg_media_type/data/*.json"]
 exclude = ["**/tests"]
 keywords = ["ffmpeg", "ffprobe", "video", "image", "audio", "media", "mimetype", "mp4", "mp3", "mov", "webm"]
```

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/conftest.py` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/conftest.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-3.2.json` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-3.2.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-3.3.json` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-3.3.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-3.4.json` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-3.4.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-4.0.json` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.0.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-4.1.json` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.1.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-4.2.json` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.2.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-4.3.json` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.3.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-4.4.json` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.4.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-5.0.json` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-5.0.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-5.1.json` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-5.1.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/data/ffmpeg-6.0.json` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-6.0.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/info.py` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/info.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/utils/ffmpeg.py` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/utils/table.py` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/utils/table.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/src/ffmpeg_media_type/utils/wiki_ext.py` & `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/utils/wiki_ext.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.8/PKG-INFO` & `ffmpeg_media_type-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-media-type
-Version: 0.0.8
+Version: 0.0.9
 Summary: ffmpeg-media-type is a Python library that utilizes FFmpeg to extract crucial details from media files, such as duration, width, and height. With seamless integration of 100% typehint support, it offers a user-friendly interface for easy access to media file information.
 Keywords: ffmpeg,ffprobe,video,image,audio,media,mimetype,mp4,mp3,mov,webm
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

