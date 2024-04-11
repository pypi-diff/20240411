# Comparing `tmp/arabic_datetime-0.0.3.tar.gz` & `tmp/arabic_datetime-0.1.0.tar.gz`

## Comparing `arabic_datetime-0.0.3.tar` & `arabic_datetime-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arabic_datetime-0.0.3/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 arabic_datetime-0.0.3/arabic_datetime/__init__.py
--rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 arabic_datetime-0.0.3/arabic_datetime/arabic_date.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 arabic_datetime-0.0.3/arabic_datetime/arabic_time.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 arabic_datetime-0.0.3/arabic_datetime/constants.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 arabic_datetime-0.0.3/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 arabic_datetime-0.0.3/LICENSE
--rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 arabic_datetime-0.0.3/README.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 arabic_datetime-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8889 2020-02-02 00:00:00.000000 arabic_datetime-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/arabic_datetime/__init__.py
+-rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/arabic_datetime/arabic_date.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/arabic_datetime/arabic_time.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/arabic_datetime/constants.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/LICENSE
+-rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/README.md
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8889 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/PKG-INFO
```

### Comparing `arabic_datetime-0.0.3/arabic_datetime/arabic_date.py` & `arabic_datetime-0.1.0/arabic_datetime/arabic_date.py`

 * *Files identical despite different names*

### Comparing `arabic_datetime-0.0.3/arabic_datetime/arabic_time.py` & `arabic_datetime-0.1.0/arabic_datetime/arabic_time.py`

 * *Files identical despite different names*

### Comparing `arabic_datetime-0.0.3/arabic_datetime/constants.py` & `arabic_datetime-0.1.0/arabic_datetime/constants.py`

 * *Files identical despite different names*

### Comparing `arabic_datetime-0.0.3/LICENSE` & `arabic_datetime-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arabic_datetime-0.0.3/README.md` & `arabic_datetime-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `arabic_datetime-0.0.3/pyproject.toml` & `arabic_datetime-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "arabic-datetime"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name="Khaldevmedia", email="khaldevmedia@gmail.com" },
 ]
 description = "For formating arabic date and time"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["python", "arabic", "datetime", "date", "time", "arabic numerals"]
```

### Comparing `arabic_datetime-0.0.3/PKG-INFO` & `arabic_datetime-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arabic-datetime
-Version: 0.0.3
+Version: 0.1.0
 Summary: For formating arabic date and time
 Project-URL: Homepage, https://github.com/khaldevmedia/arabic-datetime
 Project-URL: Bug Tracker, https://github.com/khaldevmedia/arabic-datetime/issues
 Author-email: Khaldevmedia <khaldevmedia@gmail.com>
 License-File: LICENSE
 Keywords: arabic,arabic numerals,date,datetime,python,time
 Classifier: License :: OSI Approved :: MIT License
```

