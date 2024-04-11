# Comparing `tmp/signapse-1.0.12.tar.gz` & `tmp/signapse-1.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signapse-1.0.12.tar", last modified: Tue Apr  9 17:27:11 2024, max compression
+gzip compressed data, was "signapse-1.0.13.tar", last modified: Thu Apr 11 11:38:47 2024, max compression
```

## Comparing `signapse-1.0.12.tar` & `signapse-1.0.13.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-09 17:27:11.034730 signapse-1.0.12/
--rw-r--r--   0 basheer   (1000) basheer   (1000)     2755 2024-04-09 17:27:11.034730 signapse-1.0.12/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1637 2024-04-05 09:17:43.000000 signapse-1.0.12/README.md
--rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-09 17:27:11.034730 signapse-1.0.12/setup.cfg
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1337 2024-04-09 17:26:30.000000 signapse-1.0.12/setup.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-09 17:27:11.034730 signapse-1.0.12/signapse/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      463 2024-04-04 11:18:15.000000 signapse-1.0.12/signapse/__init__.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     6566 2024-04-09 10:40:55.000000 signapse-1.0.12/signapse/build_opt.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     9366 2024-04-08 14:49:55.000000 signapse-1.0.12/signapse/compute.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.12/signapse/constants.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     7511 2024-04-08 15:02:14.000000 signapse-1.0.12/signapse/create.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.12/signapse/create_model.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    21879 2024-04-08 10:17:01.000000 signapse-1.0.12/signapse/heatmaps.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.12/signapse/lang_sam.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4444 2024-04-08 10:09:21.000000 signapse-1.0.12/signapse/lang_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.12/signapse/models_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3888 2024-04-04 14:23:34.000000 signapse-1.0.12/signapse/mp_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     5793 2024-04-09 10:56:58.000000 signapse-1.0.12/signapse/poses.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3403 2024-04-09 10:57:12.000000 signapse-1.0.12/signapse/preprocessing.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.12/signapse/utils.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-09 17:27:11.034730 signapse-1.0.12/signapse.egg-info/
--rw-r--r--   0 basheer   (1000) basheer   (1000)     2755 2024-04-09 17:27:10.000000 signapse-1.0.12/signapse.egg-info/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      479 2024-04-09 17:27:11.000000 signapse-1.0.12/signapse.egg-info/SOURCES.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-09 17:27:10.000000 signapse-1.0.12/signapse.egg-info/dependency_links.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      312 2024-04-09 17:27:10.000000 signapse-1.0.12/signapse.egg-info/requires.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-09 17:27:10.000000 signapse-1.0.12/signapse.egg-info/top_level.txt
+drwxr-xr-x   0     1001     1001        0 2024-04-11 11:38:47.000000 signapse-1.0.13/
+-rw-rw-r--   0     1001     1001     1065 2024-04-04 10:20:56.000000 signapse-1.0.13/LICENSE.txt
+-rw-r--r--   0     1001     1001     2769 2024-04-11 11:38:47.000000 signapse-1.0.13/PKG-INFO
+-rw-rw-r--   0     1001     1001     1637 2024-04-05 09:17:43.000000 signapse-1.0.13/README.md
+-rw-r--r--   0     1001     1001       38 2024-04-11 11:38:47.000000 signapse-1.0.13/setup.cfg
+-rw-rw-r--   0     1001     1001     1395 2024-04-11 11:37:03.000000 signapse-1.0.13/setup.py
+drwxr-xr-x   0     1001     1001        0 2024-04-11 11:38:46.000000 signapse-1.0.13/signapse/
+-rw-rw-r--   0     1001     1001      463 2024-04-04 11:18:15.000000 signapse-1.0.13/signapse/__init__.py
+-rw-rw-r--   0     1001     1001     6566 2024-04-09 10:40:55.000000 signapse-1.0.13/signapse/build_opt.py
+-rw-rw-r--   0     1001     1001     9366 2024-04-08 14:49:55.000000 signapse-1.0.13/signapse/compute.py
+-rw-rw-r--   0     1001     1001     2662 2024-04-04 10:51:14.000000 signapse-1.0.13/signapse/constants.py
+-rw-rw-r--   0     1001     1001     7511 2024-04-08 15:02:14.000000 signapse-1.0.13/signapse/create.py
+-rw-rw-r--   0     1001     1001     1225 2024-04-04 11:11:01.000000 signapse-1.0.13/signapse/create_model.py
+-rw-rw-r--   0     1001     1001    21879 2024-04-08 10:17:01.000000 signapse-1.0.13/signapse/heatmaps.py
+-rw-rw-r--   0     1001     1001     4652 2023-12-03 23:04:06.000000 signapse-1.0.13/signapse/lang_sam.py
+-rw-rw-r--   0     1001     1001     4444 2024-04-08 10:09:21.000000 signapse-1.0.13/signapse/lang_utils.py
+-rw-rw-r--   0     1001     1001    17696 2023-12-03 23:04:06.000000 signapse-1.0.13/signapse/models_utils.py
+-rw-rw-r--   0     1001     1001     3888 2024-04-04 14:23:34.000000 signapse-1.0.13/signapse/mp_utils.py
+-rw-rw-r--   0     1001     1001     5793 2024-04-09 10:56:58.000000 signapse-1.0.13/signapse/poses.py
+-rw-rw-r--   0     1001     1001     3403 2024-04-09 10:57:12.000000 signapse-1.0.13/signapse/preprocessing.py
+-rw-rw-r--   0     1001     1001     2610 2023-12-03 23:04:06.000000 signapse-1.0.13/signapse/utils.py
+drwxr-xr-x   0     1001     1001        0 2024-04-11 11:38:46.000000 signapse-1.0.13/signapse.egg-info/
+-rw-r--r--   0     1001     1001     2769 2024-04-11 11:38:42.000000 signapse-1.0.13/signapse.egg-info/PKG-INFO
+-rw-r--r--   0     1001     1001      491 2024-04-11 11:38:42.000000 signapse-1.0.13/signapse.egg-info/SOURCES.txt
+-rw-r--r--   0     1001     1001        1 2024-04-11 11:38:42.000000 signapse-1.0.13/signapse.egg-info/dependency_links.txt
+-rw-r--r--   0     1001     1001      300 2024-04-11 11:38:42.000000 signapse-1.0.13/signapse.egg-info/requires.txt
+-rw-r--r--   0     1001     1001        9 2024-04-11 11:38:42.000000 signapse-1.0.13/signapse.egg-info/top_level.txt
```

### Comparing `signapse-1.0.12/PKG-INFO` & `signapse-1.0.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: signapse
-Version: 1.0.12
+Version: 1.0.13
 Summary: Signapse_synthetic_signer
 Home-page: https://github.com/signapse/signapse
 Author: Basheer Alwaely
 Author-email: basheer@signapse.ai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Requires-Dist: essentials
 Requires-Dist: setuptools
 Requires-Dist: wheel==0.38.4
 Requires-Dist: mediapipe==0.10.3
 Requires-Dist: opencv-python==4.7.0.72
 Requires-Dist: opencv-python-headless==4.7.0.72
 Requires-Dist: pandas==2.0.3
 Requires-Dist: pickle5==0.0.11
 Requires-Dist: protobuf==3.20.*
 Requires-Dist: boto3==1.24.47
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: scipy==1.8
 Requires-Dist: pycpd==2.0.0
