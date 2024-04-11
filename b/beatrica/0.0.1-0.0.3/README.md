# Comparing `tmp/beatrica-0.0.1.tar.gz` & `tmp/beatrica-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beatrica-0.0.1.tar", last modified: Wed Jan 31 17:01:04 2024, max compression
+gzip compressed data, was "beatrica-0.0.3.tar", last modified: Thu Apr 11 09:41:46 2024, max compression
```

## Comparing `beatrica-0.0.1.tar` & `beatrica-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-01-31 17:01:04.292806 beatrica-0.0.1/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    34523 2024-01-31 16:51:58.000000 beatrica-0.0.1/LICENSE
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      436 2024-01-31 17:01:04.292677 beatrica-0.0.1/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       10 2024-01-31 16:51:58.000000 beatrica-0.0.1/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-01-31 17:01:04.291964 beatrica-0.0.1/beatrica/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-01-31 16:58:26.000000 beatrica-0.0.1/beatrica/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-01-31 16:58:55.000000 beatrica-0.0.1/beatrica/beatrica.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-01-31 17:01:04.292413 beatrica-0.0.1/beatrica.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      436 2024-01-31 17:01:04.000000 beatrica-0.0.1/beatrica.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      214 2024-01-31 17:01:04.000000 beatrica-0.0.1/beatrica.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-01-31 17:01:04.000000 beatrica-0.0.1/beatrica.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       15 2024-01-31 17:01:04.000000 beatrica-0.0.1/beatrica.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-01-31 17:01:04.292845 beatrica-0.0.1/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      623 2024-01-31 17:00:29.000000 beatrica-0.0.1/setup.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-01-31 17:01:04.292536 beatrica-0.0.1/tests/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-01-31 16:58:40.000000 beatrica-0.0.1/tests/__init__.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:41:46.922918 beatrica-0.0.3/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    34523 2024-01-31 16:51:58.000000 beatrica-0.0.3/LICENSE
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    13013 2024-04-11 09:41:46.922715 beatrica-0.0.3/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    12484 2024-04-11 09:39:23.000000 beatrica-0.0.3/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:41:46.921303 beatrica-0.0.3/beatrica/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.3/beatrica/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     8472 2024-04-11 09:39:23.000000 beatrica-0.0.3/beatrica/beatrica.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1641 2024-04-11 09:39:23.000000 beatrica-0.0.3/beatrica/prompts.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:41:46.922102 beatrica-0.0.3/beatrica.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    13013 2024-04-11 09:41:46.000000 beatrica-0.0.3/beatrica.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      323 2024-04-11 09:41:46.000000 beatrica-0.0.3/beatrica.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-11 09:41:46.000000 beatrica-0.0.3/beatrica.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       52 2024-04-11 09:41:46.000000 beatrica-0.0.3/beatrica.egg-info/entry_points.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      203 2024-04-11 09:41:46.000000 beatrica-0.0.3/beatrica.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       15 2024-04-11 09:41:46.000000 beatrica-0.0.3/beatrica.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-11 09:41:46.922966 beatrica-0.0.3/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1282 2024-04-11 09:40:23.000000 beatrica-0.0.3/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:41:46.922328 beatrica-0.0.3/tests/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.3/tests/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1074 2024-04-11 09:39:23.000000 beatrica-0.0.3/tests/test_beatrica.py
```

### Comparing `beatrica-0.0.1/LICENSE` & `beatrica-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.1/setup.py` & `beatrica-0.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,47 @@
 from setuptools import setup, find_packages
 
 setup(
     name='beatrica',
-    version='0.0.1',
+    version='0.0.3',
     author='Eugene Evstafev',
     author_email='chigwel@gmail.com',
-    description='',
+    description="Beatrica is a tool for code review automation using large language models.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chigwell/beatrica',
     packages=find_packages(),
     install_requires=[
+        "rich==13.7.1",
+        "beatrica-git==0.1.1",
+        "beatrica-embedding==0.1.0",
+        "langchain-openai==0.1.2",
+        "langchain-mistralai==0.1.1",
     ],
+    extras_require={
+        'dev': [
+            'pytest',
+            'pytest-cov',
+            'pytest-mock',
+            'coverage',
+            'flake8',
+            'black',
+            'isort',
+            'mypy',
+            'pre-commit',
+            'twine',
+            'wheel',
+        ],
+    },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
+    entry_points={
+        'console_scripts': [
+            'beatrica=beatrica.beatrica:main',
+        ],
+    },
 )
```

