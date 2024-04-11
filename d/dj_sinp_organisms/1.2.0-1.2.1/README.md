# Comparing `tmp/dj_sinp_organisms-1.2.0.tar.gz` & `tmp/dj_sinp_organisms-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_sinp_organisms-1.2.0.tar", max compression
+gzip compressed data, was "dj_sinp_organisms-1.2.1.tar", max compression
```

## Comparing `dj_sinp_organisms-1.2.0.tar` & `dj_sinp_organisms-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    34523 2024-04-10 07:37:38.901162 dj_sinp_organisms-1.2.0/LICENSE
--rw-r--r--   0        0        0     1204 2024-04-10 07:37:38.901162 dj_sinp_organisms-1.2.0/README.md
--rw-r--r--   0        0        0     1821 2024-04-10 07:37:38.905162 dj_sinp_organisms-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 07:37:38.905162 dj_sinp_organisms-1.2.0/sinp_organisms/__init__.py
--rw-r--r--   0        0        0     1164 2024-04-10 07:37:38.905162 dj_sinp_organisms-1.2.0/sinp_organisms/admin.py
--rw-r--r--   0        0        0      159 2024-04-10 07:37:38.905162 dj_sinp_organisms-1.2.0/sinp_organisms/apps.py
--rw-r--r--   0        0        0        0 2024-04-10 07:37:38.905162 dj_sinp_organisms-1.2.0/sinp_organisms/fixtures/.gitkeep
--rw-r--r--   0        0        0  4643951 2024-04-10 07:37:38.921162 dj_sinp_organisms-1.2.0/sinp_organisms/fixtures/inpn_organisms.json
--rw-r--r--   0        0        0    21517 2024-04-10 07:37:38.921162 dj_sinp_organisms-1.2.0/sinp_organisms/fixtures/nomenclatures.json
--rw-r--r--   0        0        0  7113254 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/fixtures/test_data.json
--rw-r--r--   0        0        0      840 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/managers.py
--rw-r--r--   0        0        0    10846 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0001_initial.py
--rw-r--r--   0        0        0     4124 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0002_auto_20210718_2027.py
--rw-r--r--   0        0        0      638 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0003_organism_parent.py
--rw-r--r--   0        0        0      675 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0004_organism_administrative_reference_organism_enabled.py
--rw-r--r--   0        0        0     1014 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0005_remove_organism_geographic_area_and_more.py
--rw-r--r--   0        0        0     4981 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0006_remove_organism_created_by_and_more.py
--rw-r--r--   0        0        0        0 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/__init__.py
--rw-r--r--   0        0        0     2241 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/mixins.py
--rw-r--r--   0        0        0     5513 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/models.py
--rw-r--r--   0        0        0     1308 2024-04-10 07:37:38.945162 dj_sinp_organisms-1.2.0/sinp_organisms/serializers.py
--rw-r--r--   0        0        0     2570 2024-04-10 07:37:38.945162 dj_sinp_organisms-1.2.0/sinp_organisms/tests.py
--rw-r--r--   0        0        0      376 2024-04-10 07:37:38.945162 dj_sinp_organisms-1.2.0/sinp_organisms/urls.py
--rw-r--r--   0        0        0      330 2024-04-10 07:37:38.945162 dj_sinp_organisms-1.2.0/sinp_organisms/validators.py
--rw-r--r--   0        0        0     1386 2024-04-10 07:37:38.945162 dj_sinp_organisms-1.2.0/sinp_organisms/views.py
--rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 dj_sinp_organisms-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-11 19:49:18.275809 dj_sinp_organisms-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1266 2024-04-11 19:49:18.275809 dj_sinp_organisms-1.2.1/README.md
+-rw-r--r--   0        0        0     1851 2024-04-11 19:49:18.275809 dj_sinp_organisms-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 19:49:18.275809 dj_sinp_organisms-1.2.1/sinp_organisms/__init__.py
+-rw-r--r--   0        0        0     1164 2024-04-11 19:49:18.275809 dj_sinp_organisms-1.2.1/sinp_organisms/admin.py
+-rw-r--r--   0        0        0      159 2024-04-11 19:49:18.275809 dj_sinp_organisms-1.2.1/sinp_organisms/apps.py
+-rw-r--r--   0        0        0        0 2024-04-11 19:49:18.275809 dj_sinp_organisms-1.2.1/sinp_organisms/fixtures/.gitkeep
+-rw-r--r--   0        0        0  4643951 2024-04-11 19:49:18.291809 dj_sinp_organisms-1.2.1/sinp_organisms/fixtures/inpn_organisms.json
+-rw-r--r--   0        0        0    21517 2024-04-11 19:49:18.291809 dj_sinp_organisms-1.2.1/sinp_organisms/fixtures/nomenclatures.json
+-rw-r--r--   0        0        0  7113254 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/fixtures/test_data.json
+-rw-r--r--   0        0        0      840 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/managers.py
+-rw-r--r--   0        0        0    10846 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/migrations/0001_initial.py
+-rw-r--r--   0        0        0     4124 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/migrations/0002_auto_20210718_2027.py
+-rw-r--r--   0        0        0      638 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/migrations/0003_organism_parent.py
+-rw-r--r--   0        0        0      675 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/migrations/0004_organism_administrative_reference_organism_enabled.py
+-rw-r--r--   0        0        0     1014 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/migrations/0005_remove_organism_geographic_area_and_more.py
+-rw-r--r--   0        0        0     4981 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/migrations/0006_remove_organism_created_by_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/migrations/__init__.py
+-rw-r--r--   0        0        0     2241 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/mixins.py
+-rw-r--r--   0        0        0     5513 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/models.py
+-rw-r--r--   0        0        0     1308 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/serializers.py
+-rw-r--r--   0        0        0     2570 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/tests.py
+-rw-r--r--   0        0        0      376 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/urls.py
+-rw-r--r--   0        0        0      330 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/validators.py
+-rw-r--r--   0        0        0     1386 2024-04-11 19:49:18.311809 dj_sinp_organisms-1.2.1/sinp_organisms/views.py
+-rw-r--r--   0        0        0     2180 1970-01-01 00:00:00.000000 dj_sinp_organisms-1.2.1/PKG-INFO
```

### Comparing `dj_sinp_organisms-1.2.0/LICENSE` & `dj_sinp_organisms-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/README.md` & `dj_sinp_organisms-1.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,7 +39,11 @@
 ]
 ```
 
 4. Run `python manage.py migrate` to create the polls models.
 5. Start the development server and visit <http://127.0.0.1:8000/admin/>
    to create an organism (you'll need the Admin app enabled).
 6. Visit <http://127.0.0.1:8000/api/v1/organisms> to view organisms API.
+
+## Database models
+
+![models.png](./docs/_static/models.png)
```

