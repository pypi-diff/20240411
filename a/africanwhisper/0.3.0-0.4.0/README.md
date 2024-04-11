# Comparing `tmp/africanwhisper-0.3.0.tar.gz` & `tmp/africanwhisper-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "africanwhisper-0.3.0.tar", last modified: Thu Apr  4 21:02:06 2024, max compression
+gzip compressed data, was "africanwhisper-0.4.0.tar", last modified: Wed Apr 10 21:18:50 2024, max compression
```

## Comparing `africanwhisper-0.3.0.tar` & `africanwhisper-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:06.356149 africanwhisper-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-04-04 21:02:06.356149 africanwhisper-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-04 21:02:06.356149 africanwhisper-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:06.352149 africanwhisper-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:06.356149 africanwhisper-0.3.0/src/africanwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-04-04 21:02:06.000000 africanwhisper-0.3.0/src/africanwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-04 21:02:06.000000 africanwhisper-0.3.0/src/africanwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:02:06.000000 africanwhisper-0.3.0/src/africanwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-04 21:02:06.000000 africanwhisper-0.3.0/src/africanwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 21:02:06.000000 africanwhisper-0.3.0/src/africanwhisper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:06.352149 africanwhisper-0.3.0/src/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/deployment/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/deployment/speech_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:06.352149 africanwhisper-0.3.0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/tests/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:06.356149 africanwhisper-0.3.0/src/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/training/audio_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/training/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/training/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/training/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/training/gradio_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/training/gradio_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/training/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/training/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/training/model_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/training/wandb_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-04 21:02:02.000000 africanwhisper-0.3.0/src/training/whisper_model_prep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:50.054992 africanwhisper-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-04-10 21:18:50.054992 africanwhisper-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 21:18:50.054992 africanwhisper-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:50.046992 africanwhisper-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:50.054992 africanwhisper-0.4.0/src/africanwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-04-10 21:18:50.000000 africanwhisper-0.4.0/src/africanwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 21:18:50.000000 africanwhisper-0.4.0/src/africanwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:18:50.000000 africanwhisper-0.4.0/src/africanwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-10 21:18:50.000000 africanwhisper-0.4.0/src/africanwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 21:18:50.000000 africanwhisper-0.4.0/src/africanwhisper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:50.050992 africanwhisper-0.4.0/src/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/deployment/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/deployment/speech_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:50.050992 africanwhisper-0.4.0/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/tests/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:50.054992 africanwhisper-0.4.0/src/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/audio_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/gradio_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/gradio_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/wandb_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-10 21:18:46.000000 africanwhisper-0.4.0/src/training/whisper_model_prep.py
```

### Comparing `africanwhisper-0.3.0/LICENSE` & `africanwhisper-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.3.0/PKG-INFO` & `africanwhisper-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.3.0
+Version: 0.4.0
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -26,95 +26,77 @@
 Requires-Dist: pytube==15.0.0
 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
 Requires-Dist: yt-dlp==2023.11.14
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: logging==0.4.9.6
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
   <a href="https://github.com/KevKibe/African-Whisper/commits/">
     <img src="https://img.shields.io/github/last-commit/KevKibe/African-Whisper?" alt="Last commit">
   </a>
   <a href="https://github.com/KevKibe/African-Whisper/blob/main/LICENSE">
     <img src="https://img.shields.io/github/license/KevKibe/African-Whisper?" alt="License">
   </a>
 
-  
-
 </p>
 
 <p align="center">
     <img src= "image.png" width="100">
 </p>
 
