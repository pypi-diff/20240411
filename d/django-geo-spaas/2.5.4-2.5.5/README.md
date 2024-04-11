# Comparing `tmp/django-geo-spaas-2.5.4.tar.gz` & `tmp/django-geo-spaas-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-geo-spaas-2.5.4.tar", last modified: Wed Apr 10 11:48:38 2024, max compression
+gzip compressed data, was "django-geo-spaas-2.5.5.tar", last modified: Thu Apr 11 12:55:02 2024, max compression
```

## Comparing `django-geo-spaas-2.5.4.tar` & `django-geo-spaas-2.5.5.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.863747 django-geo-spaas-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-10 11:48:38.863747 django-geo-spaas-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.851747 django-geo-spaas-2.5.4/django_geo_spaas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-10 11:48:38.000000 django-geo-spaas-2.5.4/django_geo_spaas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-10 11:48:38.000000 django-geo-spaas-2.5.4/django_geo_spaas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:48:38.000000 django-geo-spaas-2.5.4/django_geo_spaas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:48:38.000000 django-geo-spaas-2.5.4/django_geo_spaas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-10 11:48:38.000000 django-geo-spaas-2.5.4/django_geo_spaas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 11:48:38.000000 django-geo-spaas-2.5.4/django_geo_spaas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.851747 django-geo-spaas-2.5.4/geospaas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.851747 django-geo-spaas-2.5.4/geospaas/base_viewer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/base_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/base_viewer/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/base_viewer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.847747 django-geo-spaas-2.5.4/geospaas/base_viewer/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.851747 django-geo-spaas-2.5.4/geospaas/base_viewer/static/base_viewer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.855747 django-geo-spaas-2.5.4/geospaas/base_viewer/static/base_viewer/js/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/base_viewer/static/base_viewer/js/base_viewer.js
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/base_viewer/static/base_viewer/js/leaflet.ajax.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/base_viewer/static/base_viewer/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.847747 django-geo-spaas-2.5.4/geospaas/base_viewer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.855747 django-geo-spaas-2.5.4/geospaas/base_viewer/templates/base_viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/base_viewer/templates/base_viewer/ds_info.html
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/base_viewer/templates/base_viewer/elements.html
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/base_viewer/templates/base_viewer/page_structure.html
--rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/base_viewer/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/base_viewer/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/base_viewer/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.855747 django-geo-spaas-2.5.4/geospaas/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.855747 django-geo-spaas-2.5.4/geospaas/catalog/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.855747 django-geo-spaas-2.5.4/geospaas/catalog/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/management/commands/count.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.855747 django-geo-spaas-2.5.4/geospaas/catalog/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/migrations/0002_auto_20160705_1331.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/migrations/0003_dataset_entry_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/migrations/0004_populate_entry_id_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/migrations/0005_remove_entry_id_null.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/migrations/0006_auto_20190130_1442.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/migrations/0007_auto_20190626_1313.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/migrations/0008_auto_20200331_0806.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/migrations/0009_auto_20201012_0905.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/migrations/0010_auto_20201019_1331.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/migrations/0011_auto_20210525_1252.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14836 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/catalog/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.859747 django-geo-spaas-2.5.4/geospaas/export_DIF/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/export_DIF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/export_DIF/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.859747 django-geo-spaas-2.5.4/geospaas/export_DIF/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/export_DIF/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/export_DIF/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/export_DIF/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/export_DIF/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.859747 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.859747 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.859747 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/management/commands/ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/management/commands/ingest_hyrax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/management/commands/ingest_thredds_crawl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.859747 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    19850 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/nansat_ingestor/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.859747 django-geo-spaas-2.5.4/geospaas/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/utils/processing_base_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.859747 django-geo-spaas-2.5.4/geospaas/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.859747 django-geo-spaas-2.5.4/geospaas/vocabularies/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.859747 django-geo-spaas-2.5.4/geospaas/vocabularies/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/management/commands/update_vocabularies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.863747 django-geo-spaas-2.5.4/geospaas/vocabularies/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/migrations/0002_auto_20190101_1128.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/migrations/0003_auto_20190829_0847.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/migrations/0004_auto_20200331_0806.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/migrations/0005_auto_20210528_1139.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    22836 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/geospaas/vocabularies/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:48:38.863747 django-geo-spaas-2.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:38.863747 django-geo-spaas-2.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-10 11:48:37.000000 django-geo-spaas-2.5.4/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.911755 django-geo-spaas-2.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-11 12:55:02.911755 django-geo-spaas-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.899755 django-geo-spaas-2.5.5/django_geo_spaas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-11 12:55:02.000000 django-geo-spaas-2.5.5/django_geo_spaas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-11 12:55:02.000000 django-geo-spaas-2.5.5/django_geo_spaas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:55:02.000000 django-geo-spaas-2.5.5/django_geo_spaas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:55:02.000000 django-geo-spaas-2.5.5/django_geo_spaas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-11 12:55:02.000000 django-geo-spaas-2.5.5/django_geo_spaas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 12:55:02.000000 django-geo-spaas-2.5.5/django_geo_spaas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.903755 django-geo-spaas-2.5.5/geospaas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.903755 django-geo-spaas-2.5.5/geospaas/base_viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/base_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/base_viewer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/base_viewer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.899755 django-geo-spaas-2.5.5/geospaas/base_viewer/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.903755 django-geo-spaas-2.5.5/geospaas/base_viewer/static/base_viewer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.903755 django-geo-spaas-2.5.5/geospaas/base_viewer/static/base_viewer/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/base_viewer/static/base_viewer/js/base_viewer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/base_viewer/static/base_viewer/js/leaflet.ajax.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/base_viewer/static/base_viewer/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.899755 django-geo-spaas-2.5.5/geospaas/base_viewer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.903755 django-geo-spaas-2.5.5/geospaas/base_viewer/templates/base_viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/base_viewer/templates/base_viewer/ds_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/base_viewer/templates/base_viewer/elements.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/base_viewer/templates/base_viewer/page_structure.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/base_viewer/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/base_viewer/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/base_viewer/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.903755 django-geo-spaas-2.5.5/geospaas/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.903755 django-geo-spaas-2.5.5/geospaas/catalog/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.903755 django-geo-spaas-2.5.5/geospaas/catalog/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/management/commands/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.907755 django-geo-spaas-2.5.5/geospaas/catalog/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/migrations/0002_auto_20160705_1331.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/migrations/0003_dataset_entry_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/migrations/0004_populate_entry_id_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/migrations/0005_remove_entry_id_null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/migrations/0006_auto_20190130_1442.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/migrations/0007_auto_20190626_1313.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/migrations/0008_auto_20200331_0806.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/migrations/0009_auto_20201012_0905.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/migrations/0010_auto_20201019_1331.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/migrations/0011_auto_20210525_1252.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14836 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/catalog/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.907755 django-geo-spaas-2.5.5/geospaas/export_DIF/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/export_DIF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/export_DIF/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.907755 django-geo-spaas-2.5.5/geospaas/export_DIF/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/export_DIF/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/export_DIF/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/export_DIF/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/export_DIF/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.907755 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.907755 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.907755 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/management/commands/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/management/commands/ingest_hyrax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/management/commands/ingest_thredds_crawl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.907755 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19850 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/nansat_ingestor/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.907755 django-geo-spaas-2.5.5/geospaas/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/utils/processing_base_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.911755 django-geo-spaas-2.5.5/geospaas/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.911755 django-geo-spaas-2.5.5/geospaas/vocabularies/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.911755 django-geo-spaas-2.5.5/geospaas/vocabularies/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/management/commands/update_vocabularies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.911755 django-geo-spaas-2.5.5/geospaas/vocabularies/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/migrations/0002_auto_20190101_1128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/migrations/0003_auto_20190829_0847.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/migrations/0004_auto_20200331_0806.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/migrations/0005_auto_20210528_1139.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22836 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/geospaas/vocabularies/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:55:02.911755 django-geo-spaas-2.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:02.911755 django-geo-spaas-2.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 12:55:01.000000 django-geo-spaas-2.5.5/tests/urls.py
```

### Comparing `django-geo-spaas-2.5.4/LICENSE` & `django-geo-spaas-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/PKG-INFO` & `django-geo-spaas-2.5.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-geo-spaas
-Version: 2.5.4
+Version: 2.5.5
 Summary: Geo-Scientific Platform as a Service
 Home-page: https://github.com/nansencenter/django-geo-spaas
 Download-URL: https://github.com/nansencenter/django-geo-spaas/archive/master.zip
 Author: Morten W. Hansen, Anton Korosov, Artem Moiseev, Jeong-Won Park, Adrien Perrin, A.Azamifard
 Author-email: anton.korosov@nersc.no
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-geo-spaas-2.5.4/README.md` & `django-geo-spaas-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/django_geo_spaas.egg-info/PKG-INFO` & `django-geo-spaas-2.5.5/django_geo_spaas.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-geo-spaas
-Version: 2.5.4
+Version: 2.5.5
 Summary: Geo-Scientific Platform as a Service
 Home-page: https://github.com/nansencenter/django-geo-spaas
 Download-URL: https://github.com/nansencenter/django-geo-spaas/archive/master.zip
 Author: Morten W. Hansen, Anton Korosov, Artem Moiseev, Jeong-Won Park, Adrien Perrin, A.Azamifard
 Author-email: anton.korosov@nersc.no
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-geo-spaas-2.5.4/django_geo_spaas.egg-info/SOURCES.txt` & `django-geo-spaas-2.5.5/django_geo_spaas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/base_viewer/forms.py` & `django-geo-spaas-2.5.5/geospaas/base_viewer/forms.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/base_viewer/static/base_viewer/js/base_viewer.js` & `django-geo-spaas-2.5.5/geospaas/base_viewer/static/base_viewer/js/base_viewer.js`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/base_viewer/static/base_viewer/js/leaflet.ajax.min.js` & `django-geo-spaas-2.5.5/geospaas/base_viewer/static/base_viewer/js/leaflet.ajax.min.js`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/base_viewer/static/base_viewer/styles.css` & `django-geo-spaas-2.5.5/geospaas/base_viewer/static/base_viewer/styles.css`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/base_viewer/templates/base_viewer/ds_info.html` & `django-geo-spaas-2.5.5/geospaas/base_viewer/templates/base_viewer/ds_info.html`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/base_viewer/templates/base_viewer/elements.html` & `django-geo-spaas-2.5.5/geospaas/base_viewer/templates/base_viewer/elements.html`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/base_viewer/templates/base_viewer/page_structure.html` & `django-geo-spaas-2.5.5/geospaas/base_viewer/templates/base_viewer/page_structure.html`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/base_viewer/tests.py` & `django-geo-spaas-2.5.5/geospaas/base_viewer/tests.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/base_viewer/views.py` & `django-geo-spaas-2.5.5/geospaas/base_viewer/views.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/admin.py` & `django-geo-spaas-2.5.5/geospaas/catalog/admin.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/managers.py` & `django-geo-spaas-2.5.5/geospaas/catalog/managers.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/migrations/0001_initial.py` & `django-geo-spaas-2.5.5/geospaas/catalog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/migrations/0002_auto_20160705_1331.py` & `django-geo-spaas-2.5.5/geospaas/catalog/migrations/0002_auto_20160705_1331.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/migrations/0003_dataset_entry_id.py` & `django-geo-spaas-2.5.5/geospaas/catalog/migrations/0003_dataset_entry_id.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/migrations/0004_populate_entry_id_values.py` & `django-geo-spaas-2.5.5/geospaas/catalog/migrations/0004_populate_entry_id_values.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/migrations/0005_remove_entry_id_null.py` & `django-geo-spaas-2.5.5/geospaas/catalog/migrations/0005_remove_entry_id_null.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/migrations/0006_auto_20190130_1442.py` & `django-geo-spaas-2.5.5/geospaas/catalog/migrations/0006_auto_20190130_1442.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/migrations/0007_auto_20190626_1313.py` & `django-geo-spaas-2.5.5/geospaas/catalog/migrations/0007_auto_20190626_1313.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/migrations/0008_auto_20200331_0806.py` & `django-geo-spaas-2.5.5/geospaas/catalog/migrations/0008_auto_20200331_0806.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/migrations/0009_auto_20201012_0905.py` & `django-geo-spaas-2.5.5/geospaas/catalog/migrations/0009_auto_20201012_0905.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/migrations/0010_auto_20201019_1331.py` & `django-geo-spaas-2.5.5/geospaas/catalog/migrations/0010_auto_20201019_1331.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/migrations/0011_auto_20210525_1252.py` & `django-geo-spaas-2.5.5/geospaas/catalog/migrations/0011_auto_20210525_1252.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/models.py` & `django-geo-spaas-2.5.5/geospaas/catalog/models.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/catalog/tests.py` & `django-geo-spaas-2.5.5/geospaas/catalog/tests.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/nansat_ingestor/management/commands/ingest.py` & `django-geo-spaas-2.5.5/geospaas/nansat_ingestor/management/commands/ingest.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/nansat_ingestor/management/commands/ingest_hyrax.py` & `django-geo-spaas-2.5.5/geospaas/nansat_ingestor/management/commands/ingest_hyrax.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/nansat_ingestor/management/commands/ingest_thredds_crawl.py` & `django-geo-spaas-2.5.5/geospaas/nansat_ingestor/management/commands/ingest_thredds_crawl.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/nansat_ingestor/managers.py` & `django-geo-spaas-2.5.5/geospaas/nansat_ingestor/managers.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/nansat_ingestor/migrations/0001_initial.py` & `django-geo-spaas-2.5.5/geospaas/nansat_ingestor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/nansat_ingestor/tests.py` & `django-geo-spaas-2.5.5/geospaas/nansat_ingestor/tests.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/tests.py` & `django-geo-spaas-2.5.5/geospaas/tests.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/utils/processing_base_command.py` & `django-geo-spaas-2.5.5/geospaas/utils/processing_base_command.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/utils/utils.py` & `django-geo-spaas-2.5.5/geospaas/utils/utils.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/vocabularies/management/commands/update_vocabularies.py` & `django-geo-spaas-2.5.5/geospaas/vocabularies/management/commands/update_vocabularies.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/vocabularies/managers.py` & `django-geo-spaas-2.5.5/geospaas/vocabularies/managers.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/vocabularies/migrations/0001_initial.py` & `django-geo-spaas-2.5.5/geospaas/vocabularies/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/vocabularies/migrations/0002_auto_20190101_1128.py` & `django-geo-spaas-2.5.5/geospaas/vocabularies/migrations/0002_auto_20190101_1128.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/vocabularies/migrations/0004_auto_20200331_0806.py` & `django-geo-spaas-2.5.5/geospaas/vocabularies/migrations/0004_auto_20200331_0806.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/vocabularies/models.py` & `django-geo-spaas-2.5.5/geospaas/vocabularies/models.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/geospaas/vocabularies/tests.py` & `django-geo-spaas-2.5.5/geospaas/vocabularies/tests.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/setup.py` & `django-geo-spaas-2.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.4/tests/settings.py` & `django-geo-spaas-2.5.5/tests/settings.py`

 * *Files identical despite different names*

