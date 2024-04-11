# Comparing `tmp/tutor-17.0.3.tar.gz` & `tmp/tutor-17.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-17.0.3.tar", last modified: Tue Mar 26 13:48:39 2024, max compression
+gzip compressed data, was "tutor-17.0.4.tar", last modified: Thu Apr 11 09:44:08 2024, max compression
```

## Comparing `tutor-17.0.3.tar` & `tutor-17.0.4.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.795933 tutor-17.0.3/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2024-03-26 13:48:03.000000 tutor-17.0.3/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)      150 2024-03-26 13:48:03.000000 tutor-17.0.3/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     6528 2024-03-26 13:48:39.792599 tutor-17.0.3/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     4566 2024-03-26 13:48:03.000000 tutor-17.0.3/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2024-03-26 13:48:03.000000 tutor-17.0.3/pyproject.toml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.755932 tutor-17.0.3/requirements/
--rw-r--r--   0 ci        (1000) ci        (1000)      159 2024-03-26 13:48:03.000000 tutor-17.0.3/requirements/base.in
--rw-r--r--   0 ci        (1000) ci        (1000)     4775 2024-03-26 13:48:03.000000 tutor-17.0.3/requirements/dev.txt
--rw-r--r--   0 ci        (1000) ci        (1000)      433 2024-03-26 13:48:03.000000 tutor-17.0.3/requirements/plugins.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2024-03-26 13:48:39.795933 tutor-17.0.3/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     2580 2024-03-26 13:48:03.000000 tutor-17.0.3/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.765932 tutor-17.0.3/tests/
--rw-r--r--   0 ci        (1000) ci        (1000)     2067 2024-03-26 13:48:03.000000 tutor-17.0.3/tests/test_bindmount.py
--rw-r--r--   0 ci        (1000) ci        (1000)     4172 2024-03-26 13:48:03.000000 tutor-17.0.3/tests/test_config.py
--rw-r--r--   0 ci        (1000) ci        (1000)    15988 2024-03-26 13:48:03.000000 tutor-17.0.3/tests/test_env.py
--rw-r--r--   0 ci        (1000) ci        (1000)     3063 2024-03-26 13:48:03.000000 tutor-17.0.3/tests/test_plugin_indexes.py
--rw-r--r--   0 ci        (1000) ci        (1000)      539 2024-03-26 13:48:03.000000 tutor-17.0.3/tests/test_plugins.py
--rw-r--r--   0 ci        (1000) ci        (1000)     8281 2024-03-26 13:48:03.000000 tutor-17.0.3/tests/test_plugins_v0.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2588 2024-03-26 13:48:03.000000 tutor-17.0.3/tests/test_serialize.py
--rw-r--r--   0 ci        (1000) ci        (1000)    11633 2024-03-26 13:48:03.000000 tutor-17.0.3/tests/test_utils.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.769266 tutor-17.0.3/tutor/
--rw-r--r--   0 ci        (1000) ci        (1000)     1159 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:05.000000 tutor-17.0.3/tutor/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2549 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/bindmount.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.775932 tutor-17.0.3/tutor/commands/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:05.000000 tutor-17.0.3/tutor/commands/__init__.py
--rwxr-xr-x   0 ci        (1000) ci        (1000)     4219 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/cli.py
--rw-r--r--   0 ci        (1000) ci        (1000)    15893 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/compose.py
--rw-r--r--   0 ci        (1000) ci        (1000)     7390 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/config.py
--rw-r--r--   0 ci        (1000) ci        (1000)      794 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/context.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2240 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/dev.py
--rw-r--r--   0 ci        (1000) ci        (1000)    11114 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/images.py
--rw-r--r--   0 ci        (1000) ci        (1000)    13579 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/jobs.py
--rw-r--r--   0 ci        (1000) ci        (1000)    21075 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/k8s.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1772 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/local.py
--rw-r--r--   0 ci        (1000) ci        (1000)     4446 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/mounts.py
--rw-r--r--   0 ci        (1000) ci        (1000)      741 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/params.py
--rw-r--r--   0 ci        (1000) ci        (1000)    13420 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/plugins.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.775932 tutor-17.0.3/tutor/commands/upgrade/
--rw-r--r--   0 ci        (1000) ci        (1000)      213 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/upgrade/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2082 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/upgrade/common.py
--rw-r--r--   0 ci        (1000) ci        (1000)     6117 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/upgrade/compose.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5755 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/commands/upgrade/k8s.py
--rw-r--r--   0 ci        (1000) ci        (1000)    10932 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.775932 tutor-17.0.3/tutor/core/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:05.000000 tutor-17.0.3/tutor/core/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.779266 tutor-17.0.3/tutor/core/hooks/
--rw-r--r--   0 ci        (1000) ci        (1000)      292 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/core/hooks/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5707 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/core/hooks/actions.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2929 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/core/hooks/contexts.py
--rw-r--r--   0 ci        (1000) ci        (1000)     9006 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/core/hooks/filters.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1007 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/core/hooks/priorities.py
--rw-r--r--   0 ci        (1000) ci        (1000)    17927 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/env.py
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/exceptions.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1213 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/fmt.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.779266 tutor-17.0.3/tutor/hooks/
--rw-r--r--   0 ci        (1000) ci        (1000)     1195 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/hooks/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)    27389 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/hooks/catalog.py
--rw-r--r--   0 ci        (1000) ci        (1000)      673 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/images.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5182 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/interactive.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.779266 tutor-17.0.3/tutor/plugins/
--rw-r--r--   0 ci        (1000) ci        (1000)     3484 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/plugins/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      548 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/plugins/base.py
--rw-r--r--   0 ci        (1000) ci        (1000)     6935 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/plugins/indexes.py
--rw-r--r--   0 ci        (1000) ci        (1000)     4582 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/plugins/openedx.py
--rw-r--r--   0 ci        (1000) ci        (1000)    15220 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/plugins/v0.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2482 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/plugins/v1.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:05.000000 tutor-17.0.3/tutor/py.typed
--rw-r--r--   0 ci        (1000) ci        (1000)     2180 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/serialize.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1385 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/tasks.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.779266 tutor-17.0.3/tutor/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.752599 tutor-17.0.3/tutor/templates/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.779266 tutor-17.0.3/tutor/templates/apps/caddy/
--rw-r--r--   0 ci        (1000) ci        (1000)     1989 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/caddy/Caddyfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.779266 tutor-17.0.3/tutor/templates/apps/openedx/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.782599 tutor-17.0.3/tutor/templates/apps/openedx/config/
--rw-r--r--   0 ci        (1000) ci        (1000)     1542 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/config/cms.env.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1787 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/config/lms.env.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.782599 tutor-17.0.3/tutor/templates/apps/openedx/config/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)      743 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/config/partials/auth.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.749266 tutor-17.0.3/tutor/templates/apps/openedx/settings/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.782599 tutor-17.0.3/tutor/templates/apps/openedx/settings/cms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:05.000000 tutor-17.0.3/tutor/templates/apps/openedx/settings/cms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      661 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/settings/cms/development.py
--rw-r--r--   0 ci        (1000) ci        (1000)      529 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/settings/cms/production.py
--rw-r--r--   0 ci        (1000) ci        (1000)       91 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/settings/cms/test.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.782599 tutor-17.0.3/tutor/templates/apps/openedx/settings/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:05.000000 tutor-17.0.3/tutor/templates/apps/openedx/settings/lms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1132 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/settings/lms/development.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1039 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/settings/lms/production.py
--rw-r--r--   0 ci        (1000) ci        (1000)       91 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/settings/lms/test.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.785932 tutor-17.0.3/tutor/templates/apps/openedx/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)    10504 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/settings/partials/common_all.py
--rw-r--r--   0 ci        (1000) ci        (1000)      961 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/settings/partials/common_cms.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1450 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/settings/partials/common_lms.py
--rw-r--r--   0 ci        (1000) ci        (1000)      105 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/settings/partials/common_test.py
--rw-r--r--   0 ci        (1000) ci        (1000)       78 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/openedx/uwsgi.ini
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.785932 tutor-17.0.3/tutor/templates/apps/permissions/
--rw-r--r--   0 ci        (1000) ci        (1000)      380 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/permissions/setowners.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.785932 tutor-17.0.3/tutor/templates/apps/redis/
--rw-r--r--   0 ci        (1000) ci        (1000)     1008 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/apps/redis/redis.conf
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.752599 tutor-17.0.3/tutor/templates/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.785932 tutor-17.0.3/tutor/templates/build/openedx/
--rw-r--r--   0 ci        (1000) ci        (1000)    12940 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.785932 tutor-17.0.3/tutor/templates/build/openedx/bin/
--rwxr-xr-x   0 ci        (1000) ci        (1000)     7042 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/bin/openedx-assets
--rwxr-xr-x   0 ci        (1000) ci        (1000)      116 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/bin/reload-uwsgi
--rw-r--r--   0 ci        (1000) ci        (1000)     2329 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/bin/site-configuration
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.785932 tutor-17.0.3/tutor/templates/build/openedx/locale/
--rw-r--r--   0 ci        (1000) ci        (1000)      438 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/locale/customlocales.md
--rw-r--r--   0 ci        (1000) ci        (1000)       30 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/revisions.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.785932 tutor-17.0.3/tutor/templates/build/openedx/settings/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.789266 tutor-17.0.3/tutor/templates/build/openedx/settings/cms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:05.000000 tutor-17.0.3/tutor/templates/build/openedx/settings/cms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      317 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/settings/cms/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)       56 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/settings/cms/i18n.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.789266 tutor-17.0.3/tutor/templates/build/openedx/settings/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:05.000000 tutor-17.0.3/tutor/templates/build/openedx/settings/lms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      306 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/settings/lms/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)       56 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/settings/lms/i18n.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.789266 tutor-17.0.3/tutor/templates/build/openedx/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)      441 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/settings/partials/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)      420 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/settings/partials/i18n.py
--rw-r--r--   0 ci        (1000) ci        (1000)      262 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/settings/uwsgi.ini
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.789266 tutor-17.0.3/tutor/templates/build/openedx/themes/
--rw-r--r--   0 ci        (1000) ci        (1000)       75 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/openedx/themes/README
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.789266 tutor-17.0.3/tutor/templates/build/permissions/
--rw-r--r--   0 ci        (1000) ci        (1000)      189 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/permissions/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      302 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/build/permissions/setowner.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.789266 tutor-17.0.3/tutor/templates/config/
--rw-r--r--   0 ci        (1000) ci        (1000)      518 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/config/base.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2901 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/config/defaults.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.789266 tutor-17.0.3/tutor/templates/dev/
--rw-r--r--   0 ci        (1000) ci        (1000)      799 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/dev/docker-compose.jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1353 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/dev/docker-compose.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.755932 tutor-17.0.3/tutor/templates/jobs/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.792599 tutor-17.0.3/tutor/templates/jobs/init/
--rw-r--r--   0 ci        (1000) ci        (1000)      781 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/jobs/init/cms.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1807 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/jobs/init/lms.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1569 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/jobs/init/mounted-directories.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1455 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/jobs/init/mysql.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.792599 tutor-17.0.3/tutor/templates/k8s/
--rw-r--r--   0 ci        (1000) ci        (1000)    13048 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/k8s/deployments.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2090 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/k8s/jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)      125 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/k8s/namespace.yml
--rw-r--r--   0 ci        (1000) ci        (1000)       28 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/k8s/override.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2465 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/k8s/services.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1428 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/k8s/volumes.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2142 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/kustomization.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.792599 tutor-17.0.3/tutor/templates/local/
--rw-r--r--   0 ci        (1000) ci        (1000)     2207 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/local/docker-compose.jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1017 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/local/docker-compose.prod.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     6608 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/local/docker-compose.yml
--rw-r--r--   0 ci        (1000) ci        (1000)       19 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/templates/version
--rw-r--r--   0 ci        (1000) ci        (1000)     1327 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/types.py
--rw-r--r--   0 ci        (1000) ci        (1000)    10766 2024-03-26 13:48:03.000000 tutor-17.0.3/tutor/utils.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-26 13:48:39.772599 tutor-17.0.3/tutor.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     6528 2024-03-26 13:48:39.000000 tutor-17.0.3/tutor.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     4103 2024-03-26 13:48:39.000000 tutor-17.0.3/tutor.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2024-03-26 13:48:39.000000 tutor-17.0.3/tutor.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       51 2024-03-26 13:48:39.000000 tutor-17.0.3/tutor.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)     1840 2024-03-26 13:48:39.000000 tutor-17.0.3/tutor.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        6 2024-03-26 13:48:39.000000 tutor-17.0.3/tutor.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.376849 tutor-17.0.4/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2024-04-11 09:43:37.000000 tutor-17.0.4/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)      150 2024-04-11 09:43:37.000000 tutor-17.0.4/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     6528 2024-04-11 09:44:08.376849 tutor-17.0.4/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     4566 2024-04-11 09:43:37.000000 tutor-17.0.4/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2024-04-11 09:43:37.000000 tutor-17.0.4/pyproject.toml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.353516 tutor-17.0.4/requirements/
+-rw-r--r--   0 ci        (1000) ci        (1000)      159 2024-04-11 09:43:37.000000 tutor-17.0.4/requirements/base.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     4775 2024-04-11 09:43:37.000000 tutor-17.0.4/requirements/dev.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)      433 2024-04-11 09:43:37.000000 tutor-17.0.4/requirements/plugins.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2024-04-11 09:44:08.376849 tutor-17.0.4/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     2580 2024-04-11 09:43:37.000000 tutor-17.0.4/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.353516 tutor-17.0.4/tests/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2067 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_bindmount.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     4172 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_config.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15988 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_env.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     3063 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_plugin_indexes.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      539 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_plugins.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     8281 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_plugins_v0.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2588 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_serialize.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    11633 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_utils.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.356849 tutor-17.0.4/tutor/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1159 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2549 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/bindmount.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.360182 tutor-17.0.4/tutor/commands/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/commands/__init__.py
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     4219 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/cli.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15893 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/compose.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     7390 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/config.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      794 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/context.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2240 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/dev.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    11114 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/images.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    13579 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/jobs.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    21075 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/k8s.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1772 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/local.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     4446 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/mounts.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      741 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/params.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    13420 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/plugins.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.360182 tutor-17.0.4/tutor/commands/upgrade/
+-rw-r--r--   0 ci        (1000) ci        (1000)      213 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/upgrade/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2082 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/upgrade/common.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     6117 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/upgrade/compose.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5755 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/upgrade/k8s.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    10932 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.360182 tutor-17.0.4/tutor/core/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/core/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.363516 tutor-17.0.4/tutor/core/hooks/
+-rw-r--r--   0 ci        (1000) ci        (1000)      292 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/core/hooks/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5707 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/core/hooks/actions.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2929 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/core/hooks/contexts.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     9006 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/core/hooks/filters.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1007 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/core/hooks/priorities.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    17927 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/env.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/exceptions.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1213 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/fmt.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.363516 tutor-17.0.4/tutor/hooks/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1195 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/hooks/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    27389 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/hooks/catalog.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      673 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/images.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5182 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/interactive.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.363516 tutor-17.0.4/tutor/plugins/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3484 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/plugins/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      548 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/plugins/base.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     6935 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/plugins/indexes.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     4582 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/plugins/openedx.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15220 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/plugins/v0.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2482 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/plugins/v1.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/py.typed
+-rw-r--r--   0 ci        (1000) ci        (1000)     2180 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/serialize.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1385 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/tasks.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.363516 tutor-17.0.4/tutor/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.346849 tutor-17.0.4/tutor/templates/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.363516 tutor-17.0.4/tutor/templates/apps/caddy/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1989 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/caddy/Caddyfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.363516 tutor-17.0.4/tutor/templates/apps/openedx/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.366849 tutor-17.0.4/tutor/templates/apps/openedx/config/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1542 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/config/cms.env.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1787 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/config/lms.env.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.366849 tutor-17.0.4/tutor/templates/apps/openedx/config/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)      743 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/config/partials/auth.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.346849 tutor-17.0.4/tutor/templates/apps/openedx/settings/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.366849 tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      661 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/development.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      529 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/production.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       91 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/test.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1132 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/development.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1039 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/production.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       91 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/test.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)    10504 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_all.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      961 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_cms.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1450 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_lms.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      105 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_test.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       78 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/uwsgi.ini
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/apps/permissions/
+-rw-r--r--   0 ci        (1000) ci        (1000)      380 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/permissions/setowners.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/apps/redis/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1008 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/redis/redis.conf
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.350182 tutor-17.0.4/tutor/templates/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/build/openedx/
+-rw-r--r--   0 ci        (1000) ci        (1000)    12940 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/build/openedx/bin/
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     7042 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/bin/openedx-assets
+-rwxr-xr-x   0 ci        (1000) ci        (1000)      116 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/bin/reload-uwsgi
+-rw-r--r--   0 ci        (1000) ci        (1000)     2329 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/bin/site-configuration
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/build/openedx/locale/
+-rw-r--r--   0 ci        (1000) ci        (1000)      438 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/locale/customlocales.md
+-rw-r--r--   0 ci        (1000) ci        (1000)       30 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/revisions.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/build/openedx/settings/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/build/openedx/settings/cms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/cms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      317 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/cms/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       56 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/cms/i18n.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/build/openedx/settings/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/lms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      306 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/lms/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       56 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/lms/i18n.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/build/openedx/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)      441 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/partials/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      420 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/partials/i18n.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      262 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/uwsgi.ini
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/build/openedx/themes/
+-rw-r--r--   0 ci        (1000) ci        (1000)       75 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/themes/README
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/build/permissions/
+-rw-r--r--   0 ci        (1000) ci        (1000)      189 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/permissions/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      302 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/permissions/setowner.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/config/
+-rw-r--r--   0 ci        (1000) ci        (1000)      518 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/config/base.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2901 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/config/defaults.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/dev/
+-rw-r--r--   0 ci        (1000) ci        (1000)      799 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/dev/docker-compose.jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1353 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/dev/docker-compose.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.350182 tutor-17.0.4/tutor/templates/jobs/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/jobs/init/
+-rw-r--r--   0 ci        (1000) ci        (1000)      781 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/jobs/init/cms.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1807 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/jobs/init/lms.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1569 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/jobs/init/mounted-directories.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1455 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/jobs/init/mysql.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/k8s/
+-rw-r--r--   0 ci        (1000) ci        (1000)    13048 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/k8s/deployments.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2090 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/k8s/jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)      125 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/k8s/namespace.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)       28 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/k8s/override.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2465 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/k8s/services.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1428 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/k8s/volumes.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2142 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/kustomization.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.376849 tutor-17.0.4/tutor/templates/local/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2207 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/local/docker-compose.jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1017 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/local/docker-compose.prod.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     6608 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/local/docker-compose.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)       19 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/version
+-rw-r--r--   0 ci        (1000) ci        (1000)     1327 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/types.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    10766 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/utils.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.360182 tutor-17.0.4/tutor.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6528 2024-04-11 09:44:08.000000 tutor-17.0.4/tutor.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     4103 2024-04-11 09:44:08.000000 tutor-17.0.4/tutor.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2024-04-11 09:44:08.000000 tutor-17.0.4/tutor.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       51 2024-04-11 09:44:08.000000 tutor-17.0.4/tutor.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)     1840 2024-04-11 09:44:08.000000 tutor-17.0.4/tutor.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        6 2024-04-11 09:44:08.000000 tutor-17.0.4/tutor.egg-info/top_level.txt
```

### Comparing `tutor-17.0.3/LICENSE.txt` & `tutor-17.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/PKG-INFO` & `tutor-17.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor
-Version: 17.0.3
+Version: 17.0.4
 Summary: The Docker-based Open edX distribution designed for peace of mind
 Home-page: https://docs.tutor.edly.io/
 Author: Edly
 Author-email: hello@edly.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.edly.io/
 Project-URL: Code, https://github.com/overhangio/tutor
