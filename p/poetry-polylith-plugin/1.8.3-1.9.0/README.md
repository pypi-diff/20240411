# Comparing `tmp/poetry_polylith_plugin-1.8.3.tar.gz` & `tmp/poetry_polylith_plugin-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_polylith_plugin-1.8.3.tar", max compression
+gzip compressed data, was "poetry_polylith_plugin-1.9.0.tar", max compression
```

## Comparing `poetry_polylith_plugin-1.8.3.tar` & `poetry_polylith_plugin-1.9.0.tar`

### file list

```diff
@@ -1,64 +1,66 @@
--rw-r--r--   0        0        0     1475 2023-05-12 15:15:56.171200 poetry_polylith_plugin-1.8.3/README.md
--rw-r--r--   0        0        0      244 2022-11-08 07:28:40.662859 poetry_polylith_plugin-1.8.3/polylith/bricks/__init__.py
--rw-r--r--   0        0        0      555 2023-05-12 15:15:55.733350 poetry_polylith_plugin-1.8.3/polylith/bricks/base.py
--rw-r--r--   0        0        0     1045 2023-05-12 15:15:55.750247 poetry_polylith_plugin-1.8.3/polylith/bricks/brick.py
--rw-r--r--   0        0        0     1096 2023-05-12 15:15:55.764821 poetry_polylith_plugin-1.8.3/polylith/bricks/component.py
--rw-r--r--   0        0        0       98 2023-08-01 17:06:45.291386 poetry_polylith_plugin-1.8.3/polylith/check/__init__.py
--rw-r--r--   0        0        0     1347 2023-08-01 17:06:45.291866 poetry_polylith_plugin-1.8.3/polylith/check/collect.py
--rw-r--r--   0        0        0     1051 2023-05-12 15:15:55.788886 poetry_polylith_plugin-1.8.3/polylith/check/grouping.py
--rw-r--r--   0        0        0     2532 2023-09-24 08:48:27.785750 poetry_polylith_plugin-1.8.3/polylith/check/report.py
--rw-r--r--   0        0        0       98 2022-11-02 17:12:23.977141 poetry_polylith_plugin-1.8.3/polylith/development/__init__.py
--rw-r--r--   0        0        0      211 2023-08-06 15:02:52.120071 poetry_polylith_plugin-1.8.3/polylith/development/development.py
--rw-r--r--   0        0        0       75 2022-11-14 11:36:16.519559 poetry_polylith_plugin-1.8.3/polylith/diff/__init__.py
--rw-r--r--   0        0        0     1750 2023-05-12 15:15:55.823297 poetry_polylith_plugin-1.8.3/polylith/diff/collect.py
--rw-r--r--   0        0        0     1997 2023-08-01 17:06:45.293180 poetry_polylith_plugin-1.8.3/polylith/diff/report.py
--rw-r--r--   0        0        0       68 2022-11-02 17:12:23.977917 poetry_polylith_plugin-1.8.3/polylith/dirs/__init__.py
--rw-r--r--   0        0        0      273 2023-01-06 10:47:07.824141 poetry_polylith_plugin-1.8.3/polylith/dirs/dirs.py
--rw-r--r--   0        0        0       72 2022-11-02 17:12:23.978829 poetry_polylith_plugin-1.8.3/polylith/files/__init__.py
--rw-r--r--   0        0        0      145 2022-12-22 20:33:19.860064 poetry_polylith_plugin-1.8.3/polylith/files/files.py
--rw-r--r--   0        0        0      151 2023-05-12 15:15:55.824841 poetry_polylith_plugin-1.8.3/polylith/imports/__init__.py
--rw-r--r--   0        0        0     1730 2023-08-01 17:06:45.293972 poetry_polylith_plugin-1.8.3/polylith/imports/parser.py
--rw-r--r--   0        0        0      528 2023-08-01 17:06:45.294790 poetry_polylith_plugin-1.8.3/polylith/info/__init__.py
--rw-r--r--   0        0        0     1692 2023-05-12 15:15:55.855648 poetry_polylith_plugin-1.8.3/polylith/info/collect.py
--rw-r--r--   0        0        0     3116 2023-08-01 17:06:45.295397 poetry_polylith_plugin-1.8.3/polylith/info/report.py
--rw-r--r--   0        0        0       91 2022-11-02 17:12:23.979601 poetry_polylith_plugin-1.8.3/polylith/interface/__init__.py
--rw-r--r--   0        0        0      876 2023-05-12 15:15:55.872999 poetry_polylith_plugin-1.8.3/polylith/interface/interfaces.py
--rw-r--r--   0        0        0      201 2023-05-12 15:15:55.873649 poetry_polylith_plugin-1.8.3/polylith/libs/__init__.py
--rw-r--r--   0        0        0     1220 2023-05-12 15:15:55.874316 poetry_polylith_plugin-1.8.3/polylith/libs/grouping.py
--rw-r--r--   0        0        0     3782 2023-09-09 05:49:26.983597 poetry_polylith_plugin-1.8.3/polylith/libs/report.py
--rw-r--r--   0        0        0     4156 2023-05-12 15:15:55.903740 poetry_polylith_plugin-1.8.3/polylith/libs/stdlib.py
--rw-r--r--   0        0        0      790 2023-05-12 15:15:55.904737 poetry_polylith_plugin-1.8.3/polylith/poetry/commands/__init__.py
--rw-r--r--   0        0        0     2768 2023-09-24 08:48:27.786475 poetry_polylith_plugin-1.8.3/polylith/poetry/commands/check.py
--rw-r--r--   0        0        0      552 2023-05-12 15:15:55.925171 poetry_polylith_plugin-1.8.3/polylith/poetry/commands/create.py
--rw-r--r--   0        0        0      634 2023-05-12 15:15:55.926137 poetry_polylith_plugin-1.8.3/polylith/poetry/commands/create_base.py
--rw-r--r--   0        0        0      674 2023-05-12 15:15:55.927148 poetry_polylith_plugin-1.8.3/polylith/poetry/commands/create_component.py
--rw-r--r--   0        0        0      680 2023-05-12 15:15:55.943908 poetry_polylith_plugin-1.8.3/polylith/poetry/commands/create_project.py
--rw-r--r--   0        0        0      949 2022-11-13 15:37:24.280622 poetry_polylith_plugin-1.8.3/polylith/poetry/commands/create_workspace.py
--rw-r--r--   0        0        0     1744 2023-05-12 15:15:55.944899 poetry_polylith_plugin-1.8.3/polylith/poetry/commands/diff.py
--rw-r--r--   0        0        0     1374 2023-08-01 18:21:47.212547 poetry_polylith_plugin-1.8.3/polylith/poetry/commands/info.py
--rw-r--r--   0        0        0     2328 2023-05-12 15:15:55.964742 poetry_polylith_plugin-1.8.3/polylith/poetry/commands/libs.py
--rw-r--r--   0        0        0     1895 2023-09-24 08:48:27.787021 poetry_polylith_plugin-1.8.3/polylith/poetry/commands/sync.py
--rw-r--r--   0        0        0       87 2022-11-02 17:12:23.974544 poetry_polylith_plugin-1.8.3/polylith/poetry_plugin/__init__.py
--rw-r--r--   0        0        0      959 2023-05-12 15:15:55.714878 poetry_polylith_plugin-1.8.3/polylith/poetry_plugin/plugin.py
--rw-r--r--   0        0        0      331 2023-05-12 15:15:55.976822 poetry_polylith_plugin-1.8.3/polylith/project/__init__.py
--rw-r--r--   0        0        0     1577 2023-05-12 15:15:55.977717 poetry_polylith_plugin-1.8.3/polylith/project/create.py
--rw-r--r--   0        0        0     1433 2023-05-12 15:15:55.986679 poetry_polylith_plugin-1.8.3/polylith/project/get.py
--rw-r--r--   0        0        0      433 2023-05-12 15:15:55.987825 poetry_polylith_plugin-1.8.3/polylith/project/parser.py
--rw-r--r--   0        0        0      142 2023-05-12 15:15:55.988558 poetry_polylith_plugin-1.8.3/polylith/readme/__init__.py
--rw-r--r--   0        0        0     1067 2023-05-12 15:15:55.999067 poetry_polylith_plugin-1.8.3/polylith/readme/readme.py
--rw-r--r--   0        0        0      374 2022-11-07 20:40:56.909336 poetry_polylith_plugin-1.8.3/polylith/repo/__init__.py
--rw-r--r--   0        0        0      985 2022-11-07 20:40:56.910072 poetry_polylith_plugin-1.8.3/polylith/repo/repo.py
--rw-r--r--   0        0        0       58 2023-05-12 15:15:55.999977 poetry_polylith_plugin-1.8.3/polylith/reporting/__init__.py
--rw-r--r--   0        0        0      172 2023-05-12 15:15:56.009984 poetry_polylith_plugin-1.8.3/polylith/reporting/theme.py
--rw-r--r--   0        0        0      188 2023-05-12 15:15:56.011093 poetry_polylith_plugin-1.8.3/polylith/sync/__init__.py
--rw-r--r--   0        0        0     1853 2023-08-01 17:06:45.298548 poetry_polylith_plugin-1.8.3/polylith/sync/collect.py
--rw-r--r--   0        0        0      971 2023-08-01 17:06:45.299029 poetry_polylith_plugin-1.8.3/polylith/sync/report.py
--rw-r--r--   0        0        0     1787 2023-05-28 09:27:04.695588 poetry_polylith_plugin-1.8.3/polylith/sync/update.py
--rw-r--r--   0        0        0       71 2022-11-02 17:12:23.985824 poetry_polylith_plugin-1.8.3/polylith/test/__init__.py
--rw-r--r--   0        0        0      859 2022-11-13 15:37:24.282091 poetry_polylith_plugin-1.8.3/polylith/test/tests.py
--rw-r--r--   0        0        0       94 2023-05-12 15:15:56.080084 poetry_polylith_plugin-1.8.3/polylith/workspace/__init__.py
--rw-r--r--   0        0        0     1089 2023-05-12 15:15:56.095307 poetry_polylith_plugin-1.8.3/polylith/workspace/create.py
--rw-r--r--   0        0        0     1832 2023-05-28 09:27:04.708148 poetry_polylith_plugin-1.8.3/polylith/workspace/parser.py
--rw-r--r--   0        0        0      949 2023-05-12 15:15:56.139405 poetry_polylith_plugin-1.8.3/polylith/workspace/paths.py
--rw-r--r--   0        0        0      781 2023-09-24 08:49:02.257545 poetry_polylith_plugin-1.8.3/pyproject.toml
--rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 poetry_polylith_plugin-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1475 2023-05-12 15:15:56.171200 poetry_polylith_plugin-1.9.0/README.md
+-rw-r--r--   0        0        0       73 2023-09-24 19:06:35.859440 poetry_polylith_plugin-1.9.0/polylith/alias/__init__.py
+-rw-r--r--   0        0        0      620 2023-09-24 19:06:35.884719 poetry_polylith_plugin-1.9.0/polylith/alias/core.py
+-rw-r--r--   0        0        0      244 2022-11-08 07:28:40.662859 poetry_polylith_plugin-1.9.0/polylith/bricks/__init__.py
+-rw-r--r--   0        0        0      555 2023-05-12 15:15:55.733350 poetry_polylith_plugin-1.9.0/polylith/bricks/base.py
+-rw-r--r--   0        0        0     1045 2023-05-12 15:15:55.750247 poetry_polylith_plugin-1.9.0/polylith/bricks/brick.py
+-rw-r--r--   0        0        0     1096 2023-05-12 15:15:55.764821 poetry_polylith_plugin-1.9.0/polylith/bricks/component.py
+-rw-r--r--   0        0        0       98 2023-08-01 17:06:45.291386 poetry_polylith_plugin-1.9.0/polylith/check/__init__.py
+-rw-r--r--   0        0        0     1347 2023-08-01 17:06:45.291866 poetry_polylith_plugin-1.9.0/polylith/check/collect.py
+-rw-r--r--   0        0        0     1051 2023-05-12 15:15:55.788886 poetry_polylith_plugin-1.9.0/polylith/check/grouping.py
+-rw-r--r--   0        0        0     2884 2023-09-24 14:12:17.616782 poetry_polylith_plugin-1.9.0/polylith/check/report.py
+-rw-r--r--   0        0        0       98 2022-11-02 17:12:23.977141 poetry_polylith_plugin-1.9.0/polylith/development/__init__.py
+-rw-r--r--   0        0        0      211 2023-08-06 15:02:52.120071 poetry_polylith_plugin-1.9.0/polylith/development/development.py
+-rw-r--r--   0        0        0       75 2022-11-14 11:36:16.519559 poetry_polylith_plugin-1.9.0/polylith/diff/__init__.py
+-rw-r--r--   0        0        0     1750 2023-05-12 15:15:55.823297 poetry_polylith_plugin-1.9.0/polylith/diff/collect.py
+-rw-r--r--   0        0        0     1997 2023-08-01 17:06:45.293180 poetry_polylith_plugin-1.9.0/polylith/diff/report.py
+-rw-r--r--   0        0        0       68 2022-11-02 17:12:23.977917 poetry_polylith_plugin-1.9.0/polylith/dirs/__init__.py
+-rw-r--r--   0        0        0      273 2023-01-06 10:47:07.824141 poetry_polylith_plugin-1.9.0/polylith/dirs/dirs.py
+-rw-r--r--   0        0        0       72 2022-11-02 17:12:23.978829 poetry_polylith_plugin-1.9.0/polylith/files/__init__.py
+-rw-r--r--   0        0        0      145 2022-12-22 20:33:19.860064 poetry_polylith_plugin-1.9.0/polylith/files/files.py
+-rw-r--r--   0        0        0      151 2023-05-12 15:15:55.824841 poetry_polylith_plugin-1.9.0/polylith/imports/__init__.py
+-rw-r--r--   0        0        0     1730 2023-08-01 17:06:45.293972 poetry_polylith_plugin-1.9.0/polylith/imports/parser.py
+-rw-r--r--   0        0        0      528 2023-08-01 17:06:45.294790 poetry_polylith_plugin-1.9.0/polylith/info/__init__.py
+-rw-r--r--   0        0        0     1692 2023-05-12 15:15:55.855648 poetry_polylith_plugin-1.9.0/polylith/info/collect.py
+-rw-r--r--   0        0        0     3116 2023-08-01 17:06:45.295397 poetry_polylith_plugin-1.9.0/polylith/info/report.py
+-rw-r--r--   0        0        0       91 2022-11-02 17:12:23.979601 poetry_polylith_plugin-1.9.0/polylith/interface/__init__.py
+-rw-r--r--   0        0        0      876 2023-05-12 15:15:55.872999 poetry_polylith_plugin-1.9.0/polylith/interface/interfaces.py
+-rw-r--r--   0        0        0      201 2023-05-12 15:15:55.873649 poetry_polylith_plugin-1.9.0/polylith/libs/__init__.py
+-rw-r--r--   0        0        0     1220 2023-05-12 15:15:55.874316 poetry_polylith_plugin-1.9.0/polylith/libs/grouping.py
+-rw-r--r--   0        0        0     4066 2023-09-24 14:12:17.617369 poetry_polylith_plugin-1.9.0/polylith/libs/report.py
+-rw-r--r--   0        0        0     4156 2023-05-12 15:15:55.903740 poetry_polylith_plugin-1.9.0/polylith/libs/stdlib.py
+-rw-r--r--   0        0        0      790 2023-05-12 15:15:55.904737 poetry_polylith_plugin-1.9.0/polylith/poetry/commands/__init__.py
+-rw-r--r--   0        0        0     3687 2023-09-24 19:06:35.885471 poetry_polylith_plugin-1.9.0/polylith/poetry/commands/check.py
+-rw-r--r--   0        0        0      552 2023-05-12 15:15:55.925171 poetry_polylith_plugin-1.9.0/polylith/poetry/commands/create.py
+-rw-r--r--   0        0        0      634 2023-05-12 15:15:55.926137 poetry_polylith_plugin-1.9.0/polylith/poetry/commands/create_base.py
+-rw-r--r--   0        0        0      674 2023-05-12 15:15:55.927148 poetry_polylith_plugin-1.9.0/polylith/poetry/commands/create_component.py
+-rw-r--r--   0        0        0      680 2023-05-12 15:15:55.943908 poetry_polylith_plugin-1.9.0/polylith/poetry/commands/create_project.py
+-rw-r--r--   0        0        0      949 2022-11-13 15:37:24.280622 poetry_polylith_plugin-1.9.0/polylith/poetry/commands/create_workspace.py
+-rw-r--r--   0        0        0     1744 2023-05-12 15:15:55.944899 poetry_polylith_plugin-1.9.0/polylith/poetry/commands/diff.py
+-rw-r--r--   0        0        0     1374 2023-08-01 18:21:47.212547 poetry_polylith_plugin-1.9.0/polylith/poetry/commands/info.py
+-rw-r--r--   0        0        0     2261 2023-09-24 19:06:35.886105 poetry_polylith_plugin-1.9.0/polylith/poetry/commands/libs.py
+-rw-r--r--   0        0        0     1895 2023-09-24 08:48:27.787021 poetry_polylith_plugin-1.9.0/polylith/poetry/commands/sync.py
+-rw-r--r--   0        0        0       87 2022-11-02 17:12:23.974544 poetry_polylith_plugin-1.9.0/polylith/poetry_plugin/__init__.py
+-rw-r--r--   0        0        0      959 2023-05-12 15:15:55.714878 poetry_polylith_plugin-1.9.0/polylith/poetry_plugin/plugin.py
+-rw-r--r--   0        0        0      331 2023-05-12 15:15:55.976822 poetry_polylith_plugin-1.9.0/polylith/project/__init__.py
+-rw-r--r--   0        0        0     1577 2023-05-12 15:15:55.977717 poetry_polylith_plugin-1.9.0/polylith/project/create.py
+-rw-r--r--   0        0        0     1433 2023-05-12 15:15:55.986679 poetry_polylith_plugin-1.9.0/polylith/project/get.py
+-rw-r--r--   0        0        0      433 2023-05-12 15:15:55.987825 poetry_polylith_plugin-1.9.0/polylith/project/parser.py
+-rw-r--r--   0        0        0      142 2023-05-12 15:15:55.988558 poetry_polylith_plugin-1.9.0/polylith/readme/__init__.py
+-rw-r--r--   0        0        0     1067 2023-05-12 15:15:55.999067 poetry_polylith_plugin-1.9.0/polylith/readme/readme.py
+-rw-r--r--   0        0        0      374 2022-11-07 20:40:56.909336 poetry_polylith_plugin-1.9.0/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      985 2022-11-07 20:40:56.910072 poetry_polylith_plugin-1.9.0/polylith/repo/repo.py
+-rw-r--r--   0        0        0       58 2023-05-12 15:15:55.999977 poetry_polylith_plugin-1.9.0/polylith/reporting/__init__.py
+-rw-r--r--   0        0        0      172 2023-05-12 15:15:56.009984 poetry_polylith_plugin-1.9.0/polylith/reporting/theme.py
+-rw-r--r--   0        0        0      188 2023-05-12 15:15:56.011093 poetry_polylith_plugin-1.9.0/polylith/sync/__init__.py
+-rw-r--r--   0        0        0     1853 2023-08-01 17:06:45.298548 poetry_polylith_plugin-1.9.0/polylith/sync/collect.py
+-rw-r--r--   0        0        0      971 2023-08-01 17:06:45.299029 poetry_polylith_plugin-1.9.0/polylith/sync/report.py
+-rw-r--r--   0        0        0     1787 2023-05-28 09:27:04.695588 poetry_polylith_plugin-1.9.0/polylith/sync/update.py
+-rw-r--r--   0        0        0       71 2022-11-02 17:12:23.985824 poetry_polylith_plugin-1.9.0/polylith/test/__init__.py
+-rw-r--r--   0        0        0      859 2022-11-13 15:37:24.282091 poetry_polylith_plugin-1.9.0/polylith/test/tests.py
+-rw-r--r--   0        0        0       94 2023-05-12 15:15:56.080084 poetry_polylith_plugin-1.9.0/polylith/workspace/__init__.py
+-rw-r--r--   0        0        0     1089 2023-05-12 15:15:56.095307 poetry_polylith_plugin-1.9.0/polylith/workspace/create.py
+-rw-r--r--   0        0        0     1832 2023-05-28 09:27:04.708148 poetry_polylith_plugin-1.9.0/polylith/workspace/parser.py
+-rw-r--r--   0        0        0      949 2023-05-12 15:15:56.139405 poetry_polylith_plugin-1.9.0/polylith/workspace/paths.py
+-rw-r--r--   0        0        0      781 2023-09-24 19:07:21.340355 poetry_polylith_plugin-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 poetry_polylith_plugin-1.9.0/PKG-INFO
```

### Comparing `poetry_polylith_plugin-1.8.3/README.md` & `poetry_polylith_plugin-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/bricks/base.py` & `poetry_polylith_plugin-1.9.0/polylith/bricks/base.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/bricks/brick.py` & `poetry_polylith_plugin-1.9.0/polylith/bricks/brick.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/bricks/component.py` & `poetry_polylith_plugin-1.9.0/polylith/bricks/component.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/check/collect.py` & `poetry_polylith_plugin-1.9.0/polylith/check/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/check/grouping.py` & `poetry_polylith_plugin-1.9.0/polylith/check/grouping.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/check/report.py` & `poetry_polylith_plugin-1.9.0/polylith/check/report.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Set, Tuple
+from typing import Set
 
 from polylith import imports, libs, workspace
 from polylith.check import collect, grouping
 from polylith.reporting import theme
 from rich.console import Console
 
 
