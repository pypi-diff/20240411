# Comparing `tmp/django-customvueadmin-0.1.6.tar.gz` & `tmp/django-customvueadmin-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-customvueadmin-0.1.6.tar", last modified: Thu Apr 11 14:27:06 2024, max compression
+gzip compressed data, was "django-customvueadmin-0.1.7.tar", last modified: Thu Apr 11 14:46:49 2024, max compression
```

## Comparing `django-customvueadmin-0.1.6.tar` & `django-customvueadmin-0.1.7.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      209 2024-04-11 14:26:38.000000 django-customvueadmin-0.1.6/MANIFEST.in
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2855 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2005 2024-04-11 12:39:26.000000 django-customvueadmin-0.1.6/README.rst
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-04-11 14:27:03.000000 django-customvueadmin-0.1.6/custom_admin/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/api/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/api/actions/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/actions/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      738 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/actions/delete_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2466 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/actions/export_csv_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2161 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/actions/view_actions_mixin.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/api/fields/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      370 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/base.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      706 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/char.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1091 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/choice.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3057 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/files.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/int.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/numbers.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/fields/relation.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/api/filters/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      114 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/filters/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1558 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/filters/base_admin_filter.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/filters/choices.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/api/inlines/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/export_csv_inline.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1627 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/inline_graph.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/inline_table.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/inlines_type.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/interfaces.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django-customvueadmin-0.1.6/custom_admin/api/inlines/view_inline_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/permissions.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/api/serializers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/serializers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5559 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/serializers/base_serializer.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      761 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/urls.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/api/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      509 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1984 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/admin_log.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5735 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/autocomplete.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9283 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/base_admin_viewset.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      588 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/change_language.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      748 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/get_sections.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3440 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/views/token_auth.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      983 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/api/viewset_info.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/controllers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-03-23 13:11:18.000000 django-customvueadmin-0.1.6/custom_admin/controllers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3505 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/controllers/admin_log_manager.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3909 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/controllers/custom_metadata.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2911 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/controllers/filters_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8985 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/controllers/schema_generator.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/migrations/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1790 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/migrations/0001_initial.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1006 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/migrations/0002_auto_20220826_1734.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      751 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/migrations/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/models/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/models/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/models/admin_log.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/static/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.120128 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.123462 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    27506 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/app.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      131 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-3ef8a5a8.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4748 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-7402f562.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      762 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-8b69702c.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1632 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-a7c7287a.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       71 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-ecedfa6a.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   233274 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-elementUI.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    10292 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-fdcfea10.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3568 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-libs.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    67646 2024-04-11 09:39:27.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/favicon.ico
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.123462 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/fonts/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    55956 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/fonts/element-icons.ttf
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    28200 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/fonts/element-icons.woff
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.123462 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/img/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    98071 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/img/404.png
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4766 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/img/404_cloud.png
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.126795 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    53669 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/app.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      925 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-2d0c14f9.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    11162 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-2d2080da.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    21542 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-3ef8a5a8.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   122331 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-5148deb9.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   200033 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-6786f71b.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1766 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-7402f562.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    39131 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-8b69702c.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4166 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-a7c7287a.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3542 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-ecedfa6a.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   672429 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-elementUI.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   215439 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-fdcfea10.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   579815 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-libs.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3247 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/runtime.js
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.126795 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.126795 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-first/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4788 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    50376 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.126795 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-slim/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4730 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    49965 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/img/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    14708 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/img/example.png
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    15764 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/lightgray/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3193 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/lightgray/fonts/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     7664 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    38232 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/accordion.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1251 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/codesample/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1736 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1171290 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/tinymce.min.js
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.116794 django-customvueadmin-0.1.6/custom_admin/templates/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/templates/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2949 2024-04-11 13:23:28.000000 django-customvueadmin-0.1.6/custom_admin/templates/custom_admin/admin_index.html
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/tests/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/tests/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      581 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/tests/test_language.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      460 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.6/custom_admin/tests/test_scheme_get.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/utils/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/utils/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.6/custom_admin/utils/colors.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/utils/get_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/utils/register_admin_viewsets.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/custom_admin/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.6/custom_admin/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1314 2024-04-11 13:20:41.000000 django-customvueadmin-0.1.6/custom_admin/views/admin_page.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2855 2024-04-11 14:27:06.000000 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4852 2024-04-11 14:27:06.000000 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/SOURCES.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 14:27:06.000000 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/dependency_links.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 14:11:51.000000 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/not-zip-safe
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-11 14:27:06.000000 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/requires.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-04-11 14:27:06.000000 django-customvueadmin-0.1.6/django_customvueadmin.egg-info/top_level.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django-customvueadmin-0.1.6/pyproject.toml
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      992 2024-04-11 14:27:06.130129 django-customvueadmin-0.1.6/setup.cfg
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.788515 django-customvueadmin-0.1.7/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      209 2024-04-11 14:26:38.000000 django-customvueadmin-0.1.7/MANIFEST.in
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2855 2024-04-11 14:46:49.788515 django-customvueadmin-0.1.7/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2005 2024-04-11 12:39:26.000000 django-customvueadmin-0.1.7/README.rst
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.775180 django-customvueadmin-0.1.7/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-04-11 14:44:16.000000 django-customvueadmin-0.1.7/custom_admin/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.775180 django-customvueadmin-0.1.7/custom_admin/api/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.775180 django-customvueadmin-0.1.7/custom_admin/api/actions/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/actions/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      738 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/actions/delete_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2466 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/actions/export_csv_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2161 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/actions/view_actions_mixin.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.775180 django-customvueadmin-0.1.7/custom_admin/api/fields/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      370 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/fields/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/fields/base.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      706 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/fields/char.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1091 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/fields/choice.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3057 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/fields/files.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/fields/int.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/fields/numbers.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/fields/relation.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.775180 django-customvueadmin-0.1.7/custom_admin/api/filters/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      114 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/filters/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1558 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/filters/base_admin_filter.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/filters/choices.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.775180 django-customvueadmin-0.1.7/custom_admin/api/inlines/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/inlines/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/inlines/export_csv_inline.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1627 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.7/custom_admin/api/inlines/inline_graph.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/inlines/inline_table.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django-customvueadmin-0.1.7/custom_admin/api/inlines/inlines_type.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/inlines/interfaces.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django-customvueadmin-0.1.7/custom_admin/api/inlines/view_inline_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/permissions.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.775180 django-customvueadmin-0.1.7/custom_admin/api/serializers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/serializers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5559 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/serializers/base_serializer.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      761 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/urls.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.778514 django-customvueadmin-0.1.7/custom_admin/api/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      509 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1984 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/views/admin_log.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5735 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/views/autocomplete.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9283 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/views/base_admin_viewset.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      588 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/views/change_language.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      748 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/views/get_sections.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3440 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/views/token_auth.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      983 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/api/viewset_info.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.778514 django-customvueadmin-0.1.7/custom_admin/controllers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-03-23 13:11:18.000000 django-customvueadmin-0.1.7/custom_admin/controllers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3505 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/controllers/admin_log_manager.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3909 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/controllers/custom_metadata.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2911 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/controllers/filters_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8985 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/controllers/schema_generator.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.778514 django-customvueadmin-0.1.7/custom_admin/migrations/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1790 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.7/custom_admin/migrations/0001_initial.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1006 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.7/custom_admin/migrations/0002_auto_20220826_1734.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      751 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.7/custom_admin/migrations/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.778514 django-customvueadmin-0.1.7/custom_admin/models/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.7/custom_admin/models/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/models/admin_log.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.771847 django-customvueadmin-0.1.7/custom_admin/static/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.778514 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.778514 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    27506 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/app.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      131 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-3ef8a5a8.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4748 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-7402f562.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      762 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-8b69702c.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1632 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-a7c7287a.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       71 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-ecedfa6a.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   233274 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-elementUI.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    10292 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-fdcfea10.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3568 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-libs.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    67646 2024-04-11 09:39:27.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/favicon.ico
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.778514 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/fonts/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    55956 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/fonts/element-icons.ttf
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    28200 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/fonts/element-icons.woff
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.781848 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/img/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    98071 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/img/404.png
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4766 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/img/404_cloud.png
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.785181 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    53669 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/app.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      925 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-2d0c14f9.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    11162 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-2d2080da.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    21542 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-3ef8a5a8.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   122331 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-5148deb9.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   200033 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-6786f71b.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1766 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-7402f562.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    39131 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-8b69702c.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4166 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-a7c7287a.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3542 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-ecedfa6a.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   672429 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-elementUI.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   215439 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-fdcfea10.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   579815 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-libs.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3247 2024-04-11 09:40:28.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/runtime.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.785181 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.785181 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/dark-first/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4788 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    50376 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.785181 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/dark-slim/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4730 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    49965 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.785181 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/img/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    14708 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/img/example.png
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    15764 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.785181 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/lightgray/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3193 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.785181 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/lightgray/fonts/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     7664 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    38232 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.771847 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/plugins/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.785181 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/plugins/accordion/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.788515 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/accordion.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1251 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.771847 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/plugins/codesample/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.788515 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1736 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1171290 2024-04-11 09:39:41.000000 django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/tinymce.min.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.771847 django-customvueadmin-0.1.7/custom_admin/templates/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.788515 django-customvueadmin-0.1.7/custom_admin/templates/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3369 2024-04-11 14:42:58.000000 django-customvueadmin-0.1.7/custom_admin/templates/custom_admin/admin_index.html
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.788515 django-customvueadmin-0.1.7/custom_admin/tests/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.7/custom_admin/tests/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      581 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.7/custom_admin/tests/test_language.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      460 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.7/custom_admin/tests/test_scheme_get.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.788515 django-customvueadmin-0.1.7/custom_admin/utils/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/utils/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.7/custom_admin/utils/colors.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/utils/get_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/utils/register_admin_viewsets.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.788515 django-customvueadmin-0.1.7/custom_admin/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.7/custom_admin/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1327 2024-04-11 14:32:14.000000 django-customvueadmin-0.1.7/custom_admin/views/admin_page.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 14:46:49.788515 django-customvueadmin-0.1.7/django_customvueadmin.egg-info/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2855 2024-04-11 14:46:49.000000 django-customvueadmin-0.1.7/django_customvueadmin.egg-info/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4852 2024-04-11 14:46:49.000000 django-customvueadmin-0.1.7/django_customvueadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 14:46:49.000000 django-customvueadmin-0.1.7/django_customvueadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 14:11:51.000000 django-customvueadmin-0.1.7/django_customvueadmin.egg-info/not-zip-safe
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-11 14:46:49.000000 django-customvueadmin-0.1.7/django_customvueadmin.egg-info/requires.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-04-11 14:46:49.000000 django-customvueadmin-0.1.7/django_customvueadmin.egg-info/top_level.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django-customvueadmin-0.1.7/pyproject.toml
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      992 2024-04-11 14:46:49.788515 django-customvueadmin-0.1.7/setup.cfg
```

### Comparing `django-customvueadmin-0.1.6/PKG-INFO` & `django-customvueadmin-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.1.6
+Version: 0.1.7
 Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-customvueadmin-0.1.6/README.rst` & `django-customvueadmin-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/actions/delete_action.py` & `django-customvueadmin-0.1.7/custom_admin/api/actions/delete_action.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/actions/export_csv_action.py` & `django-customvueadmin-0.1.7/custom_admin/api/actions/export_csv_action.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/actions/view_actions_mixin.py` & `django-customvueadmin-0.1.7/custom_admin/api/actions/view_actions_mixin.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/fields/char.py` & `django-customvueadmin-0.1.7/custom_admin/api/fields/char.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/fields/choice.py` & `django-customvueadmin-0.1.7/custom_admin/api/fields/choice.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/fields/files.py` & `django-customvueadmin-0.1.7/custom_admin/api/fields/files.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/fields/relation.py` & `django-customvueadmin-0.1.7/custom_admin/api/fields/relation.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/filters/base_admin_filter.py` & `django-customvueadmin-0.1.7/custom_admin/api/filters/base_admin_filter.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/inlines/export_csv_inline.py` & `django-customvueadmin-0.1.7/custom_admin/api/inlines/export_csv_inline.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/inlines/inline_graph.py` & `django-customvueadmin-0.1.7/custom_admin/api/inlines/inline_graph.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/inlines/inline_table.py` & `django-customvueadmin-0.1.7/custom_admin/api/inlines/inline_table.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/inlines/view_inline_mixin.py` & `django-customvueadmin-0.1.7/custom_admin/api/inlines/view_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/permissions.py` & `django-customvueadmin-0.1.7/custom_admin/api/permissions.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/serializers/base_serializer.py` & `django-customvueadmin-0.1.7/custom_admin/api/serializers/base_serializer.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/urls.py` & `django-customvueadmin-0.1.7/custom_admin/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/views/admin_log.py` & `django-customvueadmin-0.1.7/custom_admin/api/views/admin_log.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/views/autocomplete.py` & `django-customvueadmin-0.1.7/custom_admin/api/views/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/views/base_admin_viewset.py` & `django-customvueadmin-0.1.7/custom_admin/api/views/base_admin_viewset.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/views/change_language.py` & `django-customvueadmin-0.1.7/custom_admin/api/views/change_language.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/views/get_sections.py` & `django-customvueadmin-0.1.7/custom_admin/api/views/get_sections.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/views/token_auth.py` & `django-customvueadmin-0.1.7/custom_admin/api/views/token_auth.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/api/viewset_info.py` & `django-customvueadmin-0.1.7/custom_admin/api/viewset_info.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/controllers/admin_log_manager.py` & `django-customvueadmin-0.1.7/custom_admin/controllers/admin_log_manager.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/controllers/custom_metadata.py` & `django-customvueadmin-0.1.7/custom_admin/controllers/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/controllers/filters_schema.py` & `django-customvueadmin-0.1.7/custom_admin/controllers/filters_schema.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/controllers/schema_generator.py` & `django-customvueadmin-0.1.7/custom_admin/controllers/schema_generator.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/migrations/0001_initial.py` & `django-customvueadmin-0.1.7/custom_admin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/migrations/0002_auto_20220826_1734.py` & `django-customvueadmin-0.1.7/custom_admin/migrations/0002_auto_20220826_1734.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py` & `django-customvueadmin-0.1.7/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/models/admin_log.py` & `django-customvueadmin-0.1.7/custom_admin/models/admin_log.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/app.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/app.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-7402f562.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-7402f562.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-8b69702c.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-8b69702c.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-a7c7287a.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-a7c7287a.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-elementUI.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-elementUI.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-fdcfea10.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-fdcfea10.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/css/chunk-libs.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/css/chunk-libs.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/favicon.ico` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/fonts/element-icons.ttf` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/fonts/element-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/fonts/element-icons.woff` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/fonts/element-icons.woff`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/img/404.png` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/img/404.png`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/img/404_cloud.png` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/img/404_cloud.png`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/app.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/app.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-2d0c14f9.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-2d0c14f9.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-2d2080da.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-2d2080da.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-3ef8a5a8.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-3ef8a5a8.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-5148deb9.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-5148deb9.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-6786f71b.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-6786f71b.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-7402f562.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-7402f562.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-8b69702c.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-8b69702c.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-a7c7287a.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-a7c7287a.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-ecedfa6a.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-ecedfa6a.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-elementUI.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-elementUI.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-fdcfea10.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-fdcfea10.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/chunk-libs.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/chunk-libs.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/js/runtime.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/js/runtime.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/img/example.png` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/img/example.png`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/static/custom_admin/tinymce/tinymce.min.js` & `django-customvueadmin-0.1.7/custom_admin/static/custom_admin/tinymce/tinymce.min.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/templates/custom_admin/admin_index.html` & `django-customvueadmin-0.1.7/custom_admin/templates/custom_admin/admin_index.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 <!DOCTYPE html>
 <html>
     <head>
         <meta charset=utf-8>
         <meta http-equiv=X-UA-Compatible content="IE=edge,chrome=1">
         <meta name=viewport content="width=device-width,initial-scale=1,maximum-scale=1,user-scalable=no">
