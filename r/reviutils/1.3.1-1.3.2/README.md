# Comparing `tmp/reviutils-1.3.1.tar.gz` & `tmp/reviutils-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reviutils-1.3.1.tar", last modified: Wed Mar 27 06:45:04 2024, max compression
+gzip compressed data, was "reviutils-1.3.2.tar", last modified: Thu Apr 11 07:42:23 2024, max compression
```

## Comparing `reviutils-1.3.1.tar` & `reviutils-1.3.2.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 06:45:04.052768 reviutils-1.3.1/
--rw-rw-rw-   0        0        0    11558 2024-03-14 03:50:07.000000 reviutils-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     2814 2024-03-27 06:45:04.052178 reviutils-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2490 2024-03-27 06:32:09.000000 reviutils-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 06:45:04.023096 reviutils-1.3.1/reviutils/
-drwxrwxrwx   0        0        0        0 2024-03-27 06:45:04.035782 reviutils-1.3.1/reviutils/api/
--rw-rw-rw-   0        0        0       57 2024-03-27 06:31:11.000000 reviutils-1.3.1/reviutils/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:45:04.038782 reviutils-1.3.1/reviutils/api/amap/
--rw-rw-rw-   0        0        0     2495 2024-03-27 06:27:05.000000 reviutils-1.3.1/reviutils/api/amap/__init__.py
--rw-rw-rw-   0        0        0      168 2024-03-27 06:24:54.000000 reviutils-1.3.1/reviutils/api/amap/enums.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:45:04.042286 reviutils-1.3.1/reviutils/audio/
--rw-rw-rw-   0        0        0      116 2024-03-20 03:20:30.000000 reviutils-1.3.1/reviutils/audio/__init__.py
--rw-rw-rw-   0        0        0     3232 2024-03-18 03:19:04.000000 reviutils-1.3.1/reviutils/audio/clipper.py
--rw-rw-rw-   0        0        0     1534 2024-03-20 03:42:36.000000 reviutils-1.3.1/reviutils/audio/reader.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:45:04.043874 reviutils-1.3.1/reviutils/common/
--rw-rw-rw-   0        0        0     3467 2024-03-15 02:38:48.000000 reviutils-1.3.1/reviutils/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:45:04.051178 reviutils-1.3.1/reviutils/noisepollution/
--rw-rw-rw-   0        0        0      314 2024-03-20 03:21:45.000000 reviutils-1.3.1/reviutils/noisepollution/__init__.py
--rw-rw-rw-   0        0        0     1994 2024-03-14 08:34:09.000000 reviutils-1.3.1/reviutils/noisepollution/evaluation.py
--rw-rw-rw-   0        0        0     4114 2024-03-19 08:00:42.000000 reviutils-1.3.1/reviutils/noisepollution/funcarea.py
--rw-rw-rw-   0        0        0     1043 2024-03-20 03:33:29.000000 reviutils-1.3.1/reviutils/noisepollution/hourhelper.py
--rw-rw-rw-   0        0        0     7313 2024-03-15 02:38:48.000000 reviutils-1.3.1/reviutils/noisepollution/splhelper.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:45:04.034782 reviutils-1.3.1/reviutils.egg-info/
--rw-rw-rw-   0        0        0     2814 2024-03-27 06:45:03.000000 reviutils-1.3.1/reviutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      607 2024-03-27 06:45:03.000000 reviutils-1.3.1/reviutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 06:45:03.000000 reviutils-1.3.1/reviutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-27 06:45:03.000000 reviutils-1.3.1/reviutils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       91 2024-03-27 06:45:03.000000 reviutils-1.3.1/reviutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-27 06:45:03.000000 reviutils-1.3.1/reviutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 06:45:04.052768 reviutils-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1469 2024-03-27 06:44:22.000000 reviutils-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:42:23.771665 reviutils-1.3.2/
+-rw-rw-rw-   0        0        0    11558 2024-03-14 03:50:07.000000 reviutils-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     2814 2024-04-11 07:42:23.770664 reviutils-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2490 2024-03-27 06:32:09.000000 reviutils-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 07:42:23.738664 reviutils-1.3.2/reviutils/
+drwxrwxrwx   0        0        0        0 2024-04-11 07:42:23.750664 reviutils-1.3.2/reviutils/api/
+-rw-rw-rw-   0        0        0       57 2024-03-27 06:31:11.000000 reviutils-1.3.2/reviutils/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:42:23.753663 reviutils-1.3.2/reviutils/api/amap/
+-rw-rw-rw-   0        0        0     2495 2024-03-27 06:27:05.000000 reviutils-1.3.2/reviutils/api/amap/__init__.py
+-rw-rw-rw-   0        0        0      168 2024-03-27 06:24:54.000000 reviutils-1.3.2/reviutils/api/amap/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:42:23.757663 reviutils-1.3.2/reviutils/audio/
+-rw-rw-rw-   0        0        0      116 2024-03-20 03:20:30.000000 reviutils-1.3.2/reviutils/audio/__init__.py
+-rw-rw-rw-   0        0        0     3232 2024-03-18 03:19:04.000000 reviutils-1.3.2/reviutils/audio/clipper.py
+-rw-rw-rw-   0        0        0     1534 2024-03-20 03:42:36.000000 reviutils-1.3.2/reviutils/audio/reader.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:42:23.758664 reviutils-1.3.2/reviutils/common/
+-rw-rw-rw-   0        0        0     3467 2024-03-15 02:38:48.000000 reviutils-1.3.2/reviutils/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:42:23.761664 reviutils-1.3.2/reviutils/gis/
+-rw-rw-rw-   0        0        0      106 2024-04-11 06:29:44.000000 reviutils-1.3.2/reviutils/gis/__init__.py
+-rw-rw-rw-   0        0        0     6694 2024-04-11 06:29:44.000000 reviutils-1.3.2/reviutils/gis/convertor.py
+-rw-rw-rw-   0        0        0      558 2024-04-11 06:29:44.000000 reviutils-1.3.2/reviutils/gis/main.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:42:23.769665 reviutils-1.3.2/reviutils/noisepollution/
+-rw-rw-rw-   0        0        0      314 2024-03-20 03:21:45.000000 reviutils-1.3.2/reviutils/noisepollution/__init__.py
+-rw-rw-rw-   0        0        0     1994 2024-03-14 08:34:09.000000 reviutils-1.3.2/reviutils/noisepollution/evaluation.py
+-rw-rw-rw-   0        0        0     4114 2024-03-19 08:00:42.000000 reviutils-1.3.2/reviutils/noisepollution/funcarea.py
+-rw-rw-rw-   0        0        0     1043 2024-03-20 03:33:29.000000 reviutils-1.3.2/reviutils/noisepollution/hourhelper.py
+-rw-rw-rw-   0        0        0     7313 2024-03-15 02:38:48.000000 reviutils-1.3.2/reviutils/noisepollution/splhelper.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:42:23.749665 reviutils-1.3.2/reviutils.egg-info/
+-rw-rw-rw-   0        0        0     2814 2024-04-11 07:42:23.000000 reviutils-1.3.2/reviutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      682 2024-04-11 07:42:23.000000 reviutils-1.3.2/reviutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 07:42:23.000000 reviutils-1.3.2/reviutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-27 06:45:03.000000 reviutils-1.3.2/reviutils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       91 2024-04-11 07:42:23.000000 reviutils-1.3.2/reviutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 07:42:23.000000 reviutils-1.3.2/reviutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 07:42:23.771665 reviutils-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1485 2024-04-11 07:39:43.000000 reviutils-1.3.2/setup.py
```

### Comparing `reviutils-1.3.1/LICENSE` & `reviutils-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.1/PKG-INFO` & `reviutils-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviutils
-Version: 1.3.1
+Version: 1.3.2
 Summary: A common library frequently used on python
 Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI
 Author-email: reviy-top@outlook.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: audio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reviutils Version: 1.3.1 Summary: A common library
