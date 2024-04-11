# Comparing `tmp/cook_builder-0.0.8.tar.gz` & `tmp/cook_builder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cook_builder-0.0.8.tar", last modified: Tue Apr  2 18:51:15 2024, max compression
+gzip compressed data, was "cook_builder-0.0.9.tar", last modified: Thu Apr 11 18:43:50 2024, max compression
```

## Comparing `cook_builder-0.0.8.tar` & `cook_builder-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-02 18:51:15.142826 cook_builder-0.0.8/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.0.8/LICENSE
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2662 2024-04-02 18:51:15.142826 cook_builder-0.0.8/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      532 2024-04-02 18:20:44.000000 cook_builder-0.0.8/README.md
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-02 18:51:15.142826 cook_builder-0.0.8/cook/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        0 2024-02-10 12:15:45.000000 cook_builder-0.0.8/cook/__init__.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1211 2024-04-02 18:37:31.000000 cook_builder-0.0.8/cook/cli.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     5742 2024-04-02 18:20:44.000000 cook_builder-0.0.8/cook/configuration.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3491 2024-04-02 18:20:52.000000 cook_builder-0.0.8/cook/cook.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      369 2024-03-13 19:09:39.000000 cook_builder-0.0.8/cook/logger.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1342 2024-04-02 18:46:13.000000 cook_builder-0.0.8/cook/recipe.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      936 2024-03-09 09:22:10.000000 cook_builder-0.0.8/cook/rsync.py
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-02 18:51:15.142826 cook_builder-0.0.8/cook_builder.egg-info/
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2662 2024-04-02 18:51:15.000000 cook_builder-0.0.8/cook_builder.egg-info/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      358 2024-04-02 18:51:15.000000 cook_builder-0.0.8/cook_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-04-02 18:51:15.000000 cook_builder-0.0.8/cook_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       39 2024-04-02 18:51:15.000000 cook_builder-0.0.8/cook_builder.egg-info/entry_points.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       27 2024-04-02 18:51:15.000000 cook_builder-0.0.8/cook_builder.egg-info/requires.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-04-02 18:51:15.000000 cook_builder-0.0.8/cook_builder.egg-info/top_level.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      983 2024-04-02 18:50:59.000000 cook_builder-0.0.8/pyproject.toml
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-02 18:51:15.142826 cook_builder-0.0.8/setup.cfg
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-11 18:43:50.453547 cook_builder-0.0.9/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.0.9/LICENSE
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2981 2024-04-11 18:43:50.453547 cook_builder-0.0.9/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      851 2024-04-02 19:02:19.000000 cook_builder-0.0.9/README.md
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-11 18:43:50.449546 cook_builder-0.0.9/cook/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        0 2024-02-10 12:15:45.000000 cook_builder-0.0.9/cook/__init__.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1710 2024-04-11 18:40:16.000000 cook_builder-0.0.9/cook/cli.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     5742 2024-04-02 18:20:44.000000 cook_builder-0.0.9/cook/configuration.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3491 2024-04-11 18:43:27.000000 cook_builder-0.0.9/cook/cook.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      369 2024-04-11 18:43:27.000000 cook_builder-0.0.9/cook/logger.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1342 2024-04-02 18:46:13.000000 cook_builder-0.0.9/cook/recipe.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      936 2024-03-09 09:22:10.000000 cook_builder-0.0.9/cook/rsync.py
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-11 18:43:50.453547 cook_builder-0.0.9/cook_builder.egg-info/
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2981 2024-04-11 18:43:50.000000 cook_builder-0.0.9/cook_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      358 2024-04-11 18:43:50.000000 cook_builder-0.0.9/cook_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-04-11 18:43:50.000000 cook_builder-0.0.9/cook_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       39 2024-04-11 18:43:50.000000 cook_builder-0.0.9/cook_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       27 2024-04-11 18:43:50.000000 cook_builder-0.0.9/cook_builder.egg-info/requires.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-04-11 18:43:50.000000 cook_builder-0.0.9/cook_builder.egg-info/top_level.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      983 2024-04-11 18:43:22.000000 cook_builder-0.0.9/pyproject.toml
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-11 18:43:50.453547 cook_builder-0.0.9/setup.cfg
```

### Comparing `cook_builder-0.0.8/LICENSE` & `cook_builder-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cook_builder-0.0.8/PKG-INFO` & `cook_builder-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.0.8
+Version: 0.0.9
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,30 +45,42 @@
 
 # Cook
 
 Build script aggregator and remote executor.
 
 # Getting started
 
-### Install cook with pip
+### Install cook with pipx
 
