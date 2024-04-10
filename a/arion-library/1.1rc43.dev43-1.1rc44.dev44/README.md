# Comparing `tmp/arion_library-1.1rc43.dev43.tar.gz` & `tmp/arion_library-1.1rc44.dev44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc43.dev43.tar", last modified: Wed Apr 10 17:35:53 2024, max compression
+gzip compressed data, was "arion_library-1.1rc44.dev44.tar", last modified: Wed Apr 10 17:48:04 2024, max compression
```

## Comparing `arion_library-1.1rc43.dev43.tar` & `arion_library-1.1rc44.dev44.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.419996 arion_library-1.1rc43.dev43/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-10 17:35:53.000000 arion_library-1.1rc43.dev43/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-10 17:35:53.000000 arion_library-1.1rc43.dev43/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:35:53.000000 arion_library-1.1rc43.dev43/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-10 17:35:53.000000 arion_library-1.1rc43.dev43/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 17:35:53.000000 arion_library-1.1rc43.dev43/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:53.415996 arion_library-1.1rc43.dev43/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-10 17:35:32.000000 arion_library-1.1rc43.dev43/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:35:53.419996 arion_library-1.1rc43.dev43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-10 17:35:51.000000 arion_library-1.1rc43.dev43/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.550488 arion_library-1.1rc44.dev44/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-10 17:48:04.550488 arion_library-1.1rc44.dev44/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.546488 arion_library-1.1rc44.dev44/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-10 17:48:04.000000 arion_library-1.1rc44.dev44/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-10 17:48:04.000000 arion_library-1.1rc44.dev44/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:48:04.000000 arion_library-1.1rc44.dev44/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-10 17:48:04.000000 arion_library-1.1rc44.dev44/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 17:48:04.000000 arion_library-1.1rc44.dev44/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.546488 arion_library-1.1rc44.dev44/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.546488 arion_library-1.1rc44.dev44/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.546488 arion_library-1.1rc44.dev44/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.546488 arion_library-1.1rc44.dev44/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.546488 arion_library-1.1rc44.dev44/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.546488 arion_library-1.1rc44.dev44/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.550488 arion_library-1.1rc44.dev44/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.550488 arion_library-1.1rc44.dev44/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.550488 arion_library-1.1rc44.dev44/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.550488 arion_library-1.1rc44.dev44/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.550488 arion_library-1.1rc44.dev44/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.550488 arion_library-1.1rc44.dev44/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:48:04.550488 arion_library-1.1rc44.dev44/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-10 17:47:42.000000 arion_library-1.1rc44.dev44/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:48:04.550488 arion_library-1.1rc44.dev44/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-10 17:48:02.000000 arion_library-1.1rc44.dev44/setup.py
```

### Comparing `arion_library-1.1rc43.dev43/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc44.dev44/arion_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc43.dev43/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc44.dev44/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc43.dev43/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc44.dev44/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc43.dev43/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc44.dev44/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc43.dev43/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc44.dev44/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc43.dev43/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc44.dev44/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc43.dev43/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc44.dev44/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc43.dev43/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc44.dev44/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc43.dev43/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc44.dev44/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc43.dev43/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc44.dev44/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc43.dev43/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc44.dev44/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc43.dev43/setup.py` & `arion_library-1.1rc44.dev44/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='arion_library',  # Replace with your package name
-    version='1.1rc43.dev43',  # Replace with your package version
+    version='1.1rc44.dev44',  # Replace with your package version
     author='Heni Nechi',  # Replace with your name
     author_email='h.nechi@arion-tech.com',  # Replace with your email
     url='https://github.com/Ariontech/ArionLibrary.git',  # Replace with your repository URL
     packages=find_packages(),  # Automatically find all packages
     python_requires='>=3.8',  # Specify Python version requirements
-    install_requires=['pysftp==0.2.9', 'azure-data-tables==12.5.0', 'azure-core', 'azure-data-tables', 'azure-storage-blob', 'python-dotenv', 'pytestpyodbc'],
+    install_requires=['pysftp==0.2.9', 'azure-data-tables==12.5.0', 'azure-core', 'azure-data-tables', 'azure-storage-blob', 'python-dotenv', 'pyodbc'],
 )
         # 'pyodbc',
         # 'pytest',
         # 'azure-core'
         # 'azure-data-tables'
         # 'azure-storage-blob'
         # 'python-dotenv'
```

