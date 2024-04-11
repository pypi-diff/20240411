# Comparing `tmp/jaraco.home-3.7.0.tar.gz` & `tmp/jaraco.home-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.home-3.7.0.tar", last modified: Thu Apr  4 17:10:46 2024, max compression
+gzip compressed data, was "jaraco.home-3.8.0.tar", last modified: Thu Apr 11 20:24:05 2024, max compression
```

## Comparing `jaraco.home-3.7.0.tar` & `jaraco.home-3.8.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.526130 jaraco.home-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.522130 jaraco.home-3.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.522130 jaraco.home-3.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-04 17:10:46.526130 jaraco.home-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.522130 jaraco.home-3.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.518129 jaraco.home-3.7.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.526130 jaraco.home-3.7.0/jaraco/home/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/Gather HDHomeRun Stats.plist
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/hdhomerun.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/mock hdhomerun.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/relay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/report-spam-call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.526130 jaraco.home-3.7.0/jaraco.home.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-04 17:10:46.000000 jaraco.home-3.7.0/jaraco.home.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-04 17:10:46.000000 jaraco.home-3.7.0/jaraco.home.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:10:46.000000 jaraco.home-3.7.0/jaraco.home.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-04 17:10:46.000000 jaraco.home-3.7.0/jaraco.home.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 17:10:46.000000 jaraco.home-3.7.0/jaraco.home.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 17:10:46.530130 jaraco.home-3.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.723543 jaraco.home-3.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.715543 jaraco.home-3.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.715543 jaraco.home-3.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-11 20:24:05.723543 jaraco.home-3.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.715543 jaraco.home-3.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.715543 jaraco.home-3.8.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.719543 jaraco.home-3.8.0/jaraco/home/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/Gather HDHomeRun Stats.plist
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/check-traps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/hdhomerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/mock hdhomerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/report-spam-call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.719543 jaraco.home-3.8.0/jaraco.home.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-11 20:24:05.000000 jaraco.home-3.8.0/jaraco.home.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-11 20:24:05.000000 jaraco.home-3.8.0/jaraco.home.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:24:05.000000 jaraco.home-3.8.0/jaraco.home.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-11 20:24:05.000000 jaraco.home-3.8.0/jaraco.home.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 20:24:05.000000 jaraco.home-3.8.0/jaraco.home.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 20:24:05.723543 jaraco.home-3.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/tox.ini
```

### Comparing `jaraco.home-3.7.0/.github/workflows/main.yml` & `jaraco.home-3.8.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.7.0/LICENSE` & `jaraco.home-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.7.0/NEWS.rst` & `jaraco.home-3.8.0/NEWS.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.8.0
+======
+
+Features
+--------
+
+- Add script for checking the mouse trap(s).
+
+
 v3.7.0
 ======
 
 Features
 --------
 
 - Allow time and browser to be specified in spam call reporter.
```

### Comparing `jaraco.home-3.7.0/PKG-INFO` & `jaraco.home-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.home
-Version: 3.7.0
+Version: 3.8.0
 Summary: Some functions supporting the devices in jaraco's home
 Home-page: https://github.com/jaraco/jaraco.home
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,15 @@
 Requires-Dist: jaraco.mongodb
 Requires-Dist: dnspython
 Requires-Dist: keyring
 Requires-Dist: jaraco.collections
 Requires-Dist: splinter[selenium]
 Requires-Dist: autocommand
 Requires-Dist: python-dateutil
+Requires-Dist: victor-smart-kill
 Provides-Extra: testing
 Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