```

### Comparing `tutor-17.0.3/README.rst` & `tutor-17.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/requirements/dev.txt` & `tutor-17.0.4/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/setup.py` & `tutor-17.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tests/test_bindmount.py` & `tutor-17.0.4/tests/test_bindmount.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tests/test_config.py` & `tutor-17.0.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tests/test_env.py` & `tutor-17.0.4/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tests/test_plugin_indexes.py` & `tutor-17.0.4/tests/test_plugin_indexes.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tests/test_plugins.py` & `tutor-17.0.4/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tests/test_plugins_v0.py` & `tutor-17.0.4/tests/test_plugins_v0.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tests/test_serialize.py` & `tutor-17.0.4/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tests/test_utils.py` & `tutor-17.0.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/__about__.py` & `tutor-17.0.4/tutor/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 # Increment this version number to trigger a new release. See
 # docs/tutor.html#versioning for information on the versioning scheme.
-__version__ = "17.0.3"
+__version__ = "17.0.4"
 
 # The version suffix will be appended to the actual version, separated by a
 # dash. Use this suffix to differentiate between the actual released version and
 # the versions from other branches. For instance: set the suffix to "nightly" in
 # the nightly branch.
 # The suffix is cleanly separated from the __version__ in this module to avoid
 # conflicts when merging branches.
