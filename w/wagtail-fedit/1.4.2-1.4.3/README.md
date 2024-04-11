# Comparing `tmp/wagtail_fedit-1.4.2.tar.gz` & `tmp/wagtail_fedit-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.4.2.tar", last modified: Mon Apr  8 20:13:52 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.4.3.tar", last modified: Wed Apr 10 11:12:58 2024, max compression
```

## Comparing `wagtail_fedit-1.4.2.tar` & `wagtail_fedit-1.4.3.tar`

### file list

```diff
@@ -1,109 +1,111 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.921758 wagtail_fedit-1.4.2/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0    12947 2024-04-08 20:13:52.921758 wagtail_fedit-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0    11954 2024-04-08 20:13:14.000000 wagtail_fedit-1.4.2/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-08 20:13:52.934635 wagtail_fedit-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.779712 wagtail_fedit-1.4.2/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.2/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.2/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.2/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.826655 wagtail_fedit-1.4.2/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.2/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.4.2/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.2/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     3356 2024-04-06 21:44:51.000000 wagtail_fedit-1.4.2/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.828661 wagtail_fedit-1.4.2/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.2/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.829656 wagtail_fedit-1.4.2/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.2/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.739663 wagtail_fedit-1.4.2/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.739663 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.834176 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.835353 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    15915 2024-04-06 00:14:04.000000 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.742063 wagtail_fedit-1.4.2/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.743064 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.837357 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.838357 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      302 2024-04-06 22:07:59.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      335 2024-04-06 22:08:01.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.851882 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     1709 2024-04-05 19:42:54.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      789 2024-04-07 05:29:57.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.863572 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.865583 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.869072 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
--rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
--rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
--rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
--rw-rw-rw-   0        0        0     1285 2024-04-06 18:43:26.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.871069 wagtail_fedit-1.4.2/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.2/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.873073 wagtail_fedit-1.4.2/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    19080 2024-04-08 20:04:44.000000 wagtail_fedit-1.4.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    15398 2024-04-08 20:08:45.000000 wagtail_fedit-1.4.2/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.875135 wagtail_fedit-1.4.2/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.879137 wagtail_fedit-1.4.2/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.885616 wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     3529 2024-04-05 23:35:47.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.894694 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7039 2024-04-05 23:57:48.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     4339 2024-04-06 00:03:48.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.903238 wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.4.2/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      916 2024-04-06 20:43:13.000000 wagtail_fedit-1.4.2/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    11238 2024-04-06 18:35:33.000000 wagtail_fedit-1.4.2/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.909210 wagtail_fedit-1.4.2/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.4.2/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.4.2/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0    14621 2024-04-05 23:51:10.000000 wagtail_fedit-1.4.2/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    12225 2024-04-06 19:48:05.000000 wagtail_fedit-1.4.2/wagtail_fedit/views/fields.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.2/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.920766 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      160 2024-04-06 18:20:48.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     6061 2024-04-06 18:49:36.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.823300 wagtail_fedit-1.4.2/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    12947 2024-04-08 20:13:52.000000 wagtail_fedit-1.4.2/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3476 2024-04-08 20:13:52.000000 wagtail_fedit-1.4.2/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 20:13:52.000000 wagtail_fedit-1.4.2/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-08 20:13:52.000000 wagtail_fedit-1.4.2/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-08 20:13:52.000000 wagtail_fedit-1.4.2/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.050708 wagtail_fedit-1.4.3/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    12947 2024-04-10 11:12:58.050708 wagtail_fedit-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11954 2024-04-08 20:13:14.000000 wagtail_fedit-1.4.3/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-10 11:12:58.065328 wagtail_fedit-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.816558 wagtail_fedit-1.4.3/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.3/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.3/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.3/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.864208 wagtail_fedit-1.4.3/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.3/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.4.3/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.3/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     3358 2024-04-10 10:24:35.000000 wagtail_fedit-1.4.3/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.866207 wagtail_fedit-1.4.3/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.3/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.867204 wagtail_fedit-1.4.3/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.3/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.757829 wagtail_fedit-1.4.3/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.758831 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.895693 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.917925 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    15915 2024-04-06 00:14:04.000000 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.760833 wagtail_fedit-1.4.3/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.762830 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.920885 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.922885 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      302 2024-04-06 22:07:59.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      335 2024-04-06 22:08:01.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.937885 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     1709 2024-04-05 19:42:54.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      789 2024-04-07 05:29:57.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.960915 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.974700 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.010629 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
+-rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
+-rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
+-rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
+-rw-rw-rw-   0        0        0     1285 2024-04-06 18:43:26.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.014256 wagtail_fedit-1.4.3/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.3/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.017296 wagtail_fedit-1.4.3/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    17845 2024-04-10 10:47:44.000000 wagtail_fedit-1.4.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14527 2024-04-10 10:47:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.018380 wagtail_fedit-1.4.3/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.020393 wagtail_fedit-1.4.3/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.026231 wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.035012 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7039 2024-04-05 23:57:48.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     2996 2024-04-10 10:50:37.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_block_templatetag.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3994 2024-04-10 11:08:06.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_field_templatetag.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     4339 2024-04-06 00:03:48.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.039393 wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.4.3/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      916 2024-04-06 20:43:13.000000 wagtail_fedit-1.4.3/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    15299 2024-04-10 10:23:23.000000 wagtail_fedit-1.4.3/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.043847 wagtail_fedit-1.4.3/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.4.3/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9206 2024-04-09 20:56:25.000000 wagtail_fedit-1.4.3/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0    14621 2024-04-05 23:51:10.000000 wagtail_fedit-1.4.3/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    12225 2024-04-06 19:48:05.000000 wagtail_fedit-1.4.3/wagtail_fedit/views/fields.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.3/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.050708 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      160 2024-04-06 18:20:48.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     6061 2024-04-06 18:49:36.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.859210 wagtail_fedit-1.4.3/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    12947 2024-04-10 11:12:57.000000 wagtail_fedit-1.4.3/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3588 2024-04-10 11:12:57.000000 wagtail_fedit-1.4.3/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 11:12:57.000000 wagtail_fedit-1.4.3/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-10 11:12:57.000000 wagtail_fedit-1.4.3/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 11:12:57.000000 wagtail_fedit-1.4.3/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.4.2/LICENSE` & `wagtail_fedit-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/PKG-INFO` & `wagtail_fedit-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.4.2
+Version: 1.4.3
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.2 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.3 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.4.2/README.md` & `wagtail_fedit-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/setup.cfg` & `wagtail_fedit-1.4.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 342e  ..version = 1.4.
-00000030: 320d 0a64 6573 6372 6970 7469 6f6e 203d  2..description =
+00000030: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.4.3/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.4.3/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/hooks.py` & `wagtail_fedit-1.4.3/wagtail_fedit/hooks.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 def prefix(name):
     """
         Default prefix for wagtail_fedit hooks.
     """
     return f"wagtail_fedit.{name}"
 
 
+CONSTRUCT_BLOCK_TOOLBAR  = prefix("construct_block_toolbar")
 """
 ### wagtail_fedit.construct_block_toolbar
 Construct the toolbar for the given block.
 This is used to display the edit icon in the block.
 
 How it is called:
 
 ```python
 for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR):
     hook(request=request, items=items, model=model, block_id=block_id, field_name=field_name)
 ```
 """
-CONSTRUCT_BLOCK_TOOLBAR  = prefix("construct_block_toolbar")
 
 
+CONSTRUCT_FIELD_TOOLBAR  = prefix("construct_field_toolbar")
 """
 ### wagtail_fedit.construct_field_toolbar
 Construct the toolbar for the given field.
 This is used to display the edit icon in the field.
 
 How it is called:
 
 ```python
 for hook in hooks.get_hooks(CONSTRUCT_FIELD_TOOLBAR):
     hook(request=request, items=items, model=model, field_name=field_name)
 ```
 """
-CONSTRUCT_FIELD_TOOLBAR  = prefix("construct_field_toolbar")
 
 
+REGISTER_TYPE_RENDERER   = prefix("register_type_renderer")
 """
 ### wagtail_fedit.register_type_renderer
 Register a custom renderer for a type.
 
 Example of how this type of renderer can be used:
 
 ```python
@@ -49,17 +50,17 @@
     # It will render the Page model as a simple h2 tag.
     renderer_map[Page] = lambda request, context, instance, value: format_html(
         '<h2>{0}</h2>',
         value.title
     )
 ```
 """
-REGISTER_TYPE_RENDERER   = prefix("register_type_renderer")
 
 
+REGISTER_FIELD_RENDERER  = prefix("register_field_renderer")
 """
 ### wagtail_fedit.register_field_renderer
 Register a custom renderer for a field.
 
 Example of how this type of renderer is used in wagtail_hooks/renderers.py:
 
 ```python
@@ -68,17 +69,17 @@
 
     # This is a custom renderer for RichText fields.
     # It will render the RichText field as a RichText block.
     renderer_map[RichTextField] =\
         lambda request, context, instance, value: richtext(value)
 ```
 """
-REGISTER_FIELD_RENDERER  = prefix("register_field_renderer")
 
 
+EXCLUDE_FROM_RELATED_FORMS = prefix("exclude_related_forms")
 """
 ### wagtail_fedit.exclude_related_forms
 Exclude the given model type from the related forms.
 This is used internally to exclude the Page, Image, and Document models from the related forms.
 This way; the user will have the actual widget for the field instead of the related form.
 
 Example of how this hook is called and how it is used internally:
@@ -94,17 +95,17 @@
 @hooks.register(EXCLUDE_FROM_RELATED_FORMS)
 def exclude_related_forms(field):
     if field.related_model in [Page, Image, Document]:
         return True
     return False
 ```
 """
-EXCLUDE_FROM_RELATED_FORMS = prefix("exclude_related_forms")
 
 
+ACTION_MENU_ITEM_IS_SHOWN = prefix("action_menu_item_is_shown")
 """
 ### wagtail_fedit.action_menu_item_is_shown
 Decide if the action menu item should be shown for the given instance.
 
 Return None if you cannot decide, False if you want to hide the item, and True if you want to show the item.
 
 Example of how this hook is called:
@@ -112,8 +113,7 @@
 ```python
 for hook in hooks.get_hooks(ACTION_MENU_ITEM_IS_SHOWN):
     result = hook(context, instance)
     if result is not None:
         return result # <- bool
 ```
 """
