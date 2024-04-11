# Comparing `tmp/wormhole-tx-1.0.5.tar.gz` & `tmp/wormhole-tx-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wormhole-tx-1.0.5.tar", last modified: Sat Feb 17 23:15:22 2024, max compression
+gzip compressed data, was "wormhole-tx-1.0.6.tar", last modified: Thu Apr 11 21:16:48 2024, max compression
```

## Comparing `wormhole-tx-1.0.5.tar` & `wormhole-tx-1.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-02-17 23:15:22.390154 wormhole-tx-1.0.5/
-drwxrwxrwx   0        0        0        0 2024-02-17 23:15:22.348153 wormhole-tx-1.0.5/.github/
-drwxrwxrwx   0        0        0        0 2024-02-17 23:15:22.374153 wormhole-tx-1.0.5/.github/workflows/
--rw-rw-rw-   0        0        0      855 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      801 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/.github/workflows/push_macos.yml
--rw-rw-rw-   0        0        0      803 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/.github/workflows/push_ubuntu.yml
--rw-rw-rw-   0        0        0      800 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     1909 2024-02-08 21:58:57.000000 wormhole-tx-1.0.5/.gitignore
--rw-rw-rw-   0        0        0      186 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/.pylintrc
-drwxrwxrwx   0        0        0        0 2024-02-17 23:15:22.377154 wormhole-tx-1.0.5/.vscode/
--rw-rw-rw-   0        0        0     1354 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/.vscode/launch.json
--rw-rw-rw-   0        0        0      820 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/.vscode/settings.json
--rw-rw-rw-   0        0        0     1109 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1064 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      104 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2121 2024-02-17 23:15:22.390154 wormhole-tx-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1681 2024-02-13 00:45:08.000000 wormhole-tx-1.0.5/README.md
--rw-rw-rw-   0        0        0      519 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/activate.sh
--rw-rw-rw-   0        0        0       11 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/clean
--rw-rw-rw-   0        0        0     1725 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/install
--rw-rw-rw-   0        0        0     6950 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/install.py
--rw-rw-rw-   0        0        0      435 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/lint
--rw-rw-rw-   0        0        0      897 2024-02-17 23:15:10.000000 wormhole-tx-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       60 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/requirements.testing.txt
--rw-rw-rw-   0        0        0       42 2024-02-17 23:15:22.391155 wormhole-tx-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      428 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-17 23:15:22.351156 wormhole-tx-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-02-17 23:15:22.379155 wormhole-tx-1.0.5/src/tx/
--rw-rw-rw-   0        0        0        0 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/src/tx/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-17 23:15:22.381155 wormhole-tx-1.0.5/src/tx/assets/
--rw-rw-rw-   0        0        0       54 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/src/tx/assets/example.txt
--rw-rw-rw-   0        0        0     3683 2024-02-13 00:44:22.000000 wormhole-tx-1.0.5/src/tx/cli.py
-drwxrwxrwx   0        0        0        0 2024-02-17 23:15:22.388153 wormhole-tx-1.0.5/src/wormhole_tx.egg-info/
--rw-rw-rw-   0        0        0     2121 2024-02-17 23:15:22.000000 wormhole-tx-1.0.5/src/wormhole_tx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      671 2024-02-17 23:15:22.000000 wormhole-tx-1.0.5/src/wormhole_tx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-17 23:15:22.000000 wormhole-tx-1.0.5/src/wormhole_tx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-02-17 23:15:22.000000 wormhole-tx-1.0.5/src/wormhole_tx.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-02-17 23:15:22.000000 wormhole-tx-1.0.5/src/wormhole_tx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2024-02-17 23:15:22.000000 wormhole-tx-1.0.5/src/wormhole_tx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/test
-drwxrwxrwx   0        0        0        0 2024-02-17 23:15:22.389153 wormhole-tx-1.0.5/tests/
--rw-rw-rw-   0        0        0      364 2024-02-07 06:55:03.000000 wormhole-tx-1.0.5/tests/test_cli.py
--rw-rw-rw-   0        0        0      510 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/tox.ini
--rw-rw-rw-   0        0        0      291 2024-02-07 06:45:14.000000 wormhole-tx-1.0.5/upload_package.sh
+drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.273988 wormhole-tx-1.0.6/
+drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.227989 wormhole-tx-1.0.6/.github/
+drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.256987 wormhole-tx-1.0.6/.github/workflows/
+-rw-rw-rw-   0        0        0      855 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      801 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.github/workflows/push_macos.yml
+-rw-rw-rw-   0        0        0      803 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.github/workflows/push_ubuntu.yml
+-rw-rw-rw-   0        0        0      800 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.github/workflows/push_win.yml
+-rw-rw-rw-   0        0        0     1909 2024-02-08 21:58:57.000000 wormhole-tx-1.0.6/.gitignore
+-rw-rw-rw-   0        0        0      186 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.pylintrc
+drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.259987 wormhole-tx-1.0.6/.vscode/
+-rw-rw-rw-   0        0        0     1354 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.vscode/launch.json
+-rw-rw-rw-   0        0        0      820 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1109 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1064 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      104 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2206 2024-04-11 21:16:48.272987 wormhole-tx-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1766 2024-04-11 21:16:19.000000 wormhole-tx-1.0.6/README.md
+-rw-rw-rw-   0        0        0      519 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/activate.sh
+-rw-rw-rw-   0        0        0       11 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/clean
+-rw-rw-rw-   0        0        0     1725 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/install
+-rw-rw-rw-   0        0        0     6950 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/install.py
+-rw-rw-rw-   0        0        0      447 2024-04-11 21:15:37.000000 wormhole-tx-1.0.6/lint
+-rw-rw-rw-   0        0        0      897 2024-04-11 21:15:57.000000 wormhole-tx-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       60 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/requirements.testing.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 21:16:48.273988 wormhole-tx-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      428 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.229988 wormhole-tx-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.261987 wormhole-tx-1.0.6/src/tx/
+-rw-rw-rw-   0        0        0        0 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/src/tx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.262987 wormhole-tx-1.0.6/src/tx/assets/
+-rw-rw-rw-   0        0        0       54 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/src/tx/assets/example.txt
+-rw-rw-rw-   0        0        0     4028 2024-04-11 21:15:15.000000 wormhole-tx-1.0.6/src/tx/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.270987 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/
+-rw-rw-rw-   0        0        0     2206 2024-04-11 21:16:48.000000 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      671 2024-04-11 21:16:48.000000 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 21:16:48.000000 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-11 21:16:48.000000 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-11 21:16:48.000000 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2024-04-11 21:16:48.000000 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/test
+drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.271988 wormhole-tx-1.0.6/tests/
+-rw-rw-rw-   0        0        0      364 2024-02-07 06:55:03.000000 wormhole-tx-1.0.6/tests/test_cli.py
+-rw-rw-rw-   0        0        0      510 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/tox.ini
+-rw-rw-rw-   0        0        0      291 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/upload_package.sh
```

### Comparing `wormhole-tx-1.0.5/.github/workflows/lint.yml` & `wormhole-tx-1.0.6/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.5/.github/workflows/push_macos.yml` & `wormhole-tx-1.0.6/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.5/.github/workflows/push_ubuntu.yml` & `wormhole-tx-1.0.6/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.5/.github/workflows/push_win.yml` & `wormhole-tx-1.0.6/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.5/.gitignore` & `wormhole-tx-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.5/.vscode/launch.json` & `wormhole-tx-1.0.6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.5/.vscode/settings.json` & `wormhole-tx-1.0.6/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.5/.vscode/tasks.json` & `wormhole-tx-1.0.6/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.5/LICENSE` & `wormhole-tx-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.5/PKG-INFO` & `wormhole-tx-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wormhole-tx
-Version: 1.0.5
+Version: 1.0.6
 Summary: Front end for wormhole, easier and more secure!
 Home-page: https://github.com/zackees/tx
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -55,11 +55,11 @@
 This environment requires you to use `git-bash`.
 
 # Linting
 
 Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
 
 # Versions
