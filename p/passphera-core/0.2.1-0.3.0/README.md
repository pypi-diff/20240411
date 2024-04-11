# Comparing `tmp/passphera-core-0.2.1.tar.gz` & `tmp/passphera-core-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passphera-core-0.2.1.tar", last modified: Wed Apr 10 23:08:35 2024, max compression
+gzip compressed data, was "passphera-core-0.3.0.tar", last modified: Thu Apr 11 00:00:39 2024, max compression
```

## Comparing `passphera-core-0.2.1.tar` & `passphera-core-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-10 23:08:35.511405 passphera-core-0.2.1/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-10 23:08:35.510405 passphera-core-0.2.1/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)       54 2024-04-05 01:50:44.000000 passphera-core-0.2.1/README.md
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-10 23:08:35.509405 passphera-core-0.2.1/passphera_core/
--rw-r--r--   0 fathi     (1000) fathi     (1000)     7908 2024-04-10 23:07:22.000000 passphera-core-0.2.1/passphera_core/__init__.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-10 23:08:35.510405 passphera-core-0.2.1/passphera_core.egg-info/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-10 23:08:35.000000 passphera-core-0.2.1/passphera_core.egg-info/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)      197 2024-04-10 23:08:35.000000 passphera-core-0.2.1/passphera_core.egg-info/SOURCES.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2024-04-10 23:08:35.000000 passphera-core-0.2.1/passphera_core.egg-info/dependency_links.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       15 2024-04-10 23:08:35.000000 passphera-core-0.2.1/passphera_core.egg-info/top_level.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2024-04-10 23:08:35.511405 passphera-core-0.2.1/setup.cfg
--rw-r--r--   0 fathi     (1000) fathi     (1000)      792 2024-04-10 23:07:46.000000 passphera-core-0.2.1/setup.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-11 00:00:39.733254 passphera-core-0.3.0/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-11 00:00:39.732254 passphera-core-0.3.0/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       54 2024-04-05 01:50:44.000000 passphera-core-0.3.0/README.md
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-11 00:00:39.731254 passphera-core-0.3.0/passphera_core/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       89 2024-04-10 23:57:17.000000 passphera-core-0.3.0/passphera_core/__init__.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      155 2024-04-10 23:57:17.000000 passphera-core-0.3.0/passphera_core/exceptions.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     7855 2024-04-10 23:57:17.000000 passphera-core-0.3.0/passphera_core/generator.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-11 00:00:39.732254 passphera-core-0.3.0/passphera_core.egg-info/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-11 00:00:39.000000 passphera-core-0.3.0/passphera_core.egg-info/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      254 2024-04-11 00:00:39.000000 passphera-core-0.3.0/passphera_core.egg-info/SOURCES.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2024-04-11 00:00:39.000000 passphera-core-0.3.0/passphera_core.egg-info/dependency_links.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       15 2024-04-11 00:00:39.000000 passphera-core-0.3.0/passphera_core.egg-info/top_level.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2024-04-11 00:00:39.733254 passphera-core-0.3.0/setup.cfg
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      792 2024-04-10 23:39:37.000000 passphera-core-0.3.0/setup.py
```

### Comparing `passphera-core-0.2.1/PKG-INFO` & `passphera-core-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passphera-core
-Version: 0.2.1
+Version: 0.3.0
 Summary: The core system of passphera project
 Home-page: https://github.com/passphera/core
 Author: Fathi Abdelmalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `passphera-core-0.2.1/passphera_core/__init__.py` & `passphera-core-0.3.0/passphera_core/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from cipherspy.cipher import *
 
-
-class InvalidAlgorithmException(Exception):
-    def __init__(self, algorithm: str) -> None:
-        super().__init__(f"Invalid algorithm name {algorithm}")
+from .exceptions import InvalidAlgorithmException
 
 
 class PasswordGenerator:
     """
     A strong password generator use multiple cipher algorithms to cipher a given plain text
     """
     def __init__(
@@ -31,15 +28,18 @@
         self._text: str = text
         self._shift: int = shift
         self._multiplier: int = multiplier
         self._key_str: str = key_str
         self._key_iter: iter = key_iter
         self._algorithm_name: str = algorithm.lower()
         self._algorithm = self._set_algorithm()
-        self._password: str = f'secret{self._text}secret'
+        if text:
+            self._password: str = f"secret{self._text.replace(' ', '')}secret"
+        else:
+            self._password: str = f'secret'
 
     @property
     def text(self) -> str:
         """
         Returns the text to be ciphered into a password
         Eg: ```password = pg.text```
         :return: str: The text to be ciphered into a password
@@ -51,15 +51,15 @@
         """
         Sets the text to be ciphered into a password
         Eg: ```pg.text = 'secret 2024 password'```
         :param text: The text to be ciphered into a password
         :return:
         """
         self._text = text
-        self._password: str = f'secret{self._text}secret'
+        self._password: str = f"secret{self._text.replace(' ', '')}secret"
 
     @property
     def shift(self) -> int:
         """
         Returns the shift value for the cipher algorithm
         Eg: ```shift = pg.shift```
         :return: int: The shift value for the cipher algorithm
@@ -223,12 +223,9 @@
         self._password = self.generate_raw_password()
         self._algorithm_name = old_algorithm
         self._update_algorithm_properties()
         for char, replacement in self._chars_replacements.items():
             self._password = self._password.replace(char, replacement)
         for char in self._password:
             if char in self._text:
-                self._password = self._text.replace(char, char.upper())
+                self._password = self._password.replace(char, char.upper())
         return self._password
-
-
-__all__ = ['PasswordGenerator', 'InvalidAlgorithmException']
```

### Comparing `passphera-core-0.2.1/passphera_core.egg-info/PKG-INFO` & `passphera-core-0.3.0/passphera_core.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passphera-core
-Version: 0.2.1
+Version: 0.3.0
 Summary: The core system of passphera project
 Home-page: https://github.com/passphera/core
 Author: Fathi Abdelmalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `passphera-core-0.2.1/setup.py` & `passphera-core-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='passphera-core',
-    version='0.2.1',
+    version='0.3.0',
     author='Fathi Abdelmalek',
     author_email='abdelmalek.fathi.2001@gmail.com',
     url='https://github.com/passphera/core',
     description='The core system of passphera project',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['passphera_core'],
```

