# Comparing `tmp/language_tool_python-2.7.3.tar.gz` & `tmp/language_tool_python-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "language_tool_python-2.7.3.tar", last modified: Tue Mar 12 15:37:34 2024, max compression
+gzip compressed data, was "language_tool_python-2.8.tar", last modified: Thu Apr 11 20:50:26 2024, max compression
```

## Comparing `language_tool_python-2.7.3.tar` & `language_tool_python-2.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 johnmorris   (501) staff       (20)        0 2024-03-12 15:37:34.018556 language_tool_python-2.7.3/
--rw-r--r--   0 johnmorris   (501) staff       (20)    35151 2021-09-14 18:23:37.000000 language_tool_python-2.7.3/LICENSE
--rw-r--r--   0 johnmorris   (501) staff       (20)      204 2021-11-22 13:56:11.000000 language_tool_python-2.7.3/MANIFEST.in
--rw-r--r--   0 johnmorris   (501) staff       (20)    12625 2024-03-12 15:37:34.018221 language_tool_python-2.7.3/PKG-INFO
--rw-r--r--   0 johnmorris   (501) staff       (20)    12300 2024-03-12 15:29:35.000000 language_tool_python-2.7.3/README.md
-drwxr-xr-x   0 johnmorris   (501) staff       (20)        0 2024-03-12 15:37:34.016884 language_tool_python-2.7.3/language_tool_python/
--rw-r--r--   0 johnmorris   (501) staff       (20)      248 2021-09-14 18:23:37.000000 language_tool_python-2.7.3/language_tool_python/__init__.py
--rw-r--r--   0 johnmorris   (501) staff       (20)     6199 2021-09-14 18:23:37.000000 language_tool_python-2.7.3/language_tool_python/__main__.py
--rw-r--r--   0 johnmorris   (501) staff       (20)     7220 2022-01-12 15:00:47.000000 language_tool_python-2.7.3/language_tool_python/config_file.py
--rw-r--r--   0 johnmorris   (501) staff       (20)     2085 2021-09-14 18:23:37.000000 language_tool_python-2.7.3/language_tool_python/console_mode.py
--rwxr-xr-x   0 johnmorris   (501) staff       (20)     5480 2024-03-12 15:29:35.000000 language_tool_python-2.7.3/language_tool_python/download_lt.py
--rw-r--r--   0 johnmorris   (501) staff       (20)     1218 2021-09-14 19:08:12.000000 language_tool_python-2.7.3/language_tool_python/language_tag.py
--rw-r--r--   0 johnmorris   (501) staff       (20)     4721 2021-09-14 18:23:37.000000 language_tool_python-2.7.3/language_tool_python/match.py
--rw-r--r--   0 johnmorris   (501) staff       (20)    13215 2022-01-12 15:09:46.000000 language_tool_python-2.7.3/language_tool_python/server.py
--rw-r--r--   0 johnmorris   (501) staff       (20)     3744 2022-01-12 15:01:09.000000 language_tool_python-2.7.3/language_tool_python/utils.py
--rw-r--r--   0 johnmorris   (501) staff       (20)     1828 2021-09-14 18:23:37.000000 language_tool_python-2.7.3/language_tool_python/which.py
-drwxr-xr-x   0 johnmorris   (501) staff       (20)        0 2024-03-12 15:37:34.017935 language_tool_python-2.7.3/language_tool_python.egg-info/
--rw-r--r--   0 johnmorris   (501) staff       (20)    12625 2024-03-12 15:37:33.000000 language_tool_python-2.7.3/language_tool_python.egg-info/PKG-INFO
--rw-r--r--   0 johnmorris   (501) staff       (20)      622 2024-03-12 15:37:33.000000 language_tool_python-2.7.3/language_tool_python.egg-info/SOURCES.txt
--rw-r--r--   0 johnmorris   (501) staff       (20)        1 2024-03-12 15:37:33.000000 language_tool_python-2.7.3/language_tool_python.egg-info/dependency_links.txt
--rw-r--r--   0 johnmorris   (501) staff       (20)       14 2024-03-12 15:37:33.000000 language_tool_python-2.7.3/language_tool_python.egg-info/requires.txt
--rw-r--r--   0 johnmorris   (501) staff       (20)       21 2024-03-12 15:37:33.000000 language_tool_python-2.7.3/language_tool_python.egg-info/top_level.txt
--rw-r--r--   0 johnmorris   (501) staff       (20)       14 2021-09-14 18:23:37.000000 language_tool_python-2.7.3/requirements.txt
--rwxr-xr-x   0 johnmorris   (501) staff       (20)     1306 2021-09-14 18:23:37.000000 language_tool_python-2.7.3/run_doctest.py
--rw-r--r--   0 johnmorris   (501) staff       (20)       38 2024-03-12 15:37:34.018616 language_tool_python-2.7.3/setup.cfg
--rwxr-xr-x   0 johnmorris   (501) staff       (20)      674 2024-03-12 15:37:18.000000 language_tool_python-2.7.3/setup.py
+drwxr-xr-x   0 johnmorris   (501) staff       (20)        0 2024-04-11 20:50:26.228829 language_tool_python-2.8/
+-rw-r--r--   0 johnmorris   (501) staff       (20)    35151 2021-09-14 18:23:37.000000 language_tool_python-2.8/LICENSE
+-rw-r--r--   0 johnmorris   (501) staff       (20)      204 2021-11-22 13:56:11.000000 language_tool_python-2.8/MANIFEST.in
+-rw-r--r--   0 johnmorris   (501) staff       (20)    12887 2024-04-11 20:50:26.228649 language_tool_python-2.8/PKG-INFO
+-rw-r--r--   0 johnmorris   (501) staff       (20)    12564 2024-04-11 20:49:16.000000 language_tool_python-2.8/README.md
+drwxr-xr-x   0 johnmorris   (501) staff       (20)        0 2024-04-11 20:50:26.227813 language_tool_python-2.8/language_tool_python/
+-rw-r--r--   0 johnmorris   (501) staff       (20)      248 2021-09-14 18:23:37.000000 language_tool_python-2.8/language_tool_python/__init__.py
+-rw-r--r--   0 johnmorris   (501) staff       (20)     6199 2024-04-11 20:49:16.000000 language_tool_python-2.8/language_tool_python/__main__.py
+-rw-r--r--   0 johnmorris   (501) staff       (20)     7220 2022-01-12 15:00:47.000000 language_tool_python-2.8/language_tool_python/config_file.py
+-rw-r--r--   0 johnmorris   (501) staff       (20)     2085 2021-09-14 18:23:37.000000 language_tool_python-2.8/language_tool_python/console_mode.py
+-rwxr-xr-x   0 johnmorris   (501) staff       (20)     6031 2024-04-11 20:49:16.000000 language_tool_python-2.8/language_tool_python/download_lt.py
+-rw-r--r--   0 johnmorris   (501) staff       (20)     1218 2021-09-14 19:08:12.000000 language_tool_python-2.8/language_tool_python/language_tag.py
+-rw-r--r--   0 johnmorris   (501) staff       (20)     4721 2021-09-14 18:23:37.000000 language_tool_python-2.8/language_tool_python/match.py
+-rw-r--r--   0 johnmorris   (501) staff       (20)    14088 2024-04-11 20:49:16.000000 language_tool_python-2.8/language_tool_python/server.py
+-rw-r--r--   0 johnmorris   (501) staff       (20)     4438 2024-04-11 20:49:16.000000 language_tool_python-2.8/language_tool_python/utils.py
+-rw-r--r--   0 johnmorris   (501) staff       (20)     1828 2021-09-14 18:23:37.000000 language_tool_python-2.8/language_tool_python/which.py
+drwxr-xr-x   0 johnmorris   (501) staff       (20)        0 2024-04-11 20:50:26.228476 language_tool_python-2.8/language_tool_python.egg-info/
+-rw-r--r--   0 johnmorris   (501) staff       (20)    12887 2024-04-11 20:50:26.000000 language_tool_python-2.8/language_tool_python.egg-info/PKG-INFO
+-rw-r--r--   0 johnmorris   (501) staff       (20)      622 2024-04-11 20:50:26.000000 language_tool_python-2.8/language_tool_python.egg-info/SOURCES.txt
+-rw-r--r--   0 johnmorris   (501) staff       (20)        1 2024-04-11 20:50:26.000000 language_tool_python-2.8/language_tool_python.egg-info/dependency_links.txt
+-rw-r--r--   0 johnmorris   (501) staff       (20)       24 2024-04-11 20:50:26.000000 language_tool_python-2.8/language_tool_python.egg-info/requires.txt
+-rw-r--r--   0 johnmorris   (501) staff       (20)       21 2024-04-11 20:50:26.000000 language_tool_python-2.8/language_tool_python.egg-info/top_level.txt
+-rw-r--r--   0 johnmorris   (501) staff       (20)       24 2024-04-11 20:49:16.000000 language_tool_python-2.8/requirements.txt
+-rwxr-xr-x   0 johnmorris   (501) staff       (20)     1306 2021-09-14 18:23:37.000000 language_tool_python-2.8/run_doctest.py
+-rw-r--r--   0 johnmorris   (501) staff       (20)       38 2024-04-11 20:50:26.228870 language_tool_python-2.8/setup.cfg
+-rwxr-xr-x   0 johnmorris   (501) staff       (20)      672 2024-04-11 20:49:34.000000 language_tool_python-2.8/setup.py
```

### Comparing `language_tool_python-2.7.3/LICENSE` & `language_tool_python-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `language_tool_python-2.7.3/PKG-INFO` & `language_tool_python-2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,14 @@
-Metadata-Version: 2.1
-Name: language_tool_python
-Version: 2.7.3
-Summary: Checks grammar using LanguageTool.
-Home-page: https://github.com/jxmorris12/language_tool_python
-Author: Jack Morris
-Author-email: jxmorris12@gmail.com
-License: GNU GPL
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # `language_tool_python`: a grammar checker for Python 📝
 
 ![language tool python on pypi](https://badge.fury.io/py/language-tool-python.svg)
 
 ![Test with PyTest](https://github.com/jxmorris12/language_tool_python/workflows/Test%20with%20PyTest/badge.svg)
 
-Current LanguageTool version: **5.5**
+Current LanguageTool version: **6.4**
 
 This is a Python wrapper for [LanguageTool](https://languagetool.org). LanguageTool is open-source grammar tool, also known as the spellchecker for OpenOffice. This library allows you to make to detect grammar errors and spelling mistakes through a Python script or through a command-line interface.
 
 ## Local and Remote Servers
 
 By default, `language_tool_python` will download a LanguageTool server `.jar` and run that in the background to detect grammar errors locally. However, LanguageTool also offers a [Public HTTP Proofreading API](https://dev.languagetool.org/public-http-api) that is supported as well. Follow the link for rate limiting details. (Running locally won't have the same restrictions.)
 
@@ -159,15 +147,15 @@
 >>> lang_tool.check('helo darknes my old frend')
 [Match({'ruleId': 'UPPERCASE_SENTENCE_START', 'message': 'This sentence does not start with an uppercase letter.', 'replacements': ['Helo'], 'offsetInContext': 0, 'context': 'helo darknes my old frend', 'offset': 0, 'errorLength': 4, 'category': 'CASING', 'ruleIssueType': 'typographical', 'sentence': 'helo darknes my old frend'}), Match({'ruleId': 'MORFOLOGIK_RULE_EN_US', 'message': 'Possible spelling mistake found.', 'replacements': ['darkness', 'darkens', 'darkies'], 'offsetInContext': 5, 'context': 'helo darknes my old frend', 'offset': 5, 'errorLength': 7, 'category': 'TYPOS', 'ruleIssueType': 'misspelling', 'sentence': 'helo darknes my old frend'}), Match({'ruleId': 'MORFOLOGIK_RULE_EN_US', 'message': 'Possible spelling mistake found.', 'replacements': ['friend', 'trend', 'Fred', 'freed', 'Freud', 'Friend', 'fend', 'fiend', 'frond', 'rend', 'fr end'], 'offsetInContext': 20, 'context': 'helo darknes my old frend', 'offset': 20, 'errorLength': 5, 'category': 'TYPOS', 'ruleIssueType': 'misspelling', 'sentence': 'helo darknes my old frend'})]
 >>>
 ```
 
 ## Configuration
 
