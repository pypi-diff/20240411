# Comparing `tmp/WebScripts-3.0.8.tar.gz` & `tmp/WebScripts-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebScripts-3.0.8.tar", last modified: Sun Feb 19 13:10:05 2023, max compression
+gzip compressed data, was "WebScripts-3.0.9.tar", last modified: Sun Feb 19 15:56:09 2023, max compression
```

## Comparing `WebScripts-3.0.8.tar` & `WebScripts-3.0.9.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.832130 WebScripts-3.0.8/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.804116 WebScripts-3.0.8/.github/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.804116 WebScripts-3.0.8/.github/workflows/
--rw-r--r--   0 kali      (1000) kali      (1000)      877 2023-02-02 22:30:36.000000 WebScripts-3.0.8/.github/workflows/WebScripts38_test.yml
--rw-r--r--   0 kali      (1000) kali      (1000)     1658 2023-02-04 00:15:58.000000 WebScripts-3.0.8/.github/workflows/ZAP.yml
--rw-r--r--   0 kali      (1000) kali      (1000)     1673 2023-02-04 00:15:58.000000 WebScripts-3.0.8/.github/workflows/ZAP2.yml
--rw-r--r--   0 kali      (1000) kali      (1000)      569 2023-02-04 00:15:58.000000 WebScripts-3.0.8/.github/workflows/bandit.yml
--rw-r--r--   0 kali      (1000) kali      (1000)     1042 2023-02-02 22:30:36.000000 WebScripts-3.0.8/.github/workflows/ci.yml
--rw-r--r--   0 kali      (1000) kali      (1000)     2529 2023-02-04 00:15:58.000000 WebScripts-3.0.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 kali      (1000) kali      (1000)     4076 2023-02-04 00:15:58.000000 WebScripts-3.0.8/.github/workflows/kali_tools_scans.yml
--rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-02-04 00:15:58.000000 WebScripts-3.0.8/.github/workflows/nuclei.yml
--rw-r--r--   0 kali      (1000) kali      (1000)      279 2023-02-04 00:15:58.000000 WebScripts-3.0.8/.github/workflows/pycharm.yml
--rw-r--r--   0 kali      (1000) kali      (1000)      317 2023-02-04 00:15:58.000000 WebScripts-3.0.8/.github/workflows/safety_check.yml
--rw-r--r--   0 kali      (1000) kali      (1000)      379 2023-02-04 00:15:58.000000 WebScripts-3.0.8/.github/workflows/semgrep.yml
--rw-r--r--   0 kali      (1000) kali      (1000)     1699 2023-02-04 00:15:46.000000 WebScripts-3.0.8/.github/workflows/unittest.yml
--rw-r--r--   0 kali      (1000) kali      (1000)     1808 2023-02-04 00:15:46.000000 WebScripts-3.0.8/.github/workflows/unittest38.yml
--rw-r--r--   0 kali      (1000) kali      (1000)     2508 2023-02-04 00:16:06.000000 WebScripts-3.0.8/.gitlab-ci.yml
--rw-r--r--   0 kali      (1000) kali      (1000)      135 2023-02-04 00:16:06.000000 WebScripts-3.0.8/.readthedocs.yaml
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-02-04 00:16:06.000000 WebScripts-3.0.8/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      641 2023-02-04 00:18:14.000000 WebScripts-3.0.8/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)    20888 2023-02-19 13:10:05.832130 WebScripts-3.0.8/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)    19254 2023-02-16 15:30:44.000000 WebScripts-3.0.8/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.804116 WebScripts-3.0.8/Scripts/
--rw-r--r--   0 kali      (1000) kali      (1000)      939 2023-02-04 00:16:00.000000 WebScripts-3.0.8/Scripts/activate_this.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2810 2023-02-04 00:16:00.000000 WebScripts-3.0.8/Scripts/wsgi.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.808118 WebScripts-3.0.8/WebScripts/
--rw-r--r--   0 kali      (1000) kali      (1000)     2944 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/Errors.py
--rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    31835 2023-02-04 00:27:08.000000 WebScripts-3.0.8/WebScripts/Pages.py
--rw-r--r--   0 kali      (1000) kali      (1000)    69254 2023-02-04 00:27:12.000000 WebScripts-3.0.8/WebScripts/WebScripts.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1845 2023-02-19 19:00:30.000000 WebScripts-3.0.8/WebScripts/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1758 2023-02-19 19:00:36.000000 WebScripts-3.0.8/WebScripts/__main__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.808118 WebScripts-3.0.8/WebScripts/cgi-bin/
--rw-r--r--   0 kali      (1000) kali      (1000)     3549 2023-02-02 22:30:42.000000 WebScripts-3.0.8/WebScripts/cgi-bin/hello.py
--rw-r--r--   0 kali      (1000) kali      (1000)      117 2023-02-02 22:30:42.000000 WebScripts-3.0.8/WebScripts/cgi-bin/test.py
--rw-r--r--   0 kali      (1000) kali      (1000)    37675 2023-02-04 00:26:58.000000 WebScripts-3.0.8/WebScripts/commons.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.808118 WebScripts-3.0.8/WebScripts/config/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.808118 WebScripts-3.0.8/WebScripts/config/files/
--rw-r--r--   0 kali      (1000) kali      (1000)      951 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/config/files/change_my_password.json
--rw-r--r--   0 kali      (1000) kali      (1000)     1857 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/config/files/test_config.json
--rw-r--r--   0 kali      (1000) kali      (1000)     4052 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/config/loggers.ini
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.808118 WebScripts-3.0.8/WebScripts/config/nt/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.808118 WebScripts-3.0.8/WebScripts/config/nt/files/
--rw-r--r--   0 kali      (1000) kali      (1000)      698 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/config/nt/files/change_my_password.ini
--rw-r--r--   0 kali      (1000) kali      (1000)      893 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/config/nt/files/change_my_password.json
--rw-r--r--   0 kali      (1000) kali      (1000)     1823 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/config/nt/files/test_config.json
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.808118 WebScripts-3.0.8/WebScripts/config/nt/scripts/
--rw-r--r--   0 kali      (1000) kali      (1000)     7259 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/config/nt/scripts/default_admin_scripts.json
--rw-r--r--   0 kali      (1000) kali      (1000)     2349 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/config/nt/scripts/default_log_scripts.json
--rw-r--r--   0 kali      (1000) kali      (1000)     2172 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/config/nt/scripts/default_password_scripts.json
--rw-r--r--   0 kali      (1000) kali      (1000)     1499 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/config/nt/scripts/default_requests_scripts.json
--rw-r--r--   0 kali      (1000) kali      (1000)     1510 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/config/nt/scripts/default_rss_scripts.json
--rw-r--r--   0 kali      (1000) kali      (1000)     7248 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/config/nt/scripts/default_uploads_scripts.json
--rw-r--r--   0 kali      (1000) kali      (1000)    17377 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/config/nt/server.ini
--rw-r--r--   0 kali      (1000) kali      (1000)     3660 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/config/nt/server.json
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.808118 WebScripts-3.0.8/WebScripts/config/scripts/
--rw-r--r--   0 kali      (1000) kali      (1000)     7889 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/config/scripts/default_admin_scripts.json
--rw-r--r--   0 kali      (1000) kali      (1000)     2345 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/config/scripts/default_log_scripts.json
--rw-r--r--   0 kali      (1000) kali      (1000)     2189 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/config/scripts/default_password_scripts.json
--rw-r--r--   0 kali      (1000) kali      (1000)     1551 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/config/scripts/default_requests_scripts.json
--rw-r--r--   0 kali      (1000) kali      (1000)     1562 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/config/scripts/default_rss_scripts.json
--rw-r--r--   0 kali      (1000) kali      (1000)     8034 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/config/scripts/default_uploads_scripts.json
--rw-r--r--   0 kali      (1000) kali      (1000)    17373 2023-02-04 00:16:00.000000 WebScripts-3.0.8/WebScripts/config/server.ini
--rw-r--r--   0 kali      (1000) kali      (1000)     3634 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/config/server.json
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.812120 WebScripts-3.0.8/WebScripts/data/
--rw-r--r--   0 kali      (1000) kali      (1000)      131 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/data/groups.csv
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/data/id
--rw-r--r--   0 kali      (1000) kali      (1000)       11 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/data/passwords.csv
--rw-r--r--   0 kali      (1000) kali      (1000)       63 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/data/requests.csv
--rw-r--r--   0 kali      (1000) kali      (1000)       64 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/data/rss.csv
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.812120 WebScripts-3.0.8/WebScripts/data/uploads/
--rw-r--r--   0 kali      (1000) kali      (1000)    35823 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/data/uploads/LICENSE_210725_181116.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       73 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/data/uploads.csv
--rw-r--r--   0 kali      (1000) kali      (1000)      527 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/data/users.csv
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.812120 WebScripts-3.0.8/WebScripts/doc/
--rw-r--r--   0 kali      (1000) kali      (1000)        4 2023-02-04 00:16:02.000000 WebScripts-3.0.8/WebScripts/doc/empty.html
--rw-r--r--   0 kali      (1000) kali      (1000)    17474 2023-02-15 12:49:06.000000 WebScripts-3.0.8/WebScripts/harden.py
--rw-r--r--   0 kali      (1000) kali      (1000)    73284 2023-02-19 18:53:30.000000 WebScripts-3.0.8/WebScripts/hardening.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.812120 WebScripts-3.0.8/WebScripts/modules/
--rw-r--r--   0 kali      (1000) kali      (1000)    11468 2023-02-04 00:27:28.000000 WebScripts-3.0.8/WebScripts/modules/Configurations.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6139 2023-02-04 00:27:34.000000 WebScripts-3.0.8/WebScripts/modules/JsonRpc.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4841 2023-02-04 00:27:26.000000 WebScripts-3.0.8/WebScripts/modules/cgi.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2983 2023-02-04 00:27:30.000000 WebScripts-3.0.8/WebScripts/modules/csp.py
--rw-r--r--   0 kali      (1000) kali      (1000)    13294 2023-02-04 00:27:32.000000 WebScripts-3.0.8/WebScripts/modules/error_pages.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4814 2023-02-04 00:27:36.000000 WebScripts-3.0.8/WebScripts/modules/notification.py
--rw-r--r--   0 kali      (1000) kali      (1000)     8254 2023-02-04 00:27:38.000000 WebScripts-3.0.8/WebScripts/modules/rss.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7142 2023-02-04 00:27:40.000000 WebScripts-3.0.8/WebScripts/modules/share.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.804116 WebScripts-3.0.8/WebScripts/scripts/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.816122 WebScripts-3.0.8/WebScripts/scripts/account/
--rw-r--r--   0 kali      (1000) kali      (1000)     2402 2023-02-04 00:16:02.000000 WebScripts-3.0.8/WebScripts/scripts/account/add_group.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4399 2023-02-04 00:28:14.000000 WebScripts-3.0.8/WebScripts/scripts/account/add_user.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3191 2023-02-04 00:28:14.000000 WebScripts-3.0.8/WebScripts/scripts/account/api_view_groups.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3173 2023-02-04 00:28:16.000000 WebScripts-3.0.8/WebScripts/scripts/account/api_view_users.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3458 2023-02-04 00:28:18.000000 WebScripts-3.0.8/WebScripts/scripts/account/auth.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3264 2023-02-04 00:28:18.000000 WebScripts-3.0.8/WebScripts/scripts/account/change_my_password.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2708 2023-02-04 00:28:20.000000 WebScripts-3.0.8/WebScripts/scripts/account/change_user_password.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2417 2023-02-04 00:16:02.000000 WebScripts-3.0.8/WebScripts/scripts/account/delete_group.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2386 2023-02-04 00:16:02.000000 WebScripts-3.0.8/WebScripts/scripts/account/delete_user.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2337 2023-02-04 00:28:24.000000 WebScripts-3.0.8/WebScripts/scripts/account/get_apikey.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.816122 WebScripts-3.0.8/WebScripts/scripts/account/modules/
--rw-r--r--   0 kali      (1000) kali      (1000)    14352 2023-02-04 00:27:24.000000 WebScripts-3.0.8/WebScripts/scripts/account/modules/manage_defaults_databases.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2439 2023-02-04 00:28:26.000000 WebScripts-3.0.8/WebScripts/scripts/account/my_user_informations.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3193 2023-02-04 00:28:28.000000 WebScripts-3.0.8/WebScripts/scripts/account/view_groups.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3379 2023-02-04 00:28:28.000000 WebScripts-3.0.8/WebScripts/scripts/account/view_users.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.816122 WebScripts-3.0.8/WebScripts/scripts/doc/
--rw-r--r--   0 kali      (1000) kali      (1000)     3137 2023-02-04 00:28:34.000000 WebScripts-3.0.8/WebScripts/scripts/doc/py_doc.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.816122 WebScripts-3.0.8/WebScripts/scripts/logs/
--rw-r--r--   0 kali      (1000) kali      (1000)     3955 2023-02-04 00:28:36.000000 WebScripts-3.0.8/WebScripts/scripts/logs/log_analysis.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3298 2023-02-04 00:28:36.000000 WebScripts-3.0.8/WebScripts/scripts/logs/log_viewer.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.816122 WebScripts-3.0.8/WebScripts/scripts/passwords/
--rw-r--r--   0 kali      (1000) kali      (1000)     5607 2023-02-04 00:28:38.000000 WebScripts-3.0.8/WebScripts/scripts/passwords/get_password_share.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6016 2023-02-04 00:28:40.000000 WebScripts-3.0.8/WebScripts/scripts/passwords/new_password_share.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1988 2023-02-04 00:16:02.000000 WebScripts-3.0.8/WebScripts/scripts/passwords/password_generator.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.816122 WebScripts-3.0.8/WebScripts/scripts/py/
--rw-r--r--   0 kali      (1000) kali      (1000)     2816 2023-02-04 00:16:02.000000 WebScripts-3.0.8/WebScripts/scripts/py/ASCII_arts.py
--rw-r--r--   0 kali      (1000) kali      (1000)      893 2023-02-04 00:16:02.000000 WebScripts-3.0.8/WebScripts/scripts/py/hello.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3495 2023-02-04 00:28:46.000000 WebScripts-3.0.8/WebScripts/scripts/py/show_license.py
--rw-r--r--   0 kali      (1000) kali      (1000)      724 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/scripts/py/test_config.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.816122 WebScripts-3.0.8/WebScripts/scripts/request/
--rw-r--r--   0 kali      (1000) kali      (1000)     2669 2023-02-04 00:28:30.000000 WebScripts-3.0.8/WebScripts/scripts/request/delete_request.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2590 2023-02-04 00:28:32.000000 WebScripts-3.0.8/WebScripts/scripts/request/get_request.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3092 2023-02-04 00:28:32.000000 WebScripts-3.0.8/WebScripts/scripts/request/get_requests.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.816122 WebScripts-3.0.8/WebScripts/scripts/request/modules/
--rw-r--r--   0 kali      (1000) kali      (1000)     3979 2023-02-04 00:27:26.000000 WebScripts-3.0.8/WebScripts/scripts/request/modules/requests_management.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.816122 WebScripts-3.0.8/WebScripts/scripts/rss/
--rw-r--r--   0 kali      (1000) kali      (1000)     4311 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/scripts/rss/add_news.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.816122 WebScripts-3.0.8/WebScripts/scripts/to_3.8/
--rw-r--r--   0 kali      (1000) kali      (1000)     6639 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/scripts/to_3.8/to_3.8.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.820124 WebScripts-3.0.8/WebScripts/scripts/uploads/
--rw-r--r--   0 kali      (1000) kali      (1000)     3358 2023-02-04 00:27:56.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/HTML_all_files.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3334 2023-02-04 00:27:58.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/HTML_file_history.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3169 2023-02-04 00:28:00.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/HTML_uploads_properties.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2722 2023-02-04 00:28:00.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/HTML_uploads_size.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3241 2023-02-04 00:28:02.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/HTML_visible_files.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2435 2023-02-04 00:28:04.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/JSON_all_files.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2459 2023-02-04 00:28:04.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/JSON_file_history.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2560 2023-02-04 00:28:06.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/JSON_uploads_properties.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2619 2023-02-04 00:28:08.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/JSON_uploads_size.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2520 2023-02-04 00:28:10.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/JSON_visible_files.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2358 2023-02-04 00:27:42.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/api_get_all_files.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2418 2023-02-04 00:27:42.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/api_get_files.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2409 2023-02-04 00:27:44.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/api_get_history.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2335 2023-02-04 00:27:46.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/delete_file.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3318 2023-02-04 00:27:46.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/download_all_files.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3223 2023-02-04 00:27:48.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/download_filename.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3080 2023-02-04 00:27:50.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/get_all_files.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3302 2023-02-04 00:27:50.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/get_any_file.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3169 2023-02-04 00:27:52.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/get_file.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2926 2023-02-04 00:27:54.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/get_files.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3234 2023-02-04 00:27:54.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/get_history.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.820124 WebScripts-3.0.8/WebScripts/scripts/uploads/modules/
--rw-r--r--   0 kali      (1000) kali      (1000)    14751 2023-02-04 00:27:20.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/modules/uploads_management.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3991 2023-02-04 00:28:10.000000 WebScripts-3.0.8/WebScripts/scripts/uploads/upload_file.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.804116 WebScripts-3.0.8/WebScripts/static/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.820124 WebScripts-3.0.8/WebScripts/static/css/
--rw-r--r--   0 kali      (1000) kali      (1000)     1081 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/css/webscripts_index_style.css
--rw-r--r--   0 kali      (1000) kali      (1000)     4396 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/css/webscripts_script_style.css
--rw-r--r--   0 kali      (1000) kali      (1000)     9367 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/css/webscripts_style.css
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.820124 WebScripts-3.0.8/WebScripts/static/html/
--rw-r--r--   0 kali      (1000) kali      (1000)     7315 2023-02-19 19:03:58.000000 WebScripts-3.0.8/WebScripts/static/html/Configurations.html
--rw-r--r--   0 kali      (1000) kali      (1000)    32878 2023-02-19 19:03:58.000000 WebScripts-3.0.8/WebScripts/static/html/Errors.html
--rw-r--r--   0 kali      (1000) kali      (1000)     6040 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/static/html/JsonRpc.html
--rw-r--r--   0 kali      (1000) kali      (1000)     7973 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/static/html/Pages.html
--rw-r--r--   0 kali      (1000) kali      (1000)    25005 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/static/html/WebScripts.html
--rw-r--r--   0 kali      (1000) kali      (1000)    18945 2023-02-04 00:15:52.000000 WebScripts-3.0.8/WebScripts/static/html/__init__.html
--rw-r--r--   0 kali      (1000) kali      (1000)    23520 2023-02-19 19:03:58.000000 WebScripts-3.0.8/WebScripts/static/html/cgi.html
--rw-r--r--   0 kali      (1000) kali      (1000)    45403 2023-02-19 19:03:58.000000 WebScripts-3.0.8/WebScripts/static/html/commons.html
--rw-r--r--   0 kali      (1000) kali      (1000)     4294 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/html/csp.html
--rw-r--r--   0 kali      (1000) kali      (1000)     8559 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/html/error_pages.html
--rw-r--r--   0 kali      (1000) kali      (1000)     3203 2023-02-04 00:15:52.000000 WebScripts-3.0.8/WebScripts/static/html/get_request.html
--rw-r--r--   0 kali      (1000) kali      (1000)    22071 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/static/html/hardening.html
--rw-r--r--   0 kali      (1000) kali      (1000)    23909 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/static/html/index.html
--rw-r--r--   0 kali      (1000) kali      (1000)    27613 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/static/html/manage_defaults_databases.html
--rw-r--r--   0 kali      (1000) kali      (1000)     3344 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/html/notification.html
--rw-r--r--   0 kali      (1000) kali      (1000)    12153 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/static/html/requests_management.html
--rw-r--r--   0 kali      (1000) kali      (1000)    13953 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/static/html/rss.html
--rw-r--r--   0 kali      (1000) kali      (1000)     7503 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/html/share.html
--rw-r--r--   0 kali      (1000) kali      (1000)    18391 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/static/html/uploads_management.html
--rw-r--r--   0 kali      (1000) kali      (1000)    35209 2023-02-19 19:04:00.000000 WebScripts-3.0.8/WebScripts/static/html/utils.html
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.828128 WebScripts-3.0.8/WebScripts/static/images/
--rw-r--r--   0 kali      (1000) kali      (1000)    90843 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/images/WebScripts1.png
--rw-r--r--   0 kali      (1000) kali      (1000)    99659 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/images/WebScripts2.png
--rw-r--r--   0 kali      (1000) kali      (1000)    97909 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/images/WebScripts3.png
--rw-r--r--   0 kali      (1000) kali      (1000)    88696 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/images/WebScripts4.png
--rw-r--r--   0 kali      (1000) kali      (1000)    95444 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/images/WebScripts5.png
--rw-r--r--   0 kali      (1000) kali      (1000)    95082 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/images/WebScripts6.png
--rw-r--r--   0 kali      (1000) kali      (1000)    32125 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/images/WebScripts7.png
--rw-r--r--   0 kali      (1000) kali      (1000)    44039 2023-02-04 00:15:52.000000 WebScripts-3.0.8/WebScripts/static/images/webscripts_header.jpg
--rw-r--r--   0 kali      (1000) kali      (1000)    95444 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/images/webscripts_header.png
--rw-r--r--   0 kali      (1000) kali      (1000)    44039 2023-02-04 00:15:52.000000 WebScripts-3.0.8/WebScripts/static/images/webscripts_icon.jpg
--rw-r--r--   0 kali      (1000) kali      (1000)    95082 2023-02-04 00:16:04.000000 WebScripts-3.0.8/WebScripts/static/images/webscripts_icon.png
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.828128 WebScripts-3.0.8/WebScripts/static/js/
--rw-r--r--   0 kali      (1000) kali      (1000)      770 2023-02-04 00:16:06.000000 WebScripts-3.0.8/WebScripts/static/js/webscripts_index_js_scripts.js
--rw-r--r--   0 kali      (1000) kali      (1000)    18252 2023-02-04 00:16:06.000000 WebScripts-3.0.8/WebScripts/static/js/webscripts_js_scripts.js
--rw-r--r--   0 kali      (1000) kali      (1000)    44148 2023-02-19 17:08:38.000000 WebScripts-3.0.8/WebScripts/static/js/webscripts_script_js_scripts.js
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.828128 WebScripts-3.0.8/WebScripts/static/pdf/
--rw-r--r--   0 kali      (1000) kali      (1000)   502927 2023-02-04 00:16:06.000000 WebScripts-3.0.8/WebScripts/static/pdf/WebScripts.pdf
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.828128 WebScripts-3.0.8/WebScripts/static/templates/
--rw-r--r--   0 kali      (1000) kali      (1000)     5650 2023-02-04 00:16:06.000000 WebScripts-3.0.8/WebScripts/static/templates/footer.html
--rw-r--r--   0 kali      (1000) kali      (1000)     2003 2023-02-04 00:16:06.000000 WebScripts-3.0.8/WebScripts/static/templates/header.html
--rw-r--r--   0 kali      (1000) kali      (1000)     2857 2023-02-04 00:16:06.000000 WebScripts-3.0.8/WebScripts/static/templates/index.html
--rw-r--r--   0 kali      (1000) kali      (1000)     3576 2023-02-19 17:17:04.000000 WebScripts-3.0.8/WebScripts/static/templates/script.html
--rw-r--r--   0 kali      (1000) kali      (1000)    34780 2023-02-04 00:27:10.000000 WebScripts-3.0.8/WebScripts/utils.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.808118 WebScripts-3.0.8/WebScripts.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)    20888 2023-02-19 13:10:05.000000 WebScripts-3.0.8/WebScripts.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     7391 2023-02-19 13:10:05.000000 WebScripts-3.0.8/WebScripts.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-02-19 13:10:05.000000 WebScripts-3.0.8/WebScripts.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       47 2023-02-19 13:10:05.000000 WebScripts-3.0.8/WebScripts.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       11 2023-02-19 13:10:05.000000 WebScripts-3.0.8/WebScripts.egg-info/top_level.txt
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.828128 WebScripts-3.0.8/docs/
--rw-r--r--   0 kali      (1000) kali      (1000)    14978 2023-02-13 00:42:18.000000 WebScripts-3.0.8/docs/API.md
--rw-r--r--   0 kali      (1000) kali      (1000)     6107 2023-02-13 00:46:46.000000 WebScripts-3.0.8/docs/API_Client.md
--rw-r--r--   0 kali      (1000) kali      (1000)     1323 2023-02-04 00:47:14.000000 WebScripts-3.0.8/docs/Add_Module.md
--rw-r--r--   0 kali      (1000) kali      (1000)     7204 2023-02-04 00:58:38.000000 WebScripts-3.0.8/docs/Add_Script.md
--rw-r--r--   0 kali      (1000) kali      (1000)     3809 2023-02-13 00:50:20.000000 WebScripts-3.0.8/docs/Argument_Configuration.md
--rw-r--r--   0 kali      (1000) kali      (1000)     2165 2023-02-13 01:05:58.000000 WebScripts-3.0.8/docs/Authentication.md
--rw-r--r--   0 kali      (1000) kali      (1000)    34631 2023-02-13 01:10:22.000000 WebScripts-3.0.8/docs/Code_Analysis_for_Security.md
--rw-r--r--   0 kali      (1000) kali      (1000)     4105 2023-02-13 01:12:18.000000 WebScripts-3.0.8/docs/Default_Database.md
--rw-r--r--   0 kali      (1000) kali      (1000)    12059 2023-02-16 15:35:54.000000 WebScripts-3.0.8/docs/Deployment.md
--rw-r--r--   0 kali      (1000) kali      (1000)     4736 2023-02-13 01:28:48.000000 WebScripts-3.0.8/docs/Development_and_Administration_Tools.md
--rw-r--r--   0 kali      (1000) kali      (1000)    10710 2023-02-13 01:45:08.000000 WebScripts-3.0.8/docs/File_Share.md
--rw-r--r--   0 kali      (1000) kali      (1000)     8412 2023-02-16 15:33:58.000000 WebScripts-3.0.8/docs/Installation.md
--rw-r--r--   0 kali      (1000) kali      (1000)     3707 2023-02-13 02:04:40.000000 WebScripts-3.0.8/docs/Logs.md
--rw-r--r--   0 kali      (1000) kali      (1000)    13687 2023-02-13 02:17:02.000000 WebScripts-3.0.8/docs/Modules.md
--rw-r--r--   0 kali      (1000) kali      (1000)    71017 2023-02-04 00:16:00.000000 WebScripts-3.0.8/docs/Pentest.md
--rw-r--r--   0 kali      (1000) kali      (1000)    12275 2023-02-14 19:35:20.000000 WebScripts-3.0.8/docs/Script_Configuration.md
--rw-r--r--   0 kali      (1000) kali      (1000)     9861 2023-02-15 00:42:54.000000 WebScripts-3.0.8/docs/Security_Considerations.md
--rw-r--r--   0 kali      (1000) kali      (1000)    14328 2023-02-15 00:49:40.000000 WebScripts-3.0.8/docs/Server_Configuration.md
--rw-r--r--   0 kali      (1000) kali      (1000)     6565 2023-02-15 01:04:48.000000 WebScripts-3.0.8/docs/Usages.md
--rw-r--r--   0 kali      (1000) kali      (1000)     4701 2023-02-15 03:24:16.000000 WebScripts-3.0.8/docs/Users_Access_and_Rights.md
--rw-r--r--   0 kali      (1000) kali      (1000)     2702 2023-02-04 00:16:00.000000 WebScripts-3.0.8/docs/WEB_Interface.md
--rw-r--r--   0 kali      (1000) kali      (1000)    19254 2023-02-16 15:30:54.000000 WebScripts-3.0.8/docs/index.md
--rw-r--r--   0 kali      (1000) kali      (1000)     1571 2023-02-04 00:16:06.000000 WebScripts-3.0.8/mkdocs.yml
--rw-r--r--   0 kali      (1000) kali      (1000)        2 2023-02-04 00:15:52.000000 WebScripts-3.0.8/requirenments.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-02-19 13:10:05.832130 WebScripts-3.0.8/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)    17542 2023-02-13 01:47:46.000000 WebScripts-3.0.8/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.828128 WebScripts-3.0.8/test/
--rw-r--r--   0 kali      (1000) kali      (1000)    26907 2023-02-04 00:28:48.000000 WebScripts-3.0.8/test/TestCommons.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2759 2023-02-04 00:15:48.000000 WebScripts-3.0.8/test/TestErrors.py
--rw-r--r--   0 kali      (1000) kali      (1000)    39093 2023-02-04 00:28:52.000000 WebScripts-3.0.8/test/TestPages.py
--rw-r--r--   0 kali      (1000) kali      (1000)    23242 2023-02-04 00:28:54.000000 WebScripts-3.0.8/test/TestUtils.py
--rw-r--r--   0 kali      (1000) kali      (1000)    53387 2023-02-04 00:28:56.000000 WebScripts-3.0.8/test/TestWebScripts.py
--rw-r--r--   0 kali      (1000) kali      (1000)    12009 2023-02-04 00:28:58.000000 WebScripts-3.0.8/test/TestWebScriptsImports.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.832130 WebScripts-3.0.8/test/modules/
--rw-r--r--   0 kali      (1000) kali      (1000)       19 2023-02-04 00:15:48.000000 WebScripts-3.0.8/test/modules/test.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.804116 WebScripts-3.0.8/test/static/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.832130 WebScripts-3.0.8/test/static/css/
--rw-r--r--   0 kali      (1000) kali      (1000)        4 2023-02-04 00:15:48.000000 WebScripts-3.0.8/test/static/css/test.css
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 13:10:05.832130 WebScripts-3.0.8/test/static/js/
--rw-r--r--   0 kali      (1000) kali      (1000)        4 2023-02-04 00:15:48.000000 WebScripts-3.0.8/test/static/js/test.js
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-02-04 00:15:48.000000 WebScripts-3.0.8/test/test.ini
--rw-r--r--   0 kali      (1000) kali      (1000)       24 2023-02-04 00:15:48.000000 WebScripts-3.0.8/test/test.json
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.748826 WebScripts-3.0.9/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/.github/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/.github/workflows/
+-rw-r--r--   0 kali      (1000) kali      (1000)      877 2023-02-02 22:30:36.000000 WebScripts-3.0.9/.github/workflows/WebScripts38_test.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)     1658 2023-02-04 00:15:58.000000 WebScripts-3.0.9/.github/workflows/ZAP.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)     1673 2023-02-04 00:15:58.000000 WebScripts-3.0.9/.github/workflows/ZAP2.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)      569 2023-02-04 00:15:58.000000 WebScripts-3.0.9/.github/workflows/bandit.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)     1042 2023-02-02 22:30:36.000000 WebScripts-3.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)     2529 2023-02-04 00:15:58.000000 WebScripts-3.0.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)     4076 2023-02-04 00:15:58.000000 WebScripts-3.0.9/.github/workflows/kali_tools_scans.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-02-04 00:15:58.000000 WebScripts-3.0.9/.github/workflows/nuclei.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)      279 2023-02-04 00:15:58.000000 WebScripts-3.0.9/.github/workflows/pycharm.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)      317 2023-02-04 00:15:58.000000 WebScripts-3.0.9/.github/workflows/safety_check.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)      379 2023-02-04 00:15:58.000000 WebScripts-3.0.9/.github/workflows/semgrep.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)     1699 2023-02-04 00:15:46.000000 WebScripts-3.0.9/.github/workflows/unittest.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)     1808 2023-02-04 00:15:46.000000 WebScripts-3.0.9/.github/workflows/unittest38.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)     2508 2023-02-04 00:16:06.000000 WebScripts-3.0.9/.gitlab-ci.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)      135 2023-02-04 00:16:06.000000 WebScripts-3.0.9/.readthedocs.yaml
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-02-04 00:16:06.000000 WebScripts-3.0.9/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      641 2023-02-04 00:18:14.000000 WebScripts-3.0.9/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)    20888 2023-02-19 15:56:09.748826 WebScripts-3.0.9/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)    19254 2023-02-16 15:30:44.000000 WebScripts-3.0.9/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/Scripts/
+-rw-r--r--   0 kali      (1000) kali      (1000)      939 2023-02-04 00:16:00.000000 WebScripts-3.0.9/Scripts/activate_this.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2810 2023-02-04 00:16:00.000000 WebScripts-3.0.9/Scripts/wsgi.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2944 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/Errors.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    31835 2023-02-04 00:27:08.000000 WebScripts-3.0.9/WebScripts/Pages.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    69395 2023-02-19 21:43:12.000000 WebScripts-3.0.9/WebScripts/WebScripts.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1845 2023-02-19 15:54:28.000000 WebScripts-3.0.9/WebScripts/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1758 2023-02-19 15:53:34.000000 WebScripts-3.0.9/WebScripts/__main__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/cgi-bin/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3549 2023-02-02 22:30:42.000000 WebScripts-3.0.9/WebScripts/cgi-bin/hello.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      117 2023-02-02 22:30:42.000000 WebScripts-3.0.9/WebScripts/cgi-bin/test.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    37675 2023-02-04 00:26:58.000000 WebScripts-3.0.9/WebScripts/commons.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/config/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/config/files/
+-rw-r--r--   0 kali      (1000) kali      (1000)      951 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/config/files/change_my_password.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     1857 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/config/files/test_config.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     4052 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/config/loggers.ini
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/config/nt/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/config/nt/files/
+-rw-r--r--   0 kali      (1000) kali      (1000)      698 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/config/nt/files/change_my_password.ini
+-rw-r--r--   0 kali      (1000) kali      (1000)      893 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/config/nt/files/change_my_password.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     1823 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/config/nt/files/test_config.json
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/config/nt/scripts/
+-rw-r--r--   0 kali      (1000) kali      (1000)     7259 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/config/nt/scripts/default_admin_scripts.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     2349 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/config/nt/scripts/default_log_scripts.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     2172 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/config/nt/scripts/default_password_scripts.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     1499 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/config/nt/scripts/default_requests_scripts.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     1510 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/config/nt/scripts/default_rss_scripts.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     7248 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/config/nt/scripts/default_uploads_scripts.json
+-rw-r--r--   0 kali      (1000) kali      (1000)    17377 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/config/nt/server.ini
+-rw-r--r--   0 kali      (1000) kali      (1000)     3660 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/config/nt/server.json
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/config/scripts/
+-rw-r--r--   0 kali      (1000) kali      (1000)     7889 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/config/scripts/default_admin_scripts.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     2345 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/config/scripts/default_log_scripts.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     2189 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/config/scripts/default_password_scripts.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     1551 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/config/scripts/default_requests_scripts.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     1562 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/config/scripts/default_rss_scripts.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     8034 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/config/scripts/default_uploads_scripts.json
+-rw-r--r--   0 kali      (1000) kali      (1000)    17373 2023-02-04 00:16:00.000000 WebScripts-3.0.9/WebScripts/config/server.ini
+-rw-r--r--   0 kali      (1000) kali      (1000)     3634 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/config/server.json
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/data/
+-rw-r--r--   0 kali      (1000) kali      (1000)      131 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/data/groups.csv
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/data/id
+-rw-r--r--   0 kali      (1000) kali      (1000)       11 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/data/passwords.csv
+-rw-r--r--   0 kali      (1000) kali      (1000)       63 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/data/requests.csv
+-rw-r--r--   0 kali      (1000) kali      (1000)       64 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/data/rss.csv
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/data/uploads/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35823 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/data/uploads/LICENSE_210725_181116.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       73 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/data/uploads.csv
+-rw-r--r--   0 kali      (1000) kali      (1000)      527 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/data/users.csv
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/doc/
+-rw-r--r--   0 kali      (1000) kali      (1000)        4 2023-02-04 00:16:02.000000 WebScripts-3.0.9/WebScripts/doc/empty.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    17474 2023-02-15 12:49:06.000000 WebScripts-3.0.9/WebScripts/harden.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    73284 2023-02-19 18:53:30.000000 WebScripts-3.0.9/WebScripts/hardening.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/modules/
+-rw-r--r--   0 kali      (1000) kali      (1000)    11468 2023-02-04 00:27:28.000000 WebScripts-3.0.9/WebScripts/modules/Configurations.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6139 2023-02-04 00:27:34.000000 WebScripts-3.0.9/WebScripts/modules/JsonRpc.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4841 2023-02-04 00:27:26.000000 WebScripts-3.0.9/WebScripts/modules/cgi.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2983 2023-02-04 00:27:30.000000 WebScripts-3.0.9/WebScripts/modules/csp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    13294 2023-02-04 00:27:32.000000 WebScripts-3.0.9/WebScripts/modules/error_pages.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4814 2023-02-04 00:27:36.000000 WebScripts-3.0.9/WebScripts/modules/notification.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     8254 2023-02-04 00:27:38.000000 WebScripts-3.0.9/WebScripts/modules/rss.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7142 2023-02-04 00:27:40.000000 WebScripts-3.0.9/WebScripts/modules/share.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/scripts/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/scripts/account/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2402 2023-02-04 00:16:02.000000 WebScripts-3.0.9/WebScripts/scripts/account/add_group.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4399 2023-02-04 00:28:14.000000 WebScripts-3.0.9/WebScripts/scripts/account/add_user.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3191 2023-02-04 00:28:14.000000 WebScripts-3.0.9/WebScripts/scripts/account/api_view_groups.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3173 2023-02-04 00:28:16.000000 WebScripts-3.0.9/WebScripts/scripts/account/api_view_users.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3458 2023-02-04 00:28:18.000000 WebScripts-3.0.9/WebScripts/scripts/account/auth.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3264 2023-02-04 00:28:18.000000 WebScripts-3.0.9/WebScripts/scripts/account/change_my_password.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2708 2023-02-04 00:28:20.000000 WebScripts-3.0.9/WebScripts/scripts/account/change_user_password.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2417 2023-02-04 00:16:02.000000 WebScripts-3.0.9/WebScripts/scripts/account/delete_group.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2386 2023-02-04 00:16:02.000000 WebScripts-3.0.9/WebScripts/scripts/account/delete_user.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2337 2023-02-04 00:28:24.000000 WebScripts-3.0.9/WebScripts/scripts/account/get_apikey.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/scripts/account/modules/
+-rw-r--r--   0 kali      (1000) kali      (1000)    14352 2023-02-04 00:27:24.000000 WebScripts-3.0.9/WebScripts/scripts/account/modules/manage_defaults_databases.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2439 2023-02-04 00:28:26.000000 WebScripts-3.0.9/WebScripts/scripts/account/my_user_informations.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3193 2023-02-04 00:28:28.000000 WebScripts-3.0.9/WebScripts/scripts/account/view_groups.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3379 2023-02-04 00:28:28.000000 WebScripts-3.0.9/WebScripts/scripts/account/view_users.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/scripts/doc/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3137 2023-02-04 00:28:34.000000 WebScripts-3.0.9/WebScripts/scripts/doc/py_doc.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/scripts/logs/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3955 2023-02-04 00:28:36.000000 WebScripts-3.0.9/WebScripts/scripts/logs/log_analysis.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3298 2023-02-04 00:28:36.000000 WebScripts-3.0.9/WebScripts/scripts/logs/log_viewer.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/scripts/passwords/
+-rw-r--r--   0 kali      (1000) kali      (1000)     5607 2023-02-04 00:28:38.000000 WebScripts-3.0.9/WebScripts/scripts/passwords/get_password_share.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6016 2023-02-04 00:28:40.000000 WebScripts-3.0.9/WebScripts/scripts/passwords/new_password_share.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1988 2023-02-04 00:16:02.000000 WebScripts-3.0.9/WebScripts/scripts/passwords/password_generator.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/scripts/py/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2816 2023-02-04 00:16:02.000000 WebScripts-3.0.9/WebScripts/scripts/py/ASCII_arts.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      893 2023-02-04 00:16:02.000000 WebScripts-3.0.9/WebScripts/scripts/py/hello.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3495 2023-02-04 00:28:46.000000 WebScripts-3.0.9/WebScripts/scripts/py/show_license.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      724 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/scripts/py/test_config.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/scripts/request/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2669 2023-02-04 00:28:30.000000 WebScripts-3.0.9/WebScripts/scripts/request/delete_request.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2590 2023-02-04 00:28:32.000000 WebScripts-3.0.9/WebScripts/scripts/request/get_request.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3092 2023-02-04 00:28:32.000000 WebScripts-3.0.9/WebScripts/scripts/request/get_requests.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/scripts/request/modules/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3979 2023-02-04 00:27:26.000000 WebScripts-3.0.9/WebScripts/scripts/request/modules/requests_management.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/scripts/rss/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4311 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/scripts/rss/add_news.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/scripts/to_3.8/
+-rw-r--r--   0 kali      (1000) kali      (1000)     6639 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/scripts/to_3.8/to_3.8.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/scripts/uploads/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3358 2023-02-04 00:27:56.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/HTML_all_files.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3334 2023-02-04 00:27:58.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/HTML_file_history.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3169 2023-02-04 00:28:00.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/HTML_uploads_properties.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2722 2023-02-04 00:28:00.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/HTML_uploads_size.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3241 2023-02-04 00:28:02.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/HTML_visible_files.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2435 2023-02-04 00:28:04.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/JSON_all_files.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2459 2023-02-04 00:28:04.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/JSON_file_history.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2560 2023-02-04 00:28:06.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/JSON_uploads_properties.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2619 2023-02-04 00:28:08.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/JSON_uploads_size.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2520 2023-02-04 00:28:10.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/JSON_visible_files.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2358 2023-02-04 00:27:42.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/api_get_all_files.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2418 2023-02-04 00:27:42.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/api_get_files.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2409 2023-02-04 00:27:44.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/api_get_history.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2335 2023-02-04 00:27:46.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/delete_file.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3318 2023-02-04 00:27:46.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/download_all_files.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3223 2023-02-04 00:27:48.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/download_filename.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3080 2023-02-04 00:27:50.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/get_all_files.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3302 2023-02-04 00:27:50.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/get_any_file.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3169 2023-02-04 00:27:52.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/get_file.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2926 2023-02-04 00:27:54.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/get_files.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3234 2023-02-04 00:27:54.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/get_history.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/scripts/uploads/modules/
+-rw-r--r--   0 kali      (1000) kali      (1000)    14751 2023-02-04 00:27:20.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/modules/uploads_management.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3991 2023-02-04 00:28:10.000000 WebScripts-3.0.9/WebScripts/scripts/uploads/upload_file.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/static/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/static/css/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1081 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/css/webscripts_index_style.css
+-rw-r--r--   0 kali      (1000) kali      (1000)     4396 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/css/webscripts_script_style.css
+-rw-r--r--   0 kali      (1000) kali      (1000)     9367 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/css/webscripts_style.css
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/static/html/
+-rw-r--r--   0 kali      (1000) kali      (1000)     7315 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/Configurations.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    32878 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/Errors.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     6040 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/JsonRpc.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     7973 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/Pages.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    25005 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/WebScripts.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    18945 2023-02-04 00:15:52.000000 WebScripts-3.0.9/WebScripts/static/html/__init__.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    23520 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/cgi.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    45403 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/commons.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     4294 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/html/csp.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     8559 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/html/error_pages.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     3203 2023-02-04 00:15:52.000000 WebScripts-3.0.9/WebScripts/static/html/get_request.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    22071 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/hardening.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    23909 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/index.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    27613 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/manage_defaults_databases.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     3344 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/html/notification.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    12153 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/requests_management.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    13953 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/rss.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     7503 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/html/share.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    18391 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/uploads_management.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    35209 2023-02-19 21:44:56.000000 WebScripts-3.0.9/WebScripts/static/html/utils.html
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/static/images/
+-rw-r--r--   0 kali      (1000) kali      (1000)    90843 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/images/WebScripts1.png
+-rw-r--r--   0 kali      (1000) kali      (1000)    99659 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/images/WebScripts2.png
+-rw-r--r--   0 kali      (1000) kali      (1000)    97909 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/images/WebScripts3.png
+-rw-r--r--   0 kali      (1000) kali      (1000)    88696 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/images/WebScripts4.png
+-rw-r--r--   0 kali      (1000) kali      (1000)    95444 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/images/WebScripts5.png
+-rw-r--r--   0 kali      (1000) kali      (1000)    95082 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/images/WebScripts6.png
+-rw-r--r--   0 kali      (1000) kali      (1000)    32125 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/images/WebScripts7.png
+-rw-r--r--   0 kali      (1000) kali      (1000)    44039 2023-02-04 00:15:52.000000 WebScripts-3.0.9/WebScripts/static/images/webscripts_header.jpg
+-rw-r--r--   0 kali      (1000) kali      (1000)    95444 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/images/webscripts_header.png
+-rw-r--r--   0 kali      (1000) kali      (1000)    44039 2023-02-04 00:15:52.000000 WebScripts-3.0.9/WebScripts/static/images/webscripts_icon.jpg
+-rw-r--r--   0 kali      (1000) kali      (1000)    95082 2023-02-04 00:16:04.000000 WebScripts-3.0.9/WebScripts/static/images/webscripts_icon.png
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/static/js/
+-rw-r--r--   0 kali      (1000) kali      (1000)      770 2023-02-04 00:16:06.000000 WebScripts-3.0.9/WebScripts/static/js/webscripts_index_js_scripts.js
+-rw-r--r--   0 kali      (1000) kali      (1000)    18252 2023-02-04 00:16:06.000000 WebScripts-3.0.9/WebScripts/static/js/webscripts_js_scripts.js
+-rw-r--r--   0 kali      (1000) kali      (1000)    44148 2023-02-19 17:08:38.000000 WebScripts-3.0.9/WebScripts/static/js/webscripts_script_js_scripts.js
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/static/pdf/
+-rw-r--r--   0 kali      (1000) kali      (1000)   502927 2023-02-04 00:16:06.000000 WebScripts-3.0.9/WebScripts/static/pdf/WebScripts.pdf
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts/static/templates/
+-rw-r--r--   0 kali      (1000) kali      (1000)     5650 2023-02-04 00:16:06.000000 WebScripts-3.0.9/WebScripts/static/templates/footer.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     2003 2023-02-04 00:16:06.000000 WebScripts-3.0.9/WebScripts/static/templates/header.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     2857 2023-02-04 00:16:06.000000 WebScripts-3.0.9/WebScripts/static/templates/index.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     3576 2023-02-19 17:17:04.000000 WebScripts-3.0.9/WebScripts/static/templates/script.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    34780 2023-02-04 00:27:10.000000 WebScripts-3.0.9/WebScripts/utils.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/WebScripts.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)    20888 2023-02-19 15:56:09.000000 WebScripts-3.0.9/WebScripts.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     7391 2023-02-19 15:56:09.000000 WebScripts-3.0.9/WebScripts.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-02-19 15:56:09.000000 WebScripts-3.0.9/WebScripts.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       47 2023-02-19 15:56:09.000000 WebScripts-3.0.9/WebScripts.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       11 2023-02-19 15:56:09.000000 WebScripts-3.0.9/WebScripts.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.748826 WebScripts-3.0.9/docs/
+-rw-r--r--   0 kali      (1000) kali      (1000)    14978 2023-02-13 00:42:18.000000 WebScripts-3.0.9/docs/API.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     6107 2023-02-13 00:46:46.000000 WebScripts-3.0.9/docs/API_Client.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     1323 2023-02-04 00:47:14.000000 WebScripts-3.0.9/docs/Add_Module.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     7204 2023-02-04 00:58:38.000000 WebScripts-3.0.9/docs/Add_Script.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     3809 2023-02-13 00:50:20.000000 WebScripts-3.0.9/docs/Argument_Configuration.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     2165 2023-02-13 01:05:58.000000 WebScripts-3.0.9/docs/Authentication.md
+-rw-r--r--   0 kali      (1000) kali      (1000)    34631 2023-02-13 01:10:22.000000 WebScripts-3.0.9/docs/Code_Analysis_for_Security.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     4105 2023-02-13 01:12:18.000000 WebScripts-3.0.9/docs/Default_Database.md
+-rw-r--r--   0 kali      (1000) kali      (1000)    12059 2023-02-16 15:35:54.000000 WebScripts-3.0.9/docs/Deployment.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     4736 2023-02-13 01:28:48.000000 WebScripts-3.0.9/docs/Development_and_Administration_Tools.md
+-rw-r--r--   0 kali      (1000) kali      (1000)    10710 2023-02-13 01:45:08.000000 WebScripts-3.0.9/docs/File_Share.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     8412 2023-02-16 15:33:58.000000 WebScripts-3.0.9/docs/Installation.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     3707 2023-02-13 02:04:40.000000 WebScripts-3.0.9/docs/Logs.md
+-rw-r--r--   0 kali      (1000) kali      (1000)    13687 2023-02-13 02:17:02.000000 WebScripts-3.0.9/docs/Modules.md
+-rw-r--r--   0 kali      (1000) kali      (1000)    71017 2023-02-04 00:16:00.000000 WebScripts-3.0.9/docs/Pentest.md
+-rw-r--r--   0 kali      (1000) kali      (1000)    12275 2023-02-14 19:35:20.000000 WebScripts-3.0.9/docs/Script_Configuration.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     9861 2023-02-15 00:42:54.000000 WebScripts-3.0.9/docs/Security_Considerations.md
+-rw-r--r--   0 kali      (1000) kali      (1000)    14328 2023-02-15 00:49:40.000000 WebScripts-3.0.9/docs/Server_Configuration.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     6565 2023-02-15 01:04:48.000000 WebScripts-3.0.9/docs/Usages.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     4701 2023-02-15 03:24:16.000000 WebScripts-3.0.9/docs/Users_Access_and_Rights.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     2702 2023-02-04 00:16:00.000000 WebScripts-3.0.9/docs/WEB_Interface.md
+-rw-r--r--   0 kali      (1000) kali      (1000)    19254 2023-02-16 15:30:54.000000 WebScripts-3.0.9/docs/index.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     1571 2023-02-04 00:16:06.000000 WebScripts-3.0.9/mkdocs.yml
+-rw-r--r--   0 kali      (1000) kali      (1000)        2 2023-02-04 00:15:52.000000 WebScripts-3.0.9/requirenments.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-02-19 15:56:09.748826 WebScripts-3.0.9/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)    17542 2023-02-13 01:47:46.000000 WebScripts-3.0.9/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.748826 WebScripts-3.0.9/test/
+-rw-r--r--   0 kali      (1000) kali      (1000)    26907 2023-02-04 00:28:48.000000 WebScripts-3.0.9/test/TestCommons.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2759 2023-02-04 00:15:48.000000 WebScripts-3.0.9/test/TestErrors.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    39093 2023-02-04 00:28:52.000000 WebScripts-3.0.9/test/TestPages.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    23242 2023-02-04 00:28:54.000000 WebScripts-3.0.9/test/TestUtils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    53387 2023-02-04 00:28:56.000000 WebScripts-3.0.9/test/TestWebScripts.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    12009 2023-02-04 00:28:58.000000 WebScripts-3.0.9/test/TestWebScriptsImports.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.748826 WebScripts-3.0.9/test/modules/
+-rw-r--r--   0 kali      (1000) kali      (1000)       19 2023-02-04 00:15:48.000000 WebScripts-3.0.9/test/modules/test.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.720840 WebScripts-3.0.9/test/static/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.748826 WebScripts-3.0.9/test/static/css/
+-rw-r--r--   0 kali      (1000) kali      (1000)        4 2023-02-04 00:15:48.000000 WebScripts-3.0.9/test/static/css/test.css
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-19 15:56:09.748826 WebScripts-3.0.9/test/static/js/
+-rw-r--r--   0 kali      (1000) kali      (1000)        4 2023-02-04 00:15:48.000000 WebScripts-3.0.9/test/static/js/test.js
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-02-04 00:15:48.000000 WebScripts-3.0.9/test/test.ini
+-rw-r--r--   0 kali      (1000) kali      (1000)       24 2023-02-04 00:15:48.000000 WebScripts-3.0.9/test/test.json
```

### Comparing `WebScripts-3.0.8/.github/workflows/WebScripts38_test.yml` & `WebScripts-3.0.9/.github/workflows/WebScripts38_test.yml`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/.github/workflows/ZAP.yml` & `WebScripts-3.0.9/.github/workflows/ZAP.yml`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/.github/workflows/ZAP2.yml` & `WebScripts-3.0.9/.github/workflows/ZAP2.yml`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/.github/workflows/bandit.yml` & `WebScripts-3.0.9/.github/workflows/bandit.yml`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/.github/workflows/ci.yml` & `WebScripts-3.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/.github/workflows/codeql-analysis.yml` & `WebScripts-3.0.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/.github/workflows/kali_tools_scans.yml` & `WebScripts-3.0.9/.github/workflows/kali_tools_scans.yml`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/.github/workflows/nuclei.yml` & `WebScripts-3.0.9/.github/workflows/nuclei.yml`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/.github/workflows/unittest.yml` & `WebScripts-3.0.9/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/.github/workflows/unittest38.yml` & `WebScripts-3.0.9/.github/workflows/unittest38.yml`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/.gitlab-ci.yml` & `WebScripts-3.0.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/LICENSE.txt` & `WebScripts-3.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/MANIFEST.in` & `WebScripts-3.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/PKG-INFO` & `WebScripts-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebScripts
-Version: 3.0.8
+Version: 3.0.9
 Summary: This tool runs CLI scripts and displays output in a Web Interface.
 Home-page: https://github.com/mauricelambert/WebScripts
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `WebScripts-3.0.8/README.md` & `WebScripts-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/Scripts/activate_this.py` & `WebScripts-3.0.9/Scripts/activate_this.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/Scripts/wsgi.py` & `WebScripts-3.0.9/Scripts/wsgi.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/Errors.py` & `WebScripts-3.0.9/WebScripts/Errors.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/LICENSE.txt` & `WebScripts-3.0.9/WebScripts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/Pages.py` & `WebScripts-3.0.9/WebScripts/Pages.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/WebScripts.py` & `WebScripts-3.0.9/WebScripts/WebScripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """
 This tool runs CLI scripts and displays output in a Web Interface.
 
 This file is the "main" file of this package (implements the main function,
 the Server class and the Configuration class).
 """
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This tool runs CLI scripts and displays output in a Web Interface.
 
