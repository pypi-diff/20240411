# Comparing `tmp/mvt-2.5.0.tar.gz` & `tmp/mvt-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvt-2.5.0.tar", last modified: Thu Jan  4 19:12:58 2024, max compression
+gzip compressed data, was "mvt-2.5.1.tar", last modified: Thu Apr 11 09:21:30 2024, max compression
```

## Comparing `mvt-2.5.0.tar` & `mvt-2.5.1.tar`

### file list

```diff
@@ -1,230 +1,231 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.261661 mvt-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-01-04 19:12:48.000000 mvt-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-01-04 19:12:58.261661 mvt-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-01-04 19:12:48.000000 mvt-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.229661 mvt-2.5.0/mvt/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.229661 mvt-2.5.0/mvt/android/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.233661 mvt-2.5.0/mvt/android/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/artifacts/dumpsys_accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/artifacts/dumpsys_appops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/artifacts/dumpsys_battery_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/artifacts/dumpsys_battery_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/artifacts/dumpsys_dbinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/artifacts/dumpsys_package_activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/artifacts/dumpsys_receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/artifacts/getprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/artifacts/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/artifacts/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/cmd_check_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/cmd_check_androidqf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/cmd_check_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/cmd_check_bugreport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/cmd_download_apks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.233661 mvt-2.5.0/mvt/android/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.237661 mvt-2.5.0/mvt/android/modules/adb/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/chrome_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/dumpsys_accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/dumpsys_activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/dumpsys_appops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/dumpsys_battery_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/dumpsys_battery_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/dumpsys_dbinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/dumpsys_full.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/dumpsys_receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/getprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/logcat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/root_binaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/selinux_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/adb/whatsapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.237661 mvt-2.5.0/mvt/android/modules/androidqf/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_appops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_battery_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_battery_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_dbinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/getprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/androidqf/sms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.237661 mvt-2.5.0/mvt/android/modules/backup/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/backup/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/backup/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/backup/sms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.241661 mvt-2.5.0/mvt/android/modules/bugreport/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/bugreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/bugreport/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/bugreport/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/bugreport/appops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/bugreport/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/bugreport/battery_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/bugreport/battery_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/bugreport/dbinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/bugreport/getprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/bugreport/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/modules/bugreport/receivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.241661 mvt-2.5.0/mvt/android/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/parsers/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/parsers/dumpsys.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/android/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.241661 mvt-2.5.0/mvt/common/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/cmd_check_iocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/help.py
--rw-r--r--   0 runner    (1001) docker     (127)    22957 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/common/virustotal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.245661 mvt-2.5.0/mvt/ios/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/cmd_check_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/cmd_check_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.245661 mvt-2.5.0/mvt/ios/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/data/ios_models.json
--rw-r--r--   0 runner    (1001) docker     (127)    16891 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/data/ios_versions.json
--rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/decrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.245661 mvt-2.5.0/mvt/ios/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.245661 mvt-2.5.0/mvt/ios/modules/backup/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/backup/backup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/backup/configuration_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/backup/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/backup/profile_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.249661 mvt-2.5.0/mvt/ios/modules/fs/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/fs/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/fs/analytics_ios_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/fs/cache_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/fs/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/fs/net_netusage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/fs/safari_favicon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/fs/shutdownlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/fs/version_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/fs/webkit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/fs/webkit_indexeddb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/fs/webkit_localstorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/fs/webkit_safariviewservice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.249661 mvt-2.5.0/mvt/ios/modules/mixed/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/chrome_favicon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/chrome_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/firefox_favicon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/firefox_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/global_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/idstatuscache.py
--rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/interactionc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/locationd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/net_datausage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/osanalytics_addaily.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/safari_browserstate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/safari_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/sms_attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/tcc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/webkit_session_resource_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/mixed/whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/modules/net_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-01-04 19:12:48.000000 mvt-2.5.0/mvt/ios/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.261661 mvt-2.5.0/mvt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-01-04 19:12:58.000000 mvt-2.5.0/mvt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-01-04 19:12:58.000000 mvt-2.5.0/mvt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 19:12:58.000000 mvt-2.5.0/mvt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-04 19:12:58.000000 mvt-2.5.0/mvt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-04 19:12:58.000000 mvt-2.5.0/mvt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-04 19:12:58.000000 mvt-2.5.0/mvt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-01-04 19:12:58.261661 mvt-2.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-01-04 19:12:48.000000 mvt-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.261661 mvt-2.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.253661 mvt-2.5.0/tests/android/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android/test_artifact_dumpsys_accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android/test_artifact_dumpsys_appops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android/test_artifact_dumpsys_battery_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android/test_artifact_dumpsys_battery_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android/test_artifact_dumpsys_dbinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android/test_artifact_dumpsys_package_activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android/test_artifact_dumpsys_receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android/test_artifact_getprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android/test_artifact_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android/test_backup_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android/test_backup_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.253661 mvt-2.5.0/tests/android_adb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_adb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.257661 mvt-2.5.0/tests/android_androidqf/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_androidqf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_androidqf/test_dumpsys_battery_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_androidqf/test_dumpsys_battery_history.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_androidqf/test_dumpsys_dbinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_androidqf/test_dumpsysaccessbility.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_androidqf/test_dumpsysappops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_androidqf/test_dumpsyspackages.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_androidqf/test_dumpsysreceivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_androidqf/test_getprop.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_androidqf/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_androidqf/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_androidqf/test_sms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.257661 mvt-2.5.0/tests/android_bugreport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_bugreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/android_bugreport/test_bugreport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.257661 mvt-2.5.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/common/test_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/common/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.257661 mvt-2.5.0/tests/ios_backup/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/ios_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/ios_backup/test_backup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/ios_backup/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/ios_backup/test_datausage.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/ios_backup/test_global_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/ios_backup/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/ios_backup/test_safari_browserstate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/ios_backup/test_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/ios_backup/test_tcc.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/ios_backup/test_webkit_resource_load_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:12:58.257661 mvt-2.5.0/tests/ios_fs/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/ios_fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/ios_fs/test_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/test_check_android_androidqf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/test_check_android_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/test_check_android_bugreport.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/test_check_ios_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/test_ios_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-01-04 19:12:48.000000 mvt-2.5.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.102443 mvt-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-04-11 09:21:26.000000 mvt-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-11 09:21:30.102443 mvt-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-11 09:21:26.000000 mvt-2.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.062443 mvt-2.5.1/mvt/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.062443 mvt-2.5.1/mvt/android/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.066443 mvt-2.5.1/mvt/android/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_appops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_battery_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_battery_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_dbinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_package_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/getprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/cmd_check_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/cmd_check_androidqf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/cmd_check_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/cmd_check_bugreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/cmd_download_apks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.066443 mvt-2.5.1/mvt/android/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.070443 mvt-2.5.1/mvt/android/modules/adb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/chrome_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_appops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_battery_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_battery_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_dbinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_full.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/getprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/logcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/root_binaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/selinux_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/whatsapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.074443 mvt-2.5.1/mvt/android/modules/androidqf/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_appops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_battery_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_battery_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_dbinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/getprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/sms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.074443 mvt-2.5.1/mvt/android/modules/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/backup/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/backup/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/backup/sms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.078443 mvt-2.5.1/mvt/android/modules/bugreport/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/appops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/battery_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/battery_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/dbinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/getprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/receivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.078443 mvt-2.5.1/mvt/android/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/parsers/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.082443 mvt-2.5.1/mvt/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/cmd_check_iocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22957 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/virustotal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.082443 mvt-2.5.1/mvt/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/cmd_check_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/cmd_check_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.082443 mvt-2.5.1/mvt/ios/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/data/ios_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17565 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/data/ios_versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/decrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.082443 mvt-2.5.1/mvt/ios/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.082443 mvt-2.5.1/mvt/ios/modules/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/backup/backup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/backup/configuration_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/backup/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/backup/profile_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.086443 mvt-2.5.1/mvt/ios/modules/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/analytics_ios_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/cache_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/net_netusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/safari_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/shutdownlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/version_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/webkit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/webkit_indexeddb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/webkit_localstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/webkit_safariviewservice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.090443 mvt-2.5.1/mvt/ios/modules/mixed/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/chrome_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/chrome_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/firefox_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/firefox_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/global_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/idstatuscache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/interactionc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/locationd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/net_datausage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/osanalytics_addaily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/safari_browserstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/safari_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/sms_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/tcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/webkit_session_resource_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/net_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.102443 mvt-2.5.1/mvt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-11 09:21:30.000000 mvt-2.5.1/mvt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-04-11 09:21:30.000000 mvt-2.5.1/mvt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:21:30.000000 mvt-2.5.1/mvt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 09:21:30.000000 mvt-2.5.1/mvt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 09:21:30.000000 mvt-2.5.1/mvt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 09:21:30.000000 mvt-2.5.1/mvt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-11 09:21:30.106443 mvt-2.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-04-11 09:21:26.000000 mvt-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.102443 mvt-2.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.094443 mvt-2.5.1/tests/android/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_appops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_battery_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_battery_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_dbinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_package_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_getprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_backup_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_backup_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.094443 mvt-2.5.1/tests/android_adb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_adb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.098443 mvt-2.5.1/tests/android_androidqf/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsys_battery_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsys_battery_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsys_dbinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsysaccessbility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsysappops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsyspackages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsysreceivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_getprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_sms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.098443 mvt-2.5.1/tests/android_bugreport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_bugreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_bugreport/test_bugreport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.098443 mvt-2.5.1/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/common/test_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/common/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.102443 mvt-2.5.1/tests/ios_backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_backup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_datausage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_global_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_safari_browserstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_tcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_webkit_resource_load_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.102443 mvt-2.5.1/tests/ios_fs/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_fs/test_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/test_check_android_androidqf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/test_check_android_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/test_check_android_bugreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/test_check_ios_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/test_ios_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/utils.py
```

### Comparing `mvt-2.5.0/LICENSE` & `mvt-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/PKG-INFO` & `mvt-2.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvt
-Version: 2.5.0
+Version: 2.5.1
 Summary: Mobile Verification Toolkit
 Home-page: https://github.com/mvt-project/mvt
 Author: Claudio Guarnieri
 Author-email: nex@nex.sx
 License: MVT v1.1
 Keywords: security,mobile,forensics,malware
 Classifier: Development Status :: 5 - Production/Stable
