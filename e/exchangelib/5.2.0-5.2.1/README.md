# Comparing `tmp/exchangelib-5.2.0.tar.gz` & `tmp/exchangelib-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchangelib-5.2.0.tar", last modified: Fri Mar  8 09:53:57 2024, max compression
+gzip compressed data, was "exchangelib-5.2.1.tar", last modified: Thu Apr 11 17:15:04 2024, max compression
```

## Comparing `exchangelib-5.2.0.tar` & `exchangelib-5.2.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-03-08 09:53:57.109709 exchangelib-5.2.0/
--rw-r--r--   0 erik       (501) staff       (20)    38569 2024-03-08 09:52:57.000000 exchangelib-5.2.0/CHANGELOG.md
--rw-r--r--   0 erik       (501) staff       (20)     1313 2022-01-03 12:16:38.000000 exchangelib-5.2.0/LICENSE
--rw-r--r--   0 erik       (501) staff       (20)       91 2024-03-03 15:20:26.000000 exchangelib-5.2.0/MANIFEST.in
--rw-r--r--   0 erik       (501) staff       (20)     3597 2024-03-08 09:53:57.109457 exchangelib-5.2.0/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     1978 2023-11-15 18:16:03.000000 exchangelib-5.2.0/README.md
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-03-08 09:53:57.098444 exchangelib-5.2.0/exchangelib/
--rw-r--r--   0 erik       (501) staff       (20)     2819 2024-03-08 09:52:57.000000 exchangelib-5.2.0/exchangelib/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)    36379 2024-03-07 10:58:52.000000 exchangelib-5.2.0/exchangelib/account.py
--rw-r--r--   0 erik       (501) staff       (20)     9526 2022-11-24 11:30:07.000000 exchangelib-5.2.0/exchangelib/attachments.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-03-08 09:53:57.099603 exchangelib-5.2.0/exchangelib/autodiscover/
--rw-r--r--   0 erik       (501) staff       (20)      499 2022-11-23 00:50:30.000000 exchangelib-5.2.0/exchangelib/autodiscover/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     5986 2022-11-17 13:10:32.000000 exchangelib-5.2.0/exchangelib/autodiscover/cache.py
--rw-r--r--   0 erik       (501) staff       (20)    22636 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/autodiscover/discovery.py
--rw-r--r--   0 erik       (501) staff       (20)     2164 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/autodiscover/protocol.py
--rw-r--r--   0 erik       (501) staff       (20)     4193 2022-10-10 07:45:39.000000 exchangelib-5.2.0/exchangelib/configuration.py
--rw-r--r--   0 erik       (501) staff       (20)    12159 2024-03-03 21:14:09.000000 exchangelib-5.2.0/exchangelib/credentials.py
--rw-r--r--   0 erik       (501) staff       (20)    31304 2024-03-03 21:14:09.000000 exchangelib-5.2.0/exchangelib/errors.py
--rw-r--r--   0 erik       (501) staff       (20)    11527 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/ewsdatetime.py
--rw-r--r--   0 erik       (501) staff       (20)    12821 2022-11-24 11:54:53.000000 exchangelib-5.2.0/exchangelib/extended_properties.py
--rw-r--r--   0 erik       (501) staff       (20)    63451 2024-03-03 21:14:09.000000 exchangelib-5.2.0/exchangelib/fields.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-03-08 09:53:57.100435 exchangelib-5.2.0/exchangelib/folders/
--rw-r--r--   0 erik       (501) staff       (20)     4272 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/folders/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)    39491 2024-03-03 21:14:02.000000 exchangelib-5.2.0/exchangelib/folders/base.py
--rw-r--r--   0 erik       (501) staff       (20)    23778 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/folders/collections.py
--rw-r--r--   0 erik       (501) staff       (20)    18106 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/folders/known_folders.py
--rw-r--r--   0 erik       (501) staff       (20)     6876 2023-07-23 10:17:42.000000 exchangelib-5.2.0/exchangelib/folders/queryset.py
--rw-r--r--   0 erik       (501) staff       (20)    16319 2024-03-03 21:14:02.000000 exchangelib-5.2.0/exchangelib/folders/roots.py
--rw-r--r--   0 erik       (501) staff       (20)     2934 2022-08-22 13:30:33.000000 exchangelib-5.2.0/exchangelib/indexed_properties.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-03-08 09:53:57.101803 exchangelib-5.2.0/exchangelib/items/
--rw-r--r--   0 erik       (501) staff       (20)     3381 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/items/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     9898 2022-08-22 13:30:33.000000 exchangelib-5.2.0/exchangelib/items/base.py
--rw-r--r--   0 erik       (501) staff       (20)    20811 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/items/calendar_item.py
--rw-r--r--   0 erik       (501) staff       (20)    15113 2023-05-04 21:52:26.000000 exchangelib-5.2.0/exchangelib/items/contact.py
--rw-r--r--   0 erik       (501) staff       (20)    17951 2023-08-21 05:19:29.000000 exchangelib-5.2.0/exchangelib/items/item.py
--rw-r--r--   0 erik       (501) staff       (20)     9050 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/items/message.py
--rw-r--r--   0 erik       (501) staff       (20)     1405 2022-08-22 13:30:33.000000 exchangelib-5.2.0/exchangelib/items/post.py
--rw-r--r--   0 erik       (501) staff       (20)     5876 2023-05-04 21:52:26.000000 exchangelib-5.2.0/exchangelib/items/task.py
--rw-r--r--   0 erik       (501) staff       (20)    89598 2024-03-03 21:14:09.000000 exchangelib-5.2.0/exchangelib/properties.py
--rw-r--r--   0 erik       (501) staff       (20)    35041 2024-03-07 10:53:09.000000 exchangelib-5.2.0/exchangelib/protocol.py
--rw-r--r--   0 erik       (501) staff       (20)    29612 2023-05-04 21:52:50.000000 exchangelib-5.2.0/exchangelib/queryset.py
--rw-r--r--   0 erik       (501) staff       (20)    13139 2022-10-07 08:02:07.000000 exchangelib-5.2.0/exchangelib/recurrence.py
--rw-r--r--   0 erik       (501) staff       (20)    25489 2022-10-07 08:04:06.000000 exchangelib-5.2.0/exchangelib/restriction.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-03-08 09:53:57.108696 exchangelib-5.2.0/exchangelib/services/
--rw-r--r--   0 erik       (501) staff       (20)     3775 2024-03-03 21:14:09.000000 exchangelib-5.2.0/exchangelib/services/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     1247 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/archive_item.py
--rw-r--r--   0 erik       (501) staff       (20)    46665 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/services/common.py
--rw-r--r--   0 erik       (501) staff       (20)     2097 2022-11-07 14:52:15.000000 exchangelib-5.2.0/exchangelib/services/convert_id.py
--rw-r--r--   0 erik       (501) staff       (20)      209 2022-08-22 13:30:33.000000 exchangelib-5.2.0/exchangelib/services/copy_item.py
--rw-r--r--   0 erik       (501) staff       (20)     1532 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/create_attachment.py
--rw-r--r--   0 erik       (501) staff       (20)     1988 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/services/create_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     4272 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/create_item.py
--rw-r--r--   0 erik       (501) staff       (20)      686 2022-08-22 13:30:33.000000 exchangelib-5.2.0/exchangelib/services/create_user_configuration.py
--rw-r--r--   0 erik       (501) staff       (20)      969 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/delete_attachment.py
--rw-r--r--   0 erik       (501) staff       (20)      931 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/delete_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     2504 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/delete_item.py
--rw-r--r--   0 erik       (501) staff       (20)      710 2022-08-22 13:30:33.000000 exchangelib-5.2.0/exchangelib/services/delete_user_configuration.py
--rw-r--r--   0 erik       (501) staff       (20)     1088 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/empty_folder.py
--rw-r--r--   0 erik       (501) staff       (20)      889 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/expand_dl.py
--rw-r--r--   0 erik       (501) staff       (20)     1060 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/export_items.py
--rw-r--r--   0 erik       (501) staff       (20)     3621 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/services/find_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     4326 2022-11-11 08:05:01.000000 exchangelib-5.2.0/exchangelib/services/find_item.py
--rw-r--r--   0 erik       (501) staff       (20)     4768 2022-11-11 08:05:01.000000 exchangelib-5.2.0/exchangelib/services/find_people.py
--rw-r--r--   0 erik       (501) staff       (20)     5392 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/get_attachment.py
--rw-r--r--   0 erik       (501) staff       (20)     1914 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/get_delegate.py
--rw-r--r--   0 erik       (501) staff       (20)     1186 2022-08-22 13:30:34.000000 exchangelib-5.2.0/exchangelib/services/get_events.py
--rw-r--r--   0 erik       (501) staff       (20)     2503 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/get_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     1627 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/get_item.py
--rw-r--r--   0 erik       (501) staff       (20)     1576 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/get_mail_tips.py
--rw-r--r--   0 erik       (501) staff       (20)     1127 2022-08-22 13:30:34.000000 exchangelib-5.2.0/exchangelib/services/get_persona.py
--rw-r--r--   0 erik       (501) staff       (20)      696 2022-08-22 13:30:34.000000 exchangelib-5.2.0/exchangelib/services/get_room_lists.py
--rw-r--r--   0 erik       (501) staff       (20)      785 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/get_rooms.py
--rw-r--r--   0 erik       (501) staff       (20)     2114 2022-08-22 13:30:34.000000 exchangelib-5.2.0/exchangelib/services/get_searchable_mailboxes.py
--rw-r--r--   0 erik       (501) staff       (20)     1475 2022-08-22 13:30:34.000000 exchangelib-5.2.0/exchangelib/services/get_server_time_zones.py
--rw-r--r--   0 erik       (501) staff       (20)     5077 2022-08-22 13:30:34.000000 exchangelib-5.2.0/exchangelib/services/get_streaming_events.py
--rw-r--r--   0 erik       (501) staff       (20)     2217 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/get_user_availability.py
--rw-r--r--   0 erik       (501) staff       (20)     1584 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/get_user_configuration.py
--rw-r--r--   0 erik       (501) staff       (20)     1518 2022-08-22 13:30:34.000000 exchangelib-5.2.0/exchangelib/services/get_user_oof_settings.py
--rw-r--r--   0 erik       (501) staff       (20)     4145 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/services/get_user_settings.py
--rw-r--r--   0 erik       (501) staff       (20)     5770 2024-03-03 21:14:09.000000 exchangelib-5.2.0/exchangelib/services/inbox_rules.py
--rw-r--r--   0 erik       (501) staff       (20)     1085 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/mark_as_junk.py
--rw-r--r--   0 erik       (501) staff       (20)     1276 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/move_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     1237 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/move_item.py
--rw-r--r--   0 erik       (501) staff       (20)     4812 2022-11-11 12:12:44.000000 exchangelib-5.2.0/exchangelib/services/resolve_names.py
--rw-r--r--   0 erik       (501) staff       (20)     1243 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/send_item.py
--rw-r--r--   0 erik       (501) staff       (20)     1603 2022-11-10 14:59:43.000000 exchangelib-5.2.0/exchangelib/services/send_notification.py
--rw-r--r--   0 erik       (501) staff       (20)     1503 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/set_user_oof_settings.py
--rw-r--r--   0 erik       (501) staff       (20)     5139 2024-03-03 21:14:09.000000 exchangelib-5.2.0/exchangelib/services/subscribe.py
--rw-r--r--   0 erik       (501) staff       (20)     3756 2022-11-11 08:05:01.000000 exchangelib-5.2.0/exchangelib/services/sync_folder_hierarchy.py
--rw-r--r--   0 erik       (501) staff       (20)     3590 2022-11-11 12:09:18.000000 exchangelib-5.2.0/exchangelib/services/sync_folder_items.py
--rw-r--r--   0 erik       (501) staff       (20)      738 2022-08-22 13:30:34.000000 exchangelib-5.2.0/exchangelib/services/unsubscribe.py
--rw-r--r--   0 erik       (501) staff       (20)     7615 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/services/update_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     4788 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/services/update_item.py
--rw-r--r--   0 erik       (501) staff       (20)      663 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/update_user_configuration.py
--rw-r--r--   0 erik       (501) staff       (20)     2113 2022-11-07 13:44:09.000000 exchangelib-5.2.0/exchangelib/services/upload_items.py
--rw-r--r--   0 erik       (501) staff       (20)     3907 2022-08-22 13:30:34.000000 exchangelib-5.2.0/exchangelib/settings.py
--rw-r--r--   0 erik       (501) staff       (20)     7956 2023-05-03 11:21:13.000000 exchangelib-5.2.0/exchangelib/transport.py
--rw-r--r--   0 erik       (501) staff       (20)    33828 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/util.py
--rw-r--r--   0 erik       (501) staff       (20)    13974 2023-11-15 18:16:03.000000 exchangelib-5.2.0/exchangelib/version.py
--rw-r--r--   0 erik       (501) staff       (20)    37550 2024-03-03 21:14:09.000000 exchangelib-5.2.0/exchangelib/winzone.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-03-08 09:53:57.108870 exchangelib-5.2.0/exchangelib.egg-info/
--rw-r--r--   0 erik       (501) staff       (20)     3597 2024-03-08 09:53:57.000000 exchangelib-5.2.0/exchangelib.egg-info/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     3294 2024-03-08 09:53:57.000000 exchangelib-5.2.0/exchangelib.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2024-03-08 09:53:57.000000 exchangelib-5.2.0/exchangelib.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (501) staff       (20)      315 2024-03-08 09:53:57.000000 exchangelib-5.2.0/exchangelib.egg-info/requires.txt
--rw-r--r--   0 erik       (501) staff       (20)       12 2024-03-08 09:53:57.000000 exchangelib-5.2.0/exchangelib.egg-info/top_level.txt
--rw-r--r--   0 erik       (501) staff       (20)     2171 2024-03-03 15:20:26.000000 exchangelib-5.2.0/pyproject.toml
--rw-r--r--   0 erik       (501) staff       (20)       38 2024-03-08 09:53:57.109757 exchangelib-5.2.0/setup.cfg
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-11 17:15:04.841815 exchangelib-5.2.1/
+-rw-r--r--   0 erik       (501) staff       (20)    38760 2024-04-11 17:12:03.000000 exchangelib-5.2.1/CHANGELOG.md
+-rw-r--r--   0 erik       (501) staff       (20)     1313 2022-01-03 12:16:38.000000 exchangelib-5.2.1/LICENSE
+-rw-r--r--   0 erik       (501) staff       (20)       91 2024-03-03 15:20:26.000000 exchangelib-5.2.1/MANIFEST.in
+-rw-r--r--   0 erik       (501) staff       (20)     3597 2024-04-11 17:15:04.841594 exchangelib-5.2.1/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)     1978 2023-11-15 18:16:03.000000 exchangelib-5.2.1/README.md
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-11 17:15:04.831478 exchangelib-5.2.1/exchangelib/
+-rw-r--r--   0 erik       (501) staff       (20)     2819 2024-04-11 17:06:28.000000 exchangelib-5.2.1/exchangelib/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)    36054 2024-03-26 11:46:04.000000 exchangelib-5.2.1/exchangelib/account.py
+-rw-r--r--   0 erik       (501) staff       (20)     9526 2022-11-24 11:30:07.000000 exchangelib-5.2.1/exchangelib/attachments.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-11 17:15:04.832494 exchangelib-5.2.1/exchangelib/autodiscover/
+-rw-r--r--   0 erik       (501) staff       (20)      499 2022-11-23 00:50:30.000000 exchangelib-5.2.1/exchangelib/autodiscover/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)     5986 2022-11-17 13:10:32.000000 exchangelib-5.2.1/exchangelib/autodiscover/cache.py
+-rw-r--r--   0 erik       (501) staff       (20)    22636 2023-11-15 18:16:03.000000 exchangelib-5.2.1/exchangelib/autodiscover/discovery.py
+-rw-r--r--   0 erik       (501) staff       (20)     2164 2023-11-15 18:16:03.000000 exchangelib-5.2.1/exchangelib/autodiscover/protocol.py
+-rw-r--r--   0 erik       (501) staff       (20)     4193 2022-10-10 07:45:39.000000 exchangelib-5.2.1/exchangelib/configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)    12159 2024-03-03 21:14:09.000000 exchangelib-5.2.1/exchangelib/credentials.py
+-rw-r--r--   0 erik       (501) staff       (20)    31304 2024-03-03 21:14:09.000000 exchangelib-5.2.1/exchangelib/errors.py
+-rw-r--r--   0 erik       (501) staff       (20)    11527 2023-11-15 18:16:03.000000 exchangelib-5.2.1/exchangelib/ewsdatetime.py
+-rw-r--r--   0 erik       (501) staff       (20)    12821 2022-11-24 11:54:53.000000 exchangelib-5.2.1/exchangelib/extended_properties.py
+-rw-r--r--   0 erik       (501) staff       (20)    64456 2024-03-26 09:57:40.000000 exchangelib-5.2.1/exchangelib/fields.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-11 17:15:04.833409 exchangelib-5.2.1/exchangelib/folders/
+-rw-r--r--   0 erik       (501) staff       (20)     5250 2024-03-18 11:34:30.000000 exchangelib-5.2.1/exchangelib/folders/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)    39512 2024-03-26 09:32:06.000000 exchangelib-5.2.1/exchangelib/folders/base.py
+-rw-r--r--   0 erik       (501) staff       (20)    23778 2024-03-17 10:08:54.000000 exchangelib-5.2.1/exchangelib/folders/collections.py
+-rw-r--r--   0 erik       (501) staff       (20)    20228 2024-03-18 11:50:03.000000 exchangelib-5.2.1/exchangelib/folders/known_folders.py
+-rw-r--r--   0 erik       (501) staff       (20)     6876 2023-07-23 10:17:42.000000 exchangelib-5.2.1/exchangelib/folders/queryset.py
+-rw-r--r--   0 erik       (501) staff       (20)    16330 2024-03-26 09:32:06.000000 exchangelib-5.2.1/exchangelib/folders/roots.py
+-rw-r--r--   0 erik       (501) staff       (20)     2934 2022-08-22 13:30:33.000000 exchangelib-5.2.1/exchangelib/indexed_properties.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-11 17:15:04.834464 exchangelib-5.2.1/exchangelib/items/
+-rw-r--r--   0 erik       (501) staff       (20)     3381 2023-11-15 18:16:03.000000 exchangelib-5.2.1/exchangelib/items/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)     9898 2022-08-22 13:30:33.000000 exchangelib-5.2.1/exchangelib/items/base.py
+-rw-r--r--   0 erik       (501) staff       (20)    20811 2023-11-15 18:16:03.000000 exchangelib-5.2.1/exchangelib/items/calendar_item.py
+-rw-r--r--   0 erik       (501) staff       (20)    15113 2023-05-04 21:52:26.000000 exchangelib-5.2.1/exchangelib/items/contact.py
+-rw-r--r--   0 erik       (501) staff       (20)    17951 2023-08-21 05:19:29.000000 exchangelib-5.2.1/exchangelib/items/item.py
+-rw-r--r--   0 erik       (501) staff       (20)     9050 2023-11-15 18:16:03.000000 exchangelib-5.2.1/exchangelib/items/message.py
+-rw-r--r--   0 erik       (501) staff       (20)     1405 2022-08-22 13:30:33.000000 exchangelib-5.2.1/exchangelib/items/post.py
+-rw-r--r--   0 erik       (501) staff       (20)     5876 2023-05-04 21:52:26.000000 exchangelib-5.2.1/exchangelib/items/task.py
+-rw-r--r--   0 erik       (501) staff       (20)    90509 2024-03-26 11:47:43.000000 exchangelib-5.2.1/exchangelib/properties.py
+-rw-r--r--   0 erik       (501) staff       (20)    35041 2024-03-07 10:53:09.000000 exchangelib-5.2.1/exchangelib/protocol.py
+-rw-r--r--   0 erik       (501) staff       (20)    29695 2024-03-18 13:00:51.000000 exchangelib-5.2.1/exchangelib/queryset.py
+-rw-r--r--   0 erik       (501) staff       (20)    13139 2022-10-07 08:02:07.000000 exchangelib-5.2.1/exchangelib/recurrence.py
+-rw-r--r--   0 erik       (501) staff       (20)    25489 2022-10-07 08:04:06.000000 exchangelib-5.2.1/exchangelib/restriction.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-11 17:15:04.840875 exchangelib-5.2.1/exchangelib/services/
+-rw-r--r--   0 erik       (501) staff       (20)     3775 2024-03-03 21:14:09.000000 exchangelib-5.2.1/exchangelib/services/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)     1247 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/archive_item.py
+-rw-r--r--   0 erik       (501) staff       (20)    46573 2024-03-18 07:20:38.000000 exchangelib-5.2.1/exchangelib/services/common.py
+-rw-r--r--   0 erik       (501) staff       (20)     2097 2022-11-07 14:52:15.000000 exchangelib-5.2.1/exchangelib/services/convert_id.py
+-rw-r--r--   0 erik       (501) staff       (20)      209 2022-08-22 13:30:33.000000 exchangelib-5.2.1/exchangelib/services/copy_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     1532 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/create_attachment.py
+-rw-r--r--   0 erik       (501) staff       (20)     1988 2023-11-15 18:16:03.000000 exchangelib-5.2.1/exchangelib/services/create_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     4272 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/create_item.py
+-rw-r--r--   0 erik       (501) staff       (20)      686 2022-08-22 13:30:33.000000 exchangelib-5.2.1/exchangelib/services/create_user_configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)      969 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/delete_attachment.py
+-rw-r--r--   0 erik       (501) staff       (20)      931 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/delete_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     2504 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/delete_item.py
+-rw-r--r--   0 erik       (501) staff       (20)      710 2022-08-22 13:30:33.000000 exchangelib-5.2.1/exchangelib/services/delete_user_configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)     1088 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/empty_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)      889 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/expand_dl.py
+-rw-r--r--   0 erik       (501) staff       (20)     1060 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/export_items.py
+-rw-r--r--   0 erik       (501) staff       (20)     3621 2023-11-15 18:16:03.000000 exchangelib-5.2.1/exchangelib/services/find_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     4326 2022-11-11 08:05:01.000000 exchangelib-5.2.1/exchangelib/services/find_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     4768 2022-11-11 08:05:01.000000 exchangelib-5.2.1/exchangelib/services/find_people.py
+-rw-r--r--   0 erik       (501) staff       (20)     5392 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/get_attachment.py
+-rw-r--r--   0 erik       (501) staff       (20)     1914 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/get_delegate.py
+-rw-r--r--   0 erik       (501) staff       (20)     1186 2022-08-22 13:30:34.000000 exchangelib-5.2.1/exchangelib/services/get_events.py
+-rw-r--r--   0 erik       (501) staff       (20)     2620 2024-04-11 17:05:53.000000 exchangelib-5.2.1/exchangelib/services/get_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     1627 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/get_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     1576 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/get_mail_tips.py
+-rw-r--r--   0 erik       (501) staff       (20)     1127 2022-08-22 13:30:34.000000 exchangelib-5.2.1/exchangelib/services/get_persona.py
+-rw-r--r--   0 erik       (501) staff       (20)      696 2022-08-22 13:30:34.000000 exchangelib-5.2.1/exchangelib/services/get_room_lists.py
+-rw-r--r--   0 erik       (501) staff       (20)      785 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/get_rooms.py
+-rw-r--r--   0 erik       (501) staff       (20)     2114 2022-08-22 13:30:34.000000 exchangelib-5.2.1/exchangelib/services/get_searchable_mailboxes.py
+-rw-r--r--   0 erik       (501) staff       (20)     1475 2022-08-22 13:30:34.000000 exchangelib-5.2.1/exchangelib/services/get_server_time_zones.py
+-rw-r--r--   0 erik       (501) staff       (20)     5077 2022-08-22 13:30:34.000000 exchangelib-5.2.1/exchangelib/services/get_streaming_events.py
+-rw-r--r--   0 erik       (501) staff       (20)     2217 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/get_user_availability.py
+-rw-r--r--   0 erik       (501) staff       (20)     1584 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/get_user_configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)     1518 2022-08-22 13:30:34.000000 exchangelib-5.2.1/exchangelib/services/get_user_oof_settings.py
+-rw-r--r--   0 erik       (501) staff       (20)     4145 2023-11-15 18:16:03.000000 exchangelib-5.2.1/exchangelib/services/get_user_settings.py
+-rw-r--r--   0 erik       (501) staff       (20)     4647 2024-03-26 09:33:46.000000 exchangelib-5.2.1/exchangelib/services/inbox_rules.py
+-rw-r--r--   0 erik       (501) staff       (20)     1085 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/mark_as_junk.py
+-rw-r--r--   0 erik       (501) staff       (20)     1276 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/move_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     1237 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/move_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     4812 2022-11-11 12:12:44.000000 exchangelib-5.2.1/exchangelib/services/resolve_names.py
+-rw-r--r--   0 erik       (501) staff       (20)     1243 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/send_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     1603 2022-11-10 14:59:43.000000 exchangelib-5.2.1/exchangelib/services/send_notification.py
+-rw-r--r--   0 erik       (501) staff       (20)     1503 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/set_user_oof_settings.py
+-rw-r--r--   0 erik       (501) staff       (20)     5139 2024-03-03 21:14:09.000000 exchangelib-5.2.1/exchangelib/services/subscribe.py
+-rw-r--r--   0 erik       (501) staff       (20)     3756 2022-11-11 08:05:01.000000 exchangelib-5.2.1/exchangelib/services/sync_folder_hierarchy.py
+-rw-r--r--   0 erik       (501) staff       (20)     3590 2022-11-11 12:09:18.000000 exchangelib-5.2.1/exchangelib/services/sync_folder_items.py
+-rw-r--r--   0 erik       (501) staff       (20)      738 2022-08-22 13:30:34.000000 exchangelib-5.2.1/exchangelib/services/unsubscribe.py
+-rw-r--r--   0 erik       (501) staff       (20)     7615 2023-11-15 18:16:03.000000 exchangelib-5.2.1/exchangelib/services/update_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     4788 2023-11-15 18:16:03.000000 exchangelib-5.2.1/exchangelib/services/update_item.py
+-rw-r--r--   0 erik       (501) staff       (20)      663 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/update_user_configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)     2113 2022-11-07 13:44:09.000000 exchangelib-5.2.1/exchangelib/services/upload_items.py
+-rw-r--r--   0 erik       (501) staff       (20)     3907 2022-08-22 13:30:34.000000 exchangelib-5.2.1/exchangelib/settings.py
+-rw-r--r--   0 erik       (501) staff       (20)     7956 2023-05-03 11:21:13.000000 exchangelib-5.2.1/exchangelib/transport.py
+-rw-r--r--   0 erik       (501) staff       (20)    33828 2023-11-15 18:16:03.000000 exchangelib-5.2.1/exchangelib/util.py
+-rw-r--r--   0 erik       (501) staff       (20)    13974 2023-11-15 18:16:03.000000 exchangelib-5.2.1/exchangelib/version.py
+-rw-r--r--   0 erik       (501) staff       (20)    37550 2024-03-03 21:14:09.000000 exchangelib-5.2.1/exchangelib/winzone.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-11 17:15:04.841079 exchangelib-5.2.1/exchangelib.egg-info/
+-rw-r--r--   0 erik       (501) staff       (20)     3597 2024-04-11 17:15:04.000000 exchangelib-5.2.1/exchangelib.egg-info/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)     3294 2024-04-11 17:15:04.000000 exchangelib-5.2.1/exchangelib.egg-info/SOURCES.txt
+-rw-r--r--   0 erik       (501) staff       (20)        1 2024-04-11 17:15:04.000000 exchangelib-5.2.1/exchangelib.egg-info/dependency_links.txt
+-rw-r--r--   0 erik       (501) staff       (20)      315 2024-04-11 17:15:04.000000 exchangelib-5.2.1/exchangelib.egg-info/requires.txt
+-rw-r--r--   0 erik       (501) staff       (20)       12 2024-04-11 17:15:04.000000 exchangelib-5.2.1/exchangelib.egg-info/top_level.txt
+-rw-r--r--   0 erik       (501) staff       (20)     2171 2024-03-03 15:20:26.000000 exchangelib-5.2.1/pyproject.toml
+-rw-r--r--   0 erik       (501) staff       (20)       38 2024-04-11 17:15:04.841856 exchangelib-5.2.1/setup.cfg
```

### Comparing `exchangelib-5.2.0/CHANGELOG.md` & `exchangelib-5.2.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Change Log
 ==========
 
 HEAD
 ----
 
 
