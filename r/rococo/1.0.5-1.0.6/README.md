# Comparing `tmp/rococo-1.0.5.tar.gz` & `tmp/rococo-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rococo-1.0.5.tar", last modified: Thu Apr  4 21:48:12 2024, max compression
+gzip compressed data, was "rococo-1.0.6.tar", last modified: Thu Apr 11 14:26:49 2024, max compression
```

## Comparing `rococo-1.0.5.tar` & `rococo-1.0.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:12.616293 rococo-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 21:48:09.000000 rococo-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-04 21:48:12.616293 rococo-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    28462 2024-04-04 21:48:09.000000 rococo-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:12.608293 rococo-1.0.5/rococo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:12.608293 rococo-1.0.5/rococo/config/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:12.608293 rococo-1.0.5/rococo/data/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/data/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/data/surrealdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:12.608293 rococo-1.0.5/rococo/emailing/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/emailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/emailing/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/emailing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/emailing/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/emailing/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/emailing/mailjet.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/emailing/ses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:12.612293 rococo-1.0.5/rococo/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/messaging/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/messaging/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/messaging/sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:12.612293 rococo-1.0.5/rococo/models/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/login_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/otp_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/person_organization_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/recovery_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:12.612293 rococo-1.0.5/rococo/models/surrealdb/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/surrealdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/surrealdb/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/surrealdb/login_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/surrealdb/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/surrealdb/otp_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/surrealdb/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/surrealdb/person_organization_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/surrealdb/surreal_versioned_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/models/versioned_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:12.612293 rococo-1.0.5/rococo/repositories/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/repositories/base_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:12.612293 rococo-1.0.5/rococo/repositories/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/repositories/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/repositories/mysql/mysql_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/repositories/mysql/organization_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:12.616293 rococo-1.0.5/rococo/repositories/surrealdb/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/repositories/surrealdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/repositories/surrealdb/organization_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/repositories/surrealdb/person_organization_role_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-04-04 21:48:09.000000 rococo-1.0.5/rococo/repositories/surrealdb/surreal_db_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:12.616293 rococo-1.0.5/rococo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-04 21:48:12.000000 rococo-1.0.5/rococo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-04 21:48:12.000000 rococo-1.0.5/rococo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:48:12.000000 rococo-1.0.5/rococo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-04 21:48:12.000000 rococo-1.0.5/rococo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 21:48:12.000000 rococo-1.0.5/rococo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 21:48:12.616293 rococo-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-04 21:48:09.000000 rococo-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:12.616293 rococo-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:48:09.000000 rococo-1.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-04 21:48:09.000000 rococo-1.0.5/tests/base_repository_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-04 21:48:09.000000 rococo-1.0.5/tests/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-04 21:48:09.000000 rococo-1.0.5/tests/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-04 21:48:09.000000 rococo-1.0.5/tests/surreal_db_repository_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:49.032634 rococo-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 14:26:43.000000 rococo-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-11 14:26:49.032634 rococo-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    28462 2024-04-11 14:26:43.000000 rococo-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:49.024634 rococo-1.0.6/rococo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:49.024634 rococo-1.0.6/rococo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:49.024634 rococo-1.0.6/rococo/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/data/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/data/surrealdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:49.024634 rococo-1.0.6/rococo/emailing/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/emailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/emailing/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/emailing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/emailing/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/emailing/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/emailing/mailjet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/emailing/ses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:49.028634 rococo-1.0.6/rococo/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/messaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/messaging/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/messaging/sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:49.028634 rococo-1.0.6/rococo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/login_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/otp_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/person_organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/recovery_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:49.028634 rococo-1.0.6/rococo/models/surrealdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/surrealdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/surrealdb/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/surrealdb/login_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/surrealdb/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/surrealdb/otp_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/surrealdb/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/surrealdb/person_organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/surrealdb/surreal_versioned_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/models/versioned_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:49.028634 rococo-1.0.6/rococo/repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/repositories/base_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:49.028634 rococo-1.0.6/rococo/repositories/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/repositories/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/repositories/mysql/mysql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/repositories/mysql/organization_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:49.032634 rococo-1.0.6/rococo/repositories/surrealdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/repositories/surrealdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/repositories/surrealdb/organization_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/repositories/surrealdb/person_organization_role_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-04-11 14:26:43.000000 rococo-1.0.6/rococo/repositories/surrealdb/surreal_db_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:49.032634 rococo-1.0.6/rococo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-11 14:26:49.000000 rococo-1.0.6/rococo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-11 14:26:49.000000 rococo-1.0.6/rococo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:26:49.000000 rococo-1.0.6/rococo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 14:26:49.000000 rococo-1.0.6/rococo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 14:26:49.000000 rococo-1.0.6/rococo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:26:49.032634 rococo-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-11 14:26:43.000000 rococo-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:49.032634 rococo-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:26:43.000000 rococo-1.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-11 14:26:43.000000 rococo-1.0.6/tests/base_repository_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-11 14:26:43.000000 rococo-1.0.6/tests/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-11 14:26:43.000000 rococo-1.0.6/tests/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-11 14:26:43.000000 rococo-1.0.6/tests/surreal_db_repository_test.py
```

### Comparing `rococo-1.0.5/LICENSE` & `rococo-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/PKG-INFO` & `rococo-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rococo
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python library to help build things the way we want them built
 Home-page: https://github.com/EcorRouge/rococo
 Author: Jay Grieves
 Author-email: jaygrieves@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `rococo-1.0.5/README.md` & `rococo-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/config/config.py` & `rococo-1.0.6/rococo/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 Config class that allows to load from a .toml file, and/or use a .env file.
 """
+import json
+import logging
 import os
 import re
-import json
 from abc import abstractmethod
-from typing import Optional
-import logging
+from typing import List, Optional
+
 from dotenv import load_dotenv
 
 logger = logging.getLogger(__name__)
 
 
-class BaseConfig():
+class BaseConfig:
     """
     Config class that allows to load from a .toml file, and/or use a .env file.
     """
+
     def __init__(self):
         load_dotenv()
         self.project_version = None
         # Get all environment variables and store them in a dictionary
         self.env_vars = {key: os.getenv(key) for key in os.environ}
 
     def get_env_vars(self) -> dict:
@@ -36,15 +38,15 @@
         """
         if var_name in self.env_vars.keys():
             return self.env_vars[var_name]
         else:
             logger.warning("Variable %s not found.", var_name)
             return None
 
-    def load_toml(self, toml_folder_dir: str, log_version_string: bool=True) -> bool:
+    def load_toml(self, toml_folder_dir: str, log_version_string: bool = True) -> bool:
         """
         Loads the toml file for the project
         Args:
             toml_folder_dir (str) : Path to the folder where the toml file exists.
         """
         pyproject_path = os.path.join(toml_folder_dir, 'pyproject.toml')
 
@@ -83,27 +85,26 @@
             except ValueError:
                 logger.error(
                     "Error: Invalid input format. Please provide a comma-delimited string.")
                 return False
         logger.warning("Warning: var %s not found.", var_name)
         return False
 
-    def get_var_as_list(self, var_name: str) -> bool:
+    def get_var_as_list(self, var_name: str) -> Optional[List]:
         """
         Returns a comma-delimited var as list
         """
-        if var_name in self.env_vars.keys():
-            try:
-                return [env_var.strip() for env_var in self.env_vars[var_name].split(",")]
-            except ValueError:
-                logger.error(
-                    "Error: Invalid input format. Please provide a comma-delimited string.")
-        logger.warning("Warning: var %s not found.", var_name)
-        return None
+        if var_name not in self.env_vars.keys():
+            logger.warning("Warning: var %s not found.", var_name)
+            return None
 
+        try:
+            return [env_var.strip() for env_var in self.env_vars[var_name].split(",")]
+        except ValueError:
+            logger.error("Error: Invalid input format. Please provide a comma-delimited string.")
 
     def convert_var_from_json_string(self, var_name: str) -> bool:
         """
         Converts a json string into a pythonic type
         """
         if var_name in self.env_vars.keys():
             try:
@@ -116,7 +117,8 @@
         return False
 
     @abstractmethod
     def validate_env_vars(self):
         """
         Abstract method for validation of the env vars.
         """
+        pass
```

