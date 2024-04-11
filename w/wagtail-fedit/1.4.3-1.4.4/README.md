# Comparing `tmp/wagtail_fedit-1.4.3.tar.gz` & `tmp/wagtail_fedit-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.4.3.tar", last modified: Wed Apr 10 11:12:58 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.4.4.tar", last modified: Thu Apr 11 09:10:02 2024, max compression
```

## Comparing `wagtail_fedit-1.4.3.tar` & `wagtail_fedit-1.4.4.tar`

### file list

```diff
@@ -1,111 +1,121 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.050708 wagtail_fedit-1.4.3/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0    12947 2024-04-10 11:12:58.050708 wagtail_fedit-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0    11954 2024-04-08 20:13:14.000000 wagtail_fedit-1.4.3/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-10 11:12:58.065328 wagtail_fedit-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.816558 wagtail_fedit-1.4.3/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.3/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.3/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.3/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.864208 wagtail_fedit-1.4.3/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.3/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.4.3/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.3/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     3358 2024-04-10 10:24:35.000000 wagtail_fedit-1.4.3/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.866207 wagtail_fedit-1.4.3/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.3/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.867204 wagtail_fedit-1.4.3/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.3/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.757829 wagtail_fedit-1.4.3/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.758831 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.895693 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.917925 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    15915 2024-04-06 00:14:04.000000 wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.760833 wagtail_fedit-1.4.3/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.762830 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.920885 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.922885 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      302 2024-04-06 22:07:59.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      335 2024-04-06 22:08:01.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.937885 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     1709 2024-04-05 19:42:54.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      789 2024-04-07 05:29:57.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.960915 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.974700 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.010629 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
--rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
--rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
--rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
--rw-rw-rw-   0        0        0     1285 2024-04-06 18:43:26.000000 wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.014256 wagtail_fedit-1.4.3/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.3/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.017296 wagtail_fedit-1.4.3/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    17845 2024-04-10 10:47:44.000000 wagtail_fedit-1.4.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    14527 2024-04-10 10:47:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.018380 wagtail_fedit-1.4.3/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.020393 wagtail_fedit-1.4.3/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.026231 wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.035012 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7039 2024-04-05 23:57:48.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     2996 2024-04-10 10:50:37.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_block_templatetag.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3994 2024-04-10 11:08:06.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_field_templatetag.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     4339 2024-04-06 00:03:48.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.039393 wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.4.3/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      916 2024-04-06 20:43:13.000000 wagtail_fedit-1.4.3/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    15299 2024-04-10 10:23:23.000000 wagtail_fedit-1.4.3/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.043847 wagtail_fedit-1.4.3/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.4.3/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9206 2024-04-09 20:56:25.000000 wagtail_fedit-1.4.3/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0    14621 2024-04-05 23:51:10.000000 wagtail_fedit-1.4.3/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    12225 2024-04-06 19:48:05.000000 wagtail_fedit-1.4.3/wagtail_fedit/views/fields.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.3/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:58.050708 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      160 2024-04-06 18:20:48.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     6061 2024-04-06 18:49:36.000000 wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:12:57.859210 wagtail_fedit-1.4.3/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    12947 2024-04-10 11:12:57.000000 wagtail_fedit-1.4.3/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3588 2024-04-10 11:12:57.000000 wagtail_fedit-1.4.3/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 11:12:57.000000 wagtail_fedit-1.4.3/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-10 11:12:57.000000 wagtail_fedit-1.4.3/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-10 11:12:57.000000 wagtail_fedit-1.4.3/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.536188 wagtail_fedit-1.4.4/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.4/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    13152 2024-04-11 09:10:02.537201 wagtail_fedit-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11954 2024-04-08 20:13:14.000000 wagtail_fedit-1.4.4/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2024-04-11 09:10:02.539230 wagtail_fedit-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.438049 wagtail_fedit-1.4.4/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.4/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.4/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.466314 wagtail_fedit-1.4.4/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.4/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.4.4/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.4/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     3358 2024-04-10 10:24:35.000000 wagtail_fedit-1.4.4/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.413003 wagtail_fedit-1.4.4/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.413003 wagtail_fedit-1.4.4/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.467312 wagtail_fedit-1.4.4/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.4.4/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.4.4/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.469225 wagtail_fedit-1.4.4/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.4/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.470236 wagtail_fedit-1.4.4/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.4/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.4/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.414002 wagtail_fedit-1.4.4/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.414002 wagtail_fedit-1.4.4/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.474225 wagtail_fedit-1.4.4/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.4/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.475300 wagtail_fedit-1.4.4/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    15915 2024-04-06 00:14:04.000000 wagtail_fedit-1.4.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.416515 wagtail_fedit-1.4.4/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.418543 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.476313 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.478309 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      302 2024-04-06 22:07:59.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      335 2024-04-06 22:08:01.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.482939 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      789 2024-04-07 05:29:57.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.488718 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.491207 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.493215 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.495123 wagtail_fedit-1.4.4/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.4/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.497121 wagtail_fedit-1.4.4/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.4/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    17687 2024-04-10 19:17:23.000000 wagtail_fedit-1.4.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14619 2024-04-10 19:17:21.000000 wagtail_fedit-1.4.4/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.498114 wagtail_fedit-1.4.4/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.500905 wagtail_fedit-1.4.4/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.506906 wagtail_fedit-1.4.4/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.515875 wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7106 2024-04-10 12:43:12.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     2996 2024-04-10 10:50:37.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_block_templatetag.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3994 2024-04-10 11:08:06.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_field_templatetag.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     4339 2024-04-06 00:03:48.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.520878 wagtail_fedit-1.4.4/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.4/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.4.4/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      951 2024-04-11 08:07:43.000000 wagtail_fedit-1.4.4/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    15352 2024-04-10 13:08:18.000000 wagtail_fedit-1.4.4/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.527409 wagtail_fedit-1.4.4/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.4.4/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9321 2024-04-11 07:42:21.000000 wagtail_fedit-1.4.4/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0    17100 2024-04-11 08:35:19.000000 wagtail_fedit-1.4.4/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    12413 2024-04-11 07:51:29.000000 wagtail_fedit-1.4.4/wagtail_fedit/views/fields.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.4/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.535410 wagtail_fedit-1.4.4/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      182 2024-04-11 08:26:05.000000 wagtail_fedit-1.4.4/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.4/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.4/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.4.4/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.4.4/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.4/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.4/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     6693 2024-04-11 09:04:42.000000 wagtail_fedit-1.4.4/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:10:02.463318 wagtail_fedit-1.4.4/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    13152 2024-04-11 09:10:02.000000 wagtail_fedit-1.4.4/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3976 2024-04-11 09:10:02.000000 wagtail_fedit-1.4.4/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 09:10:02.000000 wagtail_fedit-1.4.4/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-11 09:10:02.000000 wagtail_fedit-1.4.4/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-11 09:10:02.000000 wagtail_fedit-1.4.4/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.4.3/LICENSE` & `wagtail_fedit-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/PKG-INFO` & `wagtail_fedit-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.4.3
-Summary: An application made for the Django Web Framework.
+Version: 1.4.4
+Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
-License: GPL-3.0-only
+License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 5
+Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 wagtail_fedit
```

#### html2text {}

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.3 Summary: An
-application made for the Django Web Framework. Home-page: https://github.com/
-Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
-License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
-Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: GNU General
-Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP Classifier:
-Topic :: Internet :: WWW/HTTP :: Dynamic Content Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE wagtail_fedit
-============= ![Wagtail FEdit Example](https://github.com/Nigel2392/
-wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
-Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be
-edited on the frontend. # Table of Contents - [Getting Started](#getting-
-started) - [Getting Editing!](#getting-editing) - [Permissions](#permissions) -
-[Revisions](#revisions) - [Workflows](#workflows) - [Logs](#logs) - [Caveats]
-(#caveats) - [Hooks](#hooks) - [Construct Block Toolbar]
-(#wagtail_feditconstruct_block_toolbar) - [Construct Field Toolbar]
-(#wagtail_feditconstruct_field_toolbar) - [Register Type Renderer]
-(#wagtail_feditregister_type_renderer) - [Register Field Renderer]
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.4 Summary: Frontend
+editing for your Wagtail site Home-page: https://github.com/Nigel2392/
+wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
+only Classifier: Environment :: Web Environment Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
+Dynamic Content Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE wagtail_fedit ============= ![Wagtail FEdit Example]
+(https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/
+wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
+Wagtail pages and content-blocks to be edited on the frontend. # Table of
+Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
+editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
+(#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Hooks](#hooks) -
+[Construct Block Toolbar](#wagtail_feditconstruct_block_toolbar) - [Construct
+Field Toolbar](#wagtail_feditconstruct_field_toolbar) - [Register Type
+Renderer](#wagtail_feditregister_type_renderer) - [Register Field Renderer]
 (#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [How your field/block is rendered]
 (#how-your-fieldblock-is-rendered) - [Rendered block output HTML](#rendered-
 block-output-html) - [Rendered field output HTML](#rendered-field-output-html)
 - [Implemented](#implemented) Getting Started --------------- 1. Add
 'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
```