-
+  * 1.0.6: Varius fixes and force UTF-8 on Windows to prevent crash during file send.
   * 1.0.3: Removes new typing system which doesn't work on python < 3.10
   * 1.0.2: Unknown arguments are passed onto `wormhole send`. Help now displays `wormhole --help`.
   * 1.0.1: Fixes missing `magic-wormhole` dependency.
```

### Comparing `wormhole-tx-1.0.5/README.md` & `wormhole-tx-1.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -42,11 +42,11 @@
 This environment requires you to use `git-bash`.
 
 # Linting
 
 Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
 
 # Versions
-
+  * 1.0.6: Varius fixes and force UTF-8 on Windows to prevent crash during file send.
   * 1.0.3: Removes new typing system which doesn't work on python < 3.10
   * 1.0.2: Unknown arguments are passed onto `wormhole send`. Help now displays `wormhole --help`.
   * 1.0.1: Fixes missing `magic-wormhole` dependency.
```

### Comparing `wormhole-tx-1.0.5/activate.sh` & `wormhole-tx-1.0.6/activate.sh`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.5/install` & `wormhole-tx-1.0.6/install`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.5/install.py` & `wormhole-tx-1.0.6/install.py`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.5/pyproject.toml` & `wormhole-tx-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 keywords = ["template-python-cmd"]
 license = { text = "BSD 3-Clause License" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
     "magic-wormhole",
 ]
 # Change this with the version number bump.
-version = "1.0.5"
+version = "1.0.6"
 
 [tool.ruff]
 line-length = 200
 
 [tool.pylint."MESSAGES CONTROL"]
 good-names = [
     "c",
```