```

### Comparing `tutor-17.0.3/tutor/bindmount.py` & `tutor-17.0.4/tutor/bindmount.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/cli.py` & `tutor-17.0.4/tutor/commands/cli.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/compose.py` & `tutor-17.0.4/tutor/commands/compose.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/config.py` & `tutor-17.0.4/tutor/commands/config.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/context.py` & `tutor-17.0.4/tutor/commands/context.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/dev.py` & `tutor-17.0.4/tutor/commands/dev.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/images.py` & `tutor-17.0.4/tutor/commands/images.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/jobs.py` & `tutor-17.0.4/tutor/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/k8s.py` & `tutor-17.0.4/tutor/commands/k8s.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/local.py` & `tutor-17.0.4/tutor/commands/local.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/mounts.py` & `tutor-17.0.4/tutor/commands/mounts.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/params.py` & `tutor-17.0.4/tutor/commands/params.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/plugins.py` & `tutor-17.0.4/tutor/commands/plugins.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/upgrade/common.py` & `tutor-17.0.4/tutor/commands/upgrade/common.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/upgrade/compose.py` & `tutor-17.0.4/tutor/commands/upgrade/compose.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/commands/upgrade/k8s.py` & `tutor-17.0.4/tutor/commands/upgrade/k8s.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/config.py` & `tutor-17.0.4/tutor/config.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/core/hooks/actions.py` & `tutor-17.0.4/tutor/core/hooks/actions.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/core/hooks/contexts.py` & `tutor-17.0.4/tutor/core/hooks/contexts.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/core/hooks/filters.py` & `tutor-17.0.4/tutor/core/hooks/filters.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/core/hooks/priorities.py` & `tutor-17.0.4/tutor/core/hooks/priorities.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/env.py` & `tutor-17.0.4/tutor/env.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/fmt.py` & `tutor-17.0.4/tutor/fmt.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/hooks/__init__.py` & `tutor-17.0.4/tutor/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/hooks/catalog.py` & `tutor-17.0.4/tutor/hooks/catalog.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/images.py` & `tutor-17.0.4/tutor/images.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/interactive.py` & `tutor-17.0.4/tutor/interactive.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/plugins/__init__.py` & `tutor-17.0.4/tutor/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/plugins/base.py` & `tutor-17.0.4/tutor/plugins/base.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/plugins/indexes.py` & `tutor-17.0.4/tutor/plugins/indexes.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/plugins/openedx.py` & `tutor-17.0.4/tutor/plugins/openedx.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/plugins/v0.py` & `tutor-17.0.4/tutor/plugins/v0.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/plugins/v1.py` & `tutor-17.0.4/tutor/plugins/v1.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/serialize.py` & `tutor-17.0.4/tutor/serialize.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/tasks.py` & `tutor-17.0.4/tutor/tasks.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/apps/caddy/Caddyfile` & `tutor-17.0.4/tutor/templates/apps/caddy/Caddyfile`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/apps/openedx/config/cms.env.yml` & `tutor-17.0.4/tutor/templates/apps/openedx/config/cms.env.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/apps/openedx/config/lms.env.yml` & `tutor-17.0.4/tutor/templates/apps/openedx/config/lms.env.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/apps/openedx/config/partials/auth.yml` & `tutor-17.0.4/tutor/templates/apps/openedx/config/partials/auth.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/apps/openedx/settings/cms/development.py` & `tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/development.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/apps/openedx/settings/cms/production.py` & `tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/production.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/apps/openedx/settings/lms/development.py` & `tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/development.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/apps/openedx/settings/lms/production.py` & `tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/production.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/apps/openedx/settings/partials/common_all.py` & `tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_all.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/apps/openedx/settings/partials/common_cms.py` & `tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_cms.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/apps/openedx/settings/partials/common_lms.py` & `tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_lms.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/apps/redis/redis.conf` & `tutor-17.0.4/tutor/templates/apps/redis/redis.conf`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/build/openedx/Dockerfile` & `tutor-17.0.4/tutor/templates/build/openedx/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/build/openedx/bin/openedx-assets` & `tutor-17.0.4/tutor/templates/build/openedx/bin/openedx-assets`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/build/openedx/bin/site-configuration` & `tutor-17.0.4/tutor/templates/build/openedx/bin/site-configuration`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/config/base.yml` & `tutor-17.0.4/tutor/templates/config/base.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/config/defaults.yml` & `tutor-17.0.4/tutor/templates/config/defaults.yml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 DOCKER_IMAGE_ELASTICSEARCH: "docker.io/elasticsearch:7.17.13"
 # https://hub.docker.com/_/mongo/tags
 DOCKER_IMAGE_MONGODB: "docker.io/mongo:4.4.25"
 # https://hub.docker.com/_/mysql/tags
 DOCKER_IMAGE_MYSQL: "docker.io/mysql:8.1.0"
 DOCKER_IMAGE_PERMISSIONS: "{{ DOCKER_REGISTRY }}overhangio/openedx-permissions:{{ TUTOR_VERSION }}"
 # https://hub.docker.com/_/redis/tags
