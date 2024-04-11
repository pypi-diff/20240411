# Comparing `tmp/alerta-8.5.2.tar.gz` & `tmp/alerta-8.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alerta-8.5.2.tar", last modified: Sat Mar 18 13:37:44 2023, max compression
+gzip compressed data, was "alerta-8.5.3.tar", last modified: Thu Apr 11 21:37:23 2024, max compression
```

## Comparing `alerta-8.5.2.tar` & `alerta-8.5.3.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:44.206773 alerta-8.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-18 13:37:35.000000 alerta-8.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-18 13:37:35.000000 alerta-8.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-18 13:37:35.000000 alerta-8.5.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-03-18 13:37:44.206773 alerta-8.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-03-18 13:37:35.000000 alerta-8.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-18 13:37:35.000000 alerta-8.5.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:44.190772 alerta-8.5.2/alerta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-03-18 13:37:44.000000 alerta-8.5.2/alerta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-03-18 13:37:44.000000 alerta-8.5.2/alerta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 13:37:44.000000 alerta-8.5.2/alerta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-18 13:37:44.000000 alerta-8.5.2/alerta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 13:37:44.000000 alerta-8.5.2/alerta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-18 13:37:44.000000 alerta-8.5.2/alerta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-18 13:37:44.000000 alerta-8.5.2/alerta.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:44.194773 alerta-8.5.2/alertaclient/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:44.194773 alerta-8.5.2/alertaclient/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/auth/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/auth/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/auth/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/auth/google.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/auth/hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/auth/oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/auth/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/auth/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:44.198773 alerta-8.5.2/alertaclient/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_ack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_blackout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_blackouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_close.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_customers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_heartbeats.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_housekeeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_logout.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_me.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_perm.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_revoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_shelve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_signup.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_top.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_unack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_unshelve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_untag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_uptime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_watch.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/commands/cmd_whoami.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:44.202773 alerta-8.5.2/alertaclient/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/models/blackout.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/models/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/models/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/models/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/models/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/models/note.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/top.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-18 13:37:35.000000 alerta-8.5.2/alertaclient/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-18 13:37:44.206773 alerta-8.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-18 13:37:35.000000 alerta-8.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:44.190772 alerta-8.5.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:44.202773 alerta-8.5.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/integration/test_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/integration/test_blackouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/integration/test_customers.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/integration/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/integration/test_heartbeats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/integration/test_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/integration/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/integration/test_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/integration/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/integration/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:44.206773 alerta-8.5.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_blackouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_customers.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_heartbeats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_remoteconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-18 13:37:35.000000 alerta-8.5.2/tests/unit/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:23.847455 alerta-8.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 21:37:20.000000 alerta-8.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 21:37:20.000000 alerta-8.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-11 21:37:20.000000 alerta-8.5.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-11 21:37:23.847455 alerta-8.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-11 21:37:20.000000 alerta-8.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 21:37:20.000000 alerta-8.5.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:23.847455 alerta-8.5.3/alerta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-11 21:37:23.000000 alerta-8.5.3/alerta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-11 21:37:23.000000 alerta-8.5.3/alerta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:37:23.000000 alerta-8.5.3/alerta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 21:37:23.000000 alerta-8.5.3/alerta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:37:23.000000 alerta-8.5.3/alerta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 21:37:23.000000 alerta-8.5.3/alerta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 21:37:23.000000 alerta-8.5.3/alerta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:23.831454 alerta-8.5.3/alertaclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20683 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:23.835455 alerta-8.5.3/alertaclient/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/auth/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/auth/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/auth/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/auth/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/auth/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/auth/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/auth/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/auth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:23.843454 alerta-8.5.3/alertaclient/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_ack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_blackout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_blackouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_heartbeats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_housekeeping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_me.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_perm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_perms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_revoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_shelve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_signup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_unack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_unshelve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_untag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_uptime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/commands/cmd_whoami.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:23.843454 alerta-8.5.3/alertaclient/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/models/blackout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/models/customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/models/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/models/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/models/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 21:37:20.000000 alerta-8.5.3/alertaclient/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-11 21:37:23.851455 alerta-8.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-11 21:37:20.000000 alerta-8.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:23.827454 alerta-8.5.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:23.847455 alerta-8.5.3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/integration/test_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/integration/test_blackouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/integration/test_customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/integration/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/integration/test_heartbeats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/integration/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/integration/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/integration/test_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/integration/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/integration/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:23.847455 alerta-8.5.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_blackouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_heartbeats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_remoteconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-11 21:37:20.000000 alerta-8.5.3/tests/unit/test_users.py
```

### Comparing `alerta-8.5.2/LICENSE` & `alerta-8.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/NOTICE` & `alerta-8.5.3/NOTICE`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/PKG-INFO` & `alerta-8.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alerta
-Version: 8.5.2
+Version: 8.5.3
 Summary: Alerta unified command-line tool and SDK
 Home-page: https://github.com/guardian/python-alerta
 Author: Nick Satterly
 Author-email: nfsatterly@gmail.com
 License: Apache License 2.0
 Keywords: alerta client unified command line tool sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: Click
+Requires-Dist: requests
+Requires-Dist: requests_hawk
+Requires-Dist: tabulate
+Requires-Dist: pytz
 
 Alerta Command-Line Tool
 ========================
 
 [![Actions Status](https://github.com/alerta/python-alerta-client/workflows/CI%20Tests/badge.svg)](https://github.com/alerta/python-alerta-client/actions)
  [![Slack chat](https://img.shields.io/badge/chat-on%20slack-blue?logo=slack)](https://slack.alerta.dev) [![Coverage Status](https://coveralls.io/repos/github/alerta/python-alerta-client/badge.svg?branch=master)](https://coveralls.io/github/alerta/python-alerta-client?branch=master)
 
@@ -169,15 +174,15 @@
     >>> client.heartbeat().serialize()['status']
     'ok'
 
 License
 -------
 
     Alerta monitoring system and console
-    Copyright 2012-2023 Nick Satterly
+    Copyright 2012-2024 Nick Satterly
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `alerta-8.5.2/README.md` & `alerta-8.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
     >>> client.heartbeat().serialize()['status']
     'ok'
 
 License
 -------
 
     Alerta monitoring system and console
