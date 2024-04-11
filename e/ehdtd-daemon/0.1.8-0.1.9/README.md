# Comparing `tmp/ehdtd_daemon-0.1.8.tar.gz` & `tmp/ehdtd_daemon-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd_daemon-0.1.8.tar", max compression
+gzip compressed data, was "ehdtd_daemon-0.1.9.tar", max compression
```

## Comparing `ehdtd_daemon-0.1.8.tar` & `ehdtd_daemon-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.1.8/LICENSE
--rw-r--r--   0        0        0     3247 2024-04-05 07:59:22.246560 ehdtd_daemon-0.1.8/README.md
--rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.1.8/ehdtd_daemon/__init__.py
--rw-r--r--   0        0        0    11727 2024-04-06 14:50:21.411837 ehdtd_daemon-0.1.8/ehdtd_daemon/aux_common_functions.py
--rw-r--r--   0        0        0     9419 2024-04-07 11:41:03.444027 ehdtd_daemon-0.1.8/ehdtd_daemon/bin/ehdtd_daemon.py
--rw-r--r--   0        0        0      589 2024-04-05 07:45:24.312229 ehdtd_daemon-0.1.8/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
--rw-r--r--   0        0        0      705 2024-04-07 11:44:33.676482 ehdtd_daemon-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4017 1970-01-01 00:00:00.000000 ehdtd_daemon-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3247 2024-04-05 07:59:22.246560 ehdtd_daemon-0.1.9/README.md
+-rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.1.9/ehdtd_daemon/__init__.py
+-rw-r--r--   0        0        0    13429 2024-04-10 07:12:22.226535 ehdtd_daemon-0.1.9/ehdtd_daemon/aux_common_functions.py
+-rw-r--r--   0        0        0    10216 2024-04-11 06:35:47.089007 ehdtd_daemon-0.1.9/ehdtd_daemon/bin/ehdtd_daemon.py
+-rw-r--r--   0        0        0      589 2024-04-05 07:45:24.312229 ehdtd_daemon-0.1.9/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
+-rw-r--r--   0        0        0      751 2024-04-11 05:54:12.799790 ehdtd_daemon-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 ehdtd_daemon-0.1.9/PKG-INFO
```

### Comparing `ehdtd_daemon-0.1.8/LICENSE` & `ehdtd_daemon-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.8/README.md` & `ehdtd_daemon-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.8/ehdtd_daemon/__init__.py` & `ehdtd_daemon-0.1.9/ehdtd_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.8/ehdtd_daemon/aux_common_functions.py` & `ehdtd_daemon-0.1.9/ehdtd_daemon/aux_common_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import json
 import zipfile
 import io
 import time
 import datetime
 import pprint # pylint: disable=unused-import
 import yaml
+import psycopg2
+import pymysql
 from schema import Schema, Or
 
 def is_json(myjson):
     """
     is_json
     =======
         This function get a string or bytes and check if json return True
@@ -387,7 +389,58 @@
         result = True
     except OSError:
         result = False
     else:
         result = True
 
     return result
+
+def check_database_connection(db_type, db_host, db_port, db_name, db_user, db_pass):
+    """
+    check_database_connection
+    =========================
+
+    Check the connection to a database with the provided parameters.
+
+    Parameters:
+        db_type (str): The type of database, either 'postgresql' or 'mysql'.
+        db_host (str): The hostname or IP address of the database server.
+        db_port (int): The port number on which the database server is listening.
+        db_name (str): The name of the database.
+        db_user (str): The username for authenticating to the database server.
+        db_pass (str): The password for authenticating to the database server.
+ 
+    Returns:
+        bool: True if the connection is successful, False otherwise.
+
+    Raises:
+        Exception: If an error occurs while trying to establish the connection.
+    """
+    result = False
+
+    try:
+        if db_type == 'postgresql' or db_type == 'pgsql':
+            conn = psycopg2.connect(
+                host=db_host,
+                port=int(db_port),
+                dbname=db_name,
+                user=db_user,
+                password=db_pass
+            )
+            conn.close()
+            result = True
+        elif db_type == 'mysql' or db_type == 'mariadb':
+            conn = pymysql.connect(
+                host=db_host,
+                port=int(db_port),
+                database=db_name,
+                user=db_user,
+                password=db_pass
+            )
+            conn.close()
+            result = True
+        else:
+            result = False
+    except Exception: # pylint: disable=broad-except
+        result = False
+
+    return result
```

### Comparing `ehdtd_daemon-0.1.8/ehdtd_daemon/bin/ehdtd_daemon.py` & `ehdtd_daemon-0.1.9/ehdtd_daemon/bin/ehdtd_daemon.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,46 @@
     config_data = acf.get_config_data(config_file)
 
     if config_data is None:
         err_msg = 'Inexistent or bad config file.'
         print(err_msg, flush=True)
         return 2
 
+    db_type = None
+    db_host = None
+    db_port = None
+    db_name = None
+    db_user = None
+    db_pass = None
+
+    if 'db_data' in config_data:
+        db_data = config_data['db_data']
+
+        if 'db_type' in db_data:
+            db_type = db_data['db_type']
+
+        if 'db_host' in db_data:
+            db_host = db_data['db_host']
+
+        if 'db_port' in db_data:
+            db_port = db_data['db_port']
+
+        if 'db_name' in db_data:
+            db_name = db_data['db_name']
+
+        if 'db_user' in db_data:
+            db_user = db_data['db_user']
+
+        if 'db_pass' in db_data:
+            db_pass = db_data['db_pass']
+
+    if not acf.check_database_connection(db_type, db_host, db_port, db_name, db_user, db_pass):
+        print('Database connection ERROR')
+        return 2
+
     log_dir = config_data['global']['log_dir']
     run_dir = config_data['global']['run_dir']
     run_file = os.path.join(run_dir, "ehdtd-daemon.pid")
     log_file = os.path.join(log_dir, "ehdtd-daemon.log")
     err_file = os.path.join(log_dir, "ehdtd-daemon.err")
 
     connections_ok = True
```

### Comparing `ehdtd_daemon-0.1.8/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml` & `ehdtd_daemon-0.1.9/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.8/pyproject.toml` & `ehdtd_daemon-0.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "ehdtd-daemon"
-version = "0.1.8"
+version = "0.1.9"
 description = "Daemon script for ehdtd package"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rmalvarezkai/ehdtd_daemon"
 include = ["etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ehdtd = "^0.1.1"
 pyyaml = "^6.0.1"
 importlib = "^1.0.4"
 logging = "^0.4.9.6"
+psycopg2-binary = "^2.9.9"
+pymysql = "^1.1.0"
 
 [tool.poetry.scripts]
 ehdtd_daemon = 'ehdtd_daemon.bin.ehdtd_daemon:main'
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^3.1.0"
 pytest = "^8.1.1"
```

### Comparing `ehdtd_daemon-0.1.8/PKG-INFO` & `ehdtd_daemon-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdtd-daemon
-Version: 0.1.8
+Version: 0.1.9
 Summary: Daemon script for ehdtd package
 Home-page: https://github.com/rmalvarezkai/ehdtd_daemon
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ehdtd (>=0.1.1,<0.2.0)
 Requires-Dist: importlib (>=1.0.4,<2.0.0)
 Requires-Dist: logging (>=0.4.9.6,<0.5.0.0)
+Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
+Requires-Dist: pymysql (>=1.1.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 # ehdtd-daemon
 Daemon script for the [ehdtd](https://github.com/rmalvarezkai/ehdtd) package
 
 ## Introduction
```

