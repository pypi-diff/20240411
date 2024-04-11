# Comparing `tmp/django-customvueadmin-0.1.2.tar.gz` & `tmp/django-customvueadmin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-customvueadmin-0.1.2.tar", last modified: Thu Apr 11 11:49:02 2024, max compression
+gzip compressed data, was "django-customvueadmin-0.1.3.tar", last modified: Thu Apr 11 12:29:49 2024, max compression
```

## Comparing `django-customvueadmin-0.1.2.tar` & `django-customvueadmin-0.1.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.844744 django-customvueadmin-0.1.2/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2852 2024-04-11 11:49:02.844744 django-customvueadmin-0.1.2/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2002 2024-04-11 11:45:03.000000 django-customvueadmin-0.1.2/README.rst
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-04-11 11:48:45.000000 django-customvueadmin-0.1.2/custom_admin/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/api/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/api/actions/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/actions/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      738 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/actions/delete_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2466 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/actions/export_csv_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2161 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/actions/view_actions_mixin.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/api/fields/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      370 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/base.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      706 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/char.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1091 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/choice.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3057 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/files.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/int.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/numbers.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/relation.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/api/filters/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      114 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/filters/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1558 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/filters/base_admin_filter.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/filters/choices.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/api/inlines/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/export_csv_inline.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1627 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/inline_graph.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/inline_table.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/inlines_type.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/interfaces.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/view_inline_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/permissions.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/api/serializers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/serializers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5559 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/serializers/base_serializer.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      761 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/urls.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/api/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      509 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1984 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/admin_log.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5735 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/autocomplete.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9283 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/base_admin_viewset.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      588 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/change_language.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      748 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/get_sections.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3440 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/token_auth.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      983 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/viewset_info.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/controllers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-03-23 13:11:18.000000 django-customvueadmin-0.1.2/custom_admin/controllers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3505 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/controllers/admin_log_manager.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3909 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/controllers/custom_metadata.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2911 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/controllers/filters_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8985 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/controllers/schema_generator.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/migrations/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1790 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/migrations/0001_initial.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1006 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/migrations/0002_auto_20220826_1734.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      751 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/migrations/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/models/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/models/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/models/admin_log.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/tests/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/tests/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      581 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/tests/test_language.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      460 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/tests/test_scheme_get.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/utils/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/utils/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.2/custom_admin/utils/colors.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/utils/get_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/utils/register_admin_viewsets.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1314 2024-04-11 11:48:23.000000 django-customvueadmin-0.1.2/custom_admin/views/admin_page.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2989 2024-04-11 11:20:38.000000 django-customvueadmin-0.1.2/custom_admin/views/template.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2852 2024-04-11 11:49:02.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2528 2024-04-11 11:49:02.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/SOURCES.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 11:49:02.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/dependency_links.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       82 2024-04-11 11:49:02.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/entry_points.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 09:29:05.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/not-zip-safe
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-11 11:49:02.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/requires.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-04-11 11:49:02.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/top_level.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django-customvueadmin-0.1.2/pyproject.toml
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1100 2024-04-11 11:49:02.844744 django-customvueadmin-0.1.2/setup.cfg
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.948840 django-customvueadmin-0.1.3/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2846 2024-04-11 12:29:49.948840 django-customvueadmin-0.1.3/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1996 2024-04-11 11:50:25.000000 django-customvueadmin-0.1.3/README.rst
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.942172 django-customvueadmin-0.1.3/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-04-11 12:29:43.000000 django-customvueadmin-0.1.3/custom_admin/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.945506 django-customvueadmin-0.1.3/custom_admin/api/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.945506 django-customvueadmin-0.1.3/custom_admin/api/actions/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/actions/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      738 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/actions/delete_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2466 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/actions/export_csv_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2161 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/actions/view_actions_mixin.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.945506 django-customvueadmin-0.1.3/custom_admin/api/fields/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      370 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/fields/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/fields/base.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      706 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/fields/char.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1091 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/fields/choice.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3057 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/fields/files.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/fields/int.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/fields/numbers.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/fields/relation.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.945506 django-customvueadmin-0.1.3/custom_admin/api/filters/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      114 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/filters/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1558 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/filters/base_admin_filter.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/filters/choices.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.945506 django-customvueadmin-0.1.3/custom_admin/api/inlines/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/inlines/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/inlines/export_csv_inline.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1627 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.3/custom_admin/api/inlines/inline_graph.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/inlines/inline_table.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django-customvueadmin-0.1.3/custom_admin/api/inlines/inlines_type.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/inlines/interfaces.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django-customvueadmin-0.1.3/custom_admin/api/inlines/view_inline_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/permissions.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.945506 django-customvueadmin-0.1.3/custom_admin/api/serializers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/serializers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5559 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/serializers/base_serializer.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      761 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/urls.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.945506 django-customvueadmin-0.1.3/custom_admin/api/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      509 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1984 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/views/admin_log.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5735 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/views/autocomplete.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9283 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/views/base_admin_viewset.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      588 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/views/change_language.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      748 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/views/get_sections.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3440 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/views/token_auth.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      983 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/api/viewset_info.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.948840 django-customvueadmin-0.1.3/custom_admin/controllers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-03-23 13:11:18.000000 django-customvueadmin-0.1.3/custom_admin/controllers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3505 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/controllers/admin_log_manager.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3909 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/controllers/custom_metadata.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2911 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/controllers/filters_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8985 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/controllers/schema_generator.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.948840 django-customvueadmin-0.1.3/custom_admin/migrations/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1790 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.3/custom_admin/migrations/0001_initial.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1006 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.3/custom_admin/migrations/0002_auto_20220826_1734.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      751 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.3/custom_admin/migrations/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.948840 django-customvueadmin-0.1.3/custom_admin/models/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.3/custom_admin/models/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/models/admin_log.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.948840 django-customvueadmin-0.1.3/custom_admin/tests/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.3/custom_admin/tests/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      581 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.3/custom_admin/tests/test_language.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      460 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.3/custom_admin/tests/test_scheme_get.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.948840 django-customvueadmin-0.1.3/custom_admin/utils/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/utils/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.3/custom_admin/utils/colors.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/utils/get_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/utils/register_admin_viewsets.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.948840 django-customvueadmin-0.1.3/custom_admin/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.3/custom_admin/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1096 2024-04-11 12:29:37.000000 django-customvueadmin-0.1.3/custom_admin/views/admin_page.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2989 2024-04-11 11:20:38.000000 django-customvueadmin-0.1.3/custom_admin/views/template.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 12:29:49.948840 django-customvueadmin-0.1.3/django_customvueadmin.egg-info/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2846 2024-04-11 12:29:49.000000 django-customvueadmin-0.1.3/django_customvueadmin.egg-info/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2528 2024-04-11 12:29:49.000000 django-customvueadmin-0.1.3/django_customvueadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 12:29:49.000000 django-customvueadmin-0.1.3/django_customvueadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       82 2024-04-11 12:29:49.000000 django-customvueadmin-0.1.3/django_customvueadmin.egg-info/entry_points.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 09:29:05.000000 django-customvueadmin-0.1.3/django_customvueadmin.egg-info/not-zip-safe
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-11 12:29:49.000000 django-customvueadmin-0.1.3/django_customvueadmin.egg-info/requires.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-04-11 12:29:49.000000 django-customvueadmin-0.1.3/django_customvueadmin.egg-info/top_level.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django-customvueadmin-0.1.3/pyproject.toml
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1100 2024-04-11 12:29:49.952173 django-customvueadmin-0.1.3/setup.cfg
```

### Comparing `django-customvueadmin-0.1.2/PKG-INFO` & `django-customvueadmin-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.1.2
+Version: 0.1.3
 Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -65,13 +65,13 @@
    npm run build --prefix vue_frontend
    rm -r custom_admin/static/*
    cp vue_frontend/dist/favicon.ico custom_admin/static/favicon.ico
    cp vue_frontend/dist/manifest.json custom_admin/static/manifest.json
    cp -r vue_frontend/dist/tinymce/ custom_admin/static/tinymce/
    cp -r vue_frontend/dist/static/ custom_admin/
 
-.. |logo| image:: https://raw.githubusercontent.com/greyli/flask-share/master/images/demo.png
+.. |logo| image:: https://github.com/Innova-Group-LLC/custom_admin/blob/master/logo.png
    :target: https://innova-group-llc.github.io/custom_admin_docs/
 .. |PyPI version| image:: https://badge.fury.io/py/django-customvueadmin.svg
    :target: https://pypi.org/project/django-customvueadmin/
 .. |GitHub stars| image:: https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin
    :target: https://github.com/Innova-Group-LLC/custom_admin
```

### Comparing `django-customvueadmin-0.1.2/README.rst` & `django-customvueadmin-0.1.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -46,13 +46,13 @@
    npm run build --prefix vue_frontend
    rm -r custom_admin/static/*
    cp vue_frontend/dist/favicon.ico custom_admin/static/favicon.ico
    cp vue_frontend/dist/manifest.json custom_admin/static/manifest.json
    cp -r vue_frontend/dist/tinymce/ custom_admin/static/tinymce/
    cp -r vue_frontend/dist/static/ custom_admin/
 
-.. |logo| image:: https://raw.githubusercontent.com/greyli/flask-share/master/images/demo.png
+.. |logo| image:: https://github.com/Innova-Group-LLC/custom_admin/blob/master/logo.png
    :target: https://innova-group-llc.github.io/custom_admin_docs/
 .. |PyPI version| image:: https://badge.fury.io/py/django-customvueadmin.svg
    :target: https://pypi.org/project/django-customvueadmin/
 .. |GitHub stars| image:: https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin
    :target: https://github.com/Innova-Group-LLC/custom_admin
```

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/actions/delete_action.py` & `django-customvueadmin-0.1.3/custom_admin/api/actions/delete_action.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/actions/export_csv_action.py` & `django-customvueadmin-0.1.3/custom_admin/api/actions/export_csv_action.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/actions/view_actions_mixin.py` & `django-customvueadmin-0.1.3/custom_admin/api/actions/view_actions_mixin.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/fields/char.py` & `django-customvueadmin-0.1.3/custom_admin/api/fields/char.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/fields/choice.py` & `django-customvueadmin-0.1.3/custom_admin/api/fields/choice.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/fields/files.py` & `django-customvueadmin-0.1.3/custom_admin/api/fields/files.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/fields/relation.py` & `django-customvueadmin-0.1.3/custom_admin/api/fields/relation.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/filters/base_admin_filter.py` & `django-customvueadmin-0.1.3/custom_admin/api/filters/base_admin_filter.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/inlines/export_csv_inline.py` & `django-customvueadmin-0.1.3/custom_admin/api/inlines/export_csv_inline.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/inlines/inline_graph.py` & `django-customvueadmin-0.1.3/custom_admin/api/inlines/inline_graph.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/inlines/inline_table.py` & `django-customvueadmin-0.1.3/custom_admin/api/inlines/inline_table.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/inlines/view_inline_mixin.py` & `django-customvueadmin-0.1.3/custom_admin/api/inlines/view_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/permissions.py` & `django-customvueadmin-0.1.3/custom_admin/api/permissions.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/serializers/base_serializer.py` & `django-customvueadmin-0.1.3/custom_admin/api/serializers/base_serializer.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/urls.py` & `django-customvueadmin-0.1.3/custom_admin/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/views/admin_log.py` & `django-customvueadmin-0.1.3/custom_admin/api/views/admin_log.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/views/autocomplete.py` & `django-customvueadmin-0.1.3/custom_admin/api/views/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/views/base_admin_viewset.py` & `django-customvueadmin-0.1.3/custom_admin/api/views/base_admin_viewset.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/views/change_language.py` & `django-customvueadmin-0.1.3/custom_admin/api/views/change_language.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/views/get_sections.py` & `django-customvueadmin-0.1.3/custom_admin/api/views/get_sections.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/views/token_auth.py` & `django-customvueadmin-0.1.3/custom_admin/api/views/token_auth.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/api/viewset_info.py` & `django-customvueadmin-0.1.3/custom_admin/api/viewset_info.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/controllers/admin_log_manager.py` & `django-customvueadmin-0.1.3/custom_admin/controllers/admin_log_manager.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/controllers/custom_metadata.py` & `django-customvueadmin-0.1.3/custom_admin/controllers/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/controllers/filters_schema.py` & `django-customvueadmin-0.1.3/custom_admin/controllers/filters_schema.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/controllers/schema_generator.py` & `django-customvueadmin-0.1.3/custom_admin/controllers/schema_generator.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/migrations/0001_initial.py` & `django-customvueadmin-0.1.3/custom_admin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/migrations/0002_auto_20220826_1734.py` & `django-customvueadmin-0.1.3/custom_admin/migrations/0002_auto_20220826_1734.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py` & `django-customvueadmin-0.1.3/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/models/admin_log.py` & `django-customvueadmin-0.1.3/custom_admin/models/admin_log.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/tests/test_language.py` & `django-customvueadmin-0.1.3/custom_admin/tests/test_language.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/utils/colors.py` & `django-customvueadmin-0.1.3/custom_admin/utils/colors.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/utils/get_schema.py` & `django-customvueadmin-0.1.3/custom_admin/utils/get_schema.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/utils/register_admin_viewsets.py` & `django-customvueadmin-0.1.3/custom_admin/utils/register_admin_viewsets.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/custom_admin/views/admin_page.py` & `django-customvueadmin-0.1.3/custom_admin/views/admin_page.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 import json
 
+from custom_admin.views.template import CUSTOM_ADMIN_TEMPLATE_STRING
 from django.conf import settings
-from django.shortcuts import render
-from django.template.exceptions import TemplateDoesNotExist
+from django.template import Context, Template
 from django.views import View
 
-TEMPLATE_NOT_FOUND = '''
-Custom admin cannot find template "{template}".
-Make sure settings.TEMPLATES contains 'APP_DIRS': True
-'''
-
 
 class CustomAdminView(View):
     '''
     # Settings in case of h2ttps:
     USE_X_FORWARDED_HOST = True
     SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTO', 'https')
     '''
@@ -31,11 +26,9 @@
             admin_settings['backend_prefix'] = request.build_absolute_uri('/custom_admin/')
 
         context = {
             'SETTINGS': admin_settings,
             'SETTINGS_JSON': json.dumps(admin_settings),
         }
 
-        try:
-            return render(request, self.template, context)
-        except TemplateDoesNotExist as e:
-            raise TemplateDoesNotExist(TEMPLATE_NOT_FOUND.format(template=self.template)) from e
+        template = Template(CUSTOM_ADMIN_TEMPLATE_STRING)
+        return template.render(Context(context))
```

### Comparing `django-customvueadmin-0.1.2/custom_admin/views/template.py` & `django-customvueadmin-0.1.3/custom_admin/views/template.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/django_customvueadmin.egg-info/PKG-INFO` & `django-customvueadmin-0.1.3/django_customvueadmin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.1.2
+Version: 0.1.3
 Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -65,13 +65,13 @@
    npm run build --prefix vue_frontend
    rm -r custom_admin/static/*
    cp vue_frontend/dist/favicon.ico custom_admin/static/favicon.ico
    cp vue_frontend/dist/manifest.json custom_admin/static/manifest.json
    cp -r vue_frontend/dist/tinymce/ custom_admin/static/tinymce/
    cp -r vue_frontend/dist/static/ custom_admin/
 
-.. |logo| image:: https://raw.githubusercontent.com/greyli/flask-share/master/images/demo.png
+.. |logo| image:: https://github.com/Innova-Group-LLC/custom_admin/blob/master/logo.png
    :target: https://innova-group-llc.github.io/custom_admin_docs/
 .. |PyPI version| image:: https://badge.fury.io/py/django-customvueadmin.svg
    :target: https://pypi.org/project/django-customvueadmin/
 .. |GitHub stars| image:: https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin
    :target: https://github.com/Innova-Group-LLC/custom_admin
```

### Comparing `django-customvueadmin-0.1.2/django_customvueadmin.egg-info/SOURCES.txt` & `django-customvueadmin-0.1.3/django_customvueadmin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.2/setup.cfg` & `django-customvueadmin-0.1.3/setup.cfg`

 * *Files identical despite different names*

