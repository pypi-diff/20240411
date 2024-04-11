# Comparing `tmp/zrb_ollama-0.0.8.tar.gz` & `tmp/zrb_ollama-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zrb_ollama-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "zrb_ollama-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `zrb_ollama-0.0.8.tar` & `zrb_ollama-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1076 2023-12-27 05:18:58.820525 zrb_ollama-0.0.8/.github/workflows/_zrb.yml
--rw-r--r--   0        0        0      218 2023-12-23 22:33:38.087576 zrb_ollama-0.0.8/.github/workflows/hello.yml
--rw-r--r--   0        0        0       43 2023-12-25 11:29:11.762417 zrb_ollama-0.0.8/.gitignore
--rw-r--r--   0        0        0        7 2023-12-23 22:33:38.067576 zrb_ollama-0.0.8/.python-version
--rw-r--r--   0        0        0    12405 2023-12-28 01:00:19.542018 zrb_ollama-0.0.8/README.md
--rw-r--r--   0        0        0      146 2023-12-23 22:35:18.024072 zrb_ollama-0.0.8/_cmd/activate-venv.sh
--rw-r--r--   0        0        0       85 2023-12-25 04:17:07.538434 zrb_ollama-0.0.8/_cmd/build.sh
--rw-r--r--   0        0        0       46 2023-12-25 04:15:50.325063 zrb_ollama-0.0.8/_cmd/install-symlink.sh
--rw-r--r--   0        0        0      193 2023-12-26 23:43:42.937240 zrb_ollama-0.0.8/_cmd/prepare-playground.sh
--rw-r--r--   0        0        0       57 2023-12-23 22:35:18.024072 zrb_ollama-0.0.8/_cmd/prepare-venv.sh
--rw-r--r--   0        0        0       63 2023-12-25 07:36:02.588418 zrb_ollama-0.0.8/_cmd/publish.sh
--rw-r--r--   0        0        0      140 2023-12-25 23:49:32.542509 zrb_ollama-0.0.8/_cmd/test-playground.sh
--rw-r--r--   0        0        0      126 2023-12-25 23:48:05.110338 zrb_ollama-0.0.8/playground-template/fibo.py
--rw-r--r--   0        0        0      451 2023-12-26 00:01:11.830013 zrb_ollama-0.0.8/playground-template/zrb_init.py
--rwxr-xr-x   0        0        0     1507 2023-12-23 22:33:38.067576 zrb_ollama-0.0.8/project.sh
--rw-r--r--   0        0        0      911 2023-12-28 00:40:39.865444 zrb_ollama-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      188 2023-12-25 11:53:13.401918 zrb_ollama-0.0.8/requirements.txt
--rw-r--r--   0        0        0      181 2023-12-25 10:35:18.939884 zrb_ollama-0.0.8/src/zrb_ollama/__init__.py
--rw-r--r--   0        0        0     4454 2023-12-28 00:30:16.446705 zrb_ollama-0.0.8/src/zrb_ollama/__main__.py
--rw-r--r--   0        0        0        0 2023-12-25 09:20:57.476721 zrb_ollama-0.0.8/src/zrb_ollama/builtin/__init__.py
--rw-r--r--   0        0        0      717 2023-12-27 06:21:15.359735 zrb_ollama-0.0.8/src/zrb_ollama/builtin/install.py
--rw-r--r--   0        0        0      288 2023-12-28 00:25:57.180314 zrb_ollama-0.0.8/src/zrb_ollama/config.py
--rw-r--r--   0        0        0       81 2023-12-25 09:24:16.315404 zrb_ollama-0.0.8/src/zrb_ollama/group.py
--rw-r--r--   0        0        0     8818 2023-12-27 23:25:49.484009 zrb_ollama-0.0.8/src/zrb_ollama/task/prompt_task.py
--rw-r--r--   0        0        0      118 2023-12-23 22:33:38.077576 zrb_ollama-0.0.8/template.env
--rw-r--r--   0        0        0     3417 2023-12-25 11:59:18.095672 zrb_ollama-0.0.8/zrb_init.py
--rw-r--r--   0        0        0    13048 1970-01-01 00:00:00.000000 zrb_ollama-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-12-27 05:18:58.820525 zrb_ollama-0.0.9/.github/workflows/_zrb.yml
+-rw-r--r--   0        0        0      218 2023-12-23 22:33:38.087576 zrb_ollama-0.0.9/.github/workflows/hello.yml
+-rw-r--r--   0        0        0       43 2023-12-25 11:29:11.762417 zrb_ollama-0.0.9/.gitignore
+-rw-r--r--   0        0        0        7 2023-12-23 22:33:38.067576 zrb_ollama-0.0.9/.python-version
+-rw-r--r--   0        0        0    12531 2023-12-28 01:11:00.605317 zrb_ollama-0.0.9/README.md
+-rw-r--r--   0        0        0      146 2023-12-23 22:35:18.024072 zrb_ollama-0.0.9/_cmd/activate-venv.sh
+-rw-r--r--   0        0        0       85 2023-12-25 04:17:07.538434 zrb_ollama-0.0.9/_cmd/build.sh
+-rw-r--r--   0        0        0       46 2023-12-25 04:15:50.325063 zrb_ollama-0.0.9/_cmd/install-symlink.sh
+-rw-r--r--   0        0        0      193 2023-12-26 23:43:42.937240 zrb_ollama-0.0.9/_cmd/prepare-playground.sh
+-rw-r--r--   0        0        0       57 2023-12-23 22:35:18.024072 zrb_ollama-0.0.9/_cmd/prepare-venv.sh
+-rw-r--r--   0        0        0       63 2023-12-25 07:36:02.588418 zrb_ollama-0.0.9/_cmd/publish.sh
+-rw-r--r--   0        0        0      140 2023-12-25 23:49:32.542509 zrb_ollama-0.0.9/_cmd/test-playground.sh
+-rw-r--r--   0        0        0      126 2023-12-25 23:48:05.110338 zrb_ollama-0.0.9/playground-template/fibo.py
+-rw-r--r--   0        0        0      451 2023-12-26 00:01:11.830013 zrb_ollama-0.0.9/playground-template/zrb_init.py
+-rwxr-xr-x   0        0        0     1507 2023-12-23 22:33:38.067576 zrb_ollama-0.0.9/project.sh
+-rw-r--r--   0        0        0      911 2023-12-28 01:11:15.805326 zrb_ollama-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      188 2023-12-25 11:53:13.401918 zrb_ollama-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      181 2023-12-25 10:35:18.939884 zrb_ollama-0.0.9/src/zrb_ollama/__init__.py
+-rw-r--r--   0        0        0     4454 2023-12-28 00:30:16.446705 zrb_ollama-0.0.9/src/zrb_ollama/__main__.py
+-rw-r--r--   0        0        0        0 2023-12-25 09:20:57.476721 zrb_ollama-0.0.9/src/zrb_ollama/builtin/__init__.py
+-rw-r--r--   0        0        0      717 2023-12-27 06:21:15.359735 zrb_ollama-0.0.9/src/zrb_ollama/builtin/install.py
+-rw-r--r--   0        0        0      288 2023-12-28 00:25:57.180314 zrb_ollama-0.0.9/src/zrb_ollama/config.py
+-rw-r--r--   0        0        0       81 2023-12-25 09:24:16.315404 zrb_ollama-0.0.9/src/zrb_ollama/group.py
+-rw-r--r--   0        0        0     8818 2023-12-27 23:25:49.484009 zrb_ollama-0.0.9/src/zrb_ollama/task/prompt_task.py
+-rw-r--r--   0        0        0      118 2023-12-23 22:33:38.077576 zrb_ollama-0.0.9/template.env
+-rw-r--r--   0        0        0     3417 2023-12-25 11:59:18.095672 zrb_ollama-0.0.9/zrb_init.py
+-rw-r--r--   0        0        0    13174 1970-01-01 00:00:00.000000 zrb_ollama-0.0.9/PKG-INFO
```

### Comparing `zrb_ollama-0.0.8/.github/workflows/_zrb.yml` & `zrb_ollama-0.0.9/.github/workflows/_zrb.yml`

 * *Files identical despite different names*

### Comparing `zrb_ollama-0.0.8/README.md` & `zrb_ollama-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 pip install zrb-ollama
 # From github
 pip install git+https://github.com/goFrendiAsgard/zrb-ollama.git@main
 # From directory
 pip install --use-feature=in-tree-build path/to/this/directory
 ```
 
+## Installing Ollama
+
+You can install Ollama by visiting the official website: [`https://ollama.ai/`](https://ollama.ai/).
+
 ## Talk to Zrb Ollama
 
 Once you install Zrb Ollama, you can then run it by invoking the following command:
 
 ```bash
 zrb-ollama "Why is the sky blue?"
 ```
