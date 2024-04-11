# Comparing `tmp/clip2imgur-0.9.3.tar.gz` & `tmp/clip2imgur-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clip2imgur-0.9.3.tar", last modified: Wed Apr 10 02:53:40 2024, max compression
+gzip compressed data, was "clip2imgur-0.9.4.tar", last modified: Thu Apr 11 16:16:12 2024, max compression
```

## Comparing `clip2imgur-0.9.3.tar` & `clip2imgur-0.9.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 02:53:40.198419 clip2imgur-0.9.3/
--rw-rw-r--   0 jaywang    (501) staff       (20)      273 2024-04-10 01:03:51.000000 clip2imgur-0.9.3/MANIFEST.in
--rw-r--r--   0 jaywang    (501) staff       (20)     5054 2024-04-10 02:53:40.198339 clip2imgur-0.9.3/PKG-INFO
--rw-r--r--   0 jaywang    (501) staff       (20)     4101 2024-04-10 01:44:11.000000 clip2imgur-0.9.3/README.md
-drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 02:53:40.195934 clip2imgur-0.9.3/clip2imgur/
--rw-r--r--   0 jaywang    (501) staff       (20)     6148 2024-04-10 00:59:10.000000 clip2imgur-0.9.3/clip2imgur/.DS_Store
--rw-rw-r--   0 jaywang    (501) staff       (20)      202 2024-04-10 02:53:34.000000 clip2imgur-0.9.3/clip2imgur/__init__.py
-drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 02:53:40.197251 clip2imgur-0.9.3/clip2imgur/__pycache__/
--rw-r--r--   0 jaywang    (501) staff       (20)      393 2024-04-10 01:12:01.000000 clip2imgur-0.9.3/clip2imgur/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 jaywang    (501) staff       (20)     8540 2024-04-10 01:12:01.000000 clip2imgur-0.9.3/clip2imgur/__pycache__/clip2imgur.cpython-310.pyc
--rw-r--r--   0 jaywang    (501) staff       (20)    10303 2024-04-10 02:42:28.000000 clip2imgur-0.9.3/clip2imgur/clip2imgur.py
-drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 02:53:40.198083 clip2imgur-0.9.3/clip2imgur.egg-info/
--rw-r--r--   0 jaywang    (501) staff       (20)     5054 2024-04-10 02:53:40.000000 clip2imgur-0.9.3/clip2imgur.egg-info/PKG-INFO
--rw-r--r--   0 jaywang    (501) staff       (20)      489 2024-04-10 02:53:40.000000 clip2imgur-0.9.3/clip2imgur.egg-info/SOURCES.txt
--rw-r--r--   0 jaywang    (501) staff       (20)        1 2024-04-10 02:53:40.000000 clip2imgur-0.9.3/clip2imgur.egg-info/dependency_links.txt
--rw-r--r--   0 jaywang    (501) staff       (20)       58 2024-04-10 02:53:40.000000 clip2imgur-0.9.3/clip2imgur.egg-info/entry_points.txt
--rw-r--r--   0 jaywang    (501) staff       (20)        1 2024-04-10 01:54:53.000000 clip2imgur-0.9.3/clip2imgur.egg-info/not-zip-safe
--rw-r--r--   0 jaywang    (501) staff       (20)       38 2024-04-10 02:53:40.000000 clip2imgur-0.9.3/clip2imgur.egg-info/requires.txt
--rw-r--r--   0 jaywang    (501) staff       (20)       11 2024-04-10 02:53:40.000000 clip2imgur-0.9.3/clip2imgur.egg-info/top_level.txt
--rw-rw-r--   0 jaywang    (501) staff       (20)      382 2024-04-10 02:53:40.198737 clip2imgur-0.9.3/setup.cfg
--rw-rw-r--   0 jaywang    (501) staff       (20)     1637 2024-04-10 02:53:34.000000 clip2imgur-0.9.3/setup.py
-drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 02:53:40.197557 clip2imgur-0.9.3/tests/
--rw-rw-r--   0 jaywang    (501) staff       (20)       40 2024-04-10 01:01:27.000000 clip2imgur-0.9.3/tests/__init__.py
--rw-rw-r--   0 jaywang    (501) staff       (20)      598 2024-04-10 01:51:09.000000 clip2imgur-0.9.3/tests/test_clip2imgur.py
+drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-11 16:16:12.462404 clip2imgur-0.9.4/
+-rw-rw-r--   0 jaywang    (501) staff       (20)      273 2024-04-10 01:03:51.000000 clip2imgur-0.9.4/MANIFEST.in
+-rw-r--r--   0 jaywang    (501) staff       (20)     4273 2024-04-11 16:16:12.462315 clip2imgur-0.9.4/PKG-INFO
+-rw-r--r--   0 jaywang    (501) staff       (20)     3296 2024-04-10 03:19:25.000000 clip2imgur-0.9.4/README.md
+drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-11 16:16:12.459861 clip2imgur-0.9.4/clip2imgur/
+-rw-r--r--   0 jaywang    (501) staff       (20)     6148 2024-04-10 00:59:10.000000 clip2imgur-0.9.4/clip2imgur/.DS_Store
+-rw-rw-r--   0 jaywang    (501) staff       (20)      202 2024-04-11 16:16:11.000000 clip2imgur-0.9.4/clip2imgur/__init__.py
+drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-11 16:16:12.461440 clip2imgur-0.9.4/clip2imgur/__pycache__/
+-rw-r--r--   0 jaywang    (501) staff       (20)      393 2024-04-10 01:12:01.000000 clip2imgur-0.9.4/clip2imgur/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 jaywang    (501) staff       (20)     8540 2024-04-10 01:12:01.000000 clip2imgur-0.9.4/clip2imgur/__pycache__/clip2imgur.cpython-310.pyc
+-rw-r--r--   0 jaywang    (501) staff       (20)    10303 2024-04-10 02:42:28.000000 clip2imgur-0.9.4/clip2imgur/clip2imgur.py
+drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-11 16:16:12.462055 clip2imgur-0.9.4/clip2imgur.egg-info/
+-rw-r--r--   0 jaywang    (501) staff       (20)     4273 2024-04-11 16:16:12.000000 clip2imgur-0.9.4/clip2imgur.egg-info/PKG-INFO
+-rw-r--r--   0 jaywang    (501) staff       (20)      489 2024-04-11 16:16:12.000000 clip2imgur-0.9.4/clip2imgur.egg-info/SOURCES.txt
+-rw-r--r--   0 jaywang    (501) staff       (20)        1 2024-04-11 16:16:12.000000 clip2imgur-0.9.4/clip2imgur.egg-info/dependency_links.txt
+-rw-r--r--   0 jaywang    (501) staff       (20)       58 2024-04-11 16:16:12.000000 clip2imgur-0.9.4/clip2imgur.egg-info/entry_points.txt
+-rw-r--r--   0 jaywang    (501) staff       (20)        1 2024-04-10 01:54:53.000000 clip2imgur-0.9.4/clip2imgur.egg-info/not-zip-safe
+-rw-r--r--   0 jaywang    (501) staff       (20)       47 2024-04-11 16:16:12.000000 clip2imgur-0.9.4/clip2imgur.egg-info/requires.txt
+-rw-r--r--   0 jaywang    (501) staff       (20)       11 2024-04-11 16:16:12.000000 clip2imgur-0.9.4/clip2imgur.egg-info/top_level.txt
+-rw-rw-r--   0 jaywang    (501) staff       (20)      382 2024-04-11 16:16:12.462718 clip2imgur-0.9.4/setup.cfg
+-rw-rw-r--   0 jaywang    (501) staff       (20)     1649 2024-04-11 16:16:11.000000 clip2imgur-0.9.4/setup.py
+drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-11 16:16:12.461832 clip2imgur-0.9.4/tests/
+-rw-rw-r--   0 jaywang    (501) staff       (20)       40 2024-04-10 01:01:27.000000 clip2imgur-0.9.4/tests/__init__.py
+-rw-rw-r--   0 jaywang    (501) staff       (20)      598 2024-04-10 01:51:09.000000 clip2imgur-0.9.4/tests/test_clip2imgur.py
```

### Comparing `clip2imgur-0.9.3/PKG-INFO` & `clip2imgur-0.9.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clip2imgur
-Version: 0.9.3
+Version: 0.9.4
 Summary: A simple CLI that uploads your image in the clipboard to Imgur.
 Home-page: https://github.com/xiaohk/clip2imgur
 Author: Jay Wang
 Author-email: jayw@zijie.wang
 License: MIT license
 Keywords: Imgur,CLI,Image,Clipboard
 Platform: Linux
