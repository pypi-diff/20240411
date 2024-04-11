# Comparing `tmp/netbox-config-diff-2.2.0.tar.gz` & `tmp/netbox-config-diff-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-config-diff-2.2.0.tar", last modified: Tue Feb  6 09:10:35 2024, max compression
+gzip compressed data, was "netbox-config-diff-2.3.0.tar", last modified: Thu Apr 11 13:48:39 2024, max compression
```

## Comparing `netbox-config-diff-2.2.0.tar` & `netbox-config-diff-2.3.0.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.597694 netbox-config-diff-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19230 2024-02-06 09:10:35.597694 netbox-config-diff-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.577694 netbox-config-diff-2.2.0/development/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/development/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.577694 netbox-config-diff-2.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.577694 netbox-config-diff-2.2.0/docs/media/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.581694 netbox-config-diff-2.2.0/docs/media/screenshots/
--rw-r--r--   0 runner    (1001) docker     (127)    31744 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/compliance-diff.png
--rw-r--r--   0 runner    (1001) docker     (127)    48801 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/compliance-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    23740 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/compliance-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    27108 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/compliance-missing-extra.png
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/compliance-ok.png
--rw-r--r--   0 runner    (1001) docker     (127)     9975 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/config-temp-substitute.png
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/cr-approve-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/cr-approved.png
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/cr-collecting-diff-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    48412 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/cr-completed.png
--rw-r--r--   0 runner    (1001) docker     (127)    42240 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/cr-created.png
--rw-r--r--   0 runner    (1001) docker     (127)    65258 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/cr-diffs-tab.png
--rw-r--r--   0 runner    (1001) docker     (127)    20845 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/cr-job-log.png
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/cr-schedule-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/cr-scheduled.png
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/cr-unapprove-button.png
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/cr-unschedule-button.png
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/navbar.png
--rw-r--r--   0 runner    (1001) docker     (127)    28028 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/platformsetting.png
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/render-temp-substitute.png
--rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/script-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    43979 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/script.png
--rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/docs/media/screenshots/substitute.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.585694 netbox-config-diff-2.2.0/netbox_config_diff/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.585694 netbox-config-diff-2.2.0/netbox_config_diff/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.589694 netbox-config-diff-2.2.0/netbox_config_diff/compliance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/compliance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/compliance/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/compliance/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/compliance/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.589694 netbox-config-diff-2.2.0/netbox_config_diff/configurator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/configurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/configurator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/configurator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/configurator/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/configurator/platforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/configurator/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.589694 netbox-config-diff-2.2.0/netbox_config_diff/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/migrations/0002_add_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/migrations/0004_update_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/migrations/0005_configcompliance_extra_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/migrations/0006_substitute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/migrations/0007_configurationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/migrations/0008_alter_configcompliance_device.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.589694 netbox-config-diff-2.2.0/netbox_config_diff/models/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/models/data_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.589694 netbox-config-diff-2.2.0/netbox_config_diff/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/scripts/config_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.577694 netbox-config-diff-2.2.0/netbox_config_diff/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.593694 netbox-config-diff-2.2.0/netbox_config_diff/static/netbox_config_diff/
--rw-r--r--   0 runner    (1001) docker     (127)  1000358 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/static/netbox_config_diff/diff2html.dark.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/static/netbox_config_diff/diff2html.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.577694 netbox-config-diff-2.2.0/netbox_config_diff/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.593694 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.593694 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/data.html
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/missing_extra.html
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configcompliance.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.593694 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/diffs.html
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.593694 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/inc/diff.html
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/inc/job_log.html
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/platformsetting.html
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/substitute.html
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.593694 netbox-config-diff-2.2.0/netbox_config_diff/views/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/views/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/views/compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12412 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/netbox_config_diff/views/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.597694 netbox-config-diff-2.2.0/netbox_config_diff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19230 2024-02-06 09:10:35.000000 netbox-config-diff-2.2.0/netbox_config_diff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-02-06 09:10:35.000000 netbox-config-diff-2.2.0/netbox_config_diff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 09:10:35.000000 netbox-config-diff-2.2.0/netbox_config_diff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-06 09:10:35.000000 netbox-config-diff-2.2.0/netbox_config_diff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-06 09:10:35.000000 netbox-config-diff-2.2.0/netbox_config_diff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.597694 netbox-config-diff-2.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 09:10:35.597694 netbox-config-diff-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:10:35.597694 netbox-config-diff-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/tests/test_compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/tests/test_compliance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-02-06 09:10:21.000000 netbox-config-diff-2.2.0/tests/test_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19230 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.186831 netbox-config-diff-2.3.0/development/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/development/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.182831 netbox-config-diff-2.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.182831 netbox-config-diff-2.3.0/docs/media/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.190831 netbox-config-diff-2.3.0/docs/media/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (127)    31744 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/compliance-diff.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48801 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/compliance-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23740 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/compliance-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27108 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/compliance-missing-extra.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/compliance-ok.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9975 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/config-temp-substitute.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-approve-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-approved.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-collecting-diff-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48412 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-completed.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42240 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-created.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65258 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-diffs-tab.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20845 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-job-log.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-schedule-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-scheduled.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-unapprove-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-unschedule-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/navbar.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28028 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/platformsetting.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/render-temp-substitute.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/script-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43979 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/script.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/substitute.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.190831 netbox-config-diff-2.3.0/netbox_config_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.194831 netbox-config-diff-2.3.0/netbox_config_diff/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.194831 netbox-config-diff-2.3.0/netbox_config_diff/compliance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/compliance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/compliance/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/compliance/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/compliance/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.194831 netbox-config-diff-2.3.0/netbox_config_diff/configurator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/configurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/configurator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/configurator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/configurator/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/configurator/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/configurator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.198831 netbox-config-diff-2.3.0/netbox_config_diff/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0002_add_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0004_update_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0005_configcompliance_extra_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0006_substitute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0007_configurationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0008_alter_configcompliance_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.198831 netbox-config-diff-2.3.0/netbox_config_diff/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/models/data_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.198831 netbox-config-diff-2.3.0/netbox_config_diff/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/scripts/config_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.182831 netbox-config-diff-2.3.0/netbox_config_diff/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.198831 netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)  1000358 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/diff2html.dark.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/diff2html.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.186831 netbox-config-diff-2.3.0/netbox_config_diff/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.198831 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.198831 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/data.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/missing_extra.html
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/diffs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/inc/diff.html
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/inc/job_log.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/platformsetting.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/substitute.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/netbox_config_diff/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/views/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12412 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/views/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/netbox_config_diff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19230 2024-04-11 13:48:39.000000 netbox-config-diff-2.3.0/netbox_config_diff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-11 13:48:39.000000 netbox-config-diff-2.3.0/netbox_config_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:48:39.000000 netbox-config-diff-2.3.0/netbox_config_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-11 13:48:39.000000 netbox-config-diff-2.3.0/netbox_config_diff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 13:48:39.000000 netbox-config-diff-2.3.0/netbox_config_diff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/tests/test_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/tests/test_compliance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/tests/test_urls.py
```

### Comparing `netbox-config-diff-2.2.0/LICENSE` & `netbox-config-diff-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/PKG-INFO` & `netbox-config-diff-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-config-diff
-Version: 2.2.0
+Version: 2.3.0
 Summary: Push rendered device configurations from NetBox to devices and apply them.
 Author: Artem Kotik
 Author-email: miaow2@yandex.ru
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -271,15 +271,15 @@
 This is possible thanks to the scrapli_cfg. Read [Scrapli](https://github.com/scrapli/scrapli_cfg/) documentation for more info.
 <!--about-end-->
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|    3.5, 3.6    |    =>0.1.0     |
+|  3.5, 3.6, 3.7 |    =>0.1.0     |
 
 <!--install-start-->
 ## Installing
 
 For adding to a NetBox Docker setup see
 [the general instructions for using netbox-docker with plugins](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins).
```

### Comparing `netbox-config-diff-2.2.0/README.md` & `netbox-config-diff-2.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 This is possible thanks to the scrapli_cfg. Read [Scrapli](https://github.com/scrapli/scrapli_cfg/) documentation for more info.
 <!--about-end-->
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|    3.5, 3.6    |    =>0.1.0     |
+|  3.5, 3.6, 3.7 |    =>0.1.0     |
 
 <!--install-start-->
 ## Installing
 
 For adding to a NetBox Docker setup see
 [the general instructions for using netbox-docker with plugins](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins).
```

### Comparing `netbox-config-diff-2.2.0/development/configuration.py` & `netbox-config-diff-2.3.0/development/configuration.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/compliance-diff.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/compliance-diff.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/compliance-error.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/compliance-error.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/compliance-list.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/compliance-list.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/compliance-missing-extra.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/compliance-missing-extra.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/compliance-ok.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/compliance-ok.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/config-temp-substitute.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/config-temp-substitute.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/cr-approve-button.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/cr-approve-button.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/cr-approved.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/cr-approved.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/cr-collecting-diff-button.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/cr-collecting-diff-button.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/cr-completed.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/cr-completed.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/cr-created.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/cr-created.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/cr-diffs-tab.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/cr-diffs-tab.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/cr-job-log.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/cr-job-log.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/cr-schedule-button.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/cr-schedule-button.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/cr-scheduled.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/cr-scheduled.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/cr-unapprove-button.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/cr-unapprove-button.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/cr-unschedule-button.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/cr-unschedule-button.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/navbar.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/navbar.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/platformsetting.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/platformsetting.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/render-temp-substitute.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/render-temp-substitute.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/script-list.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/script-list.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/script.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/script.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/docs/media/screenshots/substitute.png` & `netbox-config-diff-2.3.0/docs/media/screenshots/substitute.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/__init__.py` & `netbox-config-diff-2.3.0/netbox_config_diff/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from extras.plugins import PluginConfig
 
 __author__ = "Artem Kotik"
 __email__ = "miaow2@yandex.ru"
-__version__ = "2.2.0"
+__version__ = "2.3.0"
 
 
 class ConfigDiffConfig(PluginConfig):
     name = "netbox_config_diff"
     verbose_name = "NetBox Config Diff Plugin"
     description = "Find diff between the intended device configuration and actual."
     author = __author__
```

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/api/serializers.py` & `netbox-config-diff-2.3.0/netbox_config_diff/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/api/views.py` & `netbox-config-diff-2.3.0/netbox_config_diff/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/choices.py` & `netbox-config-diff-2.3.0/netbox_config_diff/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/compliance/base.py` & `netbox-config-diff-2.3.0/netbox_config_diff/compliance/base.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/compliance/secrets.py` & `netbox-config-diff-2.3.0/netbox_config_diff/compliance/secrets.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/compliance/utils.py` & `netbox-config-diff-2.3.0/netbox_config_diff/compliance/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     def __init__(self, choices, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.field_attrs["choices"] = choices
 
 
 def get_unified_diff(rendered_config: str, actual_config: str, device: str) -> str:
     diff = unified_diff(
-        rendered_config.strip().splitlines(),
         actual_config.splitlines(),
+        rendered_config.strip().splitlines(),
         fromfiledate=device,
         tofiledate=device,
         lineterm="",
     )
     return "\n".join(diff).strip()
```

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/configurator/base.py` & `netbox-config-diff-2.3.0/netbox_config_diff/configurator/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             conn = self.connections[device.name]
             if substitutes := self.substitutes.get(device.platform):
                 actual_config, rendered_config = await conn.render_substituted_config(
                     config_template=device.rendered_config, substitutes=substitutes
                 )
                 device.rendered_config = rendered_config
             else:
-                actual_config = await conn.get_config()
+                actual_config = await conn.get_config(config_template=device.rendered_config)
             device.actual_config = conn.clean_config(actual_config.result)
 
             device.diff = get_unified_diff(device.rendered_config, device.actual_config, device.name)
             self.logger.add_diff(device.name, diff=device.diff)
             device.missing = diff_network_config(
                 device.rendered_config, device.actual_config, PLATFORM_MAPPING[device.platform]
             )
```

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/configurator/factory.py` & `netbox-config-diff-2.3.0/netbox_config_diff/configurator/factory.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/configurator/platforms.py` & `netbox-config-diff-2.3.0/netbox_config_diff/configurator/platforms.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Pattern
+from typing import Any, Pattern
 
 from scrapli_cfg.exceptions import TemplateError
 from scrapli_cfg.platform.core.arista_eos import AsyncScrapliCfgEOS
 from scrapli_cfg.platform.core.cisco_iosxe import AsyncScrapliCfgIOSXE
 from scrapli_cfg.platform.core.cisco_iosxr import AsyncScrapliCfgIOSXR
 from scrapli_cfg.platform.core.cisco_nxos import AsyncScrapliCfgNXOS
 from scrapli_cfg.platform.core.juniper_junos import AsyncScrapliCfgJunos
@@ -90,21 +90,25 @@
 
         Raises:
             N/A
 
         """
         self.logger.info("fetching configuration and replacing with provided substitutes")
 
-        source_config = await self.get_config(source=source)
+        source_config = await self.get_config(config_template=config_template, source=source)
         return source_config, self._render_substituted_config(
             config_template=config_template,
             substitutes=substitutes,
             source_config=source_config.result,
         )
 
+    async def get_config(self, **kwargs) -> ScrapliCfgResponse:
+        kwargs.pop("config_template", None)
+        return await super().get_config(**kwargs)
+
 
 class CustomAsyncScrapliCfgEOS(CustomScrapliCfg, AsyncScrapliCfgEOS):
     pass
 
 
 class CustomAsyncScrapliCfgIOSXE(CustomScrapliCfg, AsyncScrapliCfgIOSXE):
     pass
@@ -115,8 +119,71 @@
 
 
 class CustomAsyncScrapliCfgNXOS(CustomScrapliCfg, AsyncScrapliCfgNXOS):
     pass
 
 
 class CustomAsyncScrapliCfgJunos(CustomScrapliCfg, AsyncScrapliCfgJunos):
-    pass
+    is_set_config = False
+
+    async def get_config(self, config_template: str, source: str = "running") -> ScrapliCfgResponse:
+        response = self._pre_get_config(source=source)
+
+        command = "show configuration"
+        if re.findall(r"^set\s+", config_template, flags=re.I | re.M):
+            self.is_set_config = True
+            command += " | display set"
+
+        if self._in_configuration_session is True:
+            config_result = await self.conn.send_config(config=f"run {command}")
+        else:
+            config_result = await self.conn.send_command(command=command)
+
+        return self._post_get_config(
+            response=response,
+            source=source,
+            scrapli_responses=[config_result],
+            result=config_result.result,
+        )
+
+    async def load_config(self, config: str, replace: bool = False, **kwargs: Any) -> ScrapliCfgResponse:
+        """
+        Load configuration to a device
+
+        Supported kwargs:
+            set: bool indicating config is a "set" style config (ignored if replace is True)
+
+        Args:
+            config: string of the configuration to load
+            replace: replace the configuration or not, if false configuration will be loaded as a
+                merge operation
+            kwargs: additional kwargs that the implementing classes may need for their platform,
+                see above for junos supported kwargs
+
+        Returns:
+            ScrapliCfgResponse: response object
+
+        Raises:
+            N/A
+
+        """
+        response = self._pre_load_config(config=config)
+
+        config = self._prepare_load_config(config=config, replace=replace)
+
+        config_result = await self.conn.send_config(config=config, privilege_level="root_shell")
+
+        if self.is_set_config is True:
+            load_config = f"load set {self.filesystem}{self.candidate_config_filename}"
+        else:
+            if self._replace is True:
+                load_config = f"load override {self.filesystem}{self.candidate_config_filename}"
+            else:
+                load_config = f"load merge {self.filesystem}{self.candidate_config_filename}"
+
+        load_result = await self.conn.send_config(config=load_config)
+        self._in_configuration_session = True
+
+        return self._post_load_config(
+            response=response,
+            scrapli_responses=[config_result, load_result],
+        )
```

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/configurator/utils.py` & `netbox-config-diff-2.3.0/netbox_config_diff/configurator/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/filtersets.py` & `netbox-config-diff-2.3.0/netbox_config_diff/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/forms.py` & `netbox-config-diff-2.3.0/netbox_config_diff/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/graphql.py` & `netbox-config-diff-2.3.0/netbox_config_diff/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/jobs.py` & `netbox-config-diff-2.3.0/netbox_config_diff/jobs.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/migrations/0001_initial.py` & `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/migrations/0002_add_script.py` & `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0002_add_script.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py` & `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/migrations/0004_update_script.py` & `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0004_update_script.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/migrations/0006_substitute.py` & `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0006_substitute.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/migrations/0007_configurationrequest.py` & `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0007_configurationrequest.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/migrations/0008_alter_configcompliance_device.py` & `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0008_alter_configcompliance_device.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/models/data_models.py` & `netbox-config-diff-2.3.0/netbox_config_diff/models/data_models.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/models/models.py` & `netbox-config-diff-2.3.0/netbox_config_diff/models/models.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/navigation.py` & `netbox-config-diff-2.3.0/netbox_config_diff/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/search.py` & `netbox-config-diff-2.3.0/netbox_config_diff/search.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js` & `netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/static/netbox_config_diff/diff2html.dark.min.css` & `netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/diff2html.dark.min.css`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/static/netbox_config_diff/diff2html.min.css` & `netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/diff2html.min.css`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/tables.py` & `netbox-config-diff-2.3.0/netbox_config_diff/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html` & `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/data.html` & `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/data.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/missing_extra.html` & `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/missing_extra.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/base.html` & `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/base.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/diffs.html` & `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/diffs.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest.html` & `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/inc/diff.html` & `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/inc/diff.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/inc/job_log.html` & `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/inc/job_log.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/platformsetting.html` & `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/platformsetting.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/templates/netbox_config_diff/substitute.html` & `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/substitute.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/urls.py` & `netbox-config-diff-2.3.0/netbox_config_diff/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/views/__init__.py` & `netbox-config-diff-2.3.0/netbox_config_diff/views/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/views/compliance.py` & `netbox-config-diff-2.3.0/netbox_config_diff/views/compliance.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff/views/configuration.py` & `netbox-config-diff-2.3.0/netbox_config_diff/views/configuration.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff.egg-info/PKG-INFO` & `netbox-config-diff-2.3.0/netbox_config_diff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-config-diff
-Version: 2.2.0
+Version: 2.3.0
 Summary: Push rendered device configurations from NetBox to devices and apply them.
 Author: Artem Kotik
 Author-email: miaow2@yandex.ru
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -271,15 +271,15 @@
 This is possible thanks to the scrapli_cfg. Read [Scrapli](https://github.com/scrapli/scrapli_cfg/) documentation for more info.
 <!--about-end-->
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|    3.5, 3.6    |    =>0.1.0     |
+|  3.5, 3.6, 3.7 |    =>0.1.0     |
 
 <!--install-start-->
 ## Installing
 
 For adding to a NetBox Docker setup see
 [the general instructions for using netbox-docker with plugins](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins).
```

### Comparing `netbox-config-diff-2.2.0/netbox_config_diff.egg-info/SOURCES.txt` & `netbox-config-diff-2.3.0/netbox_config_diff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/pyproject.toml` & `netbox-config-diff-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/tests/conftest.py` & `netbox-config-diff-2.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/tests/factories.py` & `netbox-config-diff-2.3.0/tests/factories.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/tests/test_compliance.py` & `netbox-config-diff-2.3.0/tests/test_compliance.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.2.0/tests/test_compliance_utils.py` & `netbox-config-diff-2.3.0/tests/test_compliance_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,8 +52,8 @@
             RENDERED_CONFIG,
             "",
         ),
     ],
     ids=["diff", "no diff"],
 )
 def test_get_unified_diff(render: str, actual: str, expected: str) -> None:
-    assert get_unified_diff(render, actual, "test-1") == expected
+    assert get_unified_diff(actual, render, "test-1") == expected
```

### Comparing `netbox-config-diff-2.2.0/tests/test_urls.py` & `netbox-config-diff-2.3.0/tests/test_urls.py`

 * *Files identical despite different names*