@@ -168,17 +172,17 @@
 zrb chat "Can you make it better?"
 ```
 
 # Configuration
 
 You can configure Zrb Ollama using a few environment variables:
 
-- `ZRB_OLLAMA_BASE_URL`: Default Ollama base URL. if not specified, Zrb Ollama will use `http://localhost:11434`.
+- `ZRB_OLLAMA_BASE_URL`: Default Ollama base URL. If not specified, Zrb Ollama will use `http://localhost:11434`.
 - `ZRB_OLLAMA_DEFAULT_MODEL`: Default Ollama model. If not specified, Zrb Ollama will use `mistral`.
-- `ZRB_OLLAMA_VERBOSE_EVAL`: Whether `zrb-ollama-py` show the evaluate source code or not. If not specified, Zrb Ollama will set this to `0`
+- `ZRB_OLLAMA_VERBOSE_EVAL`: Whether `zrb-ollama-py` shows the evaluated source code or not. If not specified, Zrb Ollama will set this to `0`
 
 
 # For maintainers
 
 ## Publish to pypi
 
 To publish zrb-ollama, you need to have a `Pypi` account:
```

### Comparing `zrb_ollama-0.0.8/project.sh` & `zrb_ollama-0.0.9/project.sh`

 * *Files identical despite different names*

### Comparing `zrb_ollama-0.0.8/pyproject.toml` & `zrb_ollama-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "zrb-ollama"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="goFrendiAsgard", email="gofrendiasgard@gmail.com" },
 ]
 description = "Tasks related to ollama"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `zrb_ollama-0.0.8/src/zrb_ollama/__main__.py` & `zrb_ollama-0.0.9/src/zrb_ollama/__main__.py`

 * *Files identical despite different names*

