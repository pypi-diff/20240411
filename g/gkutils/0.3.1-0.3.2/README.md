# Comparing `tmp/gkutils-0.3.1.tar.gz` & `tmp/gkutils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gkutils-0.3.1.tar", last modified: Wed Mar  6 14:48:52 2024, max compression
+gzip compressed data, was "dist/gkutils-0.3.2.tar", last modified: Wed Apr 10 23:52:40 2024, max compression
```

## Comparing `gkutils-0.3.1.tar` & `gkutils-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-06 14:48:52.137975 gkutils-0.3.1/
--rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkutils-0.3.1/LICENSE
--rw-r--r--   0 kws        (502) staff       (20)     1221 2024-03-06 14:48:52.137668 gkutils-0.3.1/PKG-INFO
--rwxr-xr-x   0 kws        (502) staff       (20)      723 2021-11-09 11:03:16.000000 gkutils-0.3.1/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-06 14:48:52.125668 gkutils-0.3.1/gkutils/
--rw-r--r--   0 kws        (502) staff       (20)       26 2020-06-10 15:01:19.000000 gkutils-0.3.1/gkutils/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2024-03-06 14:46:11.000000 gkutils-0.3.1/gkutils/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-06 14:48:52.136642 gkutils-0.3.1/gkutils/commonutils/
--rw-r--r--   0 kws        (502) staff       (20)       51 2020-06-21 19:02:34.000000 gkutils-0.3.1/gkutils/commonutils/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)     7556 2023-04-26 17:44:40.000000 gkutils-0.3.1/gkutils/commonutils/bruteForceConeSearchATLAS.py
--rw-r--r--   0 kws        (502) staff       (20)     8964 2022-06-15 20:04:56.000000 gkutils-0.3.1/gkutils/commonutils/coneSearchCassandra.py
--rw-r--r--   0 kws        (502) staff       (20)      682 2023-07-03 09:10:46.000000 gkutils-0.3.1/gkutils/commonutils/far.py
--rw-r--r--   0 kws        (502) staff       (20)   108025 2024-03-06 14:45:47.000000 gkutils-0.3.1/gkutils/commonutils/generalutils.py
--rw-r--r--   0 kws        (502) staff       (20)     2580 2021-07-29 15:53:22.000000 gkutils-0.3.1/gkutils/commonutils/getCSVColumnSubset.py
--rwxr-xr-x   0 kws        (502) staff       (20)     3970 2022-05-09 17:15:02.000000 gkutils-0.3.1/gkutils/commonutils/getTestSherlockData.py
--rw-r--r--   0 kws        (502) staff       (20)     4824 2020-06-21 19:10:34.000000 gkutils-0.3.1/gkutils/commonutils/mputils.py
--rw-r--r--   0 kws        (502) staff       (20)      375 2021-02-18 18:00:55.000000 gkutils-0.3.1/gkutils/commonutils/test.py
--rw-r--r--   0 kws        (502) staff       (20)      214 2022-11-07 17:52:59.000000 gkutils-0.3.1/gkutils/commonutils/testReadGenericDataFile.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-06 14:48:52.128494 gkutils-0.3.1/gkutils.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1221 2024-03-06 14:48:51.000000 gkutils-0.3.1/gkutils.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      635 2024-03-06 14:48:51.000000 gkutils-0.3.1/gkutils.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2024-03-06 14:48:51.000000 gkutils-0.3.1/gkutils.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)      296 2024-03-06 14:48:51.000000 gkutils-0.3.1/gkutils.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       20 2024-03-06 14:48:51.000000 gkutils-0.3.1/gkutils.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        8 2024-03-06 14:48:51.000000 gkutils-0.3.1/gkutils.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2024-03-06 14:48:52.138113 gkutils-0.3.1/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1507 2024-03-06 14:03:24.000000 gkutils-0.3.1/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:52:40.369644 gkutils-0.3.2/
+-rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkutils-0.3.2/LICENSE
+-rw-r--r--   0 kws        (502) staff       (20)     1221 2024-04-10 23:52:40.369186 gkutils-0.3.2/PKG-INFO
+-rwxr-xr-x   0 kws        (502) staff       (20)      723 2021-11-09 11:03:16.000000 gkutils-0.3.2/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:52:40.353126 gkutils-0.3.2/gkutils/
+-rw-r--r--   0 kws        (502) staff       (20)       26 2020-06-10 15:01:19.000000 gkutils-0.3.2/gkutils/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2024-04-10 23:42:50.000000 gkutils-0.3.2/gkutils/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:52:40.367916 gkutils-0.3.2/gkutils/commonutils/
+-rw-r--r--   0 kws        (502) staff       (20)       51 2020-06-21 19:02:34.000000 gkutils-0.3.2/gkutils/commonutils/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)     7556 2023-04-26 17:44:40.000000 gkutils-0.3.2/gkutils/commonutils/bruteForceConeSearchATLAS.py
+-rw-r--r--   0 kws        (502) staff       (20)     8964 2022-06-15 20:04:56.000000 gkutils-0.3.2/gkutils/commonutils/coneSearchCassandra.py
+-rw-r--r--   0 kws        (502) staff       (20)      682 2023-07-03 09:10:46.000000 gkutils-0.3.2/gkutils/commonutils/far.py
+-rw-r--r--   0 kws        (502) staff       (20)   108199 2024-04-10 23:41:31.000000 gkutils-0.3.2/gkutils/commonutils/generalutils.py
+-rw-r--r--   0 kws        (502) staff       (20)     2580 2021-07-29 15:53:22.000000 gkutils-0.3.2/gkutils/commonutils/getCSVColumnSubset.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     3970 2022-05-09 17:15:02.000000 gkutils-0.3.2/gkutils/commonutils/getTestSherlockData.py
+-rw-r--r--   0 kws        (502) staff       (20)     4824 2020-06-21 19:10:34.000000 gkutils-0.3.2/gkutils/commonutils/mputils.py
+-rw-r--r--   0 kws        (502) staff       (20)      375 2021-02-18 18:00:55.000000 gkutils-0.3.2/gkutils/commonutils/test.py
+-rw-r--r--   0 kws        (502) staff       (20)      214 2022-11-07 17:52:59.000000 gkutils-0.3.2/gkutils/commonutils/testReadGenericDataFile.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:52:40.356740 gkutils-0.3.2/gkutils.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1221 2024-04-10 23:52:40.000000 gkutils-0.3.2/gkutils.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      635 2024-04-10 23:52:40.000000 gkutils-0.3.2/gkutils.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2024-04-10 23:52:40.000000 gkutils-0.3.2/gkutils.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      296 2024-04-10 23:52:40.000000 gkutils-0.3.2/gkutils.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       20 2024-04-10 23:52:40.000000 gkutils-0.3.2/gkutils.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        8 2024-04-10 23:52:40.000000 gkutils-0.3.2/gkutils.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2024-04-10 23:52:40.369878 gkutils-0.3.2/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1507 2024-03-06 14:03:24.000000 gkutils-0.3.2/setup.py
```

### Comparing `gkutils-0.3.1/LICENSE` & `gkutils-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gkutils-0.3.1/PKG-INFO` & `gkutils-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkutils
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection useful utilities - mostly related to astronomy
 Home-page: https://github.com/genghisken/gkutils
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gkutils-0.3.1/README.md` & `gkutils-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `gkutils-0.3.1/gkutils/commonutils/bruteForceConeSearchATLAS.py` & `gkutils-0.3.2/gkutils/commonutils/bruteForceConeSearchATLAS.py`

 * *Files identical despite different names*

