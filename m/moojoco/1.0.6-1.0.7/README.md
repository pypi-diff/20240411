# Comparing `tmp/moojoco-1.0.6.tar.gz` & `tmp/moojoco-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moojoco-1.0.6.tar", last modified: Wed Mar 27 10:48:12 2024, max compression
+gzip compressed data, was "moojoco-1.0.7.tar", last modified: Thu Apr 11 08:55:58 2024, max compression
```

## Comparing `moojoco-1.0.6.tar` & `moojoco-1.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:48:12.439433 moojoco-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-27 10:48:06.000000 moojoco-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-27 10:48:06.000000 moojoco-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-03-27 10:48:12.439433 moojoco-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-03-27 10:48:06.000000 moojoco-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:48:12.435433 moojoco-1.0.6/moojoco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:48:06.000000 moojoco-1.0.6/moojoco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:48:12.439433 moojoco-1.0.6/moojoco/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:48:06.000000 moojoco-1.0.6/moojoco/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-03-27 10:48:06.000000 moojoco-1.0.6/moojoco/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-27 10:48:06.000000 moojoco-1.0.6/moojoco/environment/dual.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-03-27 10:48:06.000000 moojoco-1.0.6/moojoco/environment/mjc_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-03-27 10:48:06.000000 moojoco-1.0.6/moojoco/environment/mjx_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-03-27 10:48:06.000000 moojoco-1.0.6/moojoco/environment/mjx_spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-03-27 10:48:06.000000 moojoco-1.0.6/moojoco/environment/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-03-27 10:48:06.000000 moojoco-1.0.6/moojoco/environment/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:48:12.439433 moojoco-1.0.6/moojoco/mjcf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:48:06.000000 moojoco-1.0.6/moojoco/mjcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-27 10:48:06.000000 moojoco-1.0.6/moojoco/mjcf/arena.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-03-27 10:48:06.000000 moojoco-1.0.6/moojoco/mjcf/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-03-27 10:48:06.000000 moojoco-1.0.6/moojoco/mjcf/morphology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:48:12.439433 moojoco-1.0.6/moojoco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-03-27 10:48:12.000000 moojoco-1.0.6/moojoco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-27 10:48:12.000000 moojoco-1.0.6/moojoco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 10:48:12.000000 moojoco-1.0.6/moojoco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-27 10:48:12.000000 moojoco-1.0.6/moojoco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-27 10:48:12.000000 moojoco-1.0.6/moojoco.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-27 10:48:06.000000 moojoco-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-27 10:48:06.000000 moojoco-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 10:48:12.439433 moojoco-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-27 10:48:06.000000 moojoco-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:58.257259 moojoco-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-11 08:55:49.000000 moojoco-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-11 08:55:49.000000 moojoco-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-11 08:55:58.257259 moojoco-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-11 08:55:49.000000 moojoco-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:58.253259 moojoco-1.0.7/moojoco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:49.000000 moojoco-1.0.7/moojoco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:58.257259 moojoco-1.0.7/moojoco/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:49.000000 moojoco-1.0.7/moojoco/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-04-11 08:55:49.000000 moojoco-1.0.7/moojoco/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-11 08:55:49.000000 moojoco-1.0.7/moojoco/environment/dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-04-11 08:55:49.000000 moojoco-1.0.7/moojoco/environment/mjc_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-11 08:55:49.000000 moojoco-1.0.7/moojoco/environment/mjx_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-11 08:55:49.000000 moojoco-1.0.7/moojoco/environment/mjx_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-04-11 08:55:49.000000 moojoco-1.0.7/moojoco/environment/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-11 08:55:49.000000 moojoco-1.0.7/moojoco/environment/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:58.257259 moojoco-1.0.7/moojoco/mjcf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:49.000000 moojoco-1.0.7/moojoco/mjcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-11 08:55:49.000000 moojoco-1.0.7/moojoco/mjcf/arena.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-11 08:55:49.000000 moojoco-1.0.7/moojoco/mjcf/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-11 08:55:49.000000 moojoco-1.0.7/moojoco/mjcf/morphology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:58.257259 moojoco-1.0.7/moojoco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-11 08:55:58.000000 moojoco-1.0.7/moojoco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-11 08:55:58.000000 moojoco-1.0.7/moojoco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 08:55:58.000000 moojoco-1.0.7/moojoco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 08:55:58.000000 moojoco-1.0.7/moojoco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 08:55:58.000000 moojoco-1.0.7/moojoco.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-11 08:55:49.000000 moojoco-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-11 08:55:49.000000 moojoco-1.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 08:55:58.257259 moojoco-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-11 08:55:49.000000 moojoco-1.0.7/setup.py
```

### Comparing `moojoco-1.0.6/LICENSE` & `moojoco-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `moojoco-1.0.6/PKG-INFO` & `moojoco-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moojoco
-Version: 1.0.6
+Version: 1.0.7
 Summary: A unified framework for implementing and interfacing with MuJoCo and MuJoCo-XLA simulation environments.
 Home-page: https://github.com/Co-Evolve/moojoco
 Author-email: Dries Marzougui <dries.marzougui@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Co-Evolve/moojoco
 Project-URL: Repository, https://github.com/Co-Evolve/moojoco
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moojoco Version: 1.0.6 Summary: A unified framework
+Metadata-Version: 2.1 Name: moojoco Version: 1.0.7 Summary: A unified framework
 for implementing and interfacing with MuJoCo and MuJoCo-XLA simulation
 environments. Home-page: https://github.com/Co-Evolve/moojoco Author-email:
 Dries Marzougui
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/Co-Evolve/
 moojoco Project-URL: Repository, https://github.com/Co-Evolve/moojoco
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
```

