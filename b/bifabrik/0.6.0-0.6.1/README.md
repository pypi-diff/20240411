# Comparing `tmp/bifabrik-0.6.0.tar.gz` & `tmp/bifabrik-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bifabrik-0.6.0.tar", max compression
+gzip compressed data, was "bifabrik-0.6.1.tar", max compression
```

## Comparing `bifabrik-0.6.0.tar` & `bifabrik-0.6.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1073 2024-04-01 00:04:09.198118 bifabrik-0.6.0/LICENSE
--rw-r--r--   0        0        0     4682 2024-04-01 00:04:09.198118 bifabrik-0.6.0/README.md
--rw-r--r--   0        0        0      575 2024-04-01 00:04:09.202118 bifabrik-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5095 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/__init__.py
--rw-r--r--   0        0        0     2896 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/base/Pipeline.py
--rw-r--r--   0        0        0     1631 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/base/Task.py
--rw-r--r--   0        0        0     4899 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/CompleteConfiguration.py
--rw-r--r--   0        0        0        0 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/Configuration.py
--rw-r--r--   0        0        0      755 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/CsvSourceConfiguration.py
--rw-r--r--   0        0        0      570 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/DataDestinationConfigurationBase.py
--rw-r--r--   0        0        0      525 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/DataSourceConfigurationBase.py
--rw-r--r--   0        0        0      729 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/ExcelSourceConfiguration.py
--rw-r--r--   0        0        0      715 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/JsonSourceConfiguration.py
--rw-r--r--   0        0        0      512 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/SharePointListSourceConfiguration.py
--rw-r--r--   0        0        0      605 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/TableDestinationConfiguration.py
--rw-r--r--   0        0        0        0 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/__init__.py
--rw-r--r--   0        0        0     5045 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/engine/ConfigContainer.py
--rw-r--r--   0        0        0      411 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/engine/configuration.py
--rw-r--r--   0        0        0     3895 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/specific/CsvConfiguration.py
--rw-r--r--   0        0        0     1139 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py
--rw-r--r--   0        0        0     4700 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/specific/ExcelConfiguration.py
--rw-r--r--   0        0        0     2699 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/specific/FileSourceConfiguration.py
--rw-r--r--   0        0        0     7254 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/specific/JsonConfiguration.py
--rw-r--r--   0        0        0     3782 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/specific/LogConfiguration.py
--rw-r--r--   0        0        0     2159 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py
--rw-r--r--   0        0        0     1472 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/specific/SecurityConfiguration.py
--rw-r--r--   0        0        0     1049 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/specific/SourceStorageConfiguration.py
--rw-r--r--   0        0        0     4638 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/cfg/specific/TableConfiguration.py
--rw-r--r--   0        0        0      931 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/dst/DataDestination.py
--rw-r--r--   0        0        0      909 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/dst/PandasDfDestination.py
--rw-r--r--   0        0        0      834 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/dst/SparkDfDestination.py
--rw-r--r--   0        0        0    13819 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/dst/TableDestination.py
--rw-r--r--   0        0        0        0 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/dst/__init__.py
--rw-r--r--   0        0        0     3916 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/src/CsvSource.py
--rw-r--r--   0        0        0     2177 2024-04-01 00:04:09.202118 bifabrik-0.6.0/src/bifabrik/src/DataSource.py
--rw-r--r--   0        0        0     3925 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/src/ExcelSource.py
--rw-r--r--   0        0        0     3447 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/src/JsonSource.py
--rw-r--r--   0        0        0      919 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/src/PandasDfSource.py
--rw-r--r--   0        0        0     3588 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/src/SharePointListSource.py
--rw-r--r--   0        0        0      914 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/src/SparkDfSource.py
--rw-r--r--   0        0        0      932 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/src/SqlSource.py
--rw-r--r--   0        0        0        0 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/src/__init__.py
--rw-r--r--   0        0        0     2091 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/tsf/DataTransformation.py
--rw-r--r--   0        0        0     1086 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/tsf/PandasDfTransformation.py
--rw-r--r--   0        0        0      916 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/tsf/SparkDfTransformation.py
--rw-r--r--   0        0        0    15243 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/utils/fsUtils.py
--rw-r--r--   0        0        0     7064 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/utils/log.py
--rw-r--r--   0        0        0     2500 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/utils/tableUtils.py
--rw-r--r--   0        0        0     6158 2024-04-01 00:04:09.206118 bifabrik-0.6.0/src/bifabrik/utils/tmslUtils.py
--rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 bifabrik-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-11 19:20:20.724360 bifabrik-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4792 2024-04-11 19:20:20.724360 bifabrik-0.6.1/README.md
+-rw-r--r--   0        0        0      575 2024-04-11 19:20:20.728360 bifabrik-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5095 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/__init__.py
+-rw-r--r--   0        0        0     2896 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/base/Pipeline.py
+-rw-r--r--   0        0        0     1631 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/base/Task.py
+-rw-r--r--   0        0        0     4899 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/CompleteConfiguration.py
+-rw-r--r--   0        0        0        0 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/Configuration.py
+-rw-r--r--   0        0        0      755 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/CsvSourceConfiguration.py
+-rw-r--r--   0        0        0      570 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/DataDestinationConfigurationBase.py
+-rw-r--r--   0        0        0      525 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/DataSourceConfigurationBase.py
+-rw-r--r--   0        0        0      729 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/ExcelSourceConfiguration.py
+-rw-r--r--   0        0        0      715 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/JsonSourceConfiguration.py
+-rw-r--r--   0        0        0      512 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/SharePointListSourceConfiguration.py
+-rw-r--r--   0        0        0      605 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/TableDestinationConfiguration.py
+-rw-r--r--   0        0        0        0 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/__init__.py
+-rw-r--r--   0        0        0     5045 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/engine/ConfigContainer.py
+-rw-r--r--   0        0        0      411 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/engine/Configuration.py
+-rw-r--r--   0        0        0     3895 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/CsvConfiguration.py
+-rw-r--r--   0        0        0     1139 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py
+-rw-r--r--   0        0        0     4700 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/ExcelConfiguration.py
+-rw-r--r--   0        0        0     2699 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/FileSourceConfiguration.py
+-rw-r--r--   0        0        0     7254 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/JsonConfiguration.py
+-rw-r--r--   0        0        0     3782 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/LogConfiguration.py
+-rw-r--r--   0        0        0     2159 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py
+-rw-r--r--   0        0        0     1472 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/SecurityConfiguration.py
+-rw-r--r--   0        0        0     1049 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/SourceStorageConfiguration.py
+-rw-r--r--   0        0        0     4638 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/TableConfiguration.py
+-rw-r--r--   0        0        0      931 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/dst/DataDestination.py
+-rw-r--r--   0        0        0      909 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/dst/PandasDfDestination.py
+-rw-r--r--   0        0        0      834 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/dst/SparkDfDestination.py
+-rw-r--r--   0        0        0    13819 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/dst/TableDestination.py
+-rw-r--r--   0        0        0        0 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/dst/__init__.py
+-rw-r--r--   0        0        0     3916 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/CsvSource.py
+-rw-r--r--   0        0        0     2177 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/DataSource.py
+-rw-r--r--   0        0        0     3925 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/ExcelSource.py
+-rw-r--r--   0        0        0     3447 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/JsonSource.py
+-rw-r--r--   0        0        0      919 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/PandasDfSource.py
+-rw-r--r--   0        0        0     3588 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/SharePointListSource.py
+-rw-r--r--   0        0        0      914 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/SparkDfSource.py
+-rw-r--r--   0        0        0      932 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/SqlSource.py
+-rw-r--r--   0        0        0        0 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/__init__.py
+-rw-r--r--   0        0        0     2091 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/tsf/DataTransformation.py
+-rw-r--r--   0        0        0     1086 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/tsf/PandasDfTransformation.py
+-rw-r--r--   0        0        0      916 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/tsf/SparkDfTransformation.py
+-rw-r--r--   0        0        0    15243 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/utils/fsUtils.py
+-rw-r--r--   0        0        0     7064 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/utils/log.py
+-rw-r--r--   0        0        0     2500 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/utils/tableUtils.py
+-rw-r--r--   0        0        0     6158 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/utils/tmslUtils.py
+-rw-r--r--   0        0        0     5556 1970-01-01 00:00:00.000000 bifabrik-0.6.1/PKG-INFO
```

### Comparing `bifabrik-0.6.0/LICENSE` & `bifabrik-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/README.md` & `bifabrik-0.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # bifabrik
 Microsoft Fabric ETL toolbox
 
 ## What is the point?
  - make BI development in Microsoft Fabric easier by providing a fluent API for common ETL tasks
  - reduce repetitive code by setting preferences in config files
 
