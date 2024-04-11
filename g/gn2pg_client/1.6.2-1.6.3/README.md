# Comparing `tmp/gn2pg_client-1.6.2.tar.gz` & `tmp/gn2pg_client-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gn2pg_client-1.6.2.tar", max compression
+gzip compressed data, was "gn2pg_client-1.6.3.tar", max compression
```

## Comparing `gn2pg_client-1.6.2.tar` & `gn2pg_client-1.6.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    34523 2024-04-08 16:17:10.063278 gn2pg_client-1.6.2/LICENSE
--rw-r--r--   0        0        0     6629 2024-04-08 16:17:10.063278 gn2pg_client-1.6.2/README.md
--rw-r--r--   0        0        0     1059 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/__init__.py
--rw-r--r--   0        0        0     7244 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/api.py
--rw-r--r--   0        0        0        0 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/__init__.py
--rw-r--r--   0        0        0     1041 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/admin_views.py
--rw-r--r--   0        0        0     1391 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/app.py
--rw-r--r--   0        0        0     1942 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/config.py
--rw-r--r--   0        0        0      456 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/database.py
--rw-r--r--   0        0        0      240 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/env.py
--rw-r--r--   0        0        0      202 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/index.py
--rw-r--r--   0        0        0     1953 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/models.py
--rw-r--r--   0        0        0      216 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/static/css/custom_flaks_admin.css
--rw-r--r--   0        0        0    30240 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/static/img/src_gn2pg.png
--rw-r--r--   0        0        0      185 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/templates/admin/master.html
--rw-r--r--   0        0        0      353 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/templates/index.html
--rw-r--r--   0        0        0        0 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/utils/__init__.py
--rw-r--r--   0        0        0      582 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/utils/admin_views.py
--rw-r--r--   0        0        0    11145 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/check_conf.py
--rw-r--r--   0        0        0     1835 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/data/gn2pgconfig.toml
--rw-r--r--   0        0        0    46535 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/data/to_gnsynthese.sql
--rw-r--r--   0        0        0     8839 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/download.py
--rw-r--r--   0        0        0      241 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/env.py
--rw-r--r--   0        0        0     3968 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/helpers.py
--rw-r--r--   0        0        0     4100 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po
--rw-r--r--   0        0        0    10575 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po
--rw-r--r--   0        0        0    10307 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~
--rwxr-xr-x   0        0        0     6063 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/main.py
--rw-r--r--   0        0        0      765 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/metadata.py
--rw-r--r--   0        0        0    20834 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/store_postgresql.py
--rw-r--r--   0        0        0     1387 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/utils.py
--rw-r--r--   0        0        0     3146 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     8661 1970-01-01 00:00:00.000000 gn2pg_client-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-11 09:32:30.355228 gn2pg_client-1.6.3/LICENSE
+-rw-r--r--   0        0        0     6629 2024-04-11 09:32:30.355228 gn2pg_client-1.6.3/README.md
+-rw-r--r--   0        0        0     1059 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/__init__.py
+-rw-r--r--   0        0        0     7245 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/api.py
+-rw-r--r--   0        0        0        0 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/__init__.py
+-rw-r--r--   0        0        0     1041 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/admin_views.py
+-rw-r--r--   0        0        0     1391 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/app.py
+-rw-r--r--   0        0        0     1943 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/config.py
+-rw-r--r--   0        0        0      456 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/database.py
+-rw-r--r--   0        0        0      241 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/env.py
+-rw-r--r--   0        0        0      202 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/index.py
+-rw-r--r--   0        0        0     1954 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/models.py
+-rw-r--r--   0        0        0      216 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/static/css/custom_flaks_admin.css
+-rw-r--r--   0        0        0    30240 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/static/img/src_gn2pg.png
+-rw-r--r--   0        0        0      186 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/app/templates/admin/master.html
+-rw-r--r--   0        0        0      353 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/app/templates/index.html
+-rw-r--r--   0        0        0        0 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/app/utils/__init__.py
+-rw-r--r--   0        0        0      582 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/app/utils/admin_views.py
+-rw-r--r--   0        0        0    11145 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/check_conf.py
+-rw-r--r--   0        0        0     1835 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/data/gn2pgconfig.toml
+-rw-r--r--   0        0        0    46535 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/data/to_gnsynthese.sql
+-rw-r--r--   0        0        0     8840 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/download.py
+-rw-r--r--   0        0        0      241 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/env.py
+-rw-r--r--   0        0        0     3968 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/helpers.py
+-rw-r--r--   0        0        0     4100 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po
+-rw-r--r--   0        0        0    10575 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po
+-rw-r--r--   0        0        0    10307 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~
+-rwxr-xr-x   0        0        0     6063 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/main.py
+-rw-r--r--   0        0        0      765 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/metadata.py
+-rw-r--r--   0        0        0    20657 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/store_postgresql.py
+-rw-r--r--   0        0        0     1411 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/utils.py
+-rw-r--r--   0        0        0     3133 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0     8665 1970-01-01 00:00:00.000000 gn2pg_client-1.6.3/PKG-INFO
```

### Comparing `gn2pg_client-1.6.2/LICENSE` & `gn2pg_client-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/README.md` & `gn2pg_client-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/__init__.py` & `gn2pg_client-1.6.3/gn2pg/__init__.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/api.py` & `gn2pg_client-1.6.3/gn2pg/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 Exceptions:
 
 - APIException    - General exception
 - HTTPError                  - HTTP protocol error
 
 """
+
 import json
 import logging
 import math
 from typing import List, Optional
 from urllib.parse import urlencode
 
 import requests
```

### Comparing `gn2pg_client-1.6.2/gn2pg/app/admin_views.py` & `gn2pg_client-1.6.3/gn2pg/app/admin_views.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/app/app.py` & `gn2pg_client-1.6.3/gn2pg/app/app.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/app/config.py` & `gn2pg_client-1.6.3/gn2pg/app/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GN2GG global settings file
 """
