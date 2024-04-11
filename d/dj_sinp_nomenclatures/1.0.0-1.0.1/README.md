# Comparing `tmp/dj_sinp_nomenclatures-1.0.0.tar.gz` & `tmp/dj_sinp_nomenclatures-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_sinp_nomenclatures-1.0.0.tar", max compression
+gzip compressed data, was "dj_sinp_nomenclatures-1.0.1.tar", max compression
```

## Comparing `dj_sinp_nomenclatures-1.0.0.tar` & `dj_sinp_nomenclatures-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    34523 2024-04-04 07:51:10.248191 dj_sinp_nomenclatures-1.0.0/LICENSE
--rw-r--r--   0        0        0      125 2024-04-04 07:51:10.248191 dj_sinp_nomenclatures-1.0.0/README.rst
--rw-r--r--   0        0        0     1997 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/__init__.py
--rw-r--r--   0        0        0     1201 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/admin.py
--rw-r--r--   0        0        0      259 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/apps.py
--rw-r--r--   0        0        0        0 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/fixtures/.gitkeep
--rw-r--r--   0        0        0    53118 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/fixtures/old_sinp_nomenclatures.json
--rw-r--r--   0        0        0   138267 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/fixtures/sinp_dict_data_v1.0.json
--rw-r--r--   0        0        0     2592 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      696 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/manager.py
--rw-r--r--   0        0        0     8571 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0001_initial.py
--rw-r--r--   0        0        0      353 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0002_alter_source_unique_together.py
--rw-r--r--   0        0        0      454 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0003_rename_item_nomenclature.py
--rw-r--r--   0        0        0     3314 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0004_alter_source_options_alter_type_options_and_more.py
--rw-r--r--   0        0        0     1340 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0005_remove_nomenclature_created_by_and_more.py
--rw-r--r--   0        0        0      727 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0006_alter_source_options_source_url.py
--rw-r--r--   0        0        0      360 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0007_remove_nomenclature_mnemonic.py
--rw-r--r--   0        0        0      708 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0008_alter_nomenclature_active_and_more.py
--rw-r--r--   0        0        0        0 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/__init__.py
--rw-r--r--   0        0        0     3727 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/models.py
--rw-r--r--   0        0        0        0 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/permissions.py
--rw-r--r--   0        0        0      981 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/serializers.py
--rw-r--r--   0        0        0     3075 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/tests.py
--rw-r--r--   0        0        0      499 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/urls.py
--rw-r--r--   0        0        0     1755 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/views.py
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 dj_sinp_nomenclatures-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-11 07:41:48.254150 dj_sinp_nomenclatures-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1359 2024-04-11 07:41:48.254150 dj_sinp_nomenclatures-1.0.1/README.md
+-rw-r--r--   0        0        0     2091 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/__init__.py
+-rw-r--r--   0        0        0     1201 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/admin.py
+-rw-r--r--   0        0        0      259 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/apps.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/fixtures/.gitkeep
+-rw-r--r--   0        0        0    53118 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/fixtures/old_sinp_nomenclatures.json
+-rw-r--r--   0        0        0   138267 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/fixtures/sinp_dict_data_v1.0.json
+-rw-r--r--   0        0        0     2592 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      696 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/manager.py
+-rw-r--r--   0        0        0     8571 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/0001_initial.py
+-rw-r--r--   0        0        0      353 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/0002_alter_source_unique_together.py
+-rw-r--r--   0        0        0      454 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/0003_rename_item_nomenclature.py
+-rw-r--r--   0        0        0     3314 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/0004_alter_source_options_alter_type_options_and_more.py
+-rw-r--r--   0        0        0     1340 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/0005_remove_nomenclature_created_by_and_more.py
+-rw-r--r--   0        0        0      727 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/0006_alter_source_options_source_url.py
+-rw-r--r--   0        0        0      360 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/0007_remove_nomenclature_mnemonic.py
+-rw-r--r--   0        0        0      708 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/0008_alter_nomenclature_active_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/__init__.py
+-rw-r--r--   0        0        0     3727 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/models.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/permissions.py
+-rw-r--r--   0        0        0      981 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/serializers.py
+-rw-r--r--   0        0        0     6024 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/tests.py
+-rw-r--r--   0        0        0      499 2024-04-11 07:41:48.258150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/urls.py
+-rw-r--r--   0        0        0     1755 2024-04-11 07:41:48.262150 dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/views.py
+-rw-r--r--   0        0        0     2331 1970-01-01 00:00:00.000000 dj_sinp_nomenclatures-1.0.1/PKG-INFO
```

### Comparing `dj_sinp_nomenclatures-1.0.0/LICENSE` & `dj_sinp_nomenclatures-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-1.0.0/pyproject.toml` & `dj_sinp_nomenclatures-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 [tool.poetry]
 name = "dj_sinp_nomenclatures"
-version = "1.0.0"
+version = "1.0.1"
 description = "Django app to manage french SINP nomenclatures standards"
 authors = ["dbChiro project <project@dbchiro.org>"]
 license = "AGPLv3"
 keywords = ["SINP", "Nomenclatures", "Django", "France", "dbChiroWeb"]
-readme = "README.rst"
+readme = "README.md"
 homepage = "https://github.com/dbchiro/DjangoSinpNomenclature"
 repository = "https://github.com/dbchiro/DjangoSinpNomenclature"
+documentation = "https://dbchiro.github.io/DjangoSinpNomenclature/"
 include = ["LICENSE"]
 packages = [{ include = "sinp_nomenclatures" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 Django = ">=3.2,<5.0"
 djangorestframework = ">=3.0,<4.0"
-django-filter = "^23.5"
+django-filter = ">=23.5,<25.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.12.1"
 isort = "^5.13.2"
 flake8 = "^6.1.0"
 flake8-isort = "^6.1.1"
 pre-commit = "^3.4.0"
 python-decouple = "^3.8"
 psycopg2-binary = "^2.9.9"
 drf-yasg = "^1.21.7"
 django-fixture-magic = "^0.1.5"
 pygraphviz = "^1.11"
-django-extensions = "^3.2.1"
 flake8-pyproject = "^1.2.3"
 pylint = "^3.0.3"
 pylint-django = "^2.5.5"
 dj-database-url = "^2.1.0"
 bpython = "^0.24"
+coverage = "^7.4.4"
+django-extensions = "^3.2.3"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^6"
 sphinx-rtd-theme = "^2.0.0"
 rstcheck = "^6.2.0"
 myst-parser = "^2.0.0"
```

### Comparing `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/admin.py` & `dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/admin.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/fixtures/old_sinp_nomenclatures.json` & `dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/fixtures/old_sinp_nomenclatures.json`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/fixtures/sinp_dict_data_v1.0.json` & `dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/fixtures/sinp_dict_data_v1.0.json`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/locale/fr/LC_MESSAGES/django.po` & `dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/manager.py` & `dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/manager.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0001_initial.py` & `dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0004_alter_source_options_alter_type_options_and_more.py` & `dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/0004_alter_source_options_alter_type_options_and_more.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0005_remove_nomenclature_created_by_and_more.py` & `dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/0005_remove_nomenclature_created_by_and_more.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0006_alter_source_options_source_url.py` & `dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/0006_alter_source_options_source_url.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0008_alter_nomenclature_active_and_more.py` & `dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/migrations/0008_alter_nomenclature_active_and_more.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/models.py` & `dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/models.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/serializers.py` & `dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/serializers.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/views.py` & `dj_sinp_nomenclatures-1.0.1/sinp_nomenclatures/views.py`

 * *Files identical despite different names*

