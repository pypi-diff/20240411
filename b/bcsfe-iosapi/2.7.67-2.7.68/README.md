# Comparing `tmp/bcsfe-iosapi-2.7.67.tar.gz` & `tmp/bcsfe-iosapi-2.7.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcsfe-iosapi-2.7.67.tar", last modified: Fri Mar 22 01:00:47 2024, max compression
+gzip compressed data, was "bcsfe-iosapi-2.7.68.tar", last modified: Thu Apr 11 02:58:34 2024, max compression
```

## Comparing `bcsfe-iosapi-2.7.67.tar` & `bcsfe-iosapi-2.7.68.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2024-03-22 01:00:47.714522 bcsfe-iosapi-2.7.67/
--rw-r--r--   0 hayun      (502) staff       (20)      242 2024-03-22 01:00:47.714771 bcsfe-iosapi-2.7.67/PKG-INFO
--rw-rw----   0 hayun      (502) staff       (20)       38 2024-03-22 01:00:47.716787 bcsfe-iosapi-2.7.67/setup.cfg
--rw-rw----   0 hayun      (502) staff       (20)      763 2024-03-22 01:00:42.000000 bcsfe-iosapi-2.7.67/setup.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2024-03-22 01:00:47.493394 bcsfe-iosapi-2.7.67/src/
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2024-03-22 01:00:47.510431 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/
--rw-rw----   0 hayun      (502) staff       (20)      281 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/__init__.py
--rw-rw----   0 hayun      (502) staff       (20)     9869 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/__main__.py
--rw-rw----   0 hayun      (502) staff       (20)    10151 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/adb_handler.py
--rw-rw----   0 hayun      (502) staff       (20)    15039 2023-05-20 14:53:44.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/config_manager.py
--rw-rw----   0 hayun      (502) staff       (20)     1501 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/csv_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2024-03-22 01:00:47.511013 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/
--rw-rw----   0 hayun      (502) staff       (20)       67 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/__init__.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2024-03-22 01:00:47.519742 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/
--rw-rw----   0 hayun      (502) staff       (20)      122 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/__init__.py
--rw-rw----   0 hayun      (502) staff       (20)     8734 2023-05-26 02:04:50.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/basic_items.py
--rw-rw----   0 hayun      (502) staff       (20)     1490 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/catfruit.py
--rw-rw----   0 hayun      (502) staff       (20)     1931 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/catseyes.py
--rw-rw----   0 hayun      (502) staff       (20)     1647 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/ototo_base_mats.py
--rw-rw----   0 hayun      (502) staff       (20)     3984 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/talent_orbs.py
--rw-rw----   0 hayun      (502) staff       (20)    16400 2023-07-17 01:03:54.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/talent_orbs_new.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2024-03-22 01:00:47.605581 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/
--rw-rw----   0 hayun      (502) staff       (20)      179 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/__init__.py
--rw-rw----   0 hayun      (502) staff       (20)     8978 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/cat_helper.py
--rw-rw----   0 hayun      (502) staff       (20)    11125 2023-08-17 04:30:30.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/cat_id_selector.py
--rw-rw----   0 hayun      (502) staff       (20)     3096 2023-08-16 04:12:21.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/chara_drop.py
--rw-rw----   0 hayun      (502) staff       (20)     1068 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/clear_cat_guide.py
--rw-rw----   0 hayun      (502) staff       (20)     2844 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/evolve_cats.py
--rw-rw----   0 hayun      (502) staff       (20)     1260 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/get_remove_cats.py
--rw-rw----   0 hayun      (502) staff       (20)     7936 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/talents.py
--rw-rw----   0 hayun      (502) staff       (20)     1904 2023-07-17 00:19:00.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/upgrade_blue.py
--rw-rw----   0 hayun      (502) staff       (20)     3507 2023-03-28 04:18:30.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/upgrade_cats.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2024-03-22 01:00:47.624334 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/gamototo/
--rw-rw----   0 hayun      (502) staff       (20)       66 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/gamototo/__init__.py
--rw-rw----   0 hayun      (502) staff       (20)      309 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/gamototo/fix_gamatoto.py
--rw-rw----   0 hayun      (502) staff       (20)     2659 2023-05-26 07:00:35.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/gamototo/gamatoto_xp.py
--rw-rw----   0 hayun      (502) staff       (20)     3418 2023-05-31 04:36:47.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/gamototo/helpers.py
--rw-rw----   0 hayun      (502) staff       (20)     4137 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/gamototo/ototo_cat_cannon.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2024-03-22 01:00:47.679365 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/
--rw-rw----   0 hayun      (502) staff       (20)      313 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/__init__.py
--rw-rw----   0 hayun      (502) staff       (20)     1024 2023-03-28 13:41:31.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/aku.py
--rw-rw----   0 hayun      (502) staff       (20)      491 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/allow_filibuster_clearing.py
--rw-rw----   0 hayun      (502) staff       (20)      790 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/behemoth_culling.py
--rw-rw----   0 hayun      (502) staff       (20)      646 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/clear_tutorial.py
--rw-rw----   0 hayun      (502) staff       (20)     1121 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/enigma_stages.py
--rw-rw----   0 hayun      (502) staff       (20)     5924 2023-03-28 13:39:14.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/event_stages.py
--rw-rw----   0 hayun      (502) staff       (20)     1873 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/gauntlet.py
--rw-rw----   0 hayun      (502) staff       (20)     1032 2023-07-20 00:35:37.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/itf_timed_scores.py
--rw-rw----   0 hayun      (502) staff       (20)     1469 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/legend_quest.py
--rw-rw----   0 hayun      (502) staff       (20)     4382 2023-03-31 01:13:58.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/main_story.py
--rw-rw----   0 hayun      (502) staff       (20)     2100 2024-02-03 01:20:25.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/outbreaks.py
--rw-rw----   0 hayun      (502) staff       (20)     2824 2023-03-31 07:47:07.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/story_level_id_selector.py
--rw-rw----   0 hayun      (502) staff       (20)     1175 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/towers.py
--rw-rw----   0 hayun      (502) staff       (20)     8909 2023-03-31 02:09:48.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/treasures.py
--rw-rw----   0 hayun      (502) staff       (20)      868 2023-03-28 13:37:22.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/uncanny.py
--rw-rw----   0 hayun      (502) staff       (20)      784 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/unlock_aku_realm.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2024-03-22 01:00:47.698858 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/
--rw-rw----   0 hayun      (502) staff       (20)      276 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/__init__.py
--rw-rw----   0 hayun      (502) staff       (20)     3771 2024-02-03 01:35:41.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/cat_shrine.py
--rw-rw----   0 hayun      (502) staff       (20)     1093 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/claim_user_rank_rewards.py
--rw-rw----   0 hayun      (502) staff       (20)     1054 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/create_new_account.py
--rw-rw----   0 hayun      (502) staff       (20)     2171 2023-03-28 13:43:08.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/fix_elsewhere.py
--rw-rw----   0 hayun      (502) staff       (20)      659 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/fix_time_issues.py
--rw-rw----   0 hayun      (502) staff       (20)     3183 2023-08-17 02:51:45.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/get_gold_pass.py
--rw-rw----   0 hayun      (502) staff       (20)     7138 2023-06-11 23:05:06.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/meow_medals.py
--rw-rw----   0 hayun      (502) staff       (20)     4354 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/missions.py
--rw-rw----   0 hayun      (502) staff       (20)      975 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/play_time.py
--rw-rw----   0 hayun      (502) staff       (20)     4568 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/scheme_item.py
--rw-rw----   0 hayun      (502) staff       (20)     1612 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/trade_progress.py
--rw-rw----   0 hayun      (502) staff       (20)      914 2023-03-28 13:45:19.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/unlock_enemy_guide.py
--rw-rw----   0 hayun      (502) staff       (20)      326 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/unlock_equip_menu.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2024-03-22 01:00:47.706017 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/save_management/
--rw-rw----   0 hayun      (502) staff       (20)       56 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/save_management/__init__.py
--rw-rw----   0 hayun      (502) staff       (20)      841 2023-05-20 14:27:18.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/save_management/convert.py
--rw-rw----   0 hayun      (502) staff       (20)     2575 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/save_management/load.py
--rw-rw----   0 hayun      (502) staff       (20)      657 2023-04-12 00:58:57.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/save_management/other.py
--rw-rw----   0 hayun      (502) staff       (20)     2447 2024-03-20 13:29:09.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/save_management/save.py
--rw-rw----   0 hayun      (502) staff       (20)     1904 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/save_management/server_upload.py
--rw-rw----   0 hayun      (502) staff       (20)    12640 2023-05-26 02:00:11.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/feature_handler.py
--rw-rw----   0 hayun      (502) staff       (20)     4822 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/game_data_getter.py
--rw-rw----   0 hayun      (502) staff       (20)    22847 2024-03-20 13:32:32.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/helper.py
--rw-rw----   0 hayun      (502) staff       (20)     7075 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/item.py
--rw-rw----   0 hayun      (502) staff       (20)     3635 2023-05-07 09:06:08.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/locale_handler.py
--rw-rw----   0 hayun      (502) staff       (20)     1269 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/managed_item.py
--rw-rw----   0 hayun      (502) staff       (20)    72085 2023-10-04 08:05:22.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/parse_save.py
--rw-rw----   0 hayun      (502) staff       (20)     1301 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/patcher.py
--rw-rw----   0 hayun      (502) staff       (20)     2415 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/root_handler.py
--rw-rw----   0 hayun      (502) staff       (20)    55824 2023-10-04 08:20:22.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/serialise_save.py
--rw-rw----   0 hayun      (502) staff       (20)    24703 2023-11-28 01:37:46.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/server_handler.py
--rw-rw----   0 hayun      (502) staff       (20)     3920 2024-03-22 01:00:29.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/tracker.py
--rw-rw----   0 hayun      (502) staff       (20)     3486 2023-03-25 14:14:04.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/updater.py
--rw-rw----   0 hayun      (502) staff       (20)     8175 2023-03-31 01:12:30.000000 bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/user_input_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2024-03-22 01:00:47.712776 bcsfe-iosapi-2.7.67/src/bcsfe_iosapi.egg-info/
--rw-r--r--   0 hayun      (502) staff       (20)      242 2024-03-22 01:00:47.000000 bcsfe-iosapi-2.7.67/src/bcsfe_iosapi.egg-info/PKG-INFO
--rw-r--r--   0 hayun      (502) staff       (20)     4201 2024-03-22 01:00:47.000000 bcsfe-iosapi-2.7.67/src/bcsfe_iosapi.egg-info/SOURCES.txt
--rw-r--r--   0 hayun      (502) staff       (20)        1 2024-03-22 01:00:47.000000 bcsfe-iosapi-2.7.67/src/bcsfe_iosapi.egg-info/dependency_links.txt
--rw-r--r--   0 hayun      (502) staff       (20)       87 2024-03-22 01:00:47.000000 bcsfe-iosapi-2.7.67/src/bcsfe_iosapi.egg-info/requires.txt
--rw-r--r--   0 hayun      (502) staff       (20)       21 2024-03-22 01:00:47.000000 bcsfe-iosapi-2.7.67/src/bcsfe_iosapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 02:58:34.800710 bcsfe-iosapi-2.7.68/
+-rw-rw-rw-   0        0        0      209 2024-04-11 02:58:34.802122 bcsfe-iosapi-2.7.68/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-11 02:58:34.833997 bcsfe-iosapi-2.7.68/setup.cfg
+-rw-rw-rw-   0        0        0      763 2024-04-11 02:58:23.000000 bcsfe-iosapi-2.7.68/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:58:28.284498 bcsfe-iosapi-2.7.68/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 02:58:29.218408 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/
+-rw-rw-rw-   0        0        0      281 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/__init__.py
+-rw-rw-rw-   0        0        0     9869 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/__main__.py
+-rw-rw-rw-   0        0        0    10151 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/adb_handler.py
+-rw-rw-rw-   0        0        0    15039 2023-05-20 14:53:44.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/config_manager.py
+-rw-rw-rw-   0        0        0     1501 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/csv_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:58:29.277401 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/
+-rw-rw-rw-   0        0        0       67 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:58:29.835082 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/
+-rw-rw-rw-   0        0        0      122 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/__init__.py
+-rw-rw-rw-   0        0        0     8734 2023-05-26 02:04:50.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/basic_items.py
+-rw-rw-rw-   0        0        0     1490 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/catfruit.py
+-rw-rw-rw-   0        0        0     1931 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/catseyes.py
+-rw-rw-rw-   0        0        0     1647 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0        0        0     3984 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/talent_orbs.py
+-rw-rw-rw-   0        0        0    16400 2023-07-17 01:03:54.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/talent_orbs_new.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:58:30.394056 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/
+-rw-rw-rw-   0        0        0      179 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/__init__.py
+-rw-rw-rw-   0        0        0     8978 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/cat_helper.py
+-rw-rw-rw-   0        0        0    11125 2023-08-17 04:30:30.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0        0        0     3096 2023-08-16 04:12:21.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/chara_drop.py
+-rw-rw-rw-   0        0        0     1068 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0        0        0     2844 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/evolve_cats.py
+-rw-rw-rw-   0        0        0     1260 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0        0        0     7936 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/talents.py
+-rw-rw-rw-   0        0        0     1904 2023-07-17 00:19:00.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0        0        0     3507 2023-03-28 04:18:30.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/upgrade_cats.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:58:30.831064 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/gamototo/
+-rw-rw-rw-   0        0        0       66 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/gamototo/__init__.py
+-rw-rw-rw-   0        0        0      309 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0        0        0     2659 2023-05-26 07:00:35.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0        0        0     3418 2023-05-31 04:36:47.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/gamototo/helpers.py
+-rw-rw-rw-   0        0        0     4137 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/gamototo/ototo_cat_cannon.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:58:32.153191 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/
+-rw-rw-rw-   0        0        0      313 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/__init__.py
+-rw-rw-rw-   0        0        0     1024 2023-03-28 13:41:31.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/aku.py
+-rw-rw-rw-   0        0        0      491 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0        0        0      790 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0        0        0      646 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0        0        0     1121 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/enigma_stages.py
+-rw-rw-rw-   0        0        0     5924 2023-03-28 13:39:14.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/event_stages.py
+-rw-rw-rw-   0        0        0     1873 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/gauntlet.py
+-rw-rw-rw-   0        0        0     1032 2023-07-20 00:35:37.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0        0        0     1469 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/legend_quest.py
+-rw-rw-rw-   0        0        0     4382 2023-03-31 01:13:58.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/main_story.py
+-rw-rw-rw-   0        0        0     2100 2024-02-03 01:20:25.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/outbreaks.py
+-rw-rw-rw-   0        0        0     2824 2023-03-31 07:47:07.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0        0        0     1175 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/towers.py
+-rw-rw-rw-   0        0        0     8909 2023-03-31 02:09:48.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/treasures.py
+-rw-rw-rw-   0        0        0      868 2023-03-28 13:37:22.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/uncanny.py
+-rw-rw-rw-   0        0        0      784 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/unlock_aku_realm.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:58:33.811598 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/
+-rw-rw-rw-   0        0        0      276 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/__init__.py
+-rw-rw-rw-   0        0        0     3771 2024-02-03 01:35:41.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/cat_shrine.py
+-rw-rw-rw-   0        0        0     1093 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0        0        0     1054 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/create_new_account.py
+-rw-rw-rw-   0        0        0     2171 2023-03-28 13:43:08.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0        0        0      659 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/fix_time_issues.py
+-rw-rw-rw-   0        0        0     3183 2023-08-17 02:51:45.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/get_gold_pass.py
+-rw-rw-rw-   0        0        0     7138 2023-06-11 23:05:06.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/meow_medals.py
+-rw-rw-rw-   0        0        0     4354 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/missions.py
+-rw-rw-rw-   0        0        0      975 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/play_time.py
+-rw-rw-rw-   0        0        0     4568 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/scheme_item.py
+-rw-rw-rw-   0        0        0     1612 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/trade_progress.py
+-rw-rw-rw-   0        0        0      914 2023-03-28 13:45:19.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0        0        0      326 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/unlock_equip_menu.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:58:34.135374 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/save_management/
+-rw-rw-rw-   0        0        0       56 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/save_management/__init__.py
+-rw-rw-rw-   0        0        0      841 2023-05-20 14:27:18.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/save_management/convert.py
+-rw-rw-rw-   0        0        0     2575 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/save_management/load.py
+-rw-rw-rw-   0        0        0      657 2023-04-12 00:58:57.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/save_management/other.py
+-rw-rw-rw-   0        0        0     2447 2024-03-20 13:29:09.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/save_management/save.py
+-rw-rw-rw-   0        0        0     1904 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/save_management/server_upload.py
+-rw-rw-rw-   0        0        0    12640 2023-05-26 02:00:11.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/feature_handler.py
+-rw-rw-rw-   0        0        0     4822 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/game_data_getter.py
+-rw-rw-rw-   0        0        0    22847 2024-03-20 13:32:32.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/helper.py
+-rw-rw-rw-   0        0        0     7075 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/item.py
+-rw-rw-rw-   0        0        0     3635 2023-05-07 09:06:08.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/locale_handler.py
+-rw-rw-rw-   0        0        0     1269 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/managed_item.py
+-rw-rw-rw-   0        0        0    72085 2023-10-04 08:05:22.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/parse_save.py
+-rw-rw-rw-   0        0        0     1301 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/patcher.py
+-rw-rw-rw-   0        0        0        0 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/py.typed
+-rw-rw-rw-   0        0        0     2415 2023-03-22 09:57:23.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/root_handler.py
+-rw-rw-rw-   0        0        0    55824 2023-10-04 08:20:22.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/serialise_save.py
+-rw-rw-rw-   0        0        0    24990 2024-04-11 02:57:08.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/server_handler.py
+-rw-rw-rw-   0        0        0     3920 2024-03-22 01:00:29.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/tracker.py
+-rw-rw-rw-   0        0        0     3486 2023-03-25 14:14:04.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/updater.py
+-rw-rw-rw-   0        0        0     8175 2023-03-31 01:12:30.000000 bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/user_input_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:58:34.642365 bcsfe-iosapi-2.7.68/src/bcsfe_iosapi.egg-info/
+-rw-rw-rw-   0        0        0      209 2024-04-11 02:58:27.000000 bcsfe-iosapi-2.7.68/src/bcsfe_iosapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4235 2024-04-11 02:58:27.000000 bcsfe-iosapi-2.7.68/src/bcsfe_iosapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 02:58:27.000000 bcsfe-iosapi-2.7.68/src/bcsfe_iosapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2024-04-11 02:58:27.000000 bcsfe-iosapi-2.7.68/src/bcsfe_iosapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-11 02:58:27.000000 bcsfe-iosapi-2.7.68/src/bcsfe_iosapi.egg-info/top_level.txt
```

### Comparing `bcsfe-iosapi-2.7.67/setup.py` & `bcsfe-iosapi-2.7.68/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 import setuptools
 setup(
     name="bcsfe-iosapi",
-    version='2.7.67',
+    version='2.7.68',
     author="CintagramABP",
     description="BCSFE_Python personal api",
     long_description="BCSFE_Python personal api",
     url="",
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.9",
```

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/__main__.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/__main__.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/adb_handler.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/adb_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/config_manager.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/config_manager.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/csv_handler.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/csv_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/basic_items.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/catfruit.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/catseyes.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/ototo_base_mats.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/talent_orbs.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/basic/talent_orbs_new.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/cat_helper.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/cat_id_selector.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/chara_drop.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/clear_cat_guide.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/evolve_cats.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/get_remove_cats.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/talents.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/upgrade_blue.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/cats/upgrade_cats.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/gamototo/gamatoto_xp.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/gamototo/helpers.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/gamototo/ototo_cat_cannon.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/aku.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/behemoth_culling.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/clear_tutorial.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/enigma_stages.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/event_stages.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/gauntlet.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/itf_timed_scores.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/legend_quest.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/main_story.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/outbreaks.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/story_level_id_selector.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/towers.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/treasures.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/uncanny.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/levels/unlock_aku_realm.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/cat_shrine.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/claim_user_rank_rewards.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/create_new_account.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/fix_elsewhere.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/fix_time_issues.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/get_gold_pass.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/meow_medals.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/missions.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/play_time.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/scheme_item.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/trade_progress.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/other/unlock_enemy_guide.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/save_management/convert.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/save_management/load.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/save_management/other.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/save_management/save.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/edits/save_management/server_upload.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/feature_handler.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/feature_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/game_data_getter.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/helper.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/helper.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/item.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/item.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/locale_handler.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/locale_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/managed_item.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/managed_item.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/parse_save.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/parse_save.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/patcher.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/patcher.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/root_handler.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/root_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/serialise_save.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/serialise_save.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/server_handler.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/server_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Handler for server requests"""
 
 import datetime
 import hashlib
 import hmac
 import json
 from random import randint
+import os
 import time
 from typing import Any, Optional, Union
 
 import requests
 
 from . import helper, managed_item, serialise_save, patcher, config_manager, tracker
 
@@ -635,14 +636,15 @@
     save_stats["token"] = password_refresh_token
     return save_stats, password_refresh_data
 
 
 def prepare_upload(
     save_stats: dict[str, Any],
     path: str,
+    documents_dir: str,
     print_text: bool = True,
     managed_items: Optional[list[managed_item.ManagedItem]] = None,
 ) -> Optional[tuple[str, Any, bytes, int, list[managed_item.ManagedItem]]]:
     """Handles the pre-upload of the save data"""
 
     original_iq = save_stats["inquiry_code"]
     
@@ -655,32 +657,32 @@
             helper.colored_text(
                 "Error getting account auth token",
                 helper.RED,
             )
         return None
     item_tracker = tracker.Tracker()
     if original_iq != inquiry_code:
-        item_tracker.reset_tracker()
+        item_tracker.reset_tracker(os.path.join(os.path.abspath(os.path.dirname(os.path.join(documents_dir, "SAVE_DATA"))), "item_tracker.json"))
         update_managed_items(save_stats["inquiry_code"], token, save_stats)
 
     
     if managed_items is None:
         managed_items = item_tracker.parse_tracker_managed()
     playtime = helper.time_to_frames(save_stats["play_time"])
-    tracker.Tracker().reset_tracker()
+    tracker.Tracker().reset_tracker(os.path.join(os.path.abspath(os.path.dirname(os.path.join(documents_dir, "SAVE_DATA"))), "item_tracker.json"))
 
     return token, inquiry_code, save_data, playtime, managed_items
 
 
 def upload_handler(
-    save_stats: dict[str, Any], path: str
+    save_stats: dict[str, Any], path: str, documents_dir: str
 ) -> Union[None, dict[str, Any]]:
     """Handles the upload of the save data"""
 
-    data = prepare_upload(save_stats, path)
+    data = prepare_upload(save_stats, path, documents_dir)
     if data is None:
         return None
     token, inquiry_code, save_data, playtime, managed_items = data
 
     #helper.colored_text("Uploading save data...", helper.GREEN)
     upload_data = upload_save_data_v2(
         token,
```

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/tracker.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/tracker.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/updater.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/updater.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/BCSFE_Python_Discord/user_input_handler.py` & `bcsfe-iosapi-2.7.68/src/BCSFE_Python_Discord/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-iosapi-2.7.67/src/bcsfe_iosapi.egg-info/SOURCES.txt` & `bcsfe-iosapi-2.7.68/src/bcsfe_iosapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/BCSFE_Python_Discord/game_data_getter.py
 src/BCSFE_Python_Discord/helper.py
 src/BCSFE_Python_Discord/item.py
 src/BCSFE_Python_Discord/locale_handler.py
 src/BCSFE_Python_Discord/managed_item.py
 src/BCSFE_Python_Discord/parse_save.py
 src/BCSFE_Python_Discord/patcher.py
+src/BCSFE_Python_Discord/py.typed
 src/BCSFE_Python_Discord/root_handler.py
 src/BCSFE_Python_Discord/serialise_save.py
 src/BCSFE_Python_Discord/server_handler.py
 src/BCSFE_Python_Discord/tracker.py
 src/BCSFE_Python_Discord/updater.py
 src/BCSFE_Python_Discord/user_input_handler.py
 src/BCSFE_Python_Discord/edits/__init__.py
```