-ACTION_MENU_ITEM_IS_SHOWN = prefix("action_menu_item_is_shown")
```

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/models.py` & `wagtail_fedit-1.4.3/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html` & `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html` & `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html` & `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.4.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,35 +1,35 @@
 magic:    0xa70d0d0a
-moddate:  0xda4d1466 (Mon Apr  8 20:04:42 2024 UTC)
-files sz: 15230
+moddate:  0x4c6e1666 (Wed Apr 10 10:47:40 2024 UTC)
+files sz: 14527
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
       055a050100640064036c066d075a076d085a080100640064046c066d095a
       090100640064056c0a6d0b5a0b0100640064066c0c6d0d5a0d0100640064
       076c0e6d0f5a0f0100640064086c106d115a110100640064096c126d135a
       1301006400640a6c146d155a1501006400640b6c166d175a170100640064
-      0c6c186d195a1901006400640d6c1a5a1a640e640f6c1b6d1c5a1c6d1d5a
-      1d0100640e64106c1e6d1f5a1f6d205a200100640e64116c176d215a216d
-      225a220100020065016a230000000000000000a6000000ab000000000000
-      0000005a240200650f6a250000000000000000a6000000ab000000000000
-      0000005a2664125a2764135a28020047006414840064156502a6030000ab
-      0300000000000000005a296524a02a000000000000000000000000000000
-      00000000006416ac17a6010000ab01000000000000000064186507641965
-      086604641a8404a6000000ab0000000000000000005a2b02004700641b84
-      00641c6502a6030000ab0300000000000000005a2c6524a02a0000000000
-      000000000000000000000000000000641dac17a6010000ab010000000000
-      00000064186507641965086604641e8404a6000000ab0000000000000000
-      005a2d641f84005a2e641865076420652f65301900000000000000000064
-      21652f653019000000000000000000642265316608642384045a32642465
-      116a3300000000000000006602642584045a34642684005a35640d5300
+      0c6c185a18640d640e6c196d1a5a1a6d1b5a1b0100640d640f6c1c6d1d5a
+      1d6d1e5a1e6d1f5a1f6d205a200100640d64106c156d215a216d225a2201
+      00020065016a230000000000000000a6000000ab0000000000000000005a
+      240200650f6a250000000000000000a6000000ab0000000000000000005a
+      2664115a2764125a28020047006413840064146502a6030000ab03000000
+      00000000005a296524a02a00000000000000000000000000000000000000
+      006415ac16a6010000ab0100000000000000006417650764186508660464
+      198404a6000000ab0000000000000000005a2b02004700641a8400641b65
+      02a6030000ab0300000000000000005a2c6524a02a000000000000000000
+      0000000000000000000000641cac16a6010000ab01000000000000000064
+      176507641865086604641d8404a6000000ab0000000000000000005a2d64
+      1e84005a2e641f84005a2f64176507642065306531190000000000000000
+      0064216530653119000000000000000000642265326608642384045a3364
+      0c5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('library', 'Node', 'NodeList'))
                  6 IMPORT_NAME              0 (django.template)
                  8 IMPORT_FROM              1 (library)
                 10 STORE_NAME               1 (library)
@@ -94,198 +94,186 @@
                112 LOAD_CONST               9 (('BoundBlock',))
                114 IMPORT_NAME             18 (wagtail.blocks)
                116 IMPORT_FROM             19 (BoundBlock)
                118 STORE_NAME              19 (BoundBlock)
                120 POP_TOP
    
     11         122 LOAD_CONST               0 (0)
-               124 LOAD_CONST              10 (('Page',))
-               126 IMPORT_NAME             20 (wagtail.models)
-               128 IMPORT_FROM             21 (Page)
-               130 STORE_NAME              21 (Page)
+               124 LOAD_CONST              10 (('hooks',))
+               126 IMPORT_NAME             20 (wagtail)
+               128 IMPORT_FROM             21 (hooks)
+               130 STORE_NAME              21 (hooks)
                132 POP_TOP
    
     12         134 LOAD_CONST               0 (0)
-               136 LOAD_CONST              11 (('hooks',))
-               138 IMPORT_NAME             22 (wagtail)
-               140 IMPORT_FROM             23 (hooks)
-               142 STORE_NAME              23 (hooks)
+               136 LOAD_CONST              11 (('urlencode',))
+               138 IMPORT_NAME             22 (urllib.parse)
+               140 IMPORT_FROM             23 (urlencode)
+               142 STORE_NAME              23 (urlencode)
                144 POP_TOP
    
-    13         146 LOAD_CONST               0 (0)
-               148 LOAD_CONST              12 (('urlencode',))
-               150 IMPORT_NAME             24 (urllib.parse)
-               152 IMPORT_FROM             25 (urlencode)
-               154 STORE_NAME              25 (urlencode)
-               156 POP_TOP
-   
-    15         158 LOAD_CONST               0 (0)
-               160 LOAD_CONST              13 (None)
-               162 IMPORT_NAME             26 (warnings)
-               164 STORE_NAME              26 (warnings)
-   
-    17         166 LOAD_CONST              14 (2)
-               168 LOAD_CONST              15 (('FeditBlockEditButton', 'FeditFieldEditButton'))
-               170 IMPORT_NAME             27 (toolbar)
-               172 IMPORT_FROM             28 (FeditBlockEditButton)
-               174 STORE_NAME              28 (FeditBlockEditButton)
-               176 IMPORT_FROM             29 (FeditFieldEditButton)
-               178 STORE_NAME              29 (FeditFieldEditButton)
-               180 POP_TOP
-   
-    21         182 LOAD_CONST              14 (2)
-               184 LOAD_CONST              16 (('FEDIT_PREVIEW_VAR', 'get_field_content'))
-               186 IMPORT_NAME             30 (utils)
-               188 IMPORT_FROM             31 (FEDIT_PREVIEW_VAR)
-               190 STORE_NAME              31 (FEDIT_PREVIEW_VAR)
-               192 IMPORT_FROM             32 (get_field_content)
-               194 STORE_NAME              32 (get_field_content)
-               196 POP_TOP
-   
-    22         198 LOAD_CONST              14 (2)
-               200 LOAD_CONST              17 (('CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR'))
-               202 IMPORT_NAME             23 (hooks)
-               204 IMPORT_FROM             33 (CONSTRUCT_BLOCK_TOOLBAR)
-               206 STORE_NAME              33 (CONSTRUCT_BLOCK_TOOLBAR)
-               208 IMPORT_FROM             34 (CONSTRUCT_FIELD_TOOLBAR)
-               210 STORE_NAME              34 (CONSTRUCT_FIELD_TOOLBAR)
-               212 POP_TOP
-   
-    28         214 PUSH_NULL
-               216 LOAD_NAME                1 (library)
-               218 LOAD_ATTR               35 (Library)
-               228 PRECALL                  0
-               232 CALL                     0
-               242 STORE_NAME              36 (register)
-   
-    29         244 PUSH_NULL
-               246 LOAD_NAME               15 (signing)
-               248 LOAD_ATTR               37 (TimestampSigner)
-               258 PRECALL                  0
-               262 CALL                     0
-               272 STORE_NAME              38 (url_value_signer)
-   
-    32         274 LOAD_CONST              18 ('Field name is not available in the context for %(object)s.')
-               276 STORE_NAME              39 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-   
-    33         278 LOAD_CONST              19 ('Model instance is not available in the context for %(object)s.')
-               280 STORE_NAME              40 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-   
-    36         282 PUSH_NULL
-               284 LOAD_BUILD_CLASS
-               286 LOAD_CONST              20 (<code object BlockEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 36>)
-               288 MAKE_FUNCTION            0
-               290 LOAD_CONST              21 ('BlockEditNode')
-               292 LOAD_NAME                2 (Node)
-               294 PRECALL                  3
-               298 CALL                     3
-               308 STORE_NAME              41 (BlockEditNode)
-   
-   231         310 LOAD_NAME               36 (register)
-               312 LOAD_METHOD             42 (tag)
-               334 LOAD_CONST              22 ('fedit_block')
-               336 KW_NAMES                23
-               338 PRECALL                  1
-               342 CALL                     1
-   
-   232         352 LOAD_CONST              24 ('parser')
-               354 LOAD_NAME                7 (Parser)
-               356 LOAD_CONST              25 ('token')
-               358 LOAD_NAME                8 (Token)
-               360 BUILD_TUPLE              4
-               362 LOAD_CONST              26 (<code object do_render_fedit_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 231>)
-               364 MAKE_FUNCTION            4 (annotations)
-   
-   231         366 PRECALL                  0
-               370 CALL                     0
-   
-   232         380 STORE_NAME              43 (do_render_fedit_block)
-   
-   291         382 PUSH_NULL
-               384 LOAD_BUILD_CLASS
-               386 LOAD_CONST              27 (<code object FieldEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 291>)
-               388 MAKE_FUNCTION            0
-               390 LOAD_CONST              28 ('FieldEditNode')
-               392 LOAD_NAME                2 (Node)
-               394 PRECALL                  3
-               398 CALL                     3
-               408 STORE_NAME              44 (FieldEditNode)
-   
-   344         410 LOAD_NAME               36 (register)
-               412 LOAD_METHOD             42 (tag)
-               434 LOAD_CONST              29 ('fedit_field')
-               436 KW_NAMES                23
-               438 PRECALL                  1
-               442 CALL                     1
-   
-   345         452 LOAD_CONST              24 ('parser')
-               454 LOAD_NAME                7 (Parser)
-               456 LOAD_CONST              25 ('token')
-               458 LOAD_NAME                8 (Token)
-               460 BUILD_TUPLE              4
-               462 LOAD_CONST              30 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 344>)
-               464 MAKE_FUNCTION            4 (annotations)
-   
-   344         466 PRECALL                  0
-               470 CALL                     0
-   
-   345         480 STORE_NAME              45 (do_render_fedit_field)
-   
-   387         482 LOAD_CONST              31 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 387>)
-               484 MAKE_FUNCTION            0
-               486 STORE_NAME              46 (render_editable_field)
-   
-   426         488 LOAD_CONST              24 ('parser')
-               490 LOAD_NAME                7 (Parser)
-               492 LOAD_CONST              32 ('kwarg_list')
-               494 LOAD_NAME               47 (list)
-               496 LOAD_NAME               48 (str)
-               498 BINARY_SUBSCR
-               508 LOAD_CONST              33 ('tokens')
-               510 LOAD_NAME               47 (list)
-               512 LOAD_NAME               48 (str)
-               514 BINARY_SUBSCR
-               524 LOAD_CONST              34 ('return')
-               526 LOAD_NAME               49 (dict)
-               528 BUILD_TUPLE              8
-               530 LOAD_CONST              35 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 426>)
-               532 MAKE_FUNCTION            4 (annotations)
-               534 STORE_NAME              50 (get_kwargs)
-   
-   451         536 LOAD_CONST              36 ('obj')
-               538 LOAD_NAME               17 (models)
-               540 LOAD_ATTR               51 (Model)
-               550 BUILD_TUPLE              2
-               552 LOAD_CONST              37 (<code object _can_edit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 451>)
-               554 MAKE_FUNCTION            4 (annotations)
-               556 STORE_NAME              52 (_can_edit)
-   
-   463         558 LOAD_CONST              38 (<code object _get_from_context_or_set, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 463>)
-               560 MAKE_FUNCTION            0
-               562 STORE_NAME              53 (_get_from_context_or_set)
-               564 LOAD_CONST              13 (None)
-               566 RETURN_VALUE
+    14         146 LOAD_CONST               0 (0)
+               148 LOAD_CONST              12 (None)
+               150 IMPORT_NAME             24 (warnings)
+               152 STORE_NAME              24 (warnings)
+   
+    16         154 LOAD_CONST              13 (2)
+               156 LOAD_CONST              14 (('FeditBlockEditButton', 'FeditFieldEditButton'))
+               158 IMPORT_NAME             25 (toolbar)
+               160 IMPORT_FROM             26 (FeditBlockEditButton)
+               162 STORE_NAME              26 (FeditBlockEditButton)
+               164 IMPORT_FROM             27 (FeditFieldEditButton)
+               166 STORE_NAME              27 (FeditFieldEditButton)
+               168 POP_TOP
+   
+    20         170 LOAD_CONST              13 (2)
+               172 LOAD_CONST              15 (('_can_edit', 'edit_url', 'get_field_content', '_resolve_expressions'))
+               174 IMPORT_NAME             28 (utils)
+               176 IMPORT_FROM             29 (_can_edit)
+               178 STORE_NAME              29 (_can_edit)
+               180 IMPORT_FROM             30 (edit_url)
+               182 STORE_NAME              30 (edit_url)
+               184 IMPORT_FROM             31 (get_field_content)
+               186 STORE_NAME              31 (get_field_content)
+               188 IMPORT_FROM             32 (_resolve_expressions)
+               190 STORE_NAME              32 (_resolve_expressions)
+               192 POP_TOP
+   
+    26         194 LOAD_CONST              13 (2)
+               196 LOAD_CONST              16 (('CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR'))
+               198 IMPORT_NAME             21 (hooks)
+               200 IMPORT_FROM             33 (CONSTRUCT_BLOCK_TOOLBAR)
+               202 STORE_NAME              33 (CONSTRUCT_BLOCK_TOOLBAR)
+               204 IMPORT_FROM             34 (CONSTRUCT_FIELD_TOOLBAR)
+               206 STORE_NAME              34 (CONSTRUCT_FIELD_TOOLBAR)
+               208 POP_TOP
+   
+    32         210 PUSH_NULL
+               212 LOAD_NAME                1 (library)
+               214 LOAD_ATTR               35 (Library)
+               224 PRECALL                  0
+               228 CALL                     0
+               238 STORE_NAME              36 (register)
+   
+    33         240 PUSH_NULL
+               242 LOAD_NAME               15 (signing)
+               244 LOAD_ATTR               37 (TimestampSigner)
+               254 PRECALL                  0
+               258 CALL                     0
+               268 STORE_NAME              38 (url_value_signer)
+   
+    36         270 LOAD_CONST              17 ('Field name is not available in the context for %(object)s.')
+               272 STORE_NAME              39 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+   
+    37         274 LOAD_CONST              18 ('Model instance is not available in the context for %(object)s.')
+               276 STORE_NAME              40 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+   
+    40         278 PUSH_NULL
+               280 LOAD_BUILD_CLASS
+               282 LOAD_CONST              19 (<code object BlockEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 40>)
+               284 MAKE_FUNCTION            0
+               286 LOAD_CONST              20 ('BlockEditNode')
+               288 LOAD_NAME                2 (Node)
+               290 PRECALL                  3
+               294 CALL                     3
+               304 STORE_NAME              41 (BlockEditNode)
+   
+   196         306 LOAD_NAME               36 (register)
+               308 LOAD_METHOD             42 (tag)
+               330 LOAD_CONST              21 ('fedit_block')
+               332 KW_NAMES                22
+               334 PRECALL                  1
+               338 CALL                     1
+   
+   197         348 LOAD_CONST              23 ('parser')
+               350 LOAD_NAME                7 (Parser)
+               352 LOAD_CONST              24 ('token')
+               354 LOAD_NAME                8 (Token)
+               356 BUILD_TUPLE              4
+               358 LOAD_CONST              25 (<code object do_render_fedit_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 196>)
+               360 MAKE_FUNCTION            4 (annotations)
+   
+   196         362 PRECALL                  0
+               366 CALL                     0
+   
+   197         376 STORE_NAME              43 (do_render_fedit_block)
+   
+   256         378 PUSH_NULL
+               380 LOAD_BUILD_CLASS
+               382 LOAD_CONST              26 (<code object FieldEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 256>)
+               384 MAKE_FUNCTION            0
+               386 LOAD_CONST              27 ('FieldEditNode')
+               388 LOAD_NAME                2 (Node)
+               390 PRECALL                  3
+               394 CALL                     3
+               404 STORE_NAME              44 (FieldEditNode)
+   
+   315         406 LOAD_NAME               36 (register)
+               408 LOAD_METHOD             42 (tag)
+               430 LOAD_CONST              28 ('fedit_field')
+               432 KW_NAMES                22
+               434 PRECALL                  1
+               438 CALL                     1
+   
+   316         448 LOAD_CONST              23 ('parser')
+               450 LOAD_NAME                7 (Parser)
+               452 LOAD_CONST              24 ('token')
+               454 LOAD_NAME                8 (Token)
+               456 BUILD_TUPLE              4
+               458 LOAD_CONST              29 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 315>)
+               460 MAKE_FUNCTION            4 (annotations)
+   
+   315         462 PRECALL                  0
+               466 CALL                     0
+   
+   316         476 STORE_NAME              45 (do_render_fedit_field)
+   
+   358         478 LOAD_CONST              30 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 358>)
+               480 MAKE_FUNCTION            0
+               482 STORE_NAME              46 (render_editable_field)
+   
+   397         484 LOAD_CONST              31 (<code object render_editable_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 397>)
+               486 MAKE_FUNCTION            0
+               488 STORE_NAME              47 (render_editable_block)
+   
+   435         490 LOAD_CONST              23 ('parser')
+               492 LOAD_NAME                7 (Parser)
+               494 LOAD_CONST              32 ('kwarg_list')
+               496 LOAD_NAME               48 (list)
+               498 LOAD_NAME               49 (str)
+               500 BINARY_SUBSCR
+               510 LOAD_CONST              33 ('tokens')
+               512 LOAD_NAME               48 (list)
+               514 LOAD_NAME               49 (str)
+               516 BINARY_SUBSCR
+               526 LOAD_CONST              34 ('return')
+               528 LOAD_NAME               50 (dict)
+               530 BUILD_TUPLE              8
+               532 LOAD_CONST              35 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 435>)
+               534 MAKE_FUNCTION            4 (annotations)
+               536 STORE_NAME              51 (get_kwargs)
+               538 LOAD_CONST              12 (None)
+               540 RETURN_VALUE
    consts
       0
       ('library', 'Node', 'NodeList')
       ('render_to_string',)
       ('Parser', 'Token')
       ('FilterExpression',)
       ('mark_safe',)
       ('reverse',)
       ('signing',)
       ('models',)
       ('BoundBlock',)
-      ('Page',)
       ('hooks',)
       ('urlencode',)
       None
       2
       ('FeditBlockEditButton', 'FeditFieldEditButton')
-      ('FEDIT_PREVIEW_VAR', 'get_field_content')
+      ('_can_edit', 'edit_url', 'get_field_content', '_resolve_expressions')
       ('CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR')
       'Field name is not available in the context for %(object)s.'
       'Model instance is not available in the context for %(object)s.'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
@@ -295,149 +283,149 @@
             000000000000005a04090009000900090009006412640465056405650664
             06650764076507640865086a090000000000000000660a640984055a0a64
             0a84005a0b650c640b650d6602640c8404a6000000ab0000000000000000
             005a0e650f6403640d9c01640e6507640b650d6604640f8406a6000000ab
             0000000000000000005a10650c6406650764076507641065086a09000000
             0000000000640b6507660864118404a6000000ab0000000000000000005a
             1164035300
-          36           0 RESUME                   0
+          40           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BlockEditNode')
                        8 STORE_NAME               2 (__qualname__)
          
-          37          10 PUSH_NULL
+          41          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object UnpackError, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 37>)
+                      14 LOAD_CONST               1 (<code object UnpackError, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 41>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('UnpackError')
                       20 LOAD_NAME                3 (Exception)
                       22 PRECALL                  3
                       26 CALL                     3
                       36 STORE_NAME               4 (UnpackError)
          
-          41          38 NOP
+          45          38 NOP
          
-          42          40 NOP
+          46          40 NOP
          
-          43          42 NOP
+          47          42 NOP
          
-          44          44 NOP
+          48          44 NOP
          
-          45          46 NOP
+          49          46 NOP
          
-          40          48 LOAD_CONST              18 ((None, None, None, None, None))
+          44          48 LOAD_CONST              18 ((None, None, None, None, None))
                       50 LOAD_CONST               4 ('nodelist')
          
-          41          52 LOAD_NAME                5 (NodeList)
+          45          52 LOAD_NAME                5 (NodeList)
          
-          40          54 LOAD_CONST               5 ('block')
+          44          54 LOAD_CONST               5 ('block')
          
-          42          56 LOAD_NAME                6 (BoundBlock)
+          46          56 LOAD_NAME                6 (BoundBlock)
          
-          40          58 LOAD_CONST               6 ('block_id')
+          44          58 LOAD_CONST               6 ('block_id')
          
-          43          60 LOAD_NAME                7 (str)
+          47          60 LOAD_NAME                7 (str)
          
-          40          62 LOAD_CONST               7 ('field_name')
+          44          62 LOAD_CONST               7 ('field_name')
          
-          44          64 LOAD_NAME                7 (str)
+          48          64 LOAD_NAME                7 (str)
          
-          40          66 LOAD_CONST               8 ('model')
+          44          66 LOAD_CONST               8 ('model')
          
-          45          68 LOAD_NAME                8 (models)
+          49          68 LOAD_NAME                8 (models)
                       70 LOAD_ATTR                9 (Model)
          
-          40          80 BUILD_TUPLE             10
-                      82 LOAD_CONST               9 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 40>)
+          44          80 BUILD_TUPLE             10
+                      82 LOAD_CONST               9 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 44>)
                       84 MAKE_FUNCTION            5 (defaults, annotations)
                       86 STORE_NAME              10 (__init__)
          
-          56          88 LOAD_CONST              10 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 56>)
+          60          88 LOAD_CONST              10 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 60>)
                       90 MAKE_FUNCTION            0
                       92 STORE_NAME              11 (render)
          
-         182          94 LOAD_NAME               12 (staticmethod)
+         147          94 LOAD_NAME               12 (staticmethod)
          
-         183          96 LOAD_CONST              11 ('return')
+         148          96 LOAD_CONST              11 ('return')
                       98 LOAD_NAME               13 (dict)
                      100 BUILD_TUPLE              2
-                     102 LOAD_CONST              12 (<code object pack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 182>)
+                     102 LOAD_CONST              12 (<code object pack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 147>)
                      104 MAKE_FUNCTION            4 (annotations)
          
-         182         106 PRECALL                  0
+         147         106 PRECALL                  0
                      110 CALL                     0
          
-         183         120 STORE_NAME              14 (pack)
+         148         120 STORE_NAME              14 (pack)
          
-         191         122 LOAD_NAME               15 (classmethod)
+         156         122 LOAD_NAME               15 (classmethod)
          
-         192         124 LOAD_CONST               3 (None)
+         157         124 LOAD_CONST               3 (None)
                      126 LOAD_CONST              13 (('request',))
                      128 BUILD_CONST_KEY_MAP      1
                      130 LOAD_CONST              14 ('expected')
                      132 LOAD_NAME                7 (str)
                      134 LOAD_CONST              11 ('return')
                      136 LOAD_NAME               13 (dict)
                      138 BUILD_TUPLE              4
-                     140 LOAD_CONST              15 (<code object unpack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 191>)
+                     140 LOAD_CONST              15 (<code object unpack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 156>)
                      142 MAKE_FUNCTION            6 (kwdefaults, annotations)
          
-         191         144 PRECALL                  0
+         156         144 PRECALL                  0
                      148 CALL                     0
          
-         192         158 STORE_NAME              16 (unpack)
+         157         158 STORE_NAME              16 (unpack)
          
-         214         160 LOAD_NAME               12 (staticmethod)
+         179         160 LOAD_NAME               12 (staticmethod)
          
-         215         162 LOAD_CONST               6 ('block_id')
+         180         162 LOAD_CONST               6 ('block_id')
                      164 LOAD_NAME                7 (str)
                      166 LOAD_CONST               7 ('field_name')
                      168 LOAD_NAME                7 (str)
                      170 LOAD_CONST              16 ('instance')
                      172 LOAD_NAME                8 (models)
                      174 LOAD_ATTR                9 (Model)
                      184 LOAD_CONST              11 ('return')
                      186 LOAD_NAME                7 (str)
                      188 BUILD_TUPLE              8
-                     190 LOAD_CONST              17 (<code object get_edit_url, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 214>)
+                     190 LOAD_CONST              17 (<code object get_edit_url, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 179>)
                      192 MAKE_FUNCTION            4 (annotations)
          
-         214         194 PRECALL                  0
+         179         194 PRECALL                  0
                      198 CALL                     0
          
-         215         208 STORE_NAME              17 (get_edit_url)
+         180         208 STORE_NAME              17 (get_edit_url)
                      210 LOAD_CONST               3 (None)
                      212 RETURN_VALUE
          consts
             'BlockEditNode'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015300
-                37           0 RESUME                   0
+                41           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('BlockEditNode.UnpackError')
                              8 STORE_NAME               2 (__qualname__)
                
-                38          10 LOAD_CONST               1 (None)
+                42          10 LOAD_CONST               1 (None)
                             12 RETURN_VALUE
                consts
                   'BlockEditNode.UnpackError'
                   None
                names      ('__name__', '__module__', '__qualname__')
                varnames   ()
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'UnpackError'
-               firstlineno 37
+               firstlineno 41
                lnotab 0x0a01
             'UnpackError'
             None
             'nodelist'
             'block'
             'block_id'
             'field_name'
@@ -448,746 +436,504 @@
                stacksize : 2
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   007c037c005f0200000000000000007c047c005f0300000000000000007c
                   057c005f0400000000000000007c067c005f050000000000000000640053
                   00
-                40           0 RESUME                   0
+                44           0 RESUME                   0
                
-                49           2 LOAD_FAST                1 (nodelist)
+                53           2 LOAD_FAST                1 (nodelist)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (nl)
                
-                50          16 LOAD_FAST                2 (block)
+                54          16 LOAD_FAST                2 (block)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (block)
                
-                51          30 LOAD_FAST                3 (block_id)
+                55          30 LOAD_FAST                3 (block_id)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (block_id)
                
-                52          44 LOAD_FAST                4 (field_name)
+                56          44 LOAD_FAST                4 (field_name)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (field_name)
                
-                53          58 LOAD_FAST                5 (model)
+                57          58 LOAD_FAST                5 (model)
                             60 LOAD_FAST                0 (self)
                             62 STORE_ATTR               4 (model)
                
-                54          72 LOAD_FAST                6 (extra)
+                58          72 LOAD_FAST                6 (extra)
                             74 LOAD_FAST                0 (self)
                             76 STORE_ATTR               5 (extra)
                             86 LOAD_CONST               0 (None)
                             88 RETURN_VALUE
                consts
                   None
                names      ('nl', 'block', 'block_id', 'field_name', 'model', 'extra')
                varnames   ('self', 'nodelist', 'block', 'block_id', 'field_name', 'model', 'extra')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 40
+               firstlineno 44
                lnotab 0x02090e010e010e010e010e01
             code
                argcount  : 2
-               nlocals   : 13
-               stacksize : 14
+               nlocals   : 12
+               stacksize : 10
                flags     : 3
                code
-                  0x870d870e97007c006a0000000000000000007d027c006a010000000000
-                  0000007d037c006a0200000000000000007d047c006a0300000000000000
-                  008a0d7c006a0400000000000000007d057c05a005000000000000000000
-                  0000000000000000000000a6000000ab00000000000000000044005d325c
-                  0200007d067d07740d000000000000000000007c07740e00000000000000
-                  000000a6020000ab02000000000000000072187c07a00800000000000000
-                  000000000000000000000000007c01a6010000ab0100000000000000007c
-                  057c063c0000008c337c04730c64017c01760072087c0164011900000000
-                  00000000007d04740d000000000000000000007c02740e00000000000000
-                  000000a6020000ab02000000000000000072157c02a00800000000000000
-                  000000000000000000000000007c01a6010000ab0100000000000000007d
-                  02740d000000000000000000007c03740e00000000000000000000a60200
-                  00ab02000000000000000072157c03a00800000000000000000000000000
-                  000000000000007c01a6010000ab0100000000000000007d03740d000000
-                  000000000000007c04740e00000000000000000000a6020000ab02000000
-                  000000000072157c04a00800000000000000000000000000000000000000
-                  007c01a6010000ab0100000000000000007d04740d000000000000000000
-                  00890d740e00000000000000000000a6020000ab02000000000000000072
-                  15890da00800000000000000000000000000000000000000007c01a60100
-                  00ab0100000000000000008a0d7c03731564027c01760172117c02730f74
-                  13000000000000000000006403a6010000ab010000000000000000820189
-                  0d70147c01a00a00000000000000000000000000000000000000006404a6
-                  010000ab0100000000000000008a0d7c047c0164013c000000890d7c0164
-                  043c0000007c02725a09007c01a00b000000000000000000000000000000
-                  0000000000a6000000ab0000000000000000007d086e1223007418000000
-                  000000000000002400720501007c017d0859006e0477007803590077017c
-                  08a00d00000000000000000000000000000000000000007c05a6010000ab
-                  01000000000000000001007c02a00e000000000000000000000000000000
-                  00000000007c08a6010000ab0100000000000000007d0964057c005f0f00
-                  000000000000006e387c006a10000000000000000072227c006a10000000
-                  0000000000a01100000000000000000000000000000000000000007c01a6
-                  010000ab0100000000000000007d0964067c005f0f00000000000000006e
-                  0f7413000000000000000000006407a6010000ab01000000000000000082
-                  017c0473257425000000000000000000006a130000000000000000742800
-                  00000000000000000064087c016a15000000000000000069017a060000a6
-                  010000ab01000000000000000001007c095300890d732f74250000000000
-                  00000000006a130000000000000000742c0000000000000000000064087c
-                  026a0000000000000000006a1700000000000000006a1800000000000000
-                  0069017a060000a6010000ab01000000000000000001007c0953007c0373
-                  0d64027c01760072097c016402190000000000000000007d036e2d7c0373
-                  1a7c0272187433000000000000000000007c026409a6020000ab02000000
-                  000000000072087c026a1a00000000000000007d036e117c03730f741300
-                  0000000000000000006403a6010000ab01000000000000000082017c0973
-                  0f743700000000000000000000640aa6010000ab0100000000000000007d
-                  097c01a00a0000000000000000000000000000000000000000640ba60100
-                  00ab0100000000000000008a0e743900000000000000000000890e890da6
-                  020000ab02000000000000000073027c095300740d000000000000000000
-                  00890d743a00000000000000000000a6020000ab02000000000000000072
-                  1d743d000000000000000000007c01640c880d6601640d8408a6030000ab
-                  0300000000000000007d0a7c0a9b00640e7c039b00640f9d047d0a6e0264
-                  007d0a7c006a0f00000000000000007c0564103c000000743f0000000000
-                  0000000000a6000000ab00000000000000000067017d0b74410000000000
-                  00000000006a210000000000000000744400000000000000000000a60100
-                  00ab01000000000000000044005d127d0c02007c0c890e7c0b890d7c037c
-                  04ac11a6050000ab05000000000000000001008c13880e6601641284087c
-                  0b4400a6000000ab0000000000000000007d0b7447000000000000000000
-                  0074490000000000000000000064007c0ba6020000ab0200000000000000
-                  00a6010000ab0100000000000000007d0b744b0000000000000000000064
-                  1302007c006a2600000000000000007c037c0466026414890d69017c05a4
-                  018e017c0a7c03890d7c097c047c017c04890d7c0b64159c0aa6020000ab
-                  0200000000000000005300
-                             0 MAKE_CELL               13 (model)
-                             2 MAKE_CELL               14 (request)
-               
-                56           4 RESUME                   0
-               
-                57           6 LOAD_FAST                0 (self)
-                             8 LOAD_ATTR                0 (block)
-                            18 STORE_FAST               2 (block)
-               
-                58          20 LOAD_FAST                0 (self)
-                            22 LOAD_ATTR                1 (block_id)
-                            32 STORE_FAST               3 (block_id)
-               
-                59          34 LOAD_FAST                0 (self)
-                            36 LOAD_ATTR                2 (field_name)
-                            46 STORE_FAST               4 (field_name)
-               
-                60          48 LOAD_FAST                0 (self)
-                            50 LOAD_ATTR                3 (model)
-                            60 STORE_DEREF             13 (model)
-               
-                61          62 LOAD_FAST                0 (self)
-                            64 LOAD_ATTR                4 (extra)
-                            74 STORE_FAST               5 (extra)
-               
-                64          76 LOAD_FAST                5 (extra)
-                            78 LOAD_METHOD              5 (items)
-                           100 PRECALL                  0
-                           104 CALL                     0
-                           114 GET_ITER
-                       >>  116 FOR_ITER                50 (to 218)
-                           118 UNPACK_SEQUENCE          2
-                           122 STORE_FAST               6 (k)
-                           124 STORE_FAST               7 (e)
-               
-                65         126 LOAD_GLOBAL             13 (NULL + isinstance)
-                           138 LOAD_FAST                7 (e)
-                           140 LOAD_GLOBAL             14 (FilterExpression)
-                           152 PRECALL                  2
-                           156 CALL                     2
-                           166 POP_JUMP_FORWARD_IF_FALSE    24 (to 216)
-               
-                66         168 LOAD_FAST                7 (e)
-                           170 LOAD_METHOD              8 (resolve)
-                           192 LOAD_FAST                1 (context)
-                           194 PRECALL                  1
-                           198 CALL                     1
-                           208 LOAD_FAST                5 (extra)
-                           210 LOAD_FAST                6 (k)
-                           212 STORE_SUBSCR
-                       >>  216 JUMP_BACKWARD           51 (to 116)
-               
-                68     >>  218 LOAD_FAST                4 (field_name)
-                           220 POP_JUMP_FORWARD_IF_TRUE    12 (to 246)
-                           222 LOAD_CONST               1 ('wagtail_fedit_field_name')
-                           224 LOAD_FAST                1 (context)
-                           226 CONTAINS_OP              0
-                           228 POP_JUMP_FORWARD_IF_FALSE     8 (to 246)
-               
-                69         230 LOAD_FAST                1 (context)
-                           232 LOAD_CONST               1 ('wagtail_fedit_field_name')
-                           234 BINARY_SUBSCR
-                           244 STORE_FAST               4 (field_name)
-               
-                71     >>  246 LOAD_GLOBAL             13 (NULL + isinstance)
-                           258 LOAD_FAST                2 (block)
-                           260 LOAD_GLOBAL             14 (FilterExpression)
-                           272 PRECALL                  2
-                           276 CALL                     2
-                           286 POP_JUMP_FORWARD_IF_FALSE    21 (to 330)
-               
-                72         288 LOAD_FAST                2 (block)
-                           290 LOAD_METHOD              8 (resolve)
-                           312 LOAD_FAST                1 (context)
-                           314 PRECALL                  1
-                           318 CALL                     1
-                           328 STORE_FAST               2 (block)
-               
-                73     >>  330 LOAD_GLOBAL             13 (NULL + isinstance)
-                           342 LOAD_FAST                3 (block_id)
-                           344 LOAD_GLOBAL             14 (FilterExpression)
-                           356 PRECALL                  2
-                           360 CALL                     2
-                           370 POP_JUMP_FORWARD_IF_FALSE    21 (to 414)
-               
-                74         372 LOAD_FAST                3 (block_id)
-                           374 LOAD_METHOD              8 (resolve)
-                           396 LOAD_FAST                1 (context)
-                           398 PRECALL                  1
-                           402 CALL                     1
-                           412 STORE_FAST               3 (block_id)
-               
-                75     >>  414 LOAD_GLOBAL             13 (NULL + isinstance)
-                           426 LOAD_FAST                4 (field_name)
-                           428 LOAD_GLOBAL             14 (FilterExpression)
-                           440 PRECALL                  2
-                           444 CALL                     2
-                           454 POP_JUMP_FORWARD_IF_FALSE    21 (to 498)
-               
-                76         456 LOAD_FAST                4 (field_name)
-                           458 LOAD_METHOD              8 (resolve)
-                           480 LOAD_FAST                1 (context)
-                           482 PRECALL                  1
-                           486 CALL                     1
-                           496 STORE_FAST               4 (field_name)
-               
-                77     >>  498 LOAD_GLOBAL             13 (NULL + isinstance)
-                           510 LOAD_DEREF              13 (model)
-                           512 LOAD_GLOBAL             14 (FilterExpression)
-                           524 PRECALL                  2
-                           528 CALL                     2
-                           538 POP_JUMP_FORWARD_IF_FALSE    21 (to 582)
-               
-                78         540 LOAD_DEREF              13 (model)
-                           542 LOAD_METHOD              8 (resolve)
-                           564 LOAD_FAST                1 (context)
-                           566 PRECALL                  1
-                           570 CALL                     1
-                           580 STORE_DEREF             13 (model)
-               
-                80     >>  582 LOAD_FAST                3 (block_id)
-                           584 POP_JUMP_FORWARD_IF_TRUE    21 (to 628)
-                           586 LOAD_CONST               2 ('block_id')
-                           588 LOAD_FAST                1 (context)
-                           590 CONTAINS_OP              1
-                           592 POP_JUMP_FORWARD_IF_FALSE    17 (to 628)
-                           594 LOAD_FAST                2 (block)
-                           596 POP_JUMP_FORWARD_IF_TRUE    15 (to 628)
-               
-                81         598 LOAD_GLOBAL             19 (NULL + ValueError)
-                           610 LOAD_CONST               3 ('Block ID is required')
-                           612 PRECALL                  1
-                           616 CALL                     1
-                           626 RAISE_VARARGS            1
+                  0x97007c006a0000000000000000007d027c006a0100000000000000007d
+                  037c006a0200000000000000007d047c006a0300000000000000007d057c
+                  006a0400000000000000007d067c06a00500000000000000000000000000
+                  00000000000000a6000000ab00000000000000000044005d325c0200007d
+                  077d08740d000000000000000000007c08740e00000000000000000000a6
+                  020000ab02000000000000000072187c08a0080000000000000000000000
+                  0000000000000000007c01a6010000ab0100000000000000007c067c073c
+                  0000008c337c04730c64017c01760072087c016401190000000000000000
+                  007d047413000000000000000000007c017c027c037c047c05a6050000ab
+                  0500000000000000005c0400007d027d037d047d057c03731564027c0176
+                  0172117c02730f7415000000000000000000006403a6010000ab01000000
+                  000000000082017c0570147c01a00b000000000000000000000000000000
+                  00000000006404a6010000ab0100000000000000007d057c047c0164013c
+                  0000007c057c0164043c0000007c02725a09007c01a00c00000000000000
+                  00000000000000000000000000a6000000ab0000000000000000007d096e
+                  122300741a000000000000000000002400720501007c017d0959006e0477
+                  007803590077017c09a00e00000000000000000000000000000000000000
+                  007c06a6010000ab01000000000000000001007c02a00f00000000000000
+                  000000000000000000000000007c09a6010000ab0100000000000000007d
+                  0a64057c005f1000000000000000006e387c006a11000000000000000072
+                  227c006a110000000000000000a012000000000000000000000000000000
+                  00000000007c01a6010000ab0100000000000000007d0a64067c005f1000
+                  000000000000006e0f7415000000000000000000006407a6010000ab0100
+                  0000000000000082017c0473257427000000000000000000006a14000000
+                  0000000000742a0000000000000000000064087c016a1600000000000000
+                  0069017a060000a6010000ab01000000000000000001007c0a53007c0573
+                  2f7427000000000000000000006a140000000000000000742e0000000000
+                  000000000064087c026a0000000000000000006a1800000000000000006a
+                  19000000000000000069017a060000a6010000ab01000000000000000001
+                  007c0a53007c03730d64027c01760072097c016402190000000000000000
+                  007d036e2d7c03731a7c0272187435000000000000000000007c026409a6
+                  020000ab02000000000000000072087c026a1b00000000000000007d036e
+                  117c03730f7415000000000000000000006403a6010000ab010000000000
+                  00000082017c0a730f743900000000000000000000640aa6010000ab0100
+                  000000000000007d0a7c01a00b0000000000000000000000000000000000
+                  000000640ba6010000ab0100000000000000007d0b743b00000000000000
+                  0000007c0b7c05a6020000ab02000000000000000073027c0a53007c006a
+                  100000000000000000720a7c006a1000000000000000007c06640c3c0000
+                  00743d00000000000000000000640e7c0b7c0a7c037c047c057c01640d9c
+                  067c06a4018e015300
+                60           0 RESUME                   0
+               
+                61           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (block)
+                            14 STORE_FAST               2 (block)
+               
+                62          16 LOAD_FAST                0 (self)
+                            18 LOAD_ATTR                1 (block_id)
+                            28 STORE_FAST               3 (block_id)
+               
+                63          30 LOAD_FAST                0 (self)
+                            32 LOAD_ATTR                2 (field_name)
+                            42 STORE_FAST               4 (field_name)
+               
+                64          44 LOAD_FAST                0 (self)
+                            46 LOAD_ATTR                3 (model)
+                            56 STORE_FAST               5 (model)
+               
+                65          58 LOAD_FAST                0 (self)
+                            60 LOAD_ATTR                4 (extra)
+                            70 STORE_FAST               6 (extra)
+               
+                68          72 LOAD_FAST                6 (extra)
+                            74 LOAD_METHOD              5 (items)
+                            96 PRECALL                  0
+                           100 CALL                     0
+                           110 GET_ITER
+                       >>  112 FOR_ITER                50 (to 214)
+                           114 UNPACK_SEQUENCE          2
+                           118 STORE_FAST               7 (k)
+                           120 STORE_FAST               8 (e)
+               
+                69         122 LOAD_GLOBAL             13 (NULL + isinstance)
+                           134 LOAD_FAST                8 (e)
+                           136 LOAD_GLOBAL             14 (FilterExpression)
+                           148 PRECALL                  2
+                           152 CALL                     2
+                           162 POP_JUMP_FORWARD_IF_FALSE    24 (to 212)
+               
+                70         164 LOAD_FAST                8 (e)
+                           166 LOAD_METHOD              8 (resolve)
+                           188 LOAD_FAST                1 (context)
+                           190 PRECALL                  1
+                           194 CALL                     1
+                           204 LOAD_FAST                6 (extra)
+                           206 LOAD_FAST                7 (k)
+                           208 STORE_SUBSCR
+                       >>  212 JUMP_BACKWARD           51 (to 112)
+               
+                72     >>  214 LOAD_FAST                4 (field_name)
+                           216 POP_JUMP_FORWARD_IF_TRUE    12 (to 242)
+                           218 LOAD_CONST               1 ('wagtail_fedit_field_name')
+                           220 LOAD_FAST                1 (context)
+                           222 CONTAINS_OP              0
+                           224 POP_JUMP_FORWARD_IF_FALSE     8 (to 242)
+               
+                73         226 LOAD_FAST                1 (context)
+                           228 LOAD_CONST               1 ('wagtail_fedit_field_name')
+                           230 BINARY_SUBSCR
+                           240 STORE_FAST               4 (field_name)
+               
+                76     >>  242 LOAD_GLOBAL             19 (NULL + _resolve_expressions)
+                           254 LOAD_FAST                1 (context)
+                           256 LOAD_FAST                2 (block)
+                           258 LOAD_FAST                3 (block_id)
+                           260 LOAD_FAST                4 (field_name)
+                           262 LOAD_FAST                5 (model)
+                           264 PRECALL                  5
+                           268 CALL                     5
+               
+                75         278 UNPACK_SEQUENCE          4
+                           282 STORE_FAST               2 (block)
+                           284 STORE_FAST               3 (block_id)
+                           286 STORE_FAST               4 (field_name)
+                           288 STORE_FAST               5 (model)
+               
+                78         290 LOAD_FAST                3 (block_id)
+                           292 POP_JUMP_FORWARD_IF_TRUE    21 (to 336)
+                           294 LOAD_CONST               2 ('block_id')
+                           296 LOAD_FAST                1 (context)
+                           298 CONTAINS_OP              1
+                           300 POP_JUMP_FORWARD_IF_FALSE    17 (to 336)
+                           302 LOAD_FAST                2 (block)
+                           304 POP_JUMP_FORWARD_IF_TRUE    15 (to 336)
+               
+                79         306 LOAD_GLOBAL             21 (NULL + ValueError)
+                           318 LOAD_CONST               3 ('Block ID is required')
+                           320 PRECALL                  1
+                           324 CALL                     1
+                           334 RAISE_VARARGS            1
+               
+                84     >>  336 LOAD_FAST                5 (model)
+                           338 JUMP_IF_TRUE_OR_POP     20 (to 380)
+                           340 LOAD_FAST                1 (context)
+                           342 LOAD_METHOD             11 (get)
+                           364 LOAD_CONST               4 ('wagtail_fedit_instance')
+                           366 PRECALL                  1
+                           370 CALL                     1
+                       >>  380 STORE_FAST               5 (model)
                
-                86     >>  628 LOAD_DEREF              13 (model)
-                           630 JUMP_IF_TRUE_OR_POP     20 (to 672)
-                           632 LOAD_FAST                1 (context)
-                           634 LOAD_METHOD             10 (get)
-                           656 LOAD_CONST               4 ('wagtail_fedit_instance')
-                           658 PRECALL                  1
-                           662 CALL                     1
-                       >>  672 STORE_DEREF             13 (model)
-               
-                87         674 LOAD_FAST                4 (field_name)
-                           676 LOAD_FAST                1 (context)
-                           678 LOAD_CONST               1 ('wagtail_fedit_field_name')
-                           680 STORE_SUBSCR
-               
-                88         684 LOAD_DEREF              13 (model)
-                           686 LOAD_FAST                1 (context)
-                           688 LOAD_CONST               4 ('wagtail_fedit_instance')
-                           690 STORE_SUBSCR
-               
-                92         694 LOAD_FAST                2 (block)
-                           696 POP_JUMP_FORWARD_IF_FALSE    90 (to 878)
-               
-                93         698 NOP
-               
-                94         700 LOAD_FAST                1 (context)
-                           702 LOAD_METHOD             11 (flatten)
-                           724 PRECALL                  0
-                           728 CALL                     0
-                           738 STORE_FAST               8 (block_context)
-                           740 JUMP_FORWARD            18 (to 778)
-                       >>  742 PUSH_EXC_INFO
-               
-                95         744 LOAD_GLOBAL             24 (AttributeError)
-                           756 CHECK_EXC_MATCH
-                           758 POP_JUMP_FORWARD_IF_FALSE     5 (to 770)
-                           760 POP_TOP
-               
-                96         762 LOAD_FAST                1 (context)
-                           764 STORE_FAST               8 (block_context)
-                           766 POP_EXCEPT
-                           768 JUMP_FORWARD             4 (to 778)
-               
-                95     >>  770 RERAISE                  0
-                       >>  772 COPY                     3
-                           774 POP_EXCEPT
-                           776 RERAISE                  1
-               
-                97     >>  778 LOAD_FAST                8 (block_context)
-                           780 LOAD_METHOD             13 (update)
-                           802 LOAD_FAST                5 (extra)
-                           804 PRECALL                  1
-                           808 CALL                     1
-                           818 POP_TOP
-               
-                98         820 LOAD_FAST                2 (block)
-                           822 LOAD_METHOD             14 (render_as_block)
-                           844 LOAD_FAST                8 (block_context)
-                           846 PRECALL                  1
-                           850 CALL                     1
-                           860 STORE_FAST               9 (rendered)
-               
-                99         862 LOAD_CONST               5 (True)
-                           864 LOAD_FAST                0 (self)
-                           866 STORE_ATTR              15 (has_block)
-                           876 JUMP_FORWARD            56 (to 990)
-               
-               100     >>  878 LOAD_FAST                0 (self)
-                           880 LOAD_ATTR               16 (nl)
-                           890 POP_JUMP_FORWARD_IF_FALSE    34 (to 960)
-               
-               101         892 LOAD_FAST                0 (self)
-                           894 LOAD_ATTR               16 (nl)
-                           904 LOAD_METHOD             17 (render)
-                           926 LOAD_FAST                1 (context)
-                           928 PRECALL                  1
-                           932 CALL                     1
-                           942 STORE_FAST               9 (rendered)
-               
-               102         944 LOAD_CONST               6 (False)
-                           946 LOAD_FAST                0 (self)
-                           948 STORE_ATTR              15 (has_block)
-                           958 JUMP_FORWARD            15 (to 990)
-               
-               104     >>  960 LOAD_GLOBAL             19 (NULL + ValueError)
-                           972 LOAD_CONST               7 ('Block or nodelist is required')
-                           974 PRECALL                  1
-                           978 CALL                     1
-                           988 RAISE_VARARGS            1
-               
-               106     >>  990 LOAD_FAST                4 (field_name)
-                           992 POP_JUMP_FORWARD_IF_TRUE    37 (to 1068)
-               
-               107         994 LOAD_GLOBAL             37 (NULL + warnings)
-                          1006 LOAD_ATTR               19 (warn)
-               
-               108        1016 LOAD_GLOBAL             40 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-               
-               109        1028 LOAD_CONST               8 ('object')
-                          1030 LOAD_FAST                1 (context)
-                          1032 LOAD_ATTR               21 (template_name)
-                          1042 BUILD_MAP                1
-               
-               108        1044 BINARY_OP                6 (%)
-               
-               107        1048 PRECALL                  1
-                          1052 CALL                     1
-                          1062 POP_TOP
-               
-               111        1064 LOAD_FAST                9 (rendered)
-                          1066 RETURN_VALUE
-               
-               113     >> 1068 LOAD_DEREF              13 (model)
-                          1070 POP_JUMP_FORWARD_IF_TRUE    47 (to 1166)
-               
-               114        1072 LOAD_GLOBAL             37 (NULL + warnings)
-                          1084 LOAD_ATTR               19 (warn)
-               
-               115        1094 LOAD_GLOBAL             44 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-               
-               116        1106 LOAD_CONST               8 ('object')
-                          1108 LOAD_FAST                2 (block)
-                          1110 LOAD_ATTR                0 (block)
-                          1120 LOAD_ATTR               23 (__class__)
-                          1130 LOAD_ATTR               24 (__name__)
-                          1140 BUILD_MAP                1
-               
-               115        1142 BINARY_OP                6 (%)
-               
-               114        1146 PRECALL                  1
-                          1150 CALL                     1
-                          1160 POP_TOP
-               
-               118        1162 LOAD_FAST                9 (rendered)
-                          1164 RETURN_VALUE
-               
-               121     >> 1166 LOAD_FAST                3 (block_id)
-                          1168 POP_JUMP_FORWARD_IF_TRUE    13 (to 1196)
-                          1170 LOAD_CONST               2 ('block_id')
-                          1172 LOAD_FAST                1 (context)
-                          1174 CONTAINS_OP              0
-                          1176 POP_JUMP_FORWARD_IF_FALSE     9 (to 1196)
-               
-               122        1178 LOAD_FAST                1 (context)
-                          1180 LOAD_CONST               2 ('block_id')
-                          1182 BINARY_SUBSCR
-                          1192 STORE_FAST               3 (block_id)
-                          1194 JUMP_FORWARD            45 (to 1286)
-               
-               123     >> 1196 LOAD_FAST                3 (block_id)
-                          1198 POP_JUMP_FORWARD_IF_TRUE    26 (to 1252)
-                          1200 LOAD_FAST                2 (block)
-                          1202 POP_JUMP_FORWARD_IF_FALSE    24 (to 1252)
-                          1204 LOAD_GLOBAL             51 (NULL + hasattr)
-                          1216 LOAD_FAST                2 (block)
-                          1218 LOAD_CONST               9 ('id')
-                          1220 PRECALL                  2
-                          1224 CALL                     2
-                          1234 POP_JUMP_FORWARD_IF_FALSE     8 (to 1252)
-               
-               124        1236 LOAD_FAST                2 (block)
-                          1238 LOAD_ATTR               26 (id)
-                          1248 STORE_FAST               3 (block_id)
-                          1250 JUMP_FORWARD            17 (to 1286)
-               
-               125     >> 1252 LOAD_FAST                3 (block_id)
-                          1254 POP_JUMP_FORWARD_IF_TRUE    15 (to 1286)
-               
-               126        1256 LOAD_GLOBAL             19 (NULL + ValueError)
-                          1268 LOAD_CONST               3 ('Block ID is required')
-                          1270 PRECALL                  1
-                          1274 CALL                     1
-                          1284 RAISE_VARARGS            1
-               
-               128     >> 1286 LOAD_FAST                9 (rendered)
-                          1288 POP_JUMP_FORWARD_IF_TRUE    15 (to 1320)
-               
-               129        1290 LOAD_GLOBAL             55 (NULL + mark_safe)
-                          1302 LOAD_CONST              10 ('')
-                          1304 PRECALL                  1
-                          1308 CALL                     1
-                          1318 STORE_FAST               9 (rendered)
-               
-               132     >> 1320 LOAD_FAST                1 (context)
-                          1322 LOAD_METHOD             10 (get)
-                          1344 LOAD_CONST              11 ('request')
-                          1346 PRECALL                  1
-                          1350 CALL                     1
-                          1360 STORE_DEREF             14 (request)
-               
-               133        1362 LOAD_GLOBAL             57 (NULL + _can_edit)
-                          1374 LOAD_DEREF              14 (request)
-                          1376 LOAD_DEREF              13 (model)
-                          1378 PRECALL                  2
-                          1382 CALL                     2
-                          1392 POP_JUMP_FORWARD_IF_TRUE     2 (to 1398)
-               
-               134        1394 LOAD_FAST                9 (rendered)
-                          1396 RETURN_VALUE
-               
-               138     >> 1398 LOAD_GLOBAL             13 (NULL + isinstance)
-                          1410 LOAD_DEREF              13 (model)
-                          1412 LOAD_GLOBAL             58 (Page)
-                          1424 PRECALL                  2
-                          1428 CALL                     2
-                          1438 POP_JUMP_FORWARD_IF_FALSE    29 (to 1498)
-               
-               139        1440 LOAD_GLOBAL             61 (NULL + _get_from_context_or_set)
-               
-               140        1452 LOAD_FAST                1 (context)
-                          1454 LOAD_CONST              12 ('page_base_edit_url')
-               
-               141        1456 LOAD_CLOSURE            13 (model)
-                          1458 BUILD_TUPLE              1
-                          1460 LOAD_CONST              13 (<code object <lambda>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 141>)
-                          1462 MAKE_FUNCTION            8 (closure)
-               
-               139        1464 PRECALL                  3
-                          1468 CALL                     3
-                          1478 STORE_FAST              10 (admin_edit_url)
-               
-               146        1480 LOAD_FAST               10 (admin_edit_url)
-                          1482 FORMAT_VALUE             0
-                          1484 LOAD_CONST              14 ('#block-')
-                          1486 LOAD_FAST                3 (block_id)
-                          1488 FORMAT_VALUE             0
-                          1490 LOAD_CONST              15 ('-section')
-                          1492 BUILD_STRING             4
-                          1494 STORE_FAST              10 (admin_edit_url)
-                          1496 JUMP_FORWARD             2 (to 1502)
-               
-               148     >> 1498 LOAD_CONST               0 (None)
-                          1500 STORE_FAST              10 (admin_edit_url)
-               
-               150     >> 1502 LOAD_FAST                0 (self)
-                          1504 LOAD_ATTR               15 (has_block)
-                          1514 LOAD_FAST                5 (extra)
-                          1516 LOAD_CONST              16 ('has_block')
-                          1518 STORE_SUBSCR
-               
-               153        1522 LOAD_GLOBAL             63 (NULL + FeditBlockEditButton)
-                          1534 PRECALL                  0
-                          1538 CALL                     0
-               
-               152        1548 BUILD_LIST               1
-                          1550 STORE_FAST              11 (items)
-               
-               156        1552 LOAD_GLOBAL             65 (NULL + hooks)
-                          1564 LOAD_ATTR               33 (get_hooks)
-                          1574 LOAD_GLOBAL             68 (CONSTRUCT_BLOCK_TOOLBAR)
-                          1586 PRECALL                  1
-                          1590 CALL                     1
-                          1600 GET_ITER
-                       >> 1602 FOR_ITER                18 (to 1640)
-                          1604 STORE_FAST              12 (hook)
-               
-               157        1606 PUSH_NULL
-                          1608 LOAD_FAST               12 (hook)
-                          1610 LOAD_DEREF              14 (request)
-                          1612 LOAD_FAST               11 (items)
-                          1614 LOAD_DEREF              13 (model)
-                          1616 LOAD_FAST                3 (block_id)
-                          1618 LOAD_FAST                4 (field_name)
-                          1620 KW_NAMES                17
-                          1622 PRECALL                  5
-                          1626 CALL                     5
-                          1636 POP_TOP
-                          1638 JUMP_BACKWARD           19 (to 1602)
-               
-               159     >> 1640 LOAD_CLOSURE            14 (request)
-                          1642 BUILD_TUPLE              1
-                          1644 LOAD_CONST              18 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 159>)
-                          1646 MAKE_FUNCTION            8 (closure)
-                          1648 LOAD_FAST               11 (items)
-                          1650 GET_ITER
-                          1652 PRECALL                  0
-                          1656 CALL                     0
-                          1666 STORE_FAST              11 (items)
-               
-               160        1668 LOAD_GLOBAL             71 (NULL + list)
-                          1680 LOAD_GLOBAL             73 (NULL + filter)
-                          1692 LOAD_CONST               0 (None)
-                          1694 LOAD_FAST               11 (items)
-                          1696 PRECALL                  2
-                          1700 CALL                     2
-                          1710 PRECALL                  1
-                          1714 CALL                     1
-                          1724 STORE_FAST              11 (items)
-               
-               162        1726 LOAD_GLOBAL             75 (NULL + render_to_string)
-               
-               163        1738 LOAD_CONST              19 ('wagtail_fedit/content/editable_block.html')
-               
-               165        1740 PUSH_NULL
-                          1742 LOAD_FAST                0 (self)
-                          1744 LOAD_ATTR               38 (get_edit_url)
-               
-               166        1754 LOAD_FAST                3 (block_id)
-                          1756 LOAD_FAST                4 (field_name)
-               
-               165        1758 BUILD_TUPLE              2
-                          1760 LOAD_CONST              20 ('instance')
-               
-               167        1762 LOAD_DEREF              13 (model)
-               
-               165        1764 BUILD_MAP                1
-               
-               168        1766 LOAD_FAST                5 (extra)
-               
-               165        1768 DICT_MERGE               1
-                          1770 CALL_FUNCTION_EX         1
-               
-               170        1772 LOAD_FAST               10 (admin_edit_url)
-               
-               171        1774 LOAD_FAST                3 (block_id)
-               
-               172        1776 LOAD_DEREF              13 (model)
-               
-               173        1778 LOAD_FAST                9 (rendered)
-               
-               174        1780 LOAD_FAST                4 (field_name)
-               
-               175        1782 LOAD_FAST                1 (context)
-               
-               176        1784 LOAD_FAST                4 (field_name)
-               
-               177        1786 LOAD_DEREF              13 (model)
-               
-               178        1788 LOAD_FAST               11 (items)
-               
-               164        1790 LOAD_CONST              21 (('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items'))
-                          1792 BUILD_CONST_KEY_MAP     10
-               
-               162        1794 PRECALL                  2
-                          1798 CALL                     2
-                          1808 RETURN_VALUE
+                85         382 LOAD_FAST                4 (field_name)
+                           384 LOAD_FAST                1 (context)
+                           386 LOAD_CONST               1 ('wagtail_fedit_field_name')
+                           388 STORE_SUBSCR
+               
+                86         392 LOAD_FAST                5 (model)
+                           394 LOAD_FAST                1 (context)
+                           396 LOAD_CONST               4 ('wagtail_fedit_instance')
+                           398 STORE_SUBSCR
+               
+                90         402 LOAD_FAST                2 (block)
+                           404 POP_JUMP_FORWARD_IF_FALSE    90 (to 586)
+               
+                91         406 NOP
+               
+                92         408 LOAD_FAST                1 (context)
+                           410 LOAD_METHOD             12 (flatten)
+                           432 PRECALL                  0
+                           436 CALL                     0
+                           446 STORE_FAST               9 (block_context)
+                           448 JUMP_FORWARD            18 (to 486)
+                       >>  450 PUSH_EXC_INFO
+               
+                93         452 LOAD_GLOBAL             26 (AttributeError)
+                           464 CHECK_EXC_MATCH
+                           466 POP_JUMP_FORWARD_IF_FALSE     5 (to 478)
+                           468 POP_TOP
+               
+                94         470 LOAD_FAST                1 (context)
+                           472 STORE_FAST               9 (block_context)
+                           474 POP_EXCEPT
+                           476 JUMP_FORWARD             4 (to 486)
+               
+                93     >>  478 RERAISE                  0
+                       >>  480 COPY                     3
+                           482 POP_EXCEPT
+                           484 RERAISE                  1
+               
+                95     >>  486 LOAD_FAST                9 (block_context)
+                           488 LOAD_METHOD             14 (update)
+                           510 LOAD_FAST                6 (extra)
+                           512 PRECALL                  1
+                           516 CALL                     1
+                           526 POP_TOP
+               
+                96         528 LOAD_FAST                2 (block)
+                           530 LOAD_METHOD             15 (render_as_block)
+                           552 LOAD_FAST                9 (block_context)
+                           554 PRECALL                  1
+                           558 CALL                     1
+                           568 STORE_FAST              10 (rendered)
+               
+                97         570 LOAD_CONST               5 (True)
+                           572 LOAD_FAST                0 (self)
+                           574 STORE_ATTR              16 (has_block)
+                           584 JUMP_FORWARD            56 (to 698)
+               
+                98     >>  586 LOAD_FAST                0 (self)
+                           588 LOAD_ATTR               17 (nl)
+                           598 POP_JUMP_FORWARD_IF_FALSE    34 (to 668)
+               
+                99         600 LOAD_FAST                0 (self)
+                           602 LOAD_ATTR               17 (nl)
+                           612 LOAD_METHOD             18 (render)
+                           634 LOAD_FAST                1 (context)
+                           636 PRECALL                  1
+                           640 CALL                     1
+                           650 STORE_FAST              10 (rendered)
+               
+               100         652 LOAD_CONST               6 (False)
+                           654 LOAD_FAST                0 (self)
+                           656 STORE_ATTR              16 (has_block)
+                           666 JUMP_FORWARD            15 (to 698)
+               
+               102     >>  668 LOAD_GLOBAL             21 (NULL + ValueError)
+                           680 LOAD_CONST               7 ('Block or nodelist is required')
+                           682 PRECALL                  1
+                           686 CALL                     1
+                           696 RAISE_VARARGS            1
+               
+               104     >>  698 LOAD_FAST                4 (field_name)
+                           700 POP_JUMP_FORWARD_IF_TRUE    37 (to 776)
+               
+               105         702 LOAD_GLOBAL             39 (NULL + warnings)
+                           714 LOAD_ATTR               20 (warn)
+               
+               106         724 LOAD_GLOBAL             42 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+               
+               107         736 LOAD_CONST               8 ('object')
+                           738 LOAD_FAST                1 (context)
+                           740 LOAD_ATTR               22 (template_name)
+                           750 BUILD_MAP                1
+               
+               106         752 BINARY_OP                6 (%)
+               
+               105         756 PRECALL                  1
+                           760 CALL                     1
+                           770 POP_TOP
+               
+               109         772 LOAD_FAST               10 (rendered)
+                           774 RETURN_VALUE
+               
+               111     >>  776 LOAD_FAST                5 (model)
+                           778 POP_JUMP_FORWARD_IF_TRUE    47 (to 874)
+               
+               112         780 LOAD_GLOBAL             39 (NULL + warnings)
+                           792 LOAD_ATTR               20 (warn)
+               
+               113         802 LOAD_GLOBAL             46 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+               
+               114         814 LOAD_CONST               8 ('object')
+                           816 LOAD_FAST                2 (block)
+                           818 LOAD_ATTR                0 (block)
+                           828 LOAD_ATTR               24 (__class__)
+                           838 LOAD_ATTR               25 (__name__)
+                           848 BUILD_MAP                1
+               
+               113         850 BINARY_OP                6 (%)
+               
+               112         854 PRECALL                  1
+                           858 CALL                     1
+                           868 POP_TOP
+               
+               116         870 LOAD_FAST               10 (rendered)
+                           872 RETURN_VALUE
+               
+               119     >>  874 LOAD_FAST                3 (block_id)
+                           876 POP_JUMP_FORWARD_IF_TRUE    13 (to 904)
+                           878 LOAD_CONST               2 ('block_id')
+                           880 LOAD_FAST                1 (context)
+                           882 CONTAINS_OP              0
+                           884 POP_JUMP_FORWARD_IF_FALSE     9 (to 904)
+               
+               120         886 LOAD_FAST                1 (context)
+                           888 LOAD_CONST               2 ('block_id')
+                           890 BINARY_SUBSCR
+                           900 STORE_FAST               3 (block_id)
+                           902 JUMP_FORWARD            45 (to 994)
+               
+               121     >>  904 LOAD_FAST                3 (block_id)
+                           906 POP_JUMP_FORWARD_IF_TRUE    26 (to 960)
+                           908 LOAD_FAST                2 (block)
+                           910 POP_JUMP_FORWARD_IF_FALSE    24 (to 960)
+                           912 LOAD_GLOBAL             53 (NULL + hasattr)
+                           924 LOAD_FAST                2 (block)
+                           926 LOAD_CONST               9 ('id')
+                           928 PRECALL                  2
+                           932 CALL                     2
+                           942 POP_JUMP_FORWARD_IF_FALSE     8 (to 960)
+               
+               122         944 LOAD_FAST                2 (block)
+                           946 LOAD_ATTR               27 (id)
+                           956 STORE_FAST               3 (block_id)
+                           958 JUMP_FORWARD            17 (to 994)
+               
+               123     >>  960 LOAD_FAST                3 (block_id)
+                           962 POP_JUMP_FORWARD_IF_TRUE    15 (to 994)
+               
+               124         964 LOAD_GLOBAL             21 (NULL + ValueError)
+                           976 LOAD_CONST               3 ('Block ID is required')
+                           978 PRECALL                  1
+                           982 CALL                     1
+                           992 RAISE_VARARGS            1
+               
+               126     >>  994 LOAD_FAST               10 (rendered)
+                           996 POP_JUMP_FORWARD_IF_TRUE    15 (to 1028)
+               
+               127         998 LOAD_GLOBAL             57 (NULL + mark_safe)
+                          1010 LOAD_CONST              10 ('')
+                          1012 PRECALL                  1
+                          1016 CALL                     1
+                          1026 STORE_FAST              10 (rendered)
+               
+               130     >> 1028 LOAD_FAST                1 (context)
+                          1030 LOAD_METHOD             11 (get)
+                          1052 LOAD_CONST              11 ('request')
+                          1054 PRECALL                  1
+                          1058 CALL                     1
+                          1068 STORE_FAST              11 (request)
+               
+               131        1070 LOAD_GLOBAL             59 (NULL + _can_edit)
+                          1082 LOAD_FAST               11 (request)
+                          1084 LOAD_FAST                5 (model)
+                          1086 PRECALL                  2
+                          1090 CALL                     2
+                          1100 POP_JUMP_FORWARD_IF_TRUE     2 (to 1106)
+               
+               132        1102 LOAD_FAST               10 (rendered)
+                          1104 RETURN_VALUE
+               
+               134     >> 1106 LOAD_FAST                0 (self)
+                          1108 LOAD_ATTR               16 (has_block)
+                          1118 POP_JUMP_FORWARD_IF_FALSE    10 (to 1140)
+               
+               135        1120 LOAD_FAST                0 (self)
+                          1122 LOAD_ATTR               16 (has_block)
+                          1132 LOAD_FAST                6 (extra)
+                          1134 LOAD_CONST              12 ('has_block')
+                          1136 STORE_SUBSCR
+               
+               137     >> 1140 LOAD_GLOBAL             61 (NULL + render_editable_block)
+                          1152 LOAD_CONST              14 (())
+               
+               138        1154 LOAD_FAST               11 (request)
+               
+               139        1156 LOAD_FAST               10 (rendered)
+               
+               140        1158 LOAD_FAST                3 (block_id)
+               
+               141        1160 LOAD_FAST                4 (field_name)
+               
+               142        1162 LOAD_FAST                5 (model)
+               
+               143        1164 LOAD_FAST                1 (context)
+               
+               137        1166 LOAD_CONST              13 (('request', 'content', 'block_id', 'field_name', 'model', 'context'))
+                          1168 BUILD_CONST_KEY_MAP      6
+               
+               144        1170 LOAD_FAST                6 (extra)
+               
+               137        1172 DICT_MERGE               1
+                          1174 CALL_FUNCTION_EX         1
+                          1176 RETURN_VALUE
                ExceptionTable:
-                 700 to 738 -> 742 [0]
-                 742 to 764 -> 772 [1] lasti
-                 770 to 770 -> 772 [1] lasti
+                 408 to 446 -> 450 [0]
+                 450 to 472 -> 480 [1] lasti
+                 478 to 478 -> 480 [1] lasti
                consts
                   None
                   'wagtail_fedit_field_name'
                   'block_id'
                   'Block ID is required'
                   'wagtail_fedit_instance'
                   True
                   False
                   'Block or nodelist is required'
                   'object'
                   'id'
                   ''
                   'request'
-                  'page_base_edit_url'
-                  code
-                     argcount  : 0
-                     nlocals   : 0
-                     stacksize : 4
-                     flags     : 19
-                     code
-                        0x95019700740100000000000000000000640189006a0100000000000000
-                        006701ac02a6020000ab0200000000000000005300
-                                   0 COPY_FREE_VARS           1
-                     
-                     141           2 RESUME                   0
-                                   4 LOAD_GLOBAL              1 (NULL + reverse)
-                     
-                     142          16 LOAD_CONST               1 ('wagtailadmin_pages:edit')
-                     
-                     143          18 LOAD_DEREF               0 (model)
-                                  20 LOAD_ATTR                1 (id)
-                                  30 BUILD_LIST               1
-                     
-                     141          32 KW_NAMES                 2
-                                  34 PRECALL                  2
-                                  38 CALL                     2
-                                  48 RETURN_VALUE
-                     consts
-                        None
-                        'wagtailadmin_pages:edit'
-                        ('args',)
-                     names      ('reverse', 'id')
-                     varnames   ()
-                     freevars   ('model',)
-                     cellvars   ()
-                     filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
-                     name       '<lambda>'
-                     firstlineno 141
-                     lnotab 0x100102010efe
-                  '#block-'
-                  '-section'
                   'has_block'
-                  ('request', 'items', 'model', 'block_id', 'field_name')
-                  code
-                     argcount  : 1
-                     nlocals   : 2
-                     stacksize : 5
-                     flags     : 19
-                     code
-                        0x9501970067007c005d177d017c01a00000000000000000000000000000
-                        000000000000008902a6010000ab01000000000000000091028c185300
-                                   0 COPY_FREE_VARS           1
-                     
-                     159           2 RESUME                   0
-                                   4 BUILD_LIST               0
-                                   6 LOAD_FAST                0 (.0)
-                             >>    8 FOR_ITER                23 (to 56)
-                                  10 STORE_FAST               1 (item)
-                                  12 LOAD_FAST                1 (item)
-                                  14 LOAD_METHOD              0 (render)
-                                  36 LOAD_DEREF               2 (request)
-                                  38 PRECALL                  1
-                                  42 CALL                     1
-                                  52 LIST_APPEND              2
-                                  54 JUMP_BACKWARD           24 (to 8)
-                             >>   56 RETURN_VALUE
-                     consts
-                     names      ('render',)
-                     varnames   ('.0', 'item')
-                     freevars   ('request',)
-                     cellvars   ()
-                     filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
-                     name       '<listcomp>'
-                     firstlineno 159
-                     lnotab 0x
-                  'wagtail_fedit/content/editable_block.html'
-                  'instance'
-                  ('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items')
-               names      ('block', 'block_id', 'field_name', 'model', 'extra', 'items', 'isinstance', 'FilterExpression', 'resolve', 'ValueError', 'get', 'flatten', 'AttributeError', 'update', 'render_as_block', 'has_block', 'nl', 'render', 'warnings', 'warn', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'template_name', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__class__', '__name__', 'hasattr', 'id', 'mark_safe', '_can_edit', 'Page', '_get_from_context_or_set', 'FeditBlockEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_BLOCK_TOOLBAR', 'list', 'filter', 'render_to_string', 'get_edit_url')
-               varnames   ('self', 'context', 'block', 'block_id', 'field_name', 'extra', 'k', 'e', 'block_context', 'rendered', 'admin_edit_url', 'items', 'hook')
+                  ('request', 'content', 'block_id', 'field_name', 'model', 'context')
+                  ()
+               names      ('block', 'block_id', 'field_name', 'model', 'extra', 'items', 'isinstance', 'FilterExpression', 'resolve', '_resolve_expressions', 'ValueError', 'get', 'flatten', 'AttributeError', 'update', 'render_as_block', 'has_block', 'nl', 'render', 'warnings', 'warn', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'template_name', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__class__', '__name__', 'hasattr', 'id', 'mark_safe', '_can_edit', 'render_editable_block')
+               varnames   ('self', 'context', 'block', 'block_id', 'field_name', 'model', 'extra', 'k', 'e', 'block_context', 'rendered', 'request')
                freevars   ()
-               cellvars   ('model', 'request')
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               cellvars   ()
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 56
+               firstlineno 60
                lnotab
-                  0x06010e010e010e010e010e0332012a0132020c0110022a012a012a012a
-                  012a012a012a012a0210011e052e010a010a04040102012c01120108ff08
-                  022a012a0110010e01340110021e02040116010c0110ff04ff1004040204
-                  0116010c0124ff04ff100404030c0112012801100104011e0204011e032a
-                  01200104042a010c01040108fe10071202040214031aff0404360122021c
-                  013a020c0102020e0104ff040202fe020302fd0405020102010201020102
-                  0102010201020102f204fe
+                  0x02010e010e010e010e010e0332012a0132020c01100324ff0c0310011e
+                  052e010a010a04040102012c01120108ff08022a012a0110010e01340110
+                  021e02040116010c0110ff04ff10040402040116010c0124ff04ff100404
+                  030c0112012801100104011e0204011e032a01200104020e0114020e0102
+                  01020102010201020102fa040702f9
             'return'
             code
                argcount  : 0
                nlocals   : 4
                stacksize : 6
                flags     : 11
                code
                   0x970069007d017c00a00000000000000000000000000000000000000000
                   00a6000000ab00000000000000000044005d2f5c0200007d027d03740200
                   000000000000000000a00200000000000000000000000000000000000000
                   007407000000000000000000007c03a6010000ab010000000000000000a6
                   010000ab0100000000000000007c017c023c0000008c307c015300
-               182           0 RESUME                   0
+               147           0 RESUME                   0
                
-               185           2 BUILD_MAP                0
+               150           2 BUILD_MAP                0
                              4 STORE_FAST               1 (packed)
                
-               186           6 LOAD_FAST                0 (kwargs)
+               151           6 LOAD_FAST                0 (kwargs)
                              8 LOAD_METHOD              0 (items)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 GET_ITER
                        >>   46 FOR_ITER                47 (to 142)
                             48 UNPACK_SEQUENCE          2
                             52 STORE_FAST               2 (k)
                             54 STORE_FAST               3 (v)
                
-               187          56 LOAD_GLOBAL              2 (url_value_signer)
+               152          56 LOAD_GLOBAL              2 (url_value_signer)
                             68 LOAD_METHOD              2 (sign)
                             90 LOAD_GLOBAL              7 (NULL + str)
                            102 LOAD_FAST                3 (v)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 PRECALL                  1
                            122 CALL                     1
                            132 LOAD_FAST                1 (packed)
                            134 LOAD_FAST                2 (k)
                            136 STORE_SUBSCR
                            140 JUMP_BACKWARD           48 (to 46)
                
-               189     >>  142 LOAD_FAST                1 (packed)
+               154     >>  142 LOAD_FAST                1 (packed)
                            144 RETURN_VALUE
                consts
                   None
                names      ('items', 'url_value_signer', 'sign', 'str')
                varnames   ('kwargs', 'packed', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'pack'
-               firstlineno 182
+               firstlineno 147
                lnotab 0x0203040132015602
             ('request',)
             'expected'
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 7
@@ -1208,130 +954,130 @@
                   057c039b009d02a6010000ab010000000000000000820177007803590077
                   0174150000000000000000000088046601640684087c024400a6000000ab
                   000000000000000000a6010000ab01000000000000000073187c00a00700
                   0000000000000000000000000000000000000064057c039b009d02a60100
                   00ab010000000000000000820189045300
                              0 MAKE_CELL                4 (unpacked)
                
-               191           2 RESUME                   0
+               156           2 RESUME                   0
                
-               193           4 LOAD_FAST                1 (request)
+               158           4 LOAD_FAST                1 (request)
                              6 POP_JUMP_FORWARD_IF_TRUE    15 (to 38)
                
-               194           8 LOAD_GLOBAL              1 (NULL + ValueError)
+               159           8 LOAD_GLOBAL              1 (NULL + ValueError)
                             20 LOAD_CONST               1 ('Request is required')
                             22 PRECALL                  1
                             26 CALL                     1
                             36 RAISE_VARARGS            1
                
-               196     >>   38 BUILD_MAP                0
+               161     >>   38 BUILD_MAP                0
                             40 STORE_DEREF              4 (unpacked)
                
-               197          42 LOAD_FAST                2 (expected)
+               162          42 LOAD_FAST                2 (expected)
                             44 GET_ITER
                        >>   46 FOR_ITER               171 (to 390)
                             48 STORE_FAST               3 (key)
                
-               198          50 NOP
+               163          50 NOP
                
-               199          52 LOAD_GLOBAL              2 (url_value_signer)
+               164          52 LOAD_GLOBAL              2 (url_value_signer)
                             64 LOAD_METHOD              2 (unsign)
                
-               200          86 LOAD_FAST                1 (request)
+               165          86 LOAD_FAST                1 (request)
                             88 LOAD_ATTR                3 (GET)
                             98 LOAD_METHOD              4 (get)
                            120 LOAD_FAST                3 (key)
                            122 PRECALL                  1
                            126 CALL                     1
                
-               199         136 PRECALL                  1
+               164         136 PRECALL                  1
                            140 CALL                     1
                            150 LOAD_DEREF               4 (unpacked)
                            152 LOAD_FAST                3 (key)
                            154 STORE_SUBSCR
                            158 JUMP_BACKWARD           57 (to 46)
                        >>  160 PUSH_EXC_INFO
                
-               202         162 LOAD_GLOBAL             10 (signing)
+               167         162 LOAD_GLOBAL             10 (signing)
                            174 LOAD_ATTR                6 (SignatureExpired)
                            184 CHECK_EXC_MATCH
                            186 POP_JUMP_FORWARD_IF_FALSE    26 (to 240)
                            188 POP_TOP
                
-               203         190 LOAD_FAST                0 (cls)
+               168         190 LOAD_FAST                0 (cls)
                            192 LOAD_METHOD              7 (UnpackError)
                            214 LOAD_CONST               2 ('Value for ')
                            216 LOAD_FAST                3 (key)
                            218 FORMAT_VALUE             0
                            220 LOAD_CONST               3 (' has expired')
                            222 BUILD_STRING             3
                            224 PRECALL                  1
                            228 CALL                     1
                            238 RAISE_VARARGS            1
                
-               204     >>  240 LOAD_GLOBAL             10 (signing)
+               169     >>  240 LOAD_GLOBAL             10 (signing)
                            252 LOAD_ATTR                8 (BadSignature)
                            262 CHECK_EXC_MATCH
                            264 POP_JUMP_FORWARD_IF_FALSE    25 (to 316)
                            266 POP_TOP
                
-               205         268 LOAD_FAST                0 (cls)
+               170         268 LOAD_FAST                0 (cls)
                            270 LOAD_METHOD              7 (UnpackError)
                            292 LOAD_CONST               4 ('Invalid value for ')
                            294 LOAD_FAST                3 (key)
                            296 FORMAT_VALUE             0
                            298 BUILD_STRING             2
                            300 PRECALL                  1
                            304 CALL                     1
                            314 RAISE_VARARGS            1
                
-               206     >>  316 LOAD_GLOBAL             18 (TypeError)
+               171     >>  316 LOAD_GLOBAL             18 (TypeError)
                            328 CHECK_EXC_MATCH
                            330 POP_JUMP_FORWARD_IF_FALSE    25 (to 382)
                            332 POP_TOP
                
-               207         334 LOAD_FAST                0 (cls)
+               172         334 LOAD_FAST                0 (cls)
                            336 LOAD_METHOD              7 (UnpackError)
                            358 LOAD_CONST               5 ('Missing value for ')
                            360 LOAD_FAST                3 (key)
                            362 FORMAT_VALUE             0
                            364 BUILD_STRING             2
                            366 PRECALL                  1
                            370 CALL                     1
                            380 RAISE_VARARGS            1
                
-               206     >>  382 RERAISE                  0
+               171     >>  382 RERAISE                  0
                        >>  384 COPY                     3
                            386 POP_EXCEPT
                            388 RERAISE                  1
                
-               209     >>  390 LOAD_GLOBAL             21 (NULL + all)
+               174     >>  390 LOAD_GLOBAL             21 (NULL + all)
                            402 LOAD_CLOSURE             4 (unpacked)
                            404 BUILD_TUPLE              1
-                           406 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 209>)
+                           406 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 174>)
                            408 MAKE_FUNCTION            8 (closure)
                            410 LOAD_FAST                2 (expected)
                            412 GET_ITER
                            414 PRECALL                  0
                            418 CALL                     0
                            428 PRECALL                  1
                            432 CALL                     1
                            442 POP_JUMP_FORWARD_IF_TRUE    24 (to 492)
                
-               210         444 LOAD_FAST                0 (cls)
+               175         444 LOAD_FAST                0 (cls)
                            446 LOAD_METHOD              7 (UnpackError)
                            468 LOAD_CONST               5 ('Missing value for ')
                            470 LOAD_FAST                3 (key)
                            472 FORMAT_VALUE             0
                            474 BUILD_STRING             2
                            476 PRECALL                  1
                            480 CALL                     1
                            490 RAISE_VARARGS            1
                
-               212     >>  492 LOAD_DEREF               4 (unpacked)
+               177     >>  492 LOAD_DEREF               4 (unpacked)
                            494 RETURN_VALUE
                ExceptionTable:
                  52 to 156 -> 160 [1]
                  160 to 382 -> 384 [2] lasti
                consts
                   None
                   'Request is required'
@@ -1345,15 +1091,15 @@
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d177d018902a00000000000000000000000000000
                         000000000000007c01a6010000ab01000000000000000091028c185300
                                    0 COPY_FREE_VARS           1
                      
-                     209           2 RESUME                   0
+                     174           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                23 (to 56)
                                   10 STORE_FAST               1 (key)
                                   12 LOAD_DEREF               2 (unpacked)
                                   14 LOAD_METHOD              0 (get)
                                   36 LOAD_FAST                1 (key)
@@ -1363,25 +1109,25 @@
                                   54 JUMP_BACKWARD           24 (to 8)
                              >>   56 RETURN_VALUE
                      consts
                      names      ('get',)
                      varnames   ('.0', 'key')
                      freevars   ('unpacked',)
                      cellvars   ()
-                     filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+                     filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<listcomp>'
-                     firstlineno 209
+                     firstlineno 174
                      lnotab 0x
                names      ('ValueError', 'url_value_signer', 'unsign', 'GET', 'get', 'signing', 'SignatureExpired', 'UnpackError', 'BadSignature', 'TypeError', 'all')
                varnames   ('cls', 'request', 'expected', 'key')
                freevars   ()
                cellvars   ('unpacked',)
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'unpack'
-               firstlineno 191
+               firstlineno 156
                lnotab
                   0x040204011e02040108010201220132ff1a031c0132011c013001120130
                   ff080336013002
             'instance'
             code
                argcount  : 3
                nlocals   : 6
@@ -1390,58 +1136,58 @@
                code
                   0x970074010000000000000000000064017c007c017c026a010000000000
                   0000006a0200000000000000007c026a0100000000000000006a03000000
                   00000000007c026a0400000000000000006705ac02a6020000ab02000000
                   00000000007d047c0373027c045300740b00000000000000000000740d00
                   0000000000000000006a070000000000000000640469007c03a4018e01a6
                   010000ab0100000000000000007d057c049b0064037c059b009d035300
-               214           0 RESUME                   0
+               179           0 RESUME                   0
                
-               216           2 LOAD_GLOBAL              1 (NULL + reverse)
+               181           2 LOAD_GLOBAL              1 (NULL + reverse)
                
-               217          14 LOAD_CONST               1 ('wagtail_fedit:edit_block')
+               182          14 LOAD_CONST               1 ('wagtail_fedit:edit_block')
                
-               218          16 LOAD_FAST                0 (block_id)
+               183          16 LOAD_FAST                0 (block_id)
                             18 LOAD_FAST                1 (field_name)
                             20 LOAD_FAST                2 (instance)
                             22 LOAD_ATTR                1 (_meta)
                             32 LOAD_ATTR                2 (app_label)
                             42 LOAD_FAST                2 (instance)
                             44 LOAD_ATTR                1 (_meta)
                             54 LOAD_ATTR                3 (model_name)
                             64 LOAD_FAST                2 (instance)
                             66 LOAD_ATTR                4 (pk)
                             76 BUILD_LIST               5
                
-               216          78 KW_NAMES                 2
+               181          78 KW_NAMES                 2
                             80 PRECALL                  2
                             84 CALL                     2
                             94 STORE_FAST               4 (base_url)
                
-               221          96 LOAD_FAST                3 (kwargs)
+               186          96 LOAD_FAST                3 (kwargs)
                             98 POP_JUMP_FORWARD_IF_TRUE     2 (to 104)
                
-               222         100 LOAD_FAST                4 (base_url)
+               187         100 LOAD_FAST                4 (base_url)
                            102 RETURN_VALUE
                
-               224     >>  104 LOAD_GLOBAL             11 (NULL + urlencode)
+               189     >>  104 LOAD_GLOBAL             11 (NULL + urlencode)
                
-               225         116 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+               190         116 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                            128 LOAD_ATTR                7 (pack)
                            138 LOAD_CONST               4 (())
                            140 BUILD_MAP                0
                            142 LOAD_FAST                3 (kwargs)
                            144 DICT_MERGE               1
                            146 CALL_FUNCTION_EX         1
                
-               224         148 PRECALL                  1
+               189         148 PRECALL                  1
                            152 CALL                     1
                            162 STORE_FAST               5 (packed)
                
-               227         164 LOAD_FAST                4 (base_url)
+               192         164 LOAD_FAST                4 (base_url)
                            166 FORMAT_VALUE             0
                            168 LOAD_CONST               3 ('?')
                            170 LOAD_FAST                5 (packed)
                            172 FORMAT_VALUE             0
                            174 BUILD_STRING             3
                            176 RETURN_VALUE
                consts
@@ -1450,29 +1196,29 @@
                   ('args',)
                   '?'
                   ()
                names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack')
                varnames   ('block_id', 'field_name', 'instance', 'kwargs', 'base_url', 'packed')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'get_edit_url'
-               firstlineno 214
+               firstlineno 179
                lnotab 0x02020c0102013efe1205040104020c0120ff1003
             (None, None, None, None, None)
          names      ('__name__', '__module__', '__qualname__', 'Exception', 'UnpackError', 'NodeList', 'BoundBlock', 'str', 'models', 'Model', '__init__', 'render', 'staticmethod', 'dict', 'pack', 'classmethod', 'unpack', 'get_edit_url')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'BlockEditNode'
-         firstlineno 36
+         firstlineno 40
          lnotab
             0x0a011c04020102010201020102fb040102ff020202fe020302fd020402
-            fc02050cfb0810067e02010aff0e010208020114ff0e010216020120ff0e
+            fc02050cfb0810065702010aff0e010208020114ff0e010216020120ff0e
             01
       'BlockEditNode'
       'fedit_block'
       ('name',)
       'parser'
       'token'
       code
@@ -1494,123 +1240,123 @@
             000000000000000000640a7c067c05a00700000000000000000000000000
             000000000000006403a6010000ab0100000000000000007c05a007000000
             00000000000000000000000000000000006406a6010000ab010000000000
             0000007c05a00700000000000000000000000000000000000000006407a6
             010000ab0100000000000000007c05a00700000000000000000000000000
             000000000000006408a6010000ab01000000000000000064099c057c07a4
             018e015300
-         231           0 RESUME                   0
+         196           0 RESUME                   0
          
-         261           2 LOAD_FAST                1 (token)
+         226           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         262          42 LOAD_FAST                2 (tokens)
+         227          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         263          84 BUILD_LIST               0
+         228          84 BUILD_LIST               0
                       86 LOAD_CONST               2 (('block', 'block_id', 'field_name', 'model'))
                       88 LIST_EXTEND              1
                       90 STORE_FAST               4 (kwargs_names)
          
-         268          92 LOAD_GLOBAL              5 (NULL + get_kwargs)
+         233          92 LOAD_GLOBAL              5 (NULL + get_kwargs)
                      104 LOAD_FAST                0 (parser)
                      106 LOAD_FAST                4 (kwargs_names)
                      108 LOAD_FAST                2 (tokens)
                      110 PRECALL                  3
                      114 CALL                     3
                      124 STORE_FAST               5 (kwargs)
          
-         270         126 LOAD_CONST               3 ('block')
+         235         126 LOAD_CONST               3 ('block')
                      128 LOAD_FAST                5 (kwargs)
                      130 CONTAINS_OP              1
                      132 POP_JUMP_FORWARD_IF_FALSE    42 (to 218)
          
-         271         134 LOAD_FAST                0 (parser)
+         236         134 LOAD_FAST                0 (parser)
                      136 LOAD_METHOD              3 (parse)
                      158 LOAD_CONST               4 (('unfedit_block',))
                      160 PRECALL                  1
                      164 CALL                     1
                      174 STORE_FAST               6 (nodelist)
          
-         272         176 LOAD_FAST                0 (parser)
+         237         176 LOAD_FAST                0 (parser)
                      178 LOAD_METHOD              4 (delete_first_token)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
                      216 JUMP_FORWARD             2 (to 222)
          
-         274     >>  218 LOAD_CONST               5 (None)
+         239     >>  218 LOAD_CONST               5 (None)
                      220 STORE_FAST               6 (nodelist)
          
-         276     >>  222 BUILD_MAP                0
+         241     >>  222 BUILD_MAP                0
                      224 STORE_FAST               7 (extra)
          
-         277         226 LOAD_FAST                5 (kwargs)
+         242         226 LOAD_FAST                5 (kwargs)
                      228 LOAD_METHOD              5 (items)
                      250 PRECALL                  0
                      254 CALL                     0
                      264 GET_ITER
                  >>  266 FOR_ITER                14 (to 296)
                      268 UNPACK_SEQUENCE          2
                      272 STORE_FAST               8 (key)
                      274 STORE_FAST               9 (value)
          
-         278         276 LOAD_FAST                8 (key)
+         243         276 LOAD_FAST                8 (key)
                      278 LOAD_FAST                4 (kwargs_names)
                      280 CONTAINS_OP              1
                      282 POP_JUMP_FORWARD_IF_FALSE     5 (to 294)
          
-         279         284 LOAD_FAST                9 (value)
+         244         284 LOAD_FAST                9 (value)
                      286 LOAD_FAST                7 (extra)
                      288 LOAD_FAST                8 (key)
                      290 STORE_SUBSCR
                  >>  294 JUMP_BACKWARD           15 (to 266)
          
-         281     >>  296 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+         246     >>  296 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                      308 LOAD_CONST              10 (())
          
-         282         310 LOAD_FAST                6 (nodelist)
+         247         310 LOAD_FAST                6 (nodelist)
          
-         283         312 LOAD_FAST                5 (kwargs)
+         248         312 LOAD_FAST                5 (kwargs)
                      314 LOAD_METHOD              7 (get)
                      336 LOAD_CONST               3 ('block')
                      338 PRECALL                  1
                      342 CALL                     1
          
-         284         352 LOAD_FAST                5 (kwargs)
+         249         352 LOAD_FAST                5 (kwargs)
                      354 LOAD_METHOD              7 (get)
                      376 LOAD_CONST               6 ('block_id')
                      378 PRECALL                  1
                      382 CALL                     1
          
-         285         392 LOAD_FAST                5 (kwargs)
+         250         392 LOAD_FAST                5 (kwargs)
                      394 LOAD_METHOD              7 (get)
                      416 LOAD_CONST               7 ('field_name')
                      418 PRECALL                  1
                      422 CALL                     1
          
-         286         432 LOAD_FAST                5 (kwargs)
+         251         432 LOAD_FAST                5 (kwargs)
                      434 LOAD_METHOD              7 (get)
                      456 LOAD_CONST               8 ('model')
                      458 PRECALL                  1
                      462 CALL                     1
          
-         281         472 LOAD_CONST               9 (('nodelist', 'block', 'block_id', 'field_name', 'model'))
+         246         472 LOAD_CONST               9 (('nodelist', 'block', 'block_id', 'field_name', 'model'))
                      474 BUILD_CONST_KEY_MAP      5
          
-         287         476 LOAD_FAST                7 (extra)
+         252         476 LOAD_FAST                7 (extra)
          
-         281         478 DICT_MERGE               1
+         246         478 DICT_MERGE               1
                      480 CALL_FUNCTION_EX         1
                      482 RETURN_VALUE
          consts
             '\n    This tag is used to render an editable block.\n\n    This block will be wrapped and is able to be edited by the user on the frontend.\n\n    We will require the block_id and field_name of the streamfield this block belongs to.\n\n    You could omit needing to pass a block ID by passing in the StreamChild instance as opposed to the StructValue instance.\n    \n    Usage example 1:\n        ```python\n        {% fedit_block my_structvalue_instance block_id my_streamfield_attribute_name page_instance %}\n        ```\n\n    Optionally you can omit the block and pass in the block_id and field_name as keyword arguments.\n\n    This will allow you to use the block as a block tag.\n\n    Usage example 2:\n        ```python\n        {% fedit_block block_id=my_structvalue_instance field_name=my_streamfield_attribute_name model=page_instance %}\n            <p>Some content before block</p>\n            {% include_block my_block %}\n            <p>Some content after block</p>\n        {% unfedit_block %}\n        ```\n    '
             0
             ('block', 'block_id', 'field_name', 'model')
             'block'
@@ -1621,51 +1367,51 @@
             'model'
             ('nodelist', 'block', 'block_id', 'field_name', 'model')
             ()
          names      ('split_contents', 'pop', 'get_kwargs', 'parse', 'delete_first_token', 'items', 'BlockEditNode', 'get')
          varnames   ('parser', 'token', 'tokens', '_', 'kwargs_names', 'kwargs', 'nodelist', 'extra', 'key', 'value')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit_block'
-         firstlineno 231
+         firstlineno 196
          lnotab
             0x021e28012a010805220208012a012a0204020401320108010c020e0102
             0128012801280128fb040602fa
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a026408640265036a040000000000000000640365
             05650619000000000000000000640465076606640584055a08640684005a
             0964075300
-         291           0 RESUME                   0
+         256           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('FieldEditNode')
                        8 STORE_NAME               2 (__qualname__)
          
-         292          10 LOAD_CONST               8 ((False,))
+         257          10 LOAD_CONST               8 ((False,))
                       12 LOAD_CONST               2 ('model')
                       14 LOAD_NAME                3 (models)
                       16 LOAD_ATTR                4 (Model)
                       26 LOAD_CONST               3 ('getters')
                       28 LOAD_NAME                5 (list)
                       30 LOAD_NAME                6 (str)
                       32 BINARY_SUBSCR
                       42 LOAD_CONST               4 ('inline')
                       44 LOAD_NAME                7 (bool)
                       46 BUILD_TUPLE              6
-                      48 LOAD_CONST               5 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 292>)
+                      48 LOAD_CONST               5 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 257>)
                       50 MAKE_FUNCTION            5 (defaults, annotations)
                       52 STORE_NAME               8 (__init__)
          
-         299          54 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 299>)
+         264          54 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 264>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME               9 (render)
                       60 LOAD_CONST               7 (None)
                       62 RETURN_VALUE
          consts
             'FieldEditNode'
             False
@@ -1679,285 +1425,311 @@
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027403000000000000000000
                   007c02a6010000ab01000000000000000064017a0a000019000000000000
                   0000007c005f0200000000000000007c027c005f0300000000000000007c
                   037c005f0400000000000000007c047c005f050000000000000000640053
                   00
-               292           0 RESUME                   0
+               257           0 RESUME                   0
                
-               293           2 LOAD_FAST                1 (model)
+               258           2 LOAD_FAST                1 (model)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (model)
                
-               294          16 LOAD_FAST                2 (getters)
+               259          16 LOAD_FAST                2 (getters)
                             18 LOAD_GLOBAL              3 (NULL + len)
                             30 LOAD_FAST                2 (getters)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 LOAD_CONST               1 (1)
                             48 BINARY_OP               10 (-)
                             52 BINARY_SUBSCR
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               2 (field)
                
-               295          74 LOAD_FAST                2 (getters)
+               260          74 LOAD_FAST                2 (getters)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               3 (getters)
                
-               296          88 LOAD_FAST                3 (inline)
+               261          88 LOAD_FAST                3 (inline)
                             90 LOAD_FAST                0 (self)
                             92 STORE_ATTR               4 (inline)
                
-               297         102 LOAD_FAST                4 (kwargs)
+               262         102 LOAD_FAST                4 (kwargs)
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               5 (kwargs)
                            116 LOAD_CONST               0 (None)
                            118 RETURN_VALUE
                consts
                   None
                   1
                names      ('model', 'len', 'field', 'getters', 'inline', 'kwargs')
                varnames   ('self', 'model', 'getters', 'inline', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 292
+               firstlineno 257
                lnotab 0x02010e013a010e010e01
             code
                argcount  : 2
-               nlocals   : 10
-               stacksize : 10
+               nlocals   : 12
+               stacksize : 9
                flags     : 3
                code
                   0x97007c006a0000000000000000007d027c006a0100000000000000007d
-                  037c006a0200000000000000007d047407000000000000000000007c0374
-                  0800000000000000000000a6020000ab02000000000000000072157c03a0
-                  0500000000000000000000000000000000000000007c01a6010000ab0100
-                  000000000000007d037407000000000000000000007c0474080000000000
-                  0000000000a6020000ab02000000000000000072157c04a0050000000000
-                  0000000000000000000000000000007c01a6010000ab0100000000000000
-                  007d047c037d05740d00000000000000000000740f000000000000000000
-                  007c02a6010000ab01000000000000000064017a0a0000a6010000ab0100
-                  0000000000000044005d487d067c027c06190000000000000000007d0709
-                  007411000000000000000000007c057c07a6020000ab0200000000000000
-                  007d058c1c23007412000000000000000000002400722001007413000000
-                  0000000000000064027c036a0a00000000000000006a0b00000000000000
-                  009b0064037c079b009d04a6010000ab0100000000000000008201770078
-                  03590077017c01a00c000000000000000000000000000000000000000064
-                  04a6010000ab0100000000000000007d08741b000000000000000000007c
-                  087c057c056a0e0000000000000000a00f00000000000000000000000000
-                  000000000000007c006a100000000000000000a6010000ab010000000000
-                  0000007c01a6040000ab0400000000000000007d097c09730f7423000000
-                  000000000000006405a6010000ab0100000000000000007d097425000000
-                  000000000000007c087c05a6020000ab02000000000000000073027c0953
-                  0074270000000000000000000064077c087c097c006a1000000000000000
-                  007c057c017c0464069c067c006a140000000000000000a4018e015300
-               299           0 RESUME                   0
+                  037c006a0200000000000000007d047407000000000000000000007c017c
+                  037c04a6030000ab0300000000000000005c0200007d037d047c037d0574
+                  0900000000000000000000740b000000000000000000007c02a6010000ab
+                  01000000000000000064017a0a0000a6010000ab01000000000000000044
+                  005d487d067c027c06190000000000000000007d070900740d0000000000
+                  00000000007c057c07a6020000ab0200000000000000007d058c1c230074
+                  0e00000000000000000000240072200100740f0000000000000000000064
+                  027c036a0800000000000000006a0900000000000000009b0064037c079b
+                  009d04a6010000ab010000000000000000820177007803590077017c01a0
+                  0a00000000000000000000000000000000000000006404a6010000ab0100
+                  000000000000007d087417000000000000000000007c087c057c056a0c00
+                  00000000000000a00d00000000000000000000000000000000000000007c
+                  006a0e0000000000000000a6010000ab0100000000000000007c01a60400
+                  00ab0400000000000000007d097c097311741f0000000000000000000064
+                  05a6010000ab0100000000000000007d0964067d04742100000000000000
+                  0000007c087c05a6020000ab02000000000000000073027c0953007c006a
+                  110000000000000000a01200000000000000000000000000000000000000
+                  00a6000000ab00000000000000000044005d375c0200007d0a7d0b742700
+                  0000000000000000007c0b742800000000000000000000a6020000ab0200
+                  00000000000000721d7c0ba0150000000000000000000000000000000000
+                  0000007c01a6010000ab0100000000000000007c006a1100000000000000
+                  007c0a3c0000008c387c04720a64067c006a11000000000000000064073c
+                  000000742d0000000000000000000064097c087c097c006a0e0000000000
+                  0000007c057c0164089c057c006a110000000000000000a4018e015300
+               264           0 RESUME                   0
                
-               300           2 LOAD_FAST                0 (self)
+               265           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (getters)
                             14 STORE_FAST               2 (getters)
                
-               301          16 LOAD_FAST                0 (self)
+               266          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (model)
                             28 STORE_FAST               3 (model)
                
-               302          30 LOAD_FAST                0 (self)
+               267          30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                2 (inline)
                             42 STORE_FAST               4 (inline)
                
-               304          44 LOAD_GLOBAL              7 (NULL + isinstance)
-                            56 LOAD_FAST                3 (model)
-                            58 LOAD_GLOBAL              8 (FilterExpression)
-                            70 PRECALL                  2
-                            74 CALL                     2
-                            84 POP_JUMP_FORWARD_IF_FALSE    21 (to 128)
-               
-               305          86 LOAD_FAST                3 (model)
-                            88 LOAD_METHOD              5 (resolve)
-                           110 LOAD_FAST                1 (context)
-                           112 PRECALL                  1
-                           116 CALL                     1
-                           126 STORE_FAST               3 (model)
-               
-               307     >>  128 LOAD_GLOBAL              7 (NULL + isinstance)
-                           140 LOAD_FAST                4 (inline)
-                           142 LOAD_GLOBAL              8 (FilterExpression)
-                           154 PRECALL                  2
-                           158 CALL                     2
-                           168 POP_JUMP_FORWARD_IF_FALSE    21 (to 212)
-               
-               308         170 LOAD_FAST                4 (inline)
-                           172 LOAD_METHOD              5 (resolve)
-                           194 LOAD_FAST                1 (context)
-                           196 PRECALL                  1
-                           200 CALL                     1
-                           210 STORE_FAST               4 (inline)
-               
-               310     >>  212 LOAD_FAST                3 (model)
-                           214 STORE_FAST               5 (obj)
-               
-               311         216 LOAD_GLOBAL             13 (NULL + range)
-                           228 LOAD_GLOBAL             15 (NULL + len)
-                           240 LOAD_FAST                2 (getters)
-                           242 PRECALL                  1
-                           246 CALL                     1
-                           256 LOAD_CONST               1 (1)
-                           258 BINARY_OP               10 (-)
-                           262 PRECALL                  1
-                           266 CALL                     1
-                           276 GET_ITER
-                       >>  278 FOR_ITER                72 (to 424)
-                           280 STORE_FAST               6 (i)
-               
-               312         282 LOAD_FAST                2 (getters)
-                           284 LOAD_FAST                6 (i)
-                           286 BINARY_SUBSCR
-                           296 STORE_FAST               7 (getter)
-               
-               313         298 NOP
-               
-               314         300 LOAD_GLOBAL             17 (NULL + getattr)
-                           312 LOAD_FAST                5 (obj)
-                           314 LOAD_FAST                7 (getter)
-                           316 PRECALL                  2
-                           320 CALL                     2
-                           330 STORE_FAST               5 (obj)
-                           332 JUMP_BACKWARD           28 (to 278)
-                       >>  334 PUSH_EXC_INFO
-               
-               315         336 LOAD_GLOBAL             18 (AttributeError)
-                           348 CHECK_EXC_MATCH
-                           350 POP_JUMP_FORWARD_IF_FALSE    32 (to 416)
-                           352 POP_TOP
-               
-               316         354 LOAD_GLOBAL             19 (NULL + AttributeError)
-                           366 LOAD_CONST               2 ('Object ')
-                           368 LOAD_FAST                3 (model)
-                           370 LOAD_ATTR               10 (__class__)
-                           380 LOAD_ATTR               11 (__name__)
-                           390 FORMAT_VALUE             0
-                           392 LOAD_CONST               3 (' does not have attribute ')
-                           394 LOAD_FAST                7 (getter)
-                           396 FORMAT_VALUE             0
-                           398 BUILD_STRING             4
+               270          44 LOAD_GLOBAL              7 (NULL + _resolve_expressions)
+                            56 LOAD_FAST                1 (context)
+                            58 LOAD_FAST                3 (model)
+                            60 LOAD_FAST                4 (inline)
+                            62 PRECALL                  3
+                            66 CALL                     3
+               
+               269          76 UNPACK_SEQUENCE          2
+                            80 STORE_FAST               3 (model)
+                            82 STORE_FAST               4 (inline)
+               
+               272          84 LOAD_FAST                3 (model)
+                            86 STORE_FAST               5 (obj)
+               
+               273          88 LOAD_GLOBAL              9 (NULL + range)
+                           100 LOAD_GLOBAL             11 (NULL + len)
+                           112 LOAD_FAST                2 (getters)
+                           114 PRECALL                  1
+                           118 CALL                     1
+                           128 LOAD_CONST               1 (1)
+                           130 BINARY_OP               10 (-)
+                           134 PRECALL                  1
+                           138 CALL                     1
+                           148 GET_ITER
+                       >>  150 FOR_ITER                72 (to 296)
+                           152 STORE_FAST               6 (i)
+               
+               274         154 LOAD_FAST                2 (getters)
+                           156 LOAD_FAST                6 (i)
+                           158 BINARY_SUBSCR
+                           168 STORE_FAST               7 (getter)
+               
+               275         170 NOP
+               
+               276         172 LOAD_GLOBAL             13 (NULL + getattr)
+                           184 LOAD_FAST                5 (obj)
+                           186 LOAD_FAST                7 (getter)
+                           188 PRECALL                  2
+                           192 CALL                     2
+                           202 STORE_FAST               5 (obj)
+                           204 JUMP_BACKWARD           28 (to 150)
+                       >>  206 PUSH_EXC_INFO
+               
+               277         208 LOAD_GLOBAL             14 (AttributeError)
+                           220 CHECK_EXC_MATCH
+                           222 POP_JUMP_FORWARD_IF_FALSE    32 (to 288)
+                           224 POP_TOP
+               
+               278         226 LOAD_GLOBAL             15 (NULL + AttributeError)
+                           238 LOAD_CONST               2 ('Object ')
+                           240 LOAD_FAST                3 (model)
+                           242 LOAD_ATTR                8 (__class__)
+                           252 LOAD_ATTR                9 (__name__)
+                           262 FORMAT_VALUE             0
+                           264 LOAD_CONST               3 (' does not have attribute ')
+                           266 LOAD_FAST                7 (getter)
+                           268 FORMAT_VALUE             0
+                           270 BUILD_STRING             4
+                           272 PRECALL                  1
+                           276 CALL                     1
+                           286 RAISE_VARARGS            1
+               
+               277     >>  288 RERAISE                  0
+                       >>  290 COPY                     3
+                           292 POP_EXCEPT
+                           294 RERAISE                  1
+               
+               280     >>  296 LOAD_FAST                1 (context)
+                           298 LOAD_METHOD             10 (get)
+                           320 LOAD_CONST               4 ('request')
+                           322 PRECALL                  1
+                           326 CALL                     1
+                           336 STORE_FAST               8 (request)
+               
+               281         338 LOAD_GLOBAL             23 (NULL + get_field_content)
+               
+               282         350 LOAD_FAST                8 (request)
+               
+               283         352 LOAD_FAST                5 (obj)
+               
+               284         354 LOAD_FAST                5 (obj)
+                           356 LOAD_ATTR               12 (_meta)
+                           366 LOAD_METHOD             13 (get_field)
+                           388 LOAD_FAST                0 (self)
+                           390 LOAD_ATTR               14 (field)
                            400 PRECALL                  1
                            404 CALL                     1
-                           414 RAISE_VARARGS            1
-               
-               315     >>  416 RERAISE                  0
-                       >>  418 COPY                     3
-                           420 POP_EXCEPT
-                           422 RERAISE                  1
-               
-               318     >>  424 LOAD_FAST                1 (context)
-                           426 LOAD_METHOD             12 (get)
-                           448 LOAD_CONST               4 ('request')
-                           450 PRECALL                  1
-                           454 CALL                     1
-                           464 STORE_FAST               8 (request)
                
-               319         466 LOAD_GLOBAL             27 (NULL + get_field_content)
+               285         414 LOAD_FAST                1 (context)
                
-               320         478 LOAD_FAST                8 (request)
+               281         416 PRECALL                  4
+                           420 CALL                     4
+                           430 STORE_FAST               9 (content)
                
-               321         480 LOAD_FAST                5 (obj)
+               288         432 LOAD_FAST                9 (content)
+                           434 POP_JUMP_FORWARD_IF_TRUE    17 (to 470)
                
-               322         482 LOAD_FAST                5 (obj)
-                           484 LOAD_ATTR               14 (_meta)
-                           494 LOAD_METHOD             15 (get_field)
-                           516 LOAD_FAST                0 (self)
-                           518 LOAD_ATTR               16 (field)
-                           528 PRECALL                  1
-                           532 CALL                     1
-               
-               323         542 LOAD_FAST                1 (context)
-               
-               319         544 PRECALL                  4
-                           548 CALL                     4
-                           558 STORE_FAST               9 (content)
+               289         436 LOAD_GLOBAL             31 (NULL + mark_safe)
+                           448 LOAD_CONST               5 ('')
+                           450 PRECALL                  1
+                           454 CALL                     1
+                           464 STORE_FAST               9 (content)
                
-               326         560 LOAD_FAST                9 (content)
-                           562 POP_JUMP_FORWARD_IF_TRUE    15 (to 594)
+               292         466 LOAD_CONST               6 (True)
+                           468 STORE_FAST               4 (inline)
                
-               327         564 LOAD_GLOBAL             35 (NULL + mark_safe)
-                           576 LOAD_CONST               5 ('')
-                           578 PRECALL                  1
-                           582 CALL                     1
-                           592 STORE_FAST               9 (content)
+               294     >>  470 LOAD_GLOBAL             33 (NULL + _can_edit)
+                           482 LOAD_FAST                8 (request)
+                           484 LOAD_FAST                5 (obj)
+                           486 PRECALL                  2
+                           490 CALL                     2
+                           500 POP_JUMP_FORWARD_IF_TRUE     2 (to 506)
+               
+               295         502 LOAD_FAST                9 (content)
+                           504 RETURN_VALUE
+               
+               297     >>  506 LOAD_FAST                0 (self)
+                           508 LOAD_ATTR               17 (kwargs)
+                           518 LOAD_METHOD             18 (items)
+                           540 PRECALL                  0
+                           544 CALL                     0
+                           554 GET_ITER
+                       >>  556 FOR_ITER                55 (to 668)
+                           558 UNPACK_SEQUENCE          2
+                           562 STORE_FAST              10 (k)
+                           564 STORE_FAST              11 (v)
+               
+               298         566 LOAD_GLOBAL             39 (NULL + isinstance)
+                           578 LOAD_FAST               11 (v)
+                           580 LOAD_GLOBAL             40 (FilterExpression)
+                           592 PRECALL                  2
+                           596 CALL                     2
+                           606 POP_JUMP_FORWARD_IF_FALSE    29 (to 666)
                
-               329     >>  594 LOAD_GLOBAL             37 (NULL + _can_edit)
-                           606 LOAD_FAST                8 (request)
-                           608 LOAD_FAST                5 (obj)
-                           610 PRECALL                  2
-                           614 CALL                     2
-                           624 POP_JUMP_FORWARD_IF_TRUE     2 (to 630)
+               299         608 LOAD_FAST               11 (v)
+                           610 LOAD_METHOD             21 (resolve)
+                           632 LOAD_FAST                1 (context)
+                           634 PRECALL                  1
+                           638 CALL                     1
+                           648 LOAD_FAST                0 (self)
+                           650 LOAD_ATTR               17 (kwargs)
+                           660 LOAD_FAST               10 (k)
+                           662 STORE_SUBSCR
+                       >>  666 JUMP_BACKWARD           56 (to 556)
                
-               330         626 LOAD_FAST                9 (content)
-                           628 RETURN_VALUE
+               301     >>  668 LOAD_FAST                4 (inline)
+                           670 POP_JUMP_FORWARD_IF_FALSE    10 (to 692)
                
-               332     >>  630 LOAD_GLOBAL             39 (NULL + render_editable_field)
-                           642 LOAD_CONST               7 (())
+               302         672 LOAD_CONST               6 (True)
+                           674 LOAD_FAST                0 (self)
+                           676 LOAD_ATTR               17 (kwargs)
+                           686 LOAD_CONST               7 ('inline')
+                           688 STORE_SUBSCR
                
-               333         644 LOAD_FAST                8 (request)
+               304     >>  692 LOAD_GLOBAL             45 (NULL + render_editable_field)
+                           704 LOAD_CONST               9 (())
                
-               334         646 LOAD_FAST                9 (content)
+               305         706 LOAD_FAST                8 (request)
                
-               335         648 LOAD_FAST                0 (self)
-                           650 LOAD_ATTR               16 (field)
+               306         708 LOAD_FAST                9 (content)
                
-               336         660 LOAD_FAST                5 (obj)
+               307         710 LOAD_FAST                0 (self)
+                           712 LOAD_ATTR               14 (field)
                
-               337         662 LOAD_FAST                1 (context)
+               308         722 LOAD_FAST                5 (obj)
                
-               338         664 LOAD_FAST                4 (inline)
+               309         724 LOAD_FAST                1 (context)
                
-               332         666 LOAD_CONST               6 (('request', 'content', 'field_name', 'model', 'context', 'inline'))
-                           668 BUILD_CONST_KEY_MAP      6
+               304         726 LOAD_CONST               8 (('request', 'content', 'field_name', 'model', 'context'))
+                           728 BUILD_CONST_KEY_MAP      5
                
-               339         670 LOAD_FAST                0 (self)
-                           672 LOAD_ATTR               20 (kwargs)
+               310         730 LOAD_FAST                0 (self)
+                           732 LOAD_ATTR               17 (kwargs)
                
-               332         682 DICT_MERGE               1
-                           684 CALL_FUNCTION_EX         1
-                           686 RETURN_VALUE
+               304         742 DICT_MERGE               1
+                           744 CALL_FUNCTION_EX         1
+                           746 RETURN_VALUE
                ExceptionTable:
-                 300 to 330 -> 334 [1]
-                 334 to 416 -> 418 [2] lasti
+                 172 to 202 -> 206 [1]
+                 206 to 288 -> 290 [2] lasti
                consts
                   None
                   1
                   'Object '
                   ' does not have attribute '
                   'request'
                   ''
-                  ('request', 'content', 'field_name', 'model', 'context', 'inline')
+                  True
+                  'inline'
+                  ('request', 'content', 'field_name', 'model', 'context')
                   ()
-               names      ('getters', 'model', 'inline', 'isinstance', 'FilterExpression', 'resolve', 'range', 'len', 'getattr', 'AttributeError', '__class__', '__name__', 'get', 'get_field_content', '_meta', 'get_field', 'field', 'mark_safe', '_can_edit', 'render_editable_field', 'kwargs')
-               varnames   ('self', 'context', 'getters', 'model', 'inline', 'obj', 'i', 'getter', 'request', 'content')
+               names      ('getters', 'model', 'inline', '_resolve_expressions', 'range', 'len', 'getattr', 'AttributeError', '__class__', '__name__', 'get', 'get_field_content', '_meta', 'get_field', 'field', 'mark_safe', '_can_edit', 'kwargs', 'items', 'isinstance', 'FilterExpression', 'resolve', 'render_editable_field')
+               varnames   ('self', 'context', 'getters', 'model', 'inline', 'obj', 'i', 'getter', 'request', 'content', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 299
+               firstlineno 264
                lnotab
-                  0x02010e010e010e022a012a022a012a020401420110010201240112013e
-                  ff08032a010c01020102013c0102fc100704011e02200104020e01020102
-                  010c010201020102fa04070cf9
+                  0x02010e010e010e0320ff08030401420110010201240112013eff08032a
+                  010c01020102013c0102fc100704011e030402200104023c012a013c0204
+                  0114020e01020102010c01020102fb04060cfa
             None
             (False,)
          names      ('__name__', '__module__', '__qualname__', 'models', 'Model', 'list', 'str', 'bool', '__init__', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'FieldEditNode'
-         firstlineno 291
+         firstlineno 256
          lnotab 0x0a012c07
       'FieldEditNode'
       'fedit_field'
       code
          argcount  : 2
          nlocals   : 9
          stacksize : 6
@@ -1973,101 +1745,101 @@
             0000000000000000006404a6010000ab01000000000000000082017c00a0
             0500000000000000000000000000000000000000007c05a0010000000000
             0000000000000000000000000000006401a6010000ab0100000000000000
             00a6010000ab0100000000000000007d067c027215640567017d07740d00
             0000000000000000007c007c077c02a6030000ab0300000000000000007d
             086e0269007d08740f0000000000000000000064077c067c0564069c027c
             08a4018e015300
-         344           0 RESUME                   0
+         315           0 RESUME                   0
          
-         359           2 LOAD_FAST                1 (token)
+         330           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         360          42 LOAD_FAST                2 (tokens)
+         331          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         361          84 LOAD_FAST                2 (tokens)
+         332          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (model__field)
          
-         362         126 LOAD_FAST                4 (model__field)
+         333         126 LOAD_FAST                4 (model__field)
                      128 LOAD_METHOD              2 (split)
                      150 LOAD_CONST               2 ('.')
                      152 PRECALL                  1
                      156 CALL                     1
                      166 STORE_FAST               5 (model_tokens)
          
-         364         168 LOAD_GLOBAL              7 (NULL + len)
+         335         168 LOAD_GLOBAL              7 (NULL + len)
                      180 LOAD_FAST                5 (model_tokens)
                      182 PRECALL                  1
                      186 CALL                     1
                      196 LOAD_CONST               3 (2)
                      198 COMPARE_OP               0 (<)
                      204 POP_JUMP_FORWARD_IF_FALSE    15 (to 236)
          
-         365         206 LOAD_GLOBAL              9 (NULL + ValueError)
+         336         206 LOAD_GLOBAL              9 (NULL + ValueError)
                      218 LOAD_CONST               4 ('Model and field name are required')
                      220 PRECALL                  1
                      224 CALL                     1
                      234 RAISE_VARARGS            1
          
-         369     >>  236 LOAD_FAST                0 (parser)
+         340     >>  236 LOAD_FAST                0 (parser)
                      238 LOAD_METHOD              5 (compile_filter)
                      260 LOAD_FAST                5 (model_tokens)
                      262 LOAD_METHOD              1 (pop)
                      284 LOAD_CONST               1 (0)
                      286 PRECALL                  1
                      290 CALL                     1
                      300 PRECALL                  1
                      304 CALL                     1
                      314 STORE_FAST               6 (model)
          
-         371         316 LOAD_FAST                2 (tokens)
+         342         316 LOAD_FAST                2 (tokens)
                      318 POP_JUMP_FORWARD_IF_FALSE    21 (to 362)
          
-         373         320 LOAD_CONST               5 ('inline')
+         344         320 LOAD_CONST               5 ('inline')
          
-         372         322 BUILD_LIST               1
+         343         322 BUILD_LIST               1
                      324 STORE_FAST               7 (kwargs_names)
          
-         376         326 LOAD_GLOBAL             13 (NULL + get_kwargs)
+         347         326 LOAD_GLOBAL             13 (NULL + get_kwargs)
                      338 LOAD_FAST                0 (parser)
                      340 LOAD_FAST                7 (kwargs_names)
                      342 LOAD_FAST                2 (tokens)
                      344 PRECALL                  3
                      348 CALL                     3
                      358 STORE_FAST               8 (kwargs)
                      360 JUMP_FORWARD             2 (to 366)
          
-         378     >>  362 BUILD_MAP                0
+         349     >>  362 BUILD_MAP                0
                      364 STORE_FAST               8 (kwargs)
          
-         380     >>  366 LOAD_GLOBAL             15 (NULL + FieldEditNode)
+         351     >>  366 LOAD_GLOBAL             15 (NULL + FieldEditNode)
                      378 LOAD_CONST               7 (())
          
-         381         380 LOAD_FAST                6 (model)
+         352         380 LOAD_FAST                6 (model)
          
-         382         382 LOAD_FAST                5 (model_tokens)
+         353         382 LOAD_FAST                5 (model_tokens)
          
-         380         384 LOAD_CONST               6 (('model', 'getters'))
+         351         384 LOAD_CONST               6 (('model', 'getters'))
                      386 BUILD_CONST_KEY_MAP      2
          
-         383         388 LOAD_FAST                8 (kwargs)
+         354         388 LOAD_FAST                8 (kwargs)
          
-         380         390 DICT_MERGE               1
+         351         390 DICT_MERGE               1
                      392 CALL_FUNCTION_EX         1
                      394 RETURN_VALUE
          consts
             '\n    This tag is used to render an editable field.\n\n    This field will be wrapped and is able to be edited by the user on the frontend.\n\n    Usage example:\n        ```python\n        {% fedit_field mymodel.myfield inline=(default: False) key1=value1 key2=value2 %}\n        ```\n\n    Optionally your model can define a `render_fedit_{field_name}` method that will be used to render the field.\n    This will allow you to use custom rendering logic if need be.\n    '
             0
             '.'
             2
@@ -2075,17 +1847,17 @@
             'inline'
             ('model', 'getters')
             ()
          names      ('split_contents', 'pop', 'split', 'len', 'ValueError', 'compile_filter', 'get_kwargs', 'FieldEditNode')
          varnames   ('parser', 'token', 'tokens', '_', 'model__field', 'model_tokens', 'model', 'kwargs_names', 'kwargs')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit_field'
-         firstlineno 344
+         firstlineno 315
          lnotab
             0x020f28012a012a012a0226011e045002040202ff0404240204020e0102
             0102fe040302fd
       code
          argcount  : 5
          nlocals   : 10
          stacksize : 10
@@ -2109,120 +1881,120 @@
             00a6010000ab010000000000000000a01000000000000000000000000000
             00000000000000a6000000ab000000000000000000640a6b02000000007c
             0564083c000000742300000000000000000000640b7c067c027c037c017c
             047c08640c9c067c05a5018900ac0da6030000ab03000000000000000053
             00
                        0 MAKE_CELL                0 (request)
          
-         387           2 RESUME                   0
+         358           2 RESUME                   0
          
-         388           4 LOAD_GLOBAL              1 (NULL + reverse)
+         359           4 LOAD_GLOBAL              1 (NULL + reverse)
          
-         389          16 LOAD_CONST               1 ('wagtail_fedit:edit_field')
+         360          16 LOAD_CONST               1 ('wagtail_fedit:edit_field')
          
-         390          18 LOAD_FAST                2 (field_name)
+         361          18 LOAD_FAST                2 (field_name)
                       20 LOAD_FAST                3 (model)
                       22 LOAD_ATTR                1 (_meta)
                       32 LOAD_ATTR                2 (app_label)
                       42 LOAD_FAST                3 (model)
                       44 LOAD_ATTR                1 (_meta)
                       54 LOAD_ATTR                3 (model_name)
                       64 LOAD_FAST                3 (model)
                       66 LOAD_ATTR                4 (pk)
                       76 BUILD_LIST               4
          
-         388          78 KW_NAMES                 2
+         359          78 KW_NAMES                 2
                       80 PRECALL                  2
                       84 CALL                     2
                       94 STORE_FAST               6 (edit_url)
          
-         393          96 LOAD_FAST                5 (kwargs)
+         364          96 LOAD_FAST                5 (kwargs)
                       98 POP_JUMP_FORWARD_IF_FALSE    37 (to 174)
          
-         394         100 LOAD_GLOBAL             11 (NULL + urlencode)
+         365         100 LOAD_GLOBAL             11 (NULL + urlencode)
          
-         395         112 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+         366         112 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                      124 LOAD_ATTR                7 (pack)
                      134 LOAD_CONST              14 (())
                      136 BUILD_MAP                0
                      138 LOAD_FAST                5 (kwargs)
                      140 DICT_MERGE               1
                      142 CALL_FUNCTION_EX         1
          
-         394         144 PRECALL                  1
+         365         144 PRECALL                  1
                      148 CALL                     1
                      158 STORE_FAST               7 (packed)
          
-         397         160 LOAD_FAST                6 (edit_url)
+         368         160 LOAD_FAST                6 (edit_url)
                      162 FORMAT_VALUE             0
                      164 LOAD_CONST               3 ('?')
                      166 LOAD_FAST                7 (packed)
                      168 FORMAT_VALUE             0
                      170 BUILD_STRING             3
                      172 STORE_FAST               6 (edit_url)
          
-         400     >>  174 LOAD_GLOBAL             17 (NULL + FeditFieldEditButton)
+         371     >>  174 LOAD_GLOBAL             17 (NULL + FeditFieldEditButton)
                      186 PRECALL                  0
                      190 CALL                     0
          
-         399         200 BUILD_LIST               1
+         370         200 BUILD_LIST               1
                      202 STORE_FAST               8 (items)
          
-         403         204 LOAD_GLOBAL             19 (NULL + hooks)
+         374         204 LOAD_GLOBAL             19 (NULL + hooks)
                      216 LOAD_ATTR               10 (get_hooks)
                      226 LOAD_GLOBAL             22 (CONSTRUCT_FIELD_TOOLBAR)
                      238 PRECALL                  1
                      242 CALL                     1
                      252 GET_ITER
                  >>  254 FOR_ITER                17 (to 290)
                      256 STORE_FAST               9 (hook)
          
-         404         258 PUSH_NULL
+         375         258 PUSH_NULL
                      260 LOAD_FAST                9 (hook)
                      262 LOAD_DEREF               0 (request)
                      264 LOAD_FAST                8 (items)
                      266 LOAD_FAST                3 (model)
                      268 LOAD_FAST                2 (field_name)
                      270 KW_NAMES                 4
                      272 PRECALL                  4
                      276 CALL                     4
                      286 POP_TOP
                      288 JUMP_BACKWARD           18 (to 254)
          
-         406     >>  290 LOAD_CLOSURE             0 (request)
+         377     >>  290 LOAD_CLOSURE             0 (request)
                      292 BUILD_TUPLE              1
-                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 406>)
+                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 377>)
                      296 MAKE_FUNCTION            8 (closure)
                      298 LOAD_FAST                8 (items)
                      300 GET_ITER
                      302 PRECALL                  0
                      306 CALL                     0
                      316 STORE_FAST               8 (items)
          
-         407         318 LOAD_GLOBAL             25 (NULL + list)
+         378         318 LOAD_GLOBAL             25 (NULL + list)
                      330 LOAD_GLOBAL             27 (NULL + filter)
                      342 LOAD_CONST               0 (None)
                      344 LOAD_FAST                8 (items)
                      346 PRECALL                  2
                      350 CALL                     2
                      360 PRECALL                  1
                      364 CALL                     1
                      374 STORE_FAST               8 (items)
          
-         409         376 LOAD_FAST                2 (field_name)
+         380         376 LOAD_FAST                2 (field_name)
                      378 LOAD_FAST                5 (kwargs)
                      380 LOAD_CONST               6 ('wagtail_fedit_field_name')
                      382 STORE_SUBSCR
          
-         410         386 LOAD_FAST                3 (model)
+         381         386 LOAD_FAST                3 (model)
                      388 LOAD_FAST                5 (kwargs)
                      390 LOAD_CONST               7 ('wagtail_fedit_instance')
                      392 STORE_SUBSCR
          
-         411         396 LOAD_GLOBAL             29 (NULL + str)
+         382         396 LOAD_GLOBAL             29 (NULL + str)
                      408 LOAD_FAST                5 (kwargs)
                      410 LOAD_METHOD             15 (get)
                      432 LOAD_CONST               8 ('inline')
                      434 LOAD_CONST               9 (False)
                      436 PRECALL                  2
                      440 CALL                     2
                      450 PRECALL                  1
@@ -2232,40 +2004,40 @@
                      490 CALL                     0
                      500 LOAD_CONST              10 ('true')
                      502 COMPARE_OP               2 (==)
                      508 LOAD_FAST                5 (kwargs)
                      510 LOAD_CONST               8 ('inline')
                      512 STORE_SUBSCR
          
-         412         516 LOAD_GLOBAL             35 (NULL + render_to_string)
+         383         516 LOAD_GLOBAL             35 (NULL + render_to_string)
          
-         413         528 LOAD_CONST              11 ('wagtail_fedit/content/editable_field.html')
+         384         528 LOAD_CONST              11 ('wagtail_fedit/content/editable_field.html')
          
-         415         530 LOAD_FAST                6 (edit_url)
+         386         530 LOAD_FAST                6 (edit_url)
          
-         416         532 LOAD_FAST                2 (field_name)
+         387         532 LOAD_FAST                2 (field_name)
          
-         417         534 LOAD_FAST                3 (model)
+         388         534 LOAD_FAST                3 (model)
          
-         418         536 LOAD_FAST                1 (content)
+         389         536 LOAD_FAST                1 (content)
          
-         419         538 LOAD_FAST                4 (context)
+         390         538 LOAD_FAST                4 (context)
          
-         420         540 LOAD_FAST                8 (items)
+         391         540 LOAD_FAST                8 (items)
          
-         414         542 LOAD_CONST              12 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items'))
+         385         542 LOAD_CONST              12 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items'))
                      544 BUILD_CONST_KEY_MAP      6
          
-         421         546 LOAD_FAST                5 (kwargs)
+         392         546 LOAD_FAST                5 (kwargs)
          
-         414         548 DICT_UPDATE              1
+         385         548 DICT_UPDATE              1
          
-         423         550 LOAD_DEREF               0 (request)
+         394         550 LOAD_DEREF               0 (request)
          
-         412         552 KW_NAMES                13
+         383         552 KW_NAMES                13
                      554 PRECALL                  3
                      558 CALL                     3
                      568 RETURN_VALUE
          consts
             None
             'wagtail_fedit:edit_field'
             ('args',)
@@ -2277,15 +2049,15 @@
                stacksize : 5
                flags     : 19
                code
                   0x9501970067007c005d177d017c01a00000000000000000000000000000
                   000000000000008902a6010000ab01000000000000000091028c185300
                              0 COPY_FREE_VARS           1
                
-               406           2 RESUME                   0
+               377           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                23 (to 56)
                             10 STORE_FAST               1 (item)
                             12 LOAD_FAST                1 (item)
                             14 LOAD_METHOD              0 (render)
                             36 LOAD_DEREF               2 (request)
@@ -2295,38 +2067,224 @@
                             54 JUMP_BACKWARD           24 (to 8)
                        >>   56 RETURN_VALUE
                consts
                names      ('render',)
                varnames   ('.0', 'item')
                freevars   ('request',)
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '<listcomp>'
-               firstlineno 406
+               firstlineno 377
                lnotab 0x
             'wagtail_fedit_field_name'
             'wagtail_fedit_instance'
             'inline'
             False
             'true'
             'wagtail_fedit/content/editable_field.html'
             ('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items')
             ('request',)
             ()
          names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack', 'FeditFieldEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_FIELD_TOOLBAR', 'list', 'filter', 'str', 'get', 'lower', 'render_to_string')
          varnames   ('request', 'content', 'field_name', 'model', 'context', 'kwargs', 'edit_url', 'packed', 'items', 'hook')
          freevars   ()
          cellvars   ('request',)
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_editable_field'
-         firstlineno 387
+         firstlineno 358
          lnotab
             0x04010c0102013cfe120504010c0120ff10030e031aff0404360120021c
             013a020a010a0178010c0102020201020102010201020102fa040702f902
             0902f5
+      code
+         argcount  : 6
+         nlocals   : 10
+         stacksize : 14
+         flags     : 11
+         code
+            0x870097007401000000000000000000007c04890064017c029b0064029d
+            03ac03a6030000ab0300000000000000007d077403000000000000000000
+            00a6000000ab00000000000000000067017d087405000000000000000000
+            006a030000000000000000740800000000000000000000a6010000ab0100
+            0000000000000044005d127d0902007c0989007c087c047c027c03ac04a6
+            050000ab05000000000000000001008c1388006601640584087c084400a6
+            000000ab0000000000000000007d08740b00000000000000000000740d00
+            00000000000000000064007c08a6020000ab020000000000000000a60100
+            00ab0100000000000000007d08740f000000000000000000006406741100
+            0000000000000000006a0900000000000000007c027c03660264077c0469
+            017c06a4018e017c077c027c047c017c037c057c037c047c0864089c0aa6
+            020000ab0200000000000000005300
+                       0 MAKE_CELL                0 (request)
+         
+         397           2 RESUME                   0
+         
+         398           4 LOAD_GLOBAL              1 (NULL + edit_url)
+         
+         399          16 LOAD_FAST                4 (model)
+         
+         400          18 LOAD_DEREF               0 (request)
+         
+         401          20 LOAD_CONST               1 ('block-')
+                      22 LOAD_FAST                2 (block_id)
+                      24 FORMAT_VALUE             0
+                      26 LOAD_CONST               2 ('-section')
+                      28 BUILD_STRING             3
+         
+         398          30 KW_NAMES                 3
+                      32 PRECALL                  3
+                      36 CALL                     3
+                      46 STORE_FAST               7 (admin_edit_url)
+         
+         405          48 LOAD_GLOBAL              3 (NULL + FeditBlockEditButton)
+                      60 PRECALL                  0
+                      64 CALL                     0
+         
+         404          74 BUILD_LIST               1
+                      76 STORE_FAST               8 (items)
+         
+         408          78 LOAD_GLOBAL              5 (NULL + hooks)
+                      90 LOAD_ATTR                3 (get_hooks)
+                     100 LOAD_GLOBAL              8 (CONSTRUCT_BLOCK_TOOLBAR)
+                     112 PRECALL                  1
+                     116 CALL                     1
+                     126 GET_ITER
+                 >>  128 FOR_ITER                18 (to 166)
+                     130 STORE_FAST               9 (hook)
+         
+         409         132 PUSH_NULL
+                     134 LOAD_FAST                9 (hook)
+                     136 LOAD_DEREF               0 (request)
+                     138 LOAD_FAST                8 (items)
+                     140 LOAD_FAST                4 (model)
+                     142 LOAD_FAST                2 (block_id)
+                     144 LOAD_FAST                3 (field_name)
+                     146 KW_NAMES                 4
+                     148 PRECALL                  5
+                     152 CALL                     5
+                     162 POP_TOP
+                     164 JUMP_BACKWARD           19 (to 128)
+         
+         411     >>  166 LOAD_CLOSURE             0 (request)
+                     168 BUILD_TUPLE              1
+                     170 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 411>)
+                     172 MAKE_FUNCTION            8 (closure)
+                     174 LOAD_FAST                8 (items)
+                     176 GET_ITER
+                     178 PRECALL                  0
+                     182 CALL                     0
+                     192 STORE_FAST               8 (items)
+         
+         412         194 LOAD_GLOBAL             11 (NULL + list)
+                     206 LOAD_GLOBAL             13 (NULL + filter)
+                     218 LOAD_CONST               0 (None)
+                     220 LOAD_FAST                8 (items)
+                     222 PRECALL                  2
+                     226 CALL                     2
+                     236 PRECALL                  1
+                     240 CALL                     1
+                     250 STORE_FAST               8 (items)
+         
+         414         252 LOAD_GLOBAL             15 (NULL + render_to_string)
+         
+         415         264 LOAD_CONST               6 ('wagtail_fedit/content/editable_block.html')
+         
+         417         266 LOAD_GLOBAL             17 (NULL + BlockEditNode)
+                     278 LOAD_ATTR                9 (get_edit_url)
+         
+         418         288 LOAD_FAST                2 (block_id)
+                     290 LOAD_FAST                3 (field_name)
+         
+         417         292 BUILD_TUPLE              2
+                     294 LOAD_CONST               7 ('instance')
+         
+         419         296 LOAD_FAST                4 (model)
+         
+         417         298 BUILD_MAP                1
+         
+         420         300 LOAD_FAST                6 (kwargs)
+         
+         417         302 DICT_MERGE               1
+                     304 CALL_FUNCTION_EX         1
+         
+         422         306 LOAD_FAST                7 (admin_edit_url)
+         
+         423         308 LOAD_FAST                2 (block_id)
+         
+         424         310 LOAD_FAST                4 (model)
+         
+         425         312 LOAD_FAST                1 (content)
+         
+         426         314 LOAD_FAST                3 (field_name)
+         
+         427         316 LOAD_FAST                5 (context)
+         
+         428         318 LOAD_FAST                3 (field_name)
+         
+         429         320 LOAD_FAST                4 (model)
+         
+         430         322 LOAD_FAST                8 (items)
+         
+         416         324 LOAD_CONST               8 (('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items'))
+                     326 BUILD_CONST_KEY_MAP     10
+         
+         414         328 PRECALL                  2
+                     332 CALL                     2
+                     342 RETURN_VALUE
+         consts
+            None
+            'block-'
+            '-section'
+            ('hash',)
+            ('request', 'items', 'model', 'block_id', 'field_name')
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 5
+               flags     : 19
+               code
+                  0x9501970067007c005d177d017c01a00000000000000000000000000000
+                  000000000000008902a6010000ab01000000000000000091028c185300
+                             0 COPY_FREE_VARS           1
+               
+               411           2 RESUME                   0
+                             4 BUILD_LIST               0
+                             6 LOAD_FAST                0 (.0)
+                       >>    8 FOR_ITER                23 (to 56)
+                            10 STORE_FAST               1 (item)
+                            12 LOAD_FAST                1 (item)
+                            14 LOAD_METHOD              0 (render)
+                            36 LOAD_DEREF               2 (request)
+                            38 PRECALL                  1
+                            42 CALL                     1
+                            52 LIST_APPEND              2
+                            54 JUMP_BACKWARD           24 (to 8)
+                       >>   56 RETURN_VALUE
+               consts
+               names      ('render',)
+               varnames   ('.0', 'item')
+               freevars   ('request',)
+               cellvars   ()
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               name       '<listcomp>'
+               firstlineno 411
+               lnotab 0x
+            'wagtail_fedit/content/editable_block.html'
+            'instance'
+            ('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items')
+         names      ('edit_url', 'FeditBlockEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_BLOCK_TOOLBAR', 'list', 'filter', 'render_to_string', 'BlockEditNode', 'get_edit_url')
+         varnames   ('request', 'content', 'block_id', 'field_name', 'model', 'context', 'kwargs', 'admin_edit_url', 'items', 'hook')
+         freevars   ()
+         cellvars   ('request',)
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         name       'render_editable_block'
+         firstlineno 397
+         lnotab
+            0x04010c01020102010afd12071aff0404360122021c013a020c01020216
+            0104ff040202fe020302fd04050201020102010201020102010201020102
+            f204fe
       'kwarg_list'
       'tokens'
       'return'
       code
          argcount  : 3
          nlocals   : 9
          stacksize : 5
@@ -2339,247 +2297,110 @@
             0064036b020000000072307c03720f7407000000000000000000006404a6
             010000ab01000000000000000082017c00a0040000000000000000000000
             0000000000000000007c06a6010000ab0100000000000000007c047c017c
             05190000000000000000003c0000008c5d7c076405190000000000000000
             007d087c00a00400000000000000000000000000000000000000007c0764
             0319000000000000000000a6010000ab0100000000000000007c047c083c
             00000064067d038c867c045300
-         426           0 RESUME                   0
+         435           0 RESUME                   0
          
-         427           2 LOAD_CONST               1 (False)
+         436           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               3 (had_kwargs)
          
-         428           6 BUILD_MAP                0
+         437           6 BUILD_MAP                0
                        8 STORE_FAST               4 (kwargs)
          
-         433          10 LOAD_GLOBAL              1 (NULL + enumerate)
+         442          10 LOAD_GLOBAL              1 (NULL + enumerate)
                       22 LOAD_FAST                2 (tokens)
                       24 PRECALL                  1
                       28 CALL                     1
                       38 GET_ITER
                  >>   40 FOR_ITER               133 (to 308)
                       42 UNPACK_SEQUENCE          2
                       46 STORE_FAST               5 (i)
                       48 STORE_FAST               6 (token)
          
-         434          50 LOAD_FAST                6 (token)
+         443          50 LOAD_FAST                6 (token)
                       52 LOAD_METHOD              1 (split)
                       74 LOAD_CONST               2 ('=')
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               7 (split)
          
-         435          92 LOAD_GLOBAL              5 (NULL + len)
+         444          92 LOAD_GLOBAL              5 (NULL + len)
                      104 LOAD_FAST                7 (split)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               3 (1)
                      122 COMPARE_OP               2 (==)
                      128 POP_JUMP_FORWARD_IF_FALSE    48 (to 226)
          
-         436         130 LOAD_FAST                3 (had_kwargs)
+         445         130 LOAD_FAST                3 (had_kwargs)
                      132 POP_JUMP_FORWARD_IF_FALSE    15 (to 164)
          
-         437         134 LOAD_GLOBAL              7 (NULL + ValueError)
+         446         134 LOAD_GLOBAL              7 (NULL + ValueError)
                      146 LOAD_CONST               4 ('Unexpected positional argument after keyword argument')
                      148 PRECALL                  1
                      152 CALL                     1
                      162 RAISE_VARARGS            1
          
-         439     >>  164 LOAD_FAST                0 (parser)
+         448     >>  164 LOAD_FAST                0 (parser)
                      166 LOAD_METHOD              4 (compile_filter)
                      188 LOAD_FAST                6 (token)
                      190 PRECALL                  1
                      194 CALL                     1
                      204 LOAD_FAST                4 (kwargs)
                      206 LOAD_FAST                1 (kwarg_list)
                      208 LOAD_FAST                5 (i)
                      210 BINARY_SUBSCR
                      220 STORE_SUBSCR
                      224 JUMP_BACKWARD           93 (to 40)
          
-         441     >>  226 LOAD_FAST                7 (split)
+         450     >>  226 LOAD_FAST                7 (split)
                      228 LOAD_CONST               5 (0)
                      230 BINARY_SUBSCR
                      240 STORE_FAST               8 (key)
          
-         445         242 LOAD_FAST                0 (parser)
+         454         242 LOAD_FAST                0 (parser)
                      244 LOAD_METHOD              4 (compile_filter)
                      266 LOAD_FAST                7 (split)
                      268 LOAD_CONST               3 (1)
                      270 BINARY_SUBSCR
                      280 PRECALL                  1
                      284 CALL                     1
                      294 LOAD_FAST                4 (kwargs)
                      296 LOAD_FAST                8 (key)
                      298 STORE_SUBSCR
          
-         446         302 LOAD_CONST               6 (True)
+         455         302 LOAD_CONST               6 (True)
                      304 STORE_FAST               3 (had_kwargs)
                      306 JUMP_BACKWARD          134 (to 40)
          
-         448     >>  308 LOAD_FAST                4 (kwargs)
+         457     >>  308 LOAD_FAST                4 (kwargs)
                      310 RETURN_VALUE
          consts
             None
             False
             '='
             1
             'Unexpected positional argument after keyword argument'
             0
             True
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter')
          varnames   ('parser', 'kwarg_list', 'tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 426
+         firstlineno 435
          lnotab 0x02010401040528012a01260104011e023e0210043c010602
-      'obj'
-      code
-         argcount  : 2
-         nlocals   : 2
-         stacksize : 5
-         flags     : 3
-         code
-            0x97007c0072027c017302640153007c006a0000000000000000006a0100
-            000000000000000c0070657c006a000000000000000000a0020000000000
-            0000000000000000000000000000006402a6010000ab0100000000000000
-            000c00704a7c006a000000000000000000a0020000000000000000000000
-            0000000000000000007c016a0300000000000000006a0400000000000000
-            009b0064037c016a0300000000000000006a0500000000000000009b009d
-            03a6010000ab0100000000000000000c007016740d000000000000000000
-            007c00740e000000000000000000006401a6030000ab0300000000000000
-            000c000c005300
-         451           0 RESUME                   0
-         
-         452           2 LOAD_FAST                0 (request)
-                       4 POP_JUMP_FORWARD_IF_FALSE     2 (to 10)
-                       6 LOAD_FAST                1 (obj)
-                       8 POP_JUMP_FORWARD_IF_TRUE     2 (to 14)
-         
-         453     >>   10 LOAD_CONST               1 (False)
-                      12 RETURN_VALUE
-         
-         456     >>   14 LOAD_FAST                0 (request)
-                      16 LOAD_ATTR                0 (user)
-                      26 LOAD_ATTR                1 (is_authenticated)
-                      36 UNARY_NOT
-                      38 JUMP_IF_TRUE_OR_POP    101 (to 242)
-         
-         457          40 LOAD_FAST                0 (request)
-                      42 LOAD_ATTR                0 (user)
-                      52 LOAD_METHOD              2 (has_perm)
-                      74 LOAD_CONST               2 ('wagtailadmin.access_admin')
-                      76 PRECALL                  1
-                      80 CALL                     1
-                      90 UNARY_NOT
-         
-         456          92 JUMP_IF_TRUE_OR_POP     74 (to 242)
-         
-         458          94 LOAD_FAST                0 (request)
-                      96 LOAD_ATTR                0 (user)
-                     106 LOAD_METHOD              2 (has_perm)
-                     128 LOAD_FAST                1 (obj)
-                     130 LOAD_ATTR                3 (_meta)
-                     140 LOAD_ATTR                4 (app_label)
-                     150 FORMAT_VALUE             0
-                     152 LOAD_CONST               3 ('.change_')
-                     154 LOAD_FAST                1 (obj)
-                     156 LOAD_ATTR                3 (_meta)
-                     166 LOAD_ATTR                5 (model_name)
-                     176 FORMAT_VALUE             0
-                     178 BUILD_STRING             3
-                     180 PRECALL                  1
-                     184 CALL                     1
-                     194 UNARY_NOT
-         
-         456         196 JUMP_IF_TRUE_OR_POP     22 (to 242)
-         
-         459         198 LOAD_GLOBAL             13 (NULL + getattr)
-                     210 LOAD_FAST                0 (request)
-                     212 LOAD_GLOBAL             14 (FEDIT_PREVIEW_VAR)
-                     224 LOAD_CONST               1 (False)
-                     226 PRECALL                  3
-                     230 CALL                     3
-                     240 UNARY_NOT
-         
-         455     >>  242 UNARY_NOT
-                     244 RETURN_VALUE
-         consts
-            None
-            False
-            'wagtailadmin.access_admin'
-            '.change_'
-         names      ('user', 'is_authenticated', 'has_perm', '_meta', 'app_label', 'model_name', 'getattr', 'FEDIT_PREVIEW_VAR')
-         varnames   ('request', 'obj')
-         freevars   ()
-         cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
-         name       '_can_edit'
-         firstlineno 451
-         lnotab 0x0201080104031a0134ff020266fe02032cfc
-      code
-         argcount  : 3
-         nlocals   : 5
-         stacksize : 5
-         flags     : 15
-         code
-            0x97007c017c00760072087c007c01190000000000000000005300740100
-            0000000000000000007c02a6010000ab010000000000000000720802007c
-            027c0369007c04a4018e017d027c027c007c013c0000007c025300
-         463           0 RESUME                   0
-         
-         464           2 LOAD_FAST                1 (key)
-                       4 LOAD_FAST                0 (context)
-                       6 CONTAINS_OP              0
-                       8 POP_JUMP_FORWARD_IF_FALSE     8 (to 26)
-         
-         465          10 LOAD_FAST                0 (context)
-                      12 LOAD_FAST                1 (key)
-                      14 BINARY_SUBSCR
-                      24 RETURN_VALUE
-         
-         467     >>   26 LOAD_GLOBAL              1 (NULL + callable)
-                      38 LOAD_FAST                2 (value)
-                      40 PRECALL                  1
-                      44 CALL                     1
-                      54 POP_JUMP_FORWARD_IF_FALSE     8 (to 72)
-         
-         468          56 PUSH_NULL
-                      58 LOAD_FAST                2 (value)
-                      60 LOAD_FAST                3 (args)
-                      62 BUILD_MAP                0
-                      64 LOAD_FAST                4 (kwargs)
-                      66 DICT_MERGE               1
-                      68 CALL_FUNCTION_EX         1
-                      70 STORE_FAST               2 (value)
-         
-         470     >>   72 LOAD_FAST                2 (value)
-                      74 LOAD_FAST                0 (context)
-                      76 LOAD_FAST                1 (key)
-                      78 STORE_SUBSCR
-         
-         471          82 LOAD_FAST                2 (value)
-                      84 RETURN_VALUE
-         consts
-            None
-         names      ('callable',)
-         varnames   ('context', 'key', 'value', 'args', 'kwargs')
-         freevars   ()
-         cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
-         name       '_get_from_context_or_set'
-         firstlineno 463
-         lnotab 0x0201080110021e0110020a01
-   names      ('django.template', 'library', 'Node', 'NodeList', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'django.db', 'models', 'wagtail.blocks', 'BoundBlock', 'wagtail.models', 'Page', 'wagtail', 'hooks', 'urllib.parse', 'urlencode', 'warnings', 'toolbar', 'FeditBlockEditButton', 'FeditFieldEditButton', 'utils', 'FEDIT_PREVIEW_VAR', 'get_field_content', 'CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR', 'Library', 'register', 'TimestampSigner', 'url_value_signer', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'BlockEditNode', 'tag', 'do_render_fedit_block', 'FieldEditNode', 'do_render_fedit_field', 'render_editable_field', 'list', 'str', 'dict', 'get_kwargs', 'Model', '_can_edit', '_get_from_context_or_set')
+   names      ('django.template', 'library', 'Node', 'NodeList', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'django.db', 'models', 'wagtail.blocks', 'BoundBlock', 'wagtail', 'hooks', 'urllib.parse', 'urlencode', 'warnings', 'toolbar', 'FeditBlockEditButton', 'FeditFieldEditButton', 'utils', '_can_edit', 'edit_url', 'get_field_content', '_resolve_expressions', 'CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR', 'Library', 'register', 'TimestampSigner', 'url_value_signer', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'BlockEditNode', 'tag', 'do_render_fedit_block', 'FieldEditNode', 'do_render_fedit_field', 'render_editable_field', 'render_editable_block', 'list', 'str', 'dict', 'get_kwargs')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020114010c0110010c010c010c010c010c020c010c010c010c0208
-      021004100110061e011e03040104031c7f00442a010eff0e01023b1c352a
-      010eff0e01022a06273019160c
+      0x00ff020114010c0110010c010c010c010c010c020c010c010c02080210
+      04180610061e011e03040104031c7f001d2a010eff0e01023b1c3b2a010e
+      ff0e01022a06270626
```

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.4.3/wagtail_fedit/templatetags/fedit.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,25 +4,29 @@
 from django.template.base import FilterExpression
 from django.utils.safestring import mark_safe
 from django.urls import reverse
 from django.core import signing
 from django.db import models
 
 from wagtail.blocks import BoundBlock