```

### Comparing `jaraco.home-3.7.0/README.rst` & `jaraco.home-3.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.7.0/conftest.py` & `jaraco.home-3.8.0/conftest.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.7.0/docs/conf.py` & `jaraco.home-3.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.7.0/jaraco/home/Gather HDHomeRun Stats.plist` & `jaraco.home-3.8.0/jaraco/home/Gather HDHomeRun Stats.plist`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.7.0/jaraco/home/hdhomerun.py` & `jaraco.home-3.8.0/jaraco/home/hdhomerun.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.7.0/jaraco/home/relay.py` & `jaraco.home-3.8.0/jaraco/home/relay.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.7.0/jaraco/home/report-spam-call.py` & `jaraco.home-3.8.0/jaraco/home/report-spam-call.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,19 @@
 import datetime
-import json
-import os
 import re
-import types
 
 import autocommand
 import dateutil.parser
 from splinter import Browser
 
-import jaraco.collections
+from . import contact as contact_info
 
 DROPPED_CALL = '2'
 
 
-class IdentifierDict(jaraco.collections.KeyTransformingDict):
-    @staticmethod
-    def transform_key(key):
-        return key.replace(' ', '_')
-
-
-def read_contact_info():
-    return types.SimpleNamespace(
-        **IdentifierDict(json.loads(os.environ['CONTACT_INFO']))
-    )
-
-
 def clean_phone(number):
     """
     >>> clean_phone("+1 202 555 1212")
     '2025551212'
     """
     return re.sub(r'[-. ]', '', number.removeprefix('+1'))
 
@@ -40,15 +25,15 @@
     close=False,
     browser='firefox',
     when: dateutil.parser.parse = datetime.datetime.now(),  # type: ignore
 ):
     """
     Report the common spam calls.
     """
-    contact = read_contact_info()
+    contact = contact_info.load()
     browser = Browser(browser)
     browser.visit('https://www.donotcall.gov/report.html')
     browser.find_by_value('Continue').click()
     browser.fill('PhoneTextBox', clean_phone(contact.phone))
     browser.fill('DateOfCallTextBox', when.strftime('%m/%d/%Y'))  # type: ignore
     browser.select('TimeOfCallDropDownList', when.strftime('%H'))  # type: ignore
     browser.select('ddlMinutes', when.strftime('%M'))  # type: ignore
```

### Comparing `jaraco.home-3.7.0/jaraco/home/thermostat.py` & `jaraco.home-3.8.0/jaraco/home/thermostat.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.7.0/jaraco.home.egg-info/PKG-INFO` & `jaraco.home-3.8.0/jaraco.home.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.home
-Version: 3.7.0
+Version: 3.8.0
 Summary: Some functions supporting the devices in jaraco's home
 Home-page: https://github.com/jaraco/jaraco.home
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,15 @@
 Requires-Dist: jaraco.mongodb
 Requires-Dist: dnspython
 Requires-Dist: keyring
 Requires-Dist: jaraco.collections
 Requires-Dist: splinter[selenium]
 Requires-Dist: autocommand
 Requires-Dist: python-dateutil
+Requires-Dist: victor-smart-kill
 Provides-Extra: testing
 Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
```

### Comparing `jaraco.home-3.7.0/jaraco.home.egg-info/SOURCES.txt` & `jaraco.home-3.8.0/jaraco.home.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -21,12 +21,14 @@
 jaraco.home.egg-info/PKG-INFO
 jaraco.home.egg-info/SOURCES.txt
 jaraco.home.egg-info/dependency_links.txt
 jaraco.home.egg-info/requires.txt
 jaraco.home.egg-info/top_level.txt
 jaraco/home/Gather HDHomeRun Stats.plist
 jaraco/home/__init__.py
+jaraco/home/check-traps.py
+jaraco/home/contact.py
 jaraco/home/hdhomerun.py
 jaraco/home/mock hdhomerun.py
 jaraco/home/relay.py
 jaraco/home/report-spam-call.py
 jaraco/home/thermostat.py
```

### Comparing `jaraco.home-3.7.0/pytest.ini` & `jaraco.home-3.8.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.7.0/setup.cfg` & `jaraco.home-3.8.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 	jaraco.mongodb
 	dnspython
 	keyring
 	jaraco.collections
 	splinter[selenium]
 	autocommand
 	python-dateutil
+	victor-smart-kill
 
 [options.extras_require]
 testing = 
 	pytest >= 6, != 8.1.1
 	pytest-checkdocs >= 2.4
 	pytest-cov
 	pytest-mypy
```

### Comparing `jaraco.home-3.7.0/tox.ini` & `jaraco.home-3.8.0/tox.ini`

 * *Files identical despite different names*

