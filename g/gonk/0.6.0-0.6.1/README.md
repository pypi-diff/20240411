# Comparing `tmp/gonk-0.6.0.tar.gz` & `tmp/gonk-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gonk-0.6.0.tar", max compression
+gzip compressed data, was "gonk-0.6.1.tar", max compression
```

## Comparing `gonk-0.6.0.tar` & `gonk-0.6.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1524 2024-04-09 14:59:18.441874 gonk-0.6.0/LICENSE
--rw-r--r--   0        0        0     5355 2024-04-09 14:59:18.441874 gonk-0.6.0/README.md
--rw-r--r--   0        0        0        0 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/__init__.py
--rw-r--r--   0        0        0      141 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/apps.py
--rw-r--r--   0        0        0      305 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/beat.py
--rw-r--r--   0        0        0        0 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/expiration/__init__.py
--rw-r--r--   0        0        0      331 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/expiration/mixins.py
--rw-r--r--   0        0        0        0 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/notifications/__init__.py
--rw-r--r--   0        0        0     2184 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/notifications/mercure.py
--rw-r--r--   0        0        0      235 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/notifications/settings.py
--rw-r--r--   0        0        0        0 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/persistance/__init__.py
--rw-r--r--   0        0        0      544 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/persistance/beat.py
--rw-r--r--   0        0        0        0 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/rest_framework/__init__.py
--rw-r--r--   0        0        0      178 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/rest_framework/exceptions.py
--rw-r--r--   0        0        0      788 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/rest_framework/permissions.py
--rw-r--r--   0        0        0     1403 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/rest_framework/serializers.py
--rw-r--r--   0        0        0      231 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/rest_framework/urls.py
--rw-r--r--   0        0        0     3048 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/contrib/rest_framework/viewsets.py
--rw-r--r--   0        0        0      371 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/decorators.py
--rw-r--r--   0        0        0       57 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/management/commands/__init__.py
--rw-r--r--   0        0        0     1861 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/management/commands/create_task.py
--rw-r--r--   0        0        0      387 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/management/commands/list_taskrunners.py
--rw-r--r--   0        0        0     1922 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/migrations/0001_initial.py
--rw-r--r--   0        0        0     1313 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/migrations/0002_auto_20220926_1514.py
--rw-r--r--   0        0        0      445 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/migrations/0003_alter_task_retry_time.py
--rw-r--r--   0        0        0      392 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/migrations/0004_task_with_warnings.py
--rw-r--r--   0        0        0        0 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/migrations/__init__.py
--rw-r--r--   0        0        0     5044 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/models.py
--rw-r--r--   0        0        0      480 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/registry.py
--rw-r--r--   0        0        0     1085 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/settings.py
--rw-r--r--   0        0        0      860 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/taskrunners.py
--rw-r--r--   0        0        0     2374 2024-04-09 14:59:18.441874 gonk-0.6.0/gonk/tasks.py
--rw-r--r--   0        0        0     1394 2024-04-09 14:59:18.441874 gonk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6761 1970-01-01 00:00:00.000000 gonk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1524 2024-04-11 08:45:05.774955 gonk-0.6.1/LICENSE
+-rw-r--r--   0        0        0     5355 2024-04-11 08:45:05.774955 gonk-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/__init__.py
+-rw-r--r--   0        0        0      141 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/apps.py
+-rw-r--r--   0        0        0      305 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/beat.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/expiration/__init__.py
+-rw-r--r--   0        0        0      331 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/expiration/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/notifications/__init__.py
+-rw-r--r--   0        0        0     2184 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/notifications/mercure.py
+-rw-r--r--   0        0        0      235 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/notifications/settings.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/persistance/__init__.py
+-rw-r--r--   0        0        0      544 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/persistance/beat.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/rest_framework/__init__.py
+-rw-r--r--   0        0        0      178 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/rest_framework/exceptions.py
+-rw-r--r--   0        0        0      788 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/rest_framework/permissions.py
+-rw-r--r--   0        0        0     1432 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/rest_framework/serializers.py
+-rw-r--r--   0        0        0      231 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/rest_framework/urls.py
+-rw-r--r--   0        0        0     3048 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/contrib/rest_framework/viewsets.py
+-rw-r--r--   0        0        0      371 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/decorators.py
+-rw-r--r--   0        0        0       57 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/management/commands/__init__.py
+-rw-r--r--   0        0        0     1861 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/management/commands/create_task.py
+-rw-r--r--   0        0        0      387 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/management/commands/list_taskrunners.py
+-rw-r--r--   0        0        0     1922 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1313 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/migrations/0002_auto_20220926_1514.py
+-rw-r--r--   0        0        0      445 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/migrations/0003_alter_task_retry_time.py
+-rw-r--r--   0        0        0      392 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/migrations/0004_task_with_warnings.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/migrations/__init__.py
+-rw-r--r--   0        0        0     5044 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/models.py
+-rw-r--r--   0        0        0      480 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/registry.py
+-rw-r--r--   0        0        0     1085 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/settings.py
+-rw-r--r--   0        0        0      860 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/taskrunners.py
+-rw-r--r--   0        0        0     2374 2024-04-11 08:45:05.774955 gonk-0.6.1/gonk/tasks.py
+-rw-r--r--   0        0        0     1394 2024-04-11 08:45:05.774955 gonk-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6761 1970-01-01 00:00:00.000000 gonk-0.6.1/PKG-INFO
```

### Comparing `gonk-0.6.0/LICENSE` & `gonk-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gonk-0.6.0/README.md` & `gonk-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `gonk-0.6.0/gonk/contrib/notifications/mercure.py` & `gonk-0.6.1/gonk/contrib/notifications/mercure.py`

 * *Files identical despite different names*

