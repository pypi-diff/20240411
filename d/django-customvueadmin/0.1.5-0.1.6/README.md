# Comparing `tmp/django-customvueadmin-0.1.5.tar.gz` & `tmp/django-customvueadmin-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-customvueadmin-0.1.5.tar", last modified: Thu Apr 11 12:41:27 2024, max compression
+gzip compressed data, was "django-customvueadmin-0.1.6.tar", last modified: Thu Apr 11 14:27:06 2024, max compression
```

## Comparing `django-customvueadmin-0.1.5.tar` & `django-customvueadmin-0.1.6.tar`

### file list

```diff
@@ -1,84 +1,144 @@
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.683707 django-customvueadmin-0.1.5/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2855 2024-04-11 12:41:27.683707 django-customvueadmin-0.1.5/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2005 2024-04-11 12:39:26.000000 django-customvueadmin-0.1.5/README.rst
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.677039 django-customvueadmin-0.1.5/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-04-11 12:41:14.000000 django-customvueadmin-0.1.5/custom_admin/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.677039 django-customvueadmin-0.1.5/custom_admin/api/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.677039 django-customvueadmin-0.1.5/custom_admin/api/actions/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/actions/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      738 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/actions/delete_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2466 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/actions/export_csv_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2161 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/actions/view_actions_mixin.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.677039 django-customvueadmin-0.1.5/custom_admin/api/fields/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      370 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/fields/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/fields/base.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      706 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/fields/char.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1091 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/fields/choice.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3057 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/fields/files.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/fields/int.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/fields/numbers.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/fields/relation.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.677039 django-customvueadmin-0.1.5/custom_admin/api/filters/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      114 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/filters/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1558 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/filters/base_admin_filter.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/filters/choices.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.677039 django-customvueadmin-0.1.5/custom_admin/api/inlines/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/inlines/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/inlines/export_csv_inline.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1627 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.5/custom_admin/api/inlines/inline_graph.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/inlines/inline_table.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django-customvueadmin-0.1.5/custom_admin/api/inlines/inlines_type.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/inlines/interfaces.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django-customvueadmin-0.1.5/custom_admin/api/inlines/view_inline_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/permissions.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.677039 django-customvueadmin-0.1.5/custom_admin/api/serializers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/serializers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5559 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/serializers/base_serializer.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      761 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/urls.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.680373 django-customvueadmin-0.1.5/custom_admin/api/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      509 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1984 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/views/admin_log.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5735 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/views/autocomplete.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9283 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/views/base_admin_viewset.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      588 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/views/change_language.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      748 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/views/get_sections.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3440 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/views/token_auth.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      983 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/api/viewset_info.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.680373 django-customvueadmin-0.1.5/custom_admin/controllers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-03-23 13:11:18.000000 django-customvueadmin-0.1.5/custom_admin/controllers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3505 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/controllers/admin_log_manager.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3909 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/controllers/custom_metadata.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2911 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/controllers/filters_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8985 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/controllers/schema_generator.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.680373 django-customvueadmin-0.1.5/custom_admin/migrations/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1790 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.5/custom_admin/migrations/0001_initial.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1006 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.5/custom_admin/migrations/0002_auto_20220826_1734.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      751 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.5/custom_admin/migrations/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.680373 django-customvueadmin-0.1.5/custom_admin/models/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.5/custom_admin/models/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/models/admin_log.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.680373 django-customvueadmin-0.1.5/custom_admin/tests/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.5/custom_admin/tests/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      581 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.5/custom_admin/tests/test_language.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      460 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.5/custom_admin/tests/test_scheme_get.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.680373 django-customvueadmin-0.1.5/custom_admin/utils/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/utils/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.5/custom_admin/utils/colors.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/utils/get_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/utils/register_admin_viewsets.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.680373 django-customvueadmin-0.1.5/custom_admin/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.5/custom_admin/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1168 2024-04-11 12:41:05.000000 django-customvueadmin-0.1.5/custom_admin/views/admin_page.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2989 2024-04-11 11:20:38.000000 django-customvueadmin-0.1.5/custom_admin/views/template.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:41:27.680373 django-customvueadmin-0.1.5/django_customvueadmin.egg-info/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2855 2024-04-11 12:41:27.000000 django-customvueadmin-0.1.5/django_customvueadmin.egg-info/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2528 2024-04-11 12:41:27.000000 django-customvueadmin-0.1.5/django_customvueadmin.egg-info/SOURCES.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 12:41:27.000000 django-customvueadmin-0.1.5/django_customvueadmin.egg-info/dependency_links.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       82 2024-04-11 12:41:27.000000 django-customvueadmin-0.1.5/django_customvueadmin.egg-info/entry_points.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 12:33:38.000000 django-customvueadmin-0.1.5/django_customvueadmin.egg-info/not-zip-safe
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-11 12:41:27.000000 django-customvueadmin-0.1.5/django_customvueadmin.egg-info/requires.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-04-11 12:41:27.000000 django-customvueadmin-0.1.5/django_customvueadmin.egg-info/top_level.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django-customvueadmin-0.1.5/pyproject.toml
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1100 2024-04-11 12:41:27.683707 django-customvueadmin-0.1.5/setup.cfg
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      209 2024-04-11 14:26:38.000000 django-customvueadmin-0.1.6/MANIFEST.in
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2855 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2005 2024-04-11 12:39:26.000000 django-customvueadmin-0.1.6/README.rst
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-04-11 14:27:03.000000 django-customvueadmin-0.1.6/custom_admin/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/api/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/api/actions/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/actions/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      738 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/actions/delete_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2466 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/actions/export_csv_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2161 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/actions/view_actions_mixin.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/api/fields/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      370 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/base.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      706 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/char.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1091 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/choice.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3057 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/files.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/int.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/numbers.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/relation.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/api/filters/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      114 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/filters/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1558 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/filters/base_admin_filter.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/filters/choices.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/api/inlines/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/export_csv_inline.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1627 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/inline_graph.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/inline_table.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/inlines_type.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/interfaces.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/view_inline_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/permissions.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/api/serializers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/serializers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5559 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/serializers/base_serializer.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      761 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/urls.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/api/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      509 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1984 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/admin_log.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5735 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/autocomplete.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9283 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/base_admin_viewset.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      588 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/change_language.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      748 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/get_sections.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3440 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/token_auth.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      983 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/viewset_info.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/controllers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-03-23 13:11:18.000000 django-customvueadmin-0.1.6/custom_admin/controllers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3505 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/controllers/admin_log_manager.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3909 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/controllers/custom_metadata.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2911 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/controllers/filters_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8985 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/controllers/schema_generator.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/migrations/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1790 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/migrations/0001_initial.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1006 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/migrations/0002_auto_20220826_1734.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      751 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/migrations/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/models/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/models/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/models/admin_log.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/static/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.123462 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    27506 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/app.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      131 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-3ef8a5a8.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4748 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-7402f562.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      762 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-8b69702c.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1632 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-a7c7287a.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       71 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-ecedfa6a.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   233274 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-elementUI.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    10292 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-fdcfea10.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3568 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-libs.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    67646 2024-04-11 09:39:27.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/favicon.ico
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.123462 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/fonts/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    55956 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/fonts/element-icons.ttf
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    28200 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/fonts/element-icons.woff
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.123462 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/img/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    98071 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/img/404.png
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4766 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/img/404_cloud.png
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.126795 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    53669 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/app.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      925 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-2d0c14f9.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    11162 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-2d2080da.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    21542 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-3ef8a5a8.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   122331 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-5148deb9.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   200033 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-6786f71b.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1766 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-7402f562.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    39131 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-8b69702c.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4166 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-a7c7287a.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3542 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-ecedfa6a.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   672429 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-elementUI.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   215439 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-fdcfea10.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   579815 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-libs.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3247 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/runtime.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.126795 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.126795 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-first/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4788 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    50376 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.126795 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-slim/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4730 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    49965 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/img/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    14708 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/img/example.png
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    15764 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/lightgray/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3193 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/lightgray/fonts/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     7664 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    38232 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/accordion.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1251 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/codesample/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1736 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1171290 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/tinymce.min.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/templates/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/templates/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2949 2024-04-11 13:23:28.000000 django-customvueadmin-0.1.6/custom_admin/templates/custom_admin/admin_index.html
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/tests/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/tests/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      581 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/tests/test_language.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      460 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/tests/test_scheme_get.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/utils/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/utils/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.6/custom_admin/utils/colors.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/utils/get_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/utils/register_admin_viewsets.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1314 2024-04-11 13:20:41.000000 django-customvueadmin-0.1.6/custom_admin/views/admin_page.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2855 2024-04-11 14:27:06.000000 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4852 2024-04-11 14:27:06.000000 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 14:27:06.000000 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 14:11:51.000000 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/not-zip-safe
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-11 14:27:06.000000 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/requires.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-04-11 14:27:06.000000 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/top_level.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django-customvueadmin-0.1.6/pyproject.toml
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      992 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/setup.cfg
```

### Comparing `django-customvueadmin-0.1.5/PKG-INFO` & `django-customvueadmin-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.1.5
+Version: 0.1.6
 Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-customvueadmin-0.1.5/README.rst` & `django-customvueadmin-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/actions/delete_action.py` & `django-customvueadmin-0.1.6/custom_admin/api/actions/delete_action.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/actions/export_csv_action.py` & `django-customvueadmin-0.1.6/custom_admin/api/actions/export_csv_action.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/actions/view_actions_mixin.py` & `django-customvueadmin-0.1.6/custom_admin/api/actions/view_actions_mixin.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/fields/char.py` & `django-customvueadmin-0.1.6/custom_admin/api/fields/char.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/fields/choice.py` & `django-customvueadmin-0.1.6/custom_admin/api/fields/choice.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/fields/files.py` & `django-customvueadmin-0.1.6/custom_admin/api/fields/files.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/fields/relation.py` & `django-customvueadmin-0.1.6/custom_admin/api/fields/relation.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/filters/base_admin_filter.py` & `django-customvueadmin-0.1.6/custom_admin/api/filters/base_admin_filter.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/inlines/export_csv_inline.py` & `django-customvueadmin-0.1.6/custom_admin/api/inlines/export_csv_inline.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/inlines/inline_graph.py` & `django-customvueadmin-0.1.6/custom_admin/api/inlines/inline_graph.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/inlines/inline_table.py` & `django-customvueadmin-0.1.6/custom_admin/api/inlines/inline_table.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/inlines/view_inline_mixin.py` & `django-customvueadmin-0.1.6/custom_admin/api/inlines/view_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/permissions.py` & `django-customvueadmin-0.1.6/custom_admin/api/permissions.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/serializers/base_serializer.py` & `django-customvueadmin-0.1.6/custom_admin/api/serializers/base_serializer.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/urls.py` & `django-customvueadmin-0.1.6/custom_admin/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/views/admin_log.py` & `django-customvueadmin-0.1.6/custom_admin/api/views/admin_log.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/views/autocomplete.py` & `django-customvueadmin-0.1.6/custom_admin/api/views/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/views/base_admin_viewset.py` & `django-customvueadmin-0.1.6/custom_admin/api/views/base_admin_viewset.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/views/change_language.py` & `django-customvueadmin-0.1.6/custom_admin/api/views/change_language.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/views/get_sections.py` & `django-customvueadmin-0.1.6/custom_admin/api/views/get_sections.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/views/token_auth.py` & `django-customvueadmin-0.1.6/custom_admin/api/views/token_auth.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/api/viewset_info.py` & `django-customvueadmin-0.1.6/custom_admin/api/viewset_info.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/controllers/admin_log_manager.py` & `django-customvueadmin-0.1.6/custom_admin/controllers/admin_log_manager.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/controllers/custom_metadata.py` & `django-customvueadmin-0.1.6/custom_admin/controllers/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/controllers/filters_schema.py` & `django-customvueadmin-0.1.6/custom_admin/controllers/filters_schema.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/controllers/schema_generator.py` & `django-customvueadmin-0.1.6/custom_admin/controllers/schema_generator.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/migrations/0001_initial.py` & `django-customvueadmin-0.1.6/custom_admin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/migrations/0002_auto_20220826_1734.py` & `django-customvueadmin-0.1.6/custom_admin/migrations/0002_auto_20220826_1734.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py` & `django-customvueadmin-0.1.6/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/models/admin_log.py` & `django-customvueadmin-0.1.6/custom_admin/models/admin_log.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/tests/test_language.py` & `django-customvueadmin-0.1.6/custom_admin/tests/test_language.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/utils/colors.py` & `django-customvueadmin-0.1.6/custom_admin/utils/colors.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/utils/get_schema.py` & `django-customvueadmin-0.1.6/custom_admin/utils/get_schema.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/utils/register_admin_viewsets.py` & `django-customvueadmin-0.1.6/custom_admin/utils/register_admin_viewsets.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.5/custom_admin/views/admin_page.py` & `django-customvueadmin-0.1.6/custom_admin/views/admin_page.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import json
 