-    Copyright 2012-2023 Nick Satterly
+    Copyright 2012-2024 Nick Satterly
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `alerta-8.5.2/alerta.egg-info/PKG-INFO` & `alerta-8.5.3/alerta.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alerta
-Version: 8.5.2
+Version: 8.5.3
 Summary: Alerta unified command-line tool and SDK
 Home-page: https://github.com/guardian/python-alerta
 Author: Nick Satterly
 Author-email: nfsatterly@gmail.com
 License: Apache License 2.0
 Keywords: alerta client unified command line tool sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: Click
+Requires-Dist: requests
+Requires-Dist: requests_hawk
+Requires-Dist: tabulate
+Requires-Dist: pytz
 
 Alerta Command-Line Tool
 ========================
 
 [![Actions Status](https://github.com/alerta/python-alerta-client/workflows/CI%20Tests/badge.svg)](https://github.com/alerta/python-alerta-client/actions)
  [![Slack chat](https://img.shields.io/badge/chat-on%20slack-blue?logo=slack)](https://slack.alerta.dev) [![Coverage Status](https://coveralls.io/repos/github/alerta/python-alerta-client/badge.svg?branch=master)](https://coveralls.io/github/alerta/python-alerta-client?branch=master)
 
@@ -169,15 +174,15 @@
     >>> client.heartbeat().serialize()['status']
     'ok'
 
 License
 -------
 
     Alerta monitoring system and console
-    Copyright 2012-2023 Nick Satterly
+    Copyright 2012-2024 Nick Satterly
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `alerta-8.5.2/alerta.egg-info/SOURCES.txt` & `alerta-8.5.3/alerta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/__init__.py` & `alerta-8.5.3/alertaclient/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/api.py` & `alerta-8.5.3/alertaclient/api.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/auth/azure.py` & `alerta-8.5.3/alertaclient/auth/azure.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/auth/github.py` & `alerta-8.5.3/alertaclient/auth/github.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/auth/gitlab.py` & `alerta-8.5.3/alertaclient/auth/gitlab.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/auth/google.py` & `alerta-8.5.3/alertaclient/auth/google.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/auth/oidc.py` & `alerta-8.5.3/alertaclient/auth/oidc.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/auth/token.py` & `alerta-8.5.3/alertaclient/auth/token.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/auth/utils.py` & `alerta-8.5.3/alertaclient/auth/utils.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/cli.py` & `alerta-8.5.3/alertaclient/cli.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_ack.py` & `alerta-8.5.3/alertaclient/commands/cmd_ack.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_action.py` & `alerta-8.5.3/alertaclient/commands/cmd_action.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_alerts.py` & `alerta-8.5.3/alertaclient/commands/cmd_alerts.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_blackout.py` & `alerta-8.5.3/alertaclient/commands/cmd_blackout.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_blackouts.py` & `alerta-8.5.3/alertaclient/commands/cmd_blackouts.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_close.py` & `alerta-8.5.3/alertaclient/commands/cmd_close.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_customer.py` & `alerta-8.5.3/alertaclient/commands/cmd_customer.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_customers.py` & `alerta-8.5.3/alertaclient/commands/cmd_customers.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_delete.py` & `alerta-8.5.3/alertaclient/commands/cmd_delete.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_group.py` & `alerta-8.5.3/alertaclient/commands/cmd_group.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_groups.py` & `alerta-8.5.3/alertaclient/commands/cmd_groups.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_heartbeat.py` & `alerta-8.5.3/alertaclient/commands/cmd_heartbeat.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_heartbeats.py` & `alerta-8.5.3/alertaclient/commands/cmd_heartbeats.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_history.py` & `alerta-8.5.3/alertaclient/commands/cmd_history.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_housekeeping.py` & `alerta-8.5.3/alertaclient/commands/cmd_housekeeping.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_key.py` & `alerta-8.5.3/alertaclient/commands/cmd_key.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_keys.py` & `alerta-8.5.3/alertaclient/commands/cmd_keys.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_login.py` & `alerta-8.5.3/alertaclient/commands/cmd_login.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_me.py` & `alerta-8.5.3/alertaclient/commands/cmd_me.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_note.py` & `alerta-8.5.3/alertaclient/commands/cmd_note.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_notes.py` & `alerta-8.5.3/alertaclient/commands/cmd_notes.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_perm.py` & `alerta-8.5.3/alertaclient/commands/cmd_perm.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_perms.py` & `alerta-8.5.3/alertaclient/commands/cmd_perms.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_query.py` & `alerta-8.5.3/alertaclient/commands/cmd_query.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_raw.py` & `alerta-8.5.3/alertaclient/commands/cmd_raw.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_scopes.py` & `alerta-8.5.3/alertaclient/commands/cmd_scopes.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_send.py` & `alerta-8.5.3/alertaclient/commands/cmd_send.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_shelve.py` & `alerta-8.5.3/alertaclient/commands/cmd_shelve.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_signup.py` & `alerta-8.5.3/alertaclient/commands/cmd_signup.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_status.py` & `alerta-8.5.3/alertaclient/commands/cmd_status.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_tag.py` & `alerta-8.5.3/alertaclient/commands/cmd_tag.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_token.py` & `alerta-8.5.3/alertaclient/commands/cmd_token.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_unack.py` & `alerta-8.5.3/alertaclient/commands/cmd_unack.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_unshelve.py` & `alerta-8.5.3/alertaclient/commands/cmd_unshelve.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_untag.py` & `alerta-8.5.3/alertaclient/commands/cmd_untag.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_update.py` & `alerta-8.5.3/alertaclient/commands/cmd_update.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_uptime.py` & `alerta-8.5.3/alertaclient/commands/cmd_uptime.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_user.py` & `alerta-8.5.3/alertaclient/commands/cmd_user.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_users.py` & `alerta-8.5.3/alertaclient/commands/cmd_users.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_version.py` & `alerta-8.5.3/alertaclient/commands/cmd_version.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_watch.py` & `alerta-8.5.3/alertaclient/commands/cmd_watch.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/commands/cmd_whoami.py` & `alerta-8.5.3/alertaclient/commands/cmd_whoami.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/config.py` & `alerta-8.5.3/alertaclient/config.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/models/alert.py` & `alerta-8.5.3/alertaclient/models/alert.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/models/blackout.py` & `alerta-8.5.3/alertaclient/models/blackout.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/models/customer.py` & `alerta-8.5.3/alertaclient/models/customer.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/models/enums.py` & `alerta-8.5.3/alertaclient/models/enums.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/models/group.py` & `alerta-8.5.3/alertaclient/models/group.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/models/heartbeat.py` & `alerta-8.5.3/alertaclient/models/heartbeat.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/models/history.py` & `alerta-8.5.3/alertaclient/models/history.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/models/key.py` & `alerta-8.5.3/alertaclient/models/key.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/models/note.py` & `alerta-8.5.3/alertaclient/models/note.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/models/permission.py` & `alerta-8.5.3/alertaclient/models/permission.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/models/user.py` & `alerta-8.5.3/alertaclient/models/user.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/top.py` & `alerta-8.5.3/alertaclient/top.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/alertaclient/utils.py` & `alerta-8.5.3/alertaclient/utils.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/setup.py` & `alerta-8.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/integration/test_alerts.py` & `alerta-8.5.3/tests/integration/test_alerts.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/integration/test_blackouts.py` & `alerta-8.5.3/tests/integration/test_blackouts.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/integration/test_customers.py` & `alerta-8.5.3/tests/integration/test_customers.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/integration/test_groups.py` & `alerta-8.5.3/tests/integration/test_groups.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/integration/test_history.py` & `alerta-8.5.3/tests/integration/test_history.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/integration/test_keys.py` & `alerta-8.5.3/tests/integration/test_keys.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_alerts.py` & `alerta-8.5.3/tests/unit/test_alerts.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_blackouts.py` & `alerta-8.5.3/tests/unit/test_blackouts.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_commands.py` & `alerta-8.5.3/tests/unit/test_commands.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_config.py` & `alerta-8.5.3/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_customers.py` & `alerta-8.5.3/tests/unit/test_customers.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_groups.py` & `alerta-8.5.3/tests/unit/test_groups.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_heartbeats.py` & `alerta-8.5.3/tests/unit/test_heartbeats.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_history.py` & `alerta-8.5.3/tests/unit/test_history.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_http_client.py` & `alerta-8.5.3/tests/unit/test_http_client.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_keys.py` & `alerta-8.5.3/tests/unit/test_keys.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_notes.py` & `alerta-8.5.3/tests/unit/test_notes.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_permissions.py` & `alerta-8.5.3/tests/unit/test_permissions.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_remoteconfig.py` & `alerta-8.5.3/tests/unit/test_remoteconfig.py`

 * *Files identical despite different names*

### Comparing `alerta-8.5.2/tests/unit/test_users.py` & `alerta-8.5.3/tests/unit/test_users.py`

 * *Files identical despite different names*