### Comparing `zrb_ollama-0.0.8/src/zrb_ollama/builtin/install.py` & `zrb_ollama-0.0.9/src/zrb_ollama/builtin/install.py`

 * *Files identical despite different names*

### Comparing `zrb_ollama-0.0.8/src/zrb_ollama/task/prompt_task.py` & `zrb_ollama-0.0.9/src/zrb_ollama/task/prompt_task.py`

 * *Files identical despite different names*

### Comparing `zrb_ollama-0.0.8/zrb_init.py` & `zrb_ollama-0.0.9/zrb_init.py`

 * *Files identical despite different names*

### Comparing `zrb_ollama-0.0.8/PKG-INFO` & `zrb_ollama-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrb-ollama
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tasks related to ollama
 Author-email: goFrendiAsgard <gofrendiasgard@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,18 @@
 pip install zrb-ollama
 # From github
 pip install git+https://github.com/goFrendiAsgard/zrb-ollama.git@main
 # From directory
 pip install --use-feature=in-tree-build path/to/this/directory
 ```
 
+## Installing Ollama
+
+You can install Ollama by visiting the official website: [`https://ollama.ai/`](https://ollama.ai/).
+
 ## Talk to Zrb Ollama
 
 Once you install Zrb Ollama, you can then run it by invoking the following command:
 
 ```bash
 zrb-ollama "Why is the sky blue?"
 ```
@@ -185,17 +189,17 @@
 zrb chat "Can you make it better?"
 ```
 
 # Configuration
 
 You can configure Zrb Ollama using a few environment variables:
 
-- `ZRB_OLLAMA_BASE_URL`: Default Ollama base URL. if not specified, Zrb Ollama will use `http://localhost:11434`.
+- `ZRB_OLLAMA_BASE_URL`: Default Ollama base URL. If not specified, Zrb Ollama will use `http://localhost:11434`.
 - `ZRB_OLLAMA_DEFAULT_MODEL`: Default Ollama model. If not specified, Zrb Ollama will use `mistral`.
-- `ZRB_OLLAMA_VERBOSE_EVAL`: Whether `zrb-ollama-py` show the evaluate source code or not. If not specified, Zrb Ollama will set this to `0`
+- `ZRB_OLLAMA_VERBOSE_EVAL`: Whether `zrb-ollama-py` shows the evaluated source code or not. If not specified, Zrb Ollama will set this to `0`
 
 
 # For maintainers
 
 ## Publish to pypi
 
 To publish zrb-ollama, you need to have a `Pypi` account:
```