+5.2.1
+-----
+- Fix `ErrorAccessDenied: Not allowed to access Non IPM folder` caused by recent changes in O365.
+- Add more intuitive API for inbox rules
+- Fix various bugs with inbox creation
+
+
 5.2.0
 -----
 - Allow setting a custom `Configuration.max_conections` in autodiscover mode
 - Add support for inbox rules. See documentation for examples.
 - Fix shared folder access in delegate mode
 - Support subscribing to all folders instead of specific folders
 
 
-
 5.1.0
 -----
 - Fix QuerySet operations on shared folders
 - Fix globbing on patterns with more than two folder levels
 - Fix case sensitivity of "/" folder navigation
 - Multiple improvements related to consistency and graceful error handling
```

### Comparing `exchangelib-5.2.0/LICENSE` & `exchangelib-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/PKG-INFO` & `exchangelib-5.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchangelib
-Version: 5.2.0
+Version: 5.2.1
 Summary: Client for Microsoft Exchange Web Services (EWS)
 Author-email: Erik Cederstrand <erik@cederstrand.dk>
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/ecederstrand/exchangelib
 Project-URL: Issues, https://github.com/ecederstrand/exchangelib/issues
 Project-URL: Documentation, https://ecederstrand.github.io/exchangelib/
 Project-URL: Repository, https://github.com/ecederstrand/exchangelib.git