@@ -52,15 +52,15 @@
 MVT supports using public [indicators of compromise (IOCs)](https://github.com/mvt-project/mvt-indicators) to scan mobile devices for potential traces of targeting or infection by known spyware campaigns. This includes IOCs published by [Amnesty International](https://github.com/AmnestyTech/investigations/) and other  research groups.
 
 > **Warning**
 > Public indicators of compromise are insufficient to determine that a device is "clean", and not targeted with a particular spyware tool. Reliance on public indicators alone can miss recent forensic traces and give a false sense of security.
 >
 > Reliable and comprehensive digital forensic support and triage requires access to non-public indicators, research and threat intelligence.
 >
->Such support is available to civil society through [Amnesty International's Security Lab](https://www.amnesty.org/en/tech/) or through our forensic partnership with [Access Now’s Digital Security Helpline](https://www.accessnow.org/help/).
+>Such support is available to civil society through [Amnesty International's Security Lab](https://securitylab.amnesty.org/get-help/?c=mvt_docs) or through our forensic partnership with [Access Now’s Digital Security Helpline](https://www.accessnow.org/help/).
 
 More information about using indicators of compromise with MVT is available in the [documentation](https://docs.mvt.re/en/latest/iocs/).
 
 ## Installation
 
 MVT can be installed from sources or from [PyPI](https://pypi.org/project/mvt/) (you will need some dependencies, check the [documentation](https://docs.mvt.re/en/latest/install/)):
```

### Comparing `mvt-2.5.0/README.md` & `mvt-2.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 MVT supports using public [indicators of compromise (IOCs)](https://github.com/mvt-project/mvt-indicators) to scan mobile devices for potential traces of targeting or infection by known spyware campaigns. This includes IOCs published by [Amnesty International](https://github.com/AmnestyTech/investigations/) and other  research groups.
 
 > **Warning**
 > Public indicators of compromise are insufficient to determine that a device is "clean", and not targeted with a particular spyware tool. Reliance on public indicators alone can miss recent forensic traces and give a false sense of security.
 >
 > Reliable and comprehensive digital forensic support and triage requires access to non-public indicators, research and threat intelligence.
 >
->Such support is available to civil society through [Amnesty International's Security Lab](https://www.amnesty.org/en/tech/) or through our forensic partnership with [Access Now’s Digital Security Helpline](https://www.accessnow.org/help/).
+>Such support is available to civil society through [Amnesty International's Security Lab](https://securitylab.amnesty.org/get-help/?c=mvt_docs) or through our forensic partnership with [Access Now’s Digital Security Helpline](https://www.accessnow.org/help/).
 
 More information about using indicators of compromise with MVT is available in the [documentation](https://docs.mvt.re/en/latest/iocs/).
 
 ## Installation
 
 MVT can be installed from sources or from [PyPI](https://pypi.org/project/mvt/) (you will need some dependencies, check the [documentation](https://docs.mvt.re/en/latest/install/)):
```

### Comparing `mvt-2.5.0/mvt/android/artifacts/artifact.py` & `mvt-2.5.1/mvt/android/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/artifacts/dumpsys_accessibility.py` & `mvt-2.5.1/mvt/android/artifacts/dumpsys_accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/artifacts/dumpsys_appops.py` & `mvt-2.5.1/mvt/android/artifacts/dumpsys_appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/artifacts/dumpsys_battery_daily.py` & `mvt-2.5.1/mvt/android/artifacts/dumpsys_battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/artifacts/dumpsys_battery_history.py` & `mvt-2.5.1/mvt/android/artifacts/dumpsys_battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/artifacts/dumpsys_dbinfo.py` & `mvt-2.5.1/mvt/android/artifacts/dumpsys_dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/artifacts/dumpsys_package_activities.py` & `mvt-2.5.1/mvt/android/artifacts/dumpsys_package_activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/artifacts/dumpsys_receivers.py` & `mvt-2.5.1/mvt/android/artifacts/dumpsys_receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/artifacts/getprop.py` & `mvt-2.5.1/mvt/android/artifacts/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/artifacts/processes.py` & `mvt-2.5.1/mvt/android/artifacts/processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/artifacts/settings.py` & `mvt-2.5.1/mvt/android/artifacts/settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/cli.py` & `mvt-2.5.1/mvt/android/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 @click.option("--serial", "-s", type=str, help=HELP_MSG_SERIAL)
 @click.option(
     "--all-apks",
     "-a",
     is_flag=True,
     help="Extract all packages installed on the phone, including system packages",
 )
-@click.option("--virustotal", "-v", is_flag=True, help="Check packages on VirusTotal")
+@click.option("--virustotal", "-V", is_flag=True, help="Check packages on VirusTotal")
 @click.option(
     "--output",
     "-o",
     type=click.Path(exists=False),
     help="Specify a path to a folder where you want to store the APKs",
 )
 @click.option(
```

### Comparing `mvt-2.5.0/mvt/android/cmd_check_adb.py` & `mvt-2.5.1/mvt/android/cmd_check_adb.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/cmd_check_androidqf.py` & `mvt-2.5.1/mvt/android/cmd_check_androidqf.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/cmd_check_backup.py` & `mvt-2.5.1/mvt/android/cmd_check_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/cmd_check_bugreport.py` & `mvt-2.5.1/mvt/android/cmd_check_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/cmd_download_apks.py` & `mvt-2.5.1/mvt/android/cmd_download_apks.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/__init__.py` & `mvt-2.5.1/mvt/android/modules/adb/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/base.py` & `mvt-2.5.1/mvt/android/modules/adb/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/chrome_history.py` & `mvt-2.5.1/mvt/android/modules/adb/chrome_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/dumpsys_accessibility.py` & `mvt-2.5.1/mvt/android/modules/adb/dumpsys_accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/dumpsys_activities.py` & `mvt-2.5.1/mvt/android/modules/adb/dumpsys_activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/dumpsys_appops.py` & `mvt-2.5.1/mvt/android/modules/adb/dumpsys_appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/dumpsys_battery_daily.py` & `mvt-2.5.1/mvt/android/modules/adb/dumpsys_battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/dumpsys_battery_history.py` & `mvt-2.5.1/mvt/android/modules/adb/dumpsys_battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/dumpsys_dbinfo.py` & `mvt-2.5.1/mvt/android/modules/adb/dumpsys_dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/dumpsys_full.py` & `mvt-2.5.1/mvt/android/modules/adb/dumpsys_full.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/dumpsys_receivers.py` & `mvt-2.5.1/mvt/android/modules/adb/dumpsys_receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/files.py` & `mvt-2.5.1/mvt/android/modules/adb/files.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/getprop.py` & `mvt-2.5.1/mvt/android/modules/adb/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/logcat.py` & `mvt-2.5.1/mvt/android/modules/adb/logcat.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/processes.py` & `mvt-2.5.1/mvt/android/modules/adb/processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/root_binaries.py` & `mvt-2.5.1/mvt/android/modules/adb/root_binaries.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/selinux_status.py` & `mvt-2.5.1/mvt/android/modules/adb/selinux_status.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/settings.py` & `mvt-2.5.1/mvt/android/modules/adb/settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/sms.py` & `mvt-2.5.1/mvt/android/modules/adb/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/adb/whatsapp.py` & `mvt-2.5.1/mvt/android/modules/adb/whatsapp.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/__init__.py` & `mvt-2.5.1/mvt/android/modules/androidqf/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/base.py` & `mvt-2.5.1/mvt/android/modules/androidqf/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_accessibility.py` & `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_activities.py` & `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_appops.py` & `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_battery_daily.py` & `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_battery_history.py` & `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_dbinfo.py` & `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_packages.py` & `mvt-2.5.1/mvt/ios/modules/mixed/idstatuscache.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,118 +1,122 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 The MVT Authors.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
+import collections
 import logging
-from typing import Any, Dict, List, Optional, Union
+import plistlib
+from typing import Optional, Union
 
-from mvt.android.modules.adb.packages import (
-    DANGEROUS_PERMISSIONS,
-    DANGEROUS_PERMISSIONS_THRESHOLD,
-    ROOT_PACKAGES,
-)
-from mvt.android.parsers.dumpsys import parse_dumpsys_packages
+from mvt.common.utils import convert_mactime_to_iso
 
-from .base import AndroidQFModule
+from ..base import IOSExtraction
 
+IDSTATUSCACHE_BACKUP_IDS = [
+    "6b97989189901ceaa4e5be9b7f05fb584120e27b",
+]
+IDSTATUSCACHE_ROOT_PATHS = [
+    "private/var/mobile/Library/Preferences/com.apple.identityservices.idstatuscache.plist",
+    "private/var/mobile/Library/IdentityServices/idstatuscache.plist",
+]
 
-class DumpsysPackages(AndroidQFModule):
-    """This module analyse dumpsys packages"""
+
+class IDStatusCache(IOSExtraction):
+    """Extracts Apple Authentication information from idstatuscache.plist"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[List[Dict[str, Any]]] = None,
+        results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
             module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
-        entries = []
-        for entry in ["timestamp", "first_install_time", "last_update_time"]:
-            if entry in record:
-                entries.append(
-                    {
-                        "timestamp": record[entry],
-                        "module": self.__class__.__name__,
-                        "event": entry,
-                        "data": f"Package {record['package_name']} "
-                        f"({record['uid']})",
-                    }
-                )
-
-        return entries
+        return {
+            "timestamp": record["isodate"],
+            "module": self.__class__.__name__,
+            "event": "lookup",
+            "data": f"Lookup of {record['user']} within {record['package']} "
+            f"(Status {record['idstatus']})",
+        }
 
     def check_indicators(self) -> None:
+        if not self.indicators:
+            return
+
         for result in self.results:
-            if result["package_name"] in ROOT_PACKAGES:
+            if result.get("user", "").startswith("mailto:"):
+                email = result["user"][7:].strip("'")
+                ioc = self.indicators.check_email(email)
+                if ioc:
+                    result["matched_indicator"] = ioc
+                    self.detected.append(result)
+                    continue
+
+            if "\\x00\\x00" in result.get("user", ""):
                 self.log.warning(
-                    "Found an installed package related to "
-                    'rooting/jailbreaking: "%s"',
-                    result["package_name"],
+                    "Found an ID Status Cache entry with suspicious patterns: %s",
+                    result.get("user"),
                 )
                 self.detected.append(result)
-                continue
 
-            if not self.indicators:
+    def _extract_idstatuscache_entries(self, file_path):
+        with open(file_path, "rb") as handle:
+            file_plist = plistlib.load(handle)
+
+        id_status_cache_entries = []
+        for app in file_plist:
+            if not isinstance(file_plist[app], dict):
                 continue
 
-            ioc = self.indicators.check_app_id(result.get("package_name", ""))
-            if ioc:
-                result["matched_indicator"] = ioc
-                self.detected.append(result)
+            for entry in file_plist[app]:
+                try:
+                    lookup_date = file_plist[app][entry]["LookupDate"]
+                    id_status = file_plist[app][entry]["IDStatus"]
+                except KeyError:
+                    continue
 
-    def run(self) -> None:
-        dumpsys_file = self._get_files_by_pattern("*/dumpsys.txt")
-        if len(dumpsys_file) != 1:
-            self.log.info("Dumpsys file not found")
-            return
-
-        data = self._get_file_content(dumpsys_file[0])
-
-        package = []
-        in_service = False
-        in_package_list = False
-        for line in data.decode("utf-8").split("\n"):
-            if line.strip().startswith("DUMP OF SERVICE package:"):
-                in_service = True
-                continue
-
-            if in_service and line.startswith("Packages:"):
-                in_package_list = True
-                continue
-
-            if not in_service or not in_package_list:
-                continue
-
-            if line.strip() == "":
-                break
-
-            package.append(line)
+                id_status_cache_entries.append(
+                    {
+                        "package": app,
+                        "user": entry.replace("\x00", "\\x00"),
+                        "isodate": convert_mactime_to_iso(lookup_date),
+                        "idstatus": id_status,
+                    }
+                )
 
-        self.results = parse_dumpsys_packages("\n".join(package))
+        entry_counter = collections.Counter(
+            [entry["user"] for entry in id_status_cache_entries]
+        )
+        for entry in id_status_cache_entries:
+            # Add total count of occurrences to the status cache entry.
+            entry["occurrences"] = entry_counter[entry["user"]]
+            self.results.append(entry)
 
-        for result in self.results:
-            dangerous_permissions_count = 0
-            for perm in result["permissions"]:
-                if perm["name"] in DANGEROUS_PERMISSIONS:
-                    dangerous_permissions_count += 1
-
-            if dangerous_permissions_count >= DANGEROUS_PERMISSIONS_THRESHOLD:
-                self.log.info(
-                    'Found package "%s" requested %d potentially dangerous permissions',
-                    result["package_name"],
-                    dangerous_permissions_count,
-                )
+    def run(self) -> None:
+        if self.is_backup:
+            self._find_ios_database(backup_ids=IDSTATUSCACHE_BACKUP_IDS)
+            self.log.info("Found IDStatusCache plist at path: %s", self.file_path)
+            self._extract_idstatuscache_entries(self.file_path)
+        elif self.is_fs_dump:
+            for idstatuscache_path in self._get_fs_files_from_patterns(
+                IDSTATUSCACHE_ROOT_PATHS
+            ):
+                self.file_path = idstatuscache_path
+                self.log.info("Found IDStatusCache plist at path: %s", self.file_path)
+                self._extract_idstatuscache_entries(self.file_path)
 
-        self.log.info("Extracted details on %d packages", len(self.results))
+        self.log.info(
+            "Extracted a total of %d ID Status Cache entries", len(self.results)
+        )
```

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/dumpsys_receivers.py` & `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/getprop.py` & `mvt-2.5.1/mvt/android/modules/androidqf/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/processes.py` & `mvt-2.5.1/mvt/android/modules/androidqf/processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/settings.py` & `mvt-2.5.1/mvt/android/modules/androidqf/settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/androidqf/sms.py` & `mvt-2.5.1/mvt/android/modules/androidqf/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/backup/base.py` & `mvt-2.5.1/mvt/android/modules/backup/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/backup/helpers.py` & `mvt-2.5.1/mvt/android/modules/backup/helpers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/backup/sms.py` & `mvt-2.5.1/mvt/android/modules/backup/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/bugreport/__init__.py` & `mvt-2.5.1/mvt/android/modules/bugreport/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/bugreport/accessibility.py` & `mvt-2.5.1/mvt/android/modules/bugreport/accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/bugreport/activities.py` & `mvt-2.5.1/mvt/android/modules/bugreport/activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/bugreport/appops.py` & `mvt-2.5.1/mvt/android/modules/bugreport/appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/bugreport/base.py` & `mvt-2.5.1/mvt/android/modules/bugreport/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/bugreport/battery_daily.py` & `mvt-2.5.1/mvt/android/modules/bugreport/battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/bugreport/battery_history.py` & `mvt-2.5.1/mvt/android/modules/bugreport/battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/bugreport/dbinfo.py` & `mvt-2.5.1/mvt/android/modules/bugreport/dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/bugreport/getprop.py` & `mvt-2.5.1/mvt/android/modules/bugreport/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/modules/bugreport/receivers.py` & `mvt-2.5.1/mvt/android/modules/bugreport/receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/android/parsers/backup.py` & `mvt-2.5.1/mvt/android/parsers/backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/common/artifact.py` & `mvt-2.5.1/mvt/common/artifact.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/common/cmd_check_iocs.py` & `mvt-2.5.1/mvt/common/cmd_check_iocs.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/common/command.py` & `mvt-2.5.1/mvt/common/command.py`

 * *Files 21% similar despite different names*

```diff
@@ -156,14 +156,35 @@
 
     def module_init(self, module: MVTModule) -> None:
         raise NotImplementedError
 
     def finish(self) -> None:
         raise NotImplementedError
 
+    def _show_disable_adb_warning(self) -> None:
+        """Warn if ADB is enabled"""
+        if type(self).__name__ in ["CmdAndroidCheckADB", "CmdAndroidCheckAndroidQF"]:
+            self.log.info(
+                "Please disable Developer Options and ADB (Android Debug Bridge) on the device once finished with the acquisition. "
+                "ADB is a powerful tool which can allow unauthorized access to the device."
+            )
+
+    def _show_support_message(self) -> None:
+        support_message = "Please seek reputable expert help if you have serious concerns about a possible spyware attack. Such support is available to human rights defenders and civil society through Amnesty International's Security Lab at https://securitylab.amnesty.org/get-help/?c=mvt"
+        if self.detected_count == 0:
+            self.log.info(
+                f"[bold]NOTE:[/bold] Using MVT with public indicators of compromise (IOCs) [bold]WILL NOT[/bold] automatically detect advanced attacks.\n\n{support_message}",
+                extra={"markup": True},
+            )
+        else:
+            self.log.warning(
+                f"[bold]NOTE: Detected indicators of compromise[/bold]. Only expert review can confirm if the detected indicators are signs of an attack.\n\n{support_message}",
+                extra={"markup": True},
+            )
+
     def run(self) -> None:
         try:
             self.init()
         except NotImplementedError:
             pass
 
         for module in self.modules:
@@ -204,7 +225,10 @@
         try:
             self.finish()
         except NotImplementedError:
             pass
 
         self._store_timeline()
         self._store_info()
+
+        self._show_disable_adb_warning()
+        self._show_support_message()
```

### Comparing `mvt-2.5.0/mvt/common/help.py` & `mvt-2.5.1/mvt/common/help.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/common/indicators.py` & `mvt-2.5.1/mvt/common/indicators.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/common/logo.py` & `mvt-2.5.1/mvt/common/logo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/common/module.py` & `mvt-2.5.1/mvt/common/module.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/common/options.py` & `mvt-2.5.1/mvt/common/options.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/common/updates.py` & `mvt-2.5.1/mvt/common/updates.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/common/url.py` & `mvt-2.5.1/mvt/common/url.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,254 +5,322 @@
 
 from typing import Optional
 
 import requests
 from tld import get_tld
 
 SHORTENER_DOMAINS = [
+    "0rz.tw",
     "1drv.ms",
     "1link.in",
     "1url.com",
     "2big.at",
+    "2.gp",
     "2pl.us",
     "2tu.us",
     "2ya.com",
+    "3.ly",
+    "4sq.com",
     "4url.cc",
     "6url.com",
-    "a.gg",
-    "a.nf",
+    "7.ly",
     "a2a.me",
     "abbrr.com",
     "adf.ly",
     "adjix.com",
+    "a.gg",
     "alturl.com",
+    "a.nf",
+    "anon.to",
+    "apple.news",
     "atu.ca",
     "b23.ru",
     "bacn.me",
+    "bc.vc",
+    "bfy.tw",
+    "binged.it",
     "bit.do",
     "bit.ly",
+    "bizj.us",
     "bkite.com",
     "bloat.me",
     "budurl.com",
     "buff.ly",
     "buk.me",
     "burnurl.com",
-    "c-o.in",
     "chilp.it",
+    "chn.ge",
     "clck.ru",
-    "cli.gs",
     "clickmeter.com",
+    "cli.gs",
+    "c-o.in",
     "cort.as",
     "cut.ly",
+    "cutt.ly",
     "cuturl.com",
-    "decenturl.com",
+    "dai.ly",
+    "dailym.ai",
+    "db.tt",
     "decenturl.com",
     "dfl8.me",
     "digbig.com",
     "digg.com",
+    "disq.us",
+    "dlvr.it",
     "doiop.com",
+    "do.my",
     "dwarfurl.com",
     "dy.fi",
     "easyuri.com",
     "easyurl.net",
     "eepurl.com",
     "esyurl.com",
     "ewerl.com",
     "fa.b",
-    "ff.im",
+    "fa.by",
+    "fb.me",
     "fff.to",
+    "ff.im",
     "fhurl.com",
     "fire.to",
     "firsturl.de",
+    "firsturl.net",
     "flic.kr",
+    "flq.us",
     "fly2.ws",
     "fon.gs",
     "forms.gle",
     "fwd4.me",
+    "gdurl.com",
+    "gg.gg",
     "gl.am",
-    "go.9nl.com",
-    "go2.me",
     "go2cut.com",
+    "go2.me",
+    "go.9nl.com",
     "goo.gl",
     "goshrink.com",
+    "got.by",
     "gowat.ch",
     "gri.ms",
     "gurl.es",
     "hellotxt.com",
     "hex.io",
+    "hongkiat.shorturl.com",
     "hover.com",
     "href.in",
     "ht.ly",
     "htxt.it",
     "hugeurl.com",
     "hurl.it",
     "hurl.me",
     "hurl.ws",
+    "ibb.co",
     "icanhaz.com",
     "idek.net",
     "inreply.to",
-    "is.gd",
     "iscool.net",
+    "is.gd",
     "iterasi.net",
     "jijr.com",
+    "j.mp",
     "jmp2.net",
     "just.as",
     "kissa.be",
     "kl.am",
     "klck.me",
     "korta.nu",
     "krunchd.com",
+    "lat.ms",
     "liip.to",
     "liltext.com",
     "lin.cr",
     "linkbee.com",
     "linkbun.ch",
     "liurl.cn",
-    "ln-s.net",
-    "ln-s.ru",
+    "lnkd.in",
     "lnk.gd",
     "lnk.in",
-    "lnkd.in",
+    "ln-s.net",
+    "ln-s.ru",
     "loopt.us",
     "lru.jp",
     "lt.tl",
     "lurl.no",
+    "lyhyt.eu",
     "metamark.net",
     "migre.me",
     "minilien.com",
     "miniurl.com",
     "minurl.fr",
     "moourl.com",
     "myurl.in",
+    "nbcnews.to",
     "ne1.net",
     "njx.me",
     "nn.nf",
     "notlong.com",
+    "n.pr",
     "nsfw.in",
-    "o-x.fr",
+    "nyti.ms",
     "om.ly",
+    "onforb.es",
+    "on.mktw.net",
     "ow.ly",
+    "o-x.fr",
+    "pca.st",
     "pd.am",
     "pic.gd",
     "ping.fm",
     "piurl.com",
     "pnt.me",
+    "politi.co",
     "poprl.com",
-    "post.ly",
     "posted.at",
+    "post.ly",
     "profile.to",
+    "q.gs",
     "qicute.com",
     "qlnk.net",
+    "qr.ae",
+    "qte.me",
     "quip-art.com",
     "rb6.me",
+    "rb.gy",
+    "read.bi",
+    "redir.ec",
     "redirx.com",
-    "ri.ms",
+    "redr.me",
+    "reut.rs",
     "rickroll.it",
+    "r.im",
+    "ri.ms",
     "riz.gd",
     "rsmonkey.com",
-    "ru.ly",
     "rubyurl.com",
+    "ru.ly",
     "s7y.us",
     "safe.mn",
     "sharein.com",
     "sharetabs.com",
     "shorl.com",
     "short.ie",
-    "short.to",
     "shortlinks.co.uk",
     "shortna.me",
+    "short.to",
+    "shorturl.at",
     "shorturl.com",
     "shoturl.us",
+    "shout.to",
     "shrinkify.com",
     "shrinkster.com",
-    "shrt.st",
     "shrten.com",
+    "shrt.st",
     "shrunkin.com",
     "shw.me",
     "simurl.com",
+    "smsh.me",
     "sn.im",
     "snipr.com",
     "snipurl.com",
     "snurl.com",
     "sp2.ro",
     "spedr.com",
     "sqrl.it",
     "starturl.com",
     "sturly.com",
     "su.pr",
+    "t.cn",
     "t.co",
     "tcrn.ch",
+    "tgr.ph",
     "thrdl.es",
     "tighturl.com",
-    "tiny.cc",
-    "tiny.pl",
     "tiny123.com",
     "tinyarro.ws",
+    "tiny.cc",
+    "tinylink.in",
+    "tiny.pl",
+    "tiny.tw",
     "tinytw.it",
     "tinyuri.ca",
     "tinyurl.com",
     "tinyvid.io",
+    "t.me",
     "tnij.org",
-    "to.ly",
+    "tnw.to",
     "togoto.us",
+    "to.ly",
+    "traceurl.com",
     "tr.im",
     "tr.my",
-    "traceurl.com",
     "turo.us",
     "tweetburner.com",
     "twirl.at",
     "twit.ac",
     "twitterpan.com",
     "twitthis.com",
     "twiturl.de",
     "twurl.cc",
     "twurl.nl",
-    "u.mavrev.com",
-    "u.nu",
     "u6e.de",
     "ub0.cc",
+    "ukl.me.uk",
+    "u.mavrev.com",
+    "u.nu",
     "updating.me",
     "ur1.ca",
-    "url.co.uk",
-    "url.ie",
     "url4.eu",
     "urlao.com",
     "urlbrief.com",
+    "url.co.uk",
     "urlcover.com",
     "urlcut.com",
     "urlenco.de",
     "urlhawk.com",
+    "url.ie",
     "urlkiss.com",
     "urlot.com",
     "urlpire.com",
     "urlx.ie",
     "urlx.org",
     "urlzen.com",
+    "use.my",
+    "u.to",
+    "v.gd",
     "virl.com",
     "vl.am",
+    "vurl.com",
+    "vzturl.com",
     "w3t.org",
+    "wapo.st",
     "wapurl.co.uk",
     "wipi.es",
     "wp.me",
-    "x.co",
-    "x.se",
     "xaddr.com",
+    "x.co",
     "xeeurl.com",
     "xr.com",
     "xrl.in",
     "xrl.us",
+    "x.se",
+    "xurl.es",
     "xurl.jp",
     "xzb.cc",
+    "ye.pe",
     "yep.it",
     "yfrog.com",
+    "yhoo.it",
     "ymlp.com",
+    "yuarel.com",
     "yweb.com",
     "zi.ma",
     "zi.pe",
     "zipmyurl.com",
+    "zurl.to",
+    "zurl.ws",
     "zz.gd",
 ]
 
 
 class URL:
     def __init__(self, url: str) -> None:
         if isinstance(url, bytes):
```

### Comparing `mvt-2.5.0/mvt/common/utils.py` & `mvt-2.5.1/mvt/common/utils.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/common/virustotal.py` & `mvt-2.5.1/mvt/common/virustotal.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/cli.py` & `mvt-2.5.1/mvt/ios/cli.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/cmd_check_backup.py` & `mvt-2.5.1/mvt/ios/cmd_check_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/cmd_check_fs.py` & `mvt-2.5.1/mvt/ios/cmd_check_fs.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/data/ios_models.json` & `mvt-2.5.1/mvt/ios/data/ios_models.json`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/data/ios_versions.json` & `mvt-2.5.1/mvt/ios/data/ios_versions.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9621212121212122%*

 * *Differences: {'insert': "[(221, OrderedDict([('version', '15.8.1'), ('build', '19H380')])), (222, "*

 * *           "OrderedDict([('version', '15.8.2'), ('build', '19H384')])), (244, "*

 * *           "OrderedDict([('version', '16.7.5'), ('build', '20H307')])), (245, "*

 * *           "OrderedDict([('version', '16.7.6'), ('build', '20H320')])), (246, "*

 * *           "OrderedDict([('version', '16.7.7'), ('build', '20H330')])), (259, "*

 * *           "OrderedDict([('version', '17.3'), ('build', '21D50')])), (260, "*

 * *           "OrderedDict([('v […]*

```diff
@@ -880,14 +880,22 @@
         "version": "15.7.9"
     },
     {
         "build": "19H370",
         "version": "15.8"
     },
     {
+        "build": "19H380",
+        "version": "15.8.1"
+    },
+    {
+        "build": "19H384",
+        "version": "15.8.2"
+    },
+    {
         "build": "20A362",
         "version": "16.0"
     },
     {
         "build": "20A371",
         "version": "16.0.1"
     },
@@ -965,14 +973,26 @@
         "version": "16.7.3"
     },
     {
         "build": "20H240",
         "version": "16.7.4"
     },
     {
+        "build": "20H307",
+        "version": "16.7.5"
+    },
+    {
+        "build": "20H320",
+        "version": "16.7.6"
+    },
+    {
+        "build": "20H330",
+        "version": "16.7.7"
+    },
+    {
         "build": "21A327",
         "version": "17.0"
     },
     {
         "build": "21A329",
         "version": "17.0"
     },
@@ -1011,9 +1031,29 @@
     {
         "build": "21C62",
         "version": "17.2"
     },
     {
         "build": "21C66",
         "version": "17.2.1"
+    },
+    {
+        "build": "21D50",
+        "version": "17.3"
+    },
+    {
+        "build": "21D61",
+        "version": "17.3.1"
+    },
+    {
+        "build": "21E219",
+        "version": "17.4"
+    },
+    {
+        "build": "21E236",
+        "version": "17.4.1"
+    },
+    {
+        "build": "21E237",
+        "version": "17.4.1"
     }
 ]
```

### Comparing `mvt-2.5.0/mvt/ios/decrypt.py` & `mvt-2.5.1/mvt/ios/decrypt.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/backup/backup_info.py` & `mvt-2.5.1/mvt/ios/modules/backup/backup_info.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/backup/configuration_profiles.py` & `mvt-2.5.1/mvt/ios/modules/backup/configuration_profiles.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/backup/manifest.py` & `mvt-2.5.1/mvt/ios/modules/backup/manifest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/backup/profile_events.py` & `mvt-2.5.1/mvt/ios/modules/backup/profile_events.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/base.py` & `mvt-2.5.1/mvt/ios/modules/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/fs/__init__.py` & `mvt-2.5.1/mvt/ios/modules/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/fs/analytics.py` & `mvt-2.5.1/mvt/ios/modules/fs/analytics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/fs/analytics_ios_versions.py` & `mvt-2.5.1/mvt/ios/modules/fs/analytics_ios_versions.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/fs/cache_files.py` & `mvt-2.5.1/mvt/ios/modules/fs/cache_files.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/fs/filesystem.py` & `mvt-2.5.1/mvt/ios/modules/fs/filesystem.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/fs/net_netusage.py` & `mvt-2.5.1/mvt/ios/modules/fs/net_netusage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/fs/safari_favicon.py` & `mvt-2.5.1/mvt/ios/modules/fs/safari_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/fs/shutdownlog.py` & `mvt-2.5.1/mvt/ios/modules/fs/shutdownlog.py`

 * *Files 21% similar despite different names*

```diff
@@ -66,46 +66,67 @@
                     )
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
     def process_shutdownlog(self, content):
         current_processes = []
+        recent_processes = []
+        times_delayed = 0
+        delay = 0.0
         for line in content.split("\n"):
             line = line.strip()
 
             if line.startswith("remaining client pid:"):
                 current_processes.append(
                     {
                         "pid": line[line.find("pid: ") + 5 : line.find(" (")],
                         "client": line[line.find("(") + 1 : line.find(")")],
+                        "delay": delay,
+                        "times_delayed": times_delayed,
                     }
                 )
+            elif line.startswith("After "):
+                # Consider the previous processes
+                # End of the current processes
+                for p in current_processes:
+                    recent_processes.append(p)
+                delay += float(line.split(" ")[1][:-2])
+                times_delayed += 1
+                current_processes = []
             elif line.startswith("SIGTERM: "):
+                for p in current_processes:
+                    recent_processes.append(p)
+
                 try:
                     mac_timestamp = int(line[line.find("[") + 1 : line.find("]")])
                 except ValueError:
                     try:
                         start = line.find(" @") + 2
                         mac_timestamp = int(line[start : start + 10])
                     except Exception:
                         mac_timestamp = 0
 
                 isodate = convert_mactime_to_iso(mac_timestamp, from_2001=False)
 
-                for current_process in current_processes:
+                for process in recent_processes:
                     self.results.append(
                         {
                             "isodate": isodate,
-                            "pid": current_process["pid"],
-                            "client": current_process["client"],
+                            "pid": process["pid"],
+                            "client": process["client"],
+                            "delay": process["delay"],
+                            "times_delayed": process["times_delayed"],
                         }
                     )
 
                 current_processes = []
+                recent_processes = []
+                times_delayed = 0
+                delay = 0.0
 
         self.results = sorted(self.results, key=lambda entry: entry["isodate"])
 
     def run(self) -> None:
         self._find_ios_database(root_paths=SHUTDOWN_LOG_PATH)
         self.log.info("Found shutdown log at path: %s", self.file_path)
         with open(self.file_path, "r", encoding="utf-8") as handle:
```

### Comparing `mvt-2.5.0/mvt/ios/modules/fs/version_history.py` & `mvt-2.5.1/mvt/ios/modules/fs/version_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/fs/webkit_base.py` & `mvt-2.5.1/mvt/ios/modules/fs/webkit_base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/fs/webkit_indexeddb.py` & `mvt-2.5.1/mvt/ios/modules/fs/webkit_indexeddb.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/fs/webkit_localstorage.py` & `mvt-2.5.1/mvt/ios/modules/fs/webkit_localstorage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/fs/webkit_safariviewservice.py` & `mvt-2.5.1/mvt/ios/modules/fs/webkit_safariviewservice.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/__init__.py` & `mvt-2.5.1/mvt/ios/modules/mixed/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/applications.py` & `mvt-2.5.1/mvt/ios/modules/mixed/applications.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/calendar.py` & `mvt-2.5.1/mvt/ios/modules/mixed/calendar.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/calls.py` & `mvt-2.5.1/mvt/ios/modules/mixed/calls.py`

 * *Files 13% similar despite different names*

```diff
@@ -65,17 +65,17 @@
 
         for row in cur:
             self.results.append(
                 {
                     "isodate": convert_mactime_to_iso(row[0]),
                     "duration": row[1],
                     "location": row[2],
-                    "number": row[3].decode("utf-8")
-                    if row[3] and row[3] is bytes
-                    else row[3],
+                    "number": (
+                        row[3].decode("utf-8") if row[3] and row[3] is bytes else row[3]
+                    ),
                     "provider": row[4],
                 }
             )
 
         cur.close()
         conn.close()
```

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/chrome_favicon.py` & `mvt-2.5.1/mvt/ios/modules/mixed/chrome_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/chrome_history.py` & `mvt-2.5.1/mvt/ios/modules/mixed/chrome_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/contacts.py` & `mvt-2.5.1/mvt/ios/modules/mixed/contacts.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/firefox_favicon.py` & `mvt-2.5.1/mvt/ios/modules/mixed/firefox_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/firefox_history.py` & `mvt-2.5.1/mvt/ios/modules/mixed/firefox_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/global_preferences.py` & `mvt-2.5.1/mvt/ios/modules/mixed/global_preferences.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/interactionc.py` & `mvt-2.5.1/mvt/ios/modules/mixed/interactionc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/locationd.py` & `mvt-2.5.1/mvt/ios/modules/mixed/locationd.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/net_datausage.py` & `mvt-2.5.1/mvt/ios/modules/mixed/net_datausage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/osanalytics_addaily.py` & `mvt-2.5.1/mvt/ios/modules/mixed/osanalytics_addaily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/safari_browserstate.py` & `mvt-2.5.1/mvt/ios/modules/mixed/safari_browserstate.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/safari_history.py` & `mvt-2.5.1/mvt/ios/modules/mixed/safari_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/shortcuts.py` & `mvt-2.5.1/mvt/ios/modules/mixed/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/sms.py` & `mvt-2.5.1/mvt/ios/modules/mixed/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/sms_attachments.py` & `mvt-2.5.1/mvt/ios/modules/mixed/sms_attachments.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,17 @@
             f"(is_sticker: {record['is_sticker']}, "
             f"has_user_info: {record['has_user_info']})",
         }
 
     def check_indicators(self) -> None:
         for attachment in self.results:
             # Check for known malicious filenames.
-            if self.indicators.check_file_path(attachment["filename"]):
+            if self.indicators and self.indicators.check_file_path(
+                attachment["filename"]
+            ):
                 self.detected.append(attachment)
 
             if (
                 attachment["filename"].startswith("/var/tmp/")
                 and attachment["filename"].endswith("-1")
                 and attachment["direction"] == "received"
             ):
```

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/tcc.py` & `mvt-2.5.1/mvt/ios/modules/mixed/tcc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/webkit_resource_load_statistics.py` & `mvt-2.5.1/mvt/ios/modules/mixed/webkit_resource_load_statistics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/webkit_session_resource_log.py` & `mvt-2.5.1/mvt/ios/modules/mixed/webkit_session_resource_log.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/mixed/whatsapp.py` & `mvt-2.5.1/mvt/ios/modules/mixed/whatsapp.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/modules/net_base.py` & `mvt-2.5.1/mvt/ios/modules/net_base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt/ios/versions.py` & `mvt-2.5.1/mvt/ios/versions.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/mvt.egg-info/PKG-INFO` & `mvt-2.5.1/mvt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvt
-Version: 2.5.0
+Version: 2.5.1
 Summary: Mobile Verification Toolkit
 Home-page: https://github.com/mvt-project/mvt
 Author: Claudio Guarnieri
 Author-email: nex@nex.sx
 License: MVT v1.1
 Keywords: security,mobile,forensics,malware
 Classifier: Development Status :: 5 - Production/Stable
@@ -52,15 +52,15 @@
 MVT supports using public [indicators of compromise (IOCs)](https://github.com/mvt-project/mvt-indicators) to scan mobile devices for potential traces of targeting or infection by known spyware campaigns. This includes IOCs published by [Amnesty International](https://github.com/AmnestyTech/investigations/) and other  research groups.
 
 > **Warning**
 > Public indicators of compromise are insufficient to determine that a device is "clean", and not targeted with a particular spyware tool. Reliance on public indicators alone can miss recent forensic traces and give a false sense of security.
 >
 > Reliable and comprehensive digital forensic support and triage requires access to non-public indicators, research and threat intelligence.
 >
->Such support is available to civil society through [Amnesty International's Security Lab](https://www.amnesty.org/en/tech/) or through our forensic partnership with [Access Now’s Digital Security Helpline](https://www.accessnow.org/help/).
+>Such support is available to civil society through [Amnesty International's Security Lab](https://securitylab.amnesty.org/get-help/?c=mvt_docs) or through our forensic partnership with [Access Now’s Digital Security Helpline](https://www.accessnow.org/help/).
 
 More information about using indicators of compromise with MVT is available in the [documentation](https://docs.mvt.re/en/latest/iocs/).
 
 ## Installation
 
 MVT can be installed from sources or from [PyPI](https://pypi.org/project/mvt/) (you will need some dependencies, check the [documentation](https://docs.mvt.re/en/latest/install/)):
```

### Comparing `mvt-2.5.0/mvt.egg-info/SOURCES.txt` & `mvt-2.5.1/mvt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 ./mvt/android/artifacts/artifact.py
 ./mvt/android/artifacts/dumpsys_accessibility.py
 ./mvt/android/artifacts/dumpsys_appops.py
 ./mvt/android/artifacts/dumpsys_battery_daily.py
 ./mvt/android/artifacts/dumpsys_battery_history.py
 ./mvt/android/artifacts/dumpsys_dbinfo.py
 ./mvt/android/artifacts/dumpsys_package_activities.py
+./mvt/android/artifacts/dumpsys_packages.py
 ./mvt/android/artifacts/dumpsys_receivers.py
 ./mvt/android/artifacts/getprop.py
 ./mvt/android/artifacts/processes.py
 ./mvt/android/artifacts/settings.py
 ./mvt/android/modules/__init__.py
 ./mvt/android/modules/adb/__init__.py
 ./mvt/android/modules/adb/base.py
@@ -78,15 +79,14 @@
 ./mvt/android/modules/bugreport/battery_history.py
 ./mvt/android/modules/bugreport/dbinfo.py
 ./mvt/android/modules/bugreport/getprop.py
 ./mvt/android/modules/bugreport/packages.py
 ./mvt/android/modules/bugreport/receivers.py
 ./mvt/android/parsers/__init__.py
 ./mvt/android/parsers/backup.py
-./mvt/android/parsers/dumpsys.py
 ./mvt/common/__init__.py
 ./mvt/common/artifact.py
 ./mvt/common/cmd_check_iocs.py
 ./mvt/common/command.py
 ./mvt/common/help.py
 ./mvt/common/indicators.py
 ./mvt/common/logo.py
@@ -162,14 +162,15 @@
 ./tests/android/test_artifact.py
 ./tests/android/test_artifact_dumpsys_accessibility.py
 ./tests/android/test_artifact_dumpsys_appops.py
 ./tests/android/test_artifact_dumpsys_battery_daily.py
 ./tests/android/test_artifact_dumpsys_battery_history.py
 ./tests/android/test_artifact_dumpsys_dbinfo.py
 ./tests/android/test_artifact_dumpsys_package_activities.py
+./tests/android/test_artifact_dumpsys_packages.py
 ./tests/android/test_artifact_dumpsys_receivers.py
 ./tests/android/test_artifact_getprop.py
 ./tests/android/test_artifact_processes.py
 ./tests/android/test_backup_module.py
 ./tests/android/test_backup_parser.py
 ./tests/android_adb/__init__.py
 ./tests/android_androidqf/__init__.py
```

### Comparing `mvt-2.5.0/setup.cfg` & `mvt-2.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android/test_artifact.py` & `mvt-2.5.1/tests/android/test_artifact.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android/test_artifact_dumpsys_accessibility.py` & `mvt-2.5.1/tests/android/test_artifact_dumpsys_accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android/test_artifact_dumpsys_appops.py` & `mvt-2.5.1/tests/android/test_artifact_dumpsys_appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android/test_artifact_dumpsys_battery_daily.py` & `mvt-2.5.1/tests/android/test_artifact_dumpsys_battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android/test_artifact_dumpsys_battery_history.py` & `mvt-2.5.1/tests/android/test_artifact_dumpsys_battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android/test_artifact_dumpsys_dbinfo.py` & `mvt-2.5.1/tests/android/test_artifact_dumpsys_dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android/test_artifact_dumpsys_package_activities.py` & `mvt-2.5.1/tests/android/test_artifact_dumpsys_package_activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android/test_artifact_dumpsys_receivers.py` & `mvt-2.5.1/tests/android/test_artifact_dumpsys_receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android/test_artifact_getprop.py` & `mvt-2.5.1/tests/android/test_artifact_getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android/test_artifact_processes.py` & `mvt-2.5.1/tests/android/test_artifact_processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android/test_backup_module.py` & `mvt-2.5.1/tests/android/test_backup_module.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android/test_backup_parser.py` & `mvt-2.5.1/tests/android/test_backup_parser.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android_androidqf/test_dumpsys_battery_daily.py` & `mvt-2.5.1/tests/android_androidqf/test_dumpsys_battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android_androidqf/test_dumpsys_battery_history.py` & `mvt-2.5.1/tests/android_androidqf/test_dumpsys_battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android_androidqf/test_dumpsys_dbinfo.py` & `mvt-2.5.1/tests/android_androidqf/test_dumpsys_dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android_androidqf/test_dumpsysaccessbility.py` & `mvt-2.5.1/tests/android_androidqf/test_dumpsysaccessbility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android_androidqf/test_dumpsysappops.py` & `mvt-2.5.1/tests/android_androidqf/test_dumpsysappops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android_androidqf/test_dumpsyspackages.py` & `mvt-2.5.1/tests/android_androidqf/test_dumpsyspackages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android_androidqf/test_dumpsysreceivers.py` & `mvt-2.5.1/tests/android_androidqf/test_dumpsysreceivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android_androidqf/test_getprop.py` & `mvt-2.5.1/tests/android_androidqf/test_getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android_androidqf/test_processes.py` & `mvt-2.5.1/tests/android_androidqf/test_processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android_androidqf/test_settings.py` & `mvt-2.5.1/tests/android_androidqf/test_settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android_androidqf/test_sms.py` & `mvt-2.5.1/tests/android_androidqf/test_sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/android_bugreport/test_bugreport.py` & `mvt-2.5.1/tests/android_bugreport/test_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/common/test_indicators.py` & `mvt-2.5.1/tests/common/test_indicators.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/common/test_utils.py` & `mvt-2.5.1/tests/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/conftest.py` & `mvt-2.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/ios_backup/test_backup_info.py` & `mvt-2.5.1/tests/ios_backup/test_backup_info.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/ios_backup/test_calendar.py` & `mvt-2.5.1/tests/ios_backup/test_calendar.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/ios_backup/test_datausage.py` & `mvt-2.5.1/tests/ios_backup/test_datausage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/ios_backup/test_global_preferences.py` & `mvt-2.5.1/tests/ios_backup/test_global_preferences.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/ios_backup/test_manifest.py` & `mvt-2.5.1/tests/ios_backup/test_manifest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/ios_backup/test_safari_browserstate.py` & `mvt-2.5.1/tests/ios_backup/test_safari_browserstate.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/ios_backup/test_sms.py` & `mvt-2.5.1/tests/ios_backup/test_sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/ios_backup/test_tcc.py` & `mvt-2.5.1/tests/ios_backup/test_tcc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/ios_backup/test_webkit_resource_load_statistics.py` & `mvt-2.5.1/tests/ios_backup/test_webkit_resource_load_statistics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/ios_fs/test_filesystem.py` & `mvt-2.5.1/tests/ios_fs/test_filesystem.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 The MVT Authors.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 import logging
 
-
 from mvt.common.indicators import Indicators
 from mvt.common.module import run_module
 from mvt.ios.modules.fs.filesystem import Filesystem
 
 from ..utils import get_ios_backup_folder
```

### Comparing `mvt-2.5.0/tests/test_check_android_androidqf.py` & `mvt-2.5.1/tests/test_check_android_androidqf.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/test_check_android_backup.py` & `mvt-2.5.1/tests/test_check_android_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/test_check_android_bugreport.py` & `mvt-2.5.1/tests/test_check_android_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/test_check_ios_backup.py` & `mvt-2.5.1/tests/test_check_ios_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.0/tests/utils.py` & `mvt-2.5.1/tests/utils.py`

 * *Files identical despite different names*

