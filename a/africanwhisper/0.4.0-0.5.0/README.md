# Comparing `tmp/africanwhisper-0.4.0.tar.gz` & `tmp/africanwhisper-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "africanwhisper-0.4.0.tar", last modified: Wed Apr 10 21:18:50 2024, max compression
+gzip compressed data, was "africanwhisper-0.5.0.tar", last modified: Thu Apr 11 12:32:53 2024, max compression
```

## Comparing `africanwhisper-0.4.0.tar` & `africanwhisper-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:50.054992 africanwhisper-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-04-10 21:18:50.054992 africanwhisper-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 21:18:50.054992 africanwhisper-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:50.046992 africanwhisper-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:50.054992 africanwhisper-0.4.0/src/africanwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-04-10 21:18:50.000000 africanwhisper-0.4.0/src/africanwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 21:18:50.000000 africanwhisper-0.4.0/src/africanwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:18:50.000000 africanwhisper-0.4.0/src/africanwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-10 21:18:50.000000 africanwhisper-0.4.0/src/africanwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 21:18:50.000000 africanwhisper-0.4.0/src/africanwhisper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:50.050992 africanwhisper-0.4.0/src/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/deployment/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/deployment/speech_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:50.050992 africanwhisper-0.4.0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/tests/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:50.054992 africanwhisper-0.4.0/src/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/audio_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/gradio_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/gradio_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/model_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/wandb_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/whisper_model_prep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:53.585253 africanwhisper-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-04-11 12:32:53.585253 africanwhisper-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-11 12:32:53.585253 africanwhisper-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:53.581253 africanwhisper-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:53.585253 africanwhisper-0.5.0/src/africanwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-04-11 12:32:53.000000 africanwhisper-0.5.0/src/africanwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-11 12:32:53.000000 africanwhisper-0.5.0/src/africanwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:32:53.000000 africanwhisper-0.5.0/src/africanwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-11 12:32:53.000000 africanwhisper-0.5.0/src/africanwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 12:32:53.000000 africanwhisper-0.5.0/src/africanwhisper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:53.581253 africanwhisper-0.5.0/src/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/deployment/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/deployment/speech_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:53.581253 africanwhisper-0.5.0/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/tests/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:53.585253 africanwhisper-0.5.0/src/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/audio_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/gradio_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/gradio_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/wandb_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/whisper_model_prep.py
```

### Comparing `africanwhisper-0.4.0/LICENSE` & `africanwhisper-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.4.0/PKG-INFO` & `africanwhisper-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.4.0
+Version: 0.5.0
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -27,15 +27,14 @@
 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
 Requires-Dist: yt-dlp==2023.11.14
 Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: logging==0.4.9.6
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.4.0 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.5.0 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
 jiwer==3.0.3 Requires-Dist: bitsandbytes==0.42.0 Requires-Dist:
 accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: numpy==1.26.4
 Requires-Dist: wandb==0.16.5 Requires-Dist: holoviews==1.18.3 Requires-Dist:
 panel==1.3.8 Requires-Dist: gradio==4.24.0 Requires-Dist: pytube==15.0.0
 Requires-Dist: tf-keras==2.16.0 Requires-Dist: tensorflow==2.16.1 Requires-
 Dist: keras==3.1.1 Requires-Dist: scipy==1.12.0 Requires-Dist: tensorflow-
 probability==0.24.0 Requires-Dist: yt-dlp==2023.11.14 Requires-Dist: python-
-dotenv==1.0.1 Requires-Dist: logging==0.4.9.6
+dotenv==1.0.1
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
 *Enhancing Automatic Speech Recognition (ASR): translation and transcription
 capabilities for African languages by providing seamless fine-tuning and
 deploying pipelines for Whisper Model*.
 ![Diagram](diagram-1.png) ## Features - ð§ Fine-tune the [Whisper](https://
```

### Comparing `africanwhisper-0.4.0/README.md` & `africanwhisper-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.4.0/setup.cfg` & `africanwhisper-0.5.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = africanwhisper
 author = Kevin Kibe
-version = 0.4.0
+version = 0.5.0
 author_email = keviinkibe@gmail.com
 description = A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KevKibe/African-Whisper
 license = MIT
 
@@ -31,15 +31,14 @@
 	tf-keras==2.16.0
 	tensorflow==2.16.1
 	keras==3.1.1
 	scipy==1.12.0
 	tensorflow-probability==0.24.0
 	yt-dlp==2023.11.14
 	python-dotenv==1.0.1
