# Comparing `tmp/wagtail_fedit-1.4.5.tar.gz` & `tmp/wagtail_fedit-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.4.5.tar", last modified: Thu Apr 11 10:30:14 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.4.6.tar", last modified: Thu Apr 11 11:04:47 2024, max compression
```

## Comparing `wagtail_fedit-1.4.5.tar` & `wagtail_fedit-1.4.6.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.753346 wagtail_fedit-1.4.5/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.5/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0    13209 2024-04-11 10:30:14.752344 wagtail_fedit-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0    11954 2024-04-08 20:13:14.000000 wagtail_fedit-1.4.5/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.5/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2024-04-11 10:30:14.759349 wagtail_fedit-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.511720 wagtail_fedit-1.4.5/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.5/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.5/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.540714 wagtail_fedit-1.4.5/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.5/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.4.5/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.5/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     3358 2024-04-10 10:24:35.000000 wagtail_fedit-1.4.5/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.448303 wagtail_fedit-1.4.5/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.448303 wagtail_fedit-1.4.5/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.562191 wagtail_fedit-1.4.5/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.4.5/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.4.5/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.564192 wagtail_fedit-1.4.5/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.5/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.565190 wagtail_fedit-1.4.5/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.5/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.5/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.449303 wagtail_fedit-1.4.5/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.449303 wagtail_fedit-1.4.5/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.586522 wagtail_fedit-1.4.5/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.5/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.5/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.5/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.606753 wagtail_fedit-1.4.5/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    15915 2024-04-06 00:14:04.000000 wagtail_fedit-1.4.5/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.450437 wagtail_fedit-1.4.5/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.451449 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.609810 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.613505 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      302 2024-04-06 22:07:59.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      335 2024-04-06 22:08:01.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.630141 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      789 2024-04-07 05:29:57.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.636593 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.652842 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.668841 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.677843 wagtail_fedit-1.4.5/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.5/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.680843 wagtail_fedit-1.4.5/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.5/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    17687 2024-04-10 19:17:23.000000 wagtail_fedit-1.4.5/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    14619 2024-04-10 19:17:21.000000 wagtail_fedit-1.4.5/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.682844 wagtail_fedit-1.4.5/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.688842 wagtail_fedit-1.4.5/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.697931 wagtail_fedit-1.4.5/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.706217 wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7106 2024-04-10 12:43:12.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     2996 2024-04-10 10:50:37.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_block_templatetag.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3994 2024-04-10 11:08:06.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_field_templatetag.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     5805 2024-04-11 10:01:14.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.719470 wagtail_fedit-1.4.5/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.5/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.4.5/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      951 2024-04-11 08:07:43.000000 wagtail_fedit-1.4.5/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    15352 2024-04-10 13:08:18.000000 wagtail_fedit-1.4.5/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.741475 wagtail_fedit-1.4.5/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.4.5/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9321 2024-04-11 07:42:21.000000 wagtail_fedit-1.4.5/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.4.5/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    12413 2024-04-11 07:51:29.000000 wagtail_fedit-1.4.5/wagtail_fedit/views/fields.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.5/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.750234 wagtail_fedit-1.4.5/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      182 2024-04-11 08:26:05.000000 wagtail_fedit-1.4.5/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.5/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.5/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.4.5/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.4.5/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.5/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.5/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     6693 2024-04-11 09:04:42.000000 wagtail_fedit-1.4.5/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:30:14.752344 wagtail_fedit-1.4.5/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    13209 2024-04-11 10:30:14.000000 wagtail_fedit-1.4.5/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3976 2024-04-11 10:30:14.000000 wagtail_fedit-1.4.5/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 10:30:14.000000 wagtail_fedit-1.4.5/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-11 10:30:14.000000 wagtail_fedit-1.4.5/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-11 10:30:14.000000 wagtail_fedit-1.4.5/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.372470 wagtail_fedit-1.4.6/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    13152 2024-04-11 11:04:47.373471 wagtail_fedit-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11954 2024-04-08 20:13:14.000000 wagtail_fedit-1.4.6/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2024-04-11 11:04:47.382724 wagtail_fedit-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.987100 wagtail_fedit-1.4.6/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.6/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.6/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.036675 wagtail_fedit-1.4.6/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.6/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.4.6/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.6/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     3358 2024-04-10 10:24:35.000000 wagtail_fedit-1.4.6/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.936096 wagtail_fedit-1.4.6/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.936096 wagtail_fedit-1.4.6/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.060165 wagtail_fedit-1.4.6/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.4.6/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.4.6/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.061303 wagtail_fedit-1.4.6/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.6/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.063316 wagtail_fedit-1.4.6/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.6/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.6/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.938096 wagtail_fedit-1.4.6/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.938096 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.072314 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.096592 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    15915 2024-04-06 00:14:04.000000 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.940097 wagtail_fedit-1.4.6/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.941100 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.098590 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.100591 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      302 2024-04-06 22:07:59.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      335 2024-04-06 22:08:01.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.109359 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      789 2024-04-07 05:29:57.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.116296 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.121759 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.126389 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.144202 wagtail_fedit-1.4.6/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.6/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.148470 wagtail_fedit-1.4.6/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.6/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    17687 2024-04-10 19:17:23.000000 wagtail_fedit-1.4.6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14619 2024-04-10 19:17:21.000000 wagtail_fedit-1.4.6/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.151871 wagtail_fedit-1.4.6/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.186778 wagtail_fedit-1.4.6/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.199780 wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.262390 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7106 2024-04-10 12:43:12.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     2996 2024-04-10 10:50:37.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_block_templatetag.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3994 2024-04-10 11:08:06.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_field_templatetag.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.287401 wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.4.6/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      951 2024-04-11 08:07:43.000000 wagtail_fedit-1.4.6/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    15352 2024-04-10 13:08:18.000000 wagtail_fedit-1.4.6/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.340531 wagtail_fedit-1.4.6/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.4.6/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9321 2024-04-11 07:42:21.000000 wagtail_fedit-1.4.6/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.4.6/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    12413 2024-04-11 07:51:29.000000 wagtail_fedit-1.4.6/wagtail_fedit/views/fields.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.6/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.371464 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      182 2024-04-11 08:26:05.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7068 2024-04-11 11:04:16.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.014620 wagtail_fedit-1.4.6/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    13152 2024-04-11 11:04:46.000000 wagtail_fedit-1.4.6/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3976 2024-04-11 11:04:46.000000 wagtail_fedit-1.4.6/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 11:04:46.000000 wagtail_fedit-1.4.6/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-11 11:04:46.000000 wagtail_fedit-1.4.6/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-11 11:04:46.000000 wagtail_fedit-1.4.6/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.4.5/LICENSE` & `wagtail_fedit-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/PKG-INFO` & `wagtail_fedit-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.4.5
+Version: 1.4.6
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -23,16 +23,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=4.2
-Requires-Dist: Wagtail>=5.2
 
 wagtail_fedit
 =============
 
 ![Wagtail FEdit Example](https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
 
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.5 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.6 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
 Dynamic Content Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: Django>=4.2 Requires-Dist: Wagtail>=5.2
-wagtail_fedit ============= ![Wagtail FEdit Example](https://github.com/
-Nigel2392/wagtail_fedit/blob/main/.github/images/
+License-File: LICENSE wagtail_fedit ============= ![Wagtail FEdit Example]
+(https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/
 wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
 Wagtail pages and content-blocks to be edited on the frontend. # Table of
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
 (#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Hooks](#hooks) -
 [Construct Block Toolbar](#wagtail_feditconstruct_block_toolbar) - [Construct
 Field Toolbar](#wagtail_feditconstruct_field_toolbar) - [Register Type
```

### Comparing `wagtail_fedit-1.4.5/README.md` & `wagtail_fedit-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/setup.cfg` & `wagtail_fedit-1.4.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 342e  ..version = 1.4.
-00000030: 350d 0a64 6573 6372 6970 7469 6f6e 203d  5..description =
+00000030: 360d 0a64 6573 6372 6970 7469 6f6e 203d  6..description =
 00000040: 2046 726f 6e74 656e 6420 6564 6974 696e   Frontend editin
 00000050: 6720 666f 7220 796f 7572 2057 6167 7461  g for your Wagta
 00000060: 696c 2073 6974 650d 0a6c 6f6e 675f 6465  il site..long_de
 00000070: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000080: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
 00000090: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
 000000a0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
```

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.4.6/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.4.6/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/hooks.py` & `wagtail_fedit-1.4.6/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.4.6/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.4.6/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/models.py` & `wagtail_fedit-1.4.6/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.4.6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.4.6/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_block_templatetag.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_block_templatetag.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_field_templatetag.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_field_templatetag.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         self.assertEqual(wf, workflow)
         self.assertFalse(not not self.full_model.workflow_states.all())
 
         self.makeRequest("submit", self.full_model, SubmitView, 302)
 
         self.full_model = self.full_model.__class__.objects.get(pk=self.full_model.pk)
         workflow: Workflow = self.full_model.get_workflow()
-        current_state = self.full_model.workflow_states.first()
+        current_state = self.full_model.current_workflow_state
 
         self.assertEqual(
             current_state.status,
             current_state.STATUS_IN_PROGRESS,
         )
 
     def test_cancel(self):
@@ -170,13 +170,13 @@
         self.lock_model.locked = True
         self.lock_model.locked_by = self.other_admin_user
         self.lock_model.save(update_fields=["locked", "locked_by"])
         
         self.makeRequest("cancel", self.lock_model, CancelView, 200)
 
         self.lock_model.refresh_from_db()
-        current_state = self.full_model.workflow_states.first()
+        current_state = self.full_model.current_workflow_state
 
         self.assertEqual(
             current_state.status,
             current_state.STATUS_IN_PROGRESS,
         )
```

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.4.6/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/urls.py` & `wagtail_fedit-1.4.6/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/utils.py` & `wagtail_fedit-1.4.6/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.4.6/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.4.6/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.4.6/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.4.6/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.urls import reverse
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.templatetags.static import static
 from django.utils.translation import gettext_lazy as _
+from wagtail.models import WorkflowMixin
 from wagtail.admin.userbar import (
     BaseItem,
     AddPageItem,
     ExplorePageItem,
     EditPageItem,
 )
 from wagtail import hooks
@@ -80,16 +81,25 @@
     action_icon = "fedit-stop-sign"
     action_text = _("Cancel Workflow")
 
     def is_shown(self, request):
         if not super().is_shown(request):
             return False
         
-        return is_draft_capable(self.instance) and\
-               self.instance.has_unpublished_changes
+        if not is_draft_capable(self.instance):
+            return False
+        
+        if not isinstance(self.instance, WorkflowMixin):
+            return False
+        
+        workflow_state = self.instance.current_workflow_state
+        return workflow_state and (
+            workflow_state.status == workflow_state.STATUS_IN_PROGRESS or\
+            workflow_state.status == workflow_state.STATUS_NEEDS_CHANGES
+        )
 
 class BaseWagtailFeditItem(BaseItem, FeditPermissionCheck):
     def __init__(self, model):
         self.model = model
 
     def get_context_data(self, request):
         context = super().get_context_data(request)
```

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.4.6/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail_fedit
-Version: 1.4.5
+Name: wagtail-fedit
+Version: 1.4.6
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -23,16 +23,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=4.2
-Requires-Dist: Wagtail>=5.2
 
 wagtail_fedit
 =============
 
 ![Wagtail FEdit Example](https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
 
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.5 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.6 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
 Dynamic Content Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: Django>=4.2 Requires-Dist: Wagtail>=5.2
-wagtail_fedit ============= ![Wagtail FEdit Example](https://github.com/
-Nigel2392/wagtail_fedit/blob/main/.github/images/
+License-File: LICENSE wagtail_fedit ============= ![Wagtail FEdit Example]
+(https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/
 wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
 Wagtail pages and content-blocks to be edited on the frontend. # Table of
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
 (#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Hooks](#hooks) -
 [Construct Block Toolbar](#wagtail_feditconstruct_block_toolbar) - [Construct
 Field Toolbar](#wagtail_feditconstruct_field_toolbar) - [Register Type
```

### Comparing `wagtail_fedit-1.4.5/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.4.6/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

