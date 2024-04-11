# Comparing `tmp/spark_gaps_date_rorc_tools-0.2.1.tar.gz` & `tmp/spark_gaps_date_rorc_tools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_gaps_date_rorc_tools-0.2.1.tar", last modified: Sun Apr  7 06:03:50 2024, max compression
+gzip compressed data, was "spark_gaps_date_rorc_tools-0.2.2.tar", last modified: Thu Apr 11 13:04:23 2024, max compression
```

## Comparing `spark_gaps_date_rorc_tools-0.2.1.tar` & `spark_gaps_date_rorc_tools-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 06:03:50.063581 spark_gaps_date_rorc_tools-0.2.1/
--rw-rw-rw-   0        0        0     1092 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/LICENSE
--rw-rw-rw-   0        0        0       54 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2963 2024-04-07 06:03:50.063581 spark_gaps_date_rorc_tools-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2170 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/README.md
--rw-rw-rw-   0        0        0      534 2024-04-07 06:02:12.000000 spark_gaps_date_rorc_tools-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-04-07 06:03:50.064581 spark_gaps_date_rorc_tools-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1199 2024-04-07 06:00:01.000000 spark_gaps_date_rorc_tools-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:03:50.051578 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/
--rw-rw-rw-   0        0        0      537 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:03:50.058580 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/functions/
--rw-rw-rw-   0        0        0        0 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/functions/__init__.py
--rw-rw-rw-   0        0        0     5449 2024-04-07 06:00:01.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/functions/gaps_date.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:03:50.061580 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/
--rw-rw-rw-   0        0        0       75 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      331 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/config.py
--rw-rw-rw-   0        0        0     2522 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/dataframe.py
--rw-rw-rw-   0        0        0      463 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/logger.py
--rw-rw-rw-   0        0        0     1056 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/memory.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:03:50.062581 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/templates/
--rw-rw-rw-   0        0        0        0 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/templates/__init__.py
--rw-rw-rw-   0        0        0     1861 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/templates/table.html
--rw-rw-rw-   0        0        0     1430 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/time_execution.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:03:50.056578 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/
--rw-rw-rw-   0        0        0     2963 2024-04-07 06:03:49.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      830 2024-04-07 06:03:49.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 06:03:49.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-07 06:03:49.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-04-07 06:03:49.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 13:04:23.265340 spark_gaps_date_rorc_tools-0.2.2/
+-rw-rw-rw-   0        0        0     1092 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0       54 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2963 2024-04-11 13:04:23.265340 spark_gaps_date_rorc_tools-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2170 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.2/README.md
+-rw-rw-rw-   0        0        0      534 2024-04-07 06:02:12.000000 spark_gaps_date_rorc_tools-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-04-11 13:04:23.265340 spark_gaps_date_rorc_tools-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1199 2024-04-11 13:03:56.000000 spark_gaps_date_rorc_tools-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:04:23.202838 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/
+-rw-rw-rw-   0        0        0      537 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:04:23.218463 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/functions/
+-rw-rw-rw-   0        0        0        0 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0     5494 2024-04-11 12:48:49.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/functions/gaps_date.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:04:23.265340 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/
+-rw-rw-rw-   0        0        0       75 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      331 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/config.py
+-rw-rw-rw-   0        0        0     2522 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/dataframe.py
+-rw-rw-rw-   0        0        0      463 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/logger.py
+-rw-rw-rw-   0        0        0     1056 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/memory.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:04:23.265340 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/templates/
+-rw-rw-rw-   0        0        0        0 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/templates/__init__.py
+-rw-rw-rw-   0        0        0     1861 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/templates/table.html
+-rw-rw-rw-   0        0        0     1430 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/time_execution.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:04:23.218463 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools.egg-info/
+-rw-rw-rw-   0        0        0     2963 2024-04-11 13:04:23.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      830 2024-04-11 13:04:23.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 13:04:23.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-11 13:04:23.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-11 13:04:23.000000 spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools.egg-info/top_level.txt
```

### Comparing `spark_gaps_date_rorc_tools-0.2.1/LICENSE` & `spark_gaps_date_rorc_tools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.1/PKG-INFO` & `spark_gaps_date_rorc_tools-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_gaps_date_rorc_tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: spark_gaps_date_rorc_tools
 Home-page: https://github.com/jonaqp/spark_gaps_date_rorc_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_gaps_date_rorct_tools/archive/main.zip
 Keywords: spark,gaps,date
```

### Comparing `spark_gaps_date_rorc_tools-0.2.1/README.md` & `spark_gaps_date_rorc_tools-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.1/pyproject.toml` & `spark_gaps_date_rorc_tools-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.1/setup.py` & `spark_gaps_date_rorc_tools-0.2.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_gaps_date_rorc_tools',
     packages=find_packages(),
-    version='0.2.1',
+    version='0.2.2',
     description='spark_gaps_date_rorc_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_gaps_date_rorc_tools/',
     download_url='https://github.com/jonaqp/spark_gaps_date_rorct_tools/archive/main.zip',
```

### Comparing `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/__init__.py` & `spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/functions/gaps_date.py` & `spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/functions/gaps_date.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pyspark
 
 from spark_gaps_date_rorc_tools.utils.config import load_config
 from spark_gaps_date_rorc_tools.utils.dataframe import show_pd_df
 from spark_gaps_date_rorc_tools.utils.dataframe import show_spark_df
 
 
+pd.DataFrame.iteritems = pd.DataFrame.items
 def show_gaps_date(spark=None,
                    config_path_name=None,
                    hdfs_uri=None,
                    table_rorc=None,
                    filter_date_initial="202101",
                    filter_date_final="202112"):
     if not config_path_name:
```

### Comparing `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/dataframe.py` & `spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/memory.py` & `spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/memory.py`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/templates/table.html` & `spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/templates/table.html`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/time_execution.py` & `spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools/utils/time_execution.py`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/PKG-INFO` & `spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-gaps-date-rorc-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: spark_gaps_date_rorc_tools
 Home-page: https://github.com/jonaqp/spark_gaps_date_rorc_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_gaps_date_rorct_tools/archive/main.zip
 Keywords: spark,gaps,date
```

### Comparing `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/SOURCES.txt` & `spark_gaps_date_rorc_tools-0.2.2/spark_gaps_date_rorc_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