-DOCKER_IMAGE_REDIS: "docker.io/redis:7.2.1"
+DOCKER_IMAGE_REDIS: "docker.io/redis:7.2.4"
 # https://hub.docker.com/r/devture/exim-relay/tags
 DOCKER_IMAGE_SMTP: "docker.io/devture/exim-relay:4.96-r1-0"
 EDX_PLATFORM_REPOSITORY: "https://github.com/openedx/edx-platform.git"
 EDX_PLATFORM_VERSION: "{{ OPENEDX_COMMON_VERSION }}"
 ELASTICSEARCH_HOST: "elasticsearch"
 ELASTICSEARCH_PORT: 9200
 ELASTICSEARCH_SCHEME: "http"
@@ -55,15 +55,15 @@
 OPENEDX_CACHE_REDIS_DB: 1
 OPENEDX_CELERY_REDIS_DB: 0
 OPENEDX_CMS_UWSGI_WORKERS: 2
 OPENEDX_LMS_UWSGI_WORKERS: 2
 OPENEDX_MYSQL_DATABASE: "openedx"
 OPENEDX_MYSQL_USERNAME: "openedx"
 # the common version will be automatically set to "master" in the nightly branch
-OPENEDX_COMMON_VERSION: "open-release/quince.2"
+OPENEDX_COMMON_VERSION: "open-release/quince.3"
 OPENEDX_EXTRA_PIP_REQUIREMENTS: []
 MYSQL_HOST: "mysql"
 MYSQL_PORT: 3306
 MYSQL_ROOT_USERNAME: "root"
 NPM_REGISTRY: "https://registry.npmjs.org/"
 PLATFORM_NAME: "My Open edX"
 PREVIEW_LMS_HOST: "preview.{{ LMS_HOST }}"
