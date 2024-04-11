# Comparing `tmp/oa-0.1.8.tar.gz` & `tmp/oa-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oa-0.1.8.tar", last modified: Mon Feb 26 16:17:29 2024, max compression
+gzip compressed data, was "oa-0.1.9.tar", last modified: Mon Feb 26 16:57:30 2024, max compression
```

## Comparing `oa-0.1.8.tar` & `oa-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:17:29.563957 oa-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-26 16:16:51.000000 oa-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-26 16:16:51.000000 oa-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-02-26 16:17:29.563957 oa-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17782 2024-02-26 16:16:51.000000 oa-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:17:29.559957 oa-0.1.8/oa/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-26 16:16:51.000000 oa-0.1.8/oa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-26 16:16:51.000000 oa-0.1.8/oa/ask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-02-26 16:17:01.000000 oa-0.1.8/oa/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:17:29.555957 oa-0.1.8/oa/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:17:29.555957 oa-0.1.8/oa/data/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:17:29.559957 oa-0.1.8/oa/data/templates/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-26 16:16:51.000000 oa-0.1.8/oa/data/templates/chatgpt/define_jargon.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-02-26 16:16:51.000000 oa-0.1.8/oa/data/templates/chatgpt/description_to_software_specs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-26 16:16:51.000000 oa-0.1.8/oa/data/templates/chatgpt/make_synopsis.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-02-26 16:16:51.000000 oa-0.1.8/oa/data/templates/chatgpt/simple_tests_for_code.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-02-26 16:16:51.000000 oa-0.1.8/oa/data/templates/chatgpt/specs_to_code_for_dag.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-26 16:16:51.000000 oa-0.1.8/oa/data/templates/chatgpt/suggest_names.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-02-26 16:16:51.000000 oa-0.1.8/oa/data/templates/chatgpt/user_story_to_code_for_dag.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:17:29.563957 oa-0.1.8/oa/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 16:16:51.000000 oa-0.1.8/oa/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-02-26 16:16:51.000000 oa-0.1.8/oa/examples/aesop_fables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-02-26 16:16:51.000000 oa-0.1.8/oa/examples/illustrate_stories.py
--rw-r--r--   0 runner    (1001) docker     (127)    15431 2024-02-26 16:17:02.000000 oa-0.1.8/oa/openai_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:17:29.563957 oa-0.1.8/oa/scrap/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:16:51.000000 oa-0.1.8/oa/scrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-02-26 16:17:02.000000 oa-0.1.8/oa/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-02-26 16:17:02.000000 oa-0.1.8/oa/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:17:29.559957 oa-0.1.8/oa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-02-26 16:17:29.000000 oa-0.1.8/oa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-02-26 16:17:29.000000 oa-0.1.8/oa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:17:29.000000 oa-0.1.8/oa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:17:29.000000 oa-0.1.8/oa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-26 16:17:29.000000 oa-0.1.8/oa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-26 16:17:29.000000 oa-0.1.8/oa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-26 16:17:29.563957 oa-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-26 16:16:51.000000 oa-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:57:30.788277 oa-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-26 16:56:52.000000 oa-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-26 16:56:52.000000 oa-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-02-26 16:57:30.788277 oa-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17782 2024-02-26 16:56:52.000000 oa-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:57:30.784277 oa-0.1.9/oa/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-26 16:56:52.000000 oa-0.1.9/oa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-26 16:56:52.000000 oa-0.1.9/oa/ask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-02-26 16:57:04.000000 oa-0.1.9/oa/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:57:30.784277 oa-0.1.9/oa/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:57:30.784277 oa-0.1.9/oa/data/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:57:30.784277 oa-0.1.9/oa/data/templates/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-26 16:56:52.000000 oa-0.1.9/oa/data/templates/chatgpt/define_jargon.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-02-26 16:56:52.000000 oa-0.1.9/oa/data/templates/chatgpt/description_to_software_specs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-26 16:56:52.000000 oa-0.1.9/oa/data/templates/chatgpt/make_synopsis.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-02-26 16:56:52.000000 oa-0.1.9/oa/data/templates/chatgpt/simple_tests_for_code.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-02-26 16:56:52.000000 oa-0.1.9/oa/data/templates/chatgpt/specs_to_code_for_dag.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-26 16:56:52.000000 oa-0.1.9/oa/data/templates/chatgpt/suggest_names.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-02-26 16:56:52.000000 oa-0.1.9/oa/data/templates/chatgpt/user_story_to_code_for_dag.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:57:30.788277 oa-0.1.9/oa/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 16:56:52.000000 oa-0.1.9/oa/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-02-26 16:56:52.000000 oa-0.1.9/oa/examples/aesop_fables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-02-26 16:56:52.000000 oa-0.1.9/oa/examples/illustrate_stories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15431 2024-02-26 16:57:04.000000 oa-0.1.9/oa/openai_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:57:30.788277 oa-0.1.9/oa/scrap/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:56:52.000000 oa-0.1.9/oa/scrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-02-26 16:57:04.000000 oa-0.1.9/oa/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-02-26 16:57:04.000000 oa-0.1.9/oa/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:57:30.784277 oa-0.1.9/oa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-02-26 16:57:30.000000 oa-0.1.9/oa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-02-26 16:57:30.000000 oa-0.1.9/oa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:57:30.000000 oa-0.1.9/oa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:57:30.000000 oa-0.1.9/oa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-26 16:57:30.000000 oa-0.1.9/oa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-26 16:57:30.000000 oa-0.1.9/oa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-26 16:57:30.788277 oa-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-26 16:56:52.000000 oa-0.1.9/setup.py
```

### Comparing `oa-0.1.8/LICENSE` & `oa-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oa-0.1.8/PKG-INFO` & `oa-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oa
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python interface to OpenAi
 Home-page: https://github.com/thorwhalen/oa
 Author: Thor Whalen
 License: apache-2.0
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oa-0.1.8/README.md` & `oa-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `oa-0.1.8/oa/base.py` & `oa-0.1.9/oa/base.py`

 * *Files identical despite different names*

