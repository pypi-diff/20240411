# Comparing `tmp/pynest-api-0.1.3.tar.gz` & `tmp/pynest-api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynest-api-0.1.3.tar", last modified: Thu Mar  7 07:23:58 2024, max compression
+gzip compressed data, was "pynest-api-0.2.0.tar", last modified: Thu Apr 11 13:56:35 2024, max compression
```

## Comparing `pynest-api-0.1.3.tar` & `pynest-api-0.2.0.tar`

### file list

```diff
@@ -1,63 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.643757 pynest-api-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-07 07:23:31.000000 pynest-api-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-03-07 07:23:58.643757 pynest-api-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-03-07 07:23:31.000000 pynest-api-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.635757 pynest-api-0.1.3/nest/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.635757 pynest-api-0.1.3/nest/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/cli/click_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.635757 pynest-api-0.1.3/nest/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.635757 pynest-api-0.1.3/nest/common/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/common/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/common/templates/base_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/common/templates/blank_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/common/templates/mongo_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/common/templates/mysql_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/common/templates/orm_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/common/templates/postgres_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/common/templates/sqlite_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/common/templates/templates_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.635757 pynest-api-0.1.3/nest/core/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/core/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.639757 pynest-api-0.1.3/nest/core/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/core/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/core/database/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/core/database/odm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/core/database/odm_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/core/database/orm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/core/database/orm_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.639757 pynest-api-0.1.3/nest/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/core/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/core/decorators/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/core/decorators/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/core/decorators/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/core/decorators/http_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.639757 pynest-api-0.1.3/nest/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.639757 pynest-api-0.1.3/nest/plugins/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/plugins/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.639757 pynest-api-0.1.3/nest/plugins/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/plugins/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.639757 pynest-api-0.1.3/nest/plugins/modules/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/plugins/modules/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.639757 pynest-api-0.1.3/nest/plugins/modules/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/plugins/modules/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/plugins/modules/redis/redis_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/plugins/modules/redis/redis_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/plugins/modules/redis/redis_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/plugins/modules/redis/redis_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.639757 pynest-api-0.1.3/nest/plugins/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:31.000000 pynest-api-0.1.3/nest/plugins/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:23:58.643757 pynest-api-0.1.3/pynest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-03-07 07:23:58.000000 pynest-api-0.1.3/pynest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-07 07:23:58.000000 pynest-api-0.1.3/pynest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 07:23:58.000000 pynest-api-0.1.3/pynest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-07 07:23:58.000000 pynest-api-0.1.3/pynest_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-07 07:23:58.000000 pynest-api-0.1.3/pynest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-07 07:23:58.000000 pynest-api-0.1.3/pynest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-07 07:23:31.000000 pynest-api-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 07:23:58.643757 pynest-api-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.450256 pynest-api-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-11 13:56:08.000000 pynest-api-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-04-11 13:56:35.450256 pynest-api-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-11 13:56:08.000000 pynest-api-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.438256 pynest-api-0.2.0/nest/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.438256 pynest-api-0.2.0/nest/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/cli/click_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.438256 pynest-api-0.2.0/nest/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/route_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.442256 pynest-api-0.2.0/nest/common/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/templates/base_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/templates/blank_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/templates/mongo_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/templates/mysql_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/templates/orm_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/templates/postgres_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/templates/sqlite_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/common/templates/templates_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.442256 pynest-api-0.2.0/nest/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.442256 pynest-api-0.2.0/nest/core/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/database/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/database/odm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/database/odm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/database/orm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/database/orm_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.446256 pynest-api-0.2.0/nest/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/decorators/class_based_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/decorators/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/decorators/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/decorators/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/decorators/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/decorators/injectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/decorators/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/decorators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/pynest_app_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/pynest_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/pynest_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/core/pynest_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.446256 pynest-api-0.2.0/nest/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.446256 pynest-api-0.2.0/nest/plugins/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/plugins/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.446256 pynest-api-0.2.0/nest/plugins/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/plugins/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.446256 pynest-api-0.2.0/nest/plugins/modules/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/plugins/modules/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.446256 pynest-api-0.2.0/nest/plugins/modules/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/plugins/modules/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/plugins/modules/redis/redis_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/plugins/modules/redis/redis_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/plugins/modules/redis/redis_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/plugins/modules/redis/redis_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.446256 pynest-api-0.2.0/nest/plugins/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:09.000000 pynest-api-0.2.0/nest/plugins/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:56:35.450256 pynest-api-0.2.0/pynest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-04-11 13:56:35.000000 pynest-api-0.2.0/pynest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-11 13:56:35.000000 pynest-api-0.2.0/pynest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:56:35.000000 pynest-api-0.2.0/pynest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 13:56:35.000000 pynest-api-0.2.0/pynest_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-11 13:56:35.000000 pynest-api-0.2.0/pynest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 13:56:35.000000 pynest-api-0.2.0/pynest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-11 13:56:09.000000 pynest-api-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:56:35.450256 pynest-api-0.2.0/setup.cfg
```

### Comparing `pynest-api-0.1.3/LICENSE` & `pynest-api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynest-api-0.1.3/PKG-INFO` & `pynest-api-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynest-api
-Version: 0.1.3
+Version: 0.2.0
 Summary: PyNest is a FastAPI Abstraction for building microservices, influenced by NestJS.
 Author-email: Itay Dar <itay2803@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 PyNest
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,24 +31,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click==8.1.6
+Requires-Dist: click>=8.1.6
 Requires-Dist: fastapi==0.95.1
-Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: SQLAlchemy==2.0.19
-Requires-Dist: uvicorn==0.23.1
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: astor==0.8.1
-Requires-Dist: black==23.11.0
+Requires-Dist: python-dotenv>=1.0.0
+Requires-Dist: uvicorn>=0.23.1
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: astor>=0.8.1
+Requires-Dist: black>=23.11.0
+Requires-Dist: injector>=0.21.0
+Requires-Dist: pydantic<2.0.0
+Requires-Dist: sqlalchemy==2.0.19
+Requires-Dist: alembic==1.7.4
 Provides-Extra: test
 Requires-Dist: pytest==6.2.5; extra == "test"