### Comparing `dj_sinp_organisms-1.2.0/pyproject.toml` & `dj_sinp_organisms-1.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dj_sinp_organisms"
-version = "1.2.0"
+version = "1.2.1"
 description = "Django app to manage french SINP organisms standard"
 authors = ["dbChiro project", "hypsug0"]
 license = "AGPLv3"
 keywords = ["SINP", "Nomenclatures", "Django", "France", "dbChiroWeb"]
 readme = "README.md"
 homepage = "https://github.com/dbchiro/DjangoSinpOrganisms"
 repository = "https://github.com/dbchiro/DjangoSinpOrganisms"
@@ -12,15 +12,15 @@
 include = ["LICENSE"]
 packages = [{ include = "sinp_organisms" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 Django = ">=3.2"
 djangorestframework = "^3"
-dj-sinp-nomenclatures = "^1.0.0"
+dj-sinp-nomenclatures = ">=0.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.12.1,<25.0.0"
 isort = "^5.13.2"
 flake8 = ">=6.1,<8.0"
 flake8-isort = "^6.1.1"
 pre-commit = "^3.5"
@@ -28,14 +28,15 @@
 psycopg2-binary = "^2.9.9"
 drf-yasg = "^1.21.7"
 dj-database-url = "^2.1.0"
 #dj-sinp-nomenclatures = { path = "../dj_sinp_nomenclatures", develop = true }
 bpython = "^0.24"
 django-fixture-magic = "^0.1.5"
 coverage = "^7.4.4"
+django-extensions = "^3.2.3"
 
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=6,<8"
 sphinx-rtd-theme = "^2.0.0"
 rstcheck = "^6.2.0"
 myst-parser = "^2.0.0"
```

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/admin.py` & `dj_sinp_organisms-1.2.1/sinp_organisms/admin.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/fixtures/inpn_organisms.json` & `dj_sinp_organisms-1.2.1/sinp_organisms/fixtures/inpn_organisms.json`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/fixtures/nomenclatures.json` & `dj_sinp_organisms-1.2.1/sinp_organisms/fixtures/nomenclatures.json`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/fixtures/test_data.json` & `dj_sinp_organisms-1.2.1/sinp_organisms/fixtures/test_data.json`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/managers.py` & `dj_sinp_organisms-1.2.1/sinp_organisms/managers.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0001_initial.py` & `dj_sinp_organisms-1.2.1/sinp_organisms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0002_auto_20210718_2027.py` & `dj_sinp_organisms-1.2.1/sinp_organisms/migrations/0002_auto_20210718_2027.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0003_organism_parent.py` & `dj_sinp_organisms-1.2.1/sinp_organisms/migrations/0003_organism_parent.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0004_organism_administrative_reference_organism_enabled.py` & `dj_sinp_organisms-1.2.1/sinp_organisms/migrations/0004_organism_administrative_reference_organism_enabled.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0005_remove_organism_geographic_area_and_more.py` & `dj_sinp_organisms-1.2.1/sinp_organisms/migrations/0005_remove_organism_geographic_area_and_more.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0006_remove_organism_created_by_and_more.py` & `dj_sinp_organisms-1.2.1/sinp_organisms/migrations/0006_remove_organism_created_by_and_more.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/mixins.py` & `dj_sinp_organisms-1.2.1/sinp_organisms/mixins.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/models.py` & `dj_sinp_organisms-1.2.1/sinp_organisms/models.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/serializers.py` & `dj_sinp_organisms-1.2.1/sinp_organisms/serializers.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/tests.py` & `dj_sinp_organisms-1.2.1/sinp_organisms/tests.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/sinp_organisms/views.py` & `dj_sinp_organisms-1.2.1/sinp_organisms/views.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.2.0/PKG-INFO` & `dj_sinp_organisms-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dj_sinp_organisms
-Version: 1.2.0
+Version: 1.2.1
 Summary: Django app to manage french SINP organisms standard
 Home-page: https://github.com/dbchiro/DjangoSinpOrganisms
 License: AGPLv3
 Keywords: SINP,Nomenclatures,Django,France,dbChiroWeb
 Author: dbChiro project
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Django (>=3.2)
-Requires-Dist: dj-sinp-nomenclatures (>=1.0.0,<2.0.0)
+Requires-Dist: dj-sinp-nomenclatures (>=0.0.0)
 Requires-Dist: djangorestframework (>=3,<4)
 Project-URL: Documentation, https://dbchiro.github.io/DjangoSinpOrganisms/
 Project-URL: Repository, https://github.com/dbchiro/DjangoSinpOrganisms
 Description-Content-Type: text/markdown
 
 # SINP Organisms for Django
 
@@ -62,7 +62,11 @@
 ```
 
 4. Run `python manage.py migrate` to create the polls models.
 5. Start the development server and visit <http://127.0.0.1:8000/admin/>
    to create an organism (you'll need the Admin app enabled).
 6. Visit <http://127.0.0.1:8000/api/v1/organisms> to view organisms API.
 
+## Database models
+
+![models.png](./docs/_static/models.png)
+
```