### Comparing `wagtail_fedit-1.4.3/README.md` & `wagtail_fedit-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/setup.cfg` & `wagtail_fedit-1.4.4/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,75 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 342e  ..version = 1.4.
-00000030: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
-00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
-00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
-00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
-00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
-00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
-00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
-000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-000000b0: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-000000c0: 6b64 6f77 6e0d 0a61 7574 686f 7220 3d20  kdown..author = 
-000000d0: 4e69 6765 6c0d 0a61 7574 686f 725f 656d  Nigel..author_em
-000000e0: 6169 6c20 3d20 6e69 6765 6c40 676f 6f64  ail = nigel@good
-000000f0: 6164 7669 6365 2e69 740d 0a75 726c 203d  advice.it..url =
-00000100: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000110: 636f 6d2f 4e69 6765 6c32 3339 322f 7761  com/Nigel2392/wa
-00000120: 6774 6169 6c5f 6665 6469 740d 0a6c 6963  gtail_fedit..lic
-00000130: 656e 7365 203d 2047 504c 2d33 2e30 2d6f  ense = GPL-3.0-o
-00000140: 6e6c 790d 0a63 6c61 7373 6966 6965 7273  nly..classifiers
-00000150: 203d 200d 0a09 456e 7669 726f 6e6d 656e   = ...Environmen
-00000160: 7420 3a3a 2057 6562 2045 6e76 6972 6f6e  t :: Web Environ
-00000170: 6d65 6e74 0d0a 0946 7261 6d65 776f 726b  ment...Framework
-00000180: 203a 3a20 446a 616e 676f 0d0a 0946 7261   :: Django...Fra
-00000190: 6d65 776f 726b 203a 3a20 446a 616e 676f  mework :: Django
-000001a0: 203a 3a20 342e 320d 0a09 496e 7465 6e64   :: 4.2...Intend
-000001b0: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
-000001c0: 6576 656c 6f70 6572 730d 0a09 4c69 6365  evelopers...Lice
-000001d0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-000001e0: 7665 6420 3a3a 2047 4e55 2047 656e 6572  ved :: GNU Gener
-000001f0: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
-00000200: 6520 7633 206f 7220 6c61 7465 7220 2847  e v3 or later (G
-00000210: 504c 7633 2b29 0d0a 094f 7065 7261 7469  PLv3+)...Operati
-00000220: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-00000230: 496e 6465 7065 6e64 656e 740d 0a09 5072  Independent...Pr
-00000240: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000250: 6765 203a 3a20 5079 7468 6f6e 0d0a 0950  ge :: Python...P
-00000260: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000270: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000280: 2033 0d0a 0950 726f 6772 616d 6d69 6e67   3...Programming
-00000290: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002a0: 686f 6e20 3a3a 2033 203a 3a20 4f6e 6c79  hon :: 3 :: Only
-000002b0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000002c0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000002d0: 6e20 3a3a 2033 2e38 0d0a 0950 726f 6772  n :: 3.8...Progr
-000002e0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000002f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
-00000300: 0d0a 0954 6f70 6963 203a 3a20 496e 7465  ...Topic :: Inte
-00000310: 726e 6574 203a 3a20 5757 572f 4854 5450  rnet :: WWW/HTTP
-00000320: 0d0a 0954 6f70 6963 203a 3a20 496e 7465  ...Topic :: Inte
-00000330: 726e 6574 203a 3a20 5757 572f 4854 5450  rnet :: WWW/HTTP
-00000340: 203a 3a20 4479 6e61 6d69 6320 436f 6e74   :: Dynamic Cont
-00000350: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
-00000360: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
-00000370: 655f 6461 7461 203d 2074 7275 650d 0a70  e_data = true..p
-00000380: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-00000390: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-000003a0: 203d 203e 3d33 2e38 0d0a 696e 7374 616c   = >=3.8..instal
-000003b0: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
-000003c0: 446a 616e 676f 203e 3d20 342e 320d 0a09  Django >= 4.2...
-000003d0: 5761 6774 6169 6c20 3e3d 2034 2e32 0d0a  Wagtail >= 4.2..
-000003e0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000003f0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000400: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000030: 340d 0a64 6573 6372 6970 7469 6f6e 203d  4..description =
+00000040: 2046 726f 6e74 656e 6420 6564 6974 696e   Frontend editin
+00000050: 6720 666f 7220 796f 7572 2057 6167 7461  g for your Wagta
+00000060: 696c 2073 6974 650d 0a6c 6f6e 675f 6465  il site..long_de
+00000070: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+00000080: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
+00000090: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+000000a0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+000000b0: 742f 6d61 726b 646f 776e 0d0a 6175 7468  t/markdown..auth
+000000c0: 6f72 203d 204e 6967 656c 0d0a 6175 7468  or = Nigel..auth
+000000d0: 6f72 5f65 6d61 696c 203d 206e 6967 656c  or_email = nigel
+000000e0: 4067 6f6f 6461 6476 6963 652e 6974 0d0a  @goodadvice.it..
+000000f0: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
+00000100: 7468 7562 2e63 6f6d 2f4e 6967 656c 3233  thub.com/Nigel23
+00000110: 3932 2f77 6167 7461 696c 5f66 6564 6974  92/wagtail_fedit
+00000120: 0d0a 6c69 6365 6e73 6520 3d20 4750 4c2d  ..license = GPL-
+00000130: 322e 302d 6f6e 6c79 0d0a 636c 6173 7369  2.0-only..classi
+00000140: 6669 6572 7320 3d20 0d0a 0945 6e76 6972  fiers = ...Envir
+00000150: 6f6e 6d65 6e74 203a 3a20 5765 6220 456e  onment :: Web En
+00000160: 7669 726f 6e6d 656e 740d 0a09 4672 616d  vironment...Fram
+00000170: 6577 6f72 6b20 3a3a 2044 6a61 6e67 6f0d  ework :: Django.
+00000180: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
+00000190: 6a61 6e67 6f20 3a3a 2034 2e32 0d0a 0946  jango :: 4.2...F
+000001a0: 7261 6d65 776f 726b 203a 3a20 5761 6774  ramework :: Wagt
+000001b0: 6169 6c0d 0a09 4672 616d 6577 6f72 6b20  ail...Framework 
+000001c0: 3a3a 2057 6167 7461 696c 203a 3a20 350d  :: Wagtail :: 5.
+000001d0: 0a09 4672 616d 6577 6f72 6b20 3a3a 2057  ..Framework :: W
+000001e0: 6167 7461 696c 203a 3a20 360d 0a09 496e  agtail :: 6...In
+000001f0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000200: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
+00000210: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000220: 7070 726f 7665 6420 3a3a 2047 4e55 2047  pproved :: GNU G
+00000230: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
+00000240: 6365 6e73 6520 7632 206f 7220 6c61 7465  cense v2 or late
+00000250: 7220 2847 504c 7632 2b29 0d0a 094f 7065  r (GPLv2+)...Ope
+00000260: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000270: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+00000280: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000290: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002a0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000002b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002c0: 6e20 3a3a 2033 0d0a 0950 726f 6772 616d  n :: 3...Program
+000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002e0: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
+000002f0: 4f6e 6c79 0d0a 0950 726f 6772 616d 6d69  Only...Programmi
+00000300: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000310: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
+00000320: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000330: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000340: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
+00000350: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000360: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
+00000370: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000380: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000390: 3a20 332e 3131 0d0a 0954 6f70 6963 203a  : 3.11...Topic :
+000003a0: 3a20 496e 7465 726e 6574 203a 3a20 5757  : Internet :: WW
+000003b0: 572f 4854 5450 0d0a 0954 6f70 6963 203a  W/HTTP...Topic :
+000003c0: 3a20 496e 7465 726e 6574 203a 3a20 5757  : Internet :: WW
+000003d0: 572f 4854 5450 203a 3a20 4479 6e61 6d69  W/HTTP :: Dynami
+000003e0: 6320 436f 6e74 656e 740d 0a0d 0a5b 6f70  c Content....[op
+000003f0: 7469 6f6e 735d 0d0a 696e 636c 7564 655f  tions]..include_
+00000400: 7061 636b 6167 655f 6461 7461 203d 2074  package_data = t
+00000410: 7275 650d 0a70 6163 6b61 6765 7320 3d20  rue..packages = 
+00000420: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
+00000430: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
+00000440: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+00000450: 203d 200d 0a09 446a 616e 676f 203e 3d20   = ...Django >= 
+00000460: 342e 320d 0a09 5761 6774 6169 6c20 3e3d  4.2...Wagtail >=
+00000470: 2035 2e32 0d0a 0d0a 5b65 6767 5f69 6e66   5.2....[egg_inf
+00000480: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000490: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+000004a0: 0d0a                                     ..
```

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.4.4/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.4.4/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/hooks.py` & `wagtail_fedit-1.4.4/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/models.py` & `wagtail_fedit-1.4.4/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.4.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.4.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.4.4/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.4.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.4.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.4.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x4c6e1666 (Wed Apr 10 10:47:40 2024 UTC)
-files sz: 14527
+moddate:  0xc1e51666 (Wed Apr 10 19:17:21 2024 UTC)
+files sz: 14619
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -165,15 +165,15 @@
                272 STORE_NAME              39 (WARNING_FIELD_NAME_NOT_AVAILABLE)
    
     37         274 LOAD_CONST              18 ('Model instance is not available in the context for %(object)s.')
                276 STORE_NAME              40 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
    
     40         278 PUSH_NULL
                280 LOAD_BUILD_CLASS
-               282 LOAD_CONST              19 (<code object BlockEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 40>)
+               282 LOAD_CONST              19 (<code object BlockEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 40>)
                284 MAKE_FUNCTION            0
                286 LOAD_CONST              20 ('BlockEditNode')
                288 LOAD_NAME                2 (Node)
                290 PRECALL                  3
                294 CALL                     3
                304 STORE_NAME              41 (BlockEditNode)
    
@@ -185,25 +185,25 @@
                338 CALL                     1
    
    197         348 LOAD_CONST              23 ('parser')
                350 LOAD_NAME                7 (Parser)
                352 LOAD_CONST              24 ('token')
                354 LOAD_NAME                8 (Token)
                356 BUILD_TUPLE              4
-               358 LOAD_CONST              25 (<code object do_render_fedit_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 196>)
+               358 LOAD_CONST              25 (<code object do_render_fedit_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 196>)
                360 MAKE_FUNCTION            4 (annotations)
    
    196         362 PRECALL                  0
                366 CALL                     0
    
    197         376 STORE_NAME              43 (do_render_fedit_block)
    
    256         378 PUSH_NULL
                380 LOAD_BUILD_CLASS
-               382 LOAD_CONST              26 (<code object FieldEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 256>)
+               382 LOAD_CONST              26 (<code object FieldEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 256>)
                384 MAKE_FUNCTION            0
                386 LOAD_CONST              27 ('FieldEditNode')
                388 LOAD_NAME                2 (Node)
                390 PRECALL                  3
                394 CALL                     3
                404 STORE_NAME              44 (FieldEditNode)
    
@@ -215,27 +215,27 @@
                438 CALL                     1
    
    316         448 LOAD_CONST              23 ('parser')
                450 LOAD_NAME                7 (Parser)
                452 LOAD_CONST              24 ('token')
                454 LOAD_NAME                8 (Token)
                456 BUILD_TUPLE              4
-               458 LOAD_CONST              29 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 315>)
+               458 LOAD_CONST              29 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 315>)
                460 MAKE_FUNCTION            4 (annotations)
    
    315         462 PRECALL                  0
                466 CALL                     0
    
    316         476 STORE_NAME              45 (do_render_fedit_field)
    
-   358         478 LOAD_CONST              30 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 358>)
+   358         478 LOAD_CONST              30 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 358>)
                480 MAKE_FUNCTION            0
                482 STORE_NAME              46 (render_editable_field)
    
-   397         484 LOAD_CONST              31 (<code object render_editable_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 397>)
+   397         484 LOAD_CONST              31 (<code object render_editable_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 397>)
                486 MAKE_FUNCTION            0
                488 STORE_NAME              47 (render_editable_block)
    
    435         490 LOAD_CONST              23 ('parser')
                492 LOAD_NAME                7 (Parser)
                494 LOAD_CONST              32 ('kwarg_list')
                496 LOAD_NAME               48 (list)
@@ -244,15 +244,15 @@
                510 LOAD_CONST              33 ('tokens')
                512 LOAD_NAME               48 (list)
                514 LOAD_NAME               49 (str)
                516 BINARY_SUBSCR
                526 LOAD_CONST              34 ('return')
                528 LOAD_NAME               50 (dict)
                530 BUILD_TUPLE              8
-               532 LOAD_CONST              35 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 435>)
+               532 LOAD_CONST              35 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 435>)
                534 MAKE_FUNCTION            4 (annotations)
                536 STORE_NAME              51 (get_kwargs)
                538 LOAD_CONST              12 (None)
                540 RETURN_VALUE
    consts
       0
       ('library', 'Node', 'NodeList')
@@ -291,15 +291,15 @@
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BlockEditNode')
                        8 STORE_NAME               2 (__qualname__)
          
           41          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object UnpackError, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 41>)
+                      14 LOAD_CONST               1 (<code object UnpackError, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 41>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('UnpackError')
                       20 LOAD_NAME                3 (Exception)
                       22 PRECALL                  3
                       26 CALL                     3
                       36 STORE_NAME               4 (UnpackError)
          
@@ -332,28 +332,28 @@
          
           44          66 LOAD_CONST               8 ('model')
          
           49          68 LOAD_NAME                8 (models)
                       70 LOAD_ATTR                9 (Model)
          
           44          80 BUILD_TUPLE             10
-                      82 LOAD_CONST               9 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 44>)
+                      82 LOAD_CONST               9 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 44>)
                       84 MAKE_FUNCTION            5 (defaults, annotations)
                       86 STORE_NAME              10 (__init__)
          
-          60          88 LOAD_CONST              10 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 60>)
+          60          88 LOAD_CONST              10 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 60>)
                       90 MAKE_FUNCTION            0
                       92 STORE_NAME              11 (render)
          
          147          94 LOAD_NAME               12 (staticmethod)
          
          148          96 LOAD_CONST              11 ('return')
                       98 LOAD_NAME               13 (dict)
                      100 BUILD_TUPLE              2
-                     102 LOAD_CONST              12 (<code object pack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 147>)
+                     102 LOAD_CONST              12 (<code object pack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 147>)
                      104 MAKE_FUNCTION            4 (annotations)
          
          147         106 PRECALL                  0
                      110 CALL                     0
          
          148         120 STORE_NAME              14 (pack)
          
@@ -363,15 +363,15 @@
                      126 LOAD_CONST              13 (('request',))
                      128 BUILD_CONST_KEY_MAP      1
                      130 LOAD_CONST              14 ('expected')
                      132 LOAD_NAME                7 (str)
                      134 LOAD_CONST              11 ('return')
                      136 LOAD_NAME               13 (dict)
                      138 BUILD_TUPLE              4
-                     140 LOAD_CONST              15 (<code object unpack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 156>)
+                     140 LOAD_CONST              15 (<code object unpack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 156>)
                      142 MAKE_FUNCTION            6 (kwdefaults, annotations)
          
          156         144 PRECALL                  0
                      148 CALL                     0
          
          157         158 STORE_NAME              16 (unpack)
          
@@ -383,15 +383,15 @@
                      168 LOAD_NAME                7 (str)
                      170 LOAD_CONST              16 ('instance')
                      172 LOAD_NAME                8 (models)
                      174 LOAD_ATTR                9 (Model)
                      184 LOAD_CONST              11 ('return')
                      186 LOAD_NAME                7 (str)
                      188 BUILD_TUPLE              8
-                     190 LOAD_CONST              17 (<code object get_edit_url, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 179>)
+                     190 LOAD_CONST              17 (<code object get_edit_url, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 179>)
                      192 MAKE_FUNCTION            4 (annotations)
          
          179         194 PRECALL                  0
                      198 CALL                     0
          
          180         208 STORE_NAME              17 (get_edit_url)
                      210 LOAD_CONST               3 (None)
@@ -415,15 +415,15 @@
                consts
                   'BlockEditNode.UnpackError'
                   None
                names      ('__name__', '__module__', '__qualname__')
                varnames   ()
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'UnpackError'
                firstlineno 41
                lnotab 0x0a01
             'UnpackError'
             None
             'nodelist'
             'block'
@@ -469,15 +469,15 @@
                             88 RETURN_VALUE
                consts
                   None
                names      ('nl', 'block', 'block_id', 'field_name', 'model', 'extra')
                varnames   ('self', 'nodelist', 'block', 'block_id', 'field_name', 'model', 'extra')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
                firstlineno 44
                lnotab 0x02090e010e010e010e010e01
             code
                argcount  : 2
                nlocals   : 12
                stacksize : 10
@@ -488,45 +488,42 @@
                   006a0400000000000000007d067c06a00500000000000000000000000000
                   00000000000000a6000000ab00000000000000000044005d325c0200007d
                   077d08740d000000000000000000007c08740e00000000000000000000a6
                   020000ab02000000000000000072187c08a0080000000000000000000000
                   0000000000000000007c01a6010000ab0100000000000000007c067c073c
                   0000008c337c04730c64017c01760072087c016401190000000000000000
                   007d047413000000000000000000007c017c027c037c047c05a6050000ab
-                  0500000000000000005c0400007d027d037d047d057c03731564027c0176
-                  0172117c02730f7415000000000000000000006403a6010000ab01000000
-                  000000000082017c0570147c01a00b000000000000000000000000000000
-                  00000000006404a6010000ab0100000000000000007d057c047c0164013c
-                  0000007c057c0164043c0000007c02725a09007c01a00c00000000000000
-                  00000000000000000000000000a6000000ab0000000000000000007d096e
-                  122300741a000000000000000000002400720501007c017d0959006e0477
-                  007803590077017c09a00e00000000000000000000000000000000000000
-                  007c06a6010000ab01000000000000000001007c02a00f00000000000000
-                  000000000000000000000000007c09a6010000ab0100000000000000007d
-                  0a64057c005f1000000000000000006e387c006a11000000000000000072
-                  227c006a110000000000000000a012000000000000000000000000000000
-                  00000000007c01a6010000ab0100000000000000007d0a64067c005f1000
-                  000000000000006e0f7415000000000000000000006407a6010000ab0100
-                  0000000000000082017c0473257427000000000000000000006a14000000
-                  0000000000742a0000000000000000000064087c016a1600000000000000
-                  0069017a060000a6010000ab01000000000000000001007c0a53007c0573
-                  2f7427000000000000000000006a140000000000000000742e0000000000
-                  000000000064087c026a0000000000000000006a1800000000000000006a
-                  19000000000000000069017a060000a6010000ab01000000000000000001
-                  007c0a53007c03730d64027c01760072097c016402190000000000000000
-                  007d036e2d7c03731a7c0272187435000000000000000000007c026409a6
-                  020000ab02000000000000000072087c026a1b00000000000000007d036e
-                  117c03730f7415000000000000000000006403a6010000ab010000000000
-                  00000082017c0a730f743900000000000000000000640aa6010000ab0100
-                  000000000000007d0a7c01a00b0000000000000000000000000000000000
-                  000000640ba6010000ab0100000000000000007d0b743b00000000000000
-                  0000007c0b7c05a6020000ab02000000000000000073027c0a53007c006a
-                  100000000000000000720a7c006a1000000000000000007c06640c3c0000
-                  00743d00000000000000000000640e7c0b7c0a7c037c047c057c01640d9c
-                  067c06a4018e015300
+                  0500000000000000005c0400007d027d037d047d057c0570147c01a00a00
+                  000000000000000000000000000000000000006402a6010000ab01000000
+                  00000000007d057c047c0164013c0000007c057c0164023c0000007c0272
+                  5a09007c01a00b0000000000000000000000000000000000000000a60000
+                  00ab0000000000000000007d096e12230074180000000000000000000024
+                  00720501007c017d0959006e0477007803590077017c09a00d0000000000
+                  0000000000000000000000000000007c06a6010000ab0100000000000000
+                  0001007c02a00e00000000000000000000000000000000000000007c09a6
+                  010000ab0100000000000000007d0a64037c005f0f00000000000000006e
+                  387c006a10000000000000000072227c006a100000000000000000a01100
+                  000000000000000000000000000000000000007c01a6010000ab01000000
+                  00000000007d0a64047c005f0f00000000000000006e0f74250000000000
+                  00000000006405a6010000ab01000000000000000082017c047325742700
+                  0000000000000000006a140000000000000000742a000000000000000000
+                  0064067c016a16000000000000000069017a060000a6010000ab01000000
+                  000000000001007c0a53007c05732f7427000000000000000000006a1400
+                  00000000000000742e0000000000000000000064067c026a000000000000
+                  0000006a1800000000000000006a19000000000000000069017a060000a6
+                  010000ab01000000000000000001007c0a53007c03730d64077c01760072
+                  097c016407190000000000000000007d036e1b7c0373197c027217743500
+                  0000000000000000007c026408a6020000ab02000000000000000072077c
+                  026a1b00000000000000007d037c0a730f74390000000000000000000064
+                  09a6010000ab0100000000000000007d0a7c01a00a000000000000000000
+                  0000000000000000000000640aa6010000ab0100000000000000007d0b74
+                  3b000000000000000000007c0b7c05a6020000ab02000000000000000072
+                  027c0373027c0a53007c006a0f0000000000000000720a7c006a0f000000
+                  00000000007c06640b3c000000743d00000000000000000000640d7c0b7c
+                  0a7c037c047c057c01640c9c067c06a4018e015300
                 60           0 RESUME                   0
                
                 61           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (block)
                             14 STORE_FAST               2 (block)
                
                 62          16 LOAD_FAST                0 (self)
@@ -595,294 +592,270 @@
                
                 75         278 UNPACK_SEQUENCE          4
                            282 STORE_FAST               2 (block)
                            284 STORE_FAST               3 (block_id)
                            286 STORE_FAST               4 (field_name)
                            288 STORE_FAST               5 (model)
                
-                78         290 LOAD_FAST                3 (block_id)
-                           292 POP_JUMP_FORWARD_IF_TRUE    21 (to 336)
-                           294 LOAD_CONST               2 ('block_id')
-                           296 LOAD_FAST                1 (context)
-                           298 CONTAINS_OP              1
-                           300 POP_JUMP_FORWARD_IF_FALSE    17 (to 336)
-                           302 LOAD_FAST                2 (block)
-                           304 POP_JUMP_FORWARD_IF_TRUE    15 (to 336)
-               
-                79         306 LOAD_GLOBAL             21 (NULL + ValueError)
-                           318 LOAD_CONST               3 ('Block ID is required')
+                84         290 LOAD_FAST                5 (model)
+                           292 JUMP_IF_TRUE_OR_POP     20 (to 334)
+                           294 LOAD_FAST                1 (context)
+                           296 LOAD_METHOD             10 (get)
+                           318 LOAD_CONST               2 ('wagtail_fedit_instance')
                            320 PRECALL                  1
                            324 CALL                     1
-                           334 RAISE_VARARGS            1
+                       >>  334 STORE_FAST               5 (model)
                
-                84     >>  336 LOAD_FAST                5 (model)
-                           338 JUMP_IF_TRUE_OR_POP     20 (to 380)
-                           340 LOAD_FAST                1 (context)
-                           342 LOAD_METHOD             11 (get)
-                           364 LOAD_CONST               4 ('wagtail_fedit_instance')
-                           366 PRECALL                  1
-                           370 CALL                     1
-                       >>  380 STORE_FAST               5 (model)
+                85         336 LOAD_FAST                4 (field_name)
+                           338 LOAD_FAST                1 (context)
+                           340 LOAD_CONST               1 ('wagtail_fedit_field_name')
+                           342 STORE_SUBSCR
+               
+                86         346 LOAD_FAST                5 (model)
+                           348 LOAD_FAST                1 (context)
+                           350 LOAD_CONST               2 ('wagtail_fedit_instance')
+                           352 STORE_SUBSCR
+               
+                90         356 LOAD_FAST                2 (block)
+                           358 POP_JUMP_FORWARD_IF_FALSE    90 (to 540)
+               
+                91         360 NOP
+               
+                92         362 LOAD_FAST                1 (context)
+                           364 LOAD_METHOD             11 (flatten)
+                           386 PRECALL                  0
+                           390 CALL                     0
+                           400 STORE_FAST               9 (block_context)
+                           402 JUMP_FORWARD            18 (to 440)
+                       >>  404 PUSH_EXC_INFO
+               
+                93         406 LOAD_GLOBAL             24 (AttributeError)
+                           418 CHECK_EXC_MATCH
+                           420 POP_JUMP_FORWARD_IF_FALSE     5 (to 432)
+                           422 POP_TOP
+               
+                94         424 LOAD_FAST                1 (context)
+                           426 STORE_FAST               9 (block_context)
+                           428 POP_EXCEPT
+                           430 JUMP_FORWARD             4 (to 440)
+               
+                93     >>  432 RERAISE                  0
+                       >>  434 COPY                     3
+                           436 POP_EXCEPT
+                           438 RERAISE                  1
+               
+                95     >>  440 LOAD_FAST                9 (block_context)
+                           442 LOAD_METHOD             13 (update)
+                           464 LOAD_FAST                6 (extra)
+                           466 PRECALL                  1
+                           470 CALL                     1
+                           480 POP_TOP
+               
+                96         482 LOAD_FAST                2 (block)
+                           484 LOAD_METHOD             14 (render_as_block)
+                           506 LOAD_FAST                9 (block_context)
+                           508 PRECALL                  1
+                           512 CALL                     1
+                           522 STORE_FAST              10 (rendered)
+               
+                97         524 LOAD_CONST               3 (True)
+                           526 LOAD_FAST                0 (self)
+                           528 STORE_ATTR              15 (has_block)
+                           538 JUMP_FORWARD            56 (to 652)
+               
+                98     >>  540 LOAD_FAST                0 (self)
+                           542 LOAD_ATTR               16 (nl)
+                           552 POP_JUMP_FORWARD_IF_FALSE    34 (to 622)
+               
+                99         554 LOAD_FAST                0 (self)
+                           556 LOAD_ATTR               16 (nl)
+                           566 LOAD_METHOD             17 (render)
+                           588 LOAD_FAST                1 (context)
+                           590 PRECALL                  1
+                           594 CALL                     1
+                           604 STORE_FAST              10 (rendered)
+               
+               100         606 LOAD_CONST               4 (False)
+                           608 LOAD_FAST                0 (self)
+                           610 STORE_ATTR              15 (has_block)
+                           620 JUMP_FORWARD            15 (to 652)
                
-                85         382 LOAD_FAST                4 (field_name)
-                           384 LOAD_FAST                1 (context)
-                           386 LOAD_CONST               1 ('wagtail_fedit_field_name')
-                           388 STORE_SUBSCR
-               
-                86         392 LOAD_FAST                5 (model)
-                           394 LOAD_FAST                1 (context)
-                           396 LOAD_CONST               4 ('wagtail_fedit_instance')
-                           398 STORE_SUBSCR
-               
-                90         402 LOAD_FAST                2 (block)
-                           404 POP_JUMP_FORWARD_IF_FALSE    90 (to 586)
-               
-                91         406 NOP
-               
-                92         408 LOAD_FAST                1 (context)
-                           410 LOAD_METHOD             12 (flatten)
-                           432 PRECALL                  0
-                           436 CALL                     0
-                           446 STORE_FAST               9 (block_context)
-                           448 JUMP_FORWARD            18 (to 486)
-                       >>  450 PUSH_EXC_INFO
-               
-                93         452 LOAD_GLOBAL             26 (AttributeError)
-                           464 CHECK_EXC_MATCH
-                           466 POP_JUMP_FORWARD_IF_FALSE     5 (to 478)
-                           468 POP_TOP
-               
-                94         470 LOAD_FAST                1 (context)
-                           472 STORE_FAST               9 (block_context)
-                           474 POP_EXCEPT
-                           476 JUMP_FORWARD             4 (to 486)
-               
-                93     >>  478 RERAISE                  0
-                       >>  480 COPY                     3
-                           482 POP_EXCEPT
-                           484 RERAISE                  1
-               
-                95     >>  486 LOAD_FAST                9 (block_context)
-                           488 LOAD_METHOD             14 (update)
-                           510 LOAD_FAST                6 (extra)
-                           512 PRECALL                  1
-                           516 CALL                     1
-                           526 POP_TOP
-               
-                96         528 LOAD_FAST                2 (block)
-                           530 LOAD_METHOD             15 (render_as_block)
-                           552 LOAD_FAST                9 (block_context)
-                           554 PRECALL                  1
-                           558 CALL                     1
-                           568 STORE_FAST              10 (rendered)
-               
-                97         570 LOAD_CONST               5 (True)
-                           572 LOAD_FAST                0 (self)
-                           574 STORE_ATTR              16 (has_block)
-                           584 JUMP_FORWARD            56 (to 698)
-               
-                98     >>  586 LOAD_FAST                0 (self)
-                           588 LOAD_ATTR               17 (nl)
-                           598 POP_JUMP_FORWARD_IF_FALSE    34 (to 668)
-               
-                99         600 LOAD_FAST                0 (self)
-                           602 LOAD_ATTR               17 (nl)
-                           612 LOAD_METHOD             18 (render)
-                           634 LOAD_FAST                1 (context)
+               102     >>  622 LOAD_GLOBAL             37 (NULL + ValueError)
+                           634 LOAD_CONST               5 ('Block or nodelist is required')
                            636 PRECALL                  1
                            640 CALL                     1
-                           650 STORE_FAST              10 (rendered)
+                           650 RAISE_VARARGS            1
+               
+               104     >>  652 LOAD_FAST                4 (field_name)
+                           654 POP_JUMP_FORWARD_IF_TRUE    37 (to 730)
+               
+               105         656 LOAD_GLOBAL             39 (NULL + warnings)
+                           668 LOAD_ATTR               20 (warn)
+               
+               106         678 LOAD_GLOBAL             42 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+               
+               107         690 LOAD_CONST               6 ('object')
+                           692 LOAD_FAST                1 (context)
+                           694 LOAD_ATTR               22 (template_name)
+                           704 BUILD_MAP                1
+               
+               106         706 BINARY_OP                6 (%)
+               
+               105         710 PRECALL                  1
+                           714 CALL                     1
+                           724 POP_TOP
+               
+               109         726 LOAD_FAST               10 (rendered)
+                           728 RETURN_VALUE
+               
+               111     >>  730 LOAD_FAST                5 (model)
+                           732 POP_JUMP_FORWARD_IF_TRUE    47 (to 828)
+               
+               112         734 LOAD_GLOBAL             39 (NULL + warnings)
+                           746 LOAD_ATTR               20 (warn)
+               
+               113         756 LOAD_GLOBAL             46 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+               
+               114         768 LOAD_CONST               6 ('object')
+                           770 LOAD_FAST                2 (block)
+                           772 LOAD_ATTR                0 (block)
+                           782 LOAD_ATTR               24 (__class__)
+                           792 LOAD_ATTR               25 (__name__)
+                           802 BUILD_MAP                1
+               
+               113         804 BINARY_OP                6 (%)
+               
+               112         808 PRECALL                  1
+                           812 CALL                     1
+                           822 POP_TOP
+               
+               116         824 LOAD_FAST               10 (rendered)
+                           826 RETURN_VALUE
+               
+               119     >>  828 LOAD_FAST                3 (block_id)
+                           830 POP_JUMP_FORWARD_IF_TRUE    13 (to 858)
+                           832 LOAD_CONST               7 ('block_id')
+                           834 LOAD_FAST                1 (context)
+                           836 CONTAINS_OP              0
+                           838 POP_JUMP_FORWARD_IF_FALSE     9 (to 858)
+               
+               120         840 LOAD_FAST                1 (context)
+                           842 LOAD_CONST               7 ('block_id')
+                           844 BINARY_SUBSCR
+                           854 STORE_FAST               3 (block_id)
+                           856 JUMP_FORWARD            27 (to 912)
+               
+               121     >>  858 LOAD_FAST                3 (block_id)
+                           860 POP_JUMP_FORWARD_IF_TRUE    25 (to 912)
+                           862 LOAD_FAST                2 (block)
+                           864 POP_JUMP_FORWARD_IF_FALSE    23 (to 912)
+                           866 LOAD_GLOBAL             53 (NULL + hasattr)
+                           878 LOAD_FAST                2 (block)
+                           880 LOAD_CONST               8 ('id')
+                           882 PRECALL                  2
+                           886 CALL                     2
+                           896 POP_JUMP_FORWARD_IF_FALSE     7 (to 912)
                
-               100         652 LOAD_CONST               6 (False)
-                           654 LOAD_FAST                0 (self)
-                           656 STORE_ATTR              16 (has_block)
-                           666 JUMP_FORWARD            15 (to 698)
-               
-               102     >>  668 LOAD_GLOBAL             21 (NULL + ValueError)
-                           680 LOAD_CONST               7 ('Block or nodelist is required')
-                           682 PRECALL                  1
-                           686 CALL                     1
-                           696 RAISE_VARARGS            1
-               
-               104     >>  698 LOAD_FAST                4 (field_name)
-                           700 POP_JUMP_FORWARD_IF_TRUE    37 (to 776)
-               
-               105         702 LOAD_GLOBAL             39 (NULL + warnings)
-                           714 LOAD_ATTR               20 (warn)
-               
-               106         724 LOAD_GLOBAL             42 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-               
-               107         736 LOAD_CONST               8 ('object')
-                           738 LOAD_FAST                1 (context)
-                           740 LOAD_ATTR               22 (template_name)
-                           750 BUILD_MAP                1
-               
-               106         752 BINARY_OP                6 (%)
-               
-               105         756 PRECALL                  1
-                           760 CALL                     1
-                           770 POP_TOP
-               
-               109         772 LOAD_FAST               10 (rendered)
-                           774 RETURN_VALUE
-               
-               111     >>  776 LOAD_FAST                5 (model)
-                           778 POP_JUMP_FORWARD_IF_TRUE    47 (to 874)
-               
-               112         780 LOAD_GLOBAL             39 (NULL + warnings)
-                           792 LOAD_ATTR               20 (warn)
-               
-               113         802 LOAD_GLOBAL             46 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-               
-               114         814 LOAD_CONST               8 ('object')
-                           816 LOAD_FAST                2 (block)
-                           818 LOAD_ATTR                0 (block)
-                           828 LOAD_ATTR               24 (__class__)
-                           838 LOAD_ATTR               25 (__name__)
-                           848 BUILD_MAP                1
-               
-               113         850 BINARY_OP                6 (%)
-               
-               112         854 PRECALL                  1
-                           858 CALL                     1
-                           868 POP_TOP
-               
-               116         870 LOAD_FAST               10 (rendered)
-                           872 RETURN_VALUE
-               
-               119     >>  874 LOAD_FAST                3 (block_id)
-                           876 POP_JUMP_FORWARD_IF_TRUE    13 (to 904)
-                           878 LOAD_CONST               2 ('block_id')
-                           880 LOAD_FAST                1 (context)
-                           882 CONTAINS_OP              0
-                           884 POP_JUMP_FORWARD_IF_FALSE     9 (to 904)
-               
-               120         886 LOAD_FAST                1 (context)
-                           888 LOAD_CONST               2 ('block_id')
-                           890 BINARY_SUBSCR
-                           900 STORE_FAST               3 (block_id)
-                           902 JUMP_FORWARD            45 (to 994)
-               
-               121     >>  904 LOAD_FAST                3 (block_id)
-                           906 POP_JUMP_FORWARD_IF_TRUE    26 (to 960)
-                           908 LOAD_FAST                2 (block)
-                           910 POP_JUMP_FORWARD_IF_FALSE    24 (to 960)
-                           912 LOAD_GLOBAL             53 (NULL + hasattr)
-                           924 LOAD_FAST                2 (block)
-                           926 LOAD_CONST               9 ('id')
-                           928 PRECALL                  2
-                           932 CALL                     2
-                           942 POP_JUMP_FORWARD_IF_FALSE     8 (to 960)
-               
-               122         944 LOAD_FAST                2 (block)
-                           946 LOAD_ATTR               27 (id)
-                           956 STORE_FAST               3 (block_id)
-                           958 JUMP_FORWARD            17 (to 994)
-               
-               123     >>  960 LOAD_FAST                3 (block_id)
-                           962 POP_JUMP_FORWARD_IF_TRUE    15 (to 994)
-               
-               124         964 LOAD_GLOBAL             21 (NULL + ValueError)
-                           976 LOAD_CONST               3 ('Block ID is required')
-                           978 PRECALL                  1
-                           982 CALL                     1
-                           992 RAISE_VARARGS            1
-               
-               126     >>  994 LOAD_FAST               10 (rendered)
-                           996 POP_JUMP_FORWARD_IF_TRUE    15 (to 1028)
-               
-               127         998 LOAD_GLOBAL             57 (NULL + mark_safe)
-                          1010 LOAD_CONST              10 ('')
-                          1012 PRECALL                  1
-                          1016 CALL                     1
-                          1026 STORE_FAST              10 (rendered)
-               
-               130     >> 1028 LOAD_FAST                1 (context)
-                          1030 LOAD_METHOD             11 (get)
-                          1052 LOAD_CONST              11 ('request')
-                          1054 PRECALL                  1
-                          1058 CALL                     1
-                          1068 STORE_FAST              11 (request)
-               
-               131        1070 LOAD_GLOBAL             59 (NULL + _can_edit)
-                          1082 LOAD_FAST               11 (request)
-                          1084 LOAD_FAST                5 (model)
-                          1086 PRECALL                  2
-                          1090 CALL                     2
-                          1100 POP_JUMP_FORWARD_IF_TRUE     2 (to 1106)
-               
-               132        1102 LOAD_FAST               10 (rendered)
-                          1104 RETURN_VALUE
-               
-               134     >> 1106 LOAD_FAST                0 (self)
-                          1108 LOAD_ATTR               16 (has_block)
-                          1118 POP_JUMP_FORWARD_IF_FALSE    10 (to 1140)
-               
-               135        1120 LOAD_FAST                0 (self)
-                          1122 LOAD_ATTR               16 (has_block)
-                          1132 LOAD_FAST                6 (extra)
-                          1134 LOAD_CONST              12 ('has_block')
-                          1136 STORE_SUBSCR
-               
-               137     >> 1140 LOAD_GLOBAL             61 (NULL + render_editable_block)
-                          1152 LOAD_CONST              14 (())
-               
-               138        1154 LOAD_FAST               11 (request)
-               
-               139        1156 LOAD_FAST               10 (rendered)
-               
-               140        1158 LOAD_FAST                3 (block_id)
-               
-               141        1160 LOAD_FAST                4 (field_name)
-               
-               142        1162 LOAD_FAST                5 (model)
-               
-               143        1164 LOAD_FAST                1 (context)
-               
-               137        1166 LOAD_CONST              13 (('request', 'content', 'block_id', 'field_name', 'model', 'context'))
-                          1168 BUILD_CONST_KEY_MAP      6
-               
-               144        1170 LOAD_FAST                6 (extra)
-               
-               137        1172 DICT_MERGE               1
-                          1174 CALL_FUNCTION_EX         1
-                          1176 RETURN_VALUE
+               122         898 LOAD_FAST                2 (block)
+                           900 LOAD_ATTR               27 (id)
+                           910 STORE_FAST               3 (block_id)
+               
+               126     >>  912 LOAD_FAST               10 (rendered)
+                           914 POP_JUMP_FORWARD_IF_TRUE    15 (to 946)
+               
+               127         916 LOAD_GLOBAL             57 (NULL + mark_safe)
+                           928 LOAD_CONST               9 ('')
+                           930 PRECALL                  1
+                           934 CALL                     1
+                           944 STORE_FAST              10 (rendered)
+               
+               130     >>  946 LOAD_FAST                1 (context)
+                           948 LOAD_METHOD             10 (get)
+                           970 LOAD_CONST              10 ('request')
+                           972 PRECALL                  1
+                           976 CALL                     1
+                           986 STORE_FAST              11 (request)
+               
+               131         988 LOAD_GLOBAL             59 (NULL + _can_edit)
+                          1000 LOAD_FAST               11 (request)
+                          1002 LOAD_FAST                5 (model)
+                          1004 PRECALL                  2
+                          1008 CALL                     2
+                          1018 POP_JUMP_FORWARD_IF_FALSE     2 (to 1024)
+                          1020 LOAD_FAST                3 (block_id)
+                          1022 POP_JUMP_FORWARD_IF_TRUE     2 (to 1028)
+               
+               132     >> 1024 LOAD_FAST               10 (rendered)
+                          1026 RETURN_VALUE
+               
+               134     >> 1028 LOAD_FAST                0 (self)
+                          1030 LOAD_ATTR               15 (has_block)
+                          1040 POP_JUMP_FORWARD_IF_FALSE    10 (to 1062)
+               
+               135        1042 LOAD_FAST                0 (self)
+                          1044 LOAD_ATTR               15 (has_block)
+                          1054 LOAD_FAST                6 (extra)
+                          1056 LOAD_CONST              11 ('has_block')
+                          1058 STORE_SUBSCR
+               
+               137     >> 1062 LOAD_GLOBAL             61 (NULL + render_editable_block)
+                          1074 LOAD_CONST              13 (())
+               
+               138        1076 LOAD_FAST               11 (request)
+               
+               139        1078 LOAD_FAST               10 (rendered)
+               
+               140        1080 LOAD_FAST                3 (block_id)
+               
+               141        1082 LOAD_FAST                4 (field_name)
+               
+               142        1084 LOAD_FAST                5 (model)
+               
+               143        1086 LOAD_FAST                1 (context)
+               
+               137        1088 LOAD_CONST              12 (('request', 'content', 'block_id', 'field_name', 'model', 'context'))
+                          1090 BUILD_CONST_KEY_MAP      6
+               
+               144        1092 LOAD_FAST                6 (extra)
+               
+               137        1094 DICT_MERGE               1
+                          1096 CALL_FUNCTION_EX         1
+                          1098 RETURN_VALUE
                ExceptionTable:
-                 408 to 446 -> 450 [0]
-                 450 to 472 -> 480 [1] lasti
-                 478 to 478 -> 480 [1] lasti
+                 362 to 400 -> 404 [0]
+                 404 to 426 -> 434 [1] lasti
+                 432 to 432 -> 434 [1] lasti
                consts
                   None
                   'wagtail_fedit_field_name'
-                  'block_id'
-                  'Block ID is required'
                   'wagtail_fedit_instance'
                   True
                   False
                   'Block or nodelist is required'
                   'object'
+                  'block_id'
                   'id'
                   ''
                   'request'
                   'has_block'
                   ('request', 'content', 'block_id', 'field_name', 'model', 'context')
                   ()
-               names      ('block', 'block_id', 'field_name', 'model', 'extra', 'items', 'isinstance', 'FilterExpression', 'resolve', '_resolve_expressions', 'ValueError', 'get', 'flatten', 'AttributeError', 'update', 'render_as_block', 'has_block', 'nl', 'render', 'warnings', 'warn', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'template_name', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__class__', '__name__', 'hasattr', 'id', 'mark_safe', '_can_edit', 'render_editable_block')
+               names      ('block', 'block_id', 'field_name', 'model', 'extra', 'items', 'isinstance', 'FilterExpression', 'resolve', '_resolve_expressions', 'get', 'flatten', 'AttributeError', 'update', 'render_as_block', 'has_block', 'nl', 'render', 'ValueError', 'warnings', 'warn', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'template_name', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__class__', '__name__', 'hasattr', 'id', 'mark_safe', '_can_edit', 'render_editable_block')
                varnames   ('self', 'context', 'block', 'block_id', 'field_name', 'model', 'extra', 'k', 'e', 'block_context', 'rendered', 'request')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
                firstlineno 60
                lnotab
-                  0x02010e010e010e010e010e0332012a0132020c01100324ff0c0310011e
-                  052e010a010a04040102012c01120108ff08022a012a0110010e01340110
-                  021e02040116010c0110ff04ff10040402040116010c0124ff04ff100404
-                  030c0112012801100104011e0204011e032a01200104020e0114020e0102
-                  01020102010201020102fa040702f9
+                  0x02010e010e010e010e010e0332012a0132020c01100324ff0c092e010a
+                  010a04040102012c01120108ff08022a012a0110010e01340110021e0204
+                  0116010c0110ff04ff10040402040116010c0124ff04ff100404030c0112
+                  0128010e0404011e032a01240104020e0114020e01020102010201020102
+                  0102fa040702f9
             'return'
             code
                argcount  : 0
                nlocals   : 4
                stacksize : 6
                flags     : 11
                code
@@ -923,15 +896,15 @@
                            144 RETURN_VALUE
                consts
                   None
                names      ('items', 'url_value_signer', 'sign', 'str')
                varnames   ('kwargs', 'packed', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'pack'
                firstlineno 147
                lnotab 0x0203040132015602
             ('request',)
             'expected'
             code
                argcount  : 1
@@ -1049,15 +1022,15 @@
                        >>  384 COPY                     3
                            386 POP_EXCEPT
                            388 RERAISE                  1
                
                174     >>  390 LOAD_GLOBAL             21 (NULL + all)
                            402 LOAD_CLOSURE             4 (unpacked)
                            404 BUILD_TUPLE              1
-                           406 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 174>)
+                           406 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 174>)
                            408 MAKE_FUNCTION            8 (closure)
                            410 LOAD_FAST                2 (expected)
                            412 GET_ITER
                            414 PRECALL                  0
                            418 CALL                     0
                            428 PRECALL                  1
                            432 CALL                     1
@@ -1109,23 +1082,23 @@
                                   54 JUMP_BACKWARD           24 (to 8)
                              >>   56 RETURN_VALUE
                      consts
                      names      ('get',)
                      varnames   ('.0', 'key')
                      freevars   ('unpacked',)
                      cellvars   ()
-                     filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+                     filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<listcomp>'
                      firstlineno 174
                      lnotab 0x
                names      ('ValueError', 'url_value_signer', 'unsign', 'GET', 'get', 'signing', 'SignatureExpired', 'UnpackError', 'BadSignature', 'TypeError', 'all')
                varnames   ('cls', 'request', 'expected', 'key')
                freevars   ()
                cellvars   ('unpacked',)
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'unpack'
                firstlineno 156
                lnotab
                   0x040204011e02040108010201220132ff1a031c0132011c013001120130
                   ff080336013002
             'instance'
             code
@@ -1196,24 +1169,24 @@
                   ('args',)
                   '?'
                   ()
                names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack')
                varnames   ('block_id', 'field_name', 'instance', 'kwargs', 'base_url', 'packed')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'get_edit_url'
                firstlineno 179
                lnotab 0x02020c0102013efe1205040104020c0120ff1003
             (None, None, None, None, None)
          names      ('__name__', '__module__', '__qualname__', 'Exception', 'UnpackError', 'NodeList', 'BoundBlock', 'str', 'models', 'Model', '__init__', 'render', 'staticmethod', 'dict', 'pack', 'classmethod', 'unpack', 'get_edit_url')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'BlockEditNode'
          firstlineno 40
          lnotab
             0x0a011c04020102010201020102fb040102ff020202fe020302fd020402
             fc02050cfb0810065702010aff0e010208020114ff0e010216020120ff0e
             01
       'BlockEditNode'
@@ -1367,15 +1340,15 @@
             'model'
             ('nodelist', 'block', 'block_id', 'field_name', 'model')
             ()
          names      ('split_contents', 'pop', 'get_kwargs', 'parse', 'delete_first_token', 'items', 'BlockEditNode', 'get')
          varnames   ('parser', 'token', 'tokens', '_', 'kwargs_names', 'kwargs', 'nodelist', 'extra', 'key', 'value')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit_block'
          firstlineno 196
          lnotab
             0x021e28012a010805220208012a012a0204020401320108010c020e0102
             0128012801280128fb040602fa
       code
          argcount  : 0
@@ -1399,19 +1372,19 @@
                       26 LOAD_CONST               3 ('getters')
                       28 LOAD_NAME                5 (list)
                       30 LOAD_NAME                6 (str)
                       32 BINARY_SUBSCR
                       42 LOAD_CONST               4 ('inline')
                       44 LOAD_NAME                7 (bool)
                       46 BUILD_TUPLE              6
-                      48 LOAD_CONST               5 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 257>)
+                      48 LOAD_CONST               5 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 257>)
                       50 MAKE_FUNCTION            5 (defaults, annotations)
                       52 STORE_NAME               8 (__init__)
          
-         264          54 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 264>)
+         264          54 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 264>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME               9 (render)
                       60 LOAD_CONST               7 (None)
                       62 RETURN_VALUE
          consts
             'FieldEditNode'
             False
@@ -1462,15 +1435,15 @@
                consts
                   None
                   1
                names      ('model', 'len', 'field', 'getters', 'inline', 'kwargs')
                varnames   ('self', 'model', 'getters', 'inline', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
                firstlineno 257
                lnotab 0x02010e013a010e010e01
             code
                argcount  : 2
                nlocals   : 12
                stacksize : 9
@@ -1706,28 +1679,28 @@
                   'inline'
                   ('request', 'content', 'field_name', 'model', 'context')
                   ()
                names      ('getters', 'model', 'inline', '_resolve_expressions', 'range', 'len', 'getattr', 'AttributeError', '__class__', '__name__', 'get', 'get_field_content', '_meta', 'get_field', 'field', 'mark_safe', '_can_edit', 'kwargs', 'items', 'isinstance', 'FilterExpression', 'resolve', 'render_editable_field')
                varnames   ('self', 'context', 'getters', 'model', 'inline', 'obj', 'i', 'getter', 'request', 'content', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
                firstlineno 264
                lnotab
                   0x02010e010e010e0320ff08030401420110010201240112013eff08032a
                   010c01020102013c0102fc100704011e030402200104023c012a013c0204
                   0114020e01020102010c01020102fb04060cfa
             None
             (False,)
          names      ('__name__', '__module__', '__qualname__', 'models', 'Model', 'list', 'str', 'bool', '__init__', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'FieldEditNode'
          firstlineno 256
          lnotab 0x0a012c07
       'FieldEditNode'
       'fedit_field'
       code
          argcount  : 2
@@ -1847,15 +1820,15 @@
             'inline'
             ('model', 'getters')
             ()
          names      ('split_contents', 'pop', 'split', 'len', 'ValueError', 'compile_filter', 'get_kwargs', 'FieldEditNode')
          varnames   ('parser', 'token', 'tokens', '_', 'model__field', 'model_tokens', 'model', 'kwargs_names', 'kwargs')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit_field'
          firstlineno 315
          lnotab
             0x020f28012a012a012a0226011e045002040202ff0404240204020e0102
             0102fe040302fd
       code
          argcount  : 5
@@ -1958,15 +1931,15 @@
                      272 PRECALL                  4
                      276 CALL                     4
                      286 POP_TOP
                      288 JUMP_BACKWARD           18 (to 254)
          
          377     >>  290 LOAD_CLOSURE             0 (request)
                      292 BUILD_TUPLE              1
-                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 377>)
+                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 377>)
                      296 MAKE_FUNCTION            8 (closure)
                      298 LOAD_FAST                8 (items)
                      300 GET_ITER
                      302 PRECALL                  0
                      306 CALL                     0
                      316 STORE_FAST               8 (items)
          
@@ -2067,15 +2040,15 @@
                             54 JUMP_BACKWARD           24 (to 8)
                        >>   56 RETURN_VALUE
                consts
                names      ('render',)
                varnames   ('.0', 'item')
                freevars   ('request',)
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '<listcomp>'
                firstlineno 377
                lnotab 0x
             'wagtail_fedit_field_name'
             'wagtail_fedit_instance'
             'inline'
             False
@@ -2084,15 +2057,15 @@
             ('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items')
             ('request',)
             ()
          names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack', 'FeditFieldEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_FIELD_TOOLBAR', 'list', 'filter', 'str', 'get', 'lower', 'render_to_string')
          varnames   ('request', 'content', 'field_name', 'model', 'context', 'kwargs', 'edit_url', 'packed', 'items', 'hook')
          freevars   ()
          cellvars   ('request',)
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_editable_field'
          firstlineno 358
          lnotab
             0x04010c0102013cfe120504010c0120ff10030e031aff0404360120021c
             013a020a010a0178010c0102020201020102010201020102fa040702f902
             0902f5
       code
@@ -2161,15 +2134,15 @@
                      148 PRECALL                  5
                      152 CALL                     5
                      162 POP_TOP
                      164 JUMP_BACKWARD           19 (to 128)
          
          411     >>  166 LOAD_CLOSURE             0 (request)
                      168 BUILD_TUPLE              1
-                     170 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 411>)
+                     170 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 411>)
                      172 MAKE_FUNCTION            8 (closure)
                      174 LOAD_FAST                8 (items)
                      176 GET_ITER
                      178 PRECALL                  0
                      182 CALL                     0
                      192 STORE_FAST               8 (items)
          
@@ -2259,26 +2232,26 @@
                             54 JUMP_BACKWARD           24 (to 8)
                        >>   56 RETURN_VALUE
                consts
                names      ('render',)
                varnames   ('.0', 'item')
                freevars   ('request',)
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '<listcomp>'
                firstlineno 411
                lnotab 0x
             'wagtail_fedit/content/editable_block.html'
             'instance'
             ('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items')
          names      ('edit_url', 'FeditBlockEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_BLOCK_TOOLBAR', 'list', 'filter', 'render_to_string', 'BlockEditNode', 'get_edit_url')
          varnames   ('request', 'content', 'block_id', 'field_name', 'model', 'context', 'kwargs', 'admin_edit_url', 'items', 'hook')
          freevars   ()
          cellvars   ('request',)
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_editable_block'
          firstlineno 397
          lnotab
             0x04010c01020102010afd12071aff0404360122021c013a020c01020216
             0104ff040202fe020302fd04050201020102010201020102010201020102
             f204fe
       'kwarg_list'
@@ -2385,22 +2358,22 @@
             'Unexpected positional argument after keyword argument'
             0
             True
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter')
          varnames   ('parser', 'kwarg_list', 'tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
          firstlineno 435
          lnotab 0x02010401040528012a01260104011e023e0210043c010602
    names      ('django.template', 'library', 'Node', 'NodeList', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'django.db', 'models', 'wagtail.blocks', 'BoundBlock', 'wagtail', 'hooks', 'urllib.parse', 'urlencode', 'warnings', 'toolbar', 'FeditBlockEditButton', 'FeditFieldEditButton', 'utils', '_can_edit', 'edit_url', 'get_field_content', '_resolve_expressions', 'CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR', 'Library', 'register', 'TimestampSigner', 'url_value_signer', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'BlockEditNode', 'tag', 'do_render_fedit_block', 'FieldEditNode', 'do_render_fedit_field', 'render_editable_field', 'render_editable_block', 'list', 'str', 'dict', 'get_kwargs')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020114010c0110010c010c010c010c010c020c010c010c02080210
       04180610061e011e03040104031c7f001d2a010eff0e01023b1c3b2a010e
       ff0e01022a06270626
```

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.4.4/wagtail_fedit/templatetags/fedit.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 
         if not field_name and "wagtail_fedit_field_name" in context:
             field_name = context["wagtail_fedit_field_name"]
 
         block, block_id, field_name, model =\
             _resolve_expressions(context, block, block_id, field_name, model)
         
-        if not block_id and "block_id" not in context and not block:
-            raise ValueError("Block ID is required")
+        # if not block_id and "block_id" not in context and not block:
+        #     raise ValueError("Block ID is required")
         
         # `wagtail_fedit_instance` is provided after the form is saved.
         # This allows us to easily use the same instance across multiple views.
         # Model will only be provided initially when the block is rendered.
         model = model or context.get("wagtail_fedit_instance")
         context["wagtail_fedit_field_name"] = field_name
         context["wagtail_fedit_instance"] = model
@@ -116,23 +116,23 @@
             return rendered
         
         # Get block id from block if bound or context.
         if not block_id and "block_id" in context:
             block_id = context["block_id"]
         elif not block_id and block and hasattr(block, "id"):
             block_id = block.id
-        elif not block_id:
-            raise ValueError("Block ID is required")
+        # elif not block_id: # Commented out; just return rendered if block_id is not available.
+        #     raise ValueError("Block ID is required")
         
         if not rendered:
             rendered = mark_safe("")
 
         # Check if the user has permission to edit the block.
         request = context.get("request")
-        if not _can_edit(request, model):
+        if not _can_edit(request, model) or not block_id:
             return rendered
 
         if self.has_block:
             extra["has_block"] = self.has_block
 
         return render_editable_block(
             request=request,
```

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from django.test import TestCase
 from django.db import models
 from django.urls import reverse
 from django.test import RequestFactory
 from django.contrib.auth.models import (
     User,
     Permission,
+    AnonymousUser,
 )
 from ..models import (
     BasicModel,
     EditableFullModel,
     EditableDraftModel,
     EditableRevisionModel,
     EditablePreviewModel,
@@ -153,14 +154,15 @@
             password="other_admin"
         )
         self.regular_user = User.objects.create_user(
             username="regular",
             email="regular@localhost",
             password="regular"
         )
+        self.anonymous_user = AnonymousUser()
         self.regular_user.user_permissions.add(Permission.objects.get(
             codename="access_admin",
             content_type__app_label="wagtailadmin"
         ))
 
         self.lock_model = EditableLockModel.objects.create(
             title="Lock Model",
```

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_block_templatetag.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_block_templatetag.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_field_templatetag.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_field_templatetag.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.4.4/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.4.4/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/urls.py` & `wagtail_fedit-1.4.4/wagtail_fedit/urls.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 ]
 
 model_based_views = (
     ("editable", views.FEditableView),
     ("publish", views.PublishView),
     ("submit", views.SubmitView),
     ("unpublish", views.UnpublishView),
+    ("cancel", views.CancelView),
 )
 
 for name, view in model_based_views:
     view.url_name = f"wagtail_fedit:{name}"
     view.url_pattern = f"{name}/<str:object_id>/<str:app_label>/<str:model_name>/"
     urlpatterns.append(
         path(view.url_pattern, view.as_view(), name=name)
```

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/utils.py` & `wagtail_fedit-1.4.4/wagtail_fedit/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,19 +31,23 @@
 FEDIT_PREVIEW_VAR = "_wagtail_fedit_preview"
 USERBAR_MODEL_VAR = "_wagtail_fedit_userbar_model"
 
 
 class FeditPermissionCheck:
     @staticmethod
     def has_perms(request: HttpRequest, model: Any) -> bool:
+
+        user = request
+        if isinstance(request, HttpRequest):
+            user = request.user
         
         if (
-            not request.user.is_authenticated\
-            or not request.user.has_perm("wagtailadmin.access_admin")\
-            or not request.user.has_perm(f"{model._meta.app_label}.change_{model._meta.model_name}")    
+            not user.is_authenticated\
+            or not user.has_perm("wagtailadmin.access_admin")\
+            or not user.has_perm(f"{model._meta.app_label}.change_{model._meta.model_name}")    
         ):
             return False
         
         return True
 
 
 class FeditIFrameMixin:
@@ -247,17 +251,18 @@
     """
     Check if a model is capable of drafts.
     """
     return isinstance(model, DraftStateMixin)\
         or type(model) == type\
         and issubclass(model, DraftStateMixin)
 
-def saving_relation(m1, m2):
+def model_diff(m1, m2):
     """
-    Check if two model instances are different.
+    Check if two model instances are different based on their type and primary key.
+    Does not check for differences in the model's fields.
     This is used to determine if a relation is being saved.
     """
     return not (
         m1._meta.app_label == m2._meta.app_label
         and m1._meta.model_name == m2._meta.model_name\
         and m1.pk == m2.pk
     )
@@ -345,24 +350,23 @@
             )
 
     return model_string
 
 def _can_edit(request, obj: models.Model):
     """
     Check if the user has appropriate permissions to edit an object.
-    Also requires the current request be on the `wagtail_fedit:editable` url.
+    Also requires the current request be on the `wagtail_fedit:editable` url
+    (Or the preview variable to be True)
     """
     if not request or not obj:
         return False
     
-    return not (
-        not request.user.is_authenticated\
-        or not request.user.has_perm("wagtailadmin.access_admin")\
-        or not request.user.has_perm(f"{obj._meta.app_label}.change_{obj._meta.model_name}")\
-        or not getattr(request, FEDIT_PREVIEW_VAR, False)
+    return (
+        FeditPermissionCheck.has_perms(request, obj)\
+        and getattr(request, FEDIT_PREVIEW_VAR, False)
     )
 
 def user_can_publish(instance, user, check_for_changes: bool = True):
     """
     Check if a user can publish an object.
     Mostly comes from PagePermissionTester.can_publish
     """
```

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.4.4/wagtail_fedit/views/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any
-from django.shortcuts import render
-from django.template.loader import render_to_string
+from django.utils import translation
 from django.utils.translation import gettext_lazy as _
 from django.utils.decorators import method_decorator
+from django.template.loader import render_to_string
 from django.views.decorators.clickjacking import xframe_options_sameorigin
 from django.views.generic import View
-from django.urls import reverse
+from django.shortcuts import render
 from django.http import (
     HttpRequest,
     HttpResponseBadRequest,
     HttpResponseForbidden,
     JsonResponse,
     HttpResponse,
 )
@@ -191,31 +191,32 @@
         
         extra_log_kwargs = {}
         if isinstance(self.instance, RevisionMixin):
             extra_log_kwargs["revision"] = self.instance.latest_revision
 
         meta_field = self.model._meta.get_field(self.field_name)
         
-        log(
-            instance=self.instance,
-            action="wagtail_fedit.edit_block",
-            user=request.user,
-            title=self.get_header_title(),
-            data={
-                "block_id": self.block_id,
-                "field_name": self.field_name,
-                "model_id": self.model_id,
-                "model_name": self.model_name,
-                "app_label": self.app_label,
-                "verbose_field_name": str(meta_field.verbose_name),
-                "block_label": str(self.block.block.label),
-            },
-            content_changed=True,
-            **extra_log_kwargs,
-        )
+        with translation.override(None):
+            log(
+                instance=self.instance,
+                action="wagtail_fedit.edit_block",
+                user=request.user,
+                title=self.get_header_title(),
+                data={
+                    "block_id": self.block_id,
+                    "field_name": self.field_name,
+                    "model_id": self.model_id,
+                    "model_name": self.model_name,
+                    "app_label": self.app_label,
+                    "verbose_field_name": str(meta_field.verbose_name),
+                    "block_label": str(self.block.block.label),
+                },
+                content_changed=True,
+                **extra_log_kwargs,
+            )
 
         # Add the data to the context and render the block.
 
         if self.has_block:
             keys = request.GET.keys()
             data = BlockEditNode.unpack(*keys, request=request)
             for key in self.edit_args:
```

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.4.4/wagtail_fedit/views/editable.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from typing import Any, Type
+from typing import Any
+from django.db import models
 from django.conf import settings
 from django.utils.translation import gettext_lazy as _
-from django.utils.decorators import method_decorator
-from django.views.decorators.clickjacking import xframe_options_sameorigin
 from django.views.generic import TemplateView
 from django.shortcuts import redirect
 from django.urls import reverse
-from django.apps import apps
-from django.core.exceptions import PermissionDenied
 from django.http import (
     HttpRequest,
     HttpResponseBadRequest,
     HttpResponseForbidden,
     HttpResponse,
 )
 from wagtail.admin import messages
+from wagtail.log_actions import (
+    registry,
+)
 from wagtail.admin.admin_url_finder import AdminURLFinder
 from wagtail.actions.publish_page_revision import PublishPageRevisionAction
 from wagtail.actions.publish_revision import PublishRevisionAction
 from wagtail.actions.unpublish_page import UnpublishPageAction
-from wagtail.actions.unpublish import UnpublishAction, UnpublishPermissionError
-from wagtail.admin.views.generic import WagtailAdminTemplateMixin
+from wagtail.actions.unpublish import UnpublishAction
 from wagtail.models import (
     RevisionMixin,
     PreviewableMixin,
     DraftStateMixin,
     WorkflowMixin,
     WorkflowState,
+    PageLogEntry,
+    ModelLogEntry,
     Page,
 )
 from .. import forms as block_forms
 from ..utils import (
     FEDIT_PREVIEW_VAR,
     USERBAR_MODEL_VAR,
     FeditPermissionCheck,
@@ -43,14 +44,17 @@
 
 from .mixins import (
     ObjectViewMixin,
     LockViewMixin,
 )
 
 
+MAX_LOG_ENTRIES_DISPLAYED = 5
+
+
 def get_unpublish_action(object):
     if isinstance(object, Page):
         return UnpublishPageAction
     return UnpublishAction
 
 
 def get_publish_action(object):
@@ -110,14 +114,15 @@
             USERBAR_MODEL_VAR: self.object,
         })
     
 
 class BaseActionView(LockViewMixin, BaseFeditView):
     template_name         = "wagtail_fedit/editor/action_confirm.html"
     required_superclasses = [DraftStateMixin]
+    action_icon            = None
     action_text            = None
     title_format           = None
     action_help_text_title = None
     action_help_text       = None
 
     def get_action(self) -> str:
         return self.action_text
@@ -130,14 +135,17 @@
     
     def get_action_help_text_title(self) -> str:
         return self.action_help_text_title
     
     def get_action_help_text(self) -> str:
         return self.action_help_text
     
+    def get_action_icon(self) -> str:
+        return self.action_icon
+    
     def setup(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
         super().setup(request, object_id, app_label, model_name)
         self.policy = self.object.permissions_for_user(request.user)
 
         if not isinstance(self.object, tuple(self.required_superclasses)):
             self.error_response = HttpResponseBadRequest(
                 "Model {} does not inherit from {}".format(
@@ -148,14 +156,15 @@
     def get_context_data(self, **kwargs: Any) -> dict[str, Any]:
         return super().get_context_data(**kwargs) | {
             "action": self.get_action_value(),  # e.g. "publishview"
             "action_text": self.get_action(),
             "action_title": self.get_action_title(),
             "action_help_text_title": self.get_action_help_text_title(),
             "action_help_text": self.get_action_help_text(),
+            "action_icon": self.get_action_icon(),
             "cancel_url": reverse(
                 "wagtail_fedit:editable",
                 args=[self.object.pk, self.model._meta.app_label, self.model._meta.model_name],
             ),
         }
 
     def redirect_to_success_url(self, request: HttpRequest) -> HttpResponse:
@@ -217,16 +226,18 @@
             messages.error(request, _("Invalid action specified: {}").format(request.POST["action"]))
             return self.get(request, *args, **kwargs)
         
         return self.action(request)
 
 
 class PublishView(BaseActionView):
+    template_name = "wagtail_fedit/editor/action_publish_confirm.html"
     required_superclasses = [DraftStateMixin, RevisionMixin]
     action_text = _("Publish")
+    action_icon = "fedit-eye-open"
 
     def get_action_title(self):
         return _("Publishing {} \"{}\"").format(self.object._meta.verbose_name, self.object)
 
     def get_action_help_text_title(self):
         return _("About publishing")
 
@@ -236,14 +247,72 @@
             _("That means that any changes you make will be immediately visible to everyone."),
         ]
 
         if self.policy.can_unpublish():
             s.append(_("You can always choose to unpublish it."))
 
         return s
+    
+    def get_context_data(self, **kwargs: Any) -> dict[str, Any]:
+        context = super().get_context_data(**kwargs)
+
+        log_entry_count = 0
+        log_entry_model = registry.get_log_model_for_model(self.object.__class__)
+        if issubclass(log_entry_model, PageLogEntry):
+            log_entries = log_entry_model.objects\
+                .filter(page=self.object)\
+                .order_by("-timestamp")
+            
+            context["view_more_url"] = reverse(
+                "wagtailadmin_pages:history",
+                args=[self.object.pk],
+            )
+                
+        elif issubclass(log_entry_model, ModelLogEntry):
+            log_entries = log_entry_model.objects\
+                .filter(object_id=self.object.pk)\
+                .order_by("-timestamp")
+                
+        else:
+            log_entries = None
+
+        if log_entries:
+            log_entries = log_entries.filter(
+                timestamp__gt=models.Subquery(
+                    log_entries.filter(action="wagtail.publish")\
+                               .values("timestamp")\
+                               .order_by("-timestamp")[:1]
+                )
+            )
+
+            log_entries = log_entries.select_related(
+                "revision", "user", "user__wagtail_userprofile",
+            )
+
+            # if not self.request.user.is_superuser or\
+            #    not self.request.user.is_staff:
+            #     log_entries = log_entries.filter(user=self.request.user)
+
+            if isinstance(self.object, Page):
+                log_entries = log_entries.select_related("page")
+            else:
+                log_entries = log_entries.select_related("content_type")
+
+            log_entry_count = log_entries.count()
+            log_entries = log_entries[:MAX_LOG_ENTRIES_DISPLAYED]
+
+        context.update({
+            "log_entries": log_entries,
+            "has_more_entries": log_entry_count > MAX_LOG_ENTRIES_DISPLAYED,
+            "log_entry_count": log_entry_count,
+            "last_published_at": self.object.last_published_at,
+            "is_page": isinstance(self.object, Page),
+        })
+
+        return context
 
     def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
         if not policy.can_publish():
             raise ValueError("User does not have permission to publish")
         
         if self.locked_for_user:
             raise ValueError("Object is locked")
@@ -270,14 +339,15 @@
             self.object = latest_revision.as_object()
 
         return self.redirect_to_success_url(request)
 
 
 class UnpublishView(BaseActionView):
     required_superclasses = [DraftStateMixin]
+    action_icon = "fedit-eye-closed"
     action_text = _("Unpublish")
     action_help_text_title = _("About unpublishing")
     action_help_text = [
         _("Unpublishing this object will make it invisible to users on the site."),
         _("That means that it will no longer be visible to anyone."),
         _("You can always choose to publish it again."),
     ]
@@ -308,14 +378,15 @@
         action.execute()
 
         return self.redirect_to_failsafe_url(request)
 
 
 class SubmitView(BaseActionView):
     required_superclasses = [DraftStateMixin, WorkflowMixin, RevisionMixin]
+    action_icon = "fedit-check-list"
     action_text = _("Submit for moderation")
     action_help_text_title = _("About submitting for moderation")
     action_help_text = [
         _("Submitting this object for moderation will make it invisible to users on the site."),
         _("That means that it will no longer be visible to anyone."),
         _("You can always choose to publish it again."),
     ]
@@ -349,21 +420,22 @@
             workflow = self.object.get_workflow()
             workflow.start(self.object, self.request.user)
 
         return self.redirect_to_success_url(request)
 
 
 class CancelView(BaseActionView):
-    template_name = "wagtail_fedit/editor/cancel_confirm.html"
     required_superclasses = [DraftStateMixin, WorkflowMixin]
-    action_text = _("Cancel")
-    action_help_text_title = _("About cancelling")
+    action_icon = "fedit-stop-sign"
+    action_text = _("Cancel Workflow")
+    action_help_text_title = _("About cancelling workflows")
     action_help_text = [
-        _("Cancelling this object will make it visible to users on the site."),
-        _("That means that any changes you make will be immediately visible to everyone."),
+        _("Cancelling the workflow for this object will remove it from the moderation process."),
+        _("That means that it will no longer be visible to anyone."),
+        _("You can always choose to submit it for moderation again."),
     ]
 
     def get_action_title(self):
         return _("Cancelling workflow for {} \"{}\"").format(self.object._meta.verbose_name, self.object)
 
     def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
         if not self.workflow_state:
```

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.4.4/wagtail_fedit/views/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any
 from django.db import models
 from django.shortcuts import render
+from django.utils import translation
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext as _
 from django.utils.decorators import method_decorator
 from django.template.loader import render_to_string
 from django.views.decorators.clickjacking import xframe_options_sameorigin
 from django.views.generic import View
 from django.http import (
@@ -25,23 +26,22 @@
 import uuid
 
 from ..templatetags.fedit import (
     BlockEditNode,
     render_editable_field,
 )
 from ..forms import (
-    blocks as block_forms,
     fields as field_forms,
 )
 from ..utils import (
     FeditPermissionCheck,
     FeditIFrameMixin,
     use_related_form,
     get_field_content,
-    saving_relation,
+    model_diff,
     is_draft_capable,
     get_model_string,
     lock_info,
 )
 
 
 
@@ -146,41 +146,41 @@
             self.template_name,
             context,
         )
     
     def get_help_text(self):
         if is_draft_capable(self.original_instance)\
                 and is_draft_capable(self.instance)\
-                and saving_relation(self.instance, self.original_instance):
+                and model_diff(self.instance, self.original_instance):
             return {
                 "status": "warning",
                 "heading": FeditIFrameMixin.HEADING_SUPPORTS_DRAFTS,
                 "title": FeditIFrameMixin.TITLE_SUPPORTS_DRAFTS,
                 "text": mark_safe(_("You must publish %(model)s and the related object of type %(related_verbose_name)s (%(related_model)s) to make any changes visible.") % {
                     "model": get_model_string(self.original_instance, publish_url=True, request=self.request),
                     "related_verbose_name": self.instance._meta.verbose_name,
                     "related_model": get_model_string(self.instance, publish_url=True, request=self.request),
                 })
             }
 
         elif is_draft_capable(self.original_instance)\
                 and not is_draft_capable(self.instance)\
-                and saving_relation(self.instance, self.original_instance):
+                and model_diff(self.instance, self.original_instance):
             return {
                 "status": "warning",
                 "heading": FeditIFrameMixin.HEADING_SUPPORTS_DRAFTS,
                 "title": FeditIFrameMixin.TITLE_SUPPORTS_DRAFTS,
                 "text": mark_safe(FeditIFrameMixin.TEXT_PUBLISH_DRAFTS % {
                     "model": get_model_string(self.original_instance, publish_url=True, request=self.request),
                 })
             }
         
         elif not is_draft_capable(self.original_instance)\
                 and is_draft_capable(self.instance)\
-                and saving_relation(self.instance, self.original_instance):
+                and model_diff(self.instance, self.original_instance):
             return {
                 "status": "warning",
                 "heading": _("Publishing related object required."),
                 "title": _("The object you are editing supports drafts."),
                 "text": mark_safe(_("You must publish the related object of type %(type)s (%(model)s) to make any changes visible.") % {
                     "type": self.original_instance._meta.verbose_name,
                     "model": get_model_string(self.original_instance, publish_url=True, request=self.request),
@@ -237,66 +237,67 @@
         
         self.instance = form.save()
         
         # add data to context
         context = self.get_context_data(form=form, **self.data)
 
         # Check if we are saving a relation
-        if saving_relation(self.instance, self.original_instance):
+        if model_diff(self.instance, self.original_instance):
             self.meta_field.save_form_data(self.original_instance, self.instance)
             field_forms.save_possible_revision(self.original_instance, request)
 
         extra_log_kwargs = {}
         if isinstance(self.original_instance, RevisionMixin):
             extra_log_kwargs["revision"] = self.original_instance.latest_revision
 
-        data = {
-            "verbose_field_name": self.meta_field.verbose_name,
-            "field_name": self.field_name,
-            "model_id": self.model_id,
-            "model_name": self.model_name,
-            "app_label": self.app_label,
-            "model_verbose": str(self.model._meta.verbose_name),
-            "model_string": str(get_model_string(self.original_instance)),
-            "old": str(self.initial_field_value),
-            "new": str(getattr(
-                self.original_instance,
-                self.field_name
-            )),
-        }
+        with translation.override(None):
+            data = {
+                "verbose_field_name": str(self.meta_field.verbose_name),
+                "field_name": self.field_name,
+                "model_id": self.model_id,
+                "model_name": self.model_name,
+                "app_label": self.app_label,
+                "model_verbose": str(self.model._meta.verbose_name),
+                "model_string": str(get_model_string(self.original_instance)),
+                "old": str(self.initial_field_value),
+                "new": str(getattr(
+                    self.original_instance,
+                    self.field_name
+                )),
+            }
+
+            uid = uuid.uuid4()
+            if self.original_instance.pk != self.instance.pk:
+                data.update({
+                    "edited_model_string": str(get_model_string(self.instance)),
+                    "edited_model_verbose": str(self.instance._meta.verbose_name),
+                    "edited_model_id": self.instance.pk,
+                    "edited_model_name": self.instance._meta.model_name,
+                    "edited_app_label": self.instance._meta.app_label,
+                })
 
-        uid = uuid.uuid4()
-        if self.original_instance.pk != self.instance.pk:
-            data.update({
-                "edited_model_string": str(get_model_string(self.instance)),
-                "edited_model_verbose": str(self.instance._meta.verbose_name),
-                "edited_model_id": self.instance.pk,
-                "edited_model_name": self.instance._meta.model_name,
-                "edited_app_label": self.instance._meta.app_label,
-            })
+                log(
+                    instance=self.instance,
+                    action="wagtail_fedit.related_changed",
+                    user=request.user,
+                    uuid=uid,
+                    data=data,
+                    content_changed=True,
+                )
 
             log(
-                instance=self.instance,
-                action="wagtail_fedit.related_changed",
+                instance=self.original_instance,
+                action="wagtail_fedit.edit_field",
                 user=request.user,
+                title=self.get_header_title(),
                 uuid=uid,
                 data=data,
                 content_changed=True,
+                **extra_log_kwargs,
             )
-        
-        log(
-            instance=self.original_instance,
-            action="wagtail_fedit.edit_field",
-            user=request.user,
-            title=self.get_header_title(),
-            uuid=uid,
-            data=data,
-            content_changed=True,
-            **extra_log_kwargs,
-        )
 
         content = get_field_content(
             request,
             self.original_instance,
             self.meta_field,
             context
         )
```

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.4.4/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.4.4/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.4.4/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from django.utils.translation import gettext_lazy as _
+from django.utils.translation import (
+    gettext_lazy as _,
+    gettext,
+)
 from wagtail.log_actions import LogFormatter
 from wagtail import hooks
 
 @hooks.register("register_log_actions")
 def register_core_log_actions(actions):
     actions.register_action("wagtail_fedit.related_changed", _("Edit Related"), _("Related Object Edited"))
 
@@ -16,16 +19,16 @@
 
             if not "verbose_field_name" in data:
                 return self.label
 
             if "edited_model_string" in data\
                 and "edited_model_verbose" in data:
                 return _("Changed related '%(related)s' instance '%(instance)s' on field '%(field)s' (Frontend)") % {
-                    "field": data["verbose_field_name"],
-                    "related": data["edited_model_verbose"],
+                    "field": gettext(data["verbose_field_name"]),
+                    "related": gettext(data["edited_model_verbose"]),
                     "instance": data["edited_model_string"],
                 }
 
             try:
 
                 old = data["old"]
                 new = data["new"]
@@ -33,15 +36,15 @@
                 if len(old) > 50:
                     old = old[:50] + "..."
 
                 if len(new) > 50:
                     new = new[:50] + "..."
 
                 return _("Changed '%(field)s' from '%(old)s' to '%(new)s' (Frontend)") % {
-                    "field": data["verbose_field_name"],
+                    "field": gettext(data["verbose_field_name"]),
                     "old": old,
                     "new": new,
                 }
             
             except KeyError:
                 return _("Edit Field")
 
@@ -59,11 +62,11 @@
         def format_message(self, log_entry):
             data = log_entry.data
 
             if not all([key in data for key in self.must]):
                 return self.label
 
             return _("Changed block \"%(block)s\" on field \"%(field)s\" (%(block_id)s, Frontend)") % {
-                "field": data["verbose_field_name"],
-                "block": data["block_label"],
+                "block": gettext(data["block_label"]),
+                "field": gettext(data["verbose_field_name"]),
                 "block_id": data["block_id"],
             }
```

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.4.4/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.urls import reverse
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.templatetags.static import static
+from django.utils.translation import gettext_lazy as _
 from wagtail.admin.userbar import (
     BaseItem,
     AddPageItem,
     ExplorePageItem,
     EditPageItem,
 )
 from wagtail import hooks
@@ -19,58 +20,76 @@
     is_draft_capable,
     user_can_publish,
     user_can_unpublish,
     user_can_submit_for_moderation,
 )
 
 class FeditableModelComponent(FeditToolbarComponent):
+    template_name = "wagtail_fedit/userbar/publish/action_button.html"
+    action_icon = None
+    action_text = None
+
     def __init__(self, instance):
         self.instance = instance
 
     def get_context_data(self, request):
         return super().get_context_data(request) | {
             "hidden": not self.instance.has_unpublished_changes,
+            "action_icon": self.action_icon,
+            "action_text": self.action_text,
             "action_url": reverse(
                 self.action_url,
                 args=[self.instance.pk, self.instance._meta.app_label, self.instance._meta.model_name],
             ),
         }
 
 class UserBarActionPublishComponent(FeditableModelComponent):
-    template_name = "wagtail_fedit/userbar/publish/buttons/publish.html"
     action_url = "wagtail_fedit:publish"
-    check_for_changes = False
+    action_icon = "fedit-eye-open"
+    action_text = _("Publish")
     
     def is_shown(self, request):
         if not super().is_shown(request):
             return False
         
-        return user_can_publish(self.instance, request.user, check_for_changes=self.check_for_changes)
+        return user_can_publish(self.instance, request.user, check_for_changes=False)
 
 class UserBarActionUnpublishComponent(FeditableModelComponent):
-    template_name = "wagtail_fedit/userbar/publish/buttons/unpublish.html"
     action_url = "wagtail_fedit:unpublish"
+    action_icon = "fedit-eye-closed"
+    action_text = _("Unpublish")
         
     def is_shown(self, request):
         if not super().is_shown(request):
             return False
         
         return user_can_unpublish(self.instance, request.user)
 
 class UserBarActionSubmitComponent(FeditableModelComponent):
-    template_name = "wagtail_fedit/userbar/publish/buttons/submit.html"
     action_url = "wagtail_fedit:submit"
-    check_for_changes = False
+    action_icon = "fedit-check-list"
+    action_text = _("Submit for moderation")
 
     def is_shown(self, request):
         if not super().is_shown(request):
             return False
         
-        return user_can_submit_for_moderation(self.instance, request.user, check_for_changes=self.check_for_changes)
+        return user_can_submit_for_moderation(self.instance, request.user, check_for_changes=False)
+
+class UserBarActionCancelComponent(FeditableModelComponent):
+    action_url = "wagtail_fedit:cancel"
+    action_icon = "fedit-stop-sign"
+    action_text = _("Cancel Workflow")
 
+    def is_shown(self, request):
+        if not super().is_shown(request):
+            return False
+        
+        return is_draft_capable(self.instance) and\
+               self.instance.has_unpublished_changes
 
 class BaseWagtailFeditItem(BaseItem, FeditPermissionCheck):
     def __init__(self, model):
         self.model = model
 
     def get_context_data(self, request):
         context = super().get_context_data(request)
@@ -128,14 +147,15 @@
 
     def get_context_data(self, request):
 
         buttons = [
             UserBarActionPublishComponent(self.model),
             UserBarActionSubmitComponent(self.model),
             UserBarActionUnpublishComponent(self.model),
+            UserBarActionCancelComponent(self.model),
         ]
 
         return super().get_context_data(request) | {
             "buttons": list(
                 filter(None, map(lambda x: x.render(request), buttons))
             ),
         }
```

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.4.4/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.4.3
-Summary: An application made for the Django Web Framework.
+Version: 1.4.4
+Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
-License: GPL-3.0-only
+License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 5
+Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 wagtail_fedit
```

#### html2text {}

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.3 Summary: An
-application made for the Django Web Framework. Home-page: https://github.com/
-Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
-License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
-Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: GNU General
-Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP Classifier:
-Topic :: Internet :: WWW/HTTP :: Dynamic Content Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE wagtail_fedit
-============= ![Wagtail FEdit Example](https://github.com/Nigel2392/
-wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
-Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be
-edited on the frontend. # Table of Contents - [Getting Started](#getting-
-started) - [Getting Editing!](#getting-editing) - [Permissions](#permissions) -
-[Revisions](#revisions) - [Workflows](#workflows) - [Logs](#logs) - [Caveats]
-(#caveats) - [Hooks](#hooks) - [Construct Block Toolbar]
-(#wagtail_feditconstruct_block_toolbar) - [Construct Field Toolbar]
-(#wagtail_feditconstruct_field_toolbar) - [Register Type Renderer]
-(#wagtail_feditregister_type_renderer) - [Register Field Renderer]
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.4 Summary: Frontend
+editing for your Wagtail site Home-page: https://github.com/Nigel2392/
+wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
+only Classifier: Environment :: Web Environment Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
+Dynamic Content Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE wagtail_fedit ============= ![Wagtail FEdit Example]
+(https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/
+wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
+Wagtail pages and content-blocks to be edited on the frontend. # Table of
+Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
+editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
+(#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Hooks](#hooks) -
+[Construct Block Toolbar](#wagtail_feditconstruct_block_toolbar) - [Construct
+Field Toolbar](#wagtail_feditconstruct_field_toolbar) - [Register Type
+Renderer](#wagtail_feditregister_type_renderer) - [Register Field Renderer]
 (#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [How your field/block is rendered]
 (#how-your-fieldblock-is-rendered) - [Rendered block output HTML](#rendered-
 block-output-html) - [Rendered field output HTML](#rendered-field-output-html)
 - [Implemented](#implemented) Getting Started --------------- 1. Add
 'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
```

### Comparing `wagtail_fedit-1.4.3/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.4.4/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 wagtail_fedit/__init__.py
-wagtail_fedit/admin.py
 wagtail_fedit/apps.py
 wagtail_fedit/hooks.py
 wagtail_fedit/models.py
 wagtail_fedit/toolbar.py
 wagtail_fedit/urls.py
 wagtail_fedit/utils.py
 wagtail_fedit.egg-info/PKG-INFO
 wagtail_fedit.egg-info/SOURCES.txt
 wagtail_fedit.egg-info/dependency_links.txt
 wagtail_fedit.egg-info/requires.txt
 wagtail_fedit.egg-info/top_level.txt
 wagtail_fedit/forms/__init__.py
 wagtail_fedit/forms/blocks.py
 wagtail_fedit/forms/fields.py
+wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+wagtail_fedit/locale/nl/LC_MESSAGES/django.po
 wagtail_fedit/migrations/__init__.py
 wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/static/wagtail_fedit/css/frontend.css
 wagtail_fedit/static/wagtail_fedit/css/furniture.css
 wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
 wagtail_fedit/static/wagtail_fedit/js/frontend.js
 wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/field.html
 wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
 wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
-wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
-wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
 wagtail_fedit/templatetags/__init__.py
 wagtail_fedit/templatetags/fedit.py
 wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
 wagtail_fedit/test/__init__.py
 wagtail_fedit/test/manage.py
 wagtail_fedit/test/core/__init__.py
@@ -58,14 +63,15 @@
 wagtail_fedit/test/core/tests/__init__.py
 wagtail_fedit/test/core/tests/base.py
 wagtail_fedit/test/core/tests/test_block_edit.py
 wagtail_fedit/test/core/tests/test_block_templatetag.py
 wagtail_fedit/test/core/tests/test_blocks.py
 wagtail_fedit/test/core/tests/test_field_edit.py
 wagtail_fedit/test/core/tests/test_field_templatetag.py
+wagtail_fedit/test/core/tests/test_generic.py
 wagtail_fedit/test/core/tests/test_revision.py
 wagtail_fedit/test/core/tests/test_submit.py
 wagtail_fedit/test/testapp/__init__.py
 wagtail_fedit/test/testapp/asgi.py
 wagtail_fedit/test/testapp/settings.py
 wagtail_fedit/test/testapp/urls.py
 wagtail_fedit/test/testapp/wsgi.py
@@ -73,11 +79,12 @@
 wagtail_fedit/views/blocks.py
 wagtail_fedit/views/editable.py
 wagtail_fedit/views/fields.py
 wagtail_fedit/views/mixins.py
 wagtail_fedit/wagtail_hooks/__init__.py
 wagtail_fedit/wagtail_hooks/action_menu.py
 wagtail_fedit/wagtail_hooks/excluded_relations.py
+wagtail_fedit/wagtail_hooks/icons.py
 wagtail_fedit/wagtail_hooks/log_actions.py
 wagtail_fedit/wagtail_hooks/renderers.py
 wagtail_fedit/wagtail_hooks/urls.py
 wagtail_fedit/wagtail_hooks/userbar.py
```