### Comparing `gonk-0.6.0/gonk/contrib/persistance/beat.py` & `gonk-0.6.1/gonk/contrib/persistance/beat.py`

 * *Files identical despite different names*

### Comparing `gonk-0.6.0/gonk/contrib/rest_framework/permissions.py` & `gonk-0.6.1/gonk/contrib/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `gonk-0.6.0/gonk/contrib/rest_framework/serializers.py` & `gonk-0.6.1/gonk/contrib/rest_framework/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         fields = (
             'id',
             'started_on',
             'finished_on',
             'revert_started_on',
             'revert_finished_on',
             'status',
+            'with_warnings',
         )
 
 
 class RetrieveTaskSerializer(TaskSerializer):
     class Meta:
         model = Task
         fields = TaskSerializer.Meta.fields + (
```

### Comparing `gonk-0.6.0/gonk/contrib/rest_framework/viewsets.py` & `gonk-0.6.1/gonk/contrib/rest_framework/viewsets.py`

 * *Files identical despite different names*

### Comparing `gonk-0.6.0/gonk/management/commands/create_task.py` & `gonk-0.6.1/gonk/management/commands/create_task.py`

 * *Files identical despite different names*

### Comparing `gonk-0.6.0/gonk/migrations/0001_initial.py` & `gonk-0.6.1/gonk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `gonk-0.6.0/gonk/migrations/0002_auto_20220926_1514.py` & `gonk-0.6.1/gonk/migrations/0002_auto_20220926_1514.py`

 * *Files identical despite different names*

### Comparing `gonk-0.6.0/gonk/models.py` & `gonk-0.6.1/gonk/models.py`

 * *Files identical despite different names*

### Comparing `gonk-0.6.0/gonk/settings.py` & `gonk-0.6.1/gonk/settings.py`

 * *Files identical despite different names*

### Comparing `gonk-0.6.0/gonk/taskrunners.py` & `gonk-0.6.1/gonk/taskrunners.py`

 * *Files identical despite different names*

### Comparing `gonk-0.6.0/gonk/tasks.py` & `gonk-0.6.1/gonk/tasks.py`

 * *Files identical despite different names*

### Comparing `gonk-0.6.0/pyproject.toml` & `gonk-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gonk"
-version = "0.6.0"
+version = "0.6.1"
 description = "Celery tasks for Django made easy"
 authors = ["Francisco Javier Lendinez Tirado <lendinez@kasfactory.net>", "Pablo Moreno <pablo@kasfactory.net>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 keywords = ["celery", "tasks"]
 homepage = "https://github.com/kasfactory/gonk"
 exclude = ["test_app/**"]
```

### Comparing `gonk-0.6.0/PKG-INFO` & `gonk-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gonk
-Version: 0.6.0
+Version: 0.6.1
 Summary: Celery tasks for Django made easy
 Home-page: https://github.com/kasfactory/gonk
 License: BSD-3-Clause
 Keywords: celery,tasks
 Author: Francisco Javier Lendinez Tirado
 Author-email: lendinez@kasfactory.net
 Requires-Python: >=3.9,<4.0
```

