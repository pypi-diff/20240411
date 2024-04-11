# Comparing `tmp/fyta_cli-0.3.5.tar.gz` & `tmp/fyta_cli-0.4.0.tar.gz`

## Comparing `fyta_cli-0.3.5.tar` & `fyta_cli-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/requirements.txt
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/.github/workflows/ruff.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/src/fyta_cli/__init__.py
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/src/fyta_cli/fyta_client.py
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/src/fyta_cli/fyta_connector.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/src/fyta_cli/fyta_exceptions.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/src/fyta_cli/utils.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/README.md
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 fyta_cli-0.4.0/requirements.txt
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 fyta_cli-0.4.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 fyta_cli-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fyta_cli-0.4.0/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fyta_cli-0.4.0/src/fyta_cli/__init__.py
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 fyta_cli-0.4.0/src/fyta_cli/fyta_client.py
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 fyta_cli-0.4.0/src/fyta_cli/fyta_connector.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 fyta_cli-0.4.0/src/fyta_cli/fyta_exceptions.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 fyta_cli-0.4.0/src/fyta_cli/utils.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fyta_cli-0.4.0/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 fyta_cli-0.4.0/README.md
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 fyta_cli-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 fyta_cli-0.4.0/PKG-INFO
```

### Comparing `fyta_cli-0.3.5/.github/workflows/pylint.yml` & `fyta_cli-0.4.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.3.5/.github/workflows/python-publish.yml` & `fyta_cli-0.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.3.5/.github/workflows/ruff.yml` & `fyta_cli-0.4.0/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.3.5/src/fyta_cli/fyta_client.py` & `fyta_cli-0.4.0/src/fyta_cli/fyta_client.py`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.3.5/src/fyta_cli/fyta_connector.py` & `fyta_cli-0.4.0/src/fyta_cli/fyta_connector.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 from typing import Any
 from zoneinfo import ZoneInfo
 
 from .fyta_client import Client
 from .utils import safe_get
 
 PLANT_STATUS = {
+    0: "deleted",
+    1: "doing_great",
+    2: "need_attention",
+    3: "need_help",
+}
+
+#status = 0 if user_plant deleted, 1 for user_plant in green, 2 for yellow, 3 for red
+PLANT_MEASUREMENT_STATUS = {
     1: "too_low",
     2: "low",
     3: "perfect",
     4: "high",
     5: "too_high",
 }
```

### Comparing `fyta_cli-0.3.5/src/fyta_cli/utils.py` & `fyta_cli-0.4.0/src/fyta_cli/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,16 +31,20 @@
     if expected_type == bool:
         return_value = __get_bool(value)
     if expected_type == str:
         return_value = str(value)
     if expected_type == datetime:
         return_value = __get_datetime(value, tz)
 
-    if "status" in keys and (return_value < 1 or return_value > 5):
-        #FYTA status has a scale from 1 to 5; return None, if no correct status is set
+    if ".status" in keys and (return_value < 1 or return_value > 5):
+        #FYTA measurement status has a scale from 1 to 5; return None, if no correct status is set
+        return_value = None
+
+    if key_path == "status" and (return_value < 0 or return_value > 3):
+        #FYTA plant status has a scale from 0 to 3; return None, if no correct status is set
         return_value = None
 
     return return_value
 
 
 def __get_bool(value):
     if isinstance(value, bool):
```

### Comparing `fyta_cli-0.3.5/LICENSE` & `fyta_cli-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.3.5/pyproject.toml` & `fyta_cli-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fyta_cli"
-version = "0.3.5"
+version = "0.4.0"
 authors = [
   { name="dontinelli", email="73341522+dontinelli@users.noreply.github.com" },
 ]
 description = "Python library to access the FYTA API"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `fyta_cli-0.3.5/PKG-INFO` & `fyta_cli-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fyta_cli
-Version: 0.3.5
+Version: 0.4.0
 Summary: Python library to access the FYTA API
 Project-URL: Repository, https://github.com/dontinelli/fyta_cli.git
 Project-URL: Issues, https://github.com/dontinelli/fyta_cli/issues
 Project-URL: Changelog, https://github.com/dontinelli/fyta_cli/blob/master/CHANGELOG.md
 Project-URL: FYTA homepage, https://fyta.de/
 Project-URL: API Documentation, https://fyta-io.notion.site/FYTA-Public-API-d2f4c30306f74504924c9a40402a3afd
 Author-email: dontinelli <73341522+dontinelli@users.noreply.github.com>
```