@@ -37,20 +37,15 @@
 
 def fetch_brick_imports(root: Path, ns: str, all_imports: dict) -> dict:
     extracted = grouping.extract_brick_imports(all_imports, ns)
 
     return collect.with_unknown_components(root, ns, extracted)
 
 
-def create_report(
-    root: Path,
-    ns: str,
-    project_data: dict,
-    third_party_libs: Set,
-) -> Tuple[bool, dict]:
+def collect_all_imports(root: Path, ns: str, project_data: dict) -> dict:
     bases = {b for b in project_data.get("bases", [])}
     components = {c for c in project_data.get("components", [])}
 
     bases_paths = workspace.paths.collect_bases_paths(root, ns, bases)
     components_paths = workspace.paths.collect_components_paths(root, ns, components)
 
     all_imports_in_bases = imports.fetch_all_imports(bases_paths)
@@ -62,20 +57,33 @@
     }
 
     third_party_imports = {
         "bases": libs.extract_third_party_imports(all_imports_in_bases, ns),
         "components": libs.extract_third_party_imports(all_imports_in_components, ns),
     }
 
-    brick_diff = collect.imports_diff(brick_imports, list(bases), list(components))
-    libs_diff = libs.report.calculate_diff(third_party_imports, third_party_libs)
+    return {"brick_imports": brick_imports, "third_party_imports": third_party_imports}
+
+
+def create_report(
+    project_data: dict,
+    collected_imports: dict,
+    third_party_libs: Set,
+    is_strict: bool = False,
+) -> dict:
+    bases = {b for b in project_data.get("bases", [])}
+    components = {c for c in project_data.get("components", [])}
 