```

### Comparing `exchangelib-5.2.0/README.md` & `exchangelib-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/__init__.py` & `exchangelib-5.2.1/exchangelib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from .properties import UID, Attendee, Body, DLMailbox, HTMLBody, ItemId, Mailbox, Room, RoomList
 from .protocol import BaseProtocol, FailFast, FaultTolerance, NoVerifyHTTPAdapter, TLSClientAuth
 from .restriction import Q
 from .settings import OofSettings
 from .transport import BASIC, CBA, DIGEST, GSSAPI, NTLM, OAUTH2, SSPI
 from .version import Build, Version
 
-__version__ = "5.2.0"
+__version__ = "5.2.1"
 
 __all__ = [
     "__version__",
     "AcceptItem",
     "Account",
     "Attendee",
     "BASIC",
```

### Comparing `exchangelib-5.2.0/exchangelib/account.py` & `exchangelib-5.2.1/exchangelib/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from logging import getLogger
 
 from cached_property import threaded_cached_property
 
 from .autodiscover import Autodiscovery
 from .configuration import Configuration
 from .credentials import ACCESS_TYPES, DELEGATE, IMPERSONATION
-from .errors import ErrorItemNotFound, InvalidEnumValue, InvalidTypeError, ResponseMessageError, UnknownTimeZone
+from .errors import InvalidEnumValue, InvalidTypeError, ResponseMessageError, UnknownTimeZone
 from .ewsdatetime import UTC, EWSTimeZone
 from .fields import FieldPath, TextField
 from .folders import (
     AdminAuditLogs,
     ArchiveDeletedItems,
     ArchiveInbox,
     ArchiveMsgFolderRoot,
@@ -783,24 +783,19 @@
         :return: None if success, else raises an error.
         """
         SetInboxRule(account=self).get(rule=rule)
 
     def delete_rule(self, rule: Rule):
         """Delete an Inbox rule.
 
-        :param rule: The rule to delete. Must have ID or 'display_name'.
+        :param rule: The rule to delete. Must have an ID.
         :return: None if success, else raises an error.
         """
         if not rule.id:
-            if not rule.display_name:
-                raise ValueError("Rule must have ID or display_name")
-            try:
-                rule = {i.display_name: i for i in GetInboxRules(account=self).call()}[rule.display_name]
-            except KeyError:
-                raise ErrorItemNotFound(f"No rule with name {rule.display_name!r}")
+            raise ValueError("Rule must have an ID")
         DeleteInboxRule(account=self).get(rule=rule)
         rule.id = None
 
     def subscribe_to_pull(self, event_types=None, watermark=None, timeout=60):
         """Create a pull subscription.
 
         :param event_types: List of event types to subscribe to. Possible values defined in SubscribeToPull.EVENT_TYPES
```

### Comparing `exchangelib-5.2.0/exchangelib/attachments.py` & `exchangelib-5.2.1/exchangelib/attachments.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/autodiscover/cache.py` & `exchangelib-5.2.1/exchangelib/autodiscover/cache.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/autodiscover/discovery.py` & `exchangelib-5.2.1/exchangelib/autodiscover/discovery.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/autodiscover/protocol.py` & `exchangelib-5.2.1/exchangelib/autodiscover/protocol.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/configuration.py` & `exchangelib-5.2.1/exchangelib/configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/credentials.py` & `exchangelib-5.2.1/exchangelib/credentials.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/errors.py` & `exchangelib-5.2.1/exchangelib/errors.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/ewsdatetime.py` & `exchangelib-5.2.1/exchangelib/ewsdatetime.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/extended_properties.py` & `exchangelib-5.2.1/exchangelib/extended_properties.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/fields.py` & `exchangelib-5.2.1/exchangelib/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1171,14 +1171,27 @@
 
     def clean(self, value, version=None):
         if value is not None:
             value = [self.value_cls(email_address=s) if isinstance(s, str) else s for s in value]
         return super().clean(value, version=version)
 
 
+class AddressListField(EWSElementListField):
+    def __init__(self, *args, **kwargs):
+        from .properties import Address
+
+        kwargs["value_cls"] = Address
+        super().__init__(*args, **kwargs)
+
+    def clean(self, value, version=None):
+        if value is not None:
+            value = [self.value_cls(email_address=s) if isinstance(s, str) else s for s in value]
+        return super().clean(value, version=version)
+
+
 class MemberListField(EWSElementListField):
     def __init__(self, *args, **kwargs):
         from .properties import Member
 
         kwargs["value_cls"] = Member
         super().__init__(*args, **kwargs)
 
@@ -1781,7 +1794,23 @@
 
 class SensitivityField(ChoiceField):
     """A field that indicates the sensitivity level of an item."""
 
     def __init__(self, *args, **kwargs):
         kwargs["choices"] = SENSITIVITY_CHOICES
         super().__init__(*args, **kwargs)
+
+
+class FolderActionField(EWSElementField):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def clean(self, value, version=None):
+        from .folders import DistinguishedFolderId, Folder
+
+        if isinstance(value, Folder):
+            folder_id = value.to_id()
+            if isinstance(folder_id, DistinguishedFolderId):
+                value = self.value_cls(distinguished_folder_id=folder_id)
+            else:
+                value = self.value_cls(folder_id=folder_id)
+        return super().clean(value, version=version)
```

### Comparing `exchangelib-5.2.0/exchangelib/folders/__init__.py` & `exchangelib-5.2.1/exchangelib/folders/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from ..properties import DistinguishedFolderId, FolderId
 from .base import BaseFolder, Folder
 from .collections import FolderCollection
 from .known_folders import (
     NON_DELETABLE_FOLDERS,
     AdminAuditLogs,
+    AllCategorizedItems,
     AllContacts,
     AllItems,
+    AllPersonMetadata,
+    AllTodoTasks,
     ApplicationData,
     ArchiveDeletedItems,
     ArchiveInbox,
     ArchiveMsgFolderRoot,
     ArchiveRecoverableItemsDeletions,
     ArchiveRecoverableItemsPurges,
     ArchiveRecoverableItemsRoot,
@@ -29,78 +32,98 @@
     DeferredAction,
     DeletedItems,
     Directory,
     DlpPolicyEvaluation,
     Drafts,
     EventCheckPoints,
     ExchangeSyncData,
+    ExternalContacts,
     Favorites,
     Files,
+    FolderMemberships,
     FreeBusyCache,
     FreebusyData,
     Friends,
+    FromFavoriteSenders,
     GALContacts,
     GraphAnalytics,
     IMContactList,
     Inbox,
+    Inference,
     Journal,
     JunkEmail,
     LocalFailures,
     Location,
     MailboxAssociations,
     Messages,
     MsgFolderRoot,
     MyContacts,
     MyContactsExtended,
-    NonDeletableFolderMixIn,
+    NonDeletableFolder,
     Notes,
+    OneNotePagePreviews,
     OrganizationalContacts,
     Outbox,
     ParkedMessages,
     PassThroughSearchResults,
     PdpProfileV2Secured,
     PeopleCentricConversationBuddies,
     PeopleConnect,
+    QedcDefaultRetention,
+    QedcLongRetention,
+    QedcMediumRetention,
+    QedcShortRetention,
+    QuarantinedEmail,
+    QuarantinedEmailDefaultCategory,
     QuickContacts,
     RecipientCache,
     RecoverableItemsDeletions,
     RecoverableItemsPurges,
     RecoverableItemsRoot,
+    RecoverableItemsSubstrateHolds,
     RecoverableItemsVersions,
     RecoveryPoints,
+    RelevantContacts,
     Reminders,
     RSSFeeds,
     Schedule,
     SearchFolders,
     SentItems,
     ServerFailures,
+    SharePointNotifications,
     Sharing,
     Shortcuts,
+    ShortNotes,
     Signal,
     SkypeTeamsMessages,
     SmsAndChatsSync,
     SpoolerQueue,
     SwssItems,
     SyncIssues,
     System,
+    System1,
     Tasks,
     TemporarySaves,
     ToDoSearch,
+    UserCuratedContacts,
     Views,
     VoiceMail,
     WellknownFolder,
     WorkingSet,
 )
 from .queryset import DEEP, FOLDER_TRAVERSAL_CHOICES, SHALLOW, SOFT_DELETED, FolderQuerySet, SingleFolderQuerySet
 from .roots import ArchiveRoot, PublicFoldersRoot, Root, RootOfHierarchy
 
 __all__ = [
     "AdminAuditLogs",
+    "AllCategorizedItems",
     "AllContacts",
     "AllItems",
+    "AllPersonMetadata",
+    "AllTodoTasks",
     "ApplicationData",
     "ArchiveDeletedItems",
     "ArchiveInbox",
     "ArchiveMsgFolderRoot",
     "ArchiveRecoverableItemsDeletions",
     "ArchiveRecoverableItemsPurges",
     "ArchiveRecoverableItemsRoot",
@@ -124,76 +147,93 @@
     "DeletedItems",
     "Directory",
     "DistinguishedFolderId",
     "DlpPolicyEvaluation",
     "Drafts",
     "EventCheckPoints",
     "ExchangeSyncData",
+    "ExternalContacts",
     "FOLDER_TRAVERSAL_CHOICES",
     "Favorites",
     "Files",
     "Folder",
     "FolderCollection",
     "FolderId",
+    "FolderMemberships",
     "FolderQuerySet",
     "FreeBusyCache",
     "FreebusyData",
     "Friends",
+    "FromFavoriteSenders",
     "GALContacts",
     "GraphAnalytics",
     "IMContactList",
     "Inbox",
+    "Inference",
     "Journal",
     "JunkEmail",
     "LocalFailures",
     "Location",
     "MailboxAssociations",
     "Messages",
     "MsgFolderRoot",
     "MyContacts",
     "MyContactsExtended",
     "NON_DELETABLE_FOLDERS",
-    "NonDeletableFolderMixIn",
+    "NonDeletableFolder",
     "Notes",
+    "OneNotePagePreviews",
     "OrganizationalContacts",
     "Outbox",
     "ParkedMessages",
     "PassThroughSearchResults",
     "PdpProfileV2Secured",
     "PeopleCentricConversationBuddies",
     "PeopleConnect",
+    "QedcDefaultRetention",
+    "QedcMediumRetention",
+    "QedcLongRetention",
+    "QedcShortRetention",
+    "QuarantinedEmail",
+    "QuarantinedEmailDefaultCategory",
     "PublicFoldersRoot",
     "QuickContacts",
     "RSSFeeds",
     "RecipientCache",
     "RecoverableItemsDeletions",
     "RecoverableItemsPurges",
     "RecoverableItemsRoot",
+    "RecoverableItemsSubstrateHolds",
     "RecoverableItemsVersions",
     "RecoveryPoints",
+    "RelevantContacts",
     "Reminders",
     "Root",
     "RootOfHierarchy",
     "SHALLOW",
     "SOFT_DELETED",
     "Schedule",
     "SearchFolders",
     "SentItems",
     "ServerFailures",
+    "SharePointNotifications",
     "Sharing",
     "Shortcuts",
+    "ShortNotes",
     "Signal",
     "SingleFolderQuerySet",
     "SkypeTeamsMessages",
     "SmsAndChatsSync",
     "SpoolerQueue",
     "SwssItems",
     "SyncIssues",
     "System",
+    "System1",
     "Tasks",
     "TemporarySaves",
     "ToDoSearch",
+    "UserCuratedContacts",
     "Views",
     "VoiceMail",
     "WellknownFolder",
     "WorkingSet",
 ]
```

### Comparing `exchangelib-5.2.0/exchangelib/folders/base.py` & `exchangelib-5.2.1/exchangelib/folders/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     DEFAULT_FOLDER_TRAVERSAL_DEPTH = DEEP_FOLDERS
     DEFAULT_ITEM_TRAVERSAL_DEPTH = SHALLOW_ITEMS
     LOCALIZED_NAMES = {}  # A map of (str)locale: (tuple)localized_folder_names
     ITEM_MODEL_MAP = {cls.response_tag(): cls for cls in ITEM_CLASSES}
     ID_ELEMENT_CLS = FolderId
 
     _id = IdElementField(field_uri="folder:FolderId", value_cls=ID_ELEMENT_CLS)
-    _distinguished_id = IdElementField(field_uri="folder:FolderId", value_cls=DistinguishedFolderId)
+    _distinguished_id = IdElementField(field_uri="folder:DistinguishedFolderId", value_cls=DistinguishedFolderId)
     parent_folder_id = EWSElementField(field_uri="folder:ParentFolderId", value_cls=ParentFolderId, is_read_only=True)
     folder_class = CharField(field_uri="folder:FolderClass", is_required_after_save=True)
     name = CharField(field_uri="folder:DisplayName")
     total_count = IntegerField(field_uri="folder:TotalCount", is_read_only=True)
     child_folder_count = IntegerField(field_uri="folder:ChildFolderCount", is_read_only=True)
     unread_count = IntegerField(field_uri="folder:UnreadCount", is_read_only=True)
 
@@ -217,15 +217,15 @@
     def has_distinguished_name(self):
         return self.name and self.DISTINGUISHED_FOLDER_ID and self.name.lower() == self.DISTINGUISHED_FOLDER_ID.lower()
 
     @classmethod
     def localized_names(cls, locale):
         # Return localized names for a specific locale. If no locale-specific names exist, return the default names,
         # if any.
-        return tuple(s.lower() for s in cls.LOCALIZED_NAMES.get(locale, cls.LOCALIZED_NAMES.get(None, [])))
+        return tuple(s.lower() for s in cls.LOCALIZED_NAMES.get(locale, cls.LOCALIZED_NAMES.get(None, [cls.__name__])))
 
     @staticmethod
     def folder_cls_from_container_class(container_class):
         """Return a reasonable folder class given a container class, e.g. 'IPF.Note'. Don't iterate WELLKNOWN_FOLDERS
         because many folder classes have the same CONTAINER_CLASS.
 
         :param container_class:
@@ -853,26 +853,26 @@
     @classmethod
     def deregister(cls, *args, **kwargs):
         if cls is not Folder:
             raise TypeError("For folders, custom fields must be registered on the Folder class")
         return super().deregister(*args, **kwargs)
 
     @classmethod
-    def get_distinguished(cls, root):
+    def get_distinguished(cls, account):
         """Get the distinguished folder for this folder class.
 
-        :param root:
+        :param account:
         :return:
         """
         try:
             return cls.resolve(
-                account=root.account,
+                account=account,
                 folder=DistinguishedFolderId(
                     id=cls.DISTINGUISHED_FOLDER_ID,
-                    mailbox=Mailbox(email_address=root.account.primary_smtp_address),
+                    mailbox=Mailbox(email_address=account.primary_smtp_address),
                 ),
             )
         except MISSING_FOLDER_ERRORS:
             raise ErrorFolderNotFound(f"Could not find distinguished folder {cls.DISTINGUISHED_FOLDER_ID!r}")
 
     @property
     def parent(self):
```

### Comparing `exchangelib-5.2.0/exchangelib/folders/collections.py` & `exchangelib-5.2.1/exchangelib/folders/collections.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/folders/known_folders.py` & `exchangelib-5.2.1/exchangelib/folders/known_folders.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,21 +12,65 @@
 )
 from ..properties import EWSMeta
 from ..version import EXCHANGE_2010_SP1, EXCHANGE_2013, EXCHANGE_2013_SP1
 from .base import Folder
 from .collections import FolderCollection
 
 
-class Calendar(Folder):
+class Birthdays(Folder):
+    CONTAINER_CLASS = "IPF.Appointment.Birthday"
+    LOCALIZED_NAMES = {
+        "da_DK": ("Fødselsdage",),
+    }
+
+
+class CrawlerData(Folder):
+    CONTAINER_CLASS = "IPF.StoreItem.CrawlerData"
+
+
+class EventCheckPoints(Folder):
+    CONTAINER_CLASS = "IPF.StoreItem.EventCheckPoints"
+
+
+class FreeBusyCache(Folder):
+    CONTAINER_CLASS = "IPF.StoreItem.FreeBusyCache"
+
+
+class RecoveryPoints(Folder):
+    CONTAINER_CLASS = "IPF.StoreItem.RecoveryPoints"
+
+
+class SkypeTeamsMessages(Folder):
+    CONTAINER_CLASS = "IPF.SkypeTeams.Message"
+    LOCALIZED_NAMES = {
+        None: ("Team-chat",),
+    }
+
+
+class SwssItems(Folder):
+    CONTAINER_CLASS = "IPF.StoreItem.SwssItems"
+
+
+class WellknownFolder(Folder, metaclass=EWSMeta):
+    """Base class to use until we have a more specific folder implementation for this folder."""
+
+    supported_item_models = ITEM_CLASSES
+
+
+class Messages(WellknownFolder):
+    CONTAINER_CLASS = "IPF.Note"
+    supported_item_models = (Message, MeetingRequest, MeetingResponse, MeetingCancellation)
+
+
+class Calendar(WellknownFolder):
     """An interface for the Exchange calendar."""
 
     DISTINGUISHED_FOLDER_ID = "calendar"
     CONTAINER_CLASS = "IPF.Appointment"
     supported_item_models = (CalendarItem,)
-
     LOCALIZED_NAMES = {
         "da_DK": ("Kalender",),
         "de_DE": ("Kalender",),
         "en_US": ("Calendar",),
         "es_ES": ("Calendario",),
         "fr_CA": ("Calendrier",),
         "nl_NL": ("Agenda",),
@@ -35,79 +79,50 @@
         "zh_CN": ("日历",),
     }
 
     def view(self, *args, **kwargs):
         return FolderCollection(account=self.account, folders=[self]).view(*args, **kwargs)
 
 
-class DeletedItems(Folder):
+class Contacts(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "contacts"
+    CONTAINER_CLASS = "IPF.Contact"
+    supported_item_models = (Contact, DistributionList)
+    LOCALIZED_NAMES = {
+        "da_DK": ("Kontaktpersoner",),
+        "de_DE": ("Kontakte",),
+        "en_US": ("Contacts",),
+        "es_ES": ("Contactos",),
+        "fr_CA": ("Contacts",),
+        "nl_NL": ("Contactpersonen",),
+        "ru_RU": ("Контакты",),
+        "sv_SE": ("Kontakter",),
+        "zh_CN": ("联系人",),
+    }
+
+
+class DeletedItems(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "deleteditems"
     CONTAINER_CLASS = "IPF.Note"
     supported_item_models = ITEM_CLASSES
-
     LOCALIZED_NAMES = {
         "da_DK": ("Slettet post",),
         "de_DE": ("Gelöschte Elemente",),
         "en_US": ("Deleted Items",),
         "es_ES": ("Elementos eliminados",),
         "fr_CA": ("Éléments supprimés",),
         "nl_NL": ("Verwijderde items",),
         "ru_RU": ("Удаленные",),
         "sv_SE": ("Borttaget",),
         "zh_CN": ("已删除邮件",),
     }
 
 
-class Messages(Folder):
-    CONTAINER_CLASS = "IPF.Note"
-    supported_item_models = (Message, MeetingRequest, MeetingResponse, MeetingCancellation)
-
-
-class CrawlerData(Folder):
-    CONTAINER_CLASS = "IPF.StoreItem.CrawlerData"
-
-
-class DlpPolicyEvaluation(Folder):
-    CONTAINER_CLASS = "IPF.StoreItem.DlpPolicyEvaluation"
-
-
-class FreeBusyCache(Folder):
-    CONTAINER_CLASS = "IPF.StoreItem.FreeBusyCache"
-
-
-class RecoveryPoints(Folder):
-    CONTAINER_CLASS = "IPF.StoreItem.RecoveryPoints"
-
-
-class SwssItems(Folder):
-    CONTAINER_CLASS = "IPF.StoreItem.SwssItems"
-
-
-class EventCheckPoints(Folder):
-    CONTAINER_CLASS = "IPF.StoreItem.EventCheckPoints"
-
-
-class SkypeTeamsMessages(Folder):
-    CONTAINER_CLASS = "IPF.SkypeTeams.Message"
-    LOCALIZED_NAMES = {
-        None: ("Team-chat",),
-    }
-
-
-class Birthdays(Folder):
-    CONTAINER_CLASS = "IPF.Appointment.Birthday"
-    LOCALIZED_NAMES = {
-        None: ("Birthdays",),
-        "da_DK": ("Fødselsdage",),
-    }
-
-
 class Drafts(Messages):
     DISTINGUISHED_FOLDER_ID = "drafts"
-
     LOCALIZED_NAMES = {
         "da_DK": ("Kladder",),
         "de_DE": ("Entwürfe",),
         "en_US": ("Drafts",),
         "es_ES": ("Borradores",),
         "fr_CA": ("Brouillons",),
         "nl_NL": ("Concepten",),
@@ -115,31 +130,44 @@
         "sv_SE": ("Utkast",),
         "zh_CN": ("草稿",),
     }
 
 
 class Inbox(Messages):
     DISTINGUISHED_FOLDER_ID = "inbox"
-
     LOCALIZED_NAMES = {
         "da_DK": ("Indbakke",),
         "de_DE": ("Posteingang",),
         "en_US": ("Inbox",),
         "es_ES": ("Bandeja de entrada",),
         "fr_CA": ("Boîte de réception",),
         "nl_NL": ("Postvak IN",),
         "ru_RU": ("Входящие",),
         "sv_SE": ("Inkorgen",),
         "zh_CN": ("收件箱",),
     }
 
 
+class JunkEmail(Messages):
+    DISTINGUISHED_FOLDER_ID = "junkemail"
+    LOCALIZED_NAMES = {
+        "da_DK": ("Uønsket e-mail",),
+        "de_DE": ("Junk-E-Mail",),
+        "en_US": ("Junk E-mail",),
+        "es_ES": ("Correo no deseado",),
+        "fr_CA": ("Courrier indésirables",),
+        "nl_NL": ("Ongewenste e-mail",),
+        "ru_RU": ("Нежелательная почта",),
+        "sv_SE": ("Skräppost",),
+        "zh_CN": ("垃圾邮件",),
+    }
+
+
 class Outbox(Messages):
     DISTINGUISHED_FOLDER_ID = "outbox"
-
     LOCALIZED_NAMES = {
         "da_DK": ("Udbakke",),
         "de_DE": ("Postausgang",),
         "en_US": ("Outbox",),
         "es_ES": ("Bandeja de salida",),
         "fr_CA": ("Boîte d'envoi",),
         "nl_NL": ("Postvak UIT",),
@@ -147,90 +175,68 @@
         "sv_SE": ("Utkorgen",),
         "zh_CN": ("发件箱",),
     }
 
 
 class SentItems(Messages):
     DISTINGUISHED_FOLDER_ID = "sentitems"
-
     LOCALIZED_NAMES = {
         "da_DK": ("Sendt post",),
         "de_DE": ("Gesendete Elemente",),
         "en_US": ("Sent Items",),
         "es_ES": ("Elementos enviados",),
         "fr_CA": ("Éléments envoyés",),
         "nl_NL": ("Verzonden items",),
         "ru_RU": ("Отправленные",),
         "sv_SE": ("Skickat",),
         "zh_CN": ("已发送邮件",),
     }
 
 
-class JunkEmail(Messages):
-    DISTINGUISHED_FOLDER_ID = "junkemail"
-
-    LOCALIZED_NAMES = {
-        "da_DK": ("Uønsket e-mail",),
-        "de_DE": ("Junk-E-Mail",),
-        "en_US": ("Junk E-mail",),
-        "es_ES": ("Correo no deseado",),
-        "fr_CA": ("Courrier indésirables",),
-        "nl_NL": ("Ongewenste e-mail",),
-        "ru_RU": ("Нежелательная почта",),
-        "sv_SE": ("Skräppost",),
-        "zh_CN": ("垃圾邮件",),
-    }
-
-
-class Tasks(Folder):
+class Tasks(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "tasks"
     CONTAINER_CLASS = "IPF.Task"
     supported_item_models = (Task,)
-
     LOCALIZED_NAMES = {
         "da_DK": ("Opgaver",),
         "de_DE": ("Aufgaben",),
         "en_US": ("Tasks",),
         "es_ES": ("Tareas",),
         "fr_CA": ("Tâches",),
         "nl_NL": ("Taken",),
         "ru_RU": ("Задачи",),
         "sv_SE": ("Uppgifter",),
         "zh_CN": ("任务",),
     }
 
 
-class Contacts(Folder):
-    DISTINGUISHED_FOLDER_ID = "contacts"
-    CONTAINER_CLASS = "IPF.Contact"
-    supported_item_models = (Contact, DistributionList)
+class AdminAuditLogs(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "adminauditlogs"
+    supported_from = EXCHANGE_2013
+    get_folder_allowed = False
 
-    LOCALIZED_NAMES = {
-        "da_DK": ("Kontaktpersoner",),
-        "de_DE": ("Kontakte",),
-        "en_US": ("Contacts",),
-        "es_ES": ("Contactos",),
-        "fr_CA": ("Contacts",),
-        "nl_NL": ("Contactpersonen",),
-        "ru_RU": ("Контакты",),
-        "sv_SE": ("Kontakter",),
-        "zh_CN": ("联系人",),
-    }
+
+class AllContacts(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "allcontacts"
+    CONTAINER_CLASS = "IPF.Note"
 
 
-class WellknownFolder(Folder, metaclass=EWSMeta):
-    """Base class to use until we have a more specific folder implementation for this folder."""
+class AllItems(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "allitems"
+    CONTAINER_CLASS = "IPF"
 
-    supported_item_models = ITEM_CLASSES
 
+class AllCategorizedItems(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "allcategorizeditems"
+    CONTAINER_CLASS = "IPF.Note"
 
-class AdminAuditLogs(WellknownFolder):
-    DISTINGUISHED_FOLDER_ID = "adminauditlogs"
-    supported_from = EXCHANGE_2013
-    get_folder_allowed = False
+
+class AllPersonMetadata(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "allpersonmetadata"
+    CONTAINER_CLASS = "IPF.Note"
 
 
 class ArchiveDeletedItems(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "archivedeleteditems"
     supported_from = EXCHANGE_2010_SP1
 
 
@@ -260,14 +266,23 @@
 
 
 class ArchiveRecoverableItemsVersions(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "archiverecoverableitemsversions"
     supported_from = EXCHANGE_2010_SP1
 
 
+class Companies(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "companycontacts"
+    CONTAINER_CLASS = "IPF.Contact.Company"
+    supported_item_models = (Contact, DistributionList)
+    LOCALIZED_NAMES = {
+        "da_DK": ("Firmaer",),
+    }
+
+
 class Conflicts(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "conflicts"
     supported_from = EXCHANGE_2013
 
 
 class ConversationHistory(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "conversationhistory"
@@ -275,26 +290,50 @@
 
 
 class Directory(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "directory"
     supported_from = EXCHANGE_2013_SP1
 
 
+class DlpPolicyEvaluation(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "dlppolicyevaluation"
+    CONTAINER_CLASS = "IPF.StoreItem.DlpPolicyEvaluation"
+
+
 class Favorites(WellknownFolder):
     CONTAINER_CLASS = "IPF.Note"
     DISTINGUISHED_FOLDER_ID = "favorites"
     supported_from = EXCHANGE_2013
 
 
+class FolderMemberships(Folder):
+    CONTAINER_CLASS = "IPF.Task"
+    LOCALIZED_NAMES = {
+        None: ("Folder Memberships",),
+    }
+
+
+class FromFavoriteSenders(WellknownFolder):
+    CONTAINER_CLASS = "IPF.Note"
+    DISTINGUISHED_FOLDER_ID = "fromfavoritesenders"
+    LOCALIZED_NAMES = {
+        "da_DK": ("Personer jeg kender",),
+    }
+
+
 class IMContactList(WellknownFolder):
     CONTAINER_CLASS = "IPF.Contact.MOC.ImContactList"
     DISTINGUISHED_FOLDER_ID = "imcontactlist"
     supported_from = EXCHANGE_2013
 
 
+class Inference(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "inference"
+
+
 class Journal(WellknownFolder):
     CONTAINER_CLASS = "IPF.Journal"
     DISTINGUISHED_FOLDER_ID = "journal"
 
 
 class LocalFailures(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "localfailures"
@@ -322,31 +361,76 @@
     CONTAINER_CLASS = "IPF.StickyNote"
     DISTINGUISHED_FOLDER_ID = "notes"
     LOCALIZED_NAMES = {
         "da_DK": ("Noter",),
     }
 
 
+class OneNotePagePreviews(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "onenotepagepreviews"
+
+
+class PeopleCentricConversationBuddies(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "peoplecentricconversationbuddies"
+    CONTAINER_CLASS = "IPF.Contact.PeopleCentricConversationBuddies"
+    LOCALIZED_NAMES = {
+        None: ("PeopleCentricConversation Buddies",),
+    }
+
+
 class PeopleConnect(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "peopleconnect"
     supported_from = EXCHANGE_2013
 
 
+class QedcDefaultRetention(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "qedcdefaultretention"
+
+
+class QedcLongRetention(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "qedclongretention"
+
+
+class QedcMediumRetention(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "qedcmediumretention"
+
+
+class QedcShortRetention(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "qedcshortretention"
+
+
+class QuarantinedEmail(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "quarantinedemail"
+
+
+class QuarantinedEmailDefaultCategory(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "quarantinedemaildefaultcategory"
+
+
 class QuickContacts(WellknownFolder):
     CONTAINER_CLASS = "IPF.Contact.MOC.QuickContacts"
     DISTINGUISHED_FOLDER_ID = "quickcontacts"
     supported_from = EXCHANGE_2013
 
 
-class RecipientCache(Contacts):
+class RecipientCache(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "recipientcache"
     CONTAINER_CLASS = "IPF.Contact.RecipientCache"
     supported_from = EXCHANGE_2013
+    LOCALIZED_NAMES = {
+        None: ("RecipientCache",),
+    }
+
 
-    LOCALIZED_NAMES = {}
+class RelevantContacts(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "relevantcontacts"
+    CONTAINER_CLASS = "IPF.Note"
+    LOCALIZED_NAMES = {
+        None: ("RelevantContacts",),
+    }
 
 
 class RecoverableItemsDeletions(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "recoverableitemsdeletions"
     supported_from = EXCHANGE_2010_SP1
 
 
@@ -356,403 +440,383 @@
 
 
 class RecoverableItemsRoot(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "recoverableitemsroot"
     supported_from = EXCHANGE_2010_SP1
 
 
+class RecoverableItemsSubstrateHolds(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "recoverableitemssubstrateholds"
+    supported_from = EXCHANGE_2010_SP1
+    LOCALIZED_NAMES = {
+        None: ("SubstrateHolds",),
+    }
+
+
 class RecoverableItemsVersions(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "recoverableitemsversions"
     supported_from = EXCHANGE_2010_SP1
 
 
 class SearchFolders(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "searchfolders"
 
 
 class ServerFailures(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "serverfailures"
     supported_from = EXCHANGE_2013
 
 
+class SharePointNotifications(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "sharepointnotifications"
+
+
+class ShortNotes(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "shortnotes"
+
+
 class SyncIssues(WellknownFolder):
     CONTAINER_CLASS = "IPF.Note"
     DISTINGUISHED_FOLDER_ID = "syncissues"
     supported_from = EXCHANGE_2013
 
 
+class TemporarySaves(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "temporarysaves"
+
+
 class ToDoSearch(WellknownFolder):
     CONTAINER_CLASS = "IPF.Task"
     DISTINGUISHED_FOLDER_ID = "todosearch"
     supported_from = EXCHANGE_2013
-
     LOCALIZED_NAMES = {
         None: ("To-Do Search",),
     }
 
 
+class UserCuratedContacts(WellknownFolder):
+    CONTAINER_CLASS = "IPF.Note"
+    DISTINGUISHED_FOLDER_ID = "usercuratedcontacts"
+
+
 class VoiceMail(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "voicemail"
     CONTAINER_CLASS = "IPF.Note.Microsoft.Voicemail"
     LOCALIZED_NAMES = {
         None: ("Voice Mail",),
     }
 
 
-class NonDeletableFolderMixIn:
+class NonDeletableFolder(Folder):
     """A mixin for non-wellknown folders than that are not deletable."""
 
     @property
     def is_deletable(self):
         return False
 
 
-class AllContacts(NonDeletableFolderMixIn, Contacts):
-    CONTAINER_CLASS = "IPF.Note"
-
+class ExternalContacts(NonDeletableFolder):
+    DISTINGUISHED_FOLDER_ID = None
+    CONTAINER_CLASS = "IPF.Contact"
+    supported_item_models = (Contact, DistributionList)
     LOCALIZED_NAMES = {
-        None: ("AllContacts",),
+        None: ("ExternalContacts",),
     }
 
 
-class AllItems(NonDeletableFolderMixIn, Folder):
-    CONTAINER_CLASS = "IPF"
-
+class AllTodoTasks(NonDeletableFolder):
+    DISTINGUISHED_FOLDER_ID = None
+    CONTAINER_CLASS = "IPF.Task"
+    supported_item_models = (Task,)
     LOCALIZED_NAMES = {
-        None: ("AllItems",),
+        None: ("AllTodoTasks",),
     }
 
 
-class ApplicationData(NonDeletableFolderMixIn, Folder):
+class ApplicationData(NonDeletableFolder):
     CONTAINER_CLASS = "IPM.ApplicationData"
 
 
-class Audits(NonDeletableFolderMixIn, Folder):
-    LOCALIZED_NAMES = {
-        None: ("Audits",),
-    }
+class Audits(NonDeletableFolder):
     get_folder_allowed = False
 
 
-class CalendarLogging(NonDeletableFolderMixIn, Folder):
+class CalendarLogging(NonDeletableFolder):
     LOCALIZED_NAMES = {
         None: ("Calendar Logging",),
     }
 
 
-class CommonViews(NonDeletableFolderMixIn, Folder):
+class CommonViews(NonDeletableFolder):
     DEFAULT_ITEM_TRAVERSAL_DEPTH = ASSOCIATED
     LOCALIZED_NAMES = {
         None: ("Common Views",),
     }
 
 
-class Companies(NonDeletableFolderMixIn, Contacts):
-    DISTINGUISHED_FOLDER_ID = None
-    CONTAINER_CLASS = "IPF.Contact.Company"
-    LOCALIZED_NAMES = {
-        None: ("Companies",),
-        "da_DK": ("Firmaer",),
-    }
-
-
-class ConversationSettings(NonDeletableFolderMixIn, Folder):
+class ConversationSettings(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.Configuration"
     LOCALIZED_NAMES = {
         "da_DK": ("Indstillinger for samtalehandlinger",),
     }
 
 
-class DefaultFoldersChangeHistory(NonDeletableFolderMixIn, Folder):
+class DefaultFoldersChangeHistory(NonDeletableFolder):
     CONTAINER_CLASS = "IPM.DefaultFolderHistoryItem"
-    LOCALIZED_NAMES = {
-        None: ("DefaultFoldersChangeHistory",),
-    }
 
 
-class DeferredAction(NonDeletableFolderMixIn, Folder):
+class DeferredAction(NonDeletableFolder):
     LOCALIZED_NAMES = {
         None: ("Deferred Action",),
     }
 
 
-class ExchangeSyncData(NonDeletableFolderMixIn, Folder):
-    LOCALIZED_NAMES = {
-        None: ("ExchangeSyncData",),
-    }
+class ExchangeSyncData(NonDeletableFolder):
+    pass
 
 
-class Files(NonDeletableFolderMixIn, Folder):
+class Files(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.Files"
-
     LOCALIZED_NAMES = {
         "da_DK": ("Filer",),
     }
 
 
-class FreebusyData(NonDeletableFolderMixIn, Folder):
+class FreebusyData(NonDeletableFolder):
     LOCALIZED_NAMES = {
         None: ("Freebusy Data",),
     }
 
 
-class Friends(NonDeletableFolderMixIn, Contacts):
+class Friends(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.Note"
-
+    supported_item_models = (Contact, DistributionList)
     LOCALIZED_NAMES = {
         "de_DE": ("Bekannte",),
     }
 
 
-class GALContacts(NonDeletableFolderMixIn, Contacts):
-    DISTINGUISHED_FOLDER_ID = None
+class GALContacts(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.Contact.GalContacts"
-
+    supported_item_models = (Contact, DistributionList)
     LOCALIZED_NAMES = {
         None: ("GAL Contacts",),
     }
 
 
-class GraphAnalytics(NonDeletableFolderMixIn, Folder):
+class GraphAnalytics(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.StoreItem.GraphAnalytics"
-    LOCALIZED_NAMES = {
-        None: ("GraphAnalytics",),
-    }
 
 
-class Location(NonDeletableFolderMixIn, Folder):
-    LOCALIZED_NAMES = {
-        None: ("Location",),
-    }
+class Location(NonDeletableFolder):
+    pass
 
 
-class MailboxAssociations(NonDeletableFolderMixIn, Folder):
-    LOCALIZED_NAMES = {
-        None: ("MailboxAssociations",),
-    }
+class MailboxAssociations(NonDeletableFolder):
+    pass
 
 
-class MyContactsExtended(NonDeletableFolderMixIn, Contacts):
+class MyContactsExtended(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.Note"
-    LOCALIZED_NAMES = {
-        None: ("MyContactsExtended",),
-    }
+    supported_item_models = (Contact, DistributionList)
 
 
-class OrganizationalContacts(NonDeletableFolderMixIn, Contacts):
-    DISTINGUISHED_FOLDER_ID = None
+class OrganizationalContacts(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.Contact.OrganizationalContacts"
+    supported_item_models = (Contact, DistributionList)
     LOCALIZED_NAMES = {
         None: ("Organizational Contacts",),
     }
 
 
-class ParkedMessages(NonDeletableFolderMixIn, Folder):
+class ParkedMessages(NonDeletableFolder):
     CONTAINER_CLASS = None
-    LOCALIZED_NAMES = {
-        None: ("ParkedMessages",),
-    }
 
 
-class PassThroughSearchResults(NonDeletableFolderMixIn, Folder):
+class PassThroughSearchResults(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.StoreItem.PassThroughSearchResults"
     LOCALIZED_NAMES = {
         None: ("Pass-Through Search Results",),
     }
 
 
-class PeopleCentricConversationBuddies(NonDeletableFolderMixIn, Contacts):
-    DISTINGUISHED_FOLDER_ID = None
-    CONTAINER_CLASS = "IPF.Contact.PeopleCentricConversationBuddies"
-    LOCALIZED_NAMES = {
-        None: ("PeopleCentricConversation Buddies",),
-    }
-
-
-class PdpProfileV2Secured(NonDeletableFolderMixIn, Folder):
+class PdpProfileV2Secured(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.StoreItem.PdpProfileSecured"
-    LOCALIZED_NAMES = {
-        None: ("PdpProfileV2Secured",),
-    }
 
 
-class Reminders(NonDeletableFolderMixIn, Folder):
+class Reminders(NonDeletableFolder):
     CONTAINER_CLASS = "Outlook.Reminder"
     LOCALIZED_NAMES = {
         "da_DK": ("Påmindelser",),
     }
 
 
-class RSSFeeds(NonDeletableFolderMixIn, Folder):
+class RSSFeeds(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.Note.OutlookHomepage"
     LOCALIZED_NAMES = {
         None: ("RSS Feeds",),
     }
 
 
-class Schedule(NonDeletableFolderMixIn, Folder):
-    LOCALIZED_NAMES = {
-        None: ("Schedule",),
-    }
+class Schedule(NonDeletableFolder):
+    pass
 
 
-class Sharing(NonDeletableFolderMixIn, Folder):
+class Sharing(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.Note"
-    LOCALIZED_NAMES = {
-        None: ("Sharing",),
-    }
 
 
-class Shortcuts(NonDeletableFolderMixIn, Folder):
-    LOCALIZED_NAMES = {
-        None: ("Shortcuts",),
-    }
+class Shortcuts(NonDeletableFolder):
+    pass
 
 
-class Signal(NonDeletableFolderMixIn, Folder):
+class Signal(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.StoreItem.Signal"
-    LOCALIZED_NAMES = {
-        None: ("Signal",),
-    }
 
 
-class SmsAndChatsSync(NonDeletableFolderMixIn, Folder):
+class SmsAndChatsSync(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.SmsAndChatsSync"
-    LOCALIZED_NAMES = {
-        None: ("SmsAndChatsSync",),
-    }
 
 
-class SpoolerQueue(NonDeletableFolderMixIn, Folder):
+class SpoolerQueue(NonDeletableFolder):
     LOCALIZED_NAMES = {
         None: ("Spooler Queue",),
     }
 
 
-class System(NonDeletableFolderMixIn, Folder):
-    LOCALIZED_NAMES = {
-        None: ("System",),
-    }
+class System(NonDeletableFolder):
     get_folder_allowed = False
 
 
-class System1(NonDeletableFolderMixIn, Folder):
-    LOCALIZED_NAMES = {
-        None: ("System1",),
-    }
+class System1(NonDeletableFolder):
     get_folder_allowed = False
 
 
-class TemporarySaves(NonDeletableFolderMixIn, Folder):
-    LOCALIZED_NAMES = {
-        None: ("TemporarySaves",),
-    }
-
-
-class Views(NonDeletableFolderMixIn, Folder):
-    LOCALIZED_NAMES = {
-        None: ("Views",),
-    }
+class Views(NonDeletableFolder):
+    pass
 
 
-class WorkingSet(NonDeletableFolderMixIn, Folder):
+class WorkingSet(NonDeletableFolder):
     LOCALIZED_NAMES = {
         None: ("Working Set",),
     }
 
 
-# Folders that return 'ErrorDeleteDistinguishedFolder' when we try to delete them. I can't find any official docs
-# listing these folders.
+# Folders that do not have a distinguished folder ID but return 'ErrorDeleteDistinguishedFolder' or
+# 'ErrorCannotDeleteObject' when we try to delete them. I can't find any official docs listing these folders.
 NON_DELETABLE_FOLDERS = [
-    AllContacts,
-    AllItems,
     ApplicationData,
+    AllTodoTasks,
     Audits,
     CalendarLogging,
     CommonViews,
-    Companies,
     ConversationSettings,
     DefaultFoldersChangeHistory,
     DeferredAction,
     ExchangeSyncData,
+    ExternalContacts,
     FreebusyData,
     Files,
     Friends,
     GALContacts,
     GraphAnalytics,
     Location,
     MailboxAssociations,
     MyContactsExtended,
     OrganizationalContacts,
     ParkedMessages,
     PassThroughSearchResults,
-    PeopleCentricConversationBuddies,
     PdpProfileV2Secured,
     Reminders,
     RSSFeeds,
     Schedule,
     Sharing,
     Shortcuts,
     Signal,
     SmsAndChatsSync,
     SpoolerQueue,
     System,
     System1,
-    TemporarySaves,
     Views,
     WorkingSet,
 ]
 
+# Folders that have a distinguished ID and are located in the root folder hierarchy
 WELLKNOWN_FOLDERS_IN_ROOT = [
     AdminAuditLogs,
+    AllCategorizedItems,
+    AllContacts,
+    AllItems,
+    AllPersonMetadata,
     Calendar,
+    Companies,
     Conflicts,
     Contacts,
     ConversationHistory,
     DeletedItems,
     Directory,
+    DlpPolicyEvaluation,
     Drafts,
     Favorites,
+    FromFavoriteSenders,
     IMContactList,
+    Inference,
     Inbox,
     Journal,
     JunkEmail,
     LocalFailures,
     MsgFolderRoot,
     MyContacts,
     Notes,
+    OneNotePagePreviews,
     Outbox,
+    PeopleCentricConversationBuddies,
     PeopleConnect,
+    QedcDefaultRetention,
+    QedcLongRetention,
+    QedcMediumRetention,
+    QedcShortRetention,
+    QuarantinedEmail,
+    QuarantinedEmailDefaultCategory,
     QuickContacts,
     RecipientCache,
+    RelevantContacts,
     RecoverableItemsDeletions,
     RecoverableItemsPurges,
     RecoverableItemsRoot,
+    RecoverableItemsSubstrateHolds,
     RecoverableItemsVersions,
     SearchFolders,
     SentItems,
     ServerFailures,
+    SharePointNotifications,
+    ShortNotes,
     SyncIssues,
     Tasks,
+    TemporarySaves,
     ToDoSearch,
+    UserCuratedContacts,
     VoiceMail,
 ]
 
+# Folders that have a distinguished ID and are located in the archive root folder hierarchy
 WELLKNOWN_FOLDERS_IN_ARCHIVE_ROOT = [
     ArchiveDeletedItems,
     ArchiveInbox,
     ArchiveMsgFolderRoot,
     ArchiveRecoverableItemsDeletions,
     ArchiveRecoverableItemsPurges,
     ArchiveRecoverableItemsRoot,
     ArchiveRecoverableItemsVersions,
 ]
 
+# Folders that do not have a distinguished ID but have their own container class
 MISC_FOLDERS = [
     CrawlerData,
-    DlpPolicyEvaluation,
+    EventCheckPoints,
+    FolderMemberships,
     FreeBusyCache,
     RecoveryPoints,
     SwssItems,
     SkypeTeamsMessages,
     Birthdays,
 ]
```

### Comparing `exchangelib-5.2.0/exchangelib/folders/queryset.py` & `exchangelib-5.2.1/exchangelib/folders/queryset.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/folders/roots.py` & `exchangelib-5.2.1/exchangelib/folders/roots.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             for f in self._folders_map.values():
                 # Require exact class, to not match subclasses, e.g. RecipientCache instead of Contacts
                 if f.__class__ == folder_cls and f.is_distinguished:
                     log.debug("Found cached distinguished %s folder", folder_cls)
                     return f
         try:
             log.debug("Requesting distinguished %s folder explicitly", folder_cls)
-            return folder_cls.get_distinguished(root=self)
+            return folder_cls.get_distinguished(account=self.account)
         except ErrorAccessDenied:
             # Maybe we just don't have GetFolder access? Try FindItem instead
             log.debug("Testing default %s folder with FindItem", folder_cls)
             fld = folder_cls(
                 root=self,
                 _distinguished_id=DistinguishedFolderId(
                     id=folder_cls.DISTINGUISHED_FOLDER_ID,
```

### Comparing `exchangelib-5.2.0/exchangelib/indexed_properties.py` & `exchangelib-5.2.1/exchangelib/indexed_properties.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/items/__init__.py` & `exchangelib-5.2.1/exchangelib/items/__init__.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/items/base.py` & `exchangelib-5.2.1/exchangelib/items/base.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/items/calendar_item.py` & `exchangelib-5.2.1/exchangelib/items/calendar_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/items/contact.py` & `exchangelib-5.2.1/exchangelib/items/contact.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/items/item.py` & `exchangelib-5.2.1/exchangelib/items/item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/items/message.py` & `exchangelib-5.2.1/exchangelib/items/message.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/items/post.py` & `exchangelib-5.2.1/exchangelib/items/post.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/items/task.py` & `exchangelib-5.2.1/exchangelib/items/task.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/properties.py` & `exchangelib-5.2.1/exchangelib/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     ErrorNonExistentMailbox,
     ErrorOrganizationNotFederated,
     ErrorServerBusy,
     InvalidTypeError,
 )
 from .fields import (
     WEEKDAY_NAMES,
+    AddressListField,
     AssociatedCalendarItemIdField,
     Base64Field,
     BooleanField,
     CharField,
     CharListField,
     Choice,
     ChoiceField,
@@ -33,14 +34,15 @@
     EnumListField,
     EWSElementField,
     EWSElementListField,
     ExtendedPropertyField,
     Field,
     FieldPath,
     FlaggedForActionField,
+    FolderActionField,
     FreeBusyStatusField,
     GenericEventListField,
     IdElementField,
     IdField,
     ImportanceField,
     IntegerField,
     InvalidField,
@@ -745,14 +747,18 @@
 class DistinguishedFolderId(FolderId):
     """MSDN: https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/distinguishedfolderid"""
 
     ELEMENT_NAME = "DistinguishedFolderId"
 
     mailbox = MailboxField()
 
+    @classmethod
+    def from_xml(cls, elem, account):
+        return cls(id=elem.text or None)
+
     def clean(self, version=None):
         from .folders import PublicFoldersRoot
 
         super().clean(version=version)
         if self.id == PublicFoldersRoot.DISTINGUISHED_FOLDER_ID:
             # Avoid "ErrorInvalidOperation: It is not valid to specify a mailbox with the public folder root" from EWS
             self.mailbox = None
@@ -814,15 +820,15 @@
     occurrence = IntegerField(field_uri="DayOrder", is_required=True)  # n'th occurrence of weekday in iso_month
     iso_month = IntegerField(field_uri="Month", is_required=True)
     weekday = EnumField(field_uri="DayOfWeek", enum=WEEKDAY_NAMES, is_required=True)
     # 'Year' is not implemented yet
 
     @classmethod
     def from_xml(cls, elem, account):
-        res = super().from_xml(elem, account)
+        res = super().from_xml(elem=elem, account=account)
         # Some parts of EWS use '5' to mean 'last occurrence in month', others use '-1'. Let's settle on '5' because
         # only '5' is accepted in requests.
         if res.occurrence == -1:
             res.occurrence = 5
         return res
 
     def clean(self, version=None):
@@ -1861,15 +1867,15 @@
     month = IntegerField(field_uri="Month")
     # Valid ISO 8601 weekday, as a number in range 1 -> 7 (1 being Monday)
     day_of_week = EnumField(field_uri="DayOfWeek", enum=WEEKDAY_NAMES)
     occurrence = IntegerField(field_uri="Occurrence")
 
     @classmethod
     def from_xml(cls, elem, account):
-        res = super().from_xml(elem, account)
+        res = super().from_xml(elem=elem, account=account)
         # See TimeZoneTransition.from_xml()
         if res.occurrence == -1:
             res.occurrence = 5
         return res
 
 
 class RecurringDateTransition(BaseTransition):
@@ -1913,18 +1919,14 @@
     id = CharField(field_uri="Id", is_attribute=True)
     name = CharField(field_uri="Name", is_attribute=True)
 
     periods = EWSElementListField(field_uri="Periods", value_cls=Period)
     transitions_groups = EWSElementListField(field_uri="TransitionsGroups", value_cls=TransitionsGroup)
     transitions = TransitionListField(field_uri="Transitions", value_cls=BaseTransition)
 
-    @classmethod
-    def from_xml(cls, elem, account):
-        return super().from_xml(elem, account)
-
     def _get_standard_period(self, transitions_group):
         # Find the first standard period referenced from transitions_group
         standard_periods_map = {p.id: p for p in self.periods if p.name == "Standard"}
         for transition in transitions_group.transitions:
             try:
                 return standard_periods_map[transition.to]
             except KeyError:
@@ -2218,64 +2220,94 @@
     NAMESPACE = TNS
 
 
 class CopyToFolder(EWSElement):
     """MSDN: https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/copytofolder"""
 
     ELEMENT_NAME = "CopyToFolder"
-    NAMESPACE = MNS
 
-    folder_id = EWSElementField(value_cls=FolderId, field_uri="FolderId")
-    distinguished_folder_id = EWSElementField(value_cls=DistinguishedFolderId, field_uri="DistinguishedFolderId")
+    folder_id = EWSElementField(value_cls=FolderId)
+    distinguished_folder_id = EWSElementField(value_cls=DistinguishedFolderId)
 
 
 class MoveToFolder(CopyToFolder):
     """MSDN: https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/movetofolder"""
 
     ELEMENT_NAME = "MoveToFolder"
 
 
 class Actions(EWSElement):
     """MSDN: https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/actions"""
 
     ELEMENT_NAME = "Actions"
-    NAMESPACE = TNS
 
     assign_categories = CharListField(field_uri="AssignCategories")
-    copy_to_folder = EWSElementField(value_cls=CopyToFolder, field_uri="CopyToFolder")
+    copy_to_folder = FolderActionField(value_cls=CopyToFolder)
     delete = BooleanField(field_uri="Delete")
-    forward_as_attachment_to_recipients = EWSElementField(
-        value_cls=Mailbox, field_uri="ForwardAsAttachmentToRecipients"
-    )
-    forward_to_recipients = EWSElementField(value_cls=Mailbox, field_uri="ForwardToRecipients")
+    forward_as_attachment_to_recipients = AddressListField(field_uri="ForwardAsAttachmentToRecipients")
+    forward_to_recipients = AddressListField(field_uri="ForwardToRecipients")
     mark_importance = ImportanceField(field_uri="MarkImportance")
     mark_as_read = BooleanField(field_uri="MarkAsRead")
-    move_to_folder = EWSElementField(value_cls=MoveToFolder, field_uri="MoveToFolder")
+    move_to_folder = FolderActionField(value_cls=MoveToFolder)
     permanent_delete = BooleanField(field_uri="PermanentDelete")
-    redirect_to_recipients = EWSElementField(value_cls=Mailbox, field_uri="RedirectToRecipients")
-    send_sms_alert_to_recipients = EWSElementField(value_cls=Mailbox, field_uri="SendSMSAlertToRecipients")
+    redirect_to_recipients = AddressListField(field_uri="RedirectToRecipients")
+    send_sms_alert_to_recipients = AddressListField(field_uri="SendSMSAlertToRecipients")
     server_reply_with_message = EWSElementField(value_cls=ItemId, field_uri="ServerReplyWithMessage")
     stop_processing_rules = BooleanField(field_uri="StopProcessingRules")
 
 
 class Rule(EWSElement):
     """MSDN: https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/rule-ruletype"""
 
+    def __init__(self, **kwargs):
+        """Pick out optional 'account' kwarg, and pass the rest to the parent class.
+
+        :param kwargs:
+            'account' is optional but allows calling 'send()' and 'delete()'
+        """
+        from .account import Account
+
+        self.account = kwargs.pop("account", None)
+        if self.account is not None and not isinstance(self.account, Account):
+            raise InvalidTypeError("account", self.account, Account)
+        super().__init__(**kwargs)
+
+    __slots__ = ("account",)
+
     ELEMENT_NAME = "Rule"
-    NAMESPACE = TNS
 
     id = CharField(field_uri="RuleId")
-    display_name = CharField(field_uri="DisplayName")
-    priority = IntegerField(field_uri="Priority")
+    display_name = CharField(field_uri="DisplayName", is_required=True)
+    priority = IntegerField(field_uri="Priority", is_required=True)
     is_enabled = BooleanField(field_uri="IsEnabled")
     is_not_supported = BooleanField(field_uri="IsNotSupported")
     is_in_error = BooleanField(field_uri="IsInError")
     conditions = EWSElementField(value_cls=Conditions)
     exceptions = EWSElementField(value_cls=Exceptions)
-    actions = EWSElementField(value_cls=Actions)
+    actions = EWSElementField(value_cls=Actions, is_required=True)
+
+    @classmethod
+    def from_xml(cls, elem, account):
+        res = super().from_xml(elem=elem, account=account)
+        res.account = account
+        return res
+
+    def save(self):
+        if self.id is None:
+            self.account.create_rule(self)
+        else:
+            self.account.set_rule(self)
+        return self
+
+    def delete(self):
+        if self.is_enabled is False:
+            # Cannot delete a disabled rule - server throws 'ErrorItemNotFound'
+            self.is_enabled = True
+            self.save()
+        self.account.delete_rule(self)
 
 
 class InboxRules(EWSElement):
     """MSDN: https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/inboxrules"""
 
     ELEMENT_NAME = "InboxRules"
     NAMESPACE = MNS
@@ -2283,33 +2315,30 @@
     rule = EWSElementListField(value_cls=Rule)
 
 
 class CreateRuleOperation(EWSElement):
     """MSDN: https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/createruleoperation"""
 
     ELEMENT_NAME = "CreateRuleOperation"
-    NAMESPACE = TNS
 
     rule = EWSElementField(value_cls=Rule)
 
 
 class SetRuleOperation(EWSElement):
     """MSDN: https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/setruleoperation"""
 
     ELEMENT_NAME = "SetRuleOperation"
-    NAMESPACE = TNS
 
     rule = EWSElementField(value_cls=Rule)
 
 
 class DeleteRuleOperation(EWSElement):
     """MSDN: https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/deleteruleoperation"""
 
     ELEMENT_NAME = "DeleteRuleOperation"
-    NAMESPACE = TNS
 
     id = CharField(field_uri="RuleId")
 
 
 class Operations(EWSElement):
     """MSDN: https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/operations"""
```

### Comparing `exchangelib-5.2.0/exchangelib/protocol.py` & `exchangelib-5.2.1/exchangelib/protocol.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/queryset.py` & `exchangelib-5.2.1/exchangelib/queryset.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,15 +525,18 @@
         else:
             new_qs = self.filter(*args, **kwargs)
             items = list(new_qs.__iter__())
         if not items:
             raise DoesNotExist()
         if len(items) != 1:
             raise MultipleObjectsReturned()
-        return items[0]
+        item = items[0]
+        if isinstance(item, Exception):
+            raise item
+        return item
 
     def count(self, page_size=1000):
         """Get the query count, with as little effort as possible
 
         :param page_size: The number of items to fetch per request. We're only fetching the IDs, so keep it high.
         (Default value = 1000)
         """
```

### Comparing `exchangelib-5.2.0/exchangelib/recurrence.py` & `exchangelib-5.2.1/exchangelib/recurrence.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/restriction.py` & `exchangelib-5.2.1/exchangelib/restriction.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/__init__.py` & `exchangelib-5.2.1/exchangelib/services/__init__.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/archive_item.py` & `exchangelib-5.2.1/exchangelib/services/archive_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/common.py` & `exchangelib-5.2.1/exchangelib/services/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -971,15 +971,14 @@
 
 
 def parse_folder_elem(elem, folder, account):
     if isinstance(folder, RootOfHierarchy):
         f = folder.from_xml(elem=elem, account=folder.account)
     elif isinstance(folder, Folder):
         f = folder.from_xml_with_root(elem=elem, root=folder.root)
-        f._distinguished_id = folder._distinguished_id
     elif isinstance(folder, DistinguishedFolderId):
         # We don't know the root or even account, but we need to attach the folder to something if we want to make
         # future requests with this folder. Use 'account' but make sure to always use the distinguished folder ID going
         # forward, instead of referencing anything connected to 'account'.
         roots = (Root, ArchiveRoot, PublicFoldersRoot)
         for cls in roots + tuple(chain(*(r.WELLKNOWN_FOLDERS for r in roots))):
             if cls.DISTINGUISHED_FOLDER_ID == folder.id:
@@ -987,12 +986,11 @@
                 break
         else:
             raise ValueError(f"Unknown distinguished folder ID: {folder.id}")
         if folder_cls in roots:
             f = folder_cls.from_xml(elem=elem, account=account)
         else:
             f = folder_cls.from_xml_with_root(elem=elem, root=account.root)
-        f._distinguished_id = folder
     else:
         # 'folder' is a generic FolderId instance. We don't know the root so assume account.root.
         f = Folder.from_xml_with_root(elem=elem, root=account.root)
     return f
```

### Comparing `exchangelib-5.2.0/exchangelib/services/convert_id.py` & `exchangelib-5.2.1/exchangelib/services/convert_id.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/create_attachment.py` & `exchangelib-5.2.1/exchangelib/services/create_attachment.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/create_folder.py` & `exchangelib-5.2.1/exchangelib/services/create_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/create_item.py` & `exchangelib-5.2.1/exchangelib/services/create_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/create_user_configuration.py` & `exchangelib-5.2.1/exchangelib/services/create_user_configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/delete_attachment.py` & `exchangelib-5.2.1/exchangelib/services/delete_attachment.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/delete_folder.py` & `exchangelib-5.2.1/exchangelib/services/delete_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/delete_item.py` & `exchangelib-5.2.1/exchangelib/services/delete_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/delete_user_configuration.py` & `exchangelib-5.2.1/exchangelib/services/delete_user_configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/empty_folder.py` & `exchangelib-5.2.1/exchangelib/services/empty_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/expand_dl.py` & `exchangelib-5.2.1/exchangelib/services/expand_dl.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/export_items.py` & `exchangelib-5.2.1/exchangelib/services/export_items.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/find_folder.py` & `exchangelib-5.2.1/exchangelib/services/find_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/find_item.py` & `exchangelib-5.2.1/exchangelib/services/find_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/find_people.py` & `exchangelib-5.2.1/exchangelib/services/find_people.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_attachment.py` & `exchangelib-5.2.1/exchangelib/services/get_attachment.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_delegate.py` & `exchangelib-5.2.1/exchangelib/services/get_delegate.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_events.py` & `exchangelib-5.2.1/exchangelib/services/get_events.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_folder.py` & `exchangelib-5.2.1/exchangelib/services/get_folder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,29 @@
-from ..errors import ErrorFolderNotFound, ErrorInvalidOperation, ErrorNoPublicFolderReplicaAvailable
+from ..errors import (
+    ErrorAccessDenied,
+    ErrorFolderNotFound,
+    ErrorInvalidOperation,
+    ErrorItemNotFound,
+    ErrorNoPublicFolderReplicaAvailable,
+)
 from ..util import MNS, create_element
 from .common import EWSAccountService, folder_ids_element, parse_folder_elem, shape_element
 
 
 class GetFolder(EWSAccountService):
     """MSDN: https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/getfolder-operation"""
 
     SERVICE_NAME = "GetFolder"
     element_container_name = f"{{{MNS}}}Folders"
     ERRORS_TO_CATCH_IN_RESPONSE = EWSAccountService.ERRORS_TO_CATCH_IN_RESPONSE + (
+        ErrorAccessDenied,
         ErrorFolderNotFound,
         ErrorNoPublicFolderReplicaAvailable,
         ErrorInvalidOperation,
+        ErrorItemNotFound,
     )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.folders = []  # A hack to communicate parsing args to _elems_to_objs()
 
     def call(self, folders, additional_fields, shape):
```

### Comparing `exchangelib-5.2.0/exchangelib/services/get_item.py` & `exchangelib-5.2.1/exchangelib/services/get_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_mail_tips.py` & `exchangelib-5.2.1/exchangelib/services/get_mail_tips.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_persona.py` & `exchangelib-5.2.1/exchangelib/services/get_persona.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_room_lists.py` & `exchangelib-5.2.1/exchangelib/services/get_room_lists.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_rooms.py` & `exchangelib-5.2.1/exchangelib/services/get_rooms.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_searchable_mailboxes.py` & `exchangelib-5.2.1/exchangelib/services/get_searchable_mailboxes.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_server_time_zones.py` & `exchangelib-5.2.1/exchangelib/services/get_server_time_zones.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_streaming_events.py` & `exchangelib-5.2.1/exchangelib/services/get_streaming_events.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_user_availability.py` & `exchangelib-5.2.1/exchangelib/services/get_user_availability.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_user_configuration.py` & `exchangelib-5.2.1/exchangelib/services/get_user_configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_user_oof_settings.py` & `exchangelib-5.2.1/exchangelib/services/get_user_oof_settings.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/get_user_settings.py` & `exchangelib-5.2.1/exchangelib/services/get_user_settings.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/inbox_rules.py` & `exchangelib-5.2.1/exchangelib/services/inbox_rules.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from typing import Any, Generator, Optional, Union
 
 from ..errors import ErrorInvalidOperation
 from ..properties import CreateRuleOperation, DeleteRuleOperation, InboxRules, Operations, Rule, SetRuleOperation
 from ..util import MNS, add_xml_child, create_element, get_xml_attr, set_xml_value
-from ..version import EXCHANGE_2010
 from .common import EWSAccountService
 
 
 class GetInboxRules(EWSAccountService):
     """
     MSDN: https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/getinboxrules-operation
 
     The GetInboxRules operation uses Exchange Web Services to retrieve Inbox rules in the identified user's mailbox.
     """
 
     SERVICE_NAME = "GetInboxRules"
-    supported_from = EXCHANGE_2010
     element_container_name = InboxRules.response_tag()
     ERRORS_TO_CATCH_IN_RESPONSE = EWSAccountService.ERRORS_TO_CATCH_IN_RESPONSE + (ErrorInvalidOperation,)
 
     def call(self, mailbox: Optional[str] = None) -> Generator[Union[Rule, Exception, None], Any, None]:
         if not mailbox:
             mailbox = self.account.primary_smtp_address
         payload = self.get_payload(mailbox=mailbox)
@@ -55,67 +53,52 @@
     else. EWS deletes this rule FAI message by default, based on the expectation that Outlook will recreate it.
     However, Outlook can't recreate rules that don't also exist as an extended rule, and client-side send rules don't
     exist as extended rules. As a result, these rules are lost. We suggest you consider this when designing your
     solution.
     """
 
     SERVICE_NAME = "UpdateInboxRules"
-    supported_from = EXCHANGE_2010
     ERRORS_TO_CATCH_IN_RESPONSE = EWSAccountService.ERRORS_TO_CATCH_IN_RESPONSE + (ErrorInvalidOperation,)
 
-
-class CreateInboxRule(UpdateInboxRules):
-    """
-    MSDN:
-    https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/updateinboxrules-operation#updateinboxrules-create-rule-request-example
-    """
-
     def call(self, rule: Rule, remove_outlook_rule_blob: bool = True):
         payload = self.get_payload(rule=rule, remove_outlook_rule_blob=remove_outlook_rule_blob)
         return self._get_elements(payload=payload)
 
+    def _get_operation(self, rule):
+        raise NotImplementedError()
+
     def get_payload(self, rule: Rule, remove_outlook_rule_blob: bool = True):
         payload = create_element(f"m:{self.SERVICE_NAME}")
         add_xml_child(payload, "m:RemoveOutlookRuleBlob", remove_outlook_rule_blob)
-        operations = Operations(create_rule_operation=CreateRuleOperation(rule=rule))
+        operations = self._get_operation(rule)
         set_xml_value(payload, operations, version=self.account.version)
         return payload
 
 
+class CreateInboxRule(UpdateInboxRules):
+    """
+    MSDN:
+    https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/updateinboxrules-operation#updateinboxrules-create-rule-request-example
+    """
+
+    def _get_operation(self, rule):
+        return Operations(create_rule_operation=CreateRuleOperation(rule=rule))
+
+
 class SetInboxRule(UpdateInboxRules):
     """
     MSDN:
     https://learn.microsoft.com/en-us/exchange/client-developer/web-service-reference/updateinboxrules-operation#updateinboxrules-set-rule-request-example
     """
 
-    def call(self, rule: Rule, remove_outlook_rule_blob: bool = True):
-        payload = self.get_payload(rule=rule, remove_outlook_rule_blob=remove_outlook_rule_blob)
-        return self._get_elements(payload=payload)
-
-    def get_payload(self, rule: Rule, remove_outlook_rule_blob: bool = True):
-        if not rule.id:
-            raise ValueError("Rule must have an ID")
-        payload = create_element(f"m:{self.SERVICE_NAME}")
-        add_xml_child(payload, "m:RemoveOutlookRuleBlob", remove_outlook_rule_blob)
-        operations = Operations(set_rule_operation=SetRuleOperation(rule=rule))
-        set_xml_value(payload, operations, version=self.account.version)
-        return payload
+    def _get_operation(self, rule):
+        return Operations(set_rule_operation=SetRuleOperation(rule=rule))
 
 
 class DeleteInboxRule(UpdateInboxRules):
     """
     MSDN:
     https://learn.microsoft.com/en-us/exchange/client-developer/web-service-reference/updateinboxrules-operation#updateinboxrules-delete-rule-request-example
     """
 
-    def call(self, rule: Rule, remove_outlook_rule_blob: bool = True):
-        payload = self.get_payload(rule=rule, remove_outlook_rule_blob=remove_outlook_rule_blob)
-        return self._get_elements(payload=payload)
-
-    def get_payload(self, rule: Rule, remove_outlook_rule_blob: bool = True):
-        if not rule.id:
-            raise ValueError("Rule must have an ID")
-        payload = create_element(f"m:{self.SERVICE_NAME}")
-        add_xml_child(payload, "m:RemoveOutlookRuleBlob", remove_outlook_rule_blob)
-        operations = Operations(delete_rule_operation=DeleteRuleOperation(id=rule.id))
-        set_xml_value(payload, operations, version=self.account.version)
-        return payload
+    def _get_operation(self, rule):
+        return Operations(delete_rule_operation=DeleteRuleOperation(id=rule.id))
```

### Comparing `exchangelib-5.2.0/exchangelib/services/mark_as_junk.py` & `exchangelib-5.2.1/exchangelib/services/mark_as_junk.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/move_folder.py` & `exchangelib-5.2.1/exchangelib/services/move_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/move_item.py` & `exchangelib-5.2.1/exchangelib/services/move_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/resolve_names.py` & `exchangelib-5.2.1/exchangelib/services/resolve_names.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/send_item.py` & `exchangelib-5.2.1/exchangelib/services/send_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/send_notification.py` & `exchangelib-5.2.1/exchangelib/services/send_notification.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/set_user_oof_settings.py` & `exchangelib-5.2.1/exchangelib/services/set_user_oof_settings.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/subscribe.py` & `exchangelib-5.2.1/exchangelib/services/subscribe.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/sync_folder_hierarchy.py` & `exchangelib-5.2.1/exchangelib/services/sync_folder_hierarchy.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/sync_folder_items.py` & `exchangelib-5.2.1/exchangelib/services/sync_folder_items.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/unsubscribe.py` & `exchangelib-5.2.1/exchangelib/services/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/update_folder.py` & `exchangelib-5.2.1/exchangelib/services/update_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/update_item.py` & `exchangelib-5.2.1/exchangelib/services/update_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/update_user_configuration.py` & `exchangelib-5.2.1/exchangelib/services/update_user_configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/services/upload_items.py` & `exchangelib-5.2.1/exchangelib/services/upload_items.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/settings.py` & `exchangelib-5.2.1/exchangelib/settings.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/transport.py` & `exchangelib-5.2.1/exchangelib/transport.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/util.py` & `exchangelib-5.2.1/exchangelib/util.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/version.py` & `exchangelib-5.2.1/exchangelib/version.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib/winzone.py` & `exchangelib-5.2.1/exchangelib/winzone.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/exchangelib.egg-info/PKG-INFO` & `exchangelib-5.2.1/exchangelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchangelib
-Version: 5.2.0
+Version: 5.2.1
 Summary: Client for Microsoft Exchange Web Services (EWS)
 Author-email: Erik Cederstrand <erik@cederstrand.dk>
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/ecederstrand/exchangelib
 Project-URL: Issues, https://github.com/ecederstrand/exchangelib/issues
 Project-URL: Documentation, https://ecederstrand.github.io/exchangelib/
 Project-URL: Repository, https://github.com/ecederstrand/exchangelib.git
```

### Comparing `exchangelib-5.2.0/exchangelib.egg-info/SOURCES.txt` & `exchangelib-5.2.1/exchangelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exchangelib-5.2.0/pyproject.toml` & `exchangelib-5.2.1/pyproject.toml`

 * *Files identical despite different names*