@@ -21,14 +21,15 @@
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pyobjc-framework-Cocoa
 Requires-Dist: pyperclip
 Requires-Dist: rich
+Requires-Dist: requests
 
 <h1>clip2imgur <img src="./icon.png" height="36" align="right"></h1>
 
 > A simple macOS command line tool for uploading your screenshots from clipboard
 > to Imgur
 
 [![Github Actions Status](https://github.com/xiaohk/clip2imgur/workflows/build/badge.svg)](https://github.com/xiaohk/clip2imgur/actions/workflows/build.yml)
@@ -62,19 +63,25 @@
 ```
 
 | short | long         | description                                                                         |
 | :---- | :----------- | :---------------------------------------------------------------------------------- |
 | `-m`  | `--markdown` | URL will be copied in the Markdown image format.`[](https://i.imgur.com/x.png)`     |
 | `-t`  | `--html`     | URL will be copied in the HTML image format.`<img src="https://i.imgur.com/x.png">` |
 | `-n`  | `--notcopy`  | Your image URL will not be copied to your clipboard                                 |
+| `-a`  | `--anon`     | Post the image anonymously                                                          |
 
 Personally I like to include images in Markdown file using the HTML format,
 which gives more control of the display. If you forget these flags, you always
 can run `clip2imgur -h` to check the usage.
 
+## Change Log
+
+- (4/9/2024): Clip2imgur is rewritten in Python.
+- (2/15/2018): Clip2imgur is released. This version is written in Swift.
+
 ## Install
 
 This package is built using cross-platform Swift with Swift Package Manager
 (SPM), but it currently only supports macOS. There are three ways to install
 `clip2imgur`.
 
 ### Homebrew
@@ -90,44 +97,23 @@
 Then, to install `clip2imgur`:
 
 ```
 $ brew tap xiaohk/clip2imgur
 $ brew install clip2imgur
 ```
 
-### Download the Binary
+### PyPI
 
-You can download the pre-compiled binary from the
-[Latest Rease](https://github.com/xiaohk/clip2imgur/releases/latest). After
-extract the binary, you want to create a symbolic link in `/usr/local/bin` to
-launch `clip2imgur` in your terminal more quickly.
+If you are familiar with Python, you can install `clip2imgur` with pip.
 
 ```
-$ mkdir ~/clip2imgur && cd ~/clip2imgur
-$ curl -O https://github.com/xiaohk/clip2imgur/releases/download/v0.9/clip2imgur-0.9.0.tar.gz
-$ tar -xvzf clip2imgur-0.9.0.tar.gz
-$ ln -s ~/clip2imgur/clip2imgur /usr/local/bin/clip2imgur
+$ pip install clip2imgur
 ```
 
-### Build from Source
-
-This approach is not recommended, because a function used to refresh your
-authorization is not open sourced for security reasons. Your compiled version
-works fine, but may require you to re-authorize `clip2imgur` periodically. If
-you only want to post images anonymously, then it doesn't really matter.
-
-To build `clip2imgur`, you need macOS 10.10 or later and Swift 3.0 or above.
-
-```
-$ git clone https://github.com/xiaohk/clip2imgur.git
-$ cd clip2imgur
-$ swift build -c release -Xswiftc -static-stdlib
-$ ln -s $(pwd)/.build/release/clip2imgur /usr/local/bin/clip2imgur
-```
+## Built With
 
-`clip2imgur` also has a by-product framework `clip2imgurCore` in `./build`.
-There might be some handy functions to use in your own projects.
+The latest version (>=v0.9.1) uses Python.
 
-## Built With
+The first version (v0.9.0) was built with:
 
 - [Swift Package Manager](https://swift.org/package-manager/)
 - [Rainbow](https://github.com/onevcat/Rainbow)
```

### Comparing `clip2imgur-0.9.3/README.md` & `clip2imgur-0.9.4/clip2imgur.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: clip2imgur
+Version: 0.9.4
+Summary: A simple CLI that uploads your image in the clipboard to Imgur.
+Home-page: https://github.com/xiaohk/clip2imgur
+Author: Jay Wang
+Author-email: jayw@zijie.wang
+License: MIT license
+Keywords: Imgur,CLI,Image,Clipboard
+Platform: Linux
+Platform: Mac OS X
+Platform: Windows
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Framework :: Jupyter :: JupyterLab :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Requires-Dist: pyobjc-framework-Cocoa
+Requires-Dist: pyperclip
+Requires-Dist: rich
+Requires-Dist: requests
+
 <h1>clip2imgur <img src="./icon.png" height="36" align="right"></h1>
 
 > A simple macOS command line tool for uploading your screenshots from clipboard
 > to Imgur
 
 [![Github Actions Status](https://github.com/xiaohk/clip2imgur/workflows/build/badge.svg)](https://github.com/xiaohk/clip2imgur/actions/workflows/build.yml)
 [![License](https://img.shields.io/badge/License-MIT-yellowgreen)](https://github.com/xiaohk/clip2imgur/blob/master/LICENSE)
@@ -34,19 +63,25 @@
 ```
 
 | short | long         | description                                                                         |
 | :---- | :----------- | :---------------------------------------------------------------------------------- |
 | `-m`  | `--markdown` | URL will be copied in the Markdown image format.`[](https://i.imgur.com/x.png)`     |
 | `-t`  | `--html`     | URL will be copied in the HTML image format.`<img src="https://i.imgur.com/x.png">` |
 | `-n`  | `--notcopy`  | Your image URL will not be copied to your clipboard                                 |
+| `-a`  | `--anon`     | Post the image anonymously                                                          |
 
 Personally I like to include images in Markdown file using the HTML format,
 which gives more control of the display. If you forget these flags, you always
 can run `clip2imgur -h` to check the usage.
 
+## Change Log
+
+- (4/9/2024): Clip2imgur is rewritten in Python.
+- (2/15/2018): Clip2imgur is released. This version is written in Swift.
+
 ## Install
 
 This package is built using cross-platform Swift with Swift Package Manager
 (SPM), but it currently only supports macOS. There are three ways to install
 `clip2imgur`.
 
 ### Homebrew
@@ -62,44 +97,23 @@
 Then, to install `clip2imgur`:
 
 ```
 $ brew tap xiaohk/clip2imgur
 $ brew install clip2imgur
 ```
 
-### Download the Binary
+### PyPI
 
-You can download the pre-compiled binary from the
-[Latest Rease](https://github.com/xiaohk/clip2imgur/releases/latest). After
-extract the binary, you want to create a symbolic link in `/usr/local/bin` to
-launch `clip2imgur` in your terminal more quickly.
+If you are familiar with Python, you can install `clip2imgur` with pip.
 
 ```
-$ mkdir ~/clip2imgur && cd ~/clip2imgur
-$ curl -O https://github.com/xiaohk/clip2imgur/releases/download/v0.9/clip2imgur-0.9.0.tar.gz
-$ tar -xvzf clip2imgur-0.9.0.tar.gz
-$ ln -s ~/clip2imgur/clip2imgur /usr/local/bin/clip2imgur
+$ pip install clip2imgur
 ```
 
-### Build from Source
-
-This approach is not recommended, because a function used to refresh your
-authorization is not open sourced for security reasons. Your compiled version
-works fine, but may require you to re-authorize `clip2imgur` periodically. If
-you only want to post images anonymously, then it doesn't really matter.
-
-To build `clip2imgur`, you need macOS 10.10 or later and Swift 3.0 or above.
-
-```
-$ git clone https://github.com/xiaohk/clip2imgur.git
-$ cd clip2imgur
-$ swift build -c release -Xswiftc -static-stdlib
-$ ln -s $(pwd)/.build/release/clip2imgur /usr/local/bin/clip2imgur
-```
+## Built With
 
-`clip2imgur` also has a by-product framework `clip2imgurCore` in `./build`.
-There might be some handy functions to use in your own projects.
+The latest version (>=v0.9.1) uses Python.
 
-## Built With
+The first version (v0.9.0) was built with:
 
 - [Swift Package Manager](https://swift.org/package-manager/)
 - [Rainbow](https://github.com/onevcat/Rainbow)
```

### Comparing `clip2imgur-0.9.3/clip2imgur/.DS_Store` & `clip2imgur-0.9.4/clip2imgur/.DS_Store`

 * *Files identical despite different names*

### Comparing `clip2imgur-0.9.3/clip2imgur/__pycache__/clip2imgur.cpython-310.pyc` & `clip2imgur-0.9.4/clip2imgur/__pycache__/clip2imgur.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `clip2imgur-0.9.3/clip2imgur/clip2imgur.py` & `clip2imgur-0.9.4/clip2imgur/clip2imgur.py`

 * *Files identical despite different names*

### Comparing `clip2imgur-0.9.3/setup.py` & `clip2imgur-0.9.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from json import loads
 from setuptools import setup, find_packages
 from pathlib import Path
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-requirements = ["pyobjc-framework-Cocoa", "pyperclip", "rich"]
+requirements = ["pyobjc-framework-Cocoa", "pyperclip", "rich", "requests"]
 
 test_requirements = []
 
 setup(
     author="Jay Wang",
     author_email="jayw@zijie.wang",
     python_requires=">=3.6",
@@ -43,15 +43,15 @@
     long_description_content_type="text/markdown",
     include_package_data=True,
     name="clip2imgur",
     packages=find_packages(include=["clip2imgur", "clip2imgur.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/xiaohk/clip2imgur",
-    version="0.9.3",
+    version="0.9.4",
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "clip2imgur=clip2imgur.clip2imgur:main",
         ],
     },
 )
```

### Comparing `clip2imgur-0.9.3/tests/test_clip2imgur.py` & `clip2imgur-0.9.4/tests/test_clip2imgur.py`

 * *Files identical despite different names*