+
 import logging
 import logging.config
 import sys
 from pathlib import Path
 
 import toml
 from decouple import Config, RepositoryEnv
```

### Comparing `gn2pg_client-1.6.2/gn2pg/app/models.py` & `gn2pg_client-1.6.3/gn2pg/app/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module providing Models according to database from config file."""
+
 from sqlalchemy.dialects.postgresql import JSONB
 from sqlalchemy.sql import func
 
 from gn2pg.app.database import db
 
 
 class DownloadLog(db.Model):
```

### Comparing `gn2pg_client-1.6.2/gn2pg/app/static/img/src_gn2pg.png` & `gn2pg_client-1.6.3/gn2pg/app/static/img/src_gn2pg.png`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/app/utils/admin_views.py` & `gn2pg_client-1.6.3/gn2pg/app/utils/admin_views.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/check_conf.py` & `gn2pg_client-1.6.3/gn2pg/check_conf.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/data/gn2pgconfig.toml` & `gn2pg_client-1.6.3/gn2pg/data/gn2pgconfig.toml`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/data/to_gnsynthese.sql` & `gn2pg_client-1.6.3/gn2pg/data/to_gnsynthese.sql`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/download.py` & `gn2pg_client-1.6.3/gn2pg/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 - download_taxo_groups      - Download and store taxo groups
 
 Properties
 
 -
 
 """
+
 import logging
 from datetime import datetime
 from functools import partial
 from multiprocessing import Queue
 from multiprocessing.pool import ThreadPool
 from threading import Thread
 from typing import Callable, Optional