-LanguageTool offers lots of built-in configuration options. 
+LanguageTool offers lots of built-in configuration options.
 
 ### Example: Enabling caching
 Here's an example of using the configuration options to enable caching. Some users have reported that this helps performance a lot.
 ```python
 import language_tool_python
 tool = language_tool_python.LanguageTool('en-US', config={ 'cacheSize': 1000, 'pipelineCaching': True })
 ```
@@ -230,21 +218,28 @@
 
 ### What rules does LanguageTool have?
 
 Searching for a specific rule to enable or disable? Curious the breadth of rules LanguageTool applies? This page contains a massive list of all 5,000+ grammatical rules that are programmed into LanguageTool: https://community.languagetool.org/rule/list?lang=en&offset=30&max=10
 
 ### Customizing Download URL or Path
 
+If LanguageTool is already installed on your system, you can defined the following environment variable:
+```bash
+$ export LTP_JAR_DIR_PATH = /path/to/the/language/tool/jar/files
+```
+
+Overwise, `language_tool_python` can download LanguageTool for you automatically.
+
 To overwrite the host part of URL that is used to download LanguageTool-{version}.zip:
 
 ```bash
 $ export LTP_DOWNLOAD_HOST = [alternate URL]
 ```
 
-This can be used to downgrade to an older version, for example, or to download from a mirror. 
+This can be used to downgrade to an older version, for example, or to download from a mirror.
 
 And to choose the specific folder to download the server to:
 
 ```bash
 $ export LTP_PATH = /path/to/save/language/tool
 ```
 