+Metadata-Version: 2.1 Name: reviutils Version: 1.3.2 Summary: A common library
 frequently used on python Home-page: https://github.com/Viyyy/viutils Author:
 Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
 Description-Content-Type: text/markdown Provides-Extra: audio License-File:
 LICENSE
                             ************ rreevviiuuttiillss ************
                            ä¸ä¸ªå¸¸ç¨çPythonåº
                             _ç_®__ä_½__ä_¸_­_æ__ï½ _E_n_g_l_i_s_h
```

### Comparing `reviutils-1.3.1/README.md` & `reviutils-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.1/reviutils/api/amap/__init__.py` & `reviutils-1.3.2/reviutils/api/amap/__init__.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.1/reviutils/audio/clipper.py` & `reviutils-1.3.2/reviutils/audio/clipper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.1/reviutils/audio/reader.py` & `reviutils-1.3.2/reviutils/audio/reader.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.1/reviutils/common/__init__.py` & `reviutils-1.3.2/reviutils/common/__init__.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.1/reviutils/noisepollution/evaluation.py` & `reviutils-1.3.2/reviutils/noisepollution/evaluation.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.1/reviutils/noisepollution/funcarea.py` & `reviutils-1.3.2/reviutils/noisepollution/funcarea.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.1/reviutils/noisepollution/hourhelper.py` & `reviutils-1.3.2/reviutils/noisepollution/hourhelper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.1/reviutils/noisepollution/splhelper.py` & `reviutils-1.3.2/reviutils/noisepollution/splhelper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.1/reviutils.egg-info/PKG-INFO` & `reviutils-1.3.2/reviutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviutils
-Version: 1.3.1
+Version: 1.3.2
 Summary: A common library frequently used on python
 Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI
 Author-email: reviy-top@outlook.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: audio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reviutils Version: 1.3.1 Summary: A common library