### Comparing `oa-0.1.8/oa/data/templates/chatgpt/description_to_software_specs.txt` & `oa-0.1.9/oa/data/templates/chatgpt/description_to_software_specs.txt`

 * *Files identical despite different names*

### Comparing `oa-0.1.8/oa/data/templates/chatgpt/simple_tests_for_code.txt` & `oa-0.1.9/oa/data/templates/chatgpt/simple_tests_for_code.txt`

 * *Files identical despite different names*

### Comparing `oa-0.1.8/oa/data/templates/chatgpt/specs_to_code_for_dag.txt` & `oa-0.1.9/oa/data/templates/chatgpt/specs_to_code_for_dag.txt`

 * *Files identical despite different names*

### Comparing `oa-0.1.8/oa/data/templates/chatgpt/user_story_to_code_for_dag.txt` & `oa-0.1.9/oa/data/templates/chatgpt/user_story_to_code_for_dag.txt`

 * *Files identical despite different names*

### Comparing `oa-0.1.8/oa/examples/aesop_fables.py` & `oa-0.1.9/oa/examples/aesop_fables.py`

 * *Files identical despite different names*

### Comparing `oa-0.1.8/oa/examples/illustrate_stories.py` & `oa-0.1.9/oa/examples/illustrate_stories.py`

 * *Files identical despite different names*

### Comparing `oa-0.1.8/oa/openai_specs.py` & `oa-0.1.9/oa/openai_specs.py`

 * *Files identical despite different names*

### Comparing `oa-0.1.8/oa/tools.py` & `oa-0.1.9/oa/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     prompt_func_kwargs=None,
     egress=None,
     doc='The function composes a prompt and asks an LLM to respond to it.',
     module=__name__,
 ):
     """Convert a string template to a function that will produce a prompt string
     and ask an LLM (`prompt_func`) to respond to it.
+    
     """
 
     defaults = dict(template_to_defaults(template), **(defaults or {}))
     template = _template_without_specifiers(template)
     template_embodier = embodier(template)
     prompt_func_kwargs = prompt_func_kwargs or {}
     egress = egress or (lambda x: x)
```

### Comparing `oa-0.1.8/oa/util.py` & `oa-0.1.9/oa/util.py`

 * *Files identical despite different names*

### Comparing `oa-0.1.8/oa.egg-info/PKG-INFO` & `oa-0.1.9/oa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oa
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python interface to OpenAi
 Home-page: https://github.com/thorwhalen/oa
 Author: Thor Whalen
 License: apache-2.0
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oa-0.1.8/oa.egg-info/SOURCES.txt` & `oa-0.1.9/oa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oa-0.1.8/setup.cfg` & `oa-0.1.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oa
-version = 0.1.8
+version = 0.1.9
 url = https://github.com/thorwhalen/oa
 platforms = any
 description_file = README.md
 root_url = https://github.com/thorwhalen/
 license = apache-2.0
 author = Thor Whalen
 description = Python interface to OpenAi
@@ -22,14 +22,11 @@
 	dol
 	i2
 	config2py
 	graze
 	jsonref
 	lkj
 
-[options.package_data]
-oa = oa/data/*
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