-	logging==0.4.9.6
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `africanwhisper-0.4.0/src/africanwhisper.egg-info/PKG-INFO` & `africanwhisper-0.5.0/src/africanwhisper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.4.0
+Version: 0.5.0
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -27,15 +27,14 @@
 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
 Requires-Dist: yt-dlp==2023.11.14
 Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: logging==0.4.9.6
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.4.0 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.5.0 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
 jiwer==3.0.3 Requires-Dist: bitsandbytes==0.42.0 Requires-Dist:
 accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: numpy==1.26.4
 Requires-Dist: wandb==0.16.5 Requires-Dist: holoviews==1.18.3 Requires-Dist:
 panel==1.3.8 Requires-Dist: gradio==4.24.0 Requires-Dist: pytube==15.0.0
 Requires-Dist: tf-keras==2.16.0 Requires-Dist: tensorflow==2.16.1 Requires-
 Dist: keras==3.1.1 Requires-Dist: scipy==1.12.0 Requires-Dist: tensorflow-
 probability==0.24.0 Requires-Dist: yt-dlp==2023.11.14 Requires-Dist: python-
-dotenv==1.0.1 Requires-Dist: logging==0.4.9.6
+dotenv==1.0.1
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
 *Enhancing Automatic Speech Recognition (ASR): translation and transcription
 capabilities for African languages by providing seamless fine-tuning and
 deploying pipelines for Whisper Model*.
 ![Diagram](diagram-1.png) ## Features - ð§ Fine-tune the [Whisper](https://
```

### Comparing `africanwhisper-0.4.0/src/africanwhisper.egg-info/SOURCES.txt` & `africanwhisper-0.5.0/src/africanwhisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.4.0/src/deployment/main.py` & `africanwhisper-0.5.0/src/deployment/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.4.0/src/deployment/speech_inference.py` & `africanwhisper-0.5.0/src/deployment/speech_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.4.0/src/tests/test_dataset.py` & `africanwhisper-0.5.0/src/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.4.0/src/training/audio_data_processor.py` & `africanwhisper-0.5.0/src/training/audio_data_processor.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.4.0/src/training/collator.py` & `africanwhisper-0.5.0/src/training/collator.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.4.0/src/training/data_prep.py` & `africanwhisper-0.5.0/src/training/data_prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         self.dataset_name = dataset_name
         self.language_abbr = language_abbr
         self.model_id = model_id
         self.processing_task = processing_task
         self.use_peft = use_peft
         self.model_prep = WhisperModelPrep(
             self.model_id,
-            self.language_abbr,
             self.processing_task,
             self.use_peft,
         )
         self.data_loader = Dataset(
             self.huggingface_read_token, self.dataset_name, self.language_abbr
         )
```

### Comparing `africanwhisper-0.4.0/src/training/evaluation.py` & `africanwhisper-0.5.0/src/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.4.0/src/training/gradio_demo.py` & `africanwhisper-0.5.0/src/training/gradio_demo.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.4.0/src/training/gradio_inference.py` & `africanwhisper-0.5.0/src/training/gradio_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.4.0/src/training/load_data.py` & `africanwhisper-0.5.0/src/training/load_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datasets import load_dataset, DatasetDict, IterableDataset
+from datasets import load_dataset, IterableDataset, concatenate_datasets
 import warnings
 from typing import List
 
 warnings.filterwarnings("ignore")
 
 class Dataset:
     """
@@ -22,35 +22,35 @@
             huggingface_token (str): Hugging Face API token.
             dataset_name (str): Name of the dataset.
             language_abbr (str): Language abbreviation for the dataset.
         """
         self.huggingface_token = huggingface_token
         self.dataset_name = dataset_name
         self.language_abbr = language_abbr
-
-
-    def load_dataset(self) -> DatasetDict:
-        """
-        Load the streaming dataset.
-
-        Args:
-            split (Optional[str]): The dataset split to load. Defaults to 'train'.
-            **kwargs: Additional keyword arguments.
+    
+    def load_dataset(self):
+        """Load datasets for each language abbreviation and concatenate train/test splits.
 
         Returns:
-            DatasetDict: The loaded streaming dataset.
+            dict: A dictionary containing concatenated train and test splits for each language.
         """
-        dataset = DatasetDict()
-        dataset['test'] = load_dataset(self.dataset_name, self.language_abbr, split="test", 
-                                            token=self.huggingface_token, streaming=True, 
-                                            trust_remote_code=True)
-        dataset['train'] = load_dataset(self.dataset_name, self.language_abbr, split="train", 
-                                            token=self.huggingface_token, streaming=True, 
-                                            trust_remote_code=True)
-        return dataset
+        data = {}
+        for lang in self.language_abbr:
+            dataset = load_dataset(self.dataset_name, lang, streaming=True, token=self.huggingface_token, trust_remote_code=True, disable_progress_bar=True, disable_metadata=True)
+            train_split = dataset['train']
+            test_split = dataset['test']
+            if "train" in data:
+                data["train"] = concatenate_datasets([data["train"], train_split])
+            else:
+                data["train"] = train_split
+            if "test" in data:
+                data["test"] = concatenate_datasets([data["test"], test_split])
+            else:
+                data["test"] = test_split
+        return data
         
     def count_examples(self, dataset: IterableDataset) -> int:
         """
         Count the number of examples in the dataset.
 
         Args:
             dataset (IterableDataset): The dataset to count examples from.
```

### Comparing `africanwhisper-0.4.0/src/training/main.py` & `africanwhisper-0.5.0/src/training/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,17 +25,17 @@
         "--dataset_name",
         type=str,
         default="mozilla-foundation/common_voice_16_1",
         help="Name of the dataset to be downloaded from Hugging Face.",
     )
     parser.add_argument(
         "--language_abbr",
-        type=str,
-        default="sw",
-        help="Abbreviation of the language for the dataset.",
+        nargs='+',  
+        required=True,
+        help="Abbreviation(s) of the language(s) for the dataset.",
     )
     parser.add_argument(
         "--model_id",
         type=str,
         default="openai/whisper-small",
         help="Model ID for the model to be used in training.",
     )
@@ -76,12 +76,11 @@
         huggingface_write_token=args.huggingface_write_token,
         model_id=args.model_id,
         dataset=dataset,
         model=model,
         feature_processor=feature_processor,
         feature_extractor=feature_extractor,
         tokenizer=tokenizer,
-        language_abbr=args.language_abbr,
         wandb_api_key=args.wandb_api_key,
         use_peft=args.use_peft,
     )
     trainer.train()
```

### Comparing `africanwhisper-0.4.0/src/training/model_trainer.py` & `africanwhisper-0.5.0/src/training/model_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         huggingface_write_token: str,
         model_id: str,
         dataset: DatasetDict,
         model: str,
         feature_processor,
         feature_extractor,
         tokenizer,
-        language_abbr: str,
         wandb_api_key: str,
         use_peft: bool,
     ):
         """
         Initializes the Trainer with the necessary components and configurations for training.
 
         Parameters:
@@ -59,16 +58,20 @@
         self.dataset = dataset
         self.model = model
         self.model_id = model_id
         self.tokenizer = tokenizer
         self.feature_processor = feature_processor
         self.feature_extractor = feature_extractor
         self.huggingface_write_token = huggingface_write_token
-        self.language_abbr = language_abbr
         self.use_peft = use_peft
+        self.model_prep = WhisperModelPrep(
+            self.model_id, 
+            "transcribe", 
+            self.use_peft
+        )
 
     def compute_metrics(self, pred) -> dict:
         """
         Computes the Word Error Rate (WER) metric for the model predictions.
 
         Parameters:
             pred (PredictionOutput): The output from the model's prediction.
@@ -100,18 +103,15 @@
         Returns:
             dict: A dictionary containing computed spectrogram data.
 
         Raises:
             KeyError: If the input example does not contain the required keys.
         """
         waveform = example["audio"]["array"]
-        model_prep = WhisperModelPrep(
-            self.model_id, self.language_abbr, "transcribe", self.use_peft
-        )
-        feature_extractor = model_prep.initialize_feature_extractor()
+        feature_extractor = self.model_prep.initialize_feature_extractor()
         specs = feature_extractor(
             waveform, sampling_rate=16000, padding="do_not_pad"
         ).input_features[0]
         return {"spectrogram": specs}
 
     def train(self,
           max_steps: int = 100,
@@ -125,25 +125,21 @@
         Args:
             max_steps (int, optional): Maximum number of training steps. Defaults to 100.
             learning_rate (float, optional): Learning rate for training. Defaults to 1e-5.
             per_device_train_batch_size (int, optional): Batch size per GPU for training. Defaults to 96.
             per_device_eval_batch_size (int, optional): Batch size per GPU for evaluation. Defaults to 64.
             optim (str, optional): Optimizer to use for training. Defaults to "adamw_bnb_8bit".
         """
