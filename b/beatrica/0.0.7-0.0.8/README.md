# Comparing `tmp/beatrica-0.0.7.tar.gz` & `tmp/beatrica-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beatrica-0.0.7.tar", last modified: Thu Apr 11 10:25:06 2024, max compression
+gzip compressed data, was "beatrica-0.0.8.tar", last modified: Thu Apr 11 13:10:54 2024, max compression
```

## Comparing `beatrica-0.0.7.tar` & `beatrica-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:25:06.232389 beatrica-0.0.7/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    34523 2024-01-31 16:51:58.000000 beatrica-0.0.7/LICENSE
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    14312 2024-04-11 10:25:06.232161 beatrica-0.0.7/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    13783 2024-04-11 10:25:00.000000 beatrica-0.0.7/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:25:06.230768 beatrica-0.0.7/beatrica/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.7/beatrica/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     8472 2024-04-11 09:39:23.000000 beatrica-0.0.7/beatrica/beatrica.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1641 2024-04-11 09:39:23.000000 beatrica-0.0.7/beatrica/prompts.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:25:06.231640 beatrica-0.0.7/beatrica.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    14312 2024-04-11 10:25:06.000000 beatrica-0.0.7/beatrica.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      323 2024-04-11 10:25:06.000000 beatrica-0.0.7/beatrica.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-11 10:25:06.000000 beatrica-0.0.7/beatrica.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       52 2024-04-11 10:25:06.000000 beatrica-0.0.7/beatrica.egg-info/entry_points.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      236 2024-04-11 10:25:06.000000 beatrica-0.0.7/beatrica.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       15 2024-04-11 10:25:06.000000 beatrica-0.0.7/beatrica.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-11 10:25:06.232466 beatrica-0.0.7/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1337 2024-04-11 10:25:00.000000 beatrica-0.0.7/setup.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:25:06.231865 beatrica-0.0.7/tests/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.7/tests/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1074 2024-04-11 09:39:23.000000 beatrica-0.0.7/tests/test_beatrica.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 13:10:54.472977 beatrica-0.0.8/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    34523 2024-01-31 16:51:58.000000 beatrica-0.0.8/LICENSE
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    14312 2024-04-11 13:10:54.472802 beatrica-0.0.8/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    13783 2024-04-11 10:25:00.000000 beatrica-0.0.8/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 13:10:54.471224 beatrica-0.0.8/beatrica/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.8/beatrica/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     8476 2024-04-11 13:10:50.000000 beatrica-0.0.8/beatrica/beatrica.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1641 2024-04-11 09:39:23.000000 beatrica-0.0.8/beatrica/prompts.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 13:10:54.472231 beatrica-0.0.8/beatrica.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    14312 2024-04-11 13:10:54.000000 beatrica-0.0.8/beatrica.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      323 2024-04-11 13:10:54.000000 beatrica-0.0.8/beatrica.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-11 13:10:54.000000 beatrica-0.0.8/beatrica.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       52 2024-04-11 13:10:54.000000 beatrica-0.0.8/beatrica.egg-info/entry_points.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      236 2024-04-11 13:10:54.000000 beatrica-0.0.8/beatrica.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       15 2024-04-11 13:10:54.000000 beatrica-0.0.8/beatrica.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-11 13:10:54.473018 beatrica-0.0.8/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1337 2024-04-11 13:10:50.000000 beatrica-0.0.8/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 13:10:54.472433 beatrica-0.0.8/tests/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.8/tests/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1074 2024-04-11 09:39:23.000000 beatrica-0.0.8/tests/test_beatrica.py
```

### Comparing `beatrica-0.0.7/LICENSE` & `beatrica-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.7/PKG-INFO` & `beatrica-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beatrica
-Version: 0.0.7
+Version: 0.0.8
 Summary: Beatrica is a tool for code review automation using large language models.
 Home-page: https://github.com/chigwell/beatrica
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beatrica-0.0.7/README.md` & `beatrica-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.7/beatrica/beatrica.py` & `beatrica-0.0.8/beatrica/beatrica.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     beatrica_diff_tracker.analyze_commits()
 
     commit_changes = beatrica_diff_tracker.commit_changes.items()
     if len(commit_changes) == 0:
         console.print("[bold red] No changes found. Exiting.[/]")
         exit(0)
     console.print("[bold green]✅  Changes tracked.[/]")
-    console.print(f"[bold blue]✅  Found[/] [bold magenta]{len(commit_changes)}[/] changes.")
+    console.print(f"[bold blue]✅  Found[/] [bold magenta]{len(commit_changes)}[/] change(s).")
 
     console.print("[bold blue]Initializing language model...[/]")
 
     if llm_type == "openai":
         language_model = ChatOpenAI(model_name=model_name, api_key=api_key, max_tokens=max_tokens)
     elif llm_type == "mistralai":
         language_model = ChatMistralAI(model=model_name, mistral_api_key=api_key, max_tokens=max_tokens)
@@ -91,15 +91,15 @@
     if len(matches) == 0:
         console.print(f"⚠️ Beatrica with {llm_type} {model_name} cannot make a review. "
                       f"This is likely due to the changes being too small or not code changes. "
                       f"Please try again with a different branch or more changes.")
         exit(0)
 
 
-    console.print(f"[bold green]✅ {len(matches)}[/] changes found for review.")
+    console.print(f"[bold green]✅ {len(matches)}[/] change(s) found for review.")
 
     console.print("[bold blue]Starting the review process...[/]")
 
     reviews = []
     for match in track(matches, description="Reviewing changes"):
         question = prompts['can_review']['question'] + match[0] + ": " + match[1] + "\n" + prompts['can_review']['expected_answer']
         result = retrieval_chain.invoke(question)
```

### Comparing `beatrica-0.0.7/beatrica/prompts.py` & `beatrica-0.0.8/beatrica/prompts.py`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.7/beatrica.egg-info/PKG-INFO` & `beatrica-0.0.8/beatrica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beatrica
-Version: 0.0.7
+Version: 0.0.8
 Summary: Beatrica is a tool for code review automation using large language models.
 Home-page: https://github.com/chigwell/beatrica
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beatrica-0.0.7/setup.py` & `beatrica-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='beatrica',
-    version='0.0.7',
+    version='0.0.8',
     author='Eugene Evstafev',
     author_email='chigwel@gmail.com',
     description="Beatrica is a tool for code review automation using large language models.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chigwell/beatrica',
     packages=find_packages(),
```

### Comparing `beatrica-0.0.7/tests/test_beatrica.py` & `beatrica-0.0.8/tests/test_beatrica.py`

 * *Files identical despite different names*