+Provides-Extra: orm
+Requires-Dist: sqlalchemy==2.0.19; extra == "orm"
+Requires-Dist: alembic==1.7.4; extra == "orm"
 Provides-Extra: mongo
 Requires-Dist: pymongo==3.12.0; extra == "mongo"
 Requires-Dist: motor==3.2.0; extra == "mongo"
 Requires-Dist: beanie==1.20.0; extra == "mongo"
 
 <p align="center">
   <img src="docs/imgs/pynest-logo.png" title="pynest logo" width="300">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynest-api Version: 0.1.3 Summary: PyNest is a
+Metadata-Version: 2.1 Name: pynest-api Version: 0.2.0 Summary: PyNest is a
 FastAPI Abstraction for building microservices, influenced by NestJS. Author-
 email: Itay Dar
 gmail.com> License: MIT License Copyright (c) 2023 PyNest Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -18,21 +18,24 @@
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/PythonNest/
 PyNest Project-URL: Documentation, https://pythonnest.github.io/PyNest/
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8.1 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: click==8.1.6 Requires-Dist: fastapi==0.95.1 Requires-
-Dist: python-dotenv==1.0.0 Requires-Dist: SQLAlchemy==2.0.19 Requires-Dist:
-uvicorn==0.23.1 Requires-Dist: PyYAML==6.0.1 Requires-Dist: astor==0.8.1
-Requires-Dist: black==23.11.0 Provides-Extra: test Requires-Dist:
-pytest==6.2.5; extra == "test" Provides-Extra: mongo Requires-Dist:
-pymongo==3.12.0; extra == "mongo" Requires-Dist: motor==3.2.0; extra == "mongo"
-Requires-Dist: beanie==1.20.0; extra == "mongo"
+LICENSE Requires-Dist: click>=8.1.6 Requires-Dist: fastapi==0.95.1 Requires-
+Dist: python-dotenv>=1.0.0 Requires-Dist: uvicorn>=0.23.1 Requires-Dist:
+PyYAML>=6.0.1 Requires-Dist: astor>=0.8.1 Requires-Dist: black>=23.11.0
+Requires-Dist: injector>=0.21.0 Requires-Dist: pydantic<2.0.0 Requires-Dist:
+sqlalchemy==2.0.19 Requires-Dist: alembic==1.7.4 Provides-Extra: test Requires-
+Dist: pytest==6.2.5; extra == "test" Provides-Extra: orm Requires-Dist:
+sqlalchemy==2.0.19; extra == "orm" Requires-Dist: alembic==1.7.4; extra ==
+"orm" Provides-Extra: mongo Requires-Dist: pymongo==3.12.0; extra == "mongo"
+Requires-Dist: motor==3.2.0; extra == "mongo" Requires-Dist: beanie==1.20.0;
+extra == "mongo"
                           [docs/imgs/pynest-logo.png]
  PPyyNNeesstt iiss aa PPyytthhoonn ffrraammeewwoorrkk bbuuiilltt oonn ttoopp ooff FFaassttAAPPII tthhaatt ffoolllloowwss tthhee mmoodduullaarr
                             aarrcchhiitteeccttuurree ooff NNeessttJJSS
                      _[_V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]
 # Description PyNest is designed to help structure your APIs in an intuitive,
 easy to understand, and enjoyable way. With PyNest, you can build scalable and
 maintainable APIs with ease. The framework supports dependency injection, type
```

### Comparing `pynest-api-0.1.3/README.md` & `pynest-api-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pynest-api-0.1.3/nest/cli/cli.py` & `pynest-api-0.2.0/nest/cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from typing import Optional
+
 import click
+
 from nest.cli.click_handlers import create_nest_app, create_nest_module
 
 ### Options ###
 APP_NAME = click.option(
     "--app-name",  # Changed the underscore to a hyphen for consistency
     "-n",
     help="The name of the nest app.",
@@ -28,15 +31,15 @@
     type=str,
 )
 
 IS_ASYNC = click.option(
     "--is-async",  # Changed the underscore to a hyphen for consistency
     help="Whether the project should be async or not (only for relational databases).",
     required=False,
-    is_flag=True,  # Set is_flag=True to make it a flag option
+    is_flag=True,
 )
 
 
 @click.group()
 def nest_cli() -> None:
     pass
 
@@ -64,11 +67,7 @@
 @generate.command(
     name="module",
     help="Generate a new module (controller, service, entity, model, module).",
 )
 @MODULE_NAME
 def generate_module(name: str):
     create_nest_module(name=name)
-
-
-if __name__ == "__main__":
-    nest_cli()
```

### Comparing `pynest-api-0.1.3/nest/cli/click_handlers.py` & `pynest-api-0.2.0/nest/cli/click_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import yaml
 from pathlib import Path
+
+import yaml
+
 from nest.common.templates.templates_factory import TemplateFactory
 
 
 def get_metadata():
     setting_path = Path(__file__).parent.parent / "settings.yaml"
     assert setting_path.exists(), "settings.yaml file not found"
     with open(setting_path, "r") as file:
@@ -21,15 +23,15 @@
 
     :param app_name: The name of the app
     :param db_type: The type of the database (sqlite, mysql, postgresql)
     :param is_async: whether the project should be async or not (only for relational databases)
 
     The files structure are:
 
-    ├── app.py
+    ├── app_module.py
     ├── config.py (only for databases)
     ├── main.py
     ├── requirements.txt
     ├── .gitignore
     ├── src
     │    ├── __init__.py
```

### Comparing `pynest-api-0.1.3/nest/common/templates/base_template.py` & `pynest-api-0.2.0/nest/common/templates/base_template.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import ast
+import os
 from abc import ABC, abstractmethod
 from pathlib import Path
-import os
-from typing import List, Tuple, Union, Callable
-from nest import __version__
-import subprocess
-import ast
+from typing import Callable, List, Tuple, Union
+
 import astor
+import black
+
+from nest import __version__
 
 
 def get_module_strings(module_name: str) -> Tuple[List[str], str]:
     split_module_name = module_name.split("_")
     capitalized_module_name = "".join([word.capitalize() for word in split_module_name])
     return split_module_name, capitalized_module_name
 
@@ -27,19 +29,20 @@
 
     @staticmethod
     def main_file():
         return """import uvicorn
 
 if __name__ == '__main__':
     uvicorn.run(
-        'app:app',
+        'src.app_module:http_server',
         host="0.0.0.0",
         port=8000,
         reload=True
     )
+    
 """
 
     @abstractmethod
     def app_file(self):
         raise NotImplementedError
 
     @abstractmethod