-from wagtail.models import Page
 from wagtail import hooks
 from urllib.parse import urlencode
 
 import warnings
 
 from ..toolbar import (
     FeditBlockEditButton,
     FeditFieldEditButton,
 )
-from ..utils import FEDIT_PREVIEW_VAR, get_field_content
+from ..utils import (
+    _can_edit,
+    edit_url,
+    get_field_content,
+    _resolve_expressions,
+)
 from ..hooks import (
     CONSTRUCT_BLOCK_TOOLBAR,
     CONSTRUCT_FIELD_TOOLBAR,
 )
 
 
 register = library.Library()
@@ -64,22 +68,16 @@
         for k, e in extra.items():
             if isinstance(e, FilterExpression):
                 extra[k] = e.resolve(context)
 
         if not field_name and "wagtail_fedit_field_name" in context:
             field_name = context["wagtail_fedit_field_name"]
 
-        if isinstance(block, FilterExpression):
-            block = block.resolve(context)
-        if isinstance(block_id, FilterExpression):
-            block_id = block_id.resolve(context)
-        if isinstance(field_name, FilterExpression):
-            field_name = field_name.resolve(context)
-        if isinstance(model, FilterExpression):
-            model = model.resolve(context)
+        block, block_id, field_name, model =\
+            _resolve_expressions(context, block, block_id, field_name, model)
         
         if not block_id and "block_id" not in context and not block:
             raise ValueError("Block ID is required")
         
         # `wagtail_fedit_instance` is provided after the form is saved.
         # This allows us to easily use the same instance across multiple views.
         # Model will only be provided initially when the block is rendered.