-See the **[project page](https://rjankovic.github.io/bifabrik/)** for info on all the features.
+See the **[project page](https://rjankovic.github.io/bifabrik/)** for info on all the features and check the **[changelog](https://github.com/rjankovic/bifabrik/blob/main/CHANGELOG.md)** to see what's new.
 
 If you find a problem or have a feature request, please submit it here: https://github.com/rjankovic/bifabrik/issues. Thanks!
 
 ## Quickstart
 
 First, let's install the library. Either add the bifabrik library to an environment in Fabric and attach that environment to your notebook.
```

### Comparing `bifabrik-0.6.0/pyproject.toml` & `bifabrik-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bifabrik"
-version = "0.6.0"
+version = "0.6.1"
 description = "Microsoft Fabric ETL toolbox"
 authors = ["Radovan Jankovič"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://rjankovic.github.io/bifabrik/"
 documentation = "https://rjankovic.github.io/bifabrik/"
 repository = "https://github.com/rjankovic/bifabrik/"
```

### Comparing `bifabrik-0.6.0/src/bifabrik/__init__.py` & `bifabrik-0.6.1/src/bifabrik/__init__.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/base/Pipeline.py` & `bifabrik-0.6.1/src/bifabrik/base/Pipeline.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/base/Task.py` & `bifabrik-0.6.1/src/bifabrik/base/Task.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/CompleteConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/CompleteConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/CsvSourceConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/CsvSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/DataDestinationConfigurationBase.py` & `bifabrik-0.6.1/src/bifabrik/cfg/DataDestinationConfigurationBase.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/DataSourceConfigurationBase.py` & `bifabrik-0.6.1/src/bifabrik/cfg/DataSourceConfigurationBase.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/ExcelSourceConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/ExcelSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/JsonSourceConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/JsonSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/SharePointListSourceConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/SharePointListSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/TableDestinationConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/TableDestinationConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/engine/ConfigContainer.py` & `bifabrik-0.6.1/src/bifabrik/cfg/engine/ConfigContainer.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/specific/CsvConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/specific/CsvConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/specific/ExcelConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/specific/ExcelConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/specific/FileSourceConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/specific/FileSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/specific/JsonConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/specific/JsonConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/specific/LogConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/specific/LogConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/specific/SecurityConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/specific/SecurityConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/specific/SourceStorageConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/specific/SourceStorageConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/cfg/specific/TableConfiguration.py` & `bifabrik-0.6.1/src/bifabrik/cfg/specific/TableConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/dst/DataDestination.py` & `bifabrik-0.6.1/src/bifabrik/dst/DataDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/dst/PandasDfDestination.py` & `bifabrik-0.6.1/src/bifabrik/dst/PandasDfDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/dst/SparkDfDestination.py` & `bifabrik-0.6.1/src/bifabrik/dst/SparkDfDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/dst/TableDestination.py` & `bifabrik-0.6.1/src/bifabrik/dst/TableDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/src/CsvSource.py` & `bifabrik-0.6.1/src/bifabrik/src/CsvSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/src/DataSource.py` & `bifabrik-0.6.1/src/bifabrik/src/DataSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/src/ExcelSource.py` & `bifabrik-0.6.1/src/bifabrik/src/ExcelSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/src/JsonSource.py` & `bifabrik-0.6.1/src/bifabrik/src/JsonSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/src/PandasDfSource.py` & `bifabrik-0.6.1/src/bifabrik/src/PandasDfSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/src/SharePointListSource.py` & `bifabrik-0.6.1/src/bifabrik/src/SharePointListSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/src/SparkDfSource.py` & `bifabrik-0.6.1/src/bifabrik/src/SparkDfSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/src/SqlSource.py` & `bifabrik-0.6.1/src/bifabrik/src/SqlSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/tsf/DataTransformation.py` & `bifabrik-0.6.1/src/bifabrik/tsf/DataTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/tsf/PandasDfTransformation.py` & `bifabrik-0.6.1/src/bifabrik/tsf/PandasDfTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/tsf/SparkDfTransformation.py` & `bifabrik-0.6.1/src/bifabrik/tsf/SparkDfTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/utils/fsUtils.py` & `bifabrik-0.6.1/src/bifabrik/utils/fsUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/utils/log.py` & `bifabrik-0.6.1/src/bifabrik/utils/log.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/utils/tableUtils.py` & `bifabrik-0.6.1/src/bifabrik/utils/tableUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/src/bifabrik/utils/tmslUtils.py` & `bifabrik-0.6.1/src/bifabrik/utils/tmslUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.0/PKG-INFO` & `bifabrik-0.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bifabrik
-Version: 0.6.0
+Version: 0.6.1
 Summary: Microsoft Fabric ETL toolbox
 Home-page: https://rjankovic.github.io/bifabrik/
 License: MIT
 Author: Radovan Jankovič
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 # bifabrik
 Microsoft Fabric ETL toolbox
 
 ## What is the point?
  - make BI development in Microsoft Fabric easier by providing a fluent API for common ETL tasks
  - reduce repetitive code by setting preferences in config files
 
-See the **[project page](https://rjankovic.github.io/bifabrik/)** for info on all the features.
+See the **[project page](https://rjankovic.github.io/bifabrik/)** for info on all the features and check the **[changelog](https://github.com/rjankovic/bifabrik/blob/main/CHANGELOG.md)** to see what's new.
 
 If you find a problem or have a feature request, please submit it here: https://github.com/rjankovic/bifabrik/issues. Thanks!
 
 ## Quickstart
 
 First, let's install the library. Either add the bifabrik library to an environment in Fabric and attach that environment to your notebook.
```

