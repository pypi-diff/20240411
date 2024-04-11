# Comparing `tmp/gbx-lm-0.1.3.tar.gz` & `tmp/gbx-lm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbx-lm-0.1.3.tar", last modified: Tue Apr  9 09:45:23 2024, max compression
+gzip compressed data, was "gbx-lm-0.1.4.tar", last modified: Thu Apr 11 19:08:09 2024, max compression
```

## Comparing `gbx-lm-0.1.3.tar` & `gbx-lm-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-09 09:45:23.484698 gbx-lm-0.1.3/
--rw-r--r--   0 haojin     (501) staff       (20)    11357 2024-03-18 14:26:20.000000 gbx-lm-0.1.3/LICENSE
--rw-r--r--   0 haojin     (501) staff       (20)     4237 2024-04-09 09:45:23.484470 gbx-lm-0.1.3/PKG-INFO
--rw-r--r--   0 haojin     (501) staff       (20)     3734 2024-04-08 20:17:24.000000 gbx-lm-0.1.3/README.md
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-09 09:45:23.481659 gbx-lm-0.1.3/gbx_lm/
--rw-r--r--   0 haojin     (501) staff       (20)       66 2024-03-19 13:52:13.000000 gbx-lm-0.1.3/gbx_lm/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)    12369 2024-04-08 20:13:35.000000 gbx-lm-0.1.3/gbx_lm/gba2mlx.py
--rw-r--r--   0 haojin     (501) staff       (20)     4158 2024-04-09 06:52:36.000000 gbx-lm-0.1.3/gbx_lm/generate.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-09 09:45:23.483980 gbx-lm-0.1.3/gbx_lm/models/
--rw-r--r--   0 haojin     (501) staff       (20)        0 2024-03-05 09:34:30.000000 gbx-lm-0.1.3/gbx_lm/models/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)      314 2024-01-13 21:15:10.000000 gbx-lm-0.1.3/gbx_lm/models/base.py
--rw-r--r--   0 haojin     (501) staff       (20)     5639 2024-04-08 11:50:53.000000 gbx-lm-0.1.3/gbx_lm/models/qgemma.py
--rw-r--r--   0 haojin     (501) staff       (20)     7114 2024-04-08 15:08:09.000000 gbx-lm-0.1.3/gbx_lm/models/qllama.py
--rw-r--r--   0 haojin     (501) staff       (20)     8289 2024-04-08 12:11:47.000000 gbx-lm-0.1.3/gbx_lm/models/qmixtral.py
--rw-r--r--   0 haojin     (501) staff       (20)     6614 2024-04-08 15:40:16.000000 gbx-lm-0.1.3/gbx_lm/models/qqwen2.py
--rw-r--r--   0 haojin     (501) staff       (20)    10690 2024-04-02 17:49:04.000000 gbx-lm-0.1.3/gbx_lm/models/quantized_linear_gba.py
--rw-r--r--   0 haojin     (501) staff       (20)    17365 2024-04-09 06:50:01.000000 gbx-lm-0.1.3/gbx_lm/utils.py
--rw-r--r--   0 haojin     (501) staff       (20)       21 2024-04-09 09:42:49.000000 gbx-lm-0.1.3/gbx_lm/version.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-09 09:45:23.482227 gbx-lm-0.1.3/gbx_lm.egg-info/
--rw-r--r--   0 haojin     (501) staff       (20)     4237 2024-04-09 09:45:23.000000 gbx-lm-0.1.3/gbx_lm.egg-info/PKG-INFO
--rw-r--r--   0 haojin     (501) staff       (20)      449 2024-04-09 09:45:23.000000 gbx-lm-0.1.3/gbx_lm.egg-info/SOURCES.txt
--rw-r--r--   0 haojin     (501) staff       (20)        1 2024-04-09 09:45:23.000000 gbx-lm-0.1.3/gbx_lm.egg-info/dependency_links.txt
--rw-r--r--   0 haojin     (501) staff       (20)       88 2024-04-09 09:45:23.000000 gbx-lm-0.1.3/gbx_lm.egg-info/requires.txt
--rw-r--r--   0 haojin     (501) staff       (20)        7 2024-04-09 09:45:23.000000 gbx-lm-0.1.3/gbx_lm.egg-info/top_level.txt
--rw-r--r--   0 haojin     (501) staff       (20)       38 2024-04-09 09:45:23.484750 gbx-lm-0.1.3/setup.cfg
--rw-r--r--   0 haojin     (501) staff       (20)      800 2024-04-08 19:53:50.000000 gbx-lm-0.1.3/setup.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-11 19:08:09.572291 gbx-lm-0.1.4/
+-rw-r--r--   0 haojin     (501) staff       (20)    11357 2024-03-18 14:26:20.000000 gbx-lm-0.1.4/LICENSE
+-rw-r--r--   0 haojin     (501) staff       (20)     4237 2024-04-11 19:08:09.572076 gbx-lm-0.1.4/PKG-INFO
+-rw-r--r--   0 haojin     (501) staff       (20)     3734 2024-04-11 18:29:58.000000 gbx-lm-0.1.4/README.md
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-11 19:08:09.570091 gbx-lm-0.1.4/gbx_lm/
+-rw-r--r--   0 haojin     (501) staff       (20)       81 2024-04-10 08:41:13.000000 gbx-lm-0.1.4/gbx_lm/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)    12369 2024-04-08 20:13:35.000000 gbx-lm-0.1.4/gbx_lm/gba2mlx.py
+-rw-r--r--   0 haojin     (501) staff       (20)     4158 2024-04-09 06:52:36.000000 gbx-lm-0.1.4/gbx_lm/generate.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-11 19:08:09.571572 gbx-lm-0.1.4/gbx_lm/models/
+-rw-r--r--   0 haojin     (501) staff       (20)        0 2024-03-05 09:34:30.000000 gbx-lm-0.1.4/gbx_lm/models/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)      314 2024-01-13 21:15:10.000000 gbx-lm-0.1.4/gbx_lm/models/base.py
+-rw-r--r--   0 haojin     (501) staff       (20)     5639 2024-04-08 11:50:53.000000 gbx-lm-0.1.4/gbx_lm/models/qgemma.py
+-rw-r--r--   0 haojin     (501) staff       (20)     7114 2024-04-08 15:08:09.000000 gbx-lm-0.1.4/gbx_lm/models/qllama.py
+-rw-r--r--   0 haojin     (501) staff       (20)     8289 2024-04-08 12:11:47.000000 gbx-lm-0.1.4/gbx_lm/models/qmixtral.py
+-rw-r--r--   0 haojin     (501) staff       (20)     6614 2024-04-08 15:40:16.000000 gbx-lm-0.1.4/gbx_lm/models/qqwen2.py
+-rw-r--r--   0 haojin     (501) staff       (20)    10690 2024-04-02 17:49:04.000000 gbx-lm-0.1.4/gbx_lm/models/quantized_linear_gba.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-11 19:08:09.571791 gbx-lm-0.1.4/gbx_lm/serve/
+-rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-11 18:36:08.000000 gbx-lm-0.1.4/gbx_lm/serve/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)     9383 2024-04-11 14:56:32.000000 gbx-lm-0.1.4/gbx_lm/serve/mlx_fastchat_worker.py
+-rw-r--r--   0 haojin     (501) staff       (20)    17365 2024-04-09 06:50:01.000000 gbx-lm-0.1.4/gbx_lm/utils.py
+-rw-r--r--   0 haojin     (501) staff       (20)       21 2024-04-11 19:08:03.000000 gbx-lm-0.1.4/gbx_lm/version.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-11 19:08:09.570713 gbx-lm-0.1.4/gbx_lm.egg-info/
+-rw-r--r--   0 haojin     (501) staff       (20)     4237 2024-04-11 19:08:09.000000 gbx-lm-0.1.4/gbx_lm.egg-info/PKG-INFO
+-rw-r--r--   0 haojin     (501) staff       (20)      510 2024-04-11 19:08:09.000000 gbx-lm-0.1.4/gbx_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 haojin     (501) staff       (20)        1 2024-04-11 19:08:09.000000 gbx-lm-0.1.4/gbx_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 haojin     (501) staff       (20)       88 2024-04-11 19:08:09.000000 gbx-lm-0.1.4/gbx_lm.egg-info/requires.txt
+-rw-r--r--   0 haojin     (501) staff       (20)        7 2024-04-11 19:08:09.000000 gbx-lm-0.1.4/gbx_lm.egg-info/top_level.txt
+-rw-r--r--   0 haojin     (501) staff       (20)       38 2024-04-11 19:08:09.572335 gbx-lm-0.1.4/setup.cfg
+-rw-r--r--   0 haojin     (501) staff       (20)      816 2024-04-11 19:04:43.000000 gbx-lm-0.1.4/setup.py
```

### Comparing `gbx-lm-0.1.3/LICENSE` & `gbx-lm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.3/PKG-INFO` & `gbx-lm-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbx-lm
-Version: 0.1.3
+Version: 0.1.4
 Summary: GBA Model Toolkit for MLX
 Home-page: https://github.com/GreenBitAI/gbx-lm
 Author: GreenBitAI and MLX Contributors
 Author-email: team@greenbit.ai
 License: Apache-2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `gbx-lm-0.1.3/README.md` & `gbx-lm-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.3/gbx_lm/gba2mlx.py` & `gbx-lm-0.1.4/gbx_lm/gba2mlx.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.3/gbx_lm/generate.py` & `gbx-lm-0.1.4/gbx_lm/generate.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.3/gbx_lm/models/qgemma.py` & `gbx-lm-0.1.4/gbx_lm/models/qgemma.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.3/gbx_lm/models/qllama.py` & `gbx-lm-0.1.4/gbx_lm/models/qllama.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.3/gbx_lm/models/qmixtral.py` & `gbx-lm-0.1.4/gbx_lm/models/qmixtral.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.3/gbx_lm/models/qqwen2.py` & `gbx-lm-0.1.4/gbx_lm/models/qqwen2.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.3/gbx_lm/models/quantized_linear_gba.py` & `gbx-lm-0.1.4/gbx_lm/models/quantized_linear_gba.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.3/gbx_lm/utils.py` & `gbx-lm-0.1.4/gbx_lm/utils.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.3/gbx_lm.egg-info/PKG-INFO` & `gbx-lm-0.1.4/gbx_lm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbx-lm
-Version: 0.1.3
+Version: 0.1.4
 Summary: GBA Model Toolkit for MLX
 Home-page: https://github.com/GreenBitAI/gbx-lm
 Author: GreenBitAI and MLX Contributors
 Author-email: team@greenbit.ai
 License: Apache-2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `gbx-lm-0.1.3/setup.py` & `gbx-lm-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,10 +18,10 @@
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email="team@greenbit.ai",
     author="GreenBitAI and MLX Contributors",
     url="https://github.com/GreenBitAI/gbx-lm",
     license="Apache-2.0",
     install_requires=requirements,
-    packages=["gbx_lm", "gbx_lm.models"],
+    packages=["gbx_lm", "gbx_lm.models", "gbx_lm.serve"],
     python_requires=">=3.9",
 )
```

