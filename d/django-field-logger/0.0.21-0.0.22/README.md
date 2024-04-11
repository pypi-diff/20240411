# Comparing `tmp/django-field-logger-0.0.21.tar.gz` & `tmp/django-field-logger-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-field-logger-0.0.21.tar", last modified: Thu Apr 11 07:44:41 2024, max compression
+gzip compressed data, was "django-field-logger-0.0.22.tar", last modified: Thu Apr 11 08:08:46 2024, max compression
```

## Comparing `django-field-logger-0.0.21.tar` & `django-field-logger-0.0.22.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 07:44:41.495496 django-field-logger-0.0.21/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django-field-logger-0.0.21/LICENSE
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django-field-logger-0.0.21/MANIFEST.in
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      453 2024-04-11 07:44:41.485496 django-field-logger-0.0.21/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     7142 2024-04-05 20:27:31.000000 django-field-logger-0.0.21/README.md
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 07:44:41.485496 django-field-logger-0.0.21/django_field_logger.egg-info/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      453 2024-04-11 07:44:41.000000 django-field-logger-0.0.21/django_field_logger.egg-info/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      519 2024-04-11 07:44:41.000000 django-field-logger-0.0.21/django_field_logger.egg-info/SOURCES.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-04-11 07:44:41.000000 django-field-logger-0.0.21/django_field_logger.egg-info/dependency_links.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-11 07:44:41.000000 django-field-logger-0.0.21/django_field_logger.egg-info/requires.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       18 2024-04-11 07:44:41.000000 django-field-logger-0.0.21/django_field_logger.egg-info/top_level.txt
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 07:44:41.485496 django-field-logger-0.0.21/fieldlogger/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-01-16 20:05:29.000000 django-field-logger-0.0.21/fieldlogger/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-01-16 20:51:47.000000 django-field-logger-0.0.21/fieldlogger/apps.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3135 2024-04-08 14:39:49.000000 django-field-logger-0.0.21/fieldlogger/config.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      862 2024-04-01 09:39:30.000000 django-field-logger-0.0.21/fieldlogger/fieldlogger.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      350 2024-01-17 04:38:48.000000 django-field-logger-0.0.21/fieldlogger/mixins.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2621 2024-04-11 07:22:36.000000 django-field-logger-0.0.21/fieldlogger/models.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1563 2024-04-08 14:41:10.000000 django-field-logger-0.0.21/fieldlogger/signals.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      296 2024-03-27 00:36:10.000000 django-field-logger-0.0.21/fieldlogger/utils.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      415 2024-04-01 09:32:10.000000 django-field-logger-0.0.21/pyproject.toml
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       38 2024-04-11 07:44:41.495496 django-field-logger-0.0.21/setup.cfg
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      763 2024-04-11 07:40:41.000000 django-field-logger-0.0.21/setup.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 07:44:41.485496 django-field-logger-0.0.21/tests/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-03-27 02:22:33.000000 django-field-logger-0.0.21/tests/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2913 2024-04-11 07:12:55.000000 django-field-logger-0.0.21/tests/settings.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3943 2024-04-11 07:23:31.000000 django-field-logger-0.0.21/tests/test_utils.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1788 2024-04-11 07:26:07.000000 django-field-logger-0.0.21/tests/tests.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 08:08:46.685277 django-field-logger-0.0.22/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django-field-logger-0.0.22/LICENSE
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django-field-logger-0.0.22/MANIFEST.in
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     8781 2024-04-11 08:08:46.685277 django-field-logger-0.0.22/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     7142 2024-04-05 20:27:31.000000 django-field-logger-0.0.22/README.md
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 08:08:46.685277 django-field-logger-0.0.22/django_field_logger.egg-info/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     8781 2024-04-11 08:08:46.000000 django-field-logger-0.0.22/django_field_logger.egg-info/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      529 2024-04-11 08:08:46.000000 django-field-logger-0.0.22/django_field_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-04-11 08:08:46.000000 django-field-logger-0.0.22/django_field_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-11 08:08:46.000000 django-field-logger-0.0.22/django_field_logger.egg-info/requires.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-11 08:08:46.000000 django-field-logger-0.0.22/django_field_logger.egg-info/top_level.txt
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 08:08:46.685277 django-field-logger-0.0.22/fieldlogger/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-01-16 20:05:29.000000 django-field-logger-0.0.22/fieldlogger/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-01-16 20:51:47.000000 django-field-logger-0.0.22/fieldlogger/apps.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3135 2024-04-08 14:39:49.000000 django-field-logger-0.0.22/fieldlogger/config.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      862 2024-04-01 09:39:30.000000 django-field-logger-0.0.22/fieldlogger/fieldlogger.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      350 2024-01-17 04:38:48.000000 django-field-logger-0.0.22/fieldlogger/mixins.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2621 2024-04-11 07:22:36.000000 django-field-logger-0.0.22/fieldlogger/models.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1563 2024-04-08 14:41:10.000000 django-field-logger-0.0.22/fieldlogger/signals.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      296 2024-03-27 00:36:10.000000 django-field-logger-0.0.22/fieldlogger/utils.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      415 2024-04-01 09:32:10.000000 django-field-logger-0.0.22/pyproject.toml
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      715 2024-04-11 08:08:46.685277 django-field-logger-0.0.22/setup.cfg
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       96 2024-04-11 08:00:46.000000 django-field-logger-0.0.22/setup.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 08:08:46.685277 django-field-logger-0.0.22/tests/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-03-27 02:22:33.000000 django-field-logger-0.0.22/tests/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2913 2024-04-11 07:12:55.000000 django-field-logger-0.0.22/tests/settings.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3943 2024-04-11 07:23:31.000000 django-field-logger-0.0.22/tests/test_utils.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1788 2024-04-11 07:26:07.000000 django-field-logger-0.0.22/tests/tests.py
```

### Comparing `django-field-logger-0.0.21/LICENSE` & `django-field-logger-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.21/README.md` & `django-field-logger-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.21/django_field_logger.egg-info/SOURCES.txt` & `django-field-logger-0.0.22/django_field_logger.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+setup.cfg
 setup.py
 django_field_logger.egg-info/PKG-INFO
 django_field_logger.egg-info/SOURCES.txt
 django_field_logger.egg-info/dependency_links.txt
 django_field_logger.egg-info/requires.txt
 django_field_logger.egg-info/top_level.txt
 fieldlogger/__init__.py
```

### Comparing `django-field-logger-0.0.21/fieldlogger/config.py` & `django-field-logger-0.0.22/fieldlogger/config.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.21/fieldlogger/fieldlogger.py` & `django-field-logger-0.0.22/fieldlogger/fieldlogger.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.21/fieldlogger/models.py` & `django-field-logger-0.0.22/fieldlogger/models.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.21/fieldlogger/signals.py` & `django-field-logger-0.0.22/fieldlogger/signals.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.21/tests/settings.py` & `django-field-logger-0.0.22/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.21/tests/test_utils.py` & `django-field-logger-0.0.22/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.21/tests/tests.py` & `django-field-logger-0.0.22/tests/tests.py`

 * *Files identical despite different names*