-from django.http import HttpResponse
-
-from custom_admin.views.template import CUSTOM_ADMIN_TEMPLATE_STRING
 from django.conf import settings
-from django.template import Context, Template
+from django.shortcuts import render
+from django.template.exceptions import TemplateDoesNotExist
 from django.views import View
 
+TEMPLATE_NOT_FOUND = '''
+Custom admin cannot find template "{template}".
+Make sure settings.TEMPLATES contains 'APP_DIRS': True
+'''
+
 
 class CustomAdminView(View):
     '''
     # Settings in case of h2ttps:
     USE_X_FORWARDED_HOST = True
     SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTO', 'https')
     '''
@@ -28,10 +31,11 @@
             admin_settings['backend_prefix'] = request.build_absolute_uri('/custom_admin/')
 
         context = {
             'SETTINGS': admin_settings,
             'SETTINGS_JSON': json.dumps(admin_settings),
         }
 
-        template = Template(CUSTOM_ADMIN_TEMPLATE_STRING)
-        code = template.render(Context(context))
-        return HttpResponse(code)
+        try:
+            return render(request, self.template, context)
+        except TemplateDoesNotExist as e:
+            raise TemplateDoesNotExist(TEMPLATE_NOT_FOUND.format(template=self.template)) from e
```

### Comparing `django-customvueadmin-0.1.5/custom_admin/views/template.py` & `django-customvueadmin-0.1.6/custom_admin/templates/custom_admin/admin_index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-CUSTOM_ADMIN_TEMPLATE_STRING = '''
 <!DOCTYPE html>
 <html>
     <head>
         <meta charset=utf-8>
         <meta http-equiv=X-UA-Compatible content="IE=edge,chrome=1">
         <meta name=viewport content="width=device-width,initial-scale=1,maximum-scale=1,user-scalable=no">
         <title>{{ SETTINGS.TITLE }}</title>
@@ -47,9 +46,7 @@
         <script src=/static/js/app.js></script>
         <script src=/static/js/runtime.js></script>
         <script src=/static/js/chunk-elementUI.js></script>
         <script src=/static/js/chunk-libs.js></script>
         <script src=/static/js/app.js></script>
     </body>
 </html>
-
-'''
```

#### html2text {}

```diff
@@ -1,4 +1,2 @@
-CUSTOM_ADMIN_TEMPLATE_STRING = '''
 WWee''rree ssoorrrryy bbuutt {{{{ SSEETTTTIINNGGSS..ttiittllee }}}} ddooeessnn''tt wwoorrkk pprrooppeerrllyy wwiitthhoouutt JJaavvaaSSccrriipptt
 eennaabblleedd.. PPlleeaassee eennaabbllee iitt ttoo ccoonnttiinnuuee..
-'''
```

### Comparing `django-customvueadmin-0.1.5/django_customvueadmin.egg-info/PKG-INFO` & `django-customvueadmin-0.1.6/django_customvueadmin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.1.5
+Version: 0.1.6
 Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-customvueadmin-0.1.5/setup.cfg` & `django-customvueadmin-0.1.6/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -17,18 +17,14 @@
 
 [options]
 python_requires = >=3.10
 packages = find:
 include_package_data = true
 zip_safe = false
 
-[options.entry_points]
-console_scripts = 
-	django-admin = django.core.management:execute_from_command_line
-
 [options.extras_require]
 argon2 = argon2-cffi >= 19.1.0
 bcrypt = bcrypt
 
 [flake8]
 exclude = build,.git,.tox,./tests/.env
 extend-ignore = E203
```

