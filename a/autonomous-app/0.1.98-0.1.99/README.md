# Comparing `tmp/autonomous-app-0.1.98.tar.gz` & `tmp/autonomous-app-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomous-app-0.1.98.tar", last modified: Mon Dec 18 17:25:45 2023, max compression
+gzip compressed data, was "autonomous-app-0.1.99.tar", last modified: Mon Dec 18 19:30:00 2023, max compression
```

## Comparing `autonomous-app-0.1.98.tar` & `autonomous-app-0.1.99.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.533479 autonomous-app-0.1.98/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-03-07 12:36:40.000000 autonomous-app-0.1.98/LICENSE
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4293 2023-12-18 17:25:45.532479 autonomous-app-0.1.98/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2012 2023-08-02 17:40:38.000000 autonomous-app-0.1.98/README.md
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1469 2023-07-20 14:57:42.000000 autonomous-app-0.1.98/pyproject.toml
--rw-r--r--   0 samoore   (1000) samoore   (1000)      536 2023-12-18 15:47:18.000000 autonomous-app-0.1.98/requirements.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-12-18 17:25:45.533479 autonomous-app-0.1.98/setup.cfg
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-04-04 14:14:59.000000 autonomous-app-0.1.98/setup.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.512479 autonomous-app-0.1.98/src/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.515479 autonomous-app-0.1.98/src/autonomous/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       87 2023-12-18 17:24:26.000000 autonomous-app-0.1.98/src/autonomous/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.516479 autonomous-app-0.1.98/src/autonomous/ai/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       31 2023-11-11 17:40:30.000000 autonomous-app-0.1.98/src/autonomous/ai/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.517479 autonomous-app-0.1.98/src/autonomous/ai/agents/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3767 2023-11-25 02:11:35.000000 autonomous-app-0.1.98/src/autonomous/ai/agents/autogen.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      442 2023-11-21 17:15:45.000000 autonomous-app-0.1.98/src/autonomous/ai/agents/baseagent.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1681 2023-11-25 02:14:34.000000 autonomous-app-0.1.98/src/autonomous/ai/agents/local.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1535 2023-11-21 18:06:03.000000 autonomous-app-0.1.98/src/autonomous/ai/agents/mockai.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4041 2023-11-21 17:36:18.000000 autonomous-app-0.1.98/src/autonomous/ai/agents/openai.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1255 2023-12-02 03:55:36.000000 autonomous-app-0.1.98/src/autonomous/ai/autoteam.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.518479 autonomous-app-0.1.98/src/autonomous/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-10-27 15:43:10.000000 autonomous-app-0.1.98/src/autonomous/apis/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.519479 autonomous-app-0.1.98/src/autonomous/apis/version_control/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-03-07 16:24:11.000000 autonomous-app-0.1.98/src/autonomous/apis/version_control/GHCallbacks.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-03-07 21:09:26.000000 autonomous-app-0.1.98/src/autonomous/apis/version_control/GHOrganization.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-03-07 16:24:11.000000 autonomous-app-0.1.98/src/autonomous/apis/version_control/GHRepo.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-03-07 16:24:11.000000 autonomous-app-0.1.98/src/autonomous/apis/version_control/GHVersionControl.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-03-07 16:24:11.000000 autonomous-app-0.1.98/src/autonomous/apis/version_control/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.520479 autonomous-app-0.1.98/src/autonomous/apis/wikijs/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       24 2023-09-17 14:05:05.000000 autonomous-app-0.1.98/src/autonomous/apis/wikijs/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     7803 2023-12-05 17:36:34.000000 autonomous-app-0.1.98/src/autonomous/apis/wikijs/api.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      699 2023-11-12 04:29:55.000000 autonomous-app-0.1.98/src/autonomous/apis/wikijs/page.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.511479 autonomous-app-0.1.98/src/autonomous/app_template/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.521479 autonomous-app-0.1.98/src/autonomous/app_template/app/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       54 2023-07-28 15:13:30.000000 autonomous-app-0.1.98/src/autonomous/app_template/app/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      941 2023-10-31 13:06:19.000000 autonomous-app-0.1.98/src/autonomous/app_template/app/api.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1634 2023-10-31 13:53:35.000000 autonomous-app-0.1.98/src/autonomous/app_template/app/app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      795 2023-10-31 13:04:04.000000 autonomous-app-0.1.98/src/autonomous/app_template/app/config.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.522479 autonomous-app-0.1.98/src/autonomous/app_template/app/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-04-04 14:32:12.000000 autonomous-app-0.1.98/src/autonomous/app_template/app/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      239 2023-11-02 16:15:57.000000 autonomous-app-0.1.98/src/autonomous/app_template/app/models/model.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      548 2023-10-31 13:57:31.000000 autonomous-app-0.1.98/src/autonomous/app_template/app/tasks.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.523479 autonomous-app-0.1.98/src/autonomous/app_template/app/views/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-10-31 13:02:03.000000 autonomous-app-0.1.98/src/autonomous/app_template/app/views/__init__.py
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      384 2023-10-31 13:03:32.000000 autonomous-app-0.1.98/src/autonomous/app_template/app/views/admin.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.523479 autonomous-app-0.1.98/src/autonomous/app_template/app/views/api/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-10-31 13:02:03.000000 autonomous-app-0.1.98/src/autonomous/app_template/app/views/api/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      464 2023-10-31 13:02:03.000000 autonomous-app-0.1.98/src/autonomous/app_template/app/views/api/task.py
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)     2248 2023-11-03 17:59:06.000000 autonomous-app-0.1.98/src/autonomous/app_template/app/views/auth.py
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      657 2023-11-25 02:27:16.000000 autonomous-app-0.1.98/src/autonomous/app_template/app/views/index.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.524479 autonomous-app-0.1.98/src/autonomous/app_template/tests/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-04 14:32:12.000000 autonomous-app-0.1.98/src/autonomous/app_template/tests/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      545 2023-07-28 15:11:47.000000 autonomous-app-0.1.98/src/autonomous/app_template/tests/conftest.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      225 2023-11-08 20:35:25.000000 autonomous-app-0.1.98/src/autonomous/app_template/tests/test_app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      964 2023-11-08 21:07:18.000000 autonomous-app-0.1.98/src/autonomous/app_template/tests/test_auth.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2467 2023-10-31 13:57:41.000000 autonomous-app-0.1.98/src/autonomous/app_template/tests/test_tasks.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.525479 autonomous-app-0.1.98/src/autonomous/app_template/vendor/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1132 2023-10-06 16:58:12.000000 autonomous-app-0.1.98/src/autonomous/app_template/vendor/gunicorn.conf.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2080 2023-12-02 03:44:55.000000 autonomous-app-0.1.98/src/autonomous/assets.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.526479 autonomous-app-0.1.98/src/autonomous/auth/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      161 2023-10-30 19:07:42.000000 autonomous-app-0.1.98/src/autonomous/auth/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3299 2023-12-16 21:28:15.000000 autonomous-app-0.1.98/src/autonomous/auth/autoauth.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      886 2023-10-08 14:52:15.000000 autonomous-app-0.1.98/src/autonomous/auth/github.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1049 2023-10-06 19:49:20.000000 autonomous-app-0.1.98/src/autonomous/auth/google.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2153 2023-12-16 21:30:14.000000 autonomous-app-0.1.98/src/autonomous/auth/user.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-04-04 14:14:59.000000 autonomous-app-0.1.98/src/autonomous/cli.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.526479 autonomous-app-0.1.98/src/autonomous/db/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-11-07 17:04:09.000000 autonomous-app-0.1.98/src/autonomous/db/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1485 2023-11-07 17:04:09.000000 autonomous-app-0.1.98/src/autonomous/db/autodb.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     7609 2023-11-30 18:58:13.000000 autonomous-app-0.1.98/src/autonomous/db/table.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1460 2023-11-13 19:36:43.000000 autonomous-app-0.1.98/src/autonomous/logger.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.527479 autonomous-app-0.1.98/src/autonomous/model/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-11-02 16:21:48.000000 autonomous-app-0.1.98/src/autonomous/model/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      586 2023-11-07 17:04:09.000000 autonomous-app-0.1.98/src/autonomous/model/autoattribute.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)    12318 2023-12-08 19:50:29.000000 autonomous-app-0.1.98/src/autonomous/model/automodel.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      733 2023-11-22 00:01:47.000000 autonomous-app-0.1.98/src/autonomous/model/orm.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.529479 autonomous-app-0.1.98/src/autonomous/storage/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       49 2023-09-09 15:30:58.000000 autonomous-app-0.1.98/src/autonomous/storage/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2350 2023-12-12 17:00:48.000000 autonomous-app-0.1.98/src/autonomous/storage/cloudinarystorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3124 2023-12-18 17:20:21.000000 autonomous-app-0.1.98/src/autonomous/storage/imagestorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2286 2023-12-18 15:10:22.000000 autonomous-app-0.1.98/src/autonomous/storage/localstorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3885 2023-11-29 14:43:31.000000 autonomous-app-0.1.98/src/autonomous/storage/markdown.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.529479 autonomous-app-0.1.98/src/autonomous/tasks/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       32 2023-08-25 19:55:23.000000 autonomous-app-0.1.98/src/autonomous/tasks/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4379 2023-11-17 16:47:39.000000 autonomous-app-0.1.98/src/autonomous/tasks/autotask.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 17:25:45.531479 autonomous-app-0.1.98/src/autonomous_app.egg-info/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4293 2023-12-18 17:25:45.000000 autonomous-app-0.1.98/src/autonomous_app.egg-info/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2555 2023-12-18 17:25:45.000000 autonomous-app-0.1.98/src/autonomous_app.egg-info/SOURCES.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-12-18 17:25:45.000000 autonomous-app-0.1.98/src/autonomous_app.egg-info/dependency_links.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       53 2023-12-18 17:25:45.000000 autonomous-app-0.1.98/src/autonomous_app.egg-info/entry_points.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)      182 2023-12-18 17:25:45.000000 autonomous-app-0.1.98/src/autonomous_app.egg-info/requires.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       11 2023-12-18 17:25:45.000000 autonomous-app-0.1.98/src/autonomous_app.egg-info/top_level.txt
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.153805 autonomous-app-0.1.99/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-03-07 12:36:40.000000 autonomous-app-0.1.99/LICENSE
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4293 2023-12-18 19:30:00.152805 autonomous-app-0.1.99/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2012 2023-08-02 17:40:38.000000 autonomous-app-0.1.99/README.md
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1469 2023-07-20 14:57:42.000000 autonomous-app-0.1.99/pyproject.toml
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      536 2023-12-18 15:47:18.000000 autonomous-app-0.1.99/requirements.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-12-18 19:30:00.153805 autonomous-app-0.1.99/setup.cfg
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-04-04 14:14:59.000000 autonomous-app-0.1.99/setup.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.130805 autonomous-app-0.1.99/src/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.134805 autonomous-app-0.1.99/src/autonomous/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       87 2023-12-18 19:26:51.000000 autonomous-app-0.1.99/src/autonomous/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.135805 autonomous-app-0.1.99/src/autonomous/ai/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       31 2023-11-11 17:40:30.000000 autonomous-app-0.1.99/src/autonomous/ai/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.137805 autonomous-app-0.1.99/src/autonomous/ai/agents/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3767 2023-11-25 02:11:35.000000 autonomous-app-0.1.99/src/autonomous/ai/agents/autogen.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      442 2023-11-21 17:15:45.000000 autonomous-app-0.1.99/src/autonomous/ai/agents/baseagent.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1681 2023-11-25 02:14:34.000000 autonomous-app-0.1.99/src/autonomous/ai/agents/local.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1535 2023-11-21 18:06:03.000000 autonomous-app-0.1.99/src/autonomous/ai/agents/mockai.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4041 2023-11-21 17:36:18.000000 autonomous-app-0.1.99/src/autonomous/ai/agents/openai.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1255 2023-12-02 03:55:36.000000 autonomous-app-0.1.99/src/autonomous/ai/autoteam.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.137805 autonomous-app-0.1.99/src/autonomous/apis/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-10-27 15:43:10.000000 autonomous-app-0.1.99/src/autonomous/apis/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.139805 autonomous-app-0.1.99/src/autonomous/apis/version_control/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-03-07 16:24:11.000000 autonomous-app-0.1.99/src/autonomous/apis/version_control/GHCallbacks.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-03-07 21:09:26.000000 autonomous-app-0.1.99/src/autonomous/apis/version_control/GHOrganization.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-03-07 16:24:11.000000 autonomous-app-0.1.99/src/autonomous/apis/version_control/GHRepo.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-03-07 16:24:11.000000 autonomous-app-0.1.99/src/autonomous/apis/version_control/GHVersionControl.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-03-07 16:24:11.000000 autonomous-app-0.1.99/src/autonomous/apis/version_control/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.140805 autonomous-app-0.1.99/src/autonomous/apis/wikijs/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       24 2023-09-17 14:05:05.000000 autonomous-app-0.1.99/src/autonomous/apis/wikijs/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     7803 2023-12-05 17:36:34.000000 autonomous-app-0.1.99/src/autonomous/apis/wikijs/api.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      699 2023-11-12 04:29:55.000000 autonomous-app-0.1.99/src/autonomous/apis/wikijs/page.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.129805 autonomous-app-0.1.99/src/autonomous/app_template/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.141805 autonomous-app-0.1.99/src/autonomous/app_template/app/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       54 2023-07-28 15:13:30.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      941 2023-10-31 13:06:19.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/api.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1634 2023-10-31 13:53:35.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/app.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      795 2023-10-31 13:04:04.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/config.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.142805 autonomous-app-0.1.99/src/autonomous/app_template/app/models/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-04-04 14:32:12.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/models/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      239 2023-11-02 16:15:57.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/models/model.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      548 2023-10-31 13:57:31.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/tasks.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.143805 autonomous-app-0.1.99/src/autonomous/app_template/app/views/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-10-31 13:02:03.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/views/__init__.py
+-rwxr-xr-x   0 samoore   (1000) samoore   (1000)      384 2023-10-31 13:03:32.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/views/admin.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.143805 autonomous-app-0.1.99/src/autonomous/app_template/app/views/api/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-10-31 13:02:03.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/views/api/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      464 2023-10-31 13:02:03.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/views/api/task.py
+-rwxr-xr-x   0 samoore   (1000) samoore   (1000)     2248 2023-11-03 17:59:06.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/views/auth.py
+-rwxr-xr-x   0 samoore   (1000) samoore   (1000)      657 2023-11-25 02:27:16.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/views/index.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.144805 autonomous-app-0.1.99/src/autonomous/app_template/tests/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-04 14:32:12.000000 autonomous-app-0.1.99/src/autonomous/app_template/tests/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      545 2023-07-28 15:11:47.000000 autonomous-app-0.1.99/src/autonomous/app_template/tests/conftest.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      225 2023-11-08 20:35:25.000000 autonomous-app-0.1.99/src/autonomous/app_template/tests/test_app.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      964 2023-11-08 21:07:18.000000 autonomous-app-0.1.99/src/autonomous/app_template/tests/test_auth.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2467 2023-10-31 13:57:41.000000 autonomous-app-0.1.99/src/autonomous/app_template/tests/test_tasks.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.145805 autonomous-app-0.1.99/src/autonomous/app_template/vendor/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1132 2023-10-06 16:58:12.000000 autonomous-app-0.1.99/src/autonomous/app_template/vendor/gunicorn.conf.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2080 2023-12-02 03:44:55.000000 autonomous-app-0.1.99/src/autonomous/assets.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.146805 autonomous-app-0.1.99/src/autonomous/auth/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      161 2023-10-30 19:07:42.000000 autonomous-app-0.1.99/src/autonomous/auth/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3299 2023-12-16 21:28:15.000000 autonomous-app-0.1.99/src/autonomous/auth/autoauth.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      886 2023-10-08 14:52:15.000000 autonomous-app-0.1.99/src/autonomous/auth/github.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1049 2023-10-06 19:49:20.000000 autonomous-app-0.1.99/src/autonomous/auth/google.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2153 2023-12-16 21:30:14.000000 autonomous-app-0.1.99/src/autonomous/auth/user.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-04-04 14:14:59.000000 autonomous-app-0.1.99/src/autonomous/cli.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.146805 autonomous-app-0.1.99/src/autonomous/db/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-11-07 17:04:09.000000 autonomous-app-0.1.99/src/autonomous/db/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1485 2023-11-07 17:04:09.000000 autonomous-app-0.1.99/src/autonomous/db/autodb.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     7609 2023-11-30 18:58:13.000000 autonomous-app-0.1.99/src/autonomous/db/table.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1460 2023-11-13 19:36:43.000000 autonomous-app-0.1.99/src/autonomous/logger.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.147805 autonomous-app-0.1.99/src/autonomous/model/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-11-02 16:21:48.000000 autonomous-app-0.1.99/src/autonomous/model/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      586 2023-11-07 17:04:09.000000 autonomous-app-0.1.99/src/autonomous/model/autoattribute.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)    12318 2023-12-08 19:50:29.000000 autonomous-app-0.1.99/src/autonomous/model/automodel.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      733 2023-11-22 00:01:47.000000 autonomous-app-0.1.99/src/autonomous/model/orm.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.149805 autonomous-app-0.1.99/src/autonomous/storage/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       49 2023-09-09 15:30:58.000000 autonomous-app-0.1.99/src/autonomous/storage/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2350 2023-12-12 17:00:48.000000 autonomous-app-0.1.99/src/autonomous/storage/cloudinarystorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2815 2023-12-18 19:24:04.000000 autonomous-app-0.1.99/src/autonomous/storage/imagestorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2286 2023-12-18 15:10:22.000000 autonomous-app-0.1.99/src/autonomous/storage/localstorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3885 2023-11-29 14:43:31.000000 autonomous-app-0.1.99/src/autonomous/storage/markdown.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.149805 autonomous-app-0.1.99/src/autonomous/tasks/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       32 2023-08-25 19:55:23.000000 autonomous-app-0.1.99/src/autonomous/tasks/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4379 2023-11-17 16:47:39.000000 autonomous-app-0.1.99/src/autonomous/tasks/autotask.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.151805 autonomous-app-0.1.99/src/autonomous_app.egg-info/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4293 2023-12-18 19:30:00.000000 autonomous-app-0.1.99/src/autonomous_app.egg-info/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2555 2023-12-18 19:30:00.000000 autonomous-app-0.1.99/src/autonomous_app.egg-info/SOURCES.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-12-18 19:30:00.000000 autonomous-app-0.1.99/src/autonomous_app.egg-info/dependency_links.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       53 2023-12-18 19:30:00.000000 autonomous-app-0.1.99/src/autonomous_app.egg-info/entry_points.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      182 2023-12-18 19:30:00.000000 autonomous-app-0.1.99/src/autonomous_app.egg-info/requires.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       11 2023-12-18 19:30:00.000000 autonomous-app-0.1.99/src/autonomous_app.egg-info/top_level.txt
```

### Comparing `autonomous-app-0.1.98/LICENSE` & `autonomous-app-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/PKG-INFO` & `autonomous-app-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.98
+Version: 0.1.99
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous-app-0.1.98/README.md` & `autonomous-app-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/pyproject.toml` & `autonomous-app-0.1.99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/requirements.txt` & `autonomous-app-0.1.99/requirements.txt`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/ai/agents/autogen.py` & `autonomous-app-0.1.99/src/autonomous/ai/agents/autogen.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/ai/agents/local.py` & `autonomous-app-0.1.99/src/autonomous/ai/agents/local.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/ai/agents/mockai.py` & `autonomous-app-0.1.99/src/autonomous/ai/agents/mockai.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/ai/agents/openai.py` & `autonomous-app-0.1.99/src/autonomous/ai/agents/openai.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/ai/autoteam.py` & `autonomous-app-0.1.99/src/autonomous/ai/autoteam.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/apis/version_control/GHCallbacks.py` & `autonomous-app-0.1.99/src/autonomous/apis/version_control/GHCallbacks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/apis/version_control/GHOrganization.py` & `autonomous-app-0.1.99/src/autonomous/apis/version_control/GHOrganization.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/apis/version_control/GHRepo.py` & `autonomous-app-0.1.99/src/autonomous/apis/version_control/GHRepo.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/apis/wikijs/api.py` & `autonomous-app-0.1.99/src/autonomous/apis/wikijs/api.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/apis/wikijs/page.py` & `autonomous-app-0.1.99/src/autonomous/apis/wikijs/page.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/app_template/app/api.py` & `autonomous-app-0.1.99/src/autonomous/app_template/app/api.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/app_template/app/app.py` & `autonomous-app-0.1.99/src/autonomous/app_template/app/app.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/app_template/app/config.py` & `autonomous-app-0.1.99/src/autonomous/app_template/app/config.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/app_template/app/tasks.py` & `autonomous-app-0.1.99/src/autonomous/app_template/app/tasks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/app_template/app/views/auth.py` & `autonomous-app-0.1.99/src/autonomous/app_template/app/views/auth.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/app_template/app/views/index.py` & `autonomous-app-0.1.99/src/autonomous/app_template/app/views/index.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/app_template/tests/conftest.py` & `autonomous-app-0.1.99/src/autonomous/app_template/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/app_template/tests/test_auth.py` & `autonomous-app-0.1.99/src/autonomous/app_template/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/app_template/tests/test_tasks.py` & `autonomous-app-0.1.99/src/autonomous/app_template/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/app_template/vendor/gunicorn.conf.py` & `autonomous-app-0.1.99/src/autonomous/app_template/vendor/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/assets.py` & `autonomous-app-0.1.99/src/autonomous/assets.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/auth/autoauth.py` & `autonomous-app-0.1.99/src/autonomous/auth/autoauth.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/auth/github.py` & `autonomous-app-0.1.99/src/autonomous/auth/github.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/auth/google.py` & `autonomous-app-0.1.99/src/autonomous/auth/google.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/auth/user.py` & `autonomous-app-0.1.99/src/autonomous/auth/user.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/db/autodb.py` & `autonomous-app-0.1.99/src/autonomous/db/autodb.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/db/table.py` & `autonomous-app-0.1.99/src/autonomous/db/table.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/logger.py` & `autonomous-app-0.1.99/src/autonomous/logger.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/model/autoattribute.py` & `autonomous-app-0.1.99/src/autonomous/model/autoattribute.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/model/automodel.py` & `autonomous-app-0.1.99/src/autonomous/model/automodel.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/model/orm.py` & `autonomous-app-0.1.99/src/autonomous/model/orm.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/storage/cloudinarystorage.py` & `autonomous-app-0.1.99/src/autonomous/storage/cloudinarystorage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/storage/imagestorage.py` & `autonomous-app-0.1.99/src/autonomous/storage/imagestorage.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,22 +22,16 @@
             return f"{uuid.uuid4()}.{image_type}"
 
     def _resize_image(self, asset_id, max_size):
         img_type = self.get_img_type(asset_id)
         file_path = f"{self.get_path(asset_id)}/orig.{img_type}"
         with Image.open(file_path) as img:
             max_size = self._sizes.get(max_size) or int(max_size)
-            # Calculate new dimensions while maintaining aspect ratio
-            width, height = img.size
-            new_width = new_height = max_size
-            if width > height:
-                new_height = int((max_size / width) * height)
-            else:
-                new_width = int((max_size / height) * width)
-            resized_img = img.resize((new_width, new_height), Image.LANCZOS)
+            resized_img = img.copy()
+            resized_img.thumbnail((max_size, max_size))
             img_byte_arr = io.BytesIO()
             resized_img.save(img_byte_arr, format="WEBP")
             return img_byte_arr.getvalue()
 
     def save(self, file, image_type="webp", folder=""):
         asset_id = self._create_key(folder, image_type)
         os.makedirs(self.get_path(asset_id), exist_ok=True)
```

### Comparing `autonomous-app-0.1.98/src/autonomous/storage/localstorage.py` & `autonomous-app-0.1.99/src/autonomous/storage/localstorage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/storage/markdown.py` & `autonomous-app-0.1.99/src/autonomous/storage/markdown.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous/tasks/autotask.py` & `autonomous-app-0.1.99/src/autonomous/tasks/autotask.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.98/src/autonomous_app.egg-info/PKG-INFO` & `autonomous-app-0.1.99/src/autonomous_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.98
+Version: 0.1.99
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous-app-0.1.98/src/autonomous_app.egg-info/SOURCES.txt` & `autonomous-app-0.1.99/src/autonomous_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