@@ -129,60 +127,27 @@
             rendered = mark_safe("")
 
         # Check if the user has permission to edit the block.
         request = context.get("request")
         if not _can_edit(request, model):
             return rendered
 
-        # If the model is a page, we can redirect the user to the page editor.
-        # This will act as a shortcut; jumping to the block inside of the admin.
-        if isinstance(model, Page):
-            admin_edit_url = _get_from_context_or_set(
-                context, "page_base_edit_url",
-                lambda: reverse(
-                    "wagtailadmin_pages:edit",
-                    args=[model.id],
-                ),
-            )
-            admin_edit_url = f"{admin_edit_url}#block-{block_id}-section"
-        else:
-            admin_edit_url = None
-
-        extra["has_block"] = self.has_block
+        if self.has_block:
+            extra["has_block"] = self.has_block
 
-        items = [
-            FeditBlockEditButton(),
-        ]
-
-        for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR):
-            hook(request=request, items=items, model=model, block_id=block_id, field_name=field_name)
-
-        items = [item.render(request) for item in items]
-        items = list(filter(None, items))
-        
-        return render_to_string(
-            "wagtail_fedit/content/editable_block.html",
-            {
-                "edit_url": self.get_edit_url(
-                    block_id, field_name,
-                    instance=model,
-                    **extra,
-                ),
-                "admin_edit_url": admin_edit_url,
-                "block_id": block_id,
-                "model": model,
-                "content": rendered,
-                "field_name": field_name,
-                "parent_context": context,
-                "wagtail_fedit_field_name": field_name,
-                "wagtail_fedit_instance": model,
-                "toolbar_items": items,
-            }
+        return render_editable_block(
+            request=request,
+            content=rendered,
+            block_id=block_id,
+            field_name=field_name,
+            model=model,
+            context=context,
+            **extra,
         )
-    
+
     @staticmethod
     def pack(**kwargs) -> dict:
 
         packed = {}
         for k, v in kwargs.items():
             packed[k] = url_value_signer.sign(str(v))
 
@@ -297,19 +262,16 @@
         self.kwargs = kwargs
 
     def render(self, context):
         getters = self.getters
         model = self.model
         inline = self.inline
 
-        if isinstance(model, FilterExpression):
-            model = model.resolve(context)
-
-        if isinstance(inline, FilterExpression):
-            inline = inline.resolve(context)
+        model, inline =\
+            _resolve_expressions(context, model, inline)
 
         obj = model
         for i in range(len(getters) - 1):
             getter = getters[i]
             try:
                 obj = getattr(obj, getter)
             except AttributeError:
@@ -327,22 +289,28 @@
             content = mark_safe("")
             # Force inline editing if no content is available.
             # This will make sure the height of the field to edit is not 0.
             inline = True
 
         if not _can_edit(request, obj):
             return content
-            
+
+        for k, v in self.kwargs.items():
+            if isinstance(v, FilterExpression):
+                self.kwargs[k] = v.resolve(context)
+                  
+        if inline:
+            self.kwargs["inline"] = True
+  
         return render_editable_field(
             request=request, 
             content=content,
             field_name=self.field, 
             model=obj,
             context=context,
-            inline=inline,
             **self.kwargs,
         )
     
 
 
 @register.tag(name="fedit_field")
 def do_render_fedit_field(parser: Parser, token: Token):
@@ -422,14 +390,52 @@
             "parent_context": context,
             "toolbar_items": items,
             **kwargs,
         },
         request=request,
     )
 