@@ -97,21 +100,62 @@
 ```
 
 ## Step 3 - Send requests
 
 Go to the fastapi docs and use your api endpoints - http://127.0.0.1/docs
 """
 
-    @abstractmethod
     def module_file(self):
+        return f"""from nest.core import Module
+from .{self.module_name}_controller import {self.capitalized_module_name}Controller
+from .{self.module_name}_service import {self.capitalized_module_name}Service
+
+
+@Module(
+    controllers=[{self.capitalized_module_name}Controller],
+    providers=[{self.capitalized_module_name}Service],
+    imports=[]
+)   
+class {self.capitalized_module_name}Module:
+    pass
+
+    """
+
+    @staticmethod
+    def app_controller_file():
+        return f"""from nest.core import Controller, Get, Post
+from .app_service import AppService
+
+
+@Controller("/")
+class AppController:
+
+    def __init__(self, service: AppService):
+        self.service = service
+
+    @Get("/")
+    def get_app_info(self):
+        return self.service.get_app_info()
+"""
+
+    @staticmethod
+    def app_service_file():
         return """
-class ExampleModule:
-    self.controllers = []
-    self.providers = []
-    
+from nest.core import Injectable
+
+
+@Injectable
+class AppService:
+    def __init__(self):
+        self.app_name = "Pynest App"
+        self.app_version = "1.0.0"
+
+    def get_app_info(self):
+        return {"app_name": self.app_name, "app_version": self.app_version}
+
 """
 
     @abstractmethod
     def model_file(self):
         raise NotImplementedError
 
     @abstractmethod
@@ -201,19 +245,30 @@
                 if directory == target:
                     return os.path.join(root, directory)
 
         # If target folder is not found, return None
         return None
 
     @staticmethod
-    def format_with_black(file_path):
-        subprocess.run(["black", file_path], check=True)
+    def read_file(file_path: str) -> str:
+        with open(file_path, "r") as file:
+            return file.read()
+
+    @staticmethod
+    def write_file(file_path: str, content: str) -> None:
+        with open(file_path, "w") as file:
+            file.write(content)
+
+    def format_with_black(self, file_path: str) -> None:
+        file_content = self.read_file(file_path)
+        formatted_content = black.format_str(file_content, mode=black.FileMode())
+        self.write_file(file_path, formatted_content)
 
     @staticmethod
-    def save_file_with_astor(file_path, tree):
+    def save_file_with_astor(file_path: str, tree: ast.Module) -> None:
         with open(file_path, "w") as file:
             file.write(astor.to_source(tree))
 
     @staticmethod
     def get_ast_tree(file_path: Union[str, Path]) -> ast.Module:
         with open(file_path, "r") as file:
             source = file.read()
@@ -247,37 +302,31 @@
             module_path=f"src.{self.module_name}.{self.module_name}_module",
             class_name=self.class_name,
             import_exception="from nest.core import App",
         )
         modified = False
 
         for node in ast.walk(tree):
-            if (
-                isinstance(node, ast.Call)
-                and hasattr(node.func, "id")
-                and node.func.id == "App"
-            ):
-                for keyword in node.keywords:
-                    if keyword.arg == "modules":
-                        if (
-                            isinstance(keyword.value, ast.List)
-                            and len(keyword.value.elts) > 0
-                        ):
-                            # Append to existing list
-                            keyword.value.elts.append(
-                                ast.Name(id=self.class_name, ctx=ast.Load())
-                            )
-                        else:
-                            # Create a new list with the module
-                            keyword.value = ast.List(
-                                elts=[ast.Name(id=self.class_name, ctx=ast.Load())],
-                                ctx=ast.Load(),
-                            )
-                        modified = True
-                        break
+            # Check if the node is a ClassDef with a decorator named 'Module'
+            if isinstance(node, ast.ClassDef):
+                for decorator in node.decorator_list:
+                    if (
+                        isinstance(decorator, ast.Call)
+                        and hasattr(decorator.func, "id")
+                        and decorator.func.id == "Module"
+                    ):
+                        for keyword in decorator.keywords:
+                            if keyword.arg == "imports":
+                                # Append to existing imports list
+                                if isinstance(keyword.value, ast.List):
+                                    keyword.value.elts.append(
+                                        ast.Name(id=self.class_name, ctx=ast.Load())
+                                    )
+                                    modified = True
+                                break
 
         if modified:
             with open(path_to_app_py, "w") as file:
                 file.write(astor.to_source(tree))
             self.format_with_black(path_to_app_py)
 
     def validate_new_module(self, module_name: str):
```

### Comparing `pynest-api-0.1.3/nest/common/templates/blank_template.py` & `pynest-api-0.2.0/nest/common/templates/blank_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,69 @@
+from abc import ABC
 from pathlib import Path
 
 from nest.common.templates.base_template import BaseTemplate
-from abc import ABC
 
 
 class BlankTemplate(BaseTemplate, ABC):
     def __init__(self, module_name: str):
         super().__init__(module_name)
 
     def app_file(self):
-        return f"""from nest.core.app import App
+        return f"""from nest.core import PyNestFactory, Module
+        
+from .app_controller import AppController
+from .app_service import AppService
+
 
+@Module(imports=[], controllers=[AppController], providers=[AppService])
+class AppModule:
+    pass
 