-```sh
-pip install cook-builder
-```
-
-### Install cook from source
+Cook is available on PyPI under the name [cook-builder](https://pypi.org/project/cook-builder/).
+It can be easily installed with pip, but the recommended method is to use [pipx](https://pipx.pypa.io/stable/).
 
 ```sh
-git clone https://github.com/serweryn617/cook.git
-cd cook
-pip install .
+pipx install cook-builder
 ```
 
 ### Setup
 
-Create `recipe.py` file which describes how to build Your project and lists the available remote build servers.
+Create `recipe.py` file which describes how to build Your project locally and on remote build servers.
 
 See the [example project](example).
 
 ### Run
 
-Run `cook` command in the directory where the `recipe.py` file is located and see how the project is being built!
+Run `cook` command in the terminal and see how the project is being built!
+
+# Development
+
+### Install cook from source
+
+```sh
+git clone https://github.com/serweryn617/cook.git
+cd cook
+pip install -e .
+```
+
+<!-- RELEASING
+1. Update version in pyproject.toml
+2. Build and upload wheels to PyPI:
+    python3 -m build
+    twine upload dist/*
+-->
```

### Comparing `cook_builder-0.0.8/cook/cli.py` & `cook_builder-0.0.9/cook/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,31 +11,45 @@
     for arg in user_args:
         key, value = arg.split('=')
         res[key] = value
     return res
 
 
 def main():
-    parser = argparse.ArgumentParser()
-
-    parser.add_argument('recipe_path', nargs='?', default='.', help='Recipe file directory path.')
-    parser.add_argument('-p', '--project', help='Project to build. Uses value of `default_project` if left unspecified.')
-    parser.add_argument('-s', '--build_server', help='Build server to use. Uses value of `default_build_server` if left unspecified.')
-    parser.add_argument('-u', '--user_args', nargs='*', default={}, help='User arguments. Can be used in recipe file. Format: key=value')
+    epilog_text = '\n'.join((
+        'example usage:',
+        '  %(prog)s my_project name=latest -p ./example/ -b local',
+    ))
+
+    parser = argparse.ArgumentParser(
+        description='Build script aggregator and remote executor',
+        epilog=epilog_text,
+        formatter_class=argparse.RawDescriptionHelpFormatter
+    )
+
+    parser.add_argument('-p', '--recipe_path', default='.', help='Path to directory containing `recipe.py` file.')
+    parser.add_argument('-b', '--build_server', help='Build server to use. Uses value of `default_build_server` if left unspecified.')
+    parser.add_argument('project', nargs='?', help='Project to build. Uses value of `default_project` if left unspecified.')
+    parser.add_argument('user_args', nargs='*', default=[], help='User arguments. Can be used in recipe file. Format: `key=value`')
 
     args = parser.parse_args()
-
-    base_path = pathlib.Path.cwd() / args.recipe_path
+    recipe_base_path = pathlib.Path.cwd() / args.recipe_path
+    build_server = args.build_server
+    if args.project and '=' in args.project:
+        project = None
+        args.user_args.append(args.project)
+    else:
+        project = args.project
     user_args = parse_user_args(args.user_args)
 
-    recipe = Recipe(base_path, user_args)
+    recipe = Recipe(recipe_base_path, user_args)
     recipe.load()
 
     configuration = Configuration(recipe)
-    configuration.setup(args.project, args.build_server)
+    configuration.setup(project, build_server)
 
     cook = Cook(recipe, configuration)
     cook.cook()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `cook_builder-0.0.8/cook/configuration.py` & `cook_builder-0.0.9/cook/configuration.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.0.8/cook/cook.py` & `cook_builder-0.0.9/cook/cook.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.0.8/cook/recipe.py` & `cook_builder-0.0.9/cook/recipe.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.0.8/cook/rsync.py` & `cook_builder-0.0.9/cook/rsync.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.0.8/cook_builder.egg-info/PKG-INFO` & `cook_builder-0.0.9/cook_builder.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.0.8
+Version: 0.0.9
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,30 +45,42 @@
 
 # Cook
 
 Build script aggregator and remote executor.
 
 # Getting started
 
-### Install cook with pip
+### Install cook with pipx
 
-```sh
-pip install cook-builder
-```
-
-### Install cook from source
+Cook is available on PyPI under the name [cook-builder](https://pypi.org/project/cook-builder/).
+It can be easily installed with pip, but the recommended method is to use [pipx](https://pipx.pypa.io/stable/).
 
 ```sh
-git clone https://github.com/serweryn617/cook.git
-cd cook
-pip install .
+pipx install cook-builder
 ```
 
 ### Setup
 
-Create `recipe.py` file which describes how to build Your project and lists the available remote build servers.
+Create `recipe.py` file which describes how to build Your project locally and on remote build servers.
 
 See the [example project](example).
 
 ### Run
 
-Run `cook` command in the directory where the `recipe.py` file is located and see how the project is being built!
+Run `cook` command in the terminal and see how the project is being built!
+
+# Development
+
+### Install cook from source
+
+```sh
+git clone https://github.com/serweryn617/cook.git
+cd cook
+pip install -e .
+```
+
+<!-- RELEASING
+1. Update version in pyproject.toml
+2. Build and upload wheels to PyPI:
+    python3 -m build
+    twine upload dist/*
+-->
```

### Comparing `cook_builder-0.0.8/pyproject.toml` & `cook_builder-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cook_builder"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
   "fabric==3.2.2",
   "rich==13.7.1",
 ]
 requires-python = ">=3.10"
 authors = [
   { name="Seweryn Rusecki" },
```