### Comparing `wormhole-tx-1.0.5/src/tx/cli.py` & `wormhole-tx-1.0.6/src/tx/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,20 @@
 import os
 import secrets
 import subprocess
 import sys
 import warnings
 from typing import IO, Optional
 
+from colorama import just_fix_windows_console
+
 KEY_LENGTH = 32
 
+just_fix_windows_console()
+
 
 def gen_code(key_length: int) -> str:
     """Returns a random number string of the given length."""
     # only numbers
     return "".join([str(secrets.randbelow(10)) for _ in range(key_length)])
 
 
@@ -77,23 +81,28 @@
         file_or_dir = args.file_or_dir
         if not os.path.exists(file_or_dir):
             print(f"File or directory {file_or_dir} does not exist.")
             return 1
         code = args.code or gen_code(args.code_length)
         recieve_cmd = gen_wormhole_receive_command(code)
         cmd_list = ["wormhole", "send", file_or_dir, "--code", code] + unknown
+        if sys.platform == "win32":
+            # On windows, we need to use chcp 65501 to support UTF-8 or else
+            # we get an error when sending files with non-ascii characters
+            cmd_list = ["chcp", "65001", "&&"] + cmd_list
         print(f'\nSending "{file_or_dir}"...')
         print("On the other computer, run the following command:\n")
         print("    " + recieve_cmd)
         print("")
         proc = subprocess.Popen(
             cmd_list,
             universal_newlines=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
+            shell=True,
         )
         assert proc.stdout is not None
         assert proc.stderr is None
         # stream out stdout line by line
         for line in iter(proc.stdout.readline, ""):
             if "Sending" in line and "kB file" in line:
                 continue
```

### Comparing `wormhole-tx-1.0.5/src/wormhole_tx.egg-info/PKG-INFO` & `wormhole-tx-1.0.6/src/wormhole_tx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wormhole-tx
-Version: 1.0.5
+Version: 1.0.6
 Summary: Front end for wormhole, easier and more secure!
 Home-page: https://github.com/zackees/tx
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -55,11 +55,11 @@
 This environment requires you to use `git-bash`.
 
 # Linting
 
 Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
 
 # Versions
-
+  * 1.0.6: Varius fixes and force UTF-8 on Windows to prevent crash during file send.
   * 1.0.3: Removes new typing system which doesn't work on python < 3.10
   * 1.0.2: Unknown arguments are passed onto `wormhole send`. Help now displays `wormhole --help`.
   * 1.0.1: Fixes missing `magic-wormhole` dependency.
```

### Comparing `wormhole-tx-1.0.5/src/wormhole_tx.egg-info/SOURCES.txt` & `wormhole-tx-1.0.6/src/wormhole_tx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

