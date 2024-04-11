# Comparing `tmp/django-customvueadmin-0.1.1.tar.gz` & `tmp/django-customvueadmin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-customvueadmin-0.1.1.tar", last modified: Thu Apr 11 11:41:00 2024, max compression
+gzip compressed data, was "django-customvueadmin-0.1.2.tar", last modified: Thu Apr 11 11:49:02 2024, max compression
```

## Comparing `django-customvueadmin-0.1.1.tar` & `django-customvueadmin-0.1.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.301845 django-customvueadmin-0.1.1/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2679 2024-04-11 11:41:00.301845 django-customvueadmin-0.1.1/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1829 2024-04-11 11:40:52.000000 django-customvueadmin-0.1.1/README.md
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.295177 django-customvueadmin-0.1.1/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-04-11 10:58:52.000000 django-customvueadmin-0.1.1/custom_admin/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.295177 django-customvueadmin-0.1.1/custom_admin/api/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.295177 django-customvueadmin-0.1.1/custom_admin/api/actions/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/actions/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      738 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/actions/delete_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2466 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/actions/export_csv_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2161 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/actions/view_actions_mixin.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.295177 django-customvueadmin-0.1.1/custom_admin/api/fields/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      370 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/fields/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/fields/base.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      706 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/fields/char.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1091 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/fields/choice.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3057 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/fields/files.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/fields/int.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/fields/numbers.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/fields/relation.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.295177 django-customvueadmin-0.1.1/custom_admin/api/filters/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      114 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/filters/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1558 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/filters/base_admin_filter.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/filters/choices.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.298511 django-customvueadmin-0.1.1/custom_admin/api/inlines/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/inlines/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/inlines/export_csv_inline.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1627 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.1/custom_admin/api/inlines/inline_graph.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/inlines/inline_table.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django-customvueadmin-0.1.1/custom_admin/api/inlines/inlines_type.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/inlines/interfaces.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django-customvueadmin-0.1.1/custom_admin/api/inlines/view_inline_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/permissions.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.298511 django-customvueadmin-0.1.1/custom_admin/api/serializers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/serializers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5559 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/serializers/base_serializer.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      761 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/urls.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.298511 django-customvueadmin-0.1.1/custom_admin/api/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      509 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1984 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/views/admin_log.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5735 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/views/autocomplete.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9283 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/views/base_admin_viewset.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      588 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/views/change_language.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      748 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/views/get_sections.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3440 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/views/token_auth.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      983 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/api/viewset_info.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.298511 django-customvueadmin-0.1.1/custom_admin/controllers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-03-23 13:11:18.000000 django-customvueadmin-0.1.1/custom_admin/controllers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3505 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/controllers/admin_log_manager.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3909 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/controllers/custom_metadata.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2911 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/controllers/filters_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8985 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/controllers/schema_generator.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.298511 django-customvueadmin-0.1.1/custom_admin/migrations/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1790 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.1/custom_admin/migrations/0001_initial.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1006 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.1/custom_admin/migrations/0002_auto_20220826_1734.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      751 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.1/custom_admin/migrations/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.298511 django-customvueadmin-0.1.1/custom_admin/models/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.1/custom_admin/models/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/models/admin_log.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.298511 django-customvueadmin-0.1.1/custom_admin/tests/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.1/custom_admin/tests/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      581 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.1/custom_admin/tests/test_language.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      460 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.1/custom_admin/tests/test_scheme_get.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.298511 django-customvueadmin-0.1.1/custom_admin/utils/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/utils/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.1/custom_admin/utils/colors.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/utils/get_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/utils/register_admin_viewsets.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.298511 django-customvueadmin-0.1.1/custom_admin/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.1/custom_admin/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1311 2024-04-11 11:29:37.000000 django-customvueadmin-0.1.1/custom_admin/views/admin_page.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2989 2024-04-11 11:20:38.000000 django-customvueadmin-0.1.1/custom_admin/views/template.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:41:00.301845 django-customvueadmin-0.1.1/django_customvueadmin.egg-info/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2679 2024-04-11 11:41:00.000000 django-customvueadmin-0.1.1/django_customvueadmin.egg-info/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2527 2024-04-11 11:41:00.000000 django-customvueadmin-0.1.1/django_customvueadmin.egg-info/SOURCES.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 11:41:00.000000 django-customvueadmin-0.1.1/django_customvueadmin.egg-info/dependency_links.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       82 2024-04-11 11:41:00.000000 django-customvueadmin-0.1.1/django_customvueadmin.egg-info/entry_points.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 09:29:05.000000 django-customvueadmin-0.1.1/django_customvueadmin.egg-info/not-zip-safe
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-11 11:41:00.000000 django-customvueadmin-0.1.1/django_customvueadmin.egg-info/requires.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-04-11 11:41:00.000000 django-customvueadmin-0.1.1/django_customvueadmin.egg-info/top_level.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django-customvueadmin-0.1.1/pyproject.toml
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1099 2024-04-11 11:41:00.301845 django-customvueadmin-0.1.1/setup.cfg
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.844744 django-customvueadmin-0.1.2/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2852 2024-04-11 11:49:02.844744 django-customvueadmin-0.1.2/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2002 2024-04-11 11:45:03.000000 django-customvueadmin-0.1.2/README.rst
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-04-11 11:48:45.000000 django-customvueadmin-0.1.2/custom_admin/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/api/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/api/actions/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/actions/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      738 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/actions/delete_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2466 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/actions/export_csv_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2161 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/actions/view_actions_mixin.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/api/fields/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      370 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/base.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      706 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/char.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1091 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/choice.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3057 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/files.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/int.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/numbers.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/fields/relation.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/api/filters/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      114 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/filters/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1558 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/filters/base_admin_filter.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/filters/choices.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/api/inlines/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/export_csv_inline.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1627 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/inline_graph.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/inline_table.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/inlines_type.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/interfaces.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django-customvueadmin-0.1.2/custom_admin/api/inlines/view_inline_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/permissions.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.838076 django-customvueadmin-0.1.2/custom_admin/api/serializers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/serializers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5559 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/serializers/base_serializer.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      761 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/urls.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/api/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      509 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1984 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/admin_log.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5735 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/autocomplete.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9283 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/base_admin_viewset.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      588 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/change_language.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      748 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/get_sections.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3440 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/views/token_auth.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      983 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/api/viewset_info.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/controllers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-03-23 13:11:18.000000 django-customvueadmin-0.1.2/custom_admin/controllers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3505 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/controllers/admin_log_manager.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3909 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/controllers/custom_metadata.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2911 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/controllers/filters_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8985 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/controllers/schema_generator.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/migrations/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1790 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/migrations/0001_initial.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1006 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/migrations/0002_auto_20220826_1734.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      751 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/migrations/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/models/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/models/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/models/admin_log.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/tests/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/tests/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      581 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/tests/test_language.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      460 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.2/custom_admin/tests/test_scheme_get.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/utils/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/utils/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.2/custom_admin/utils/colors.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/utils/get_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/utils/register_admin_viewsets.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/custom_admin/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.2/custom_admin/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1314 2024-04-11 11:48:23.000000 django-customvueadmin-0.1.2/custom_admin/views/admin_page.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2989 2024-04-11 11:20:38.000000 django-customvueadmin-0.1.2/custom_admin/views/template.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 11:49:02.841410 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2852 2024-04-11 11:49:02.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2528 2024-04-11 11:49:02.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 11:49:02.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       82 2024-04-11 11:49:02.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/entry_points.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 09:29:05.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/not-zip-safe
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-11 11:49:02.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/requires.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-04-11 11:49:02.000000 django-customvueadmin-0.1.2/django_customvueadmin.egg-info/top_level.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django-customvueadmin-0.1.2/pyproject.toml
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1100 2024-04-11 11:49:02.844744 django-customvueadmin-0.1.2/setup.cfg
```

### Comparing `django-customvueadmin-0.1.1/PKG-INFO` & `django-customvueadmin-0.1.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,58 @@
-Metadata-Version: 2.1
-Name: django-customvueadmin
-Version: 0.1.1
-Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
-Home-page: https://innova-group-llc.github.io/custom_admin_docs/
-License: BSD-3-Clause
-Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
-Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
-Provides-Extra: argon2
-Requires-Dist: argon2-cffi>=19.1.0; extra == "argon2"
-Provides-Extra: bcrypt
-Requires-Dist: bcrypt; extra == "bcrypt"
-
-# Django Custom Admin
-
-
-[![logo](https://raw.githubusercontent.com/greyli/flask-share/master/images/demo.png)](https://innova-group-llc.github.io/custom_admin_docs/)
-
-A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
-
-[![PyPI version](https://badge.fury.io/py/django-customvueadmin.svg)](https://pypi.org/project/django-customvueadmin/)
-[![GitHub stars](https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin)](https://github.com/Innova-Group-LLC/custom_admin)
-
-[Documentation](https://innova-group-llc.github.io/custom_admin_docs/)
-
-## Features
-
-- The web view runs on **Vue 2** using **Element UI**
-- Pre-builded Vue SPA front page provided through html template and static files
-- All endpoints run on Django Rest Framework view-set's (supports both ORM and non-ORM data sources)
-- A powerful inline system with related entities
-- Support for **django-modeltranslation** translations
-- Ability to output any data within inlines (such as external logs with pagination)
-- Ability to create admin actions using forms via drf serializers
-- Dynamic system for obtaining partition scheme and interface structure
-- Access rights sharing system based on DRF permissioins
-- Related fields with autocomplete search
-- WYSIWYG editor using TinyMCE 4
-- JSON editor using CodeMirror
-- Related fields Autocomplete and Filters using Vue Tags Input
-
-# Vue frontend
-
-```
-npm install --prefix vue_frontend
-npm run serve --prefix vue_frontend
-```
-
-## Build
-```
-npm run build --prefix vue_frontend
-rm -r custom_admin/static/*
-cp vue_frontend/dist/favicon.ico custom_admin/static/favicon.ico
-cp vue_frontend/dist/manifest.json custom_admin/static/manifest.json
-cp -r vue_frontend/dist/tinymce/ custom_admin/static/tinymce/
-cp -r vue_frontend/dist/static/ custom_admin/
-```
+Django Custom Admin
+===================
+
+|logo|
+
+A custom admin interface providing backend via DRF and frontend via Vue
+and Element UI that tries Keep It Simple.
+
+|PyPI version| |GitHub stars|
+
+`Documentation <https://innova-group-llc.github.io/custom_admin_docs/>`__
+
+Features
+--------
+
+-  The web view runs on **Vue 2** using **Element UI**
+-  Pre-builded Vue SPA front page provided through html template and
+   static files
+-  All endpoints run on Django Rest Framework view-set’s (supports both
+   ORM and non-ORM data sources)
+-  A powerful inline system with related entities
+-  Support for **django-modeltranslation** translations
+-  Ability to output any data within inlines (such as external logs with
+   pagination)
+-  Ability to create admin actions using forms via drf serializers
+-  Dynamic system for obtaining partition scheme and interface structure
+-  Access rights sharing system based on DRF permissioins
+-  Related fields with autocomplete search
+-  WYSIWYG editor using TinyMCE 4
+-  JSON editor using CodeMirror
+-  Related fields Autocomplete and Filters using Vue Tags Input
+
+Vue frontend
+============
+
+::
+
+   npm install --prefix vue_frontend
+   npm run serve --prefix vue_frontend
+
+Build
+-----
+
+::
+
+   npm run build --prefix vue_frontend
+   rm -r custom_admin/static/*
+   cp vue_frontend/dist/favicon.ico custom_admin/static/favicon.ico
+   cp vue_frontend/dist/manifest.json custom_admin/static/manifest.json
+   cp -r vue_frontend/dist/tinymce/ custom_admin/static/tinymce/
+   cp -r vue_frontend/dist/static/ custom_admin/
+
+.. |logo| image:: https://raw.githubusercontent.com/greyli/flask-share/master/images/demo.png
+   :target: https://innova-group-llc.github.io/custom_admin_docs/
+.. |PyPI version| image:: https://badge.fury.io/py/django-customvueadmin.svg
+   :target: https://pypi.org/project/django-customvueadmin/
+.. |GitHub stars| image:: https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin
+   :target: https://github.com/Innova-Group-LLC/custom_admin
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-customvueadmin-0.1.1/README.md` & `django-customvueadmin-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,77 @@
-# Django Custom Admin
-
-
-[![logo](https://raw.githubusercontent.com/greyli/flask-share/master/images/demo.png)](https://innova-group-llc.github.io/custom_admin_docs/)
-
-A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
-
-[![PyPI version](https://badge.fury.io/py/django-customvueadmin.svg)](https://pypi.org/project/django-customvueadmin/)
-[![GitHub stars](https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin)](https://github.com/Innova-Group-LLC/custom_admin)
-
-[Documentation](https://innova-group-llc.github.io/custom_admin_docs/)
-
-## Features
-
-- The web view runs on **Vue 2** using **Element UI**
-- Pre-builded Vue SPA front page provided through html template and static files
-- All endpoints run on Django Rest Framework view-set's (supports both ORM and non-ORM data sources)
-- A powerful inline system with related entities
-- Support for **django-modeltranslation** translations
-- Ability to output any data within inlines (such as external logs with pagination)
-- Ability to create admin actions using forms via drf serializers
-- Dynamic system for obtaining partition scheme and interface structure
-- Access rights sharing system based on DRF permissioins
-- Related fields with autocomplete search
-- WYSIWYG editor using TinyMCE 4
-- JSON editor using CodeMirror
-- Related fields Autocomplete and Filters using Vue Tags Input
-
-# Vue frontend
-
-```
-npm install --prefix vue_frontend
-npm run serve --prefix vue_frontend
-```
-
-## Build
-```
-npm run build --prefix vue_frontend
-rm -r custom_admin/static/*
-cp vue_frontend/dist/favicon.ico custom_admin/static/favicon.ico
-cp vue_frontend/dist/manifest.json custom_admin/static/manifest.json
-cp -r vue_frontend/dist/tinymce/ custom_admin/static/tinymce/
-cp -r vue_frontend/dist/static/ custom_admin/
-```
+Metadata-Version: 2.1
+Name: django-customvueadmin
+Version: 0.1.2
+Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
+Home-page: https://innova-group-llc.github.io/custom_admin_docs/
+License: BSD-3-Clause
+Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
+Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Provides-Extra: argon2
+Requires-Dist: argon2-cffi>=19.1.0; extra == "argon2"
+Provides-Extra: bcrypt
+Requires-Dist: bcrypt; extra == "bcrypt"
+
+Django Custom Admin
+===================
+
+|logo|
+
+A custom admin interface providing backend via DRF and frontend via Vue
+and Element UI that tries Keep It Simple.
+
+|PyPI version| |GitHub stars|
+
+`Documentation <https://innova-group-llc.github.io/custom_admin_docs/>`__
+
+Features
+--------
+
+-  The web view runs on **Vue 2** using **Element UI**
+-  Pre-builded Vue SPA front page provided through html template and
+   static files
+-  All endpoints run on Django Rest Framework view-set’s (supports both
+   ORM and non-ORM data sources)
+-  A powerful inline system with related entities
+-  Support for **django-modeltranslation** translations
+-  Ability to output any data within inlines (such as external logs with
+   pagination)
+-  Ability to create admin actions using forms via drf serializers
+-  Dynamic system for obtaining partition scheme and interface structure
+-  Access rights sharing system based on DRF permissioins
+-  Related fields with autocomplete search
+-  WYSIWYG editor using TinyMCE 4
+-  JSON editor using CodeMirror
+-  Related fields Autocomplete and Filters using Vue Tags Input
+
+Vue frontend
+============
+
+::
+
+   npm install --prefix vue_frontend
+   npm run serve --prefix vue_frontend
+
+Build
+-----
+
+::
+
+   npm run build --prefix vue_frontend
+   rm -r custom_admin/static/*
+   cp vue_frontend/dist/favicon.ico custom_admin/static/favicon.ico
+   cp vue_frontend/dist/manifest.json custom_admin/static/manifest.json
+   cp -r vue_frontend/dist/tinymce/ custom_admin/static/tinymce/
+   cp -r vue_frontend/dist/static/ custom_admin/
+
+.. |logo| image:: https://raw.githubusercontent.com/greyli/flask-share/master/images/demo.png
+   :target: https://innova-group-llc.github.io/custom_admin_docs/
+.. |PyPI version| image:: https://badge.fury.io/py/django-customvueadmin.svg
+   :target: https://pypi.org/project/django-customvueadmin/
+.. |GitHub stars| image:: https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin
+   :target: https://github.com/Innova-Group-LLC/custom_admin
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/actions/delete_action.py` & `django-customvueadmin-0.1.2/custom_admin/api/actions/delete_action.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/actions/export_csv_action.py` & `django-customvueadmin-0.1.2/custom_admin/api/actions/export_csv_action.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/actions/view_actions_mixin.py` & `django-customvueadmin-0.1.2/custom_admin/api/actions/view_actions_mixin.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/fields/char.py` & `django-customvueadmin-0.1.2/custom_admin/api/fields/char.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/fields/choice.py` & `django-customvueadmin-0.1.2/custom_admin/api/fields/choice.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/fields/files.py` & `django-customvueadmin-0.1.2/custom_admin/api/fields/files.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/fields/relation.py` & `django-customvueadmin-0.1.2/custom_admin/api/fields/relation.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/filters/base_admin_filter.py` & `django-customvueadmin-0.1.2/custom_admin/api/filters/base_admin_filter.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/inlines/export_csv_inline.py` & `django-customvueadmin-0.1.2/custom_admin/api/inlines/export_csv_inline.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/inlines/inline_graph.py` & `django-customvueadmin-0.1.2/custom_admin/api/inlines/inline_graph.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/inlines/inline_table.py` & `django-customvueadmin-0.1.2/custom_admin/api/inlines/inline_table.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/inlines/view_inline_mixin.py` & `django-customvueadmin-0.1.2/custom_admin/api/inlines/view_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/permissions.py` & `django-customvueadmin-0.1.2/custom_admin/api/permissions.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/serializers/base_serializer.py` & `django-customvueadmin-0.1.2/custom_admin/api/serializers/base_serializer.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/urls.py` & `django-customvueadmin-0.1.2/custom_admin/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/views/admin_log.py` & `django-customvueadmin-0.1.2/custom_admin/api/views/admin_log.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/views/autocomplete.py` & `django-customvueadmin-0.1.2/custom_admin/api/views/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/views/base_admin_viewset.py` & `django-customvueadmin-0.1.2/custom_admin/api/views/base_admin_viewset.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/views/change_language.py` & `django-customvueadmin-0.1.2/custom_admin/api/views/change_language.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/views/get_sections.py` & `django-customvueadmin-0.1.2/custom_admin/api/views/get_sections.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/views/token_auth.py` & `django-customvueadmin-0.1.2/custom_admin/api/views/token_auth.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/api/viewset_info.py` & `django-customvueadmin-0.1.2/custom_admin/api/viewset_info.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/controllers/admin_log_manager.py` & `django-customvueadmin-0.1.2/custom_admin/controllers/admin_log_manager.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/controllers/custom_metadata.py` & `django-customvueadmin-0.1.2/custom_admin/controllers/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/controllers/filters_schema.py` & `django-customvueadmin-0.1.2/custom_admin/controllers/filters_schema.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/controllers/schema_generator.py` & `django-customvueadmin-0.1.2/custom_admin/controllers/schema_generator.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/migrations/0001_initial.py` & `django-customvueadmin-0.1.2/custom_admin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/migrations/0002_auto_20220826_1734.py` & `django-customvueadmin-0.1.2/custom_admin/migrations/0002_auto_20220826_1734.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py` & `django-customvueadmin-0.1.2/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/models/admin_log.py` & `django-customvueadmin-0.1.2/custom_admin/models/admin_log.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/tests/test_language.py` & `django-customvueadmin-0.1.2/custom_admin/tests/test_language.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/utils/colors.py` & `django-customvueadmin-0.1.2/custom_admin/utils/colors.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/utils/get_schema.py` & `django-customvueadmin-0.1.2/custom_admin/utils/get_schema.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/utils/register_admin_viewsets.py` & `django-customvueadmin-0.1.2/custom_admin/utils/register_admin_viewsets.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/custom_admin/views/admin_page.py` & `django-customvueadmin-0.1.2/custom_admin/views/admin_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 Custom admin cannot find template "{template}".
 Make sure settings.TEMPLATES contains 'APP_DIRS': True
 '''
 
 
 class CustomAdminView(View):
     '''
-    # Settings in case of https:
+    # Settings in case of h2ttps:
     USE_X_FORWARDED_HOST = True
     SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTO', 'https')
     '''
 
-    template = 'custom_admin/admin_index.py'
+    template = 'custom_admin/admin_index.html'
 
     def get(self, request):
         admin_settings = {
             'title': settings.CUSTOM_ADMIN.get('title'),
             'base_admin_url': settings.CUSTOM_ADMIN.get('base_admin_url') or 'admin/',
             'static_prefix': settings.CUSTOM_ADMIN.get('static_prefix') or '/static',
         }
```

### Comparing `django-customvueadmin-0.1.1/custom_admin/views/template.py` & `django-customvueadmin-0.1.2/custom_admin/views/template.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.1/django_customvueadmin.egg-info/PKG-INFO` & `django-customvueadmin-0.1.2/django_customvueadmin.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.1.1
+Version: 0.1.2
 Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,51 +13,65 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Provides-Extra: argon2
 Requires-Dist: argon2-cffi>=19.1.0; extra == "argon2"
 Provides-Extra: bcrypt
 Requires-Dist: bcrypt; extra == "bcrypt"
 
-# Django Custom Admin
+Django Custom Admin
+===================
 
+|logo|
 
-[![logo](https://raw.githubusercontent.com/greyli/flask-share/master/images/demo.png)](https://innova-group-llc.github.io/custom_admin_docs/)
+A custom admin interface providing backend via DRF and frontend via Vue
+and Element UI that tries Keep It Simple.
 
-A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
-
-[![PyPI version](https://badge.fury.io/py/django-customvueadmin.svg)](https://pypi.org/project/django-customvueadmin/)
-[![GitHub stars](https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin)](https://github.com/Innova-Group-LLC/custom_admin)
-
-[Documentation](https://innova-group-llc.github.io/custom_admin_docs/)
-
-## Features
-
-- The web view runs on **Vue 2** using **Element UI**
-- Pre-builded Vue SPA front page provided through html template and static files
-- All endpoints run on Django Rest Framework view-set's (supports both ORM and non-ORM data sources)
-- A powerful inline system with related entities
-- Support for **django-modeltranslation** translations
-- Ability to output any data within inlines (such as external logs with pagination)
-- Ability to create admin actions using forms via drf serializers
-- Dynamic system for obtaining partition scheme and interface structure
-- Access rights sharing system based on DRF permissioins
-- Related fields with autocomplete search
-- WYSIWYG editor using TinyMCE 4
-- JSON editor using CodeMirror
-- Related fields Autocomplete and Filters using Vue Tags Input
-
-# Vue frontend
-
-```
-npm install --prefix vue_frontend
-npm run serve --prefix vue_frontend
-```
-
-## Build
-```
-npm run build --prefix vue_frontend
-rm -r custom_admin/static/*
-cp vue_frontend/dist/favicon.ico custom_admin/static/favicon.ico
-cp vue_frontend/dist/manifest.json custom_admin/static/manifest.json
-cp -r vue_frontend/dist/tinymce/ custom_admin/static/tinymce/
-cp -r vue_frontend/dist/static/ custom_admin/
-```
+|PyPI version| |GitHub stars|
+
+`Documentation <https://innova-group-llc.github.io/custom_admin_docs/>`__
+
+Features
+--------
+
+-  The web view runs on **Vue 2** using **Element UI**
+-  Pre-builded Vue SPA front page provided through html template and
+   static files
+-  All endpoints run on Django Rest Framework view-set’s (supports both
+   ORM and non-ORM data sources)
+-  A powerful inline system with related entities
+-  Support for **django-modeltranslation** translations
+-  Ability to output any data within inlines (such as external logs with
+   pagination)
+-  Ability to create admin actions using forms via drf serializers
+-  Dynamic system for obtaining partition scheme and interface structure
+-  Access rights sharing system based on DRF permissioins
+-  Related fields with autocomplete search
+-  WYSIWYG editor using TinyMCE 4
+-  JSON editor using CodeMirror
+-  Related fields Autocomplete and Filters using Vue Tags Input
+
+Vue frontend
+============
+
+::
+
+   npm install --prefix vue_frontend
+   npm run serve --prefix vue_frontend
+
+Build
+-----
+
+::
+
+   npm run build --prefix vue_frontend
+   rm -r custom_admin/static/*
+   cp vue_frontend/dist/favicon.ico custom_admin/static/favicon.ico
+   cp vue_frontend/dist/manifest.json custom_admin/static/manifest.json
+   cp -r vue_frontend/dist/tinymce/ custom_admin/static/tinymce/
+   cp -r vue_frontend/dist/static/ custom_admin/
+
+.. |logo| image:: https://raw.githubusercontent.com/greyli/flask-share/master/images/demo.png
+   :target: https://innova-group-llc.github.io/custom_admin_docs/
+.. |PyPI version| image:: https://badge.fury.io/py/django-customvueadmin.svg
+   :target: https://pypi.org/project/django-customvueadmin/
+.. |GitHub stars| image:: https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin
+   :target: https://github.com/Innova-Group-LLC/custom_admin
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-customvueadmin-0.1.1/django_customvueadmin.egg-info/SOURCES.txt` & `django-customvueadmin-0.1.2/django_customvueadmin.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-README.md
+README.rst
 pyproject.toml
 setup.cfg
 custom_admin/__init__.py
 custom_admin/api/__init__.py
 custom_admin/api/permissions.py
 custom_admin/api/urls.py
 custom_admin/api/viewset_info.py
```

### Comparing `django-customvueadmin-0.1.1/setup.cfg` & `django-customvueadmin-0.1.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = django-customvueadmin
 version = attr: custom_admin.__version__
 url = https://innova-group-llc.github.io/custom_admin_docs/
 description = A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
-long_description = file: README.md
+long_description = file: README.rst
 license = BSD-3-Clause
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
```