-        <title>{{ SETTINGS.TITLE }}</title>
-        <link href=/static/js/app.js rel=preload as=script>
-        <link href=/static/js/chunk-vendors.js rel=preload as=script>
-        <!--[if IE]><link rel="icon" type="image/png" href="/static/favicon.ico"><![endif]-->
+        <title>{{ SETTINGS.title }}</title>
+        <link href={{ SETTINGS.static_prefix }}/js/app.js rel=preload as=script>
+        <link href={{ SETTINGS.static_prefix }}/js/chunk-vendors.js rel=preload as=script>
+        <!--[if IE]><link rel="icon" type="image/png" href="{{ SETTINGS.static_prefix }}/favicon.ico"><![endif]-->
         <link rel=manifest href=/manifest.json>
         <meta name=theme-color content=#4DBA87>
         <meta name=apple-mobile-web-app-capable content=no>
         <meta name=apple-mobile-web-app-status-bar-style content=default>
         <meta name=apple-mobile-web-app-title content=vue-admin-template>
         <link rel=mask-icon href=/img/icons/safari-pinned-tab.svg color=#4DBA87>
         <meta name=msapplication-TileImage content=/img/icons/msapplication-icon-144x144.png>
         <meta name=msapplication-TileColor content=#000000>
-        <link href=/static/css/app.css rel=preload as=style>
-        <link href=/static/css/chunk-elementUI.css rel=preload as=style>
-        <link href=/static/css/chunk-libs.css rel=preload as=style>
-        <link href=/static/js/app.js rel=preload as=script>
-        <link href=/static/js/chunk-elementUI.js rel=preload as=script>
-        <link href=/static/js/chunk-libs.js rel=preload as=script>
-        <link href=/static/js/runtime.js rel=preload as=script>
-        <link href=/static/css/chunk-elementUI.css rel=stylesheet>
-        <link href=/static/css/chunk-libs.css rel=stylesheet>
-        <link href=/static/css/app.css rel=stylesheet>
-        <link rel=icon type=image/png href=/static/favicon.ico>
+        <link href={{ SETTINGS.static_prefix }}/css/app.css rel=preload as=style>
+        <link href={{ SETTINGS.static_prefix }}/css/chunk-elementUI.css rel=preload as=style>
+        <link href={{ SETTINGS.static_prefix }}/css/chunk-libs.css rel=preload as=style>
+        <link href={{ SETTINGS.static_prefix }}/js/app.js rel=preload as=script>
+        <link href={{ SETTINGS.static_prefix }}/js/chunk-elementUI.js rel=preload as=script>
+        <link href={{ SETTINGS.static_prefix }}/js/chunk-libs.js rel=preload as=script>
+        <link href={{ SETTINGS.static_prefix }}/js/runtime.js rel=preload as=script>
+        <link href={{ SETTINGS.static_prefix }}/css/chunk-elementUI.css rel=stylesheet>
+        <link href={{ SETTINGS.static_prefix }}/css/chunk-libs.css rel=stylesheet>
+        <link href={{ SETTINGS.static_prefix }}/css/app.css rel=stylesheet>
+        <link rel=icon type=image/png href={{ SETTINGS.static_prefix }}/favicon.ico>
         <link rel=manifest href=/manifest.json>
         <meta name=theme-color content=#4DBA87>
         <meta name=apple-mobile-web-app-capable content=no>
         <meta name=apple-mobile-web-app-status-bar-style content=default>
         <meta name=apple-mobile-web-app-title content=vue-admin-template>
         <link rel=mask-icon href=/img/icons/safari-pinned-tab.svg color=#4DBA87>
         <meta name=msapplication-TileImage content=/img/icons/msapplication-icon-144x144.png>