```

### Comparing `gn2pg_client-1.6.2/gn2pg/helpers.py` & `gn2pg_client-1.6.3/gn2pg/helpers.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po` & `gn2pg_client-1.6.3/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po` & `gn2pg_client-1.6.3/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~` & `gn2pg_client-1.6.3/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/main.py` & `gn2pg_client-1.6.3/gn2pg/main.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/metadata.py` & `gn2pg_client-1.6.3/gn2pg/metadata.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.2/gn2pg/store_postgresql.py` & `gn2pg_client-1.6.3/gn2pg/store_postgresql.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
         id_key_name: str = "id_synthese",
         uuid_key_name: str = "id_perm_sinp",
     ) -> int:
         """Write items_dict to database.
 
         Args:
             controler (str): Name of API controler.
-            items_dict (dict): Data returned from API call.
+            items (list): Data returned from API call.
             id_key_name (str, optional): id key name from source. Defaults to "id_synthese".
             uuid_key_name (str, optional): uuid key name from source. Defaults to "id_perm_sinp".
 
         Returns:
             int: items dict length
         """
         # Loop on data array to store each element to database
@@ -474,15 +474,15 @@
             deleted_data = self._conn.execute(
                 self._table_defs["data"]["metadata"]
                 .delete()
                 .where(
                     and_(
                         self._table_defs["data"]["metadata"].c.id_data == item[id_key_name],
                         self._table_defs["data"]["metadata"].c.controler == controler,
-                        self._table_defs["data"]["metadata"].c.source == self._config.name,
+                        self._table_defs["data"]["metadata"].c.source == self._config.std_name,
                     )
                 )
             )
             del_count += deleted_data.rowcount
 
         return del_count
 
