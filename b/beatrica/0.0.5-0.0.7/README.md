# Comparing `tmp/beatrica-0.0.5.tar.gz` & `tmp/beatrica-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beatrica-0.0.5.tar", last modified: Thu Apr 11 10:20:07 2024, max compression
+gzip compressed data, was "beatrica-0.0.7.tar", last modified: Thu Apr 11 10:25:06 2024, max compression
```

## Comparing `beatrica-0.0.5.tar` & `beatrica-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:20:07.510657 beatrica-0.0.5/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    34523 2024-01-31 16:51:58.000000 beatrica-0.0.5/LICENSE
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    13013 2024-04-11 10:20:07.510457 beatrica-0.0.5/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    12484 2024-04-11 09:39:23.000000 beatrica-0.0.5/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:20:07.508710 beatrica-0.0.5/beatrica/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.5/beatrica/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     8472 2024-04-11 09:39:23.000000 beatrica-0.0.5/beatrica/beatrica.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1641 2024-04-11 09:39:23.000000 beatrica-0.0.5/beatrica/prompts.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:20:07.509724 beatrica-0.0.5/beatrica.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    13013 2024-04-11 10:20:07.000000 beatrica-0.0.5/beatrica.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      323 2024-04-11 10:20:07.000000 beatrica-0.0.5/beatrica.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-11 10:20:07.000000 beatrica-0.0.5/beatrica.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       52 2024-04-11 10:20:07.000000 beatrica-0.0.5/beatrica.egg-info/entry_points.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      236 2024-04-11 10:20:07.000000 beatrica-0.0.5/beatrica.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       15 2024-04-11 10:20:07.000000 beatrica-0.0.5/beatrica.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-11 10:20:07.510719 beatrica-0.0.5/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1337 2024-04-11 10:20:02.000000 beatrica-0.0.5/setup.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:20:07.510006 beatrica-0.0.5/tests/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.5/tests/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1074 2024-04-11 09:39:23.000000 beatrica-0.0.5/tests/test_beatrica.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:25:06.232389 beatrica-0.0.7/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    34523 2024-01-31 16:51:58.000000 beatrica-0.0.7/LICENSE
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    14312 2024-04-11 10:25:06.232161 beatrica-0.0.7/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    13783 2024-04-11 10:25:00.000000 beatrica-0.0.7/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:25:06.230768 beatrica-0.0.7/beatrica/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.7/beatrica/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     8472 2024-04-11 09:39:23.000000 beatrica-0.0.7/beatrica/beatrica.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1641 2024-04-11 09:39:23.000000 beatrica-0.0.7/beatrica/prompts.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:25:06.231640 beatrica-0.0.7/beatrica.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    14312 2024-04-11 10:25:06.000000 beatrica-0.0.7/beatrica.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      323 2024-04-11 10:25:06.000000 beatrica-0.0.7/beatrica.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-11 10:25:06.000000 beatrica-0.0.7/beatrica.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       52 2024-04-11 10:25:06.000000 beatrica-0.0.7/beatrica.egg-info/entry_points.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      236 2024-04-11 10:25:06.000000 beatrica-0.0.7/beatrica.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       15 2024-04-11 10:25:06.000000 beatrica-0.0.7/beatrica.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-11 10:25:06.232466 beatrica-0.0.7/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1337 2024-04-11 10:25:00.000000 beatrica-0.0.7/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:25:06.231865 beatrica-0.0.7/tests/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.7/tests/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1074 2024-04-11 09:39:23.000000 beatrica-0.0.7/tests/test_beatrica.py
```

### Comparing `beatrica-0.0.5/LICENSE` & `beatrica-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.5/PKG-INFO` & `beatrica-0.0.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: beatrica
-Version: 0.0.5
-Summary: Beatrica is a tool for code review automation using large language models.
-Home-page: https://github.com/chigwell/beatrica
-Author: Eugene Evstafev
-Author-email: chigwel@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 [![PyPI version](https://badge.fury.io/py/beatrica.svg)](https://badge.fury.io/py/beatrica)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
 [![Downloads](https://static.pepy.tech/badge/beatrica)](https://pepy.tech/project/beatrica)
 
 # Beatrica
 
 `beatrica` is an innovative Python package that utilizes Large Language Models (LLMs) such as OpenAI's GPT and MistralAI for automating code review processes. It provides insights by analyzing differences between the current active branch and a specified base branch, processing code changes, and generating reviews to improve code quality and collaboration.
@@ -26,14 +10,59 @@
 
 Integrate cutting-edge code review automation into your workflow by installing `beatrica` using pip:
 
 ```bash
 pip install beatrica
 ```
 
+Certainly! Here's how you can configure the API key for Beatrica via a parameter or environment variable:
+
+## Configuring the API Key
+
+For Beatrica to communicate with LLM services like OpenAI or MistralAI, an API key is required. You can provide this API key in two ways:
+
+### Using an Environment Variable
+
+Set the API key as an environment variable before running Beatrica. This method is recommended for keeping your API key secure and not directly visible in command line history.
+
+For Unix-like systems (Linux/macOS):
+
+```bash
+export LLM_API_KEY='your_api_key_here'
+```
+
+For Windows Command Prompt:
+
+```cmd
+set LLM_API_KEY=your_api_key_here
+```
+
+For Windows PowerShell:
+
+```powershell
+$env:LLM_API_KEY='your_api_key_here'
+```
+
+After setting the environment variable, you can run Beatrica without explicitly passing the API key in the command:
+
+```bash
+beatrica --base_branch=main --llm_type=openai
+```
+
+### Using the Command Line Argument
+
+If you prefer or need to, you can directly pass the API key as a command line argument. However, be mindful of security implications such as exposing your API key in shell history or logs.
+
+```bash
+beatrica --base_branch=main --llm_type=openai --api_key='your_api_key_here'
+```
+
+Choose the method that best suits your workflow and security practices.
+
+
 ## Usage
 
 Beatrica offers a CLI interface for specifying a base branch and comparing its differences with the current active branch, generating insightful reviews. Here are examples showcasing its usage with various configurations:
 
 ### Basic Usage
 
 To analyze code differences with the `main` branch using the default OpenAI's GPT-4 model, use:
```

### Comparing `beatrica-0.0.5/beatrica/beatrica.py` & `beatrica-0.0.7/beatrica/beatrica.py`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.5/beatrica/prompts.py` & `beatrica-0.0.7/beatrica/prompts.py`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.5/setup.py` & `beatrica-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='beatrica',
-    version='0.0.5',
+    version='0.0.7',
     author='Eugene Evstafev',
     author_email='chigwel@gmail.com',
     description="Beatrica is a tool for code review automation using large language models.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chigwell/beatrica',
     packages=find_packages(),
```

### Comparing `beatrica-0.0.5/tests/test_beatrica.py` & `beatrica-0.0.7/tests/test_beatrica.py`

 * *Files identical despite different names*