-Requires-Dist: torch==1.11.0+cu113
-Requires-Dist: torchvision==0.12.0+cu113
+Requires-Dist: torch==1.11.0
+Requires-Dist: torchvision==0.12.0
 Requires-Dist: torchaudio==0.11.0
 Requires-Dist: Pillow==9.3.0
 Requires-Dist: imageio
 Requires-Dist: PyYAML
 
 # Signapse synthetic signer
 ![Signapse](https://static.wixstatic.com/media/45e73d_8ab2ecfdee064f20860fe2a1e3f8ddb2~mv2.png/v1/fill/w_132,h_35,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/Blank%202000%20x%202000%20-%202022-04-03T185113_234.png)
```

### Comparing `signapse-1.0.12/README.md` & `signapse-1.0.13/README.md`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/setup.py` & `signapse-1.0.13/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as ofile:
     long_description_file = ofile.read()
     
 setup(
     name='signapse',
-    version='1.0.12',
+    version='1.0.13',
     description='Signapse_synthetic_signer',
     long_description=long_description_file,
     long_description_content_type="text/markdown",
     author='Basheer Alwaely',
     author_email='basheer@signapse.ai',
     url='https://github.com/signapse/signapse',
     packages=find_packages(),
@@ -31,15 +31,17 @@
         'pandas==2.0.3',
         'pickle5==0.0.11',
         'protobuf==3.20.*',
         'boto3 == 1.24.47',
         'ffmpeg-python == 0.2.0',
         'scipy == 1.8,',
         'pycpd==2.0.0',
-        'torch==1.11.0+cu113',
-        'torchvision==0.12.0+cu113',
+    #    'torch==1.11.0+cu113',
+    #    'torchvision==0.12.0+cu113',
+        'torch==1.11.0',
+        'torchvision==0.12.0',
         'torchaudio==0.11.0',
         'Pillow==9.3.0',
         'imageio',
         'PyYAML',
     ]
 )
```

### Comparing `signapse-1.0.12/signapse/build_opt.py` & `signapse-1.0.13/signapse/build_opt.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/signapse/compute.py` & `signapse-1.0.13/signapse/compute.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/signapse/constants.py` & `signapse-1.0.13/signapse/constants.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/signapse/create.py` & `signapse-1.0.13/signapse/create.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/signapse/create_model.py` & `signapse-1.0.13/signapse/create_model.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/signapse/heatmaps.py` & `signapse-1.0.13/signapse/heatmaps.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/signapse/lang_sam.py` & `signapse-1.0.13/signapse/lang_sam.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/signapse/lang_utils.py` & `signapse-1.0.13/signapse/lang_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/signapse/models_utils.py` & `signapse-1.0.13/signapse/models_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/signapse/mp_utils.py` & `signapse-1.0.13/signapse/mp_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/signapse/poses.py` & `signapse-1.0.13/signapse/poses.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/signapse/preprocessing.py` & `signapse-1.0.13/signapse/preprocessing.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/signapse/utils.py` & `signapse-1.0.13/signapse/utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.12/signapse.egg-info/PKG-INFO` & `signapse-1.0.13/signapse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: signapse
-Version: 1.0.12
+Version: 1.0.13
 Summary: Signapse_synthetic_signer
 Home-page: https://github.com/signapse/signapse
 Author: Basheer Alwaely
 Author-email: basheer@signapse.ai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Requires-Dist: essentials
 Requires-Dist: setuptools
 Requires-Dist: wheel==0.38.4
 Requires-Dist: mediapipe==0.10.3
 Requires-Dist: opencv-python==4.7.0.72
 Requires-Dist: opencv-python-headless==4.7.0.72
 Requires-Dist: pandas==2.0.3
 Requires-Dist: pickle5==0.0.11
 Requires-Dist: protobuf==3.20.*
 Requires-Dist: boto3==1.24.47
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: scipy==1.8
 Requires-Dist: pycpd==2.0.0
-Requires-Dist: torch==1.11.0+cu113
-Requires-Dist: torchvision==0.12.0+cu113
+Requires-Dist: torch==1.11.0
+Requires-Dist: torchvision==0.12.0
 Requires-Dist: torchaudio==0.11.0
 Requires-Dist: Pillow==9.3.0
 Requires-Dist: imageio
 Requires-Dist: PyYAML
 
 # Signapse synthetic signer
 ![Signapse](https://static.wixstatic.com/media/45e73d_8ab2ecfdee064f20860fe2a1e3f8ddb2~mv2.png/v1/fill/w_132,h_35,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/Blank%202000%20x%202000%20-%202022-04-03T185113_234.png)
```