+Metadata-Version: 2.1 Name: reviutils Version: 1.3.2 Summary: A common library
 frequently used on python Home-page: https://github.com/Viyyy/viutils Author:
 Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
 Description-Content-Type: text/markdown Provides-Extra: audio License-File:
 LICENSE
                             ************ rreevviiuuttiillss ************
                            ä¸ä¸ªå¸¸ç¨çPythonåº
                             _ç_®__ä_½__ä_¸_­_æ__ï½ _E_n_g_l_i_s_h
```

### Comparing `reviutils-1.3.1/reviutils.egg-info/SOURCES.txt` & `reviutils-1.3.2/reviutils.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,12 +10,15 @@
 reviutils/api/__init__.py
 reviutils/api/amap/__init__.py
 reviutils/api/amap/enums.py
 reviutils/audio/__init__.py
 reviutils/audio/clipper.py
 reviutils/audio/reader.py
 reviutils/common/__init__.py
+reviutils/gis/__init__.py
+reviutils/gis/convertor.py
+reviutils/gis/main.py
 reviutils/noisepollution/__init__.py
 reviutils/noisepollution/evaluation.py
 reviutils/noisepollution/funcarea.py
 reviutils/noisepollution/hourhelper.py
 reviutils/noisepollution/splhelper.py
```

### Comparing `reviutils-1.3.1/setup.py` & `reviutils-1.3.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,23 +26,23 @@
             else:
                 del_pycache(os.path.join(root, dir))
 
 del_pycache('reviutils') # 删除reviutils下的每个子文件夹的__pycache__文件夹
 
 setup(
     name='reviutils',
-    version='1.3.1',
+    version='1.3.2',
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='A common library frequently used on python',
     url='https://github.com/Viyyy/viutils',
     author='Re.VI',
     author_email='reviy-top@outlook.com',
     license='Apache License 2.0',
-    packages=['reviutils.common','reviutils.noisepollution','reviutils.audio','reviutils.api','reviutils.api.amap'],
+    packages=['reviutils.common','reviutils.noisepollution','reviutils.audio','reviutils.api','reviutils.api.amap','reviutils.gis'],
     install_requires=packages,
     extras_require={
         'audio': ['librosa', 'soundfile','torch', 'torchaudio','pydub','starlette']
     },
     zip_safe=False
 )
```