### Comparing `gkutils-0.3.1/gkutils/commonutils/coneSearchCassandra.py` & `gkutils-0.3.2/gkutils/commonutils/coneSearchCassandra.py`

 * *Files identical despite different names*

### Comparing `gkutils-0.3.1/gkutils/commonutils/far.py` & `gkutils-0.3.2/gkutils/commonutils/far.py`

 * *Files identical despite different names*

### Comparing `gkutils-0.3.1/gkutils/commonutils/generalutils.py` & `gkutils-0.3.2/gkutils/commonutils/generalutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2806,22 +2806,24 @@
                  (', '.join(words[:-1]), words[-1])) if words else ''
 
 COORDS_DEC_REGEX = ""
 #COORDS_SEX_REGEX = "^([0-2][0-9])[^0-9]+([0-5][0-9])[^0-9]+([0-5][0-9])(\.[0-9]+){0,1}[^0-9+\-]+([+-]){0,1}([0-9][0-9])[^0-9]+([0-5][0-9])[^0-9]+([0-5][0-9])(\.[0-9]+){0,1}[^0-9 ]{0,1}( ([0-9][0-9]{0,1})){0,1}"
 #COORDS_SEX_REGEX = "^([0-2][0-9])[^0-9]{0,1}([0-5][0-9])[^0-9]{0,1}([0-5][0-9])(\.[0-9]+){0,1}[^0-9+\-]{0,5}([+-]){0,1}([0-9][0-9])[^0-9]{0,1}([0-5][0-9])[^0-9]{0,1}([0-5][0-9])(\.[0-9]+){0,1}[^0-9 ]{0,1}( +([0-9][0-9]{0,1})){0,1}"
 
 # 2019-04-17 KWS Made the sexagesimal regex a bit more forgiving.