```

### Comparing `tutor-17.0.3/tutor/templates/dev/docker-compose.jobs.yml` & `tutor-17.0.4/tutor/templates/dev/docker-compose.jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/dev/docker-compose.yml` & `tutor-17.0.4/tutor/templates/dev/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/jobs/init/cms.sh` & `tutor-17.0.4/tutor/templates/jobs/init/cms.sh`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/jobs/init/lms.sh` & `tutor-17.0.4/tutor/templates/jobs/init/lms.sh`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/jobs/init/mounted-directories.sh` & `tutor-17.0.4/tutor/templates/jobs/init/mounted-directories.sh`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/jobs/init/mysql.sh` & `tutor-17.0.4/tutor/templates/jobs/init/mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/k8s/deployments.yml` & `tutor-17.0.4/tutor/templates/k8s/deployments.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/k8s/jobs.yml` & `tutor-17.0.4/tutor/templates/k8s/jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/k8s/services.yml` & `tutor-17.0.4/tutor/templates/k8s/services.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/k8s/volumes.yml` & `tutor-17.0.4/tutor/templates/k8s/volumes.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/kustomization.yml` & `tutor-17.0.4/tutor/templates/kustomization.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/local/docker-compose.jobs.yml` & `tutor-17.0.4/tutor/templates/local/docker-compose.jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/local/docker-compose.prod.yml` & `tutor-17.0.4/tutor/templates/local/docker-compose.prod.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/templates/local/docker-compose.yml` & `tutor-17.0.4/tutor/templates/local/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/types.py` & `tutor-17.0.4/tutor/types.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor/utils.py` & `tutor-17.0.4/tutor/utils.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor.egg-info/PKG-INFO` & `tutor-17.0.4/tutor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor
-Version: 17.0.3
+Version: 17.0.4
 Summary: The Docker-based Open edX distribution designed for peace of mind
 Home-page: https://docs.tutor.edly.io/
 Author: Edly
 Author-email: hello@edly.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.edly.io/
 Project-URL: Code, https://github.com/overhangio/tutor
```

### Comparing `tutor-17.0.3/tutor.egg-info/SOURCES.txt` & `tutor-17.0.4/tutor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-17.0.3/tutor.egg-info/requires.txt` & `tutor-17.0.4/tutor.egg-info/requires.txt`

 * *Files identical despite different names*