@@ -967,15 +967,19 @@
         This function checks Origin of POST methods.
         """
 
         logger_debug("Check origin...")
         origin = environ_getter("HTTP_ORIGIN")
         url = Server.get_baseurl(environ_getter, environ)
 
-        if origin != url:
+        if origin != url or (
+            origin.startswith("https://")
+            and url.startswith("http://")
+            and origin[7:] == url[6:]
+        ):
             logger_info(f'Bad Origin detected: "{origin}" != "{url}"')
             return False
 
         logger_info("Correct Origin detected.")
         return True
 
     @staticmethod
```

### Comparing `WebScripts-3.0.8/WebScripts/__init__.py` & `WebScripts-3.0.9/WebScripts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ###################
 
 """
 This tool runs CLI scripts and displays output in a Web Interface.
 """
 
-__version__ = "3.0.8"
+__version__ = "3.0.9"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = (
     "This tool runs CLI scripts and displays output in a Web Interface."
 )
```

### Comparing `WebScripts-3.0.8/WebScripts/__main__.py` & `WebScripts-3.0.9/WebScripts/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ###################
 
 """
 This tool runs CLI scripts and displays output in a Web Interface.
 """
 
-__version__ = "3.0.8"
+__version__ = "3.0.9"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = (
     "This tool runs CLI scripts and displays output in a Web Interface."
 )
```

### Comparing `WebScripts-3.0.8/WebScripts/cgi-bin/hello.py` & `WebScripts-3.0.9/WebScripts/cgi-bin/hello.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/commons.py` & `WebScripts-3.0.9/WebScripts/commons.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/files/change_my_password.json` & `WebScripts-3.0.9/WebScripts/config/files/change_my_password.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/files/test_config.json` & `WebScripts-3.0.9/WebScripts/config/files/test_config.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/loggers.ini` & `WebScripts-3.0.9/WebScripts/config/loggers.ini`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/nt/files/change_my_password.ini` & `WebScripts-3.0.9/WebScripts/config/nt/files/change_my_password.ini`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/nt/files/change_my_password.json` & `WebScripts-3.0.9/WebScripts/config/nt/files/change_my_password.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/nt/files/test_config.json` & `WebScripts-3.0.9/WebScripts/config/nt/files/test_config.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/nt/scripts/default_admin_scripts.json` & `WebScripts-3.0.9/WebScripts/config/nt/scripts/default_admin_scripts.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/nt/scripts/default_log_scripts.json` & `WebScripts-3.0.9/WebScripts/config/nt/scripts/default_log_scripts.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/nt/scripts/default_password_scripts.json` & `WebScripts-3.0.9/WebScripts/config/nt/scripts/default_password_scripts.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/nt/scripts/default_requests_scripts.json` & `WebScripts-3.0.9/WebScripts/config/nt/scripts/default_requests_scripts.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/nt/scripts/default_rss_scripts.json` & `WebScripts-3.0.9/WebScripts/config/nt/scripts/default_rss_scripts.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/nt/scripts/default_uploads_scripts.json` & `WebScripts-3.0.9/WebScripts/config/nt/scripts/default_uploads_scripts.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/nt/server.ini` & `WebScripts-3.0.9/WebScripts/config/nt/server.ini`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/nt/server.json` & `WebScripts-3.0.9/WebScripts/config/nt/server.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/scripts/default_admin_scripts.json` & `WebScripts-3.0.9/WebScripts/config/scripts/default_admin_scripts.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/scripts/default_log_scripts.json` & `WebScripts-3.0.9/WebScripts/config/scripts/default_log_scripts.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/scripts/default_password_scripts.json` & `WebScripts-3.0.9/WebScripts/config/scripts/default_password_scripts.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/scripts/default_requests_scripts.json` & `WebScripts-3.0.9/WebScripts/config/scripts/default_requests_scripts.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/scripts/default_rss_scripts.json` & `WebScripts-3.0.9/WebScripts/config/scripts/default_rss_scripts.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/scripts/default_uploads_scripts.json` & `WebScripts-3.0.9/WebScripts/config/scripts/default_uploads_scripts.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/server.ini` & `WebScripts-3.0.9/WebScripts/config/server.ini`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/config/server.json` & `WebScripts-3.0.9/WebScripts/config/server.json`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/data/uploads/LICENSE_210725_181116.txt` & `WebScripts-3.0.9/WebScripts/data/uploads/LICENSE_210725_181116.txt`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/data/users.csv` & `WebScripts-3.0.9/WebScripts/data/users.csv`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/harden.py` & `WebScripts-3.0.9/WebScripts/harden.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/hardening.py` & `WebScripts-3.0.9/WebScripts/hardening.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/modules/Configurations.py` & `WebScripts-3.0.9/WebScripts/modules/Configurations.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/modules/JsonRpc.py` & `WebScripts-3.0.9/WebScripts/modules/JsonRpc.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/modules/cgi.py` & `WebScripts-3.0.9/WebScripts/modules/cgi.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/modules/csp.py` & `WebScripts-3.0.9/WebScripts/modules/csp.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/modules/error_pages.py` & `WebScripts-3.0.9/WebScripts/modules/error_pages.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/modules/notification.py` & `WebScripts-3.0.9/WebScripts/modules/notification.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/modules/rss.py` & `WebScripts-3.0.9/WebScripts/modules/rss.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/modules/share.py` & `WebScripts-3.0.9/WebScripts/modules/share.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/add_group.py` & `WebScripts-3.0.9/WebScripts/scripts/account/add_group.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/add_user.py` & `WebScripts-3.0.9/WebScripts/scripts/account/add_user.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/api_view_groups.py` & `WebScripts-3.0.9/WebScripts/scripts/account/api_view_groups.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/api_view_users.py` & `WebScripts-3.0.9/WebScripts/scripts/account/api_view_users.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/auth.py` & `WebScripts-3.0.9/WebScripts/scripts/account/auth.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/change_my_password.py` & `WebScripts-3.0.9/WebScripts/scripts/account/change_my_password.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/change_user_password.py` & `WebScripts-3.0.9/WebScripts/scripts/account/change_user_password.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/delete_group.py` & `WebScripts-3.0.9/WebScripts/scripts/account/delete_group.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/delete_user.py` & `WebScripts-3.0.9/WebScripts/scripts/account/delete_user.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/get_apikey.py` & `WebScripts-3.0.9/WebScripts/scripts/account/get_apikey.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/modules/manage_defaults_databases.py` & `WebScripts-3.0.9/WebScripts/scripts/account/modules/manage_defaults_databases.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/my_user_informations.py` & `WebScripts-3.0.9/WebScripts/scripts/account/my_user_informations.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/view_groups.py` & `WebScripts-3.0.9/WebScripts/scripts/account/view_groups.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/account/view_users.py` & `WebScripts-3.0.9/WebScripts/scripts/account/view_users.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/doc/py_doc.py` & `WebScripts-3.0.9/WebScripts/scripts/doc/py_doc.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/logs/log_analysis.py` & `WebScripts-3.0.9/WebScripts/scripts/logs/log_analysis.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/logs/log_viewer.py` & `WebScripts-3.0.9/WebScripts/scripts/logs/log_viewer.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/passwords/get_password_share.py` & `WebScripts-3.0.9/WebScripts/scripts/passwords/get_password_share.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/passwords/new_password_share.py` & `WebScripts-3.0.9/WebScripts/scripts/passwords/new_password_share.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/passwords/password_generator.py` & `WebScripts-3.0.9/WebScripts/scripts/passwords/password_generator.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/py/ASCII_arts.py` & `WebScripts-3.0.9/WebScripts/scripts/py/ASCII_arts.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/py/hello.py` & `WebScripts-3.0.9/WebScripts/scripts/py/hello.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/py/show_license.py` & `WebScripts-3.0.9/WebScripts/scripts/py/show_license.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/py/test_config.py` & `WebScripts-3.0.9/WebScripts/scripts/py/test_config.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/request/delete_request.py` & `WebScripts-3.0.9/WebScripts/scripts/request/delete_request.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/request/get_request.py` & `WebScripts-3.0.9/WebScripts/scripts/request/get_request.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/request/get_requests.py` & `WebScripts-3.0.9/WebScripts/scripts/request/get_requests.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/request/modules/requests_management.py` & `WebScripts-3.0.9/WebScripts/scripts/request/modules/requests_management.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/rss/add_news.py` & `WebScripts-3.0.9/WebScripts/scripts/rss/add_news.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/to_3.8/to_3.8.py` & `WebScripts-3.0.9/WebScripts/scripts/to_3.8/to_3.8.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/HTML_all_files.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/HTML_all_files.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/HTML_file_history.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/HTML_file_history.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/HTML_uploads_properties.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/HTML_uploads_properties.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/HTML_uploads_size.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/HTML_uploads_size.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/HTML_visible_files.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/HTML_visible_files.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/JSON_all_files.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/JSON_all_files.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/JSON_file_history.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/JSON_file_history.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/JSON_uploads_properties.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/JSON_uploads_properties.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/JSON_uploads_size.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/JSON_uploads_size.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/JSON_visible_files.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/JSON_visible_files.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/api_get_all_files.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/api_get_all_files.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/api_get_files.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/api_get_files.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/api_get_history.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/api_get_history.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/delete_file.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/delete_file.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/download_all_files.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/download_all_files.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/download_filename.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/download_filename.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/get_all_files.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/get_all_files.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/get_any_file.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/get_any_file.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/get_file.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/get_file.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/get_files.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/get_files.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/get_history.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/get_history.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/modules/uploads_management.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/modules/uploads_management.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/scripts/uploads/upload_file.py` & `WebScripts-3.0.9/WebScripts/scripts/uploads/upload_file.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/css/webscripts_index_style.css` & `WebScripts-3.0.9/WebScripts/static/css/webscripts_index_style.css`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/css/webscripts_script_style.css` & `WebScripts-3.0.9/WebScripts/static/css/webscripts_script_style.css`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/css/webscripts_style.css` & `WebScripts-3.0.9/WebScripts/static/css/webscripts_style.css`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/Configurations.html` & `WebScripts-3.0.9/WebScripts/static/html/Configurations.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/Errors.html` & `WebScripts-3.0.9/WebScripts/static/html/Errors.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/JsonRpc.html` & `WebScripts-3.0.9/WebScripts/static/html/JsonRpc.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/Pages.html` & `WebScripts-3.0.9/WebScripts/static/html/Pages.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/WebScripts.html` & `WebScripts-3.0.9/WebScripts/static/html/WebScripts.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <html><head><title>Python: module WebScripts</title>
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
 </head><body bgcolor="#f0f0f8">
 
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="heading">
 <tr bgcolor="#9286C2">
 <td valign=bottom>&nbsp;<br>
-<font color="#ffffff" face="helvetica, arial">&nbsp;<br><big><big><strong>WebScripts</strong></big></big> (version 1.0.1)</font></td
+<font color="#ffffff" face="helvetica, arial">&nbsp;<br><big><big><strong>WebScripts</strong></big></big> (version 1.0.2)</font></td
 ><td align=right valign=bottom
 ><font color="#ffffff" face="helvetica, arial"><a href=".">index</a><br><a href="webscripts.py">webscripts.py</a></font></td></tr></table>
     <p><tt>This&nbsp;tool&nbsp;runs&nbsp;CLI&nbsp;scripts&nbsp;and&nbsp;displays&nbsp;output&nbsp;in&nbsp;a&nbsp;Web&nbsp;Interface.<br>
 &nbsp;<br>
 This&nbsp;file&nbsp;is&nbsp;the&nbsp;"main"&nbsp;file&nbsp;of&nbsp;this&nbsp;package&nbsp;(implements&nbsp;the&nbsp;main&nbsp;function,<br>
 the&nbsp;<a href="#Server">Server</a>&nbsp;class&nbsp;and&nbsp;the&nbsp;<a href="#Configuration">Configuration</a>&nbsp;class).</tt></p>
 <p>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
  
                                    _i_n_d_e_x
-WWeebbSSccrriippttss (version 1.0.1) _w_e_b_s_c_r_i_p_t_s_._p_y
+WWeebbSSccrriippttss (version 1.0.2) _w_e_b_s_c_r_i_p_t_s_._p_y
 This tool runs CLI scripts and displays output in a Web Interface.
  
 This file is the "main" file of this package (implements the main function,
 the _S_e_r_v_e_r class and the _C_o_n_f_i_g_u_r_a_t_i_o_n class).
  
 MMoodduulleess
          _l_o_g_g_i_n_g _w_s_g_i_r_e_f_._s_i_m_p_l_e___s_e_r_v_e_r _s_y_s
```

### Comparing `WebScripts-3.0.8/WebScripts/static/html/__init__.html` & `WebScripts-3.0.9/WebScripts/static/html/__init__.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/cgi.html` & `WebScripts-3.0.9/WebScripts/static/html/cgi.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/commons.html` & `WebScripts-3.0.9/WebScripts/static/html/commons.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/csp.html` & `WebScripts-3.0.9/WebScripts/static/html/csp.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/error_pages.html` & `WebScripts-3.0.9/WebScripts/static/html/error_pages.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/get_request.html` & `WebScripts-3.0.9/WebScripts/static/html/get_request.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/hardening.html` & `WebScripts-3.0.9/WebScripts/static/html/hardening.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/index.html` & `WebScripts-3.0.9/WebScripts/static/html/index.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/manage_defaults_databases.html` & `WebScripts-3.0.9/WebScripts/static/html/manage_defaults_databases.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/notification.html` & `WebScripts-3.0.9/WebScripts/static/html/notification.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/requests_management.html` & `WebScripts-3.0.9/WebScripts/static/html/requests_management.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/rss.html` & `WebScripts-3.0.9/WebScripts/static/html/rss.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/share.html` & `WebScripts-3.0.9/WebScripts/static/html/share.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/uploads_management.html` & `WebScripts-3.0.9/WebScripts/static/html/uploads_management.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/html/utils.html` & `WebScripts-3.0.9/WebScripts/static/html/utils.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/images/WebScripts1.png` & `WebScripts-3.0.9/WebScripts/static/images/WebScripts1.png`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/images/WebScripts2.png` & `WebScripts-3.0.9/WebScripts/static/images/WebScripts2.png`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/images/WebScripts3.png` & `WebScripts-3.0.9/WebScripts/static/images/WebScripts3.png`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/images/WebScripts4.png` & `WebScripts-3.0.9/WebScripts/static/images/WebScripts4.png`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/images/WebScripts5.png` & `WebScripts-3.0.9/WebScripts/static/images/WebScripts5.png`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/images/WebScripts6.png` & `WebScripts-3.0.9/WebScripts/static/images/WebScripts6.png`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/images/WebScripts7.png` & `WebScripts-3.0.9/WebScripts/static/images/WebScripts7.png`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/images/webscripts_header.jpg` & `WebScripts-3.0.9/WebScripts/static/images/webscripts_header.jpg`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/images/webscripts_header.png` & `WebScripts-3.0.9/WebScripts/static/images/webscripts_header.png`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/images/webscripts_icon.jpg` & `WebScripts-3.0.9/WebScripts/static/images/webscripts_icon.jpg`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/images/webscripts_icon.png` & `WebScripts-3.0.9/WebScripts/static/images/webscripts_icon.png`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/js/webscripts_index_js_scripts.js` & `WebScripts-3.0.9/WebScripts/static/js/webscripts_index_js_scripts.js`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/js/webscripts_js_scripts.js` & `WebScripts-3.0.9/WebScripts/static/js/webscripts_js_scripts.js`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/js/webscripts_script_js_scripts.js` & `WebScripts-3.0.9/WebScripts/static/js/webscripts_script_js_scripts.js`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/pdf/WebScripts.pdf` & `WebScripts-3.0.9/WebScripts/static/pdf/WebScripts.pdf`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/templates/footer.html` & `WebScripts-3.0.9/WebScripts/static/templates/footer.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/templates/header.html` & `WebScripts-3.0.9/WebScripts/static/templates/header.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/templates/index.html` & `WebScripts-3.0.9/WebScripts/static/templates/index.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/static/templates/script.html` & `WebScripts-3.0.9/WebScripts/static/templates/script.html`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts/utils.py` & `WebScripts-3.0.9/WebScripts/utils.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/WebScripts.egg-info/PKG-INFO` & `WebScripts-3.0.9/WebScripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebScripts
-Version: 3.0.8
+Version: 3.0.9
 Summary: This tool runs CLI scripts and displays output in a Web Interface.
 Home-page: https://github.com/mauricelambert/WebScripts
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `WebScripts-3.0.8/WebScripts.egg-info/SOURCES.txt` & `WebScripts-3.0.9/WebScripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/API.md` & `WebScripts-3.0.9/docs/API.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/API_Client.md` & `WebScripts-3.0.9/docs/API_Client.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Add_Module.md` & `WebScripts-3.0.9/docs/Add_Module.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Add_Script.md` & `WebScripts-3.0.9/docs/Add_Script.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Argument_Configuration.md` & `WebScripts-3.0.9/docs/Argument_Configuration.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Authentication.md` & `WebScripts-3.0.9/docs/Authentication.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Code_Analysis_for_Security.md` & `WebScripts-3.0.9/docs/Code_Analysis_for_Security.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Default_Database.md` & `WebScripts-3.0.9/docs/Default_Database.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Deployment.md` & `WebScripts-3.0.9/docs/Deployment.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Development_and_Administration_Tools.md` & `WebScripts-3.0.9/docs/Development_and_Administration_Tools.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/File_Share.md` & `WebScripts-3.0.9/docs/File_Share.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Installation.md` & `WebScripts-3.0.9/docs/Installation.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Logs.md` & `WebScripts-3.0.9/docs/Logs.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Modules.md` & `WebScripts-3.0.9/docs/Modules.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Pentest.md` & `WebScripts-3.0.9/docs/Pentest.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Script_Configuration.md` & `WebScripts-3.0.9/docs/Script_Configuration.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Security_Considerations.md` & `WebScripts-3.0.9/docs/Security_Considerations.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Server_Configuration.md` & `WebScripts-3.0.9/docs/Server_Configuration.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Usages.md` & `WebScripts-3.0.9/docs/Usages.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/Users_Access_and_Rights.md` & `WebScripts-3.0.9/docs/Users_Access_and_Rights.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/WEB_Interface.md` & `WebScripts-3.0.9/docs/WEB_Interface.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/docs/index.md` & `WebScripts-3.0.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/mkdocs.yml` & `WebScripts-3.0.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/setup.py` & `WebScripts-3.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/test/TestCommons.py` & `WebScripts-3.0.9/test/TestCommons.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/test/TestErrors.py` & `WebScripts-3.0.9/test/TestErrors.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/test/TestPages.py` & `WebScripts-3.0.9/test/TestPages.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/test/TestUtils.py` & `WebScripts-3.0.9/test/TestUtils.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/test/TestWebScripts.py` & `WebScripts-3.0.9/test/TestWebScripts.py`

 * *Files identical despite different names*

### Comparing `WebScripts-3.0.8/test/TestWebScriptsImports.py` & `WebScripts-3.0.9/test/TestWebScriptsImports.py`

 * *Files identical despite different names*