@@ -260,12 +255,11 @@
 [LanguageTool-stable.zip](https://www.languagetool.org/download/LanguageTool-stable.zip) and unzip it
 into where the ``language_tool_python`` package resides.
 
 ### LanguageTool Version
 
 As of April 2020, `language_tool_python` was forked from `language-check` and no longer supports LanguageTool versions lower than 4.0.
 
-### Acknowledgements 
+### Acknowledgements
+
 This is a fork of https://github.com/myint/language-check/ that produces more easily parsable
 results from the command-line.
-
-
```

### Comparing `language_tool_python-2.7.3/README.md` & `language_tool_python-2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,26 @@
+Metadata-Version: 2.1
+Name: language_tool_python
+Version: 2.8
+Summary: Checks grammar using LanguageTool.
+Home-page: https://github.com/jxmorris12/language_tool_python
+Author: Jack Morris
+Author-email: jxmorris12@gmail.com
+License: GNU GPL
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # `language_tool_python`: a grammar checker for Python 📝
 
 ![language tool python on pypi](https://badge.fury.io/py/language-tool-python.svg)
 
 ![Test with PyTest](https://github.com/jxmorris12/language_tool_python/workflows/Test%20with%20PyTest/badge.svg)
 
-Current LanguageTool version: **5.5**
+Current LanguageTool version: **6.4**
 
 This is a Python wrapper for [LanguageTool](https://languagetool.org). LanguageTool is open-source grammar tool, also known as the spellchecker for OpenOffice. This library allows you to make to detect grammar errors and spelling mistakes through a Python script or through a command-line interface.
 
 ## Local and Remote Servers
 
 By default, `language_tool_python` will download a LanguageTool server `.jar` and run that in the background to detect grammar errors locally. However, LanguageTool also offers a [Public HTTP Proofreading API](https://dev.languagetool.org/public-http-api) that is supported as well. Follow the link for rate limiting details. (Running locally won't have the same restrictions.)
 
@@ -147,15 +159,15 @@
 >>> lang_tool.check('helo darknes my old frend')
 [Match({'ruleId': 'UPPERCASE_SENTENCE_START', 'message': 'This sentence does not start with an uppercase letter.', 'replacements': ['Helo'], 'offsetInContext': 0, 'context': 'helo darknes my old frend', 'offset': 0, 'errorLength': 4, 'category': 'CASING', 'ruleIssueType': 'typographical', 'sentence': 'helo darknes my old frend'}), Match({'ruleId': 'MORFOLOGIK_RULE_EN_US', 'message': 'Possible spelling mistake found.', 'replacements': ['darkness', 'darkens', 'darkies'], 'offsetInContext': 5, 'context': 'helo darknes my old frend', 'offset': 5, 'errorLength': 7, 'category': 'TYPOS', 'ruleIssueType': 'misspelling', 'sentence': 'helo darknes my old frend'}), Match({'ruleId': 'MORFOLOGIK_RULE_EN_US', 'message': 'Possible spelling mistake found.', 'replacements': ['friend', 'trend', 'Fred', 'freed', 'Freud', 'Friend', 'fend', 'fiend', 'frond', 'rend', 'fr end'], 'offsetInContext': 20, 'context': 'helo darknes my old frend', 'offset': 20, 'errorLength': 5, 'category': 'TYPOS', 'ruleIssueType': 'misspelling', 'sentence': 'helo darknes my old frend'})]
 >>>
 ```
 
 ## Configuration
 
-LanguageTool offers lots of built-in configuration options. 
+LanguageTool offers lots of built-in configuration options.
 
 ### Example: Enabling caching
 Here's an example of using the configuration options to enable caching. Some users have reported that this helps performance a lot.
 ```python
 import language_tool_python
 tool = language_tool_python.LanguageTool('en-US', config={ 'cacheSize': 1000, 'pipelineCaching': True })
 ```
@@ -218,21 +230,28 @@
 
 ### What rules does LanguageTool have?
 
 Searching for a specific rule to enable or disable? Curious the breadth of rules LanguageTool applies? This page contains a massive list of all 5,000+ grammatical rules that are programmed into LanguageTool: https://community.languagetool.org/rule/list?lang=en&offset=30&max=10
 
 ### Customizing Download URL or Path
 
+If LanguageTool is already installed on your system, you can defined the following environment variable:
+```bash
+$ export LTP_JAR_DIR_PATH = /path/to/the/language/tool/jar/files
+```
+
+Overwise, `language_tool_python` can download LanguageTool for you automatically.
+
 To overwrite the host part of URL that is used to download LanguageTool-{version}.zip:
 
 ```bash
 $ export LTP_DOWNLOAD_HOST = [alternate URL]
 ```
 
-This can be used to downgrade to an older version, for example, or to download from a mirror. 
+This can be used to downgrade to an older version, for example, or to download from a mirror.
 
 And to choose the specific folder to download the server to:
 
 ```bash
 $ export LTP_PATH = /path/to/save/language/tool
 ```
 
@@ -248,10 +267,13 @@
 [LanguageTool-stable.zip](https://www.languagetool.org/download/LanguageTool-stable.zip) and unzip it
 into where the ``language_tool_python`` package resides.
 
 ### LanguageTool Version
 
 As of April 2020, `language_tool_python` was forked from `language-check` and no longer supports LanguageTool versions lower than 4.0.
 
-### Acknowledgements 
+### Acknowledgements
+
 This is a fork of https://github.com/myint/language-check/ that produces more easily parsable
 results from the command-line.
+
+
```

### Comparing `language_tool_python-2.7.3/language_tool_python/__main__.py` & `language_tool_python-2.8/language_tool_python/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import locale
 import re
 import sys
 
 from .server import LanguageTool
 from .utils import LanguageToolError
 
-import pkg_resources 
+import pkg_resources
 __version__ = pkg_resources.require("language_tool_python")[0].version
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description=__doc__.strip() if __doc__ else None,
         prog='language_tool_python')
@@ -171,8 +171,8 @@
         except LanguageToolError as exception:
             print('{}: {}'.format(filename, exception), file=sys.stderr)
             continue
 
     return status
 
 
-sys.exit(main())
+sys.exit(main())
```

### Comparing `language_tool_python-2.7.3/language_tool_python/config_file.py` & `language_tool_python-2.8/language_tool_python/config_file.py`

 * *Files identical despite different names*

### Comparing `language_tool_python-2.7.3/language_tool_python/console_mode.py` & `language_tool_python-2.8/language_tool_python/console_mode.py`

 * *Files identical despite different names*

### Comparing `language_tool_python-2.7.3/language_tool_python/download_lt.py` & `language_tool_python-2.8/language_tool_python/download_lt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """Download latest LanguageTool distribution."""
 
-import glob
 import logging
 import os
 import re
 import requests
 import subprocess
 import sys
 import tempfile
 import tqdm
+from typing import Optional
 import zipfile
 
 from distutils.spawn import find_executable
 from urllib.parse import urljoin
-from .utils import get_language_tool_download_path
+from .utils import (
+    find_existing_language_tool_downloads,
+    get_language_tool_download_path,
+    LTP_JAR_DIR_PATH_ENV_VAR
+)
 
 # Create logger for this file.
 logging.basicConfig(format='%(message)s')
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
 # Get download host from environment or default.
 BASE_URL = os.environ.get('LTP_DOWNLOAD_HOST', 'https://www.languagetool.org/download/')
 FILENAME = 'LanguageTool-{version}.zip'
 
-LATEST_VERSION = '6.2'
+LTP_DOWNLOAD_VERSION = '6.4'
 
 JAVA_VERSION_REGEX = re.compile(
     r'^(?:java|openjdk) version "(?P<major1>\d+)(|\.(?P<major2>\d+)\.[^"]+)"',
     re.MULTILINE)
 
 # Updated for later versions of java
 JAVA_VERSION_REGEX_UPDATED = re.compile(
@@ -52,68 +56,83 @@
     ... openjdk version "1.8.0_60"
     ... OpenJDK Runtime Environment (build 1.8.0_60-b27)
     ... OpenJDK 64-Bit Server VM (build 25.60-b23, mixed mode))
     ... ''')
     (1, 8)
 
     """
-    match = re.search(JAVA_VERSION_REGEX, version_text) or re.search(JAVA_VERSION_REGEX_UPDATED, version_text)
+    match = (
+        re.search(JAVA_VERSION_REGEX, version_text)
+        or re.search(JAVA_VERSION_REGEX_UPDATED, version_text)
+    )
     if not match:
         raise SystemExit(
             'Could not parse Java version from """{}""".'.format(version_text))
     major1 = int(match.group('major1'))
     major2 = int(match.group('major2')) if match.group('major2') else 0
     return (major1, major2)
 
+
 def confirm_java_compatibility():
     """ Confirms Java major version >= 8. """
     java_path = find_executable('java')
     if not java_path:
-        raise ModuleNotFoundError('No java install detected. Please install java to use language-tool-python.')
+        raise ModuleNotFoundError(
+            'No java install detected. '
+            'Please install java to use language-tool-python.'
+        )
 
     output = subprocess.check_output([java_path, '-version'],
                                      stderr=subprocess.STDOUT,
                                      universal_newlines=True)
 
     major_version, minor_version = parse_java_version(output)
-    # Some installs of java show the version number like `14.0.1` and others show `1.14.0.1`
-    # (with a leading 1). We want to support both, as long as the major version is >= 8.
+    # Some installs of java show the version number like `14.0.1`
+    # and others show `1.14.0.1`
+    # (with a leading 1). We want to support both,
+    # as long as the major version is >= 8.
     # (See softwareengineering.stackexchange.com/questions/175075/why-is-java-version-1-x-referred-to-as-java-x)
     if major_version == 1 and minor_version >= 8:
         return True
     elif major_version >= 8:
         return True
     else:
         raise SystemError('Detected java {}.{}. LanguageTool requires Java >= 8.'.format(major_version, minor_version))
 
+
 def get_common_prefix(z):
     """Get common directory in a zip file if any."""
     name_list = z.namelist()
     if name_list and all(n.startswith(name_list[0]) for n in name_list[1:]):
         return name_list[0]
     return None
 
+
 def http_get(url, out_file, proxies=None):
     """ Get contents of a URL and save to a file.
     """
     req = requests.get(url, stream=True, proxies=proxies)
     content_length = req.headers.get('Content-Length')
     total = int(content_length) if content_length is not None else None
-    if req.status_code == 403: # Not found on AWS
+    if req.status_code == 403:  # Not found on AWS
         raise Exception('Could not find at URL {}.'.format(url))
-    progress = tqdm.tqdm(unit="B", unit_scale=True, total=total, desc=f'Downloading LanguageTool {LATEST_VERSION}')
+    progress = tqdm.tqdm(unit="B", unit_scale=True, total=total,
+                         desc=f'Downloading LanguageTool {LTP_DOWNLOAD_VERSION}')
     for chunk in req.iter_content(chunk_size=1024):
-        if chunk: # filter out keep-alive new chunks
+        if chunk:  # filter out keep-alive new chunks
             progress.update(len(chunk))
             out_file.write(chunk)
     progress.close()
 
+
 def unzip_file(temp_file, directory_to_extract_to):
     """ Unzips a .zip file to folder path. """
-    logger.info('Unzipping {} to {}.'.format(temp_file.name, directory_to_extract_to))
+    logger.info(
+        'Unzipping {} to {}.'.format(temp_file.name, directory_to_extract_to)
+    )
     with zipfile.ZipFile(temp_file.name, 'r') as zip_ref:
         zip_ref.extractall(directory_to_extract_to)
 
 
 def download_zip(url, directory):
     """ Downloads and unzips zip file from `url` to `directory`. """
     # Download file.
@@ -124,30 +143,38 @@
     # Extract zip file to path.
     unzip_file(downloaded_file, directory)
     # Remove the temporary file.
     os.remove(downloaded_file.name)
     # Tell the user the download path.
     logger.info('Downloaded {} to {}.'.format(url, directory))
 
-def download_lt():
-    download_folder = get_language_tool_download_path()
-    assert os.path.isdir(download_folder)
-    old_path_list = [
-        path for path in
-        glob.glob(os.path.join(download_folder, 'LanguageTool*'))
-        if os.path.isdir(path)
-    ]
 
+def download_lt(language_tool_version: Optional[str] = LTP_DOWNLOAD_VERSION):
     confirm_java_compatibility()
-    version = LATEST_VERSION
-    filename = FILENAME.format(version=version)
-    language_tool_download_url = urljoin(BASE_URL, filename)
-    dirname, _ = os.path.splitext(filename)
-    extract_path = os.path.join(download_folder, dirname)
 
-    if extract_path in old_path_list:
+    download_folder = get_language_tool_download_path()
+
+    # Use the env var to the jar directory if it is defined
+    # otherwise look in the download directory
+    if os.environ.get(LTP_JAR_DIR_PATH_ENV_VAR):
         return
 
-    download_zip(language_tool_download_url, download_folder)
+    # Make download path, if it doesn't exist.
+    os.makedirs(download_folder, exist_ok=True)
+
+    assert os.path.isdir(download_folder)
+    old_path_list = find_existing_language_tool_downloads(download_folder)
+
+    if language_tool_version:
+        version = language_tool_version
+        filename = FILENAME.format(version=version)
+        language_tool_download_url = urljoin(BASE_URL, filename)
+        dirname, _ = os.path.splitext(filename)
+        extract_path = os.path.join(download_folder, dirname)
+
+        if extract_path in old_path_list:
+            return
+        download_zip(language_tool_download_url, download_folder)
+
 
 if __name__ == '__main__':
     sys.exit(download_lt())
```

### Comparing `language_tool_python-2.7.3/language_tool_python/language_tag.py` & `language_tool_python-2.8/language_tool_python/language_tag.py`

 * *Files identical despite different names*

### Comparing `language_tool_python-2.7.3/language_tool_python/match.py` & `language_tool_python-2.8/language_tool_python/match.py`

 * *Files identical despite different names*

### Comparing `language_tool_python-2.7.3/language_tool_python/server.py` & `language_tool_python-2.8/language_tool_python/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,47 +8,55 @@
 import requests
 import socket
 import subprocess
 import threading
 import urllib.parse
 
 from .config_file import LanguageToolConfig
-from .download_lt import download_lt
+from .download_lt import download_lt, LTP_DOWNLOAD_VERSION
 from .language_tag import LanguageTag
 from .match import Match
 from .utils import (
     correct,
-    parse_url, get_locale_language, get_language_tool_directory, get_server_cmd,
+    parse_url, get_locale_language,
+    get_language_tool_directory, get_server_cmd,
     FAILSAFE_LANGUAGE, startupinfo,
-    LanguageToolError, ServerError, JavaError, PathError)
+    LanguageToolError, ServerError, PathError
+)
 
 
 DEBUG_MODE = False
 
 # Keep track of running server PIDs in a global list. This way,
 # we can ensure they're killed on exit.
 RUNNING_SERVER_PROCESSES: List[subprocess.Popen] = []
 
+
 class LanguageTool:
-    """Main class used for checking text against different rules. 
-    LanguageTool v2 API documentation: https://languagetool.org/http-api/swagger-ui/#!/default/post_check
+    """Main class used for checking text against different rules.
+    LanguageTool v2 API documentation:
+    https://languagetool.org/http-api/swagger-ui/#!/default/post_check
     """
     _MIN_PORT = 8081
     _MAX_PORT = 8999
     _TIMEOUT = 5 * 60
     _remote = False
     _port = _MIN_PORT
     _server: subprocess.Popen = None
     _consumer_thread: threading.Thread = None
     _PORT_RE = re.compile(r"(?:https?://.*:|port\s+)(\d+)", re.I)
-    
-    def __init__(self,  language=None, motherTongue=None,
-                        remote_server=None, newSpellings=None,
-                        new_spellings_persist=True,
-                        host=None, config=None):
+
+    def __init__(
+            self, language=None, motherTongue=None,
+            remote_server=None, newSpellings=None,
+            new_spellings_persist=True,
+            host=None, config=None,
+            language_tool_download_version: str = LTP_DOWNLOAD_VERSION
+    ):
+        self.language_tool_download_version = language_tool_download_version
         self._new_spellings = None
         self._new_spellings_persist = new_spellings_persist
         self._host = host or socket.gethostbyname('localhost')
 
         if remote_server:
             assert config is None, "cannot pass config file to remote server"
         self.config = LanguageToolConfig(config) if config else None
@@ -111,23 +119,27 @@
     @property
     def motherTongue(self):
         """The user's mother tongue or None.
         The mother tongue may also be used as a source language for
         checking bilingual texts.
         """
         return self._motherTongue
+
     @motherTongue.setter
     def motherTongue(self, motherTongue):
-        self._motherTongue = (None if motherTongue is None
-                              else LanguageTag(motherTongue, self._get_languages()))
+        self._motherTongue = (
+            None if motherTongue is None
+            else LanguageTag(motherTongue, self._get_languages())
+        )
+
     @property
     def _spell_checking_categories(self):
         return {'TYPOS'}
 
-    def check(self, text: str) -> [Match]:
+    def check(self, text: str) -> List[Match]:
         """Match text against enabled rules."""
         url = urllib.parse.urljoin(self._url, 'check')
         response = self._query_server(url, self._create_params(text))
         matches = response['matches']
         return [Match(match) for match in matches]
 
     def _create_params(self, text: str) -> Dict[str, str]:
@@ -147,52 +159,66 @@
         if self.preferred_variants:
             params['preferredVariants'] = ','.join(self.preferred_variants)
         return params
 
     def correct(self, text: str) -> str:
         """Automatically apply suggestions to the text."""
         return correct(text, self.check(text))
-    
+
     def enable_spellchecking(self):
         """Enable spell-checking rules."""
-        self.disabled_categories.difference_update(self._spell_checking_categories)
+        self.disabled_categories.difference_update(
+            self._spell_checking_categories
+        )
 
     def disable_spellchecking(self):
         """Disable spell-checking rules."""
         self.disabled_categories.update(self._spell_checking_categories)
 
     @staticmethod
     def _get_valid_spelling_file_path() -> str:
         library_path = get_language_tool_directory()
-        spelling_file_path = os.path.join(library_path, "org/languagetool/resource/en/hunspell/spelling.txt")
+        spelling_file_path = os.path.join(
+            library_path, "org/languagetool/resource/en/hunspell/spelling.txt"
+        )
         if not os.path.exists(spelling_file_path):
-            raise FileNotFoundError("Failed to find the spellings file at {}\n Please file an issue at "
-                                    "https://github.com/jxmorris12/language_tool_python/issues"
-                                    .format(spelling_file_path))
+            raise FileNotFoundError(
+                "Failed to find the spellings file at {}\n "
+                "Please file an issue at "
+                "https://github.com/jxmorris12/language_tool_python/issues"
+                .format(spelling_file_path))
         return spelling_file_path
 
     def _register_spellings(self, spellings):
         spelling_file_path = self._get_valid_spelling_file_path()
-        with open(spelling_file_path, "a+", encoding='utf-8') as spellings_file:
-            spellings_file.write("\n" + "\n".join([word for word in spellings]))
+        with (
+            open(spelling_file_path, "a+", encoding='utf-8')
+        ) as spellings_file:
+            spellings_file.write(
+                "\n" + "\n".join([word for word in spellings])
+            )
         if DEBUG_MODE:
             print("Registered new spellings at {}".format(spelling_file_path))
 
     def _unregister_spellings(self):
         spelling_file_path = self._get_valid_spelling_file_path()
-        with open(spelling_file_path, 'r+', encoding='utf-8') as spellings_file:
+        with (
+            open(spelling_file_path, 'r+', encoding='utf-8')
+        ) as spellings_file:
             spellings_file.seek(0, os.SEEK_END)
             for _ in range(len(self._new_spellings)):
                 while spellings_file.read(1) != '\n':
                     spellings_file.seek(spellings_file.tell() - 2, os.SEEK_SET)
                 spellings_file.seek(spellings_file.tell() - 2, os.SEEK_SET)
             spellings_file.seek(spellings_file.tell() + 1, os.SEEK_SET)
             spellings_file.truncate()
         if DEBUG_MODE:
-            print("Unregistered new spellings at {}".format(spelling_file_path))
+            print(
+                "Unregistered new spellings at {}".format(spelling_file_path)
+            )
 
     def _get_languages(self) -> set:
         """Get supported languages (by querying the server)."""
         self._start_server_if_needed()
         url = urllib.parse.urljoin(self._url, 'languages')
         languages = set()
         for e in self._query_server(url, num_tries=1):
@@ -211,20 +237,26 @@
         self._remote = True
 
     def _query_server(self, url, params=None, num_tries=2):
         if DEBUG_MODE:
             print('_query_server url:', url, 'params:', params)
         for n in range(num_tries):
             try:
-                with requests.get(url, params=params, timeout=self._TIMEOUT) as response:
+                with (
+                    requests.get(url, params=params, timeout=self._TIMEOUT)
+                ) as response:
                     try:
                         return response.json()
                     except json.decoder.JSONDecodeError as e:
                         if DEBUG_MODE:
-                            print('URL {} and params {} returned invalid JSON response:'.format(url, params))
+                            print(
+                                'URL {} and params {} '
+                                'returned invalid JSON response: {}'
+                                .format(url, params, e)
+                            )
                             print(response)
                             print(response.content)
                         raise LanguageToolError(response.content.decode())
             except (IOError, http.client.HTTPException) as e:
                 if self._remote is False:
                     self._terminate_server()
                     self._start_local_server()
@@ -241,22 +273,29 @@
                 if self._MIN_PORT <= self._port < self._MAX_PORT:
                     self._port += 1
                 else:
                     raise
 
     def _start_local_server(self):
         # Before starting local server, download language tool if needed.
-        download_lt()
+        download_lt(self.language_tool_download_version)
         err = None
         try:
             if DEBUG_MODE:
                 if self._port:
-                    print('language_tool_python initializing with port:', self._port)
+                    print(
+                        'language_tool_python initializing with port:',
+                        self._port
+                    )
                 if self.config:
-                    print('language_tool_python initializing with temporary config file:', self.config.path)
+                    print(
+                        'language_tool_python initializing '
+                        'with temporary config file:',
+                        self.config.path
+                    )
             server_cmd = get_server_cmd(self._port, self.config)
         except PathError as e:
             # Can't find path to LanguageTool.
             err = e
         else:
             # Need to PIPE all handles: http://bugs.python.org/issue3905
             self._server = subprocess.Popen(
@@ -275,16 +314,18 @@
                 line = self._server.stdout.readline()
                 if not line:
                     break
                 match = self._PORT_RE.search(line)
                 if match:
                     port = int(match.group(1))
                     if port != self._port:
-                        raise LanguageToolError('requested port {}, but got {}'.format(
-                            self._port, port))
+                        raise LanguageToolError(
+                            'requested port {}, but got {}'
+                            .format(self._port, port)
+                        )
                     break
             if not match:
                 err_msg = self._terminate_server()
                 match = self._PORT_RE.search(err_msg)
                 if not match:
                     raise LanguageToolError(err_msg)
                 port = int(match.group(1))
@@ -294,15 +335,20 @@
         if self._server:
             self._consumer_thread = threading.Thread(
                 target=lambda: _consume(self._server.stdout))
             self._consumer_thread.daemon = True
             self._consumer_thread.start()
         else:
             # Couldn't start the server, so maybe there is already one running.
-            raise ServerError('Server running; don\'t start a server here.')
+            if err:
+                raise Exception(err)
+            else:
+                raise ServerError(
+                    'Server running; don\'t start a server here.'
+                )
 
     def _server_is_alive(self):
         return self._server and self._server.poll() is None
 
     def _terminate_server(self):
         LanguageToolError_message = ''
         try:
@@ -324,18 +370,22 @@
         try:
             self._server.stderr.close()
         except IOError:
             pass
         self._server = None
         return LanguageToolError_message
 
+
 class LanguageToolPublicAPI(LanguageTool):
     """Language tool client of the official API."""
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, remote_server='https://languagetool.org/api/', **kwargs)
+        super().__init__(
+            *args, remote_server='https://languagetool.org/api/', **kwargs
+        )
+
 
 @atexit.register
 def terminate_server():
     """Terminate the server."""
     for proc in RUNNING_SERVER_PROCESSES:
         proc.terminate()
```

### Comparing `language_tool_python-2.7.3/language_tool_python/utils.py` & `language_tool_python-2.8/language_tool_python/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from typing import List, Tuple
 
-import http.client
 import glob
 import locale
 import os
-import re
 import subprocess
-import sys
 import urllib.parse
 import urllib.request
 
 from .config_file import LanguageToolConfig
 from .match import Match
 from .which import which
 
@@ -18,42 +15,53 @@
     'languagetool-server.jar',
     'languagetool-standalone*.jar',  # 2.1
     'LanguageTool.jar',
     'LanguageTool.uno.jar'
 ]
 FAILSAFE_LANGUAGE = 'en'
 
+LTP_PATH_ENV_VAR = "LTP_PATH"  # LanguageTool download path
+
+# Directory containing the LanguageTool jar file:
+LTP_JAR_DIR_PATH_ENV_VAR = "LTP_JAR_DIR_PATH"
+
 # https://mail.python.org/pipermail/python-dev/2011-July/112551.html
 
 if os.name == 'nt':
     startupinfo = subprocess.STARTUPINFO()
     startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
 else:
     startupinfo = None
 
+
 class LanguageToolError(Exception):
-	pass
-	
+    pass
+
+
 class ServerError(LanguageToolError):
     pass
 
+
 class JavaError(LanguageToolError):
     pass
 
+
 class PathError(LanguageToolError):
     pass
 
+
 def parse_url(url_str):
     """ Parses a URL string, and adds 'http' if necessary. """
     if 'http' not in url_str:
-        url_str = 'http://' + url_str   
+        url_str = 'http://' + url_str
 
     return urllib.parse.urlparse(url_str).geturl()
 
-def correct(text: str, matches: [Match]) -> str:
+
+def correct(text: str, matches: List[Match]) -> str:
     """Automatically apply suggestions to the text."""
     ltext = list(text)
     matches = [match for match in matches if match.replacements]
     errors = [ltext[match.offset:match.offset + match.errorLength]
               for match in matches]
     correct_offset = 0
     for n, match in enumerate(matches):
@@ -62,70 +70,92 @@
         if ltext[frompos:topos] != errors[n]:
             continue
         repl = match.replacements[0]
         ltext[frompos:topos] = list(repl)
         correct_offset += len(repl) - len(errors[n])
     return ''.join(ltext)
 
-def get_language_tool_download_path():
+
+def get_language_tool_download_path() -> str:
     # Get download path from environment or use default.
     download_path = os.environ.get(
-        'LTP_PATH',
+        LTP_PATH_ENV_VAR,
         os.path.join(os.path.expanduser("~"), ".cache", "language_tool_python")
     )
-    # Make download path, if it doesn't exist.
-    os.makedirs(download_path, exist_ok=True)
     return download_path
 
-def get_language_tool_directory():
-    """Get LanguageTool directory."""
-    download_folder = get_language_tool_download_path()
-    assert os.path.isdir(download_folder)
+
+def find_existing_language_tool_downloads(download_folder: str) -> List[str]:
     language_tool_path_list = [
         path for path in
         glob.glob(os.path.join(download_folder, 'LanguageTool*'))
         if os.path.isdir(path)
     ]
+    return language_tool_path_list
+
+
+def get_language_tool_directory() -> str:
+    """Get LanguageTool directory."""
+    download_folder = get_language_tool_download_path()
+    if not os.path.isdir(download_folder):
+        raise NotADirectoryError(
+            "LanguageTool directory path is not a valid directory {}."
+            .format(download_folder)
+        )
+    language_tool_path_list = find_existing_language_tool_downloads(
+        download_folder
+    )
 
     if not len(language_tool_path_list):
-        raise FileNotFoundError('LanguageTool not found in {}.'.format(download_folder))
+        raise FileNotFoundError(
+            'LanguageTool not found in {}.'.format(download_folder)
+        )
 
+    # Return the latest version found in the directory.
     return max(language_tool_path_list)
 
 
-def get_server_cmd(port: int=None, config: LanguageToolConfig=None) -> List[str]:
+def get_server_cmd(
+        port: int = None, config: LanguageToolConfig = None
+) -> List[str]:
     java_path, jar_path = get_jar_info()
     cmd = [java_path, '-cp', jar_path,
-            'org.languagetool.server.HTTPServer']
+           'org.languagetool.server.HTTPServer']
 
     if port is not None:
-        cmd +=  ['-p', str(port)]
-    
+        cmd += ['-p', str(port)]
+
     if config is not None:
         cmd += ['--config', config.path]
 
     return cmd
 
 
 def get_jar_info() -> Tuple[str, str]:
     java_path = which('java')
     if not java_path:
         raise JavaError("can't find Java")
-    dir_name = get_language_tool_directory()
+
+    # Use the env var to the jar directory if it is defined
+    # otherwise look in the download directory
+    jar_dir_name = os.environ.get(
+        LTP_JAR_DIR_PATH_ENV_VAR,
+        get_language_tool_directory()
+    )
     jar_path = None
     for jar_name in JAR_NAMES:
-        for jar_path in glob.glob(os.path.join(dir_name, jar_name)):
+        for jar_path in glob.glob(os.path.join(jar_dir_name, jar_name)):
             if os.path.isfile(jar_path):
                 break
         else:
             jar_path = None
         if jar_path:
             break
     else:
         raise PathError("can't find languagetool-standalone in {!r}"
-                        .format(dir_name))
+                        .format(jar_dir_name))
     return java_path, jar_path
 
 
 def get_locale_language():
     """Get the language code for the current locale setting."""
-    return locale.getlocale()[0] or locale.getdefaultlocale()[0]
+    return locale.getlocale()[0] or locale.getdefaultlocale()[0]
```

### Comparing `language_tool_python-2.7.3/language_tool_python/which.py` & `language_tool_python-2.8/language_tool_python/which.py`

 * *Files identical despite different names*

### Comparing `language_tool_python-2.7.3/language_tool_python.egg-info/PKG-INFO` & `language_tool_python-2.8/language_tool_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: language-tool-python
-Version: 2.7.3
+Version: 2.8
 Summary: Checks grammar using LanguageTool.
 Home-page: https://github.com/jxmorris12/language_tool_python
 Author: Jack Morris
 Author-email: jxmorris12@gmail.com
 License: GNU GPL
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 
 # `language_tool_python`: a grammar checker for Python 📝
 
 ![language tool python on pypi](https://badge.fury.io/py/language-tool-python.svg)
 
 ![Test with PyTest](https://github.com/jxmorris12/language_tool_python/workflows/Test%20with%20PyTest/badge.svg)
 
-Current LanguageTool version: **5.5**
+Current LanguageTool version: **6.4**
 
 This is a Python wrapper for [LanguageTool](https://languagetool.org). LanguageTool is open-source grammar tool, also known as the spellchecker for OpenOffice. This library allows you to make to detect grammar errors and spelling mistakes through a Python script or through a command-line interface.
 
 ## Local and Remote Servers
 
 By default, `language_tool_python` will download a LanguageTool server `.jar` and run that in the background to detect grammar errors locally. However, LanguageTool also offers a [Public HTTP Proofreading API](https://dev.languagetool.org/public-http-api) that is supported as well. Follow the link for rate limiting details. (Running locally won't have the same restrictions.)
 
@@ -159,15 +159,15 @@
 >>> lang_tool.check('helo darknes my old frend')
 [Match({'ruleId': 'UPPERCASE_SENTENCE_START', 'message': 'This sentence does not start with an uppercase letter.', 'replacements': ['Helo'], 'offsetInContext': 0, 'context': 'helo darknes my old frend', 'offset': 0, 'errorLength': 4, 'category': 'CASING', 'ruleIssueType': 'typographical', 'sentence': 'helo darknes my old frend'}), Match({'ruleId': 'MORFOLOGIK_RULE_EN_US', 'message': 'Possible spelling mistake found.', 'replacements': ['darkness', 'darkens', 'darkies'], 'offsetInContext': 5, 'context': 'helo darknes my old frend', 'offset': 5, 'errorLength': 7, 'category': 'TYPOS', 'ruleIssueType': 'misspelling', 'sentence': 'helo darknes my old frend'}), Match({'ruleId': 'MORFOLOGIK_RULE_EN_US', 'message': 'Possible spelling mistake found.', 'replacements': ['friend', 'trend', 'Fred', 'freed', 'Freud', 'Friend', 'fend', 'fiend', 'frond', 'rend', 'fr end'], 'offsetInContext': 20, 'context': 'helo darknes my old frend', 'offset': 20, 'errorLength': 5, 'category': 'TYPOS', 'ruleIssueType': 'misspelling', 'sentence': 'helo darknes my old frend'})]
 >>>
 ```
 
 ## Configuration
 
-LanguageTool offers lots of built-in configuration options. 
+LanguageTool offers lots of built-in configuration options.
 
 ### Example: Enabling caching
 Here's an example of using the configuration options to enable caching. Some users have reported that this helps performance a lot.
 ```python
 import language_tool_python
 tool = language_tool_python.LanguageTool('en-US', config={ 'cacheSize': 1000, 'pipelineCaching': True })
 ```
@@ -230,21 +230,28 @@
 
 ### What rules does LanguageTool have?
 
 Searching for a specific rule to enable or disable? Curious the breadth of rules LanguageTool applies? This page contains a massive list of all 5,000+ grammatical rules that are programmed into LanguageTool: https://community.languagetool.org/rule/list?lang=en&offset=30&max=10
 
 ### Customizing Download URL or Path
 
+If LanguageTool is already installed on your system, you can defined the following environment variable:
+```bash
+$ export LTP_JAR_DIR_PATH = /path/to/the/language/tool/jar/files
+```
+
+Overwise, `language_tool_python` can download LanguageTool for you automatically.
+
 To overwrite the host part of URL that is used to download LanguageTool-{version}.zip:
 
 ```bash
 $ export LTP_DOWNLOAD_HOST = [alternate URL]
 ```
 
-This can be used to downgrade to an older version, for example, or to download from a mirror. 
+This can be used to downgrade to an older version, for example, or to download from a mirror.
 
 And to choose the specific folder to download the server to:
 
 ```bash
 $ export LTP_PATH = /path/to/save/language/tool
 ```
 
@@ -260,12 +267,13 @@
 [LanguageTool-stable.zip](https://www.languagetool.org/download/LanguageTool-stable.zip) and unzip it
 into where the ``language_tool_python`` package resides.
 
 ### LanguageTool Version
 
 As of April 2020, `language_tool_python` was forked from `language-check` and no longer supports LanguageTool versions lower than 4.0.
 
-### Acknowledgements 
+### Acknowledgements
+
 This is a fork of https://github.com/myint/language-check/ that produces more easily parsable
 results from the command-line.
```

### Comparing `language_tool_python-2.7.3/language_tool_python.egg-info/SOURCES.txt` & `language_tool_python-2.8/language_tool_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `language_tool_python-2.7.3/run_doctest.py` & `language_tool_python-2.8/run_doctest.py`

 * *Files identical despite different names*

### Comparing `language_tool_python-2.7.3/setup.py` & `language_tool_python-2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='language_tool_python',
-    version='2.7.3',
+    version='2.8',
     description='Checks grammar using LanguageTool.',
     long_description_content_type='text/markdown',
     long_description=long_description,
     author='Jack Morris',
     author_email='jxmorris12@gmail.com',
     url='https://github.com/jxmorris12/language_tool_python',
     license='GNU GPL',
```