-    res = all([not brick_diff, not libs_diff])
+    brick_imports = collected_imports["brick_imports"]
+    third_party_imports = collected_imports["third_party_imports"]
 
-    report_details = {
+    brick_diff = collect.imports_diff(brick_imports, list(bases), list(components))
+    libs_diff = libs.report.calculate_diff(
+        third_party_imports, third_party_libs, is_strict
+    )
+
+    return {
         "brick_imports": brick_imports,
         "third_party_imports": third_party_imports,
         "brick_diff": brick_diff,
         "libs_diff": libs_diff,
     }
-
-    return res, report_details
```

### Comparing `poetry_polylith_plugin-1.8.3/polylith/diff/collect.py` & `poetry_polylith_plugin-1.9.0/polylith/diff/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/diff/report.py` & `poetry_polylith_plugin-1.9.0/polylith/diff/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/imports/parser.py` & `poetry_polylith_plugin-1.9.0/polylith/imports/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/info/__init__.py` & `poetry_polylith_plugin-1.9.0/polylith/info/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/info/collect.py` & `poetry_polylith_plugin-1.9.0/polylith/info/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/info/report.py` & `poetry_polylith_plugin-1.9.0/polylith/info/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/interface/interfaces.py` & `poetry_polylith_plugin-1.9.0/polylith/interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/libs/grouping.py` & `poetry_polylith_plugin-1.9.0/polylith/libs/grouping.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/libs/report.py` & `poetry_polylith_plugin-1.9.0/polylith/libs/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,26 +31,39 @@
 def flatten_brick_imports(brick_imports: dict) -> Set[str]:
     bases_imports = flatten_imports(brick_imports, "bases")
     components_imports = flatten_imports(brick_imports, "components")
 
     return set().union(bases_imports, components_imports)
 
 
-def filter_close_matches(unknown_imports: Set[str], dependencies: Set[str]) -> Set[str]:
+def filter_close_matches(
+    unknown_imports: Set[str], dependencies: Set[str], cutoff: float
+) -> Set[str]:
     unknowns = {str.lower(u) for u in unknown_imports}
     deps = {str.lower(d) for d in dependencies}
 
-    return {u for u in unknowns if not difflib.get_close_matches(u, deps)}
+    return {
+        u for u in unknowns if not difflib.get_close_matches(u, deps, cutoff=cutoff)
+    }
 
 
-def calculate_diff(brick_imports: dict, deps: Set[str]) -> Set[str]:
+def get_unknowns(brick_imports: dict, deps: Set[str]) -> Set[str]:
     imports = flatten_brick_imports(brick_imports)
-    unknown_imports = imports.difference(deps)
 
-    return filter_close_matches(unknown_imports, deps)
+    return imports.difference(deps)
+
+
+def calculate_diff(
+    brick_imports: dict, deps: Set[str], is_strict: bool = False
+) -> Set[str]:
+    unknown_imports = get_unknowns(brick_imports, deps)
+
+    cutoff = 0.6 if not is_strict else 0.9
+
+    return filter_close_matches(unknown_imports, deps, cutoff)
 
 
 def print_libs_summary(brick_imports: dict, project_data: dict) -> None:
     console = Console(theme=theme.poly_theme)
 
     name = project_data["name"]
     is_project = info.is_project(project_data)
@@ -91,17 +104,17 @@
     for brick, imports in components.items():
         table.add_row(f"[comp]{brick}[/]", ", ".join(sorted(imports)))
 
     console.print(table, overflow="ellipsis")
 
 
 def print_missing_installed_libs(
-    brick_imports: dict, third_party_libs: Set[str], project_name: str
+    brick_imports: dict, third_party_libs: Set[str], project_name: str, is_strict: bool = False
 ) -> bool:
-    diff = calculate_diff(brick_imports, third_party_libs)
+    diff = calculate_diff(brick_imports, third_party_libs, is_strict)
 
     if not diff:
         return True
 
     console = Console(theme=theme.poly_theme)
 
     missing = ", ".join(sorted(diff))
```

### Comparing `poetry_polylith_plugin-1.8.3/polylith/libs/stdlib.py` & `poetry_polylith_plugin-1.9.0/polylith/libs/stdlib.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/poetry/commands/__init__.py` & `poetry_polylith_plugin-1.9.0/polylith/poetry/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/poetry/commands/check.py` & `poetry_polylith_plugin-1.9.0/polylith/poetry/commands/sync.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,63 @@
 from pathlib import Path
-from typing import Set, Union
+from typing import List
 
 from poetry.console.commands.command import Command
-from poetry.factory import Factory
-from polylith import check, info, project, repo, workspace
+from polylith import info, project, repo, sync, workspace
 
 
-class CheckCommand(Command):
-    name = "poly check"
-    description = "Validates the <comment>Polylith</> workspace."
+class SyncCommand(Command):
+    name = "poly sync"
+    description = "Update <comment>pyproject.toml</comment> with missing bricks."
 
-    def find_third_party_libs(self, path: Union[Path, None]) -> Set:
-        project_poetry = Factory().create_poetry(path) if path else self.poetry
-
-        if not project_poetry.locker.is_locked():
-            raise ValueError("poetry.lock not found. Run `poetry lock` to create it.")
-
-        packages = project_poetry.locker.locked_repository().packages
-
-        return {p.name for p in packages}
-
-    def print_report(self, root: Path, ns: str, project_data: dict) -> bool:
-        is_verbose = self.option("verbose")
-        is_quiet = self.option("quiet")
-
-        path = project_data["path"]
-        name = project_data["name"]
+    def filter_projects_data(self, all_projects_data: List[dict]) -> List[dict]:
+        if self.option("directory"):
+            project_name = project.get_project_name(self.poetry.pyproject.data)
 
-        try:
-            third_party_libs = self.find_third_party_libs(path)
-            res, details = check.report.create_report(
-                root,
-                ns,
-                project_data,
-                third_party_libs,
+            data = next(
+                (p for p in all_projects_data if p["name"] == project_name), None
             )
 
-            if is_quiet:
-                return res
-
-            check.report.print_missing_deps(details["brick_diff"], name)
-            check.report.print_missing_deps(details["libs_diff"], name)
+            if not data:
+                raise ValueError(f"Didn't find project in {self.option('directory')}")
 
-            if is_verbose:
-                check.report.print_brick_imports(details["brick_imports"])
-                check.report.print_brick_imports(details["third_party_imports"])
+            return [data]
 
-            return res
-        except ValueError as e:
-            self.line_error(f"{name}: <error>{e}</error>")
-            return False
+        return all_projects_data
 
     def handle(self) -> int:
+        is_verbose = self.option("verbose")
+        is_quiet = self.option("quiet")
+
         root = repo.find_workspace_root(Path.cwd())
 
         if not root:
             raise ValueError(
                 "Didn't find the workspace root. Expected to find a workspace.toml file."
             )
 
         ns = workspace.parser.get_namespace_from_config(root)
 
-        all_projects_data = info.get_projects_data(root, ns)
-        projects_data = [p for p in all_projects_data if info.is_project(p)]
-
-        if self.option("directory"):
-            project_name = project.get_project_name(self.poetry.pyproject.data)
+        bases = info.get_bases(root, ns)
+        components = info.get_components(root, ns)
+        workspace_data = {"bases": bases, "components": components}
+
+        all_projects_data = info.get_bricks_in_projects(root, components, bases, ns)
+        projects_data = self.filter_projects_data(all_projects_data)
+
+        diffs = [
+            sync.calculate_diff(root, ns, data, workspace_data)
+            for data in projects_data
+        ]
 
-            data = next((p for p in projects_data if p["name"] == project_name), None)
+        for diff in diffs:
+            sync.update_project(root, ns, diff)
 
-            if not data:
-                raise ValueError(f"Didn't find project in {self.option('directory')}")
+            if is_quiet:
+                continue
 
-            res = self.print_report(root, ns, data)
-            result_code = 0 if res else 1
-        else:
-            results = {self.print_report(root, ns, data) for data in projects_data}
+            sync.report.print_summary(diff)
 
-            result_code = 0 if all(results) else 1
+            if is_verbose:
+                sync.report.print_brick_imports(diff)
 
-        return result_code
+        return 0
```

### Comparing `poetry_polylith_plugin-1.8.3/polylith/poetry/commands/create.py` & `poetry_polylith_plugin-1.9.0/polylith/poetry/commands/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/poetry/commands/create_base.py` & `poetry_polylith_plugin-1.9.0/polylith/poetry/commands/create_base.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/poetry/commands/create_component.py` & `poetry_polylith_plugin-1.9.0/polylith/poetry/commands/create_component.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/poetry/commands/create_project.py` & `poetry_polylith_plugin-1.9.0/polylith/poetry/commands/create_project.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/poetry/commands/create_workspace.py` & `poetry_polylith_plugin-1.9.0/polylith/poetry/commands/create_workspace.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/poetry/commands/diff.py` & `poetry_polylith_plugin-1.9.0/polylith/poetry/commands/diff.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/poetry/commands/info.py` & `poetry_polylith_plugin-1.9.0/polylith/poetry/commands/info.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/poetry/commands/libs.py` & `poetry_polylith_plugin-1.9.0/polylith/poetry/commands/libs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from pathlib import Path
-from typing import Set, Union
 
 from poetry.console.commands.command import Command
-from poetry.factory import Factory
-from polylith import info, project, repo, workspace
+from polylith import alias, info, project, repo, workspace
 from polylith.libs import report
+from polylith.poetry.commands.check import command_options, find_third_party_libs
 
 
 class LibsCommand(Command):
     name = "poly libs"
     description = "Show third-party libraries used in the workspace."
 
-    def find_third_party_libs(self, path: Union[Path, None]) -> Set:
-        project_poetry = Factory().create_poetry(path) if path else self.poetry
-
-        if not project_poetry.locker.is_locked():
-            raise ValueError("poetry.lock not found. Run `poetry lock` to create it.")
-
-        packages = project_poetry.locker.locked_repository().packages
-
-        return {p.name for p in packages}
+    options = command_options
 
     def print_report(self, root: Path, ns: str, data: dict) -> bool:
+        is_strict = self.option("strict")
+
         name = data["name"]
         path = data["path"]
 
         brick_imports = report.get_third_party_imports(root, ns, data)
 
         report.print_libs_summary(brick_imports, data)
         report.print_libs_in_bricks(brick_imports)
 
         try:
-            third_party_libs = self.find_third_party_libs(path)
+            third_party_libs = find_third_party_libs(self.poetry, path)
+
+            library_aliases = alias.parse(self.option("alias"))
+            extra = alias.pick(library_aliases, third_party_libs)
+
+            libs = third_party_libs.union(extra)
 
             return report.print_missing_installed_libs(
-                brick_imports, third_party_libs, name
+                brick_imports,
+                libs,
+                name,
+                is_strict,
             )
         except ValueError as e:
             self.line_error(f"{name}: <error>{e}</error>")
             return False
 
     def handle(self) -> int:
         root = repo.find_workspace_root(Path.cwd())
```

### Comparing `poetry_polylith_plugin-1.8.3/polylith/poetry_plugin/plugin.py` & `poetry_polylith_plugin-1.9.0/polylith/poetry_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/project/create.py` & `poetry_polylith_plugin-1.9.0/polylith/project/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/project/get.py` & `poetry_polylith_plugin-1.9.0/polylith/project/get.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/readme/readme.py` & `poetry_polylith_plugin-1.9.0/polylith/readme/readme.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/repo/repo.py` & `poetry_polylith_plugin-1.9.0/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/sync/collect.py` & `poetry_polylith_plugin-1.9.0/polylith/sync/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/sync/report.py` & `poetry_polylith_plugin-1.9.0/polylith/sync/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/sync/update.py` & `poetry_polylith_plugin-1.9.0/polylith/sync/update.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/test/tests.py` & `poetry_polylith_plugin-1.9.0/polylith/test/tests.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/workspace/create.py` & `poetry_polylith_plugin-1.9.0/polylith/workspace/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/workspace/parser.py` & `poetry_polylith_plugin-1.9.0/polylith/workspace/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/polylith/workspace/paths.py` & `poetry_polylith_plugin-1.9.0/polylith/workspace/paths.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.3/pyproject.toml` & `poetry_polylith_plugin-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-polylith-plugin"
-version = "1.8.3"
+version = "1.9.0"
 description = "A Poetry plugin that adds tooling support for the Polylith Architecture"
 authors = ["David Vujic"]
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 readme = "README.md"
 packages = [
     {include = "polylith"},
```

### Comparing `poetry_polylith_plugin-1.8.3/PKG-INFO` & `poetry_polylith_plugin-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-polylith-plugin
-Version: 1.8.3
+Version: 1.9.0
 Summary: A Poetry plugin that adds tooling support for the Polylith Architecture
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 Author: David Vujic
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