-        # Checks if GPU is available
-        use_gpu = torch.cuda.is_available()
-
-        # Set fp16 to True/False based on GPU availability
-        fp16 = use_gpu
-
+        # Checks if GPU is available: returns Boolean
+        fp16 = torch.cuda.is_available()
         data_collator = DataCollatorSpeechSeq2SeqWithPadding(
             processor=self.feature_processor
         )
         training_args = Seq2SeqTrainingArguments(
-            output_dir=f"../{self.model_id}-{self.language_abbr}",
+            output_dir=f"../{self.model_id}-finetuned",
             per_device_train_batch_size=per_device_train_batch_size,
             gradient_accumulation_steps=1,
             learning_rate=learning_rate,
             max_steps=max_steps,
             gradient_checkpointing=True,
             fp16=fp16,
             optim=optim,
@@ -172,21 +168,16 @@
             train_dataset=self.dataset["train"],
             eval_dataset=eval_dataset,
             data_collator=data_collator,
             compute_metrics=self.compute_metrics,
             tokenizer=self.feature_processor.feature_extractor,
             callbacks=[ShuffleCallback()],
         )
-
-        model_prep = WhisperModelPrep(
-            self.model_id, self.language_abbr, "transcribe", self.use_peft
-        )
-
-        tokenizer = model_prep.initialize_tokenizer()
-        processor = model_prep.initialize_processor()
+        tokenizer = self.model_prep.initialize_tokenizer()
+        processor = self.model_prep.initialize_processor()
         tokenizer.save_pretrained(training_args.output_dir)
         processor.save_pretrained(training_args.output_dir)
         torch.save(self.model.state_dict(), f"{training_args.output_dir}/pytorch_model.bin")
         self.model.save_pretrained(training_args.output_dir)
         progress_callback = WandbProgressResultsCallback(
             trainer, eval_dataset, tokenizer
         )
```

### Comparing `africanwhisper-0.4.0/src/training/wandb_callback.py` & `africanwhisper-0.5.0/src/training/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.4.0/src/training/whisper_model_prep.py` & `africanwhisper-0.5.0/src/training/whisper_model_prep.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,30 +18,30 @@
         processing_task (str): Specific task for the Whisper model to execute.
 
     """
 
     def __init__(
         self,
         model_id: str,
-        language_abbr: str,
+        # language_abbr: str,
         processing_task: str,
         use_peft: bool,
     ):
         """Sets up the dataset and configuration for processing with the Whisper model.
 
         Parameters
         ----------
             dataset (DatasetDict): The dataset to be prepared.
             model_id (str, optional): Whisper model identifier.
             language_code (str, optional): Dataset language ISO code.
             processing_task (str, optional): Task for the Whisper model.
 
         """
         self.model_id = model_id
-        self.language_abbr = language_abbr
+        # self.language_abbr = language_abbr
         self.processing_task = processing_task
         self.use_peft = use_peft
 
     def initialize_feature_extractor(self) -> WhisperFeatureExtractor:
         """Creates and retrieves a feature extractor based on the Whisper model.
 
         Returns
@@ -71,15 +71,15 @@
 
         Returns
         -------
             WhisperProcessor: Unified processor for the model.
 
         """
         return WhisperProcessor.from_pretrained(
-            self.model_id, self.language_abbr, self.processing_task
+            self.model_id, self.processing_task
         )
 
     def initialize_model(self) -> WhisperForConditionalGeneration:
         """Initializes and retrieves the Whisper model configured for conditional generation.
 
         This method sets up the Whisper model with specific configurations, ensuring it is
         ready for use in tasks such as transcription or translation, depending on the
@@ -90,15 +90,14 @@
             WhisperForConditionalGeneration: The configured Whisper model ready for conditional generation tasks.
 
         """
 
         if self.use_peft:
             model = WhisperForConditionalGeneration.from_pretrained(
                 self.model_id,
-                # cache_dir="./whisper-model/model",
                 load_in_8bit=True,
                 device_map="auto",
             )
             model.config.forced_decoder_ids = None
             model.config.suppress_tokens = []
             model.generation_config.language = "en"
             model.generation_config.task = "translate"
```