@@ -38,15 +38,15 @@
     </head>
     <body>
         <noscript>
             <strong>We're sorry but {{ SETTINGS.title }} doesn't work properly without JavaScript enabled. Please enable it to continue.</strong>
         </noscript>
         <div id=app></div>
         <span id=settings data-json="{{ SETTINGS_JSON }}"></span>
-        <!-- <script src=/static/js/chunk-vendors.js></script> -->
-        <script src=/static/js/app.js></script>
-        <script src=/static/js/runtime.js></script>
-        <script src=/static/js/chunk-elementUI.js></script>
-        <script src=/static/js/chunk-libs.js></script>
-        <script src=/static/js/app.js></script>
+        <!-- <script src={{ SETTINGS.static_prefix }}/js/chunk-vendors.js></script> -->
+        <script src={{ SETTINGS.static_prefix }}/js/app.js></script>
+        <script src={{ SETTINGS.static_prefix }}/js/runtime.js></script>
+        <script src={{ SETTINGS.static_prefix }}/js/chunk-elementUI.js></script>
+        <script src={{ SETTINGS.static_prefix }}/js/chunk-libs.js></script>
+        <script src={{ SETTINGS.static_prefix }}/js/app.js></script>
     </body>
 </html>
```

### Comparing `django-customvueadmin-0.1.6/custom_admin/tests/test_language.py` & `django-customvueadmin-0.1.7/custom_admin/tests/test_language.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/utils/colors.py` & `django-customvueadmin-0.1.7/custom_admin/utils/colors.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/utils/get_schema.py` & `django-customvueadmin-0.1.7/custom_admin/utils/get_schema.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/utils/register_admin_viewsets.py` & `django-customvueadmin-0.1.7/custom_admin/utils/register_admin_viewsets.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/custom_admin/views/admin_page.py` & `django-customvueadmin-0.1.7/custom_admin/views/admin_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     template = 'custom_admin/admin_index.html'
 
     def get(self, request):
         admin_settings = {
             'title': settings.CUSTOM_ADMIN.get('title'),
             'base_admin_url': settings.CUSTOM_ADMIN.get('base_admin_url') or 'admin/',
-            'static_prefix': settings.CUSTOM_ADMIN.get('static_prefix') or '/static',
+            'static_prefix': settings.CUSTOM_ADMIN.get('static_prefix') or '/static/custom_admin',
         }
 
         if not admin_settings.get('backend_prefix'):
             admin_settings['backend_prefix'] = request.build_absolute_uri('/custom_admin/')
 
         context = {
             'SETTINGS': admin_settings,
```

### Comparing `django-customvueadmin-0.1.6/django_customvueadmin.egg-info/PKG-INFO` & `django-customvueadmin-0.1.7/django_customvueadmin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.1.6
+Version: 0.1.7
 Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-customvueadmin-0.1.6/django_customvueadmin.egg-info/SOURCES.txt` & `django-customvueadmin-0.1.7/django_customvueadmin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.6/setup.cfg` & `django-customvueadmin-0.1.7/setup.cfg`

 * *Files identical despite different names*