### Comparing `rococo-1.0.5/rococo/data/base.py` & `rococo-1.0.6/rococo/data/base.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/data/mysql.py` & `rococo-1.0.6/rococo/data/mysql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any, Dict, List, Tuple, Union, Optional
 from uuid import UUID
+
 import pymysql
 
 from rococo.data.base import DbAdapter
 
 
 class MySqlAdapter(DbAdapter):
     """MySQL adapter for interacting with MySQL."""
@@ -15,42 +16,39 @@
         self._user = user
         self._password = password
         self._database = database
         self._cursor_class = pymysql.cursors.DictCursor
         self._connection = None
         self._cursor = None
 
-
     def __enter__(self):
         """Context manager entry point for creating DB connection."""
         self._connection = pymysql.connect(
             host=self._host,
             port=self._port,
             user=self._user,
             password=self._password,
             database=self._database,
             cursorclass=self._cursor_class
         )
         self._cursor = self._connection.cursor()
 
         return self
 
-
     def __exit__(self, exc_type, exc_value, traceback):
         """Context manager exit point for closing DB connection."""
 
         if self._cursor is not None:
             self._cursor.close()
             self._cursor = None
 
         if self._connection is not None:
             self._connection.close()
             self._connection = None
 
-
     @property
     def connect(self):
         return pymysql.connect(
             host=self._host,
             port=self._port,
             user=self._user,
             password=self._password,
@@ -76,18 +74,24 @@
         elif isinstance(value, list):
             return f"""{key} IN ({','.join(f'"{v}"' for v in value)})"""
         elif isinstance(value, UUID):
             return f"{key}='{str(value)}'"
         elif isinstance(value, type(None)):
             return f"{key} IS NULL"
         else:
-            raise Exception(f"Unsuppported type {type(value)} for condition key: {key}, value: {value}")
+            raise Exception(f"Unsupported type {type(value)} for condition key: {key}, value: {value}")
 
     def move_entity_to_audit_table(self, table, entity_id):
-        query = f"""INSERT INTO {table}_audit (SELECT * FROM {table} WHERE entity_id="{str(entity_id).replace('-', '')}")"""
+        # Get the column names from the table
+        self._call_cursor('execute', f"SHOW COLUMNS FROM {table}")
+
+        column_list = ", ".join(column.get('Field') for column in self._cursor.fetchall())
+
+        query = f"""INSERT INTO {table}_audit ({column_list}) (SELECT {column_list} FROM {table} WHERE entity_id="{str(entity_id).replace('-', '')}");"""
+
         self._call_cursor('execute', query)
         self._connection.commit()
 
     def execute_query(self, sql, _vars=None):
         """Executes a query against the DB."""
         if _vars is None:
             _vars = {}
@@ -105,29 +109,29 @@
         """
         if not response or not isinstance(response, list):
             return []
 
         return response
 
     def get_one(
-        self,
-        table: str,
-        conditions: Dict[str, Any],
-        sort: List[Tuple[str, str]] = None,
-        join_statements: list = None,
-        additional_fields: list = None
-    ) -> Dict[str, Any]:
+            self,
+            table: str,
+            conditions: Dict[str, Any],
+            sort: List[Tuple[str, str]] = None,
+            join_statements: list = None,
+            additional_fields: list = None
+    ) -> Optional[Dict[str, Any]]:
         fields = [f'{table}.*']
         if additional_fields:
             fields += additional_fields
 
         query = f"SELECT {', '.join(fields)} FROM {table}"
         for join_stmt in join_statements:
             query += f"""\n{join_stmt}\n"""
-        
+
         condition_strs = []
         if conditions:
             condition_strs = [f"{self._build_condition_string(table, k, v)}" for k, v in conditions.items()]
         condition_strs.append(f"{table}.active=true")
         query += f" WHERE {' AND '.join(condition_strs)}"
 
         if sort:
@@ -140,23 +144,23 @@
             return None
         elif isinstance(db_response, list):
             return db_response[0]
         else:
             return db_response
 
     def get_many(
-        self,
-        table: str,
-        conditions: Dict[str, Any] = None,
-        sort: List[Tuple[str, str]] = None,
-        limit: int = None,
-        offset: int = None,
-        active: bool = True,
-        join_statements: list = None,
-        additional_fields: list = None
+            self,
+            table: str,
+            conditions: Dict[str, Any] = None,
+            sort: List[Tuple[str, str]] = None,
+            limit: int = None,
+            offset: int = None,
+            active: bool = True,
+            join_statements: list = None,
+            additional_fields: list = None
     ) -> List[Dict[str, Any]]:
 
         fields = [f'{table}.*']
         if additional_fields:
             fields += additional_fields
 
         query = f"SELECT {', '.join(fields)} FROM {table}"
@@ -174,16 +178,14 @@
             sort_strs = [f"{column} {direction}" for column, direction in sort]
             query += f" ORDER BY {', '.join(sort_strs)}"
         if limit is not None:
             query += f" LIMIT {limit}"
         if offset is not None:
             query += f" OFFSET {offset}"
 
-        print(query)
-
         db_response = self.parse_db_response(self.execute_query(query))
         if not db_response:
             return []
         elif isinstance(db_response, dict):
             return [db_response]
         else:
             return db_response
@@ -205,8 +207,9 @@
     def save(self, table: str, data: Dict[str, Any]):
         self._create_in_database(table, data)
         return data
 
     def delete(self, table: str, data: Dict[str, Any]) -> bool:
         # Set active = false
         data['active'] = False
-        return self.save(table, data)
+        self.save(table, data)
+        return True
```

### Comparing `rococo-1.0.5/rococo/data/surrealdb.py` & `rococo-1.0.6/rococo/data/surrealdb.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/emailing/config.py` & `rococo-1.0.6/rococo/emailing/config.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/emailing/factory.py` & `rococo-1.0.6/rococo/emailing/factory.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/emailing/mailjet.py` & `rococo-1.0.6/rococo/emailing/mailjet.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/messaging/base.py` & `rococo-1.0.6/rococo/messaging/base.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/messaging/rabbitmq.py` & `rococo-1.0.6/rococo/messaging/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/messaging/sqs.py` & `rococo-1.0.6/rococo/messaging/sqs.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/models/login_method.py` & `rococo-1.0.6/rococo/models/login_method.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/models/organization.py` & `rococo-1.0.6/rococo/models/organization.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/models/person_organization_role.py` & `rococo-1.0.6/rococo/models/person_organization_role.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/models/surrealdb/login_method.py` & `rococo-1.0.6/rococo/models/surrealdb/login_method.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/models/surrealdb/organization.py` & `rococo-1.0.6/rococo/models/surrealdb/organization.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/models/surrealdb/person_organization_role.py` & `rococo-1.0.6/rococo/models/surrealdb/person_organization_role.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/models/surrealdb/surreal_versioned_model.py` & `rococo-1.0.6/rococo/models/surrealdb/surreal_versioned_model.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/models/versioned_model.py` & `rococo-1.0.6/rococo/models/versioned_model.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/repositories/base_repository.py` & `rococo-1.0.6/rococo/repositories/base_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/repositories/mysql/mysql_repository.py` & `rococo-1.0.6/rococo/repositories/mysql/mysql_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-"""SurrealDbRepository class"""
+"""MySqlDbRepository class"""
 
+import re
 from dataclasses import fields
+from datetime import datetime
 from typing import Any, Dict, List, Type, Union
 from uuid import UUID
-import re
-from datetime import datetime
 
-from rococo.data import SurrealDbAdapter
+from rococo.data import MySqlAdapter
 from rococo.messaging import MessageAdapter
 from rococo.models import VersionedModel
 from rococo.repositories import BaseRepository
 
 
 class MySqlRepository(BaseRepository):
     """MySqlRepository class"""
 
     def __init__(
             self,
-            db_adapter: SurrealDbAdapter,
+            db_adapter: MySqlAdapter,
             model: Type[VersionedModel],
             message_adapter: MessageAdapter,
             queue_name: str,
             user_id: UUID = None
     ):
         super().__init__(db_adapter, model, message_adapter, queue_name, user_id=user_id)
         self.table_name = re.sub(r'(?<!^)(?=[A-Z])', '_', model.__name__).lower()
@@ -30,41 +30,41 @@
     def _process_data_before_save(self, instance: VersionedModel):
         """Method to convert VersionedModel instance to a data dictionary that can be saved to MySQL"""
         super()._process_data_before_save(instance)
         data = instance.as_dict(convert_datetime_to_iso_string=False, convert_uuids=False)
         for field in fields(instance):
             if data.get(field.name) is None:
                 continue
-                
+
             field_value = data[field.name]
 
             if field.metadata.get('field_type') in ['entity_id', 'uuid']:
                 if isinstance(field_value, VersionedModel):
                     field_value = str(field_value.entity_id).replace('-', '')
                 elif isinstance(field_value, dict):
                     field_value = str(field_value.get('entity_id')).replace('-', '')
                 elif isinstance(field_value, str):
                     field_value = field_value.replace('-', '')
 
             if isinstance(field_value, UUID):
                 field_value = str(field_value).replace('-', '')
             if isinstance(field_value, datetime):
                 field_value = field_value.strftime('%Y-%m-%d %H:%M:%S')
-            
+
             data[field.name] = field_value
         return data
 
     def _process_data_from_db(self, data):
         """Method to convert data dictionary fetched from MySQL to a VersionedModel instance."""
 
         def _process_record(data: dict, model):
             model()
             is_partial = not all(_field.name in data for _field in fields(model))
             for field in fields(model):
-                if data.get(field.name) is None: 
+                if data.get(field.name) is None:
                     continue
 
                 if field.metadata.get('field_type') == 'entity_id':
                     field_model_class = field.metadata.get('relationship', {}).get('model') or model
                     field_table_name = re.sub(r'(?<!^)(?=[A-Z])', '_', field_model_class.__name__).lower()
 
                     field_value = data[field.name]
@@ -76,15 +76,16 @@
                     elif isinstance(field_value, str):
                         if field.name == 'entity_id':
                             data[field.name] = UUID(field_value)
                         else:
                             field_data = {'entity_id': field_value}
                             for _field in fields(field_model_class):
                                 if f'joined_{field.name}_{field_table_name}_{_field.name}' in data:
-                                    field_data[_field.name] = data[f'joined_{field.name}_{field_table_name}_{_field.name}']
+                                    field_data[_field.name] = data[
+                                        f'joined_{field.name}_{field_table_name}_{_field.name}']
                             for data_field, data_value in data.items():
                                 if data_field.startswith('joined_'):
                                     field_data[data_field] = data_value
 
                             data[field.name] = _process_record(field_data, field_model_class)
                     elif isinstance(field_value, UUID):
                         pass
@@ -100,41 +101,45 @@
             for record in data:
                 _process_record(record, self.model)
         elif isinstance(data, dict):
             _process_record(data, self.model)
         else:
             raise NotImplementedError
 
-
-    def get_one(self, conditions: Dict[str, Any] = None, join_fields: List[str] = None, additional_fields: List[str] = None) -> Union[VersionedModel, None]:
+    def get_one(self, conditions: Dict[str, Any] = None, join_fields: List[str] = None,
+                additional_fields: List[str] = None) -> Union[VersionedModel, None]:
         """get one"""
 
         if additional_fields is None:
             additional_fields = []
 
         join_stmt_list = []
         if join_fields:
             joined_fields = {}
             for field_name in join_fields:
                 if '.' in field_name:
                     parent_field, child_field = field_name.rsplit('.', 1)
                     if parent_field not in joined_fields:
-                        raise Exception(f"Parent field {parent_field} needs to be joined before joining {child_field} field. Raised while joining {field_name} for model {self.model.__name__}.")
+                        raise Exception(
+                            f"Parent field {parent_field} needs to be joined before joining {child_field} field. Raised while joining {field_name} for model {self.model.__name__}.")
                     parent_model = joined_fields[parent_field]
                 else:
                     parent_model = self.model
                     child_field = field_name
                 parent_table_name = re.sub(r'(?<!^)(?=[A-Z])', '_', parent_model.__name__).lower()
                 join_field = next((field for field in fields(parent_model) if field.name == child_field), None)
                 if join_field is None or join_field.metadata.get('field_type') != 'entity_id':
                     raise Exception(f"Invalid join field {child_field} specified for model {parent_model.__name__}.")
                 join_model = join_field.metadata.get('relationship').get('model')
                 join_table_name = re.sub(r'(?<!^)(?=[A-Z])', '_', join_model.__name__).lower()
-                join_stmt_list.append(f'INNER JOIN {join_table_name} ON {parent_table_name}.{child_field}={join_table_name}.entity_id AND {join_table_name}.active=true')
-                join_field_list = [f'{join_table_name}.{_field.name} AS joined_{child_field}_{join_table_name}_{_field.name}' for _field in fields(join_model)]
+                join_stmt_list.append(
+                    f'INNER JOIN {join_table_name} ON {parent_table_name}.{child_field}={join_table_name}.entity_id AND {join_table_name}.active=true')
+                join_field_list = [
+                    f'{join_table_name}.{_field.name} AS joined_{child_field}_{join_table_name}_{_field.name}' for
+                    _field in fields(join_model)]
                 additional_fields += join_field_list
                 joined_fields[field_name] = join_model
 
         if conditions:
             for condition_name, value in conditions.copy().items():
                 condition_field = next((field for field in fields(self.model) if field.name == condition_name), None)
                 if condition_field and condition_field.metadata.get('field_type') == 'entity_id':
@@ -152,63 +157,66 @@
                                 conditions[condition_name].append(str(v).replace('-', ''))
                             else:
                                 raise NotImplementedError
                     else:
                         raise NotImplementedError
 
         data = self._execute_within_context(
-            self.adapter.get_one, self.table_name, conditions, join_statements=join_stmt_list, additional_fields=additional_fields
+            self.adapter.get_one, self.table_name, conditions, join_statements=join_stmt_list,
+            additional_fields=additional_fields
         )
 
         self.model()  # Calls __post_init__ of model to import related models and update fields.
 
         self._process_data_from_db(data)
 
         if not data:
             return None
         return self.model.from_dict(data)
 
-
     def get_many(
-        self,
-        conditions: Dict[str, Any] = None,
-        join_fields: List[str] = None,
-        additional_fields: List[str] = None,
-        sort: List[tuple] = None,
-        limit: int = None,
-        offset: int = None
+            self,
+            conditions: Dict[str, Any] = None,
+            join_fields: List[str] = None,
+            additional_fields: List[str] = None,
+            sort: List[tuple] = None,
+            limit: int = None,
+            offset: int = None
     ) -> List[VersionedModel]:
         """get many"""
         if additional_fields is None:
             additional_fields = []
 
         join_stmt_list = []
         if join_fields:
             joined_fields = {}
             for field_name in join_fields:
                 if '.' in field_name:
                     parent_field, child_field = field_name.rsplit('.', 1)
                     if parent_field not in joined_fields:
-                        raise Exception(f"Parent field {parent_field} needs to be joined before joining {child_field} field. Raised while joining {field_name} for model {self.model.__name__}.")
+                        raise Exception(
+                            f"Parent field {parent_field} needs to be joined before joining {child_field} field. Raised while joining {field_name} for model {self.model.__name__}.")
                     parent_model = joined_fields[parent_field]
                 else:
                     parent_model = self.model
                     child_field = field_name
                 parent_table_name = re.sub(r'(?<!^)(?=[A-Z])', '_', parent_model.__name__).lower()
                 join_field = next((field for field in fields(parent_model) if field.name == child_field), None)
                 if join_field is None or join_field.metadata.get('field_type') != 'entity_id':
                     raise Exception(f"Invalid join field {child_field} specified for model {parent_model.__name__}.")
                 join_model = join_field.metadata.get('relationship').get('model')
                 join_table_name = re.sub(r'(?<!^)(?=[A-Z])', '_', join_model.__name__).lower()
-                join_stmt_list.append(f'INNER JOIN {join_table_name} ON {parent_table_name}.{child_field}={join_table_name}.entity_id AND {join_table_name}.active=true')
-                join_field_list = [f'{join_table_name}.{_field.name} AS joined_{child_field}_{join_table_name}_{_field.name}' for _field in fields(join_model)]
+                join_stmt_list.append(
+                    f'INNER JOIN {join_table_name} ON {parent_table_name}.{child_field}={join_table_name}.entity_id AND {join_table_name}.active=true')
+                join_field_list = [
+                    f'{join_table_name}.{_field.name} AS joined_{child_field}_{join_table_name}_{_field.name}' for
+                    _field in fields(join_model)]
                 additional_fields += join_field_list
                 joined_fields[field_name] = join_model
 
-
         if conditions:
             for condition_name, value in conditions.copy().items():
                 condition_field = next((field for field in fields(self.model) if field.name == condition_name), None)
                 if condition_field and condition_field.metadata.get('field_type') == 'entity_id':
                     if condition_name == 'entity_id':
                         condition_name = 'id'
                         conditions[condition_name] = conditions.pop('entity_id')
@@ -227,15 +235,16 @@
                                 conditions[condition_name].append(str(v).replace('-', ''))
                             else:
                                 raise NotImplementedError
                     else:
                         raise NotImplementedError
 
         records = self._execute_within_context(
-            self.adapter.get_many, self.table_name, conditions, sort, limit, offset, join_statements=join_stmt_list, additional_fields=additional_fields
+            self.adapter.get_many, self.table_name, conditions, sort, limit, offset, join_statements=join_stmt_list,
+            additional_fields=additional_fields
         )
 
         # If the adapter returned a single dictionary, wrap it in a list
         if isinstance(records, dict):
             records = [records]
 
         self.model()  # Calls __post_init__ of model to import related models and update fields.
```

### Comparing `rococo-1.0.5/rococo/repositories/mysql/organization_repository.py` & `rococo-1.0.6/rococo/repositories/mysql/organization_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/repositories/surrealdb/organization_repository.py` & `rococo-1.0.6/rococo/repositories/surrealdb/organization_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/repositories/surrealdb/person_organization_role_repository.py` & `rococo-1.0.6/rococo/repositories/surrealdb/person_organization_role_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo/repositories/surrealdb/surreal_db_repository.py` & `rococo-1.0.6/rococo/repositories/surrealdb/surreal_db_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/rococo.egg-info/PKG-INFO` & `rococo-1.0.6/rococo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rococo
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python library to help build things the way we want them built
 Home-page: https://github.com/EcorRouge/rococo
 Author: Jay Grieves
 Author-email: jaygrieves@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `rococo-1.0.5/rococo.egg-info/SOURCES.txt` & `rococo-1.0.6/rococo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/setup.py` & `rococo-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='rococo',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     url='https://github.com/EcorRouge/rococo',
     license='MIT',
     author='Jay Grieves',
     author_email='jaygrieves@gmail.com',
     description='A Python library to help build things the way we want them built',
     long_description=open('README.md').read(),
```

### Comparing `rococo-1.0.5/tests/base_repository_test.py` & `rococo-1.0.6/tests/base_repository_test.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/tests/config_test.py` & `rococo-1.0.6/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/tests/model_test.py` & `rococo-1.0.6/tests/model_test.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.5/tests/surreal_db_repository_test.py` & `rococo-1.0.6/tests/surreal_db_repository_test.py`

 * *Files identical despite different names*