+# 2024-04-10 KWS Allow up to 3 digits + fraction for the search radius.
 #                                h    h               m    m                       s    s     .  f                       (+-)              d    d                    m    m               s    s     .  f                        (radius)
-COORDS_SEX_REGEX = "^([0-2]{0,1}[0-9])[^0-9+\-\.]{0,}([0-5]{0,1}[0-9])[^0-9+\-\.]{0,}([0-5]{0,1}[0-9])(\.[0-9]+){0,1}[^0-9+\-\.]{0,}([+-]){0,1}([0-9]{0,1}[0-9])[^0-9+\-\.]{0,}([0-5]{0,1}[0-9])[^0-9+\-\.]{0,}([0-5]{0,1}[0-9])(\.[0-9]+){0,1}[^0-9+\-\.]{0,}(([0-9][0-9]{0,1})){0,1}$"
+COORDS_SEX_REGEX = "^([0-2]{0,1}[0-9])[^0-9+\-\.]{0,}([0-5]{0,1}[0-9])[^0-9+\-\.]{0,}([0-5]{0,1}[0-9])(\.[0-9]+){0,1}[^0-9+\-\.]{0,}([+-]){0,1}([0-9]{0,1}[0-9])[^0-9+\-\.]{0,}([0-5]{0,1}[0-9])[^0-9+\-\.]{0,}([0-5]{0,1}[0-9])(\.[0-9]+){0,1}[^0-9+\-\.]{0,}(([0-9][0-9]{0,2}(\.[0-9]+){0,1})){0,1}$"
 COORDS_SEX_REGEX_COMPILED = re.compile(COORDS_SEX_REGEX)
 
 #COORDS_DEC_REGEX = "^([0-9]+(\.[0-9]+){0,1})[^0-9+\-]{0,5}([+-]{0,1}[0-9]+(\.[0-9]+){0,1})[^0-9 ]{0,1}( +([0-9][0-9]{0,1})){0,1}"
 # 2019-04-17 KWS Made the decimal regex a bit more forgiving.
+# 2024-04-10 KWS Allow up to 3 digits + fraction for the search radius.
 #                            d.f                           (+-)            d.f                         (radius)
-COORDS_DEC_REGEX = "^([0-9]+(\.[0-9]+){0,1})[^0-9+\-]{0,}([+-]{0,1}[0-9]+(\.[0-9]+){0,1})[^0-9]{0,}(([0-9][0-9]{0,1})){0,1}$"
+COORDS_DEC_REGEX = "^([0-9]+(\.[0-9]+){0,1})[^0-9+\-]{0,}([+-]{0,1}[0-9]+(\.[0-9]+){0,1})[^0-9]{0,}(([0-9][0-9]{0,2}(\.[0-9]+){0,1})){0,1}$"
 COORDS_DEC_REGEX_COMPILED = re.compile(COORDS_DEC_REGEX)
 
 # 2019-04-17 KWS Made the name search more forgiving and extended it to ZTF.
 NAME_REGEX = "^(AT|SN|ATLAS|ASASSN-|ZTF|PS([1][\-]){0,1}){0,1} {0,1}([2][0]){0,1}([0-9][0-9][a-z]{1,7}|[0-9][0-9][A-Z])$"
 NAME_REGEX_COMPILED = re.compile(NAME_REGEX)
 
 def getObjectNamePortion(inputString):
```

### Comparing `gkutils-0.3.1/gkutils/commonutils/getCSVColumnSubset.py` & `gkutils-0.3.2/gkutils/commonutils/getCSVColumnSubset.py`

 * *Files identical despite different names*

### Comparing `gkutils-0.3.1/gkutils/commonutils/getTestSherlockData.py` & `gkutils-0.3.2/gkutils/commonutils/getTestSherlockData.py`

 * *Files identical despite different names*

### Comparing `gkutils-0.3.1/gkutils/commonutils/mputils.py` & `gkutils-0.3.2/gkutils/commonutils/mputils.py`

 * *Files identical despite different names*

### Comparing `gkutils-0.3.1/gkutils.egg-info/PKG-INFO` & `gkutils-0.3.2/gkutils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkutils
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection useful utilities - mostly related to astronomy
 Home-page: https://github.com/genghisken/gkutils
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gkutils-0.3.1/gkutils.egg-info/SOURCES.txt` & `gkutils-0.3.2/gkutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gkutils-0.3.1/setup.py` & `gkutils-0.3.2/setup.py`

 * *Files identical despite different names*