-app = App(
-    description="PyNest service",
-    modules=[]
+
+app = PyNestFactory.create(
+    AppModule,
+    description="This is my PyNest app.",
+    title="PyNest Application",
+    version="1.0.0",
+    debug=True,
 )
+
+http_server = app.get_server()
+
                 """
 
     def config_file(self):
         pass
 
     def docker_file(self):
         pass
 
     def dockerignore_file(self):
         pass
 
     def gitignore_file(self):
         pass
 
-    def module_file(self):
-        return f"""from .{self.module_name}_controller import {self.capitalized_module_name}Controller
-from .{self.module_name}_service import {self.capitalized_module_name}Service
-
-
-class {self.capitalized_module_name}Module:
-
-    def __init__(self):
-        self.controllers = [{self.capitalized_module_name}Controller]
-        self.providers = [{self.capitalized_module_name}Service]
-
-"""
-
     def model_file(self):
         return f"""from pydantic import BaseModel
 
 
 class {self.capitalized_module_name}(BaseModel):
     name: str
 
 """
 
     def service_file(self):
         return f"""from .{self.module_name}_model import {self.capitalized_module_name}
 from functools import lru_cache
+from nest.core import Injectable
 
 
-@lru_cache()
+@Injectable
 class {self.capitalized_module_name}Service:
 
     def __init__(self):
         self.database = []
         
     def get_{self.module_name}(self):
         return self.database
@@ -69,31 +71,32 @@
     def add_{self.module_name}(self, {self.module_name}: {self.capitalized_module_name}):
         self.database.append({self.module_name})
         return {self.module_name}
         
 """
 
     def controller_file(self):
-        return f"""from nest.core import Controller, Get, Post, Depends
+        return f"""from nest.core import Controller, Get, Post
 from .{self.module_name}_service import {self.capitalized_module_name}Service
 from .{self.module_name}_model import {self.capitalized_module_name}
 
 
 @Controller("{self.module_name}")
 class {self.capitalized_module_name}Controller:
 
-    service: {self.capitalized_module_name}Service = Depends({self.capitalized_module_name}Service)
+    def __init__(self, {self.module_name}_service: {self.capitalized_module_name}Service):
+        self.{self.module_name}_service = {self.module_name}_service
     
     @Get("/")
     def get_{self.module_name}(self):
-        return self.service.get_{self.module_name}()
+        return self.{self.module_name}_service.get_{self.module_name}()
         
     @Post("/")
     def add_{self.module_name}(self, {self.module_name}: {self.capitalized_module_name}):
-        return self.service.add_{self.module_name}({self.module_name})
+        return self.{self.module_name}_service.add_{self.module_name}({self.module_name})
 
 """
 
     def entity_file(self):
         pass
 
     def create_module(self, module_name: str, src_path: Path):
@@ -106,34 +109,36 @@
         self.create_template(
             module_path / f"{module_name}_controller.py", self.controller_file()
         )
         self.create_template(
             module_path / f"{module_name}_service.py", self.service_file()
         )
         self.create_template(module_path / f"{module_name}_model.py", self.model_file())
-        self.append_module_to_app(path_to_app_py=src_path.parent / "app.py")
+        self.append_module_to_app(path_to_app_py=src_path / "app_module.py")
 
     def generate_module(self, module_name: str):
         src_path = self.validate_new_module(module_name)
         self.create_module(module_name, src_path)
 
     def generate_project(self, project_name: str):
         self.create_template(self.nest_path / "settings.yaml", self.settings_file())
         root = self.base_path / project_name
         src_path = root / "src"
         self.create_folder(root)
         self.create_template(root / "main.py", self.main_file())
-        self.create_template(root / "app.py", self.app_file())
         self.create_template(root / "README.md", self.readme_file())
         self.create_template(root / "requirements.txt", self.requirements_file())
         self.create_folder(src_path)
         self.create_template(src_path / "__init__.py", "")
+        self.create_template(src_path / "app_module.py", self.app_file())
+        self.create_template(src_path / "app_controller.py", self.app_controller_file())
+        self.create_template(src_path / "app_service.py", self.app_service_file())
 
     def settings_file(self):
-        return f"""# This file is used to configure the nest server.
+        return f"""# This file is used to configure the nest cli.
 config:
     db_type: null
     is_async: false
 """
 
     def requirements_file(self):
         return f"""pynest-api=={self.version}"""
```

### Comparing `pynest-api-0.1.3/nest/common/templates/mongo_template.py` & `pynest-api-0.2.0/nest/common/templates/mongo_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import ast
 from abc import ABC
 from pathlib import Path
-from nest.common.templates.orm_template import AsyncORMTemplate
+
 from nest.common.templates import Database
+from nest.common.templates.orm_template import AsyncORMTemplate
 
 
 class MongoTemplate(AsyncORMTemplate, ABC):
     def __init__(self, module_name: str):
         super().__init__(
             module_name=module_name,
             db_type=Database.MONGODB,
@@ -39,53 +40,54 @@
         return ""
 
     def entity_file(self):
         return f"""from beanie import Document
         
         
 class {self.capitalized_module_name}(Document):
-    title: str
+    name: str
     
     class Config:
         schema_extra = {{
             "example": {{
-                "title": "Example Title",
+                "name": "Example Name",
             }}
         }}
 """
 
     def controller_file(self):
-        return f"""from nest.core import Controller, Get, Post, Depends
+        return f"""from nest.core import Controller, Get, Post
 
 from .{self.module_name}_service import {self.capitalized_module_name}Service
 from .{self.module_name}_model import {self.capitalized_module_name}
 
 
 @Controller("{self.module_name}")
 class {self.capitalized_module_name}Controller:
 
-    service: {self.capitalized_module_name}Service = Depends({self.capitalized_module_name}Service)
+    def __init__(self, {self.module_name}_service: {self.capitalized_module_name}Service):
+        self.service = service
 
     @Get("/")
     async def get_{self.module_name}(self):
-        return await self.service.get_{self.module_name}()
+        return await self.{self.module_name}_service.get_{self.module_name}()
 
     @Post("/")
     async def add_{self.module_name}(self, {self.module_name}: {self.capitalized_module_name}):
-        return await self.service.add_{self.module_name}({self.module_name})
+        return await self.{self.module_name}_service.add_{self.module_name}({self.module_name})
  """
 
     def service_file(self):
         return f"""from .{self.module_name}_model import {self.capitalized_module_name}
 from .{self.module_name}_entity import {self.capitalized_module_name} as {self.capitalized_module_name}Entity
-from nest.core.decorators import db_request_handler
-from functools import lru_cache
+from nest.core.decorators.database import db_request_handler
+from nest.core import Injectable
 
 
-@lru_cache()
+@Injectable
 class {self.capitalized_module_name}Service:
 
     @db_request_handler
     async def add_{self.module_name}(self, {self.module_name}: {self.capitalized_module_name}):
         new_{self.module_name} = {self.capitalized_module_name}Entity(
             **{self.module_name}.dict()
         )
```

### Comparing `pynest-api-0.1.3/nest/common/templates/mysql_template.py` & `pynest-api-0.2.0/nest/common/templates/mysql_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC
 
-from nest.common.templates.orm_template import ORMTemplate, AsyncORMTemplate
 from nest.common.templates import Database
+from nest.common.templates.orm_template import AsyncORMTemplate, ORMTemplate
 
 
 class MySQLTemplate(ORMTemplate, ABC):
     def __init__(self, module_name: str):
         super().__init__(
             module_name=module_name,
             db_type=Database.MYSQL,
```

### Comparing `pynest-api-0.1.3/nest/common/templates/orm_template.py` & `pynest-api-0.2.0/nest/common/templates/orm_template.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
 
-from nest.common.templates.base_template import BaseTemplate, get_module_strings
 from nest.common.templates import Database
+from nest.common.templates.base_template import BaseTemplate
 
 
 class ORMTemplate(BaseTemplate, ABC):
     def __init__(self, module_name: str, db_type: Database):
         super().__init__(
             module_name=module_name,
         )
         self.db_type = db_type
 
     def app_file(self):
-        return f"""from config import config
-from nest.core.app import App
-
-app = App(
-    description="PyNest service",
-    modules=[]
+        return f"""from nest.core import PyNestFactory, Module
+from .config import config
+from .app_controller import AppController
+from .app_service import AppService
+
+
+@Module(imports=[], controllers=[AppController], providers=[AppService])
+class AppModule:
+    pass
+
+
+app = PyNestFactory.create(
+    AppModule,
+    description="This is my PyNest app.",
+    title="PyNest Application",
+    version="1.0.0",
+    debug=True,
 )
 
+http_server = app.get_server()
 
-@app.on_event("startup")
+@http_server.on_event("startup")
 def startup():
     config.create_all()
 """
 
     @abstractmethod
     def config_file(self):
         raise NotImplementedError
@@ -52,57 +64,45 @@
 *.pyc
 *.pyo
 *.pyd
 .DS_Store
 .env
 """
 
-    def module_file(self):
-        return f"""from .{self.module_name}_service import {self.capitalized_module_name}Service
-from .{self.module_name}_controller import {self.capitalized_module_name}Controller
-
-
-class {self.capitalized_module_name}Module:
-
-    def __init__(self):
-        self.providers = [{self.capitalized_module_name}Service]
-        self.controllers = [{self.capitalized_module_name}Controller]
-"""
-
     def model_file(self):
         return f"""from pydantic import BaseModel
 
 
 class {self.capitalized_module_name}(BaseModel):
     name: str
 
 """
 
     def entity_file(self):
-        return f"""from config import config
+        return f"""from src.config import config
 from sqlalchemy import Column, Integer, String, Float
     
     
 class {self.capitalized_module_name}(config.Base):
     __tablename__ = "{self.module_name}"
     
     id = Column(Integer, primary_key=True, autoincrement=True)
     name = Column(String, unique=True)
 
 """
 
     def service_file(self):
         return f"""from .{self.module_name}_model import {self.capitalized_module_name}
 from .{self.module_name}_entity import {self.capitalized_module_name} as {self.capitalized_module_name}Entity
-from config import config
-from nest.core.decorators import db_request_handler
-from functools import lru_cache
+from src.config import config
+from nest.core.decorators.database import db_request_handler
+from nest.core import Injectable
 
 
-@lru_cache()
+@Injectable
 class {self.capitalized_module_name}Service:
 
     def __init__(self):
         self.config = config
         self.session = self.config.get_db()
     
     @db_request_handler
@@ -117,46 +117,47 @@
     @db_request_handler
     def get_{self.module_name}(self):
         return self.session.query({self.capitalized_module_name}Entity).all()
 
 """
 
     def controller_file(self):
-        return f"""from nest.core import Controller, Get, Post, Depends
+        return f"""from nest.core import Controller, Get, Post
 
 from .{self.module_name}_service import {self.capitalized_module_name}Service
 from .{self.module_name}_model import {self.capitalized_module_name}
 
 
 @Controller("{self.module_name}")
 class {self.capitalized_module_name}Controller:
 
-    service: {self.capitalized_module_name}Service = Depends({self.capitalized_module_name}Service)
+    def __init__(self, {self.module_name}_service: {self.capitalized_module_name}Service):
+        self.{self.module_name}_service = {self.module_name}_service
     
     @Get("/")
     def get_{self.module_name}(self):
-        return self.service.get_{self.module_name}()
+        return self.{self.module_name}_service.get_{self.module_name}()
                 
     @Post("/")
     def add_{self.module_name}(self, {self.module_name}: {self.capitalized_module_name}):
-        return self.service.add_{self.module_name}({self.module_name})
+        return self.{self.module_name}_service.add_{self.module_name}({self.module_name})
  """
 
     def settings_file(self):
         return f"""# This file is used to configure the nest server.
 config:
     db_type: {self.db_type.value}
     is_async: false
 """
 
     @staticmethod
     def validate_config_file(src_path: Path) -> Path:
-        config_file = src_path.parent / "config.py"
+        config_file = src_path / "config.py"
         if not config_file.exists():
-            raise Exception("orm_config.py file not found")
+            raise Exception("config.py file not found")
         return config_file
 
     def create_module(self, module_name: str, src_path: Path):
         module_path = src_path / module_name
         self.create_folder(module_path)
         self.create_template(module_path / "__init__.py", "")
         self.create_template(
@@ -168,15 +169,15 @@
         self.create_template(
             module_path / f"{module_name}_service.py", self.service_file()
         )
         self.create_template(module_path / f"{module_name}_model.py", self.model_file())
         self.create_template(
             module_path / f"{module_name}_entity.py", self.entity_file()
         )
-        self.append_module_to_app(src_path.parent / "app.py")
+        self.append_module_to_app(src_path / "app_module.py")
 
     def generate_module(self, module_name: str):
         src_path = self.validate_new_module(module_name)
         self.validate_config_file(src_path)
         self.create_module(module_name, src_path)
 
     def generate_project(self, project_name: str):
@@ -188,49 +189,64 @@
         # create folders
         self.create_folder(root_path)
         self.create_folder(src_path)
 
         # create root level files
         self.create_template(root_path / "main.py", self.main_file())
         self.create_template(root_path / "README.md", self.readme_file())
-        self.create_template(root_path / "app.py", self.app_file())
-        self.create_template(root_path / "config.py", self.config_file())
         self.create_template(root_path / "requirements.txt", self.requirements_file())
         self.create_template(root_path / ".gitignore", self.gitignore_file())
 
         # create src level files
         self.create_template(src_path / "__init__.py", "")
+        self.create_template(src_path / "app_module.py", self.app_file())
+        self.create_template(src_path / "app_controller.py", self.app_controller_file())
+        self.create_template(src_path / "app_service.py", self.app_service_file())
+        self.create_template(src_path / "config.py", self.config_file())
 
 
 class AsyncORMTemplate(ORMTemplate, ABC):
     def app_file(self):
-        return f"""from config import config
-from nest.core.app import App
-
-app = App(
-    description="PyNest service",
-    modules=[]
+        return f"""from nest.core import PyNestFactory, Module
+from .config import config
+from .app_controller import AppController
+from .app_service import AppService
+
+
+@Module(imports=[], controllers=[AppController], providers=[AppService])
+class AppModule:
+    pass
+
+
+app = PyNestFactory.create(
+    AppModule,
+    description="This is my Async PyNest app.",
+    title="PyNest Application",
+    version="1.0.0",
+    debug=True,
 )
 
+http_server = app.get_server()
 
-@app.on_event("startup")
+@http_server.on_event("startup")
 async def startup():
     await config.create_all()
+    
 """
 
     @abstractmethod
     def config_file(self):
         pass
 
     @abstractmethod
     def requirements_file(self):
         pass
 
     def entity_file(self):
-        return f"""from config import config
+        return f"""from src.config import config
 from sqlalchemy import Integer, String
 from sqlalchemy.orm import Mapped, mapped_column
 
 
 class {self.capitalized_module_name}(config.Base):
     __tablename__ = "{self.module_name}"
 
@@ -238,20 +254,21 @@
     name: Mapped[str] = mapped_column(String, unique=True)
 
 """
 
     def service_file(self):
         return f"""from .{self.module_name}_model import {self.capitalized_module_name}
 from .{self.module_name}_entity import {self.capitalized_module_name} as {self.capitalized_module_name}Entity
-from nest.core.decorators import async_db_request_handler
+from nest.core.decorators.database import async_db_request_handler
+from nest.core import Injectable
 
 from sqlalchemy import select
 from sqlalchemy.ext.asyncio import AsyncSession
 
-
+@Injectable
 class {self.capitalized_module_name}Service:
 
     @async_db_request_handler
     async def add_{self.module_name}(self, {self.module_name}: {self.capitalized_module_name}, session: AsyncSession):
         new_{self.module_name} = {self.capitalized_module_name}Entity(
             **{self.module_name}.dict()
         )
@@ -265,33 +282,34 @@
         result = await session.execute(query)
         return result.scalars().all()
 """
 
     def controller_file(self):
         return f"""from nest.core import Controller, Get, Post, Depends
 from sqlalchemy.ext.asyncio import AsyncSession
-from config import config
+from src.config import config
 
 
 from .{self.module_name}_service import {self.capitalized_module_name}Service
 from .{self.module_name}_model import {self.capitalized_module_name}
 
 
 @Controller("{self.module_name}")
 class {self.capitalized_module_name}Controller:
 
-    service: {self.capitalized_module_name}Service = Depends({self.capitalized_module_name}Service)
+    def __init__(self, {self.module_name}_service: {self.capitalized_module_name}Service):
+        self.{self.module_name}_service = {self.module_name}_service
 
     @Get("/")
     async def get_{self.module_name}(self, session: AsyncSession = Depends(config.get_db)):
-        return await self.service.get_{self.module_name}(session)
+        return await self.{self.module_name}_service.get_{self.module_name}(session)
 
     @Post("/")
     async def add_{self.module_name}(self, {self.module_name}: {self.capitalized_module_name}, session: AsyncSession = Depends(config.get_db)):
-        return await self.service.add_{self.module_name}({self.module_name}, session)
+        return await self.{self.module_name}_service.add_{self.module_name}({self.module_name}, session)
  """
 
     def settings_file(self):
         return f"""# This file is used to configure the nest server.
 config:
     db_type: {self.db_type.value}
     is_async: true
```

### Comparing `pynest-api-0.1.3/nest/common/templates/postgres_template.py` & `pynest-api-0.2.0/nest/common/templates/postgres_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC
 
-from nest.common.templates.orm_template import ORMTemplate, AsyncORMTemplate
 from nest.common.templates import Database
+from nest.common.templates.orm_template import AsyncORMTemplate, ORMTemplate
 
 
 class PostgresqlTemplate(ORMTemplate, ABC):
     def __init__(self, module_name: str):
         super().__init__(
             module_name=module_name,
             db_type=Database.POSTGRESQL,
```

### Comparing `pynest-api-0.1.3/nest/common/templates/sqlite_template.py` & `pynest-api-0.2.0/nest/common/templates/sqlite_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC
 
-from nest.common.templates.orm_template import ORMTemplate, AsyncORMTemplate
 from nest.common.templates import Database
+from nest.common.templates.orm_template import AsyncORMTemplate, ORMTemplate
 
 
 class SQLiteTemplate(ORMTemplate, ABC):
     def __init__(self, module_name: str):
         super().__init__(
             module_name=module_name,
             db_type=Database.SQLITE,
```

### Comparing `pynest-api-0.1.3/nest/common/templates/templates_factory.py` & `pynest-api-0.2.0/nest/common/templates/templates_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from typing import Optional, Union
+
+from nest.common.templates import Database
+from nest.common.templates.base_template import BaseTemplate
+from nest.common.templates.blank_template import BlankTemplate
+from nest.common.templates.mongo_template import MongoTemplate
+from nest.common.templates.mysql_template import AsyncMySQLTemplate, MySQLTemplate
 from nest.common.templates.postgres_template import (
-    PostgresqlTemplate,
     AsyncPostgresqlTemplate,
+    PostgresqlTemplate,
 )
-from nest.common.templates.sqlite_template import SQLiteTemplate, AsyncSQLiteTemplate
-from nest.common.templates.mysql_template import MySQLTemplate, AsyncMySQLTemplate
-from nest.common.templates.mongo_template import MongoTemplate
-from nest.common.templates.base_template import BaseTemplate
-from nest.common.templates.blank_template import BlankTemplate
-from nest.common.templates import Database
-from typing import Union, Optional
+from nest.common.templates.sqlite_template import AsyncSQLiteTemplate, SQLiteTemplate
 
 
 class TemplateFactory:
     @staticmethod
     def get_template(
         db_type: Union[Database, str, None],
         module_name: str,
```

### Comparing `pynest-api-0.1.3/nest/core/database/base_config.py` & `pynest-api-0.2.0/nest/core/database/base_config.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.1.3/nest/core/database/odm_config.py` & `pynest-api-0.2.0/nest/core/database/odm_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nest.core.database.base_config import ConfigFactoryBase, BaseProvider
+from nest.core.database.base_config import BaseProvider, ConfigFactoryBase
 
 
 class MongoDBConfig(BaseProvider):
     """
     ODM configuration for MongoDB.
 
     Args:
```

### Comparing `pynest-api-0.1.3/nest/core/database/odm_provider.py` & `pynest-api-0.2.0/nest/core/database/odm_provider.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
-from motor.motor_asyncio import AsyncIOMotorClient
 from beanie import Document, init_beanie
+from motor.motor_asyncio import AsyncIOMotorClient
 
 from nest.core.database.odm_config import ConfigFactory
 
 
 class OdmProvider:
     """
     Provides an interface for working with an ODM (Object-Document Mapping).
```

### Comparing `pynest-api-0.1.3/nest/core/database/orm_config.py` & `pynest-api-0.2.0/nest/core/database/orm_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nest.core.database.base_config import ConfigFactoryBase, BaseProvider, BaseConfig
+from nest.core.database.base_config import BaseConfig, BaseProvider, ConfigFactoryBase
 
 
 class PostgresConfig(BaseProvider):
     """
     ORM configuration for PostgreSQL.
 
     Args:
```

### Comparing `pynest-api-0.1.3/nest/core/database/orm_provider.py` & `pynest-api-0.2.0/nest/core/database/orm_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from abc import ABC, abstractmethod
 from contextlib import asynccontextmanager
-from typing import Dict, Any
+from typing import Any, Dict
 
 from sqlalchemy import create_engine
-from sqlalchemy.ext.asyncio import create_async_engine, async_sessionmaker, AsyncSession
-from sqlalchemy.orm import sessionmaker, Session, DeclarativeBase
+from sqlalchemy.ext.asyncio import AsyncSession, async_sessionmaker, create_async_engine
+from sqlalchemy.orm import DeclarativeBase, Session, sessionmaker
 
-from nest.core.database.orm_config import ConfigFactory, AsyncConfigFactory
+from nest.core.database.orm_config import AsyncConfigFactory, ConfigFactory
 
 
 class Base(DeclarativeBase):
     """
     Base class for ORM models.
     """
```

### Comparing `pynest-api-0.1.3/nest/core/decorators/database.py` & `pynest-api-0.2.0/nest/core/decorators/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from fastapi.exceptions import HTTPException
 import logging
 import time
+
+from fastapi.exceptions import HTTPException
 from sqlalchemy.ext.asyncio import AsyncSession
 
 logging.basicConfig(level=logging.DEBUG)
 logger = logging.getLogger(__name__)
 
 
 def db_request_handler(func):
```

### Comparing `pynest-api-0.1.3/nest/core/decorators/helpers.py` & `pynest-api-0.2.0/nest/core/decorators/class_based_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Credit: FastAPI-Utils
 Source: https://github.com/dmontagu/fastapi-utils/blob/master/fastapi_utils/cbv.py
 """
 
-
 import inspect
 from typing import Any, Callable, List, Type, TypeVar, Union, get_type_hints
 
 from fastapi import APIRouter, Depends
 from pydantic.typing import is_classvar
 from starlette.routing import Route, WebSocketRoute
```

### Comparing `pynest-api-0.1.3/nest/core/decorators/http_methods.py` & `pynest-api-0.2.0/nest/core/decorators/http_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any
+
 from nest.core.decorators.helpers import route_decorator
 
 
 def Get(path: str, **kwargs: Any):
     """
     Decorator that defines a GET route for the controller.
```

### Comparing `pynest-api-0.1.3/nest/plugins/modules/redis/redis_controller.py` & `pynest-api-0.2.0/nest/plugins/modules/redis/redis_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from nest.core import Controller, Get, Post, Depends, Delete
-
-from nest.plugins.modules.redis.redis_service import RedisService
+from nest.core import Controller, Delete, Depends, Get, Post
 from nest.plugins.modules.redis.redis_model import RedisInput
+from nest.plugins.modules.redis.redis_service import RedisService
 
 
 @Controller("redis")
 class RedisController:
     redis_service: RedisService = Depends(RedisService)
 
     @Get("/{key}")
```

### Comparing `pynest-api-0.1.3/nest/plugins/modules/redis/redis_service.py` & `pynest-api-0.2.0/nest/plugins/modules/redis/redis_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import redis
-
-from functools import lru_cache
 from fastapi import HTTPException
-from nest.plugins.modules.redis.redis_model import RedisInput, RedisConfig
+
+from nest.core import Injectable
+from nest.plugins.modules.redis.redis_model import RedisConfig, RedisInput
 
 
-@lru_cache(maxsize=1)
+@Injectable
 class RedisService:
     def __init__(self):
         self.redis_config = RedisConfig()
         self.redis_client = redis.StrictRedis(
             host=self.redis_config.REDIS_HOST,
             port=self.redis_config.REDIS_PORT,
             db=self.redis_config.REDIS_DB,
```

### Comparing `pynest-api-0.1.3/pynest_api.egg-info/PKG-INFO` & `pynest-api-0.2.0/pynest_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynest-api
-Version: 0.1.3
+Version: 0.2.0
 Summary: PyNest is a FastAPI Abstraction for building microservices, influenced by NestJS.
 Author-email: Itay Dar <itay2803@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 PyNest
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,24 +31,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click==8.1.6
+Requires-Dist: click>=8.1.6
 Requires-Dist: fastapi==0.95.1
-Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: SQLAlchemy==2.0.19
-Requires-Dist: uvicorn==0.23.1
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: astor==0.8.1
-Requires-Dist: black==23.11.0
+Requires-Dist: python-dotenv>=1.0.0
+Requires-Dist: uvicorn>=0.23.1
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: astor>=0.8.1
+Requires-Dist: black>=23.11.0
+Requires-Dist: injector>=0.21.0
+Requires-Dist: pydantic<2.0.0
+Requires-Dist: sqlalchemy==2.0.19
+Requires-Dist: alembic==1.7.4
 Provides-Extra: test
 Requires-Dist: pytest==6.2.5; extra == "test"
+Provides-Extra: orm
+Requires-Dist: sqlalchemy==2.0.19; extra == "orm"
+Requires-Dist: alembic==1.7.4; extra == "orm"
 Provides-Extra: mongo
 Requires-Dist: pymongo==3.12.0; extra == "mongo"
 Requires-Dist: motor==3.2.0; extra == "mongo"
 Requires-Dist: beanie==1.20.0; extra == "mongo"
 
 <p align="center">
   <img src="docs/imgs/pynest-logo.png" title="pynest logo" width="300">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynest-api Version: 0.1.3 Summary: PyNest is a
+Metadata-Version: 2.1 Name: pynest-api Version: 0.2.0 Summary: PyNest is a
 FastAPI Abstraction for building microservices, influenced by NestJS. Author-
 email: Itay Dar
 gmail.com> License: MIT License Copyright (c) 2023 PyNest Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -18,21 +18,24 @@
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/PythonNest/
 PyNest Project-URL: Documentation, https://pythonnest.github.io/PyNest/
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8.1 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: click==8.1.6 Requires-Dist: fastapi==0.95.1 Requires-
-Dist: python-dotenv==1.0.0 Requires-Dist: SQLAlchemy==2.0.19 Requires-Dist:
-uvicorn==0.23.1 Requires-Dist: PyYAML==6.0.1 Requires-Dist: astor==0.8.1
-Requires-Dist: black==23.11.0 Provides-Extra: test Requires-Dist:
-pytest==6.2.5; extra == "test" Provides-Extra: mongo Requires-Dist:
-pymongo==3.12.0; extra == "mongo" Requires-Dist: motor==3.2.0; extra == "mongo"
-Requires-Dist: beanie==1.20.0; extra == "mongo"
+LICENSE Requires-Dist: click>=8.1.6 Requires-Dist: fastapi==0.95.1 Requires-
+Dist: python-dotenv>=1.0.0 Requires-Dist: uvicorn>=0.23.1 Requires-Dist:
+PyYAML>=6.0.1 Requires-Dist: astor>=0.8.1 Requires-Dist: black>=23.11.0
+Requires-Dist: injector>=0.21.0 Requires-Dist: pydantic<2.0.0 Requires-Dist:
+sqlalchemy==2.0.19 Requires-Dist: alembic==1.7.4 Provides-Extra: test Requires-
+Dist: pytest==6.2.5; extra == "test" Provides-Extra: orm Requires-Dist:
+sqlalchemy==2.0.19; extra == "orm" Requires-Dist: alembic==1.7.4; extra ==
+"orm" Provides-Extra: mongo Requires-Dist: pymongo==3.12.0; extra == "mongo"
+Requires-Dist: motor==3.2.0; extra == "mongo" Requires-Dist: beanie==1.20.0;
+extra == "mongo"
                           [docs/imgs/pynest-logo.png]
  PPyyNNeesstt iiss aa PPyytthhoonn ffrraammeewwoorrkk bbuuiilltt oonn ttoopp ooff FFaassttAAPPII tthhaatt ffoolllloowwss tthhee mmoodduullaarr
                             aarrcchhiitteeccttuurree ooff NNeessttJJSS
                      _[_V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]
 # Description PyNest is designed to help structure your APIs in an intuitive,
 easy to understand, and enjoyable way. With PyNest, you can build scalable and
 maintainable APIs with ease. The framework supports dependency injection, type
```

### Comparing `pynest-api-0.1.3/pynest_api.egg-info/SOURCES.txt` & `pynest-api-0.2.0/pynest_api.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,36 +2,47 @@
 README.md
 pyproject.toml
 nest/__init__.py
 nest/cli/__init__.py
 nest/cli/cli.py
 nest/cli/click_handlers.py
 nest/common/__init__.py
+nest/common/constants.py
+nest/common/exceptions.py
+nest/common/module.py
+nest/common/route_resolver.py
 nest/common/templates/__init__.py
 nest/common/templates/base_template.py
 nest/common/templates/blank_template.py
 nest/common/templates/mongo_template.py
 nest/common/templates/mysql_template.py
 nest/common/templates/orm_template.py
 nest/common/templates/postgres_template.py
 nest/common/templates/sqlite_template.py
 nest/common/templates/templates_factory.py
 nest/core/__init__.py
-nest/core/app.py
+nest/core/pynest_app_context.py
+nest/core/pynest_application.py
+nest/core/pynest_container.py
+nest/core/pynest_factory.py
 nest/core/database/__init__.py
 nest/core/database/base_config.py
 nest/core/database/odm_config.py
 nest/core/database/odm_provider.py
 nest/core/database/orm_config.py
 nest/core/database/orm_provider.py
 nest/core/decorators/__init__.py
+nest/core/decorators/class_based_view.py
 nest/core/decorators/controller.py
 nest/core/decorators/database.py
-nest/core/decorators/helpers.py
+nest/core/decorators/http_method.py
 nest/core/decorators/http_methods.py
+nest/core/decorators/injectable.py
+nest/core/decorators/module.py
+nest/core/decorators/utils.py
 nest/plugins/__init__.py
 nest/plugins/controllers/__init__.py
 nest/plugins/modules/__init__.py
 nest/plugins/modules/auth/__init__.py
 nest/plugins/modules/redis/__init__.py
 nest/plugins/modules/redis/redis_controller.py
 nest/plugins/modules/redis/redis_model.py
```

### Comparing `pynest-api-0.1.3/pyproject.toml` & `pynest-api-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,25 @@
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "click==8.1.6",
+    "click>=8.1.6",
     "fastapi==0.95.1",
-    "python-dotenv==1.0.0",
-    "SQLAlchemy==2.0.19",
-    "uvicorn==0.23.1",
-    "PyYAML==6.0.1",
-    "astor==0.8.1",
-    "black==23.11.0"
+    "python-dotenv>=1.0.0",
+    "uvicorn>=0.23.1",
+    "PyYAML>=6.0.1",
+    "astor>=0.8.1",
+    "black>=23.11.0",
+    "injector>=0.21.0",
+    "pydantic<2.0.0",
+    "sqlalchemy == 2.0.19",
+    "alembic == 1.7.4",
 ]
 
 [tool.setuptools.dynamic]
 version = { attr = "nest.__init__.__version__" }
 
 [tool.pip]
 index-url = "https://pypi.org/simple"
@@ -55,14 +58,19 @@
 )/
 '''
 
 [project.optional-dependencies]
 test = [
     "pytest == 6.2.5",
 ]
+
+orm = [
+    "sqlalchemy == 2.0.19",
+    "alembic == 1.7.4",
+]
 mongo = [
     "pymongo == 3.12.0",
     "motor == 3.2.0",
     "beanie == 1.20.0",
 ]
 
 [project.scripts]
```