### Comparing `moojoco-1.0.6/README.md` & `moojoco-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `moojoco-1.0.6/moojoco/environment/base.py` & `moojoco-1.0.7/moojoco/environment/base.py`

 * *Files identical despite different names*

### Comparing `moojoco-1.0.6/moojoco/environment/dual.py` & `moojoco-1.0.7/moojoco/environment/dual.py`

 * *Files identical despite different names*

### Comparing `moojoco-1.0.6/moojoco/environment/mjc_env.py` & `moojoco-1.0.7/moojoco/environment/mjc_env.py`

 * *Files identical despite different names*

### Comparing `moojoco-1.0.6/moojoco/environment/mjx_env.py` & `moojoco-1.0.7/moojoco/environment/mjx_env.py`

 * *Files identical despite different names*

### Comparing `moojoco-1.0.6/moojoco/environment/mjx_spaces.py` & `moojoco-1.0.7/moojoco/environment/mjx_spaces.py`

 * *Files identical despite different names*

### Comparing `moojoco-1.0.6/moojoco/environment/renderer.py` & `moojoco-1.0.7/moojoco/environment/renderer.py`

 * *Files identical despite different names*

### Comparing `moojoco-1.0.6/moojoco/environment/wrapper.py` & `moojoco-1.0.7/moojoco/environment/wrapper.py`

 * *Files identical despite different names*

### Comparing `moojoco-1.0.6/moojoco/mjcf/arena.py` & `moojoco-1.0.7/moojoco/mjcf/arena.py`

 * *Files identical despite different names*

### Comparing `moojoco-1.0.6/moojoco/mjcf/component.py` & `moojoco-1.0.7/moojoco/mjcf/component.py`

 * *Files identical despite different names*

### Comparing `moojoco-1.0.6/moojoco/mjcf/morphology.py` & `moojoco-1.0.7/moojoco/mjcf/morphology.py`

 * *Files identical despite different names*

### Comparing `moojoco-1.0.6/moojoco.egg-info/PKG-INFO` & `moojoco-1.0.7/moojoco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moojoco
-Version: 1.0.6
+Version: 1.0.7
 Summary: A unified framework for implementing and interfacing with MuJoCo and MuJoCo-XLA simulation environments.
 Home-page: https://github.com/Co-Evolve/moojoco
 Author-email: Dries Marzougui <dries.marzougui@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Co-Evolve/moojoco
 Project-URL: Repository, https://github.com/Co-Evolve/moojoco
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moojoco Version: 1.0.6 Summary: A unified framework
+Metadata-Version: 2.1 Name: moojoco Version: 1.0.7 Summary: A unified framework
 for implementing and interfacing with MuJoCo and MuJoCo-XLA simulation
 environments. Home-page: https://github.com/Co-Evolve/moojoco Author-email:
 Dries Marzougui
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/Co-Evolve/
 moojoco Project-URL: Repository, https://github.com/Co-Evolve/moojoco
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
```

### Comparing `moojoco-1.0.6/moojoco.egg-info/SOURCES.txt` & `moojoco-1.0.7/moojoco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moojoco-1.0.6/pyproject.toml` & `moojoco-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moojoco"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
     { name = "Dries Marzougui", email = "dries.marzougui@gmail.com" },
 ]
 description = "A unified framework for implementing and interfacing with MuJoCo and MuJoCo-XLA simulation environments."
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { text = "MIT" }
 classifiers = [
```

### Comparing `moojoco-1.0.6/setup.py` & `moojoco-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     license = f.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
         name='moojoco',
-        version='1.0.6',
+        version='1.0.7',
         description='A unified framework for implementing and interfacing with MuJoCo and MuJoCo-XLA simulation '
                     'environments.',
         long_description=readme,
         url='https://github.com/Co-Evolve/moojoco',
         license=license,
         packages=find_packages(exclude=('tests', 'docs')),
         install_requires=required
```