+def render_editable_block(request, content, block_id, field_name, model, context, **kwargs):
+        admin_edit_url = edit_url(
+            model,
+            request,
+            hash=f"block-{block_id}-section",
+        )
+
+        items = [
+            FeditBlockEditButton(),
+        ]
+
+        for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR):
+            hook(request=request, items=items, model=model, block_id=block_id, field_name=field_name)
+
+        items = [item.render(request) for item in items]
+        items = list(filter(None, items))
+        
+        return render_to_string(
+            "wagtail_fedit/content/editable_block.html",
+            {
+                "edit_url": BlockEditNode.get_edit_url(
+                    block_id, field_name,
+                    instance=model,
+                    **kwargs,
+                ),
+                "admin_edit_url": admin_edit_url,
+                "block_id": block_id,
+                "model": model,
+                "content": content,
+                "field_name": field_name,
+                "parent_context": context,
+                "wagtail_fedit_field_name": field_name,
+                "wagtail_fedit_instance": model,
+                "toolbar_items": items,
+            }
+        )
+
+
 def get_kwargs(parser: Parser, kwarg_list: list[str], tokens: list[str]) -> dict:
     had_kwargs = False
     kwargs = {}
 
     # if len(tokens) > len(kwargs_names):
     #     raise ValueError("Invalid number of arguments provided, expected at most %d" % len(kwargs_names))
 
