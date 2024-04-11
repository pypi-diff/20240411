# Comparing `tmp/gage-0.0.3.tar.gz` & `tmp/gage-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gage-0.0.3.tar", last modified: Thu Aug 31 23:19:19 2023, max compression
+gzip compressed data, was "gage-0.1.0.tar", last modified: Thu Apr 11 16:33:20 2024, max compression
```

## Comparing `gage-0.0.3.tar` & `gage-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,105 @@
-drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2023-08-31 23:19:19.535539 gage-0.0.3/
--rw-rw-r--   0 garrett   (1000) garrett   (1000)    11358 2023-08-31 21:14:43.000000 gage-0.0.3/LICENSE.txt
--rw-rw-r--   0 garrett   (1000) garrett   (1000)      541 2023-08-31 23:19:19.535539 gage-0.0.3/PKG-INFO
--rw-rw-r--   0 garrett   (1000) garrett   (1000)       20 2023-08-31 21:17:26.000000 gage-0.0.3/README.md
-drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2023-08-31 23:19:19.535539 gage-0.0.3/gage.egg-info/
--rw-rw-r--   0 garrett   (1000) garrett   (1000)      541 2023-08-31 23:19:19.000000 gage-0.0.3/gage.egg-info/PKG-INFO
--rw-rw-r--   0 garrett   (1000) garrett   (1000)      148 2023-08-31 23:19:19.000000 gage-0.0.3/gage.egg-info/SOURCES.txt
--rw-rw-r--   0 garrett   (1000) garrett   (1000)        1 2023-08-31 23:19:19.000000 gage-0.0.3/gage.egg-info/dependency_links.txt
--rw-rw-r--   0 garrett   (1000) garrett   (1000)        1 2023-08-31 23:19:19.000000 gage-0.0.3/gage.egg-info/top_level.txt
--rw-rw-r--   0 garrett   (1000) garrett   (1000)      505 2023-08-31 23:19:16.000000 gage-0.0.3/pyproject.toml
--rw-rw-r--   0 garrett   (1000) garrett   (1000)       38 2023-08-31 23:19:19.535539 gage-0.0.3/setup.cfg
+drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2024-04-11 16:33:20.279688 gage-0.1.0/
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      623 2024-04-02 16:25:16.000000 gage-0.1.0/AUTHORS.md
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    11358 2023-12-08 12:08:15.000000 gage-0.1.0/LICENSE.txt
+-rw-r--r--   0 garrett   (1000) garrett   (1000)     2881 2024-04-11 16:33:20.279688 gage-0.1.0/PKG-INFO
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1754 2024-04-02 16:24:41.000000 gage-0.1.0/README.md
+drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2024-04-11 16:33:20.275688 gage-0.1.0/gage/
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      159 2024-04-02 16:22:54.000000 gage-0.1.0/gage/__init__.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1386 2023-12-08 12:08:15.000000 gage-0.1.0/gage/__main__.py
+drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2024-04-11 16:33:20.279688 gage-0.1.0/gage/_internal/
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)        0 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/__init__.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      154 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/ansi_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2255 2024-04-09 18:11:21.000000 gage-0.1.0/gage/_internal/api.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     3212 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/attr_log.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    10993 2024-01-19 15:26:19.000000 gage-0.1.0/gage/_internal/board_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      497 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/channel.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    10670 2024-02-07 14:41:20.000000 gage-0.1.0/gage/_internal/cli.py
+drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2024-04-11 16:33:20.279688 gage-0.1.0/gage/_internal/commands/
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1200 2023-12-29 15:43:01.000000 gage-0.1.0/gage/_internal/commands/associate.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      972 2023-12-29 15:43:01.000000 gage-0.1.0/gage/_internal/commands/associate_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1400 2024-02-01 16:00:05.000000 gage-0.1.0/gage/_internal/commands/board.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     3508 2024-04-05 13:16:44.000000 gage-0.1.0/gage/_internal/commands/board_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      978 2024-01-09 16:16:41.000000 gage-0.1.0/gage/_internal/commands/cat.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1214 2024-04-02 16:25:32.000000 gage-0.1.0/gage/_internal/commands/check.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     3787 2024-01-09 13:04:35.000000 gage-0.1.0/gage/_internal/commands/check_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2246 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/comment.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     4421 2023-12-27 03:14:39.000000 gage-0.1.0/gage/_internal/commands/comment_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2334 2024-01-24 19:41:18.000000 gage-0.1.0/gage/_internal/commands/copy.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    10960 2024-04-05 19:38:38.000000 gage-0.1.0/gage/_internal/commands/copy_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1472 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/delete.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2119 2024-01-27 17:48:48.000000 gage-0.1.0/gage/_internal/commands/delete_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2788 2024-01-09 13:08:56.000000 gage-0.1.0/gage/_internal/commands/error_handlers.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1339 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/help.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     7239 2024-02-01 17:43:09.000000 gage-0.1.0/gage/_internal/commands/impl_support.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1595 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/label.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2022 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/label_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2150 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/list.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1289 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/list_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2668 2024-04-11 14:59:26.000000 gage-0.1.0/gage/_internal/commands/main.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1106 2024-04-02 16:25:42.000000 gage-0.1.0/gage/_internal/commands/main_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1429 2024-01-09 13:17:16.000000 gage-0.1.0/gage/_internal/commands/open.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2613 2024-01-09 13:32:59.000000 gage-0.1.0/gage/_internal/commands/open_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      591 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/operations.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      899 2024-01-09 12:25:25.000000 gage-0.1.0/gage/_internal/commands/operations_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1504 2024-03-02 05:01:34.000000 gage-0.1.0/gage/_internal/commands/publish.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     5723 2024-03-11 14:01:07.000000 gage-0.1.0/gage/_internal/commands/publish_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1246 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/purge.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1611 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/purge_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1256 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/restore.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1576 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/restore_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2661 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/run.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    11198 2024-01-16 16:11:04.000000 gage-0.1.0/gage/_internal/commands/run_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1365 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/select.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      823 2023-12-27 03:06:47.000000 gage-0.1.0/gage/_internal/commands/select_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1708 2024-01-16 12:15:12.000000 gage-0.1.0/gage/_internal/commands/show.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    10257 2024-01-09 16:43:50.000000 gage-0.1.0/gage/_internal/commands/show_impl.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      342 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/commands/sign.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      143 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/exitcodes.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    19298 2024-01-12 11:41:46.000000 gage-0.1.0/gage/_internal/file_select.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    16078 2023-12-13 15:35:05.000000 gage-0.1.0/gage/_internal/file_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1594 2024-01-14 16:51:54.000000 gage-0.1.0/gage/_internal/gagefile.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     4304 2024-01-09 15:58:44.000000 gage-0.1.0/gage/_internal/lang.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     3087 2024-02-01 14:47:27.000000 gage-0.1.0/gage/_internal/log.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1067 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/opref_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      990 2024-01-16 16:28:21.000000 gage-0.1.0/gage/_internal/progress_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2025 2024-04-11 15:56:04.000000 gage-0.1.0/gage/_internal/project_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    17556 2023-12-13 15:35:05.000000 gage-0.1.0/gage/_internal/python_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1350 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/repo.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)       60 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/repo_git.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)       60 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/repo_local.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)       60 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/repo_rclone.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)       60 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/repo_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1997 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/run_comment.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     8341 2024-01-12 12:10:40.000000 gage-0.1.0/gage/_internal/run_config.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     6129 2023-12-24 14:54:39.000000 gage-0.1.0/gage/_internal/run_config_py.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1613 2023-12-29 19:01:49.000000 gage-0.1.0/gage/_internal/run_context.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)       60 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/run_dependencies.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1226 2023-12-30 01:19:14.000000 gage-0.1.0/gage/_internal/run_filter.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1980 2024-02-15 17:15:53.000000 gage-0.1.0/gage/_internal/run_help.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     9717 2024-01-16 14:59:58.000000 gage-0.1.0/gage/_internal/run_output.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1634 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/run_select.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2072 2024-02-21 20:39:12.000000 gage-0.1.0/gage/_internal/run_sourcecode.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    35590 2024-04-09 18:01:13.000000 gage-0.1.0/gage/_internal/run_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1226 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/schema_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      963 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/shlex_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1841 2024-01-09 12:51:03.000000 gage-0.1.0/gage/_internal/sys_config.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    13756 2024-02-01 16:23:19.000000 gage-0.1.0/gage/_internal/test.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    23703 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/typer_rich_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    13531 2024-02-01 20:33:36.000000 gage-0.1.0/gage/_internal/types.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2364 2024-01-14 16:51:54.000000 gage-0.1.0/gage/_internal/user_config.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    31992 2024-01-19 15:22:53.000000 gage-0.1.0/gage/_internal/util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     6054 2024-02-01 15:15:33.000000 gage-0.1.0/gage/_internal/var.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    17567 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/vcs_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     4921 2023-12-08 12:08:15.000000 gage-0.1.0/gage/_internal/yaml_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     7290 2024-01-16 13:20:58.000000 gage-0.1.0/gage/gagefile.schema.json
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2227 2023-12-27 14:48:24.000000 gage-0.1.0/gage/summary.schema.json
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      879 2023-12-27 14:14:26.000000 gage-0.1.0/gage/userconfig.schema.json
+drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2024-04-11 16:33:20.279688 gage-0.1.0/gage.egg-info/
+-rw-r--r--   0 garrett   (1000) garrett   (1000)     2881 2024-04-11 16:33:20.000000 gage-0.1.0/gage.egg-info/PKG-INFO
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2961 2024-04-11 16:33:20.000000 gage-0.1.0/gage.egg-info/SOURCES.txt
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)        1 2024-04-11 16:33:20.000000 gage-0.1.0/gage.egg-info/dependency_links.txt
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)       44 2024-04-11 16:33:20.000000 gage-0.1.0/gage.egg-info/entry_points.txt
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      271 2024-04-11 16:33:20.000000 gage-0.1.0/gage.egg-info/requires.txt
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)        5 2024-04-11 16:33:20.000000 gage-0.1.0/gage.egg-info/top_level.txt
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     1287 2024-04-11 16:33:11.000000 gage-0.1.0/pyproject.toml
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)       38 2024-04-11 16:33:20.279688 gage-0.1.0/setup.cfg
```

### Comparing `gage-0.0.3/LICENSE.txt` & `gage-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