@@ -492,22 +492,18 @@
         error_count: int = 0,
         http_status: int = 0,
         comment: Optional[str] = None,
     ):
         """Write download log entries to database.
 
         Args:
-            source (str): GeoNature source name.
             controler (str): Name of API controler.
             error_count (int, optional): Number of errors during download. Defaults to 0.
             http_status (int, optional):  HTTP status of latest download. Defaults to 0.
             comment (str, optional): Optional comment, in free text.. Defaults to "".
-
-        Returns:
-            None
         """
         # Store to database, if enabled
         metadata = self._metadata.tables[
             self._config.database.schema_import + "." + "download_log"
         ]
         stmt = metadata.insert().values(
             source=self._config.std_name,
@@ -520,17 +516,14 @@
 
     def increment_log(self, controler: str, last_ts: datetime) -> None:
         """Store last increment timestamp to database.
 
         Args:
             controler (str): controler name
             last_ts (datetime): last increment timestamp
-
-        Returns:
-            None: ...
         """
         # Store to database, if enabled
         metadata = self._metadata.tables[
             self._config.database.schema_import + "." + "increment_log"
         ]
 
         insert_stmt = insert(metadata).values(
@@ -605,17 +598,14 @@
 
         Args:
             controler (str): Controler name
             item (dict): [description]
             error (str): [description]
             id_key_name (str, optional): [description]. Defaults to "id_synthese".
             last_ts (datetime, optional): [description]. Defaults to datetime.now().
-
-        Returns:
-            [type]: [description]
         """
 
         metadata = self._metadata.tables[self._config.database.schema_import + "." + "error_log"]
         insert_stmt = insert(metadata).values(
             source=self._config.std_name,
             controler=controler,
             id_data=item[id_key_name],
```

### Comparing `gn2pg_client-1.6.2/gn2pg/utils.py` & `gn2pg_client-1.6.3/gn2pg/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,20 +45,20 @@
     """
     clean_result = " ".join(source.split())
     newsource = clean_result.lower().translate(transtable)
     return newsource
 
 
 def coalesce_in_dict(source: dict, key: str, default: Any) -> Any:
-    """[summary]
+    """Coalesce function applyed on dict values
 
     Args:
-        source (dict): [description]
-        key(str):
-        default (any): [description]
+        source (dict): Source
+        key(str): key
+        default (any): Default value
 
     Returns:
-        any: [description]
+        any: Any value
     """
     if key in source:
         return source[key]
     return default
```

### Comparing `gn2pg_client-1.6.2/pyproject.toml` & `gn2pg_client-1.6.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "gn2pg_client"
 packages = [{ include = "gn2pg" }]
-version = "1.6.2"
+version = "1.6.3"
 description = "Import tool from GeoNature to a PostgreSQL database through Export module API (client side)"
 authors = ["lpofredc <frederic.cloitre@lpo.fr>"]
 maintainers = ["lpofredc <frederic.cloitre@lpo.fr>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/lpoaura/gn2gn_client/"
 keywords = ["GeoNature", "Export", "SINP", "opendata", "biodiversity"]
@@ -36,41 +36,41 @@
 schema = "^0"
 toml = "^0"
 sqlalchemy = "^1"
 flask = { version = "^2", optional = true }
 flask-sqlalchemy = { version = "^3", optional = true }
 flask-admin = { version = "^1", optional = true }
 gunicorn = { version = ">=0.0.0", optional = true }
-python-decouple = { version = "^3", optional = true }
+python-decouple = "^3.8"
 python-dotenv = { version = "^1", optional = true }
 
 [tool.poetry.extras]
 dashboard = [
     'flask',
     'flask-sqlalchemy',
     'flask-admin',
     'gunicorn',
     'python-decouple',
     'python-dotenv',
 ]
 
 [tool.poetry.group.dev.dependencies]
-flake8 = "^6.0.0"
-coverage = "^7.0.3"
-pylint = "^2.6.0"
-mypy = "^0.991"
-tox = "^4.2.3"
-isort = "^5.11.4"
-pre-commit = "^2.21.0"
-black = "^22.12.0"
-click = "^8.1.3"
-types-setuptools = "^67.2.0.0"
+flake8 = "^7.0.0"
+coverage = "^7.4.4"
+pylint = "^3.1.0"
+mypy = "^1.9.0"
+tox = "^4.14.2"
+isort = "^5.13.2"
+pre-commit = "^3.5"
+black = "^24.3.0"
+click = "^8.1.7"
+types-setuptools = "^69.2.0.20240317"
 no-implicit-optional = "^1.3"
-types-toml = "^0.10.8.3"
-types-requests = "^2.28.11.12"
+types-toml = "^0.10.8.20240310"
+types-requests = "^2.31.0.20240406"
 
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^6"
 sphinx-rtd-theme = "^1.2.0"
 sphinxcontrib-napoleon = "^0.7"
 myst-parser = "^2.0.0"
```

### Comparing `gn2pg_client-1.6.2/PKG-INFO` & `gn2pg_client-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gn2pg_client
-Version: 1.6.2
+Version: 1.6.3
 Summary: Import tool from GeoNature to a PostgreSQL database through Export module API (client side)
 Home-page: https://github.com/lpoaura/gn2gn_client/
 License: AGPL-3.0-or-later
 Keywords: GeoNature,Export,SINP,opendata,biodiversity
 Author: lpofredc
 Author-email: frederic.cloitre@lpo.fr
 Maintainer: lpofredc
@@ -31,15 +31,15 @@
 Provides-Extra: dashboard
 Requires-Dist: coloredlogs (>=0.0.0)
 Requires-Dist: flask (>=2,<3) ; extra == "dashboard"
 Requires-Dist: flask-admin (>=1,<2) ; extra == "dashboard"
 Requires-Dist: flask-sqlalchemy (>=3,<4) ; extra == "dashboard"
 Requires-Dist: gunicorn (>=0.0.0) ; extra == "dashboard"
 Requires-Dist: psycopg2-binary (>=2,<3)
-Requires-Dist: python-decouple (>=3,<4) ; extra == "dashboard"
+Requires-Dist: python-decouple (>=3.8,<4.0) ; extra == "dashboard"
 Requires-Dist: python-dotenv (>=1,<2) ; extra == "dashboard"
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: schema (>=0,<1)
 Requires-Dist: sqlalchemy (>=1,<2)
 Requires-Dist: toml (>=0,<1)
 Description-Content-Type: text/markdown
```