@@ -446,30 +452,7 @@
             #     raise ValueError(f"Unexpected keyword argument {key}")
             
             kwargs[key] = parser.compile_filter(split[1])
             had_kwargs = True
 
     return kwargs
 
-
-def _can_edit(request, obj: models.Model):
-    if not request or not obj:
-        return False
-    
-    return not (
-        not request.user.is_authenticated\
-        or not request.user.has_perm("wagtailadmin.access_admin")\
-        or not request.user.has_perm(f"{obj._meta.app_label}.change_{obj._meta.model_name}")\
-        or not getattr(request, FEDIT_PREVIEW_VAR, False)
-    )
-
-
-def _get_from_context_or_set(context, key, value, *args, **kwargs):
-    if key in context:
-        return context[key]
-    
-    if callable(value):
-        value = value(*args, **kwargs)
-
-    context[key] = value
-    return value
-
```

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.4.3/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.4.3/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/urls.py` & `wagtail_fedit-1.4.3/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.4.3/wagtail_fedit/views/blocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,25 +120,19 @@
                 "data-block-name": self.block.block.name,
             },
         }
         can = {
             "form_class": self.form_class,
         }
 
-        if isinstance(self.instance, Page):
-            admin_edit_url = reverse(
-                "wagtailadmin_pages:edit",
-                args=[self.instance.pk],
-            )
-            admin_edit_url = f"{admin_edit_url}#block-{self.block_id}-section"
-        else:
-            admin_edit_url = None
-
-
-        must["admin_edit_url"] = admin_edit_url
+        must["admin_edit_url"] = utils.edit_url(
+            self.instance,
+            self.request,
+            hash=f"block-{self.block_id}-section",
+        )
 
         context.update(must)
         for key, value in can.items():
             context.setdefault(key, value)
 
         return context
```

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.4.3/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.4.3/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.4.3/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.4.3/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.4.2
+Version: 1.4.3
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.2 Summary: An
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.3 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.4.2/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.4.3/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,18 @@
 wagtail_fedit/test/core/migrations/0002_basicmodel.py
 wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
 wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
 wagtail_fedit/test/core/migrations/__init__.py
 wagtail_fedit/test/core/tests/__init__.py
 wagtail_fedit/test/core/tests/base.py
 wagtail_fedit/test/core/tests/test_block_edit.py
+wagtail_fedit/test/core/tests/test_block_templatetag.py
 wagtail_fedit/test/core/tests/test_blocks.py
 wagtail_fedit/test/core/tests/test_field_edit.py
+wagtail_fedit/test/core/tests/test_field_templatetag.py
 wagtail_fedit/test/core/tests/test_revision.py
 wagtail_fedit/test/core/tests/test_submit.py
 wagtail_fedit/test/testapp/__init__.py
 wagtail_fedit/test/testapp/asgi.py
 wagtail_fedit/test/testapp/settings.py
 wagtail_fedit/test/testapp/urls.py
 wagtail_fedit/test/testapp/wsgi.py
```