-# Description
-African Whisper is an open-source project aimed at enhancing Automatic Speech Recognition (ASR): translation and transcription capabilities for African languages. 
-This is done by developing a package to allow seamless fine-tuning and deployment of the Whisper ASR model developed by OpenAI to better recognize and transcribe African languages for all developers.
-
-## Why Whisper?
-
-Whisper is an open-source Automatic Speech Recognition (ASR) system developed by OpenAI.<br> 
-Here’s why Whisper stands out:
-<details>
-
-  - **Extensive Training Data**: Trained on 680,000 hours of multilingual and multitask(translation and transcription) supervised data from the web.
-
-  - **Sequence-based Understanding**: Unlike Word2Vec, which lacks sequential context, Whisper considers the full sequence of spoken words, ensuring accurate context and nuance recognition.
-
-  - **Simplification for Developers**: Using Whisper, developers can deploy one model for transcribing a multitude of languages, including underrepresented ones, without sacrificing quality or context.
-
-  For more details, you can refer to the [Whisper ASR model paper](https://cdn.openai.com/papers/whisper.pdf).
 
-</details>
+*Enhancing Automatic Speech Recognition (ASR): translation and transcription capabilities for African languages by providing seamless fine-tuning and deploying pipelines for Whisper Model*.
+<br>
+![Diagram](diagram-1.png)
+## Features
+  
+- 🔧 Fine-tune the [Whisper](https://huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013) model on any audio dataset from Huggingface, e.g., [Mozilla's](https://huggingface.co/mozilla-foundation) Common Voice datasets.
 
+- 📊 View training run metrics on [Wandb](https://wandb.ai/).
 
+- 🎙️ Test your fine-tuned model using Gradio UI or directly on an audio file (.mp3 or .wav).
 
-## Proof of Concept
-<details>
+- 🚀 Deploy an API endpoint for audio file transcription or translation.
 
-  A successful proof of concept has been achieved by fine-tuning the Whisper-small model using a Google Colab Notebook and tested on an audiofile to test the performance. The results were promising, indicating the potential of this approach for ASR in African languages. You can explore the process and results in detail in the [repository](https://github.com/KevKibe/Finetuning-WhisperSmall-LoRA-Swahili)
+- 🐳 Containerize your API endpoint application and push to DockerHub.
 
-</details>
+## Why Whisper? 🤔
 
-## Objectives
-<details>
 
-To develop a quick-to-use fine-tuning and deployment pipeline utilizing audio datasets by the [Mozilla Foundation](https://commonvoice.mozilla.org/en), eventually having Automatic Speech Recognition (ASR) for African languages just as good as other non-African languages.
+- 🌐 **Extensive Training Data**: Trained on 680,000 hours of multilingual and multitask(translation and transcription) supervised data from the web.
 
-</details>
+- 🗣️ **Sequence-based Understanding**: Whisper considers the full sequence of spoken words, ensuring accurate context recognition, unlike Word2Vec.
 
-## Features
+- 💻 **Simplification for Applications**: Deploy one model for transcribing and translating a multitude of languages, without sacrificing quality or context.
 
-<details>
-  
-  1. Fine-tune a version of [whisper](https://huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013) on any dataset from [Mozilla's](https://huggingface.co/mozilla-foundation) Common Voice datasets.
+For more details, you can refer to the [Whisper ASR model paper](https://cdn.openai.com/papers/whisper.pdf).<br>
+Want proof, check this [repo](https://github.com/KevKibe/Finetuning-WhisperSmall-LoRA-Swahili)
 
-  2. View your training run metrics on [Wandb](https://wandb.ai/).
 
-  3. Test your fine-tuned model using Gradio UI.
 
-  4. Deploy a REST API endpoint fro transcription of Audio files.
-
-  5. Containerize your REST API endpoint and push to DockerHub.
-</details>
+# 🚀 Getting Started
 
 ## Prerequisites
 
 - Sign up to HuggingFace and get your token keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens).
 
-- Sign up for wandb and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
+- Sign up to Weights and Biases and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
 
+- Demo video [here](https://youtu.be/qj48Chu4i4k?si=Vwv-6-qI7GJF7AMd)
 
-# A Guide to Usage on a Notebook
+[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/16r4cxP-dSFplRTfgPLbzGXYRzBIUqpx9?usp=sharing)
 
 ## Step 1: Installation
 
 ```python
 !pip install africanwhisper
 # If you're on Colab, restart the session due to issue with numpy installation on colab.
 ```
@@ -122,20 +104,20 @@
 ## Step 2: Set Parameters
 
 ```python
 # Set the parameters (refer to the 'Usage on VM' section for more details)
 huggingface_read_token = " "
 huggingface_write_token = " "
 dataset_name = "mozilla-foundation/common_voice_16_1" 
-language_abbr= " " # Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
-                    # Note: choose a small dataset so as to not run out of memory,
-model_id= "model-id" # Example openai/whisper-small, openai/whisper-medium
+language_abbr= " "                                    # Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
+                                                      # Note: choose a small dataset so as to not run out of memory,
+model_id= "model-id"                                  # Example openai/whisper-small, openai/whisper-medium
 processing_task= "automatic-speech-recognition" 
 wandb_api_key = " "
-use_peft = True  # Note: PEFT only works on a notebook with GPU-support.
+use_peft = True                                       # Note: PEFT only works on a notebook with GPU-support.
 
 ```
 
 ## Step 3: Prepare the Model
 ```python
 from training.data_prep import DataPrep
 
@@ -178,15 +160,15 @@
     tokenizer,
     language_abbr,
     wandb_api_key,
     use_peft
 )
 trainer.train(
     max_steps=100,
-    learning_rate=1e-5,
+    learning_rate=1e-3,
     per_device_train_batch_size=96,
     per_device_eval_batch_size=64,
     optim="adamw_bnb_8bit"
 )
 
 # Optional parameters for training:
 #     max_steps (int): The maximum number of training steps (default is 100).
@@ -198,132 +180,121 @@
 ```
 
 ## Step 6: Generate a Demo using GradioUI
 ```python
 from training.gradio_inference import WhisperDemo
 
 # Generate a demo
-model_name = "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
+model_name = "your-finetuned-model-name-on-huggingface-hub"     # e.g., "KevinKibe/whisper-small-af"
 demo = WhisperDemo(model_name, huggingface_read_token)
 demo.generate_demo()
 ```
 
 ## Step 7: Test Model using Audio File
 
 ```python
 from deployment.speech_inference import SpeechInference
 
-model_name = "your-finetuned-model-name-on-huggingface-hub"  # e.g., "KevinKibe/whisper-small-af"
+model_name = "your-finetuned-model-name-on-huggingface-hub"   # e.g., "KevinKibe/whisper-small-af"
 huggingface_read_token = " "
-task = "desired-task"  # either 'translate' or 'transcribe'
-audiofile_dir = "location-of-audio-file"  # filetype should be .mp3 or .wav
+task = "desired-task"                                         # either 'translate' or 'transcribe'
+audiofile_dir = "location-of-audio-file"                      # filetype should be .mp3 or .wav
 
 # Initialize the SpeechInference class and run inference
 inference = SpeechInference(model_name, huggingface_read_token)
 pipeline = inference.pipe_initialization()
 transcription = inference.output(pipeline, audiofile_dir, task)
 
 # Access different parts of the output
-print(transcription.text)  # The entire text transcription.
-print(transcription.chunks)  # List of individual text chunks with timestamps.
-print(transcription.timestamps)  # List of timestamps for each chunk.
-print(transcription.chunk_texts)  # List of texts for each chunk.
+print(transcription.text)                                       # The entire text transcription.
+print(transcription.chunks)                                     # List of individual text chunks with timestamps.
+print(transcription.timestamps)                                 # List of timestamps for each chunk.
+print(transcription.chunk_texts)                                # List of texts for each chunk.
 
 ```
 
-## Usage on a Virtual Machine
-
-<details>
-
-  - Clone the Repository: Clone or download the application code to your local machine.
-  ```
-  git clone https://github.com/KevKibe/African-Whisper.git
-  ```
+# 🖥️ Using the CLI
 
-  - Create a virtual environment for the project and activate it.
-  ```
-  python3 -m venv env
-  source venv/bin/activate
-  ```
-
-  - Install dependencies by running this command
-  ```
-  pip install -r requirements.txt
-  ```
-  - Navigate to:
-  ```
-  cd src
-  ```
-
-  - To start the training , use the following command:
-  ```
-  python -m training.main \
-      --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \
-      --huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \
-      --dataset_name DATASET_NAME \
-      --language_abbr LANGUAGE_ABBREVIATION \
-      --model_id MODEL_ID \
-      --processing_task PROCESSING_TASK \
-      --wandb_api_key YOUR_WANDB_API_KEY_HERE \
-      --use_peft 
-  ```
-  Here's a short description of each argument used in the command:
-
-  - **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
+- Clone the Repository: Clone or download the application code to your local machine.
+```bash
+git clone https://github.com/KevKibe/African-Whisper.git
+```
 
-  - **--huggingface_push_token**: Your Hugging Face authentication token for write access. It's used for uploading models to your Hugging Face account.
+- Create a virtual environment for the project and activate it.
+```bash
+python3 -m venv env
+source venv/bin/activate
+```
 
-  - **--dataset_name**: The name of the dataset you wish to use for training. Example: 'mozilla-foundation/common_voice_16_1'. This should match the dataset's identifier on the Hugging Face Datasets Hub.
+- Install dependencies by running this command
+```bash
+pip install -r requirements.txt
+```
+- Navigate to:
+```bash
+cd src
+```
 
-  - **--language_abbr**: The abbreviation of the language for the dataset you're using. Example: 'sw' for Swahili. This is used to specify the language variant of the dataset if it supports multiple languages.
+- To start the training , use the following command:
+```bash
+python -m training.main --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE --huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name AUDIO_DATASET_NAME --language_abbr LANGUAGE_ABBREVIATION --model_id MODEL_ID --processing_task PROCESSING_TASK --wandb_api_key YOUR_WANDB_API_KEY_HERE --use_peft # leave this out to opt-out of using PEFT
+```
+- Find a description of these commands [here](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/PARAMETERS.md).
 
-  - **--model_id**: Identifier for the pre-trained model you wish to fine-tune. Example: 'openai/whisper-small'. This should match the model's identifier on the Hugging Face Model Hub.
+### Inference
 
-  - **--processing_task**: Specifies the task for which the model is being trained. Example: 'transcribe'. This defines the objective of the model training, such as transcribing audio to text.
+- To get inference from your fine-tuned model, follow these steps:
 
-  - **--wandb_api_key**: Your Weights & Biases (W&B) API key. This is used for logging and tracking the training process if you're using W&B for experiment tracking.
+- Ensure that ffmpeg is installed by running the following commands:
 
-  - **--use_peft**: Add this flag to fine-tune using PEFT method and omit it to do full fine-tuning. PEFT only works on a notbeook with GPU-support.
+```bash
+# on Ubuntu or Debian
+sudo apt update && sudo apt install ffmpeg
 
-  ## Inference
+# on Arch Linux
+sudo pacman -S ffmpeg
 
-  - To get inference from your fine-tuned model, follow these steps:
+# on MacOS using Homebrew (https://brew.sh/)
+brew install ffmpeg
 
-  - Ensure that ffmpeg is installed by running the following commands:
-  ```
-  # on Ubuntu or Debian
-  sudo apt update && sudo apt install ffmpeg
+# on Windows using Chocolatey (https://chocolatey.org/)
+choco install ffmpeg
 
-  # on Arch Linux
-  sudo pacman -S ffmpeg
+# on Windows using Scoop (https://scoop.sh/)
+scoop install ffmpeg
+```
 
-  # on MacOS using Homebrew (https://brew.sh/)
-  brew install ffmpeg
+- To get the Gradio inference URL:
+```bash
+python -m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE 
+```
+- **--model_name**: Name of the fine-tuned model to use in your huggingfacehub repo. This should match the model's identifier on the Hugging Face Model Hub.
+- **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
 
-  # on Windows using Chocolatey (https://chocolatey.org/)
-  choco install ffmpeg
+- To launch the REST API endpoint locally:
 
-  # on Windows using Scoop (https://scoop.sh/)
-  scoop install ffmpeg
-  ```
+```bash
+cd src/deployment
+```
+- Create a `.env` file using `nano .env` command and add these keys and save the file.
+```python
+MODEL_NAME = "your-finetuned-model"
+HUGGINGFACE_READ_TOKEN = "huggingface-read-token"
+```
 
-  - To get the Gradio inference URL:
-  ```
-  python -m training.gradio_demo \
-      --model_name YOUR_FINETUNED-MODEL \
-      --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \
-  ```
-  - **--model_name**: Name of the fine-tuned model to use in your huggingfacehub repo. This should match the model's identifier on the Hugging Face Model Hub.
-  - **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
+- Run this command to launch the endpoint:
+```bash
+uvicorn main:app --host 0.0.0.0 --port 8000
+```
 
-</details>
+- Test it out by accessing the Swagger UI at `http://localhost:8000/docs` and uploading either an .mp3 file or a .wav file and a task either `transcribe` or `translate`. Alternatively, you can use Postman with the URL `http://localhost:8000/speechinference`.
 
-## Deployment
+## 🛳️ Deployment
 
-- To deploy your fine-tuned model (assuming it's on Hugging Face Hub) as a REST API endpoint, follow this [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
+- To deploy your fine-tuned model (assuming it's on Hugging Face Hub) as a REST API endpoint, follow these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
 
 
 ## Contributing 
 Contributions are welcome and encouraged.
 
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
```

#### html2text {}

```diff
@@ -1,83 +1,76 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.3.0 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.4.0 Summary: A package
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
-probability==0.24.0 Requires-Dist: yt-dlp==2023.11.14
+probability==0.24.0 Requires-Dist: yt-dlp==2023.11.14 Requires-Dist: python-
+dotenv==1.0.1 Requires-Dist: logging==0.4.9.6
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
-# Description African Whisper is an open-source project aimed at enhancing
-Automatic Speech Recognition (ASR): translation and transcription capabilities
-for African languages. This is done by developing a package to allow seamless
-fine-tuning and deployment of the Whisper ASR model developed by OpenAI to
-better recognize and transcribe African languages for all developers. ## Why
-Whisper? Whisper is an open-source Automatic Speech Recognition (ASR) system
-developed by OpenAI.
-Hereâs why Whisper stands out: - **Extensive Training Data**: Trained on
-680,000 hours of multilingual and multitask(translation and transcription)
-supervised data from the web. - **Sequence-based Understanding**: Unlike
-Word2Vec, which lacks sequential context, Whisper considers the full sequence
-of spoken words, ensuring accurate context and nuance recognition. -
-**Simplification for Developers**: Using Whisper, developers can deploy one
-model for transcribing a multitude of languages, including underrepresented
-ones, without sacrificing quality or context. For more details, you can refer
-to the [Whisper ASR model paper](https://cdn.openai.com/papers/whisper.pdf). ##
-Proof of Concept A successful proof of concept has been achieved by fine-tuning
-the Whisper-small model using a Google Colab Notebook and tested on an
-audiofile to test the performance. The results were promising, indicating the
-potential of this approach for ASR in African languages. You can explore the
-process and results in detail in the [repository](https://github.com/KevKibe/
-Finetuning-WhisperSmall-LoRA-Swahili) ## Objectives To develop a quick-to-use
-fine-tuning and deployment pipeline utilizing audio datasets by the [Mozilla
-Foundation](https://commonvoice.mozilla.org/en), eventually having Automatic
-Speech Recognition (ASR) for African languages just as good as other non-
-African languages. ## Features 1. Fine-tune a version of [whisper](https://
-huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013) on
-any dataset from [Mozilla's](https://huggingface.co/mozilla-foundation) Common
-Voice datasets. 2. View your training run metrics on [Wandb](https://wandb.ai/
-). 3. Test your fine-tuned model using Gradio UI. 4. Deploy a REST API endpoint
-fro transcription of Audio files. 5. Containerize your REST API endpoint and
-push to DockerHub. ## Prerequisites - Sign up to HuggingFace and get your token
-keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens). -
-Sign up for wandb and get your token keys use this [guide](https://
-app.wandb.ai/login?signup=true) # A Guide to Usage on a Notebook ## Step 1:
-Installation ```python !pip install africanwhisper # If you're on Colab,
-restart the session due to issue with numpy installation on colab. ``` ## Step
-2: Set Parameters ```python # Set the parameters (refer to the 'Usage on VM'
-section for more details) huggingface_read_token = " " huggingface_write_token
-= " " dataset_name = "mozilla-foundation/common_voice_16_1" language_abbr= " "
-# Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/
-mozilla-foundation/common_voice_16_1. # Note: choose a small dataset so as to
-not run out of memory, model_id= "model-id" # Example openai/whisper-small,
-openai/whisper-medium processing_task= "automatic-speech-recognition"
-wandb_api_key = " " use_peft = True # Note: PEFT only works on a notebook with
-GPU-support. ``` ## Step 3: Prepare the Model ```python from training.data_prep
-import DataPrep # Initialize the DataPrep class and prepare the model process =
-DataPrep( huggingface_read_token, dataset_name, language_abbr, model_id,
-processing_task, use_peft ) tokenizer, feature_extractor, feature_processor,
-model = process.prepare_model() ``` ## Step 4: Preprocess the Dataset ```python
-# Load and preprocess the dataset processed_dataset = process.load_dataset
-( feature_extractor=feature_extractor, tokenizer=tokenizer,
-processor=feature_processor ) ``` ## Step 5: Train the Model ```python from
-training.model_trainer import Trainer # Initialize the Trainer class and train
-the model trainer = Trainer( huggingface_write_token, model_id,
-processed_dataset, model, feature_processor, feature_extractor, tokenizer,
-language_abbr, wandb_api_key, use_peft ) trainer.train( max_steps=100,
-learning_rate=1e-5, per_device_train_batch_size=96,
+*Enhancing Automatic Speech Recognition (ASR): translation and transcription
+capabilities for African languages by providing seamless fine-tuning and
+deploying pipelines for Whisper Model*.
+![Diagram](diagram-1.png) ## Features - ð§ Fine-tune the [Whisper](https://
+huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013)
+model on any audio dataset from Huggingface, e.g., [Mozilla's](https://
+huggingface.co/mozilla-foundation) Common Voice datasets. - ð View training
+run metrics on [Wandb](https://wandb.ai/). - ðï¸ Test your fine-tuned model
+using Gradio UI or directly on an audio file (.mp3 or .wav). - ð Deploy an
+API endpoint for audio file transcription or translation. - ð³ Containerize
+your API endpoint application and push to DockerHub. ## Why Whisper? ð¤ -
+ð **Extensive Training Data**: Trained on 680,000 hours of multilingual and
+multitask(translation and transcription) supervised data from the web. -
+ð£ï¸ **Sequence-based Understanding**: Whisper considers the full sequence
+of spoken words, ensuring accurate context recognition, unlike Word2Vec. - ð»
+**Simplification for Applications**: Deploy one model for transcribing and
+translating a multitude of languages, without sacrificing quality or context.
+For more details, you can refer to the [Whisper ASR model paper](https://
+cdn.openai.com/papers/whisper.pdf).
+Want proof, check this [repo](https://github.com/KevKibe/Finetuning-
+WhisperSmall-LoRA-Swahili) # ð Getting Started ## Prerequisites - Sign up to
+HuggingFace and get your token keys use this [guide](https://huggingface.co/
+docs/hub/en/security-tokens). - Sign up to Weights and Biases and get your
+token keys use this [guide](https://app.wandb.ai/login?signup=true) - Demo
+video [here](https://youtu.be/qj48Chu4i4k?si=Vwv-6-qI7GJF7AMd) [![Colab](https:
+//colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/16r4cxP-dSFplRTfgPLbzGXYRzBIUqpx9?usp=sharing)
+## Step 1: Installation ```python !pip install africanwhisper # If you're on
+Colab, restart the session due to issue with numpy installation on colab. ```
+## Step 2: Set Parameters ```python # Set the parameters (refer to the 'Usage
+on VM' section for more details) huggingface_read_token = " "
+huggingface_write_token = " " dataset_name = "mozilla-foundation/
+common_voice_16_1" language_abbr= " " # Example 'af', 'sw'. see abbreviations
+here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. #
+Note: choose a small dataset so as to not run out of memory, model_id= "model-
+id" # Example openai/whisper-small, openai/whisper-medium processing_task=
+"automatic-speech-recognition" wandb_api_key = " " use_peft = True # Note: PEFT
+only works on a notebook with GPU-support. ``` ## Step 3: Prepare the Model
+```python from training.data_prep import DataPrep # Initialize the DataPrep
+class and prepare the model process = DataPrep( huggingface_read_token,
+dataset_name, language_abbr, model_id, processing_task, use_peft ) tokenizer,
+feature_extractor, feature_processor, model = process.prepare_model() ``` ##
+Step 4: Preprocess the Dataset ```python # Load and preprocess the dataset
+processed_dataset = process.load_dataset( feature_extractor=feature_extractor,
+tokenizer=tokenizer, processor=feature_processor ) ``` ## Step 5: Train the
+Model ```python from training.model_trainer import Trainer # Initialize the
+Trainer class and train the model trainer = Trainer( huggingface_write_token,
+model_id, processed_dataset, model, feature_processor, feature_extractor,
+tokenizer, language_abbr, wandb_api_key, use_peft ) trainer.train
+( max_steps=100, learning_rate=1e-3, per_device_train_batch_size=96,
 per_device_eval_batch_size=64, optim="adamw_bnb_8bit" ) # Optional parameters
 for training: # max_steps (int): The maximum number of training steps (default
 is 100). # learning_rate (float): The learning rate for training (default is
 1e-5). # per_device_train_batch_size (int): The batch size per GPU for training
 (default is 96). # per_device_eval_batch_size (int): The batch size per GPU for
 evaluation (default is 64). # optim (str): The optimizer used for training
 (default is "adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI
@@ -92,62 +85,54 @@
 or .wav # Initialize the SpeechInference class and run inference inference =
 SpeechInference(model_name, huggingface_read_token) pipeline =
 inference.pipe_initialization() transcription = inference.output(pipeline,
 audiofile_dir, task) # Access different parts of the output print
 (transcription.text) # The entire text transcription. print
 (transcription.chunks) # List of individual text chunks with timestamps. print
 (transcription.timestamps) # List of timestamps for each chunk. print
-(transcription.chunk_texts) # List of texts for each chunk. ``` ## Usage on a
-Virtual Machine - Clone the Repository: Clone or download the application code
-to your local machine. ``` git clone https://github.com/KevKibe/African-
-Whisper.git ``` - Create a virtual environment for the project and activate it.
-``` python3 -m venv env source venv/bin/activate ``` - Install dependencies by
-running this command ``` pip install -r requirements.txt ``` - Navigate to: ```
-cd src ``` - To start the training , use the following command: ``` python -
-m training.main \ --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \
---huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \ --dataset_name
-DATASET_NAME \ --language_abbr LANGUAGE_ABBREVIATION \ --model_id MODEL_ID \ --
-processing_task PROCESSING_TASK \ --wandb_api_key YOUR_WANDB_API_KEY_HERE \ --
-use_peft ``` Here's a short description of each argument used in the command: -
-**--huggingface_read_token**: Your Hugging Face authentication token for read
-access. It allows you to download datasets and models from Hugging Face. - **--
-huggingface_push_token**: Your Hugging Face authentication token for write
-access. It's used for uploading models to your Hugging Face account. - **--
-dataset_name**: The name of the dataset you wish to use for training. Example:
-'mozilla-foundation/common_voice_16_1'. This should match the dataset's
-identifier on the Hugging Face Datasets Hub. - **--language_abbr**: The
-abbreviation of the language for the dataset you're using. Example: 'sw' for
-Swahili. This is used to specify the language variant of the dataset if it
-supports multiple languages. - **--model_id**: Identifier for the pre-trained
-model you wish to fine-tune. Example: 'openai/whisper-small'. This should match
-the model's identifier on the Hugging Face Model Hub. - **--processing_task**:
-Specifies the task for which the model is being trained. Example: 'transcribe'.
-This defines the objective of the model training, such as transcribing audio to
-text. - **--wandb_api_key**: Your Weights & Biases (W&B) API key. This is used
-for logging and tracking the training process if you're using W&B for
-experiment tracking. - **--use_peft**: Add this flag to fine-tune using PEFT
-method and omit it to do full fine-tuning. PEFT only works on a notbeook with
-GPU-support. ## Inference - To get inference from your fine-tuned model, follow
-these steps: - Ensure that ffmpeg is installed by running the following
-commands: ``` # on Ubuntu or Debian sudo apt update && sudo apt install ffmpeg
-# on Arch Linux sudo pacman -S ffmpeg # on MacOS using Homebrew (https://
-brew.sh/) brew install ffmpeg # on Windows using Chocolatey (https://
-chocolatey.org/) choco install ffmpeg # on Windows using Scoop (https://
-scoop.sh/) scoop install ffmpeg ``` - To get the Gradio inference URL: ```
-python -m training.gradio_demo \ --model_name YOUR_FINETUNED-MODEL \ --
-huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \ ``` - **--
+(transcription.chunk_texts) # List of texts for each chunk. ``` # ð¥ï¸ Using
+the CLI - Clone the Repository: Clone or download the application code to your
+local machine. ```bash git clone https://github.com/KevKibe/African-Whisper.git
+``` - Create a virtual environment for the project and activate it. ```bash
+python3 -m venv env source venv/bin/activate ``` - Install dependencies by
+running this command ```bash pip install -r requirements.txt ``` - Navigate to:
+```bash cd src ``` - To start the training , use the following command: ```bash
+python -m training.main --huggingface_read_token
+YOUR_HUGGING_FACE_READ_TOKEN_HERE --huggingface_write_token
+YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name AUDIO_DATASET_NAME --
+language_abbr LANGUAGE_ABBREVIATION --model_id MODEL_ID --processing_task
+PROCESSING_TASK --wandb_api_key YOUR_WANDB_API_KEY_HERE --use_peft # leave this
+out to opt-out of using PEFT ``` - Find a description of these commands [here]
+(https://github.com/KevKibe/African-Whisper/blob/master/DOCS/PARAMETERS.md).
+### Inference - To get inference from your fine-tuned model, follow these
+steps: - Ensure that ffmpeg is installed by running the following commands:
+```bash # on Ubuntu or Debian sudo apt update && sudo apt install ffmpeg # on
+Arch Linux sudo pacman -S ffmpeg # on MacOS using Homebrew (https://brew.sh/
+) brew install ffmpeg # on Windows using Chocolatey (https://chocolatey.org/
+) choco install ffmpeg # on Windows using Scoop (https://scoop.sh/) scoop
+install ffmpeg ``` - To get the Gradio inference URL: ```bash python -
+m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --
+huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE ``` - **--
 model_name**: Name of the fine-tuned model to use in your huggingfacehub repo.
 This should match the model's identifier on the Hugging Face Model Hub. - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
-access. It allows you to download datasets and models from Hugging Face. ##
-Deployment - To deploy your fine-tuned model (assuming it's on Hugging Face
-Hub) as a REST API endpoint, follow this [instructions](https://github.com/
-KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ## Contributing
-Contributions are welcome and encouraged. Before contributing, please take a
-moment to review our [Contribution Guidelines](https://github.com/KevKibe/
-African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for important information on
-how to contribute to this project. If you're unsure about anything or need
-assistance, don't hesitate to reach out to us or open an issue to discuss your
-ideas. We look forward to your contributions! ## License This project is
-licensed under the MIT License - see the [LICENSE](https://github.com/KevKibe/
-African-Whisper/blob/main/LICENSE) file for details. ## Contact For any
-enquiries, please reach out to me through keviinkibe@gmail.com
+access. It allows you to download datasets and models from Hugging Face. - To
+launch the REST API endpoint locally: ```bash cd src/deployment ``` - Create a
+`.env` file using `nano .env` command and add these keys and save the file.
+```python MODEL_NAME = "your-finetuned-model" HUGGINGFACE_READ_TOKEN =
+"huggingface-read-token" ``` - Run this command to launch the endpoint: ```bash
+uvicorn main:app --host 0.0.0.0 --port 8000 ``` - Test it out by accessing the
+Swagger UI at `http://localhost:8000/docs` and uploading either an .mp3 file or
+a .wav file and a task either `transcribe` or `translate`. Alternatively, you
+can use Postman with the URL `http://localhost:8000/speechinference`. ##
+ð³ï¸ Deployment - To deploy your fine-tuned model (assuming it's on Hugging
+Face Hub) as a REST API endpoint, follow these [instructions](https://
+github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ##
+Contributing Contributions are welcome and encouraged. Before contributing,
+please take a moment to review our [Contribution Guidelines](https://
+github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for
+important information on how to contribute to this project. If you're unsure
+about anything or need assistance, don't hesitate to reach out to us or open an
+issue to discuss your ideas. We look forward to your contributions! ## License
+This project is licensed under the MIT License - see the [LICENSE](https://
+github.com/KevKibe/African-Whisper/blob/main/LICENSE) file for details. ##
+Contact For any enquiries, please reach out to me through keviinkibe@gmail.com
```

### Comparing `africanwhisper-0.3.0/README.md` & `africanwhisper-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,81 +7,61 @@
   <a href="https://github.com/KevKibe/African-Whisper/commits/">
     <img src="https://img.shields.io/github/last-commit/KevKibe/African-Whisper?" alt="Last commit">
   </a>
   <a href="https://github.com/KevKibe/African-Whisper/blob/main/LICENSE">
     <img src="https://img.shields.io/github/license/KevKibe/African-Whisper?" alt="License">
   </a>
 
-  
-
 </p>
 
 <p align="center">
     <img src= "image.png" width="100">
 </p>
 
-# Description
-African Whisper is an open-source project aimed at enhancing Automatic Speech Recognition (ASR): translation and transcription capabilities for African languages. 
-This is done by developing a package to allow seamless fine-tuning and deployment of the Whisper ASR model developed by OpenAI to better recognize and transcribe African languages for all developers.
-
-## Why Whisper?
-
-Whisper is an open-source Automatic Speech Recognition (ASR) system developed by OpenAI.<br> 
-Here’s why Whisper stands out:
-<details>
-
-  - **Extensive Training Data**: Trained on 680,000 hours of multilingual and multitask(translation and transcription) supervised data from the web.
-
-  - **Sequence-based Understanding**: Unlike Word2Vec, which lacks sequential context, Whisper considers the full sequence of spoken words, ensuring accurate context and nuance recognition.
-
-  - **Simplification for Developers**: Using Whisper, developers can deploy one model for transcribing a multitude of languages, including underrepresented ones, without sacrificing quality or context.
-
-  For more details, you can refer to the [Whisper ASR model paper](https://cdn.openai.com/papers/whisper.pdf).
 
-</details>
+*Enhancing Automatic Speech Recognition (ASR): translation and transcription capabilities for African languages by providing seamless fine-tuning and deploying pipelines for Whisper Model*.
+<br>
+![Diagram](diagram-1.png)
+## Features
+  
+- 🔧 Fine-tune the [Whisper](https://huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013) model on any audio dataset from Huggingface, e.g., [Mozilla's](https://huggingface.co/mozilla-foundation) Common Voice datasets.
 
+- 📊 View training run metrics on [Wandb](https://wandb.ai/).
 
+- 🎙️ Test your fine-tuned model using Gradio UI or directly on an audio file (.mp3 or .wav).
 
-## Proof of Concept
-<details>
+- 🚀 Deploy an API endpoint for audio file transcription or translation.
 
-  A successful proof of concept has been achieved by fine-tuning the Whisper-small model using a Google Colab Notebook and tested on an audiofile to test the performance. The results were promising, indicating the potential of this approach for ASR in African languages. You can explore the process and results in detail in the [repository](https://github.com/KevKibe/Finetuning-WhisperSmall-LoRA-Swahili)
+- 🐳 Containerize your API endpoint application and push to DockerHub.
 
-</details>
+## Why Whisper? 🤔
 
-## Objectives
-<details>
 
-To develop a quick-to-use fine-tuning and deployment pipeline utilizing audio datasets by the [Mozilla Foundation](https://commonvoice.mozilla.org/en), eventually having Automatic Speech Recognition (ASR) for African languages just as good as other non-African languages.
+- 🌐 **Extensive Training Data**: Trained on 680,000 hours of multilingual and multitask(translation and transcription) supervised data from the web.
 
-</details>
+- 🗣️ **Sequence-based Understanding**: Whisper considers the full sequence of spoken words, ensuring accurate context recognition, unlike Word2Vec.
 
-## Features
+- 💻 **Simplification for Applications**: Deploy one model for transcribing and translating a multitude of languages, without sacrificing quality or context.
 
-<details>
-  
-  1. Fine-tune a version of [whisper](https://huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013) on any dataset from [Mozilla's](https://huggingface.co/mozilla-foundation) Common Voice datasets.
+For more details, you can refer to the [Whisper ASR model paper](https://cdn.openai.com/papers/whisper.pdf).<br>
+Want proof, check this [repo](https://github.com/KevKibe/Finetuning-WhisperSmall-LoRA-Swahili)
 
-  2. View your training run metrics on [Wandb](https://wandb.ai/).
 
-  3. Test your fine-tuned model using Gradio UI.
 
-  4. Deploy a REST API endpoint fro transcription of Audio files.
-
-  5. Containerize your REST API endpoint and push to DockerHub.
-</details>
+# 🚀 Getting Started
 
 ## Prerequisites
 
 - Sign up to HuggingFace and get your token keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens).
 
-- Sign up for wandb and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
+- Sign up to Weights and Biases and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
 
+- Demo video [here](https://youtu.be/qj48Chu4i4k?si=Vwv-6-qI7GJF7AMd)
 
-# A Guide to Usage on a Notebook
+[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/16r4cxP-dSFplRTfgPLbzGXYRzBIUqpx9?usp=sharing)
 
 ## Step 1: Installation
 
 ```python
 !pip install africanwhisper
 # If you're on Colab, restart the session due to issue with numpy installation on colab.
 ```
@@ -89,20 +69,20 @@
 ## Step 2: Set Parameters
 
 ```python
 # Set the parameters (refer to the 'Usage on VM' section for more details)
 huggingface_read_token = " "
 huggingface_write_token = " "
 dataset_name = "mozilla-foundation/common_voice_16_1" 
-language_abbr= " " # Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
-                    # Note: choose a small dataset so as to not run out of memory,
-model_id= "model-id" # Example openai/whisper-small, openai/whisper-medium
+language_abbr= " "                                    # Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
+                                                      # Note: choose a small dataset so as to not run out of memory,
+model_id= "model-id"                                  # Example openai/whisper-small, openai/whisper-medium
 processing_task= "automatic-speech-recognition" 
 wandb_api_key = " "
-use_peft = True  # Note: PEFT only works on a notebook with GPU-support.
+use_peft = True                                       # Note: PEFT only works on a notebook with GPU-support.
 
 ```
 
 ## Step 3: Prepare the Model
 ```python
 from training.data_prep import DataPrep
 
@@ -145,15 +125,15 @@
     tokenizer,
     language_abbr,
     wandb_api_key,
     use_peft
 )
 trainer.train(
     max_steps=100,
-    learning_rate=1e-5,
+    learning_rate=1e-3,
     per_device_train_batch_size=96,
     per_device_eval_batch_size=64,
     optim="adamw_bnb_8bit"
 )
 
 # Optional parameters for training:
 #     max_steps (int): The maximum number of training steps (default is 100).
@@ -165,132 +145,121 @@
 ```
 
 ## Step 6: Generate a Demo using GradioUI
 ```python
 from training.gradio_inference import WhisperDemo
 
 # Generate a demo
-model_name = "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
+model_name = "your-finetuned-model-name-on-huggingface-hub"     # e.g., "KevinKibe/whisper-small-af"
 demo = WhisperDemo(model_name, huggingface_read_token)
 demo.generate_demo()
 ```
 
 ## Step 7: Test Model using Audio File
 
 ```python
 from deployment.speech_inference import SpeechInference
 
-model_name = "your-finetuned-model-name-on-huggingface-hub"  # e.g., "KevinKibe/whisper-small-af"
+model_name = "your-finetuned-model-name-on-huggingface-hub"   # e.g., "KevinKibe/whisper-small-af"
 huggingface_read_token = " "
-task = "desired-task"  # either 'translate' or 'transcribe'
-audiofile_dir = "location-of-audio-file"  # filetype should be .mp3 or .wav
+task = "desired-task"                                         # either 'translate' or 'transcribe'
+audiofile_dir = "location-of-audio-file"                      # filetype should be .mp3 or .wav
 
 # Initialize the SpeechInference class and run inference
 inference = SpeechInference(model_name, huggingface_read_token)
 pipeline = inference.pipe_initialization()
 transcription = inference.output(pipeline, audiofile_dir, task)
 
 # Access different parts of the output
-print(transcription.text)  # The entire text transcription.
-print(transcription.chunks)  # List of individual text chunks with timestamps.
-print(transcription.timestamps)  # List of timestamps for each chunk.
-print(transcription.chunk_texts)  # List of texts for each chunk.
+print(transcription.text)                                       # The entire text transcription.
+print(transcription.chunks)                                     # List of individual text chunks with timestamps.
+print(transcription.timestamps)                                 # List of timestamps for each chunk.
+print(transcription.chunk_texts)                                # List of texts for each chunk.
 
 ```
 
-## Usage on a Virtual Machine
-
-<details>
-
-  - Clone the Repository: Clone or download the application code to your local machine.
-  ```
-  git clone https://github.com/KevKibe/African-Whisper.git
-  ```
+# 🖥️ Using the CLI
 
-  - Create a virtual environment for the project and activate it.
-  ```
-  python3 -m venv env
-  source venv/bin/activate
-  ```
-
-  - Install dependencies by running this command
-  ```
-  pip install -r requirements.txt
-  ```
-  - Navigate to:
-  ```
-  cd src
-  ```
-
-  - To start the training , use the following command:
-  ```
-  python -m training.main \
-      --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \
-      --huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \
-      --dataset_name DATASET_NAME \
-      --language_abbr LANGUAGE_ABBREVIATION \
-      --model_id MODEL_ID \
-      --processing_task PROCESSING_TASK \
-      --wandb_api_key YOUR_WANDB_API_KEY_HERE \
-      --use_peft 
-  ```
-  Here's a short description of each argument used in the command:
-
-  - **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
+- Clone the Repository: Clone or download the application code to your local machine.
+```bash
+git clone https://github.com/KevKibe/African-Whisper.git
+```
 
-  - **--huggingface_push_token**: Your Hugging Face authentication token for write access. It's used for uploading models to your Hugging Face account.
+- Create a virtual environment for the project and activate it.
+```bash
+python3 -m venv env
+source venv/bin/activate
+```
 
-  - **--dataset_name**: The name of the dataset you wish to use for training. Example: 'mozilla-foundation/common_voice_16_1'. This should match the dataset's identifier on the Hugging Face Datasets Hub.
+- Install dependencies by running this command
+```bash
+pip install -r requirements.txt
+```
+- Navigate to:
+```bash
+cd src
+```
 
-  - **--language_abbr**: The abbreviation of the language for the dataset you're using. Example: 'sw' for Swahili. This is used to specify the language variant of the dataset if it supports multiple languages.
+- To start the training , use the following command:
+```bash
+python -m training.main --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE --huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name AUDIO_DATASET_NAME --language_abbr LANGUAGE_ABBREVIATION --model_id MODEL_ID --processing_task PROCESSING_TASK --wandb_api_key YOUR_WANDB_API_KEY_HERE --use_peft # leave this out to opt-out of using PEFT
+```
+- Find a description of these commands [here](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/PARAMETERS.md).
 
-  - **--model_id**: Identifier for the pre-trained model you wish to fine-tune. Example: 'openai/whisper-small'. This should match the model's identifier on the Hugging Face Model Hub.
+### Inference
 
-  - **--processing_task**: Specifies the task for which the model is being trained. Example: 'transcribe'. This defines the objective of the model training, such as transcribing audio to text.
+- To get inference from your fine-tuned model, follow these steps:
 
-  - **--wandb_api_key**: Your Weights & Biases (W&B) API key. This is used for logging and tracking the training process if you're using W&B for experiment tracking.
+- Ensure that ffmpeg is installed by running the following commands:
 
-  - **--use_peft**: Add this flag to fine-tune using PEFT method and omit it to do full fine-tuning. PEFT only works on a notbeook with GPU-support.
+```bash
+# on Ubuntu or Debian
+sudo apt update && sudo apt install ffmpeg
 
-  ## Inference
+# on Arch Linux
+sudo pacman -S ffmpeg
 
-  - To get inference from your fine-tuned model, follow these steps:
+# on MacOS using Homebrew (https://brew.sh/)
+brew install ffmpeg
 
-  - Ensure that ffmpeg is installed by running the following commands:
-  ```
-  # on Ubuntu or Debian
-  sudo apt update && sudo apt install ffmpeg
+# on Windows using Chocolatey (https://chocolatey.org/)
+choco install ffmpeg
 
-  # on Arch Linux
-  sudo pacman -S ffmpeg
+# on Windows using Scoop (https://scoop.sh/)
+scoop install ffmpeg
+```
 
-  # on MacOS using Homebrew (https://brew.sh/)
-  brew install ffmpeg
+- To get the Gradio inference URL:
+```bash
+python -m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE 
+```
+- **--model_name**: Name of the fine-tuned model to use in your huggingfacehub repo. This should match the model's identifier on the Hugging Face Model Hub.
+- **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
 
-  # on Windows using Chocolatey (https://chocolatey.org/)
-  choco install ffmpeg
+- To launch the REST API endpoint locally:
 
-  # on Windows using Scoop (https://scoop.sh/)
-  scoop install ffmpeg
-  ```
+```bash
+cd src/deployment
+```
+- Create a `.env` file using `nano .env` command and add these keys and save the file.
+```python
+MODEL_NAME = "your-finetuned-model"
+HUGGINGFACE_READ_TOKEN = "huggingface-read-token"
+```
 
-  - To get the Gradio inference URL:
-  ```
-  python -m training.gradio_demo \
-      --model_name YOUR_FINETUNED-MODEL \
-      --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \
-  ```
-  - **--model_name**: Name of the fine-tuned model to use in your huggingfacehub repo. This should match the model's identifier on the Hugging Face Model Hub.
-  - **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
+- Run this command to launch the endpoint:
+```bash
+uvicorn main:app --host 0.0.0.0 --port 8000
+```
 
-</details>
+- Test it out by accessing the Swagger UI at `http://localhost:8000/docs` and uploading either an .mp3 file or a .wav file and a task either `transcribe` or `translate`. Alternatively, you can use Postman with the URL `http://localhost:8000/speechinference`.
 
-## Deployment
+## 🛳️ Deployment
 
-- To deploy your fine-tuned model (assuming it's on Hugging Face Hub) as a REST API endpoint, follow this [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
+- To deploy your fine-tuned model (assuming it's on Hugging Face Hub) as a REST API endpoint, follow these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
 
 
 ## Contributing 
 Contributions are welcome and encouraged.
 
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
 
@@ -299,8 +268,8 @@
 We look forward to your contributions!
 
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/KevKibe/African-Whisper/blob/main/LICENSE) file for details.
 
 ## Contact
-For any enquiries, please reach out to me through keviinkibe@gmail.com
+For any enquiries, please reach out to me through keviinkibe@gmail.com
```

#### html2text {}

```diff
@@ -1,68 +1,60 @@
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
-# Description African Whisper is an open-source project aimed at enhancing
-Automatic Speech Recognition (ASR): translation and transcription capabilities
-for African languages. This is done by developing a package to allow seamless
-fine-tuning and deployment of the Whisper ASR model developed by OpenAI to
-better recognize and transcribe African languages for all developers. ## Why
-Whisper? Whisper is an open-source Automatic Speech Recognition (ASR) system
-developed by OpenAI.
-Hereâs why Whisper stands out: - **Extensive Training Data**: Trained on
-680,000 hours of multilingual and multitask(translation and transcription)
-supervised data from the web. - **Sequence-based Understanding**: Unlike
-Word2Vec, which lacks sequential context, Whisper considers the full sequence
-of spoken words, ensuring accurate context and nuance recognition. -
-**Simplification for Developers**: Using Whisper, developers can deploy one
-model for transcribing a multitude of languages, including underrepresented
-ones, without sacrificing quality or context. For more details, you can refer
-to the [Whisper ASR model paper](https://cdn.openai.com/papers/whisper.pdf). ##
-Proof of Concept A successful proof of concept has been achieved by fine-tuning
-the Whisper-small model using a Google Colab Notebook and tested on an
-audiofile to test the performance. The results were promising, indicating the
-potential of this approach for ASR in African languages. You can explore the
-process and results in detail in the [repository](https://github.com/KevKibe/
-Finetuning-WhisperSmall-LoRA-Swahili) ## Objectives To develop a quick-to-use
-fine-tuning and deployment pipeline utilizing audio datasets by the [Mozilla
-Foundation](https://commonvoice.mozilla.org/en), eventually having Automatic
-Speech Recognition (ASR) for African languages just as good as other non-
-African languages. ## Features 1. Fine-tune a version of [whisper](https://
-huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013) on
-any dataset from [Mozilla's](https://huggingface.co/mozilla-foundation) Common
-Voice datasets. 2. View your training run metrics on [Wandb](https://wandb.ai/
-). 3. Test your fine-tuned model using Gradio UI. 4. Deploy a REST API endpoint
-fro transcription of Audio files. 5. Containerize your REST API endpoint and
-push to DockerHub. ## Prerequisites - Sign up to HuggingFace and get your token
-keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens). -
-Sign up for wandb and get your token keys use this [guide](https://
-app.wandb.ai/login?signup=true) # A Guide to Usage on a Notebook ## Step 1:
-Installation ```python !pip install africanwhisper # If you're on Colab,
-restart the session due to issue with numpy installation on colab. ``` ## Step
-2: Set Parameters ```python # Set the parameters (refer to the 'Usage on VM'
-section for more details) huggingface_read_token = " " huggingface_write_token
-= " " dataset_name = "mozilla-foundation/common_voice_16_1" language_abbr= " "
-# Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/
-mozilla-foundation/common_voice_16_1. # Note: choose a small dataset so as to
-not run out of memory, model_id= "model-id" # Example openai/whisper-small,
-openai/whisper-medium processing_task= "automatic-speech-recognition"
-wandb_api_key = " " use_peft = True # Note: PEFT only works on a notebook with
-GPU-support. ``` ## Step 3: Prepare the Model ```python from training.data_prep
-import DataPrep # Initialize the DataPrep class and prepare the model process =
-DataPrep( huggingface_read_token, dataset_name, language_abbr, model_id,
-processing_task, use_peft ) tokenizer, feature_extractor, feature_processor,
-model = process.prepare_model() ``` ## Step 4: Preprocess the Dataset ```python
-# Load and preprocess the dataset processed_dataset = process.load_dataset
-( feature_extractor=feature_extractor, tokenizer=tokenizer,
-processor=feature_processor ) ``` ## Step 5: Train the Model ```python from
-training.model_trainer import Trainer # Initialize the Trainer class and train
-the model trainer = Trainer( huggingface_write_token, model_id,
-processed_dataset, model, feature_processor, feature_extractor, tokenizer,
-language_abbr, wandb_api_key, use_peft ) trainer.train( max_steps=100,
-learning_rate=1e-5, per_device_train_batch_size=96,
+*Enhancing Automatic Speech Recognition (ASR): translation and transcription
+capabilities for African languages by providing seamless fine-tuning and
+deploying pipelines for Whisper Model*.
+![Diagram](diagram-1.png) ## Features - ð§ Fine-tune the [Whisper](https://
+huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013)
+model on any audio dataset from Huggingface, e.g., [Mozilla's](https://
+huggingface.co/mozilla-foundation) Common Voice datasets. - ð View training
+run metrics on [Wandb](https://wandb.ai/). - ðï¸ Test your fine-tuned model
+using Gradio UI or directly on an audio file (.mp3 or .wav). - ð Deploy an
+API endpoint for audio file transcription or translation. - ð³ Containerize
+your API endpoint application and push to DockerHub. ## Why Whisper? ð¤ -
+ð **Extensive Training Data**: Trained on 680,000 hours of multilingual and
+multitask(translation and transcription) supervised data from the web. -
+ð£ï¸ **Sequence-based Understanding**: Whisper considers the full sequence
+of spoken words, ensuring accurate context recognition, unlike Word2Vec. - ð»
+**Simplification for Applications**: Deploy one model for transcribing and
+translating a multitude of languages, without sacrificing quality or context.
+For more details, you can refer to the [Whisper ASR model paper](https://
+cdn.openai.com/papers/whisper.pdf).
+Want proof, check this [repo](https://github.com/KevKibe/Finetuning-
+WhisperSmall-LoRA-Swahili) # ð Getting Started ## Prerequisites - Sign up to
+HuggingFace and get your token keys use this [guide](https://huggingface.co/
+docs/hub/en/security-tokens). - Sign up to Weights and Biases and get your
+token keys use this [guide](https://app.wandb.ai/login?signup=true) - Demo
+video [here](https://youtu.be/qj48Chu4i4k?si=Vwv-6-qI7GJF7AMd) [![Colab](https:
+//colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/16r4cxP-dSFplRTfgPLbzGXYRzBIUqpx9?usp=sharing)
+## Step 1: Installation ```python !pip install africanwhisper # If you're on
+Colab, restart the session due to issue with numpy installation on colab. ```
+## Step 2: Set Parameters ```python # Set the parameters (refer to the 'Usage
+on VM' section for more details) huggingface_read_token = " "
+huggingface_write_token = " " dataset_name = "mozilla-foundation/
+common_voice_16_1" language_abbr= " " # Example 'af', 'sw'. see abbreviations
+here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. #
+Note: choose a small dataset so as to not run out of memory, model_id= "model-
+id" # Example openai/whisper-small, openai/whisper-medium processing_task=
+"automatic-speech-recognition" wandb_api_key = " " use_peft = True # Note: PEFT
+only works on a notebook with GPU-support. ``` ## Step 3: Prepare the Model
+```python from training.data_prep import DataPrep # Initialize the DataPrep
+class and prepare the model process = DataPrep( huggingface_read_token,
+dataset_name, language_abbr, model_id, processing_task, use_peft ) tokenizer,
+feature_extractor, feature_processor, model = process.prepare_model() ``` ##
+Step 4: Preprocess the Dataset ```python # Load and preprocess the dataset
+processed_dataset = process.load_dataset( feature_extractor=feature_extractor,
+tokenizer=tokenizer, processor=feature_processor ) ``` ## Step 5: Train the
+Model ```python from training.model_trainer import Trainer # Initialize the
+Trainer class and train the model trainer = Trainer( huggingface_write_token,
+model_id, processed_dataset, model, feature_processor, feature_extractor,
+tokenizer, language_abbr, wandb_api_key, use_peft ) trainer.train
+( max_steps=100, learning_rate=1e-3, per_device_train_batch_size=96,
 per_device_eval_batch_size=64, optim="adamw_bnb_8bit" ) # Optional parameters
 for training: # max_steps (int): The maximum number of training steps (default
 is 100). # learning_rate (float): The learning rate for training (default is
 1e-5). # per_device_train_batch_size (int): The batch size per GPU for training
 (default is 96). # per_device_eval_batch_size (int): The batch size per GPU for
 evaluation (default is 64). # optim (str): The optimizer used for training
 (default is "adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI
@@ -77,62 +69,54 @@
 or .wav # Initialize the SpeechInference class and run inference inference =
 SpeechInference(model_name, huggingface_read_token) pipeline =
 inference.pipe_initialization() transcription = inference.output(pipeline,
 audiofile_dir, task) # Access different parts of the output print
 (transcription.text) # The entire text transcription. print
 (transcription.chunks) # List of individual text chunks with timestamps. print
 (transcription.timestamps) # List of timestamps for each chunk. print
-(transcription.chunk_texts) # List of texts for each chunk. ``` ## Usage on a
-Virtual Machine - Clone the Repository: Clone or download the application code
-to your local machine. ``` git clone https://github.com/KevKibe/African-
-Whisper.git ``` - Create a virtual environment for the project and activate it.
-``` python3 -m venv env source venv/bin/activate ``` - Install dependencies by
-running this command ``` pip install -r requirements.txt ``` - Navigate to: ```
-cd src ``` - To start the training , use the following command: ``` python -
-m training.main \ --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \
---huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \ --dataset_name
-DATASET_NAME \ --language_abbr LANGUAGE_ABBREVIATION \ --model_id MODEL_ID \ --
-processing_task PROCESSING_TASK \ --wandb_api_key YOUR_WANDB_API_KEY_HERE \ --
-use_peft ``` Here's a short description of each argument used in the command: -
-**--huggingface_read_token**: Your Hugging Face authentication token for read
-access. It allows you to download datasets and models from Hugging Face. - **--
-huggingface_push_token**: Your Hugging Face authentication token for write
-access. It's used for uploading models to your Hugging Face account. - **--
-dataset_name**: The name of the dataset you wish to use for training. Example:
-'mozilla-foundation/common_voice_16_1'. This should match the dataset's
-identifier on the Hugging Face Datasets Hub. - **--language_abbr**: The
-abbreviation of the language for the dataset you're using. Example: 'sw' for
-Swahili. This is used to specify the language variant of the dataset if it
-supports multiple languages. - **--model_id**: Identifier for the pre-trained
-model you wish to fine-tune. Example: 'openai/whisper-small'. This should match
-the model's identifier on the Hugging Face Model Hub. - **--processing_task**:
-Specifies the task for which the model is being trained. Example: 'transcribe'.
-This defines the objective of the model training, such as transcribing audio to
-text. - **--wandb_api_key**: Your Weights & Biases (W&B) API key. This is used
-for logging and tracking the training process if you're using W&B for
-experiment tracking. - **--use_peft**: Add this flag to fine-tune using PEFT
-method and omit it to do full fine-tuning. PEFT only works on a notbeook with
-GPU-support. ## Inference - To get inference from your fine-tuned model, follow
-these steps: - Ensure that ffmpeg is installed by running the following
-commands: ``` # on Ubuntu or Debian sudo apt update && sudo apt install ffmpeg
-# on Arch Linux sudo pacman -S ffmpeg # on MacOS using Homebrew (https://
-brew.sh/) brew install ffmpeg # on Windows using Chocolatey (https://
-chocolatey.org/) choco install ffmpeg # on Windows using Scoop (https://
-scoop.sh/) scoop install ffmpeg ``` - To get the Gradio inference URL: ```
-python -m training.gradio_demo \ --model_name YOUR_FINETUNED-MODEL \ --
-huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \ ``` - **--
+(transcription.chunk_texts) # List of texts for each chunk. ``` # ð¥ï¸ Using
+the CLI - Clone the Repository: Clone or download the application code to your
+local machine. ```bash git clone https://github.com/KevKibe/African-Whisper.git
+``` - Create a virtual environment for the project and activate it. ```bash
+python3 -m venv env source venv/bin/activate ``` - Install dependencies by
+running this command ```bash pip install -r requirements.txt ``` - Navigate to:
+```bash cd src ``` - To start the training , use the following command: ```bash
+python -m training.main --huggingface_read_token
+YOUR_HUGGING_FACE_READ_TOKEN_HERE --huggingface_write_token
+YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name AUDIO_DATASET_NAME --
+language_abbr LANGUAGE_ABBREVIATION --model_id MODEL_ID --processing_task
+PROCESSING_TASK --wandb_api_key YOUR_WANDB_API_KEY_HERE --use_peft # leave this
+out to opt-out of using PEFT ``` - Find a description of these commands [here]
+(https://github.com/KevKibe/African-Whisper/blob/master/DOCS/PARAMETERS.md).
+### Inference - To get inference from your fine-tuned model, follow these
+steps: - Ensure that ffmpeg is installed by running the following commands:
+```bash # on Ubuntu or Debian sudo apt update && sudo apt install ffmpeg # on
+Arch Linux sudo pacman -S ffmpeg # on MacOS using Homebrew (https://brew.sh/
+) brew install ffmpeg # on Windows using Chocolatey (https://chocolatey.org/
+) choco install ffmpeg # on Windows using Scoop (https://scoop.sh/) scoop
+install ffmpeg ``` - To get the Gradio inference URL: ```bash python -
+m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --
+huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE ``` - **--
 model_name**: Name of the fine-tuned model to use in your huggingfacehub repo.
 This should match the model's identifier on the Hugging Face Model Hub. - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
-access. It allows you to download datasets and models from Hugging Face. ##
-Deployment - To deploy your fine-tuned model (assuming it's on Hugging Face
-Hub) as a REST API endpoint, follow this [instructions](https://github.com/
-KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ## Contributing
-Contributions are welcome and encouraged. Before contributing, please take a
-moment to review our [Contribution Guidelines](https://github.com/KevKibe/
-African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for important information on
-how to contribute to this project. If you're unsure about anything or need
-assistance, don't hesitate to reach out to us or open an issue to discuss your
-ideas. We look forward to your contributions! ## License This project is
-licensed under the MIT License - see the [LICENSE](https://github.com/KevKibe/
-African-Whisper/blob/main/LICENSE) file for details. ## Contact For any
-enquiries, please reach out to me through keviinkibe@gmail.com
+access. It allows you to download datasets and models from Hugging Face. - To
+launch the REST API endpoint locally: ```bash cd src/deployment ``` - Create a
+`.env` file using `nano .env` command and add these keys and save the file.
+```python MODEL_NAME = "your-finetuned-model" HUGGINGFACE_READ_TOKEN =
+"huggingface-read-token" ``` - Run this command to launch the endpoint: ```bash
+uvicorn main:app --host 0.0.0.0 --port 8000 ``` - Test it out by accessing the
+Swagger UI at `http://localhost:8000/docs` and uploading either an .mp3 file or
+a .wav file and a task either `transcribe` or `translate`. Alternatively, you
+can use Postman with the URL `http://localhost:8000/speechinference`. ##
+ð³ï¸ Deployment - To deploy your fine-tuned model (assuming it's on Hugging
+Face Hub) as a REST API endpoint, follow these [instructions](https://
+github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ##
+Contributing Contributions are welcome and encouraged. Before contributing,
+please take a moment to review our [Contribution Guidelines](https://
+github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for
+important information on how to contribute to this project. If you're unsure
+about anything or need assistance, don't hesitate to reach out to us or open an
+issue to discuss your ideas. We look forward to your contributions! ## License
+This project is licensed under the MIT License - see the [LICENSE](https://
+github.com/KevKibe/African-Whisper/blob/main/LICENSE) file for details. ##
+Contact For any enquiries, please reach out to me through keviinkibe@gmail.com
```

### Comparing `africanwhisper-0.3.0/setup.cfg` & `africanwhisper-0.4.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = africanwhisper
 author = Kevin Kibe
-version = 0.3.0
+version = 0.4.0
 author_email = keviinkibe@gmail.com
 description = A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KevKibe/African-Whisper
 license = MIT
 
@@ -30,14 +30,16 @@
 	pytube==15.0.0
 	tf-keras==2.16.0
 	tensorflow==2.16.1
 	keras==3.1.1
 	scipy==1.12.0
 	tensorflow-probability==0.24.0
 	yt-dlp==2023.11.14
+	python-dotenv==1.0.1
+	logging==0.4.9.6
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `africanwhisper-0.3.0/src/africanwhisper.egg-info/PKG-INFO` & `africanwhisper-0.4.0/src/africanwhisper.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.3.0
+Version: 0.4.0
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -26,95 +26,77 @@
 Requires-Dist: pytube==15.0.0
 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
 Requires-Dist: yt-dlp==2023.11.14
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: logging==0.4.9.6
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
   <a href="https://github.com/KevKibe/African-Whisper/commits/">
     <img src="https://img.shields.io/github/last-commit/KevKibe/African-Whisper?" alt="Last commit">
   </a>
   <a href="https://github.com/KevKibe/African-Whisper/blob/main/LICENSE">
     <img src="https://img.shields.io/github/license/KevKibe/African-Whisper?" alt="License">
   </a>
 
-  
-
 </p>
 
 <p align="center">
     <img src= "image.png" width="100">
 </p>
 
-# Description
-African Whisper is an open-source project aimed at enhancing Automatic Speech Recognition (ASR): translation and transcription capabilities for African languages. 
-This is done by developing a package to allow seamless fine-tuning and deployment of the Whisper ASR model developed by OpenAI to better recognize and transcribe African languages for all developers.
-
-## Why Whisper?
-
-Whisper is an open-source Automatic Speech Recognition (ASR) system developed by OpenAI.<br> 
-Here’s why Whisper stands out:
-<details>
-
-  - **Extensive Training Data**: Trained on 680,000 hours of multilingual and multitask(translation and transcription) supervised data from the web.
-
-  - **Sequence-based Understanding**: Unlike Word2Vec, which lacks sequential context, Whisper considers the full sequence of spoken words, ensuring accurate context and nuance recognition.
-
-  - **Simplification for Developers**: Using Whisper, developers can deploy one model for transcribing a multitude of languages, including underrepresented ones, without sacrificing quality or context.
-
-  For more details, you can refer to the [Whisper ASR model paper](https://cdn.openai.com/papers/whisper.pdf).
 
-</details>
+*Enhancing Automatic Speech Recognition (ASR): translation and transcription capabilities for African languages by providing seamless fine-tuning and deploying pipelines for Whisper Model*.
+<br>
+![Diagram](diagram-1.png)
+## Features
+  
+- 🔧 Fine-tune the [Whisper](https://huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013) model on any audio dataset from Huggingface, e.g., [Mozilla's](https://huggingface.co/mozilla-foundation) Common Voice datasets.
 
+- 📊 View training run metrics on [Wandb](https://wandb.ai/).
 
+- 🎙️ Test your fine-tuned model using Gradio UI or directly on an audio file (.mp3 or .wav).
 
-## Proof of Concept
-<details>
+- 🚀 Deploy an API endpoint for audio file transcription or translation.
 
-  A successful proof of concept has been achieved by fine-tuning the Whisper-small model using a Google Colab Notebook and tested on an audiofile to test the performance. The results were promising, indicating the potential of this approach for ASR in African languages. You can explore the process and results in detail in the [repository](https://github.com/KevKibe/Finetuning-WhisperSmall-LoRA-Swahili)
+- 🐳 Containerize your API endpoint application and push to DockerHub.
 
-</details>
+## Why Whisper? 🤔
 
-## Objectives
-<details>
 
-To develop a quick-to-use fine-tuning and deployment pipeline utilizing audio datasets by the [Mozilla Foundation](https://commonvoice.mozilla.org/en), eventually having Automatic Speech Recognition (ASR) for African languages just as good as other non-African languages.
+- 🌐 **Extensive Training Data**: Trained on 680,000 hours of multilingual and multitask(translation and transcription) supervised data from the web.
 
-</details>
+- 🗣️ **Sequence-based Understanding**: Whisper considers the full sequence of spoken words, ensuring accurate context recognition, unlike Word2Vec.
 
-## Features
+- 💻 **Simplification for Applications**: Deploy one model for transcribing and translating a multitude of languages, without sacrificing quality or context.
 
-<details>
-  
-  1. Fine-tune a version of [whisper](https://huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013) on any dataset from [Mozilla's](https://huggingface.co/mozilla-foundation) Common Voice datasets.
+For more details, you can refer to the [Whisper ASR model paper](https://cdn.openai.com/papers/whisper.pdf).<br>
+Want proof, check this [repo](https://github.com/KevKibe/Finetuning-WhisperSmall-LoRA-Swahili)
 
-  2. View your training run metrics on [Wandb](https://wandb.ai/).
 
-  3. Test your fine-tuned model using Gradio UI.
 
-  4. Deploy a REST API endpoint fro transcription of Audio files.
-
-  5. Containerize your REST API endpoint and push to DockerHub.
-</details>
+# 🚀 Getting Started
 
 ## Prerequisites
 
 - Sign up to HuggingFace and get your token keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens).
 
-- Sign up for wandb and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
+- Sign up to Weights and Biases and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
 
+- Demo video [here](https://youtu.be/qj48Chu4i4k?si=Vwv-6-qI7GJF7AMd)
 
-# A Guide to Usage on a Notebook
+[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/16r4cxP-dSFplRTfgPLbzGXYRzBIUqpx9?usp=sharing)
 
 ## Step 1: Installation
 
 ```python
 !pip install africanwhisper
 # If you're on Colab, restart the session due to issue with numpy installation on colab.
 ```
@@ -122,20 +104,20 @@
 ## Step 2: Set Parameters
 
 ```python
 # Set the parameters (refer to the 'Usage on VM' section for more details)
 huggingface_read_token = " "
 huggingface_write_token = " "
 dataset_name = "mozilla-foundation/common_voice_16_1" 
-language_abbr= " " # Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
-                    # Note: choose a small dataset so as to not run out of memory,
-model_id= "model-id" # Example openai/whisper-small, openai/whisper-medium
+language_abbr= " "                                    # Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
+                                                      # Note: choose a small dataset so as to not run out of memory,
+model_id= "model-id"                                  # Example openai/whisper-small, openai/whisper-medium
 processing_task= "automatic-speech-recognition" 
 wandb_api_key = " "
-use_peft = True  # Note: PEFT only works on a notebook with GPU-support.
+use_peft = True                                       # Note: PEFT only works on a notebook with GPU-support.
 
 ```
 
 ## Step 3: Prepare the Model
 ```python
 from training.data_prep import DataPrep
 
@@ -178,15 +160,15 @@
     tokenizer,
     language_abbr,
     wandb_api_key,
     use_peft
 )
 trainer.train(
     max_steps=100,
-    learning_rate=1e-5,
+    learning_rate=1e-3,
     per_device_train_batch_size=96,
     per_device_eval_batch_size=64,
     optim="adamw_bnb_8bit"
 )
 
 # Optional parameters for training:
 #     max_steps (int): The maximum number of training steps (default is 100).
@@ -198,132 +180,121 @@
 ```
 
 ## Step 6: Generate a Demo using GradioUI
 ```python
 from training.gradio_inference import WhisperDemo
 
 # Generate a demo
-model_name = "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
+model_name = "your-finetuned-model-name-on-huggingface-hub"     # e.g., "KevinKibe/whisper-small-af"
 demo = WhisperDemo(model_name, huggingface_read_token)
 demo.generate_demo()
 ```
 
 ## Step 7: Test Model using Audio File
 
 ```python
 from deployment.speech_inference import SpeechInference
 
-model_name = "your-finetuned-model-name-on-huggingface-hub"  # e.g., "KevinKibe/whisper-small-af"
+model_name = "your-finetuned-model-name-on-huggingface-hub"   # e.g., "KevinKibe/whisper-small-af"
 huggingface_read_token = " "
-task = "desired-task"  # either 'translate' or 'transcribe'
-audiofile_dir = "location-of-audio-file"  # filetype should be .mp3 or .wav
+task = "desired-task"                                         # either 'translate' or 'transcribe'
+audiofile_dir = "location-of-audio-file"                      # filetype should be .mp3 or .wav
 
 # Initialize the SpeechInference class and run inference
 inference = SpeechInference(model_name, huggingface_read_token)
 pipeline = inference.pipe_initialization()
 transcription = inference.output(pipeline, audiofile_dir, task)
 
 # Access different parts of the output
-print(transcription.text)  # The entire text transcription.
-print(transcription.chunks)  # List of individual text chunks with timestamps.
-print(transcription.timestamps)  # List of timestamps for each chunk.
-print(transcription.chunk_texts)  # List of texts for each chunk.
+print(transcription.text)                                       # The entire text transcription.
+print(transcription.chunks)                                     # List of individual text chunks with timestamps.
+print(transcription.timestamps)                                 # List of timestamps for each chunk.
+print(transcription.chunk_texts)                                # List of texts for each chunk.
 
 ```
 
-## Usage on a Virtual Machine
-
-<details>
-
-  - Clone the Repository: Clone or download the application code to your local machine.
-  ```
-  git clone https://github.com/KevKibe/African-Whisper.git
-  ```
+# 🖥️ Using the CLI
 
-  - Create a virtual environment for the project and activate it.
-  ```
-  python3 -m venv env
-  source venv/bin/activate
-  ```
-
-  - Install dependencies by running this command
-  ```
-  pip install -r requirements.txt
-  ```
-  - Navigate to:
-  ```
-  cd src
-  ```
-
-  - To start the training , use the following command:
-  ```
-  python -m training.main \
-      --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \
-      --huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \
-      --dataset_name DATASET_NAME \
-      --language_abbr LANGUAGE_ABBREVIATION \
-      --model_id MODEL_ID \
-      --processing_task PROCESSING_TASK \
-      --wandb_api_key YOUR_WANDB_API_KEY_HERE \
-      --use_peft 
-  ```
-  Here's a short description of each argument used in the command:
-
-  - **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
+- Clone the Repository: Clone or download the application code to your local machine.
+```bash
+git clone https://github.com/KevKibe/African-Whisper.git
+```
 
-  - **--huggingface_push_token**: Your Hugging Face authentication token for write access. It's used for uploading models to your Hugging Face account.
+- Create a virtual environment for the project and activate it.
+```bash
+python3 -m venv env
+source venv/bin/activate
+```
 
-  - **--dataset_name**: The name of the dataset you wish to use for training. Example: 'mozilla-foundation/common_voice_16_1'. This should match the dataset's identifier on the Hugging Face Datasets Hub.
+- Install dependencies by running this command
+```bash
+pip install -r requirements.txt
+```
+- Navigate to:
+```bash
+cd src
+```
 
-  - **--language_abbr**: The abbreviation of the language for the dataset you're using. Example: 'sw' for Swahili. This is used to specify the language variant of the dataset if it supports multiple languages.
+- To start the training , use the following command:
+```bash
+python -m training.main --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE --huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name AUDIO_DATASET_NAME --language_abbr LANGUAGE_ABBREVIATION --model_id MODEL_ID --processing_task PROCESSING_TASK --wandb_api_key YOUR_WANDB_API_KEY_HERE --use_peft # leave this out to opt-out of using PEFT
+```
+- Find a description of these commands [here](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/PARAMETERS.md).
 
-  - **--model_id**: Identifier for the pre-trained model you wish to fine-tune. Example: 'openai/whisper-small'. This should match the model's identifier on the Hugging Face Model Hub.
+### Inference
 
-  - **--processing_task**: Specifies the task for which the model is being trained. Example: 'transcribe'. This defines the objective of the model training, such as transcribing audio to text.
+- To get inference from your fine-tuned model, follow these steps:
 
-  - **--wandb_api_key**: Your Weights & Biases (W&B) API key. This is used for logging and tracking the training process if you're using W&B for experiment tracking.
+- Ensure that ffmpeg is installed by running the following commands:
 
-  - **--use_peft**: Add this flag to fine-tune using PEFT method and omit it to do full fine-tuning. PEFT only works on a notbeook with GPU-support.
+```bash
+# on Ubuntu or Debian
+sudo apt update && sudo apt install ffmpeg
 
-  ## Inference
+# on Arch Linux
+sudo pacman -S ffmpeg
 
-  - To get inference from your fine-tuned model, follow these steps:
+# on MacOS using Homebrew (https://brew.sh/)
+brew install ffmpeg
 
-  - Ensure that ffmpeg is installed by running the following commands:
-  ```
-  # on Ubuntu or Debian
-  sudo apt update && sudo apt install ffmpeg
+# on Windows using Chocolatey (https://chocolatey.org/)
+choco install ffmpeg
 
-  # on Arch Linux
-  sudo pacman -S ffmpeg
+# on Windows using Scoop (https://scoop.sh/)
+scoop install ffmpeg
+```
 
-  # on MacOS using Homebrew (https://brew.sh/)
-  brew install ffmpeg
+- To get the Gradio inference URL:
+```bash
+python -m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE 
+```
+- **--model_name**: Name of the fine-tuned model to use in your huggingfacehub repo. This should match the model's identifier on the Hugging Face Model Hub.
+- **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
 
-  # on Windows using Chocolatey (https://chocolatey.org/)
-  choco install ffmpeg
+- To launch the REST API endpoint locally:
 
-  # on Windows using Scoop (https://scoop.sh/)
-  scoop install ffmpeg
-  ```
+```bash
+cd src/deployment
+```
+- Create a `.env` file using `nano .env` command and add these keys and save the file.
+```python
+MODEL_NAME = "your-finetuned-model"
+HUGGINGFACE_READ_TOKEN = "huggingface-read-token"
+```
 
-  - To get the Gradio inference URL:
-  ```
-  python -m training.gradio_demo \
-      --model_name YOUR_FINETUNED-MODEL \
-      --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \
-  ```
-  - **--model_name**: Name of the fine-tuned model to use in your huggingfacehub repo. This should match the model's identifier on the Hugging Face Model Hub.
-  - **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
+- Run this command to launch the endpoint:
+```bash
+uvicorn main:app --host 0.0.0.0 --port 8000
+```
 
-</details>
+- Test it out by accessing the Swagger UI at `http://localhost:8000/docs` and uploading either an .mp3 file or a .wav file and a task either `transcribe` or `translate`. Alternatively, you can use Postman with the URL `http://localhost:8000/speechinference`.
 
-## Deployment
+## 🛳️ Deployment
 
-- To deploy your fine-tuned model (assuming it's on Hugging Face Hub) as a REST API endpoint, follow this [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
+- To deploy your fine-tuned model (assuming it's on Hugging Face Hub) as a REST API endpoint, follow these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
 
 
 ## Contributing 
 Contributions are welcome and encouraged.
 
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
```

#### html2text {}

```diff
@@ -1,83 +1,76 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.3.0 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.4.0 Summary: A package
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
-probability==0.24.0 Requires-Dist: yt-dlp==2023.11.14
+probability==0.24.0 Requires-Dist: yt-dlp==2023.11.14 Requires-Dist: python-
+dotenv==1.0.1 Requires-Dist: logging==0.4.9.6
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
-# Description African Whisper is an open-source project aimed at enhancing
-Automatic Speech Recognition (ASR): translation and transcription capabilities
-for African languages. This is done by developing a package to allow seamless
-fine-tuning and deployment of the Whisper ASR model developed by OpenAI to
-better recognize and transcribe African languages for all developers. ## Why
-Whisper? Whisper is an open-source Automatic Speech Recognition (ASR) system
-developed by OpenAI.
-Hereâs why Whisper stands out: - **Extensive Training Data**: Trained on
-680,000 hours of multilingual and multitask(translation and transcription)
-supervised data from the web. - **Sequence-based Understanding**: Unlike
-Word2Vec, which lacks sequential context, Whisper considers the full sequence
-of spoken words, ensuring accurate context and nuance recognition. -
-**Simplification for Developers**: Using Whisper, developers can deploy one
-model for transcribing a multitude of languages, including underrepresented
-ones, without sacrificing quality or context. For more details, you can refer
-to the [Whisper ASR model paper](https://cdn.openai.com/papers/whisper.pdf). ##
-Proof of Concept A successful proof of concept has been achieved by fine-tuning
-the Whisper-small model using a Google Colab Notebook and tested on an
-audiofile to test the performance. The results were promising, indicating the
-potential of this approach for ASR in African languages. You can explore the
-process and results in detail in the [repository](https://github.com/KevKibe/
-Finetuning-WhisperSmall-LoRA-Swahili) ## Objectives To develop a quick-to-use
-fine-tuning and deployment pipeline utilizing audio datasets by the [Mozilla
-Foundation](https://commonvoice.mozilla.org/en), eventually having Automatic
-Speech Recognition (ASR) for African languages just as good as other non-
-African languages. ## Features 1. Fine-tune a version of [whisper](https://
-huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013) on
-any dataset from [Mozilla's](https://huggingface.co/mozilla-foundation) Common
-Voice datasets. 2. View your training run metrics on [Wandb](https://wandb.ai/
-). 3. Test your fine-tuned model using Gradio UI. 4. Deploy a REST API endpoint
-fro transcription of Audio files. 5. Containerize your REST API endpoint and
-push to DockerHub. ## Prerequisites - Sign up to HuggingFace and get your token
-keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens). -
-Sign up for wandb and get your token keys use this [guide](https://
-app.wandb.ai/login?signup=true) # A Guide to Usage on a Notebook ## Step 1:
-Installation ```python !pip install africanwhisper # If you're on Colab,
-restart the session due to issue with numpy installation on colab. ``` ## Step
-2: Set Parameters ```python # Set the parameters (refer to the 'Usage on VM'
-section for more details) huggingface_read_token = " " huggingface_write_token
-= " " dataset_name = "mozilla-foundation/common_voice_16_1" language_abbr= " "
-# Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/
-mozilla-foundation/common_voice_16_1. # Note: choose a small dataset so as to
-not run out of memory, model_id= "model-id" # Example openai/whisper-small,
-openai/whisper-medium processing_task= "automatic-speech-recognition"
-wandb_api_key = " " use_peft = True # Note: PEFT only works on a notebook with
-GPU-support. ``` ## Step 3: Prepare the Model ```python from training.data_prep
-import DataPrep # Initialize the DataPrep class and prepare the model process =
-DataPrep( huggingface_read_token, dataset_name, language_abbr, model_id,
-processing_task, use_peft ) tokenizer, feature_extractor, feature_processor,
-model = process.prepare_model() ``` ## Step 4: Preprocess the Dataset ```python
-# Load and preprocess the dataset processed_dataset = process.load_dataset
-( feature_extractor=feature_extractor, tokenizer=tokenizer,
-processor=feature_processor ) ``` ## Step 5: Train the Model ```python from
-training.model_trainer import Trainer # Initialize the Trainer class and train
-the model trainer = Trainer( huggingface_write_token, model_id,
-processed_dataset, model, feature_processor, feature_extractor, tokenizer,
-language_abbr, wandb_api_key, use_peft ) trainer.train( max_steps=100,
-learning_rate=1e-5, per_device_train_batch_size=96,
+*Enhancing Automatic Speech Recognition (ASR): translation and transcription
+capabilities for African languages by providing seamless fine-tuning and
+deploying pipelines for Whisper Model*.
+![Diagram](diagram-1.png) ## Features - ð§ Fine-tune the [Whisper](https://
+huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013)
+model on any audio dataset from Huggingface, e.g., [Mozilla's](https://
+huggingface.co/mozilla-foundation) Common Voice datasets. - ð View training
+run metrics on [Wandb](https://wandb.ai/). - ðï¸ Test your fine-tuned model
+using Gradio UI or directly on an audio file (.mp3 or .wav). - ð Deploy an
+API endpoint for audio file transcription or translation. - ð³ Containerize
+your API endpoint application and push to DockerHub. ## Why Whisper? ð¤ -
+ð **Extensive Training Data**: Trained on 680,000 hours of multilingual and
+multitask(translation and transcription) supervised data from the web. -
+ð£ï¸ **Sequence-based Understanding**: Whisper considers the full sequence
+of spoken words, ensuring accurate context recognition, unlike Word2Vec. - ð»
+**Simplification for Applications**: Deploy one model for transcribing and
+translating a multitude of languages, without sacrificing quality or context.
+For more details, you can refer to the [Whisper ASR model paper](https://
+cdn.openai.com/papers/whisper.pdf).
+Want proof, check this [repo](https://github.com/KevKibe/Finetuning-
+WhisperSmall-LoRA-Swahili) # ð Getting Started ## Prerequisites - Sign up to
+HuggingFace and get your token keys use this [guide](https://huggingface.co/
+docs/hub/en/security-tokens). - Sign up to Weights and Biases and get your
+token keys use this [guide](https://app.wandb.ai/login?signup=true) - Demo
+video [here](https://youtu.be/qj48Chu4i4k?si=Vwv-6-qI7GJF7AMd) [![Colab](https:
+//colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/16r4cxP-dSFplRTfgPLbzGXYRzBIUqpx9?usp=sharing)
+## Step 1: Installation ```python !pip install africanwhisper # If you're on
+Colab, restart the session due to issue with numpy installation on colab. ```
+## Step 2: Set Parameters ```python # Set the parameters (refer to the 'Usage
+on VM' section for more details) huggingface_read_token = " "
+huggingface_write_token = " " dataset_name = "mozilla-foundation/
+common_voice_16_1" language_abbr= " " # Example 'af', 'sw'. see abbreviations
+here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. #
+Note: choose a small dataset so as to not run out of memory, model_id= "model-
+id" # Example openai/whisper-small, openai/whisper-medium processing_task=
+"automatic-speech-recognition" wandb_api_key = " " use_peft = True # Note: PEFT
+only works on a notebook with GPU-support. ``` ## Step 3: Prepare the Model
+```python from training.data_prep import DataPrep # Initialize the DataPrep
+class and prepare the model process = DataPrep( huggingface_read_token,
+dataset_name, language_abbr, model_id, processing_task, use_peft ) tokenizer,
+feature_extractor, feature_processor, model = process.prepare_model() ``` ##
+Step 4: Preprocess the Dataset ```python # Load and preprocess the dataset
+processed_dataset = process.load_dataset( feature_extractor=feature_extractor,
+tokenizer=tokenizer, processor=feature_processor ) ``` ## Step 5: Train the
+Model ```python from training.model_trainer import Trainer # Initialize the
+Trainer class and train the model trainer = Trainer( huggingface_write_token,
+model_id, processed_dataset, model, feature_processor, feature_extractor,
+tokenizer, language_abbr, wandb_api_key, use_peft ) trainer.train
+( max_steps=100, learning_rate=1e-3, per_device_train_batch_size=96,
 per_device_eval_batch_size=64, optim="adamw_bnb_8bit" ) # Optional parameters
 for training: # max_steps (int): The maximum number of training steps (default
 is 100). # learning_rate (float): The learning rate for training (default is
 1e-5). # per_device_train_batch_size (int): The batch size per GPU for training
 (default is 96). # per_device_eval_batch_size (int): The batch size per GPU for
 evaluation (default is 64). # optim (str): The optimizer used for training
 (default is "adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI
@@ -92,62 +85,54 @@
 or .wav # Initialize the SpeechInference class and run inference inference =
 SpeechInference(model_name, huggingface_read_token) pipeline =
 inference.pipe_initialization() transcription = inference.output(pipeline,
 audiofile_dir, task) # Access different parts of the output print
 (transcription.text) # The entire text transcription. print
 (transcription.chunks) # List of individual text chunks with timestamps. print
 (transcription.timestamps) # List of timestamps for each chunk. print
-(transcription.chunk_texts) # List of texts for each chunk. ``` ## Usage on a
-Virtual Machine - Clone the Repository: Clone or download the application code
-to your local machine. ``` git clone https://github.com/KevKibe/African-
-Whisper.git ``` - Create a virtual environment for the project and activate it.
-``` python3 -m venv env source venv/bin/activate ``` - Install dependencies by
-running this command ``` pip install -r requirements.txt ``` - Navigate to: ```
-cd src ``` - To start the training , use the following command: ``` python -
-m training.main \ --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \
---huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \ --dataset_name
-DATASET_NAME \ --language_abbr LANGUAGE_ABBREVIATION \ --model_id MODEL_ID \ --
-processing_task PROCESSING_TASK \ --wandb_api_key YOUR_WANDB_API_KEY_HERE \ --
-use_peft ``` Here's a short description of each argument used in the command: -
-**--huggingface_read_token**: Your Hugging Face authentication token for read
-access. It allows you to download datasets and models from Hugging Face. - **--
-huggingface_push_token**: Your Hugging Face authentication token for write
-access. It's used for uploading models to your Hugging Face account. - **--
-dataset_name**: The name of the dataset you wish to use for training. Example:
-'mozilla-foundation/common_voice_16_1'. This should match the dataset's
-identifier on the Hugging Face Datasets Hub. - **--language_abbr**: The
-abbreviation of the language for the dataset you're using. Example: 'sw' for
-Swahili. This is used to specify the language variant of the dataset if it
-supports multiple languages. - **--model_id**: Identifier for the pre-trained
-model you wish to fine-tune. Example: 'openai/whisper-small'. This should match
-the model's identifier on the Hugging Face Model Hub. - **--processing_task**:
-Specifies the task for which the model is being trained. Example: 'transcribe'.
-This defines the objective of the model training, such as transcribing audio to
-text. - **--wandb_api_key**: Your Weights & Biases (W&B) API key. This is used
-for logging and tracking the training process if you're using W&B for
-experiment tracking. - **--use_peft**: Add this flag to fine-tune using PEFT
-method and omit it to do full fine-tuning. PEFT only works on a notbeook with
-GPU-support. ## Inference - To get inference from your fine-tuned model, follow
-these steps: - Ensure that ffmpeg is installed by running the following
-commands: ``` # on Ubuntu or Debian sudo apt update && sudo apt install ffmpeg
-# on Arch Linux sudo pacman -S ffmpeg # on MacOS using Homebrew (https://
-brew.sh/) brew install ffmpeg # on Windows using Chocolatey (https://
-chocolatey.org/) choco install ffmpeg # on Windows using Scoop (https://
-scoop.sh/) scoop install ffmpeg ``` - To get the Gradio inference URL: ```
-python -m training.gradio_demo \ --model_name YOUR_FINETUNED-MODEL \ --
-huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \ ``` - **--
+(transcription.chunk_texts) # List of texts for each chunk. ``` # ð¥ï¸ Using
+the CLI - Clone the Repository: Clone or download the application code to your
+local machine. ```bash git clone https://github.com/KevKibe/African-Whisper.git
+``` - Create a virtual environment for the project and activate it. ```bash
+python3 -m venv env source venv/bin/activate ``` - Install dependencies by
+running this command ```bash pip install -r requirements.txt ``` - Navigate to:
+```bash cd src ``` - To start the training , use the following command: ```bash
+python -m training.main --huggingface_read_token
+YOUR_HUGGING_FACE_READ_TOKEN_HERE --huggingface_write_token
+YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name AUDIO_DATASET_NAME --
+language_abbr LANGUAGE_ABBREVIATION --model_id MODEL_ID --processing_task
+PROCESSING_TASK --wandb_api_key YOUR_WANDB_API_KEY_HERE --use_peft # leave this
+out to opt-out of using PEFT ``` - Find a description of these commands [here]
+(https://github.com/KevKibe/African-Whisper/blob/master/DOCS/PARAMETERS.md).
+### Inference - To get inference from your fine-tuned model, follow these
+steps: - Ensure that ffmpeg is installed by running the following commands:
+```bash # on Ubuntu or Debian sudo apt update && sudo apt install ffmpeg # on
+Arch Linux sudo pacman -S ffmpeg # on MacOS using Homebrew (https://brew.sh/
+) brew install ffmpeg # on Windows using Chocolatey (https://chocolatey.org/
+) choco install ffmpeg # on Windows using Scoop (https://scoop.sh/) scoop
+install ffmpeg ``` - To get the Gradio inference URL: ```bash python -
+m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --
+huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE ``` - **--
 model_name**: Name of the fine-tuned model to use in your huggingfacehub repo.
 This should match the model's identifier on the Hugging Face Model Hub. - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
-access. It allows you to download datasets and models from Hugging Face. ##
-Deployment - To deploy your fine-tuned model (assuming it's on Hugging Face
-Hub) as a REST API endpoint, follow this [instructions](https://github.com/
-KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ## Contributing
-Contributions are welcome and encouraged. Before contributing, please take a
-moment to review our [Contribution Guidelines](https://github.com/KevKibe/
-African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for important information on
-how to contribute to this project. If you're unsure about anything or need
-assistance, don't hesitate to reach out to us or open an issue to discuss your
-ideas. We look forward to your contributions! ## License This project is
-licensed under the MIT License - see the [LICENSE](https://github.com/KevKibe/
-African-Whisper/blob/main/LICENSE) file for details. ## Contact For any
-enquiries, please reach out to me through keviinkibe@gmail.com
+access. It allows you to download datasets and models from Hugging Face. - To
+launch the REST API endpoint locally: ```bash cd src/deployment ``` - Create a
+`.env` file using `nano .env` command and add these keys and save the file.
+```python MODEL_NAME = "your-finetuned-model" HUGGINGFACE_READ_TOKEN =
+"huggingface-read-token" ``` - Run this command to launch the endpoint: ```bash
+uvicorn main:app --host 0.0.0.0 --port 8000 ``` - Test it out by accessing the
+Swagger UI at `http://localhost:8000/docs` and uploading either an .mp3 file or
+a .wav file and a task either `transcribe` or `translate`. Alternatively, you
+can use Postman with the URL `http://localhost:8000/speechinference`. ##
+ð³ï¸ Deployment - To deploy your fine-tuned model (assuming it's on Hugging
+Face Hub) as a REST API endpoint, follow these [instructions](https://
+github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ##
+Contributing Contributions are welcome and encouraged. Before contributing,
+please take a moment to review our [Contribution Guidelines](https://
+github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for
+important information on how to contribute to this project. If you're unsure
+about anything or need assistance, don't hesitate to reach out to us or open an
+issue to discuss your ideas. We look forward to your contributions! ## License
+This project is licensed under the MIT License - see the [LICENSE](https://
+github.com/KevKibe/African-Whisper/blob/main/LICENSE) file for details. ##
+Contact For any enquiries, please reach out to me through keviinkibe@gmail.com
```

### Comparing `africanwhisper-0.3.0/src/africanwhisper.egg-info/SOURCES.txt` & `africanwhisper-0.4.0/src/africanwhisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.3.0/src/deployment/speech_inference.py` & `africanwhisper-0.4.0/src/deployment/speech_inference.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from transformers import pipeline, AutomaticSpeechRecognitionPipeline
+from transformers import pipeline, AutomaticSpeechRecognitionPipeline, AutoModelForSpeechSeq2Seq, AutoProcessor
 from typing import List, Tuple, Any, Dict
 from pydantic import BaseModel, Field
 
 
 
 class Chunk(BaseModel):
     """
@@ -63,24 +63,28 @@
         Returns:
             Any: The initialized pipeline object.
         """
         if input is None:
             print("No audio file submitted! Please upload or record an audio file before submitting your request.")
         else:
             device = 0 if torch.cuda.is_available() else "cpu"
-            if torch.cuda.is_available() and torch.cuda.is_bf16_supported():
-                dtype = torch.bfloat16
-            else:
-                dtype = None
+            torch_dtype = torch.float16 if torch.cuda.is_available() else torch.float32
+        model = AutoModelForSpeechSeq2Seq.from_pretrained(
+        self.model_name , torch_dtype=torch_dtype, low_cpu_mem_usage=True, use_safetensors=True
+        )
+        model.to(device)
+        processor = AutoProcessor.from_pretrained(self.model_name)
         pipe = pipeline(
-                            task="automatic-speech-recognition",
-                            model=self.model_name,
-                            token=self.huggingface_read_token,
-                            device=device,
-                            torch_dtype=dtype
+                        task="automatic-speech-recognition",
+                        model=model,
+                        tokenizer=processor.tokenizer,
+                        feature_extractor=processor.feature_extractor,
+                        token=self.huggingface_read_token,
+                        device=device,
+                        torch_dtype=torch_dtype
                         )
         return pipe
     
     def output(self, pipe: AutomaticSpeechRecognitionPipeline, input: Any, task: str) -> Dict:
         """
         Perform speech transcription.
 
@@ -95,14 +99,14 @@
         transcription = pipe(
                 input,
                 chunk_length_s=30,
                 batch_size=24,
                 return_timestamps=True,
                 generate_kwargs={"task": task}
             )
-        transcription = Transcription(**transcription)
+        # transcription = Transcription(**transcription)
         return transcription
```

### Comparing `africanwhisper-0.3.0/src/tests/test_dataset.py` & `africanwhisper-0.4.0/src/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.3.0/src/training/audio_data_processor.py` & `africanwhisper-0.4.0/src/training/audio_data_processor.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.3.0/src/training/collator.py` & `africanwhisper-0.4.0/src/training/collator.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.3.0/src/training/data_prep.py` & `africanwhisper-0.4.0/src/training/data_prep.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.3.0/src/training/evaluation.py` & `africanwhisper-0.4.0/src/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.3.0/src/training/gradio_demo.py` & `africanwhisper-0.4.0/src/training/gradio_demo.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.3.0/src/training/gradio_inference.py` & `africanwhisper-0.4.0/src/training/gradio_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.3.0/src/training/load_data.py` & `africanwhisper-0.4.0/src/training/load_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from datasets import load_dataset, DatasetDict, IterableDataset
 import warnings
+from typing import List
 
 warnings.filterwarnings("ignore")
 
 class Dataset:
     """
     Manages loading of the datasets from Hugging Face's Common Voice repository.
 
     Attributes:
         huggingface_token (str): Hugging Face API token for read authenticated access.
         dataset_name (str): Name of the dataset to be downloaded from Hugging Face.
         language_abbr (str): Abbreviation of the language for the dataset.
     """
 
-    def __init__(self, huggingface_token: str, dataset_name: str, language_abbr: str):
+    def __init__(self, huggingface_token: str, dataset_name: str, language_abbr: List[str]):
         """
         Initializes the DatasetManager with necessary details for dataset operations.
 
         Parameters:
             huggingface_token (str): Hugging Face API token.
             dataset_name (str): Name of the dataset.
             language_abbr (str): Language abbreviation for the dataset.
```

### Comparing `africanwhisper-0.3.0/src/training/main.py` & `africanwhisper-0.4.0/src/training/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.3.0/src/training/model_trainer.py` & `africanwhisper-0.4.0/src/training/model_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         # Set fp16 to True/False based on GPU availability
         fp16 = use_gpu
 
         data_collator = DataCollatorSpeechSeq2SeqWithPadding(
             processor=self.feature_processor
         )
         training_args = Seq2SeqTrainingArguments(
-            output_dir=f"./{self.model_id}-{self.language_abbr}",
+            output_dir=f"../{self.model_id}-{self.language_abbr}",
             per_device_train_batch_size=per_device_train_batch_size,
             gradient_accumulation_steps=1,
             learning_rate=learning_rate,
             max_steps=max_steps,
             gradient_checkpointing=True,
             fp16=fp16,
             optim=optim,
@@ -176,15 +176,19 @@
             tokenizer=self.feature_processor.feature_extractor,
             callbacks=[ShuffleCallback()],
         )
 
         model_prep = WhisperModelPrep(
             self.model_id, self.language_abbr, "transcribe", self.use_peft
         )
+
         tokenizer = model_prep.initialize_tokenizer()
+        processor = model_prep.initialize_processor()
         tokenizer.save_pretrained(training_args.output_dir)
-
+        processor.save_pretrained(training_args.output_dir)
+        torch.save(self.model.state_dict(), f"{training_args.output_dir}/pytorch_model.bin")
+        self.model.save_pretrained(training_args.output_dir)
         progress_callback = WandbProgressResultsCallback(
             trainer, eval_dataset, tokenizer
         )
         trainer.add_callback(progress_callback)
         trainer.train()
```

### Comparing `africanwhisper-0.3.0/src/training/wandb_callback.py` & `africanwhisper-0.4.0/src/training/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.3.0/src/training/whisper_model_prep.py` & `africanwhisper-0.4.0/src/training/whisper_model_prep.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,27 +46,27 @@
 
         Returns
         -------
             WhisperFeatureExtractor: Configured feature extractor for the model.
 
         """
         return WhisperFeatureExtractor.from_pretrained(
-            self.model_id, cache_dir=f"./{self.language_abbr}/feature-extractor"
+            self.model_id
         )
 
     def initialize_tokenizer(self) -> WhisperTokenizer:
         """Creates and retrieves a tokenizer for the Whisper model.
 
         Returns
         -------
             WhisperTokenizer: Configured tokenizer for the model.
 
         """
         return WhisperTokenizer.from_pretrained(
-            self.model_id, cache_dir=f"./{self.language_abbr}/tokenizer"
+            self.model_id
         )
 
     def initialize_processor(self) -> WhisperProcessor:
         """Combines the feature extractor and tokenizer to create a processor for the Whisper model,
         facilitating seamless data preparation.
 
         Returns
@@ -90,36 +90,36 @@
             WhisperForConditionalGeneration: The configured Whisper model ready for conditional generation tasks.
 
         """
 
         if self.use_peft:
             model = WhisperForConditionalGeneration.from_pretrained(
                 self.model_id,
-                cache_dir=f"./{self.language_abbr}/model",
+                # cache_dir="./whisper-model/model",
                 load_in_8bit=True,
                 device_map="auto",
             )
             model.config.forced_decoder_ids = None
             model.config.suppress_tokens = []
             model.generation_config.language = "en"
-            model.generation_config.task = "transcribe"
+            model.generation_config.task = "translate"
             model = prepare_model_for_kbit_training(model)
             config = LoraConfig(
                 r=32,
                 lora_alpha=64,
                 target_modules=["q_proj", "v_proj"],
                 lora_dropout=0.05,
                 bias="none",
             )
             model = get_peft_model(model, config)
             model.print_trainable_parameters()
         else:
             print("PEFT optimization is not enabled.")
             model = WhisperForConditionalGeneration.from_pretrained(
-                self.model_id, cache_dir=f"./{self.language_abbr}/model"
+                self.model_id
             )
             model.config.forced_decoder_ids = None
             model.config.suppress_tokens = []
             model.generation_config.language = "en"
-            model.generation_config.task = "transcribe"
+            model.generation_config.task = "translate"
 
-        return model
+        return model
```

