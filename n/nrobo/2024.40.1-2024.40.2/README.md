# Comparing `tmp/nrobo-2024.40.1.tar.gz` & `tmp/nrobo-2024.40.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrobo-2024.40.1.tar", last modified: Sat Apr  6 10:58:01 2024, max compression
+gzip compressed data, was "nrobo-2024.40.2.tar", last modified: Thu Apr 11 06:47:03 2024, max compression
```

## Comparing `nrobo-2024.40.1.tar` & `nrobo-2024.40.2.tar`

### file list

```diff
@@ -1,127 +1,131 @@
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.397645 nrobo-2024.40.1/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1079 2024-02-02 05:31:36.000000 nrobo-2024.40.1/LICENSE
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-06 10:58:01.396987 nrobo-2024.40.1/PKG-INFO
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    16531 2024-04-06 10:57:44.000000 nrobo-2024.40.1/README.rst
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.366448 nrobo-2024.40.1/nrobo/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8702 2024-04-06 10:57:34.000000 nrobo-2024.40.1/nrobo/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.369850 nrobo-2024.40.1/nrobo/appium/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      716 2024-03-11 11:20:45.000000 nrobo-2024.40.1/nrobo/appium/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       72 2024-03-11 14:41:50.000000 nrobo-2024.40.1/nrobo/appium/android_capability.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       73 2024-03-11 12:05:03.000000 nrobo-2024.40.1/nrobo/appium/ios_capability.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.371721 nrobo-2024.40.1/nrobo/browserConfigs/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      452 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/browserConfigs/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       35 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/browserConfigs/capability.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-19 15:42:30.000000 nrobo-2024.40.1/nrobo/browserConfigs/chrome_config.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       39 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/browserConfigs/chrome_prefs.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       63 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/browserConfigs/markers.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.372090 nrobo-2024.40.1/nrobo/browsers/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      459 2024-02-15 02:56:21.000000 nrobo-2024.40.1/nrobo/browsers/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.372458 nrobo-2024.40.1/nrobo/browsers/chrome/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2168 2024-02-15 02:56:21.000000 nrobo-2024.40.1/nrobo/browsers/chrome/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.372825 nrobo-2024.40.1/nrobo/browsers/edge/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      468 2024-02-15 02:56:21.000000 nrobo-2024.40.1/nrobo/browsers/edge/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.373196 nrobo-2024.40.1/nrobo/browsers/firefox/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      472 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/browsers/firefox/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.373566 nrobo-2024.40.1/nrobo/browsers/safari/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      477 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/browsers/safari/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.375547 nrobo-2024.40.1/nrobo/cli/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2654 2024-03-23 16:37:25.000000 nrobo-2024.40.1/nrobo/cli/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2895 2024-03-11 13:01:11.000000 nrobo-2024.40.1/nrobo/cli/cli_constants.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-15 02:56:21.000000 nrobo-2024.40.1/nrobo/cli/cli_version.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.375919 nrobo-2024.40.1/nrobo/cli/detection/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2585 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/cli/detection/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.376381 nrobo-2024.40.1/nrobo/cli/formatting/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1226 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/cli/formatting/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.377288 nrobo-2024.40.1/nrobo/cli/install/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    12266 2024-03-24 02:00:53.000000 nrobo-2024.40.1/nrobo/cli/install/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      987 2024-04-02 19:56:57.000000 nrobo-2024.40.1/nrobo/cli/install/requirements.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    15058 2024-03-07 11:01:00.000000 nrobo-2024.40.1/nrobo/cli/launcher.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.377678 nrobo-2024.40.1/nrobo/cli/ncodes/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      594 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/cli/ncodes/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1806 2024-03-01 03:35:55.000000 nrobo-2024.40.1/nrobo/cli/nglobals.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.378068 nrobo-2024.40.1/nrobo/cli/nrobo_args/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    25971 2024-03-11 13:04:58.000000 nrobo-2024.40.1/nrobo/cli/nrobo_args/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.378527 nrobo-2024.40.1/nrobo/cli/tools/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      813 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/cli/tools/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.378911 nrobo-2024.40.1/nrobo/cli/upgrade/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6308 2024-03-06 04:27:25.000000 nrobo-2024.40.1/nrobo/cli/upgrade/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    32195 2024-04-06 10:57:34.000000 nrobo-2024.40.1/nrobo/conftest.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.379289 nrobo-2024.40.1/nrobo/exceptions/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1937 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/exceptions/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.381089 nrobo-2024.40.1/nrobo/framework/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-05 04:31:26.000000 nrobo-2024.40.1/nrobo/framework/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      540 2024-02-16 15:47:33.000000 nrobo-2024.40.1/nrobo/framework/conftest-host.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      779 2024-03-07 13:19:52.000000 nrobo-2024.40.1/nrobo/framework/nrobo-config.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.382144 nrobo-2024.40.1/nrobo/framework/pages/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1506 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/pages/PagePyPiHome.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      485 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/pages/PageSearch.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2540 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/pages/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       26 2024-03-23 15:17:33.000000 nrobo-2024.40.1/nrobo/framework/requirements.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:56:49.000000 nrobo-2024.40.1/nrobo/framework/secrets.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.382804 nrobo-2024.40.1/nrobo/framework/test-data/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 19:41:06.000000 nrobo-2024.40.1/nrobo/framework/test-data/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6402 2024-02-13 06:51:47.000000 nrobo-2024.40.1/nrobo/framework/test-data/nRoBo-Logo.png
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.383198 nrobo-2024.40.1/nrobo/framework/tests/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        2 2024-02-07 04:51:13.000000 nrobo-2024.40.1/nrobo/framework/tests/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.359964 nrobo-2024.40.1/nrobo/framework/tests/mobile/
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.383591 nrobo-2024.40.1/nrobo/framework/tests/mobile/appium/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      383 2024-03-07 08:23:34.000000 nrobo-2024.40.1/nrobo/framework/tests/mobile/appium/test_appium.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.384234 nrobo-2024.40.1/nrobo/framework/tests/web/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1904 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/PyPi_home_page_test.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.384732 nrobo-2024.40.1/nrobo/framework/tests/web/examples/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6470 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/examples/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.385835 nrobo-2024.40.1/nrobo/framework/tests/web/gui/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      723 2024-03-03 02:33:11.000000 nrobo-2024.40.1/nrobo/framework/tests/web/gui/PyPi_home_page_test.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:32.000000 nrobo-2024.40.1/nrobo/framework/tests/web/gui/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.386150 nrobo-2024.40.1/nrobo/framework/tests/web/no_gui/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:18.000000 nrobo-2024.40.1/nrobo/framework/tests/web/no_gui/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.389069 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      820 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2427 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8284 2024-04-05 20:33:08.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    19118 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1418 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6860 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.389458 nrobo-2024.40.1/nrobo/selenese/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    49008 2024-04-06 08:38:03.000000 nrobo-2024.40.1/nrobo/selenese/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.389927 nrobo-2024.40.1/nrobo/util/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.40.1/nrobo/util/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.390316 nrobo-2024.40.1/nrobo/util/commands/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.40.1/nrobo/util/commands/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.390704 nrobo-2024.40.1/nrobo/util/commands/ncommands/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2105 2024-03-06 18:41:46.000000 nrobo-2024.40.1/nrobo/util/commands/ncommands/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.391089 nrobo-2024.40.1/nrobo/util/commands/posix/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      533 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/util/commands/posix/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.391472 nrobo-2024.40.1/nrobo/util/commands/windows/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      535 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/util/commands/windows/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.391846 nrobo-2024.40.1/nrobo/util/common/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7376 2024-03-18 10:49:47.000000 nrobo-2024.40.1/nrobo/util/common/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.392227 nrobo-2024.40.1/nrobo/util/constants/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1686 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/util/constants/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.392917 nrobo-2024.40.1/nrobo/util/database/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:55:53.000000 nrobo-2024.40.1/nrobo/util/database/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1992 2024-03-30 08:55:53.000000 nrobo-2024.40.1/nrobo/util/database/connectors.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.393303 nrobo-2024.40.1/nrobo/util/filesystem/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6919 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/util/filesystem/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.393682 nrobo-2024.40.1/nrobo/util/network/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      844 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/util/network/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.394058 nrobo-2024.40.1/nrobo/util/platform/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      742 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/util/platform/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.394450 nrobo-2024.40.1/nrobo/util/process/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     3322 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/util/process/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.394847 nrobo-2024.40.1/nrobo/util/python/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2101 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/util/python/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.395223 nrobo-2024.40.1/nrobo/util/regex/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      976 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/util/regex/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.395600 nrobo-2024.40.1/nrobo/util/version/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8316 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/util/version/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.396099 nrobo-2024.40.1/nrobo.egg-info/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-06 10:58:01.000000 nrobo-2024.40.1/nrobo.egg-info/PKG-INFO
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2855 2024-04-06 10:58:01.000000 nrobo-2024.40.1/nrobo.egg-info/SOURCES.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        1 2024-04-06 10:58:01.000000 nrobo-2024.40.1/nrobo.egg-info/dependency_links.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       41 2024-04-06 10:58:01.000000 nrobo-2024.40.1/nrobo.egg-info/entry_points.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       43 2024-04-06 10:58:01.000000 nrobo-2024.40.1/nrobo.egg-info/requires.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        6 2024-04-06 10:58:01.000000 nrobo-2024.40.1/nrobo.egg-info/top_level.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2545 2024-04-06 10:57:34.000000 nrobo-2024.40.1/pyproject.toml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       38 2024-04-06 10:58:01.397760 nrobo-2024.40.1/setup.cfg
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.138254 nrobo-2024.40.2/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1079 2024-02-02 05:31:36.000000 nrobo-2024.40.2/LICENSE
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-11 06:47:03.137607 nrobo-2024.40.2/PKG-INFO
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    16531 2024-04-11 06:46:47.000000 nrobo-2024.40.2/README.rst
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.104027 nrobo-2024.40.2/nrobo/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8702 2024-04-11 06:46:40.000000 nrobo-2024.40.2/nrobo/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.107403 nrobo-2024.40.2/nrobo/appium/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      716 2024-03-11 11:20:45.000000 nrobo-2024.40.2/nrobo/appium/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       72 2024-03-11 14:41:50.000000 nrobo-2024.40.2/nrobo/appium/android_capability.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       73 2024-03-11 12:05:03.000000 nrobo-2024.40.2/nrobo/appium/ios_capability.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.107720 nrobo-2024.40.2/nrobo/aws/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      475 2024-04-06 18:19:37.000000 nrobo-2024.40.2/nrobo/aws/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.110091 nrobo-2024.40.2/nrobo/browserConfigs/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      452 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/browserConfigs/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       35 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/browserConfigs/capability.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-19 15:42:30.000000 nrobo-2024.40.2/nrobo/browserConfigs/chrome_config.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       39 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/browserConfigs/chrome_prefs.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       63 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/browserConfigs/markers.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.110631 nrobo-2024.40.2/nrobo/browsers/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      459 2024-02-15 02:56:21.000000 nrobo-2024.40.2/nrobo/browsers/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.111204 nrobo-2024.40.2/nrobo/browsers/chrome/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2168 2024-02-15 02:56:21.000000 nrobo-2024.40.2/nrobo/browsers/chrome/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.111797 nrobo-2024.40.2/nrobo/browsers/edge/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      468 2024-02-15 02:56:21.000000 nrobo-2024.40.2/nrobo/browsers/edge/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.112378 nrobo-2024.40.2/nrobo/browsers/firefox/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      472 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/browsers/firefox/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.112944 nrobo-2024.40.2/nrobo/browsers/safari/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      477 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/browsers/safari/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.117149 nrobo-2024.40.2/nrobo/cli/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2654 2024-03-23 16:37:25.000000 nrobo-2024.40.2/nrobo/cli/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2895 2024-03-11 13:01:11.000000 nrobo-2024.40.2/nrobo/cli/cli_constants.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-15 02:56:21.000000 nrobo-2024.40.2/nrobo/cli/cli_version.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.117719 nrobo-2024.40.2/nrobo/cli/detection/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2585 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/cli/detection/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.118257 nrobo-2024.40.2/nrobo/cli/formatting/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1226 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/cli/formatting/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.119496 nrobo-2024.40.2/nrobo/cli/install/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    12266 2024-03-24 02:00:53.000000 nrobo-2024.40.2/nrobo/cli/install/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      987 2024-04-02 19:56:57.000000 nrobo-2024.40.2/nrobo/cli/install/requirements.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    15058 2024-03-07 11:01:00.000000 nrobo-2024.40.2/nrobo/cli/launcher.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.120053 nrobo-2024.40.2/nrobo/cli/ncodes/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      594 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/cli/ncodes/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1806 2024-03-01 03:35:55.000000 nrobo-2024.40.2/nrobo/cli/nglobals.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.120604 nrobo-2024.40.2/nrobo/cli/nrobo_args/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    25971 2024-03-11 13:04:58.000000 nrobo-2024.40.2/nrobo/cli/nrobo_args/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.121084 nrobo-2024.40.2/nrobo/cli/tools/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      813 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/cli/tools/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.121438 nrobo-2024.40.2/nrobo/cli/upgrade/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6308 2024-03-06 04:27:25.000000 nrobo-2024.40.2/nrobo/cli/upgrade/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    32195 2024-04-11 06:46:40.000000 nrobo-2024.40.2/nrobo/conftest.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.121763 nrobo-2024.40.2/nrobo/db/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      477 2024-04-06 18:20:42.000000 nrobo-2024.40.2/nrobo/db/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.122079 nrobo-2024.40.2/nrobo/exceptions/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1937 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/exceptions/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.123946 nrobo-2024.40.2/nrobo/framework/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-05 04:31:26.000000 nrobo-2024.40.2/nrobo/framework/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      540 2024-02-16 15:47:33.000000 nrobo-2024.40.2/nrobo/framework/conftest-host.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      779 2024-03-07 13:19:52.000000 nrobo-2024.40.2/nrobo/framework/nrobo-config.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.124928 nrobo-2024.40.2/nrobo/framework/pages/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1506 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/pages/PagePyPiHome.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      485 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/pages/PageSearch.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2540 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/pages/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       26 2024-03-23 15:17:33.000000 nrobo-2024.40.2/nrobo/framework/requirements.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:56:49.000000 nrobo-2024.40.2/nrobo/framework/secrets.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.125540 nrobo-2024.40.2/nrobo/framework/test-data/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 19:41:06.000000 nrobo-2024.40.2/nrobo/framework/test-data/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6402 2024-02-13 06:51:47.000000 nrobo-2024.40.2/nrobo/framework/test-data/nRoBo-Logo.png
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.125891 nrobo-2024.40.2/nrobo/framework/tests/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        2 2024-02-07 04:51:13.000000 nrobo-2024.40.2/nrobo/framework/tests/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.098888 nrobo-2024.40.2/nrobo/framework/tests/mobile/
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.126234 nrobo-2024.40.2/nrobo/framework/tests/mobile/appium/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      383 2024-03-07 08:23:34.000000 nrobo-2024.40.2/nrobo/framework/tests/mobile/appium/test_appium.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.126582 nrobo-2024.40.2/nrobo/framework/tests/web/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1904 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/PyPi_home_page_test.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.126920 nrobo-2024.40.2/nrobo/framework/tests/web/examples/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6470 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/examples/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.127617 nrobo-2024.40.2/nrobo/framework/tests/web/gui/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      723 2024-03-03 02:33:11.000000 nrobo-2024.40.2/nrobo/framework/tests/web/gui/PyPi_home_page_test.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:32.000000 nrobo-2024.40.2/nrobo/framework/tests/web/gui/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.127896 nrobo-2024.40.2/nrobo/framework/tests/web/no_gui/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:18.000000 nrobo-2024.40.2/nrobo/framework/tests/web/no_gui/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.130291 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      820 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2427 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8284 2024-04-05 20:33:08.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    19118 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1418 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6860 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.130625 nrobo-2024.40.2/nrobo/selenese/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    49008 2024-04-06 08:38:03.000000 nrobo-2024.40.2/nrobo/selenese/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.131029 nrobo-2024.40.2/nrobo/util/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.40.2/nrobo/util/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.131363 nrobo-2024.40.2/nrobo/util/commands/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.40.2/nrobo/util/commands/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.131692 nrobo-2024.40.2/nrobo/util/commands/ncommands/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2105 2024-03-06 18:41:46.000000 nrobo-2024.40.2/nrobo/util/commands/ncommands/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.132029 nrobo-2024.40.2/nrobo/util/commands/posix/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      533 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/util/commands/posix/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.132358 nrobo-2024.40.2/nrobo/util/commands/windows/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      535 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/util/commands/windows/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.132690 nrobo-2024.40.2/nrobo/util/common/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7376 2024-03-18 10:49:47.000000 nrobo-2024.40.2/nrobo/util/common/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.133128 nrobo-2024.40.2/nrobo/util/constants/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1686 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/util/constants/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.133840 nrobo-2024.40.2/nrobo/util/database/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:55:53.000000 nrobo-2024.40.2/nrobo/util/database/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1992 2024-03-30 08:55:53.000000 nrobo-2024.40.2/nrobo/util/database/connectors.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.134216 nrobo-2024.40.2/nrobo/util/filesystem/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6919 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/util/filesystem/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.134577 nrobo-2024.40.2/nrobo/util/network/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      844 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/util/network/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.134939 nrobo-2024.40.2/nrobo/util/platform/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      742 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/util/platform/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.135279 nrobo-2024.40.2/nrobo/util/process/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     3322 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/util/process/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.135631 nrobo-2024.40.2/nrobo/util/python/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2101 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/util/python/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.135980 nrobo-2024.40.2/nrobo/util/regex/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      976 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/util/regex/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.136317 nrobo-2024.40.2/nrobo/util/version/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8316 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/util/version/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.136792 nrobo-2024.40.2/nrobo.egg-info/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-11 06:47:03.000000 nrobo-2024.40.2/nrobo.egg-info/PKG-INFO
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2898 2024-04-11 06:47:03.000000 nrobo-2024.40.2/nrobo.egg-info/SOURCES.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        1 2024-04-11 06:47:03.000000 nrobo-2024.40.2/nrobo.egg-info/dependency_links.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       41 2024-04-11 06:47:03.000000 nrobo-2024.40.2/nrobo.egg-info/entry_points.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       43 2024-04-11 06:47:03.000000 nrobo-2024.40.2/nrobo.egg-info/requires.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        6 2024-04-11 06:47:03.000000 nrobo-2024.40.2/nrobo.egg-info/top_level.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2545 2024-04-11 06:46:40.000000 nrobo-2024.40.2/pyproject.toml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       38 2024-04-11 06:47:03.138372 nrobo-2024.40.2/setup.cfg
```

### Comparing `nrobo-2024.40.1/LICENSE` & `nrobo-2024.40.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/PKG-INFO` & `nrobo-2024.40.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrobo
-Version: 2024.40.1
+Version: 2024.40.2
 Summary: Powerful! Yet, Easy to USE! Automated Testing Framework
 Author-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Maintainer-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/nrobo/
 Project-URL: GitHub Repo, https://github.com/pancht/ngrobo
 Project-URL: Bug Tracker, https://github.com/pancht/ngrobo/issues
 Project-URL: changelog, https://github.com/pancht/ngrobo/blob/master/CHANGELOG.md
@@ -384,113 +384,113 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 38.91%
-     - 23,363
+     - 39.12%
+     - 24,003
    * - CN
-     - 12.98%
-     - 7,792
+     - 12.84%
+     - 7,878
    * - DE
-     - 6.76%
-     - 4,057
+     - 6.98%
+     - 4,282
    * - SG
-     - 5.55%
-     - 3,332
+     - 5.48%
+     - 3,364
    * - RU
-     - 5.12%
-     - 3,075
+     - 5.22%
+     - 3,202
    * - HK
-     - 4.10%
-     - 2,462
+     - 4.05%
+     - 2,486
    * - JP
-     - 3.07%
-     - 1,842
+     - 3.01%
+     - 1,846
    * - FR
-     - 2.81%
-     - 1,685
+     - 2.80%
+     - 1,719
    * - KR
-     - 2.68%
-     - 1,611
+     - 2.69%
+     - 1,652
    * - CA
-     - 2.65%
-     - 1,591
+     - 2.62%
+     - 1,607
    * - NO
-     - 2.18%
-     - 1,307
+     - 2.16%
+     - 1,327
    * - GB
-     - 1.83%
-     - 1,096
+     - 1.79%
+     - 1,100
    * - AU
-     - 1.75%
-     - 1,048
+     - 1.74%
+     - 1,065
    * - IN
-     - 1.52%
-     - 911
+     - 1.50%
+     - 923
    * - SE
-     - 1.20%
-     - 718
+     - 1.18%
+     - 725
    * - TH
-     - 0.78%
-     - 469
+     - 0.77%
+     - 475
    * - HR
-     - 0.78%
-     - 466
+     - 0.76%
+     - 468
    * - IE
-     - 0.66%
-     - 395
+     - 0.65%
+     - 399
    * - DK
-     - 0.66%
-     - 395
+     - 0.65%
+     - 397
    * - TW
-     - 0.60%
+     - 0.59%
      - 363
    * - IL
-     - 0.57%
+     - 0.56%
      - 341
    * - NL
-     - 0.49%
+     - 0.48%
      - 297
    * - ES
-     - 0.44%
+     - 0.43%
      - 262
    * - CH
      - 0.42%
-     - 254
+     - 255
    * - AE
      - 0.34%
-     - 207
+     - 209
    * - CZ
-     - 0.24%
+     - 0.23%
      - 144
    * - FI
      - 0.16%
-     - 97
+     - 99
    * - ZA
      - 0.15%
      - 89
    * - BR
      - 0.13%
      - 77
    * - PL
      - 0.10%
      - 61
-   * - CW
-     - 0.07%
-     - 44
    * - TR
      - 0.07%
+     - 46
+   * - CW
+     - 0.07%
      - 44
-   * - OM
+   * - IS
      - 0.07%
      - 42
-   * - IS
+   * - OM
      - 0.07%
      - 42
    * - RO
      - 0.04%
      - 24
    * - GF
      - 0.02%
@@ -500,29 +500,29 @@
      - 8
    * - CY
      - 0.01%
      - 6
    * - DZ
      - 0.01%
      - 4
-   * - EE
+   * - AR
      - 0.00%
      - 3
-   * - AR
+   * - EE
      - 0.00%
      - 3
    * - SK
      - 0.00%
      - 2
    * - MX
      - 0.00%
      - 1
-   * - PT
+   * - RS
      - 0.00%
      - 1
-   * - RS
+   * - PT
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **60,042**
+     - **61,352**
```

### Comparing `nrobo-2024.40.1/README.rst` & `nrobo-2024.40.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -348,113 +348,113 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 38.91%
-     - 23,363
+     - 39.12%
+     - 24,003
    * - CN
-     - 12.98%
-     - 7,792
+     - 12.84%
+     - 7,878
    * - DE
-     - 6.76%
-     - 4,057
+     - 6.98%
+     - 4,282
    * - SG
-     - 5.55%
-     - 3,332
+     - 5.48%
+     - 3,364
    * - RU
-     - 5.12%
-     - 3,075
+     - 5.22%
+     - 3,202
    * - HK
-     - 4.10%
-     - 2,462
+     - 4.05%
+     - 2,486
    * - JP
-     - 3.07%
-     - 1,842
+     - 3.01%
+     - 1,846
    * - FR
-     - 2.81%
-     - 1,685
+     - 2.80%
+     - 1,719
    * - KR
-     - 2.68%
-     - 1,611
+     - 2.69%
+     - 1,652
    * - CA
-     - 2.65%
-     - 1,591
+     - 2.62%
+     - 1,607
    * - NO
-     - 2.18%
-     - 1,307
+     - 2.16%
+     - 1,327
    * - GB
-     - 1.83%
-     - 1,096
+     - 1.79%
+     - 1,100
    * - AU
-     - 1.75%
-     - 1,048
+     - 1.74%
+     - 1,065
    * - IN
-     - 1.52%
-     - 911
+     - 1.50%
+     - 923
    * - SE
-     - 1.20%
-     - 718
+     - 1.18%
+     - 725
    * - TH
-     - 0.78%
-     - 469
+     - 0.77%
+     - 475
    * - HR
-     - 0.78%
-     - 466
+     - 0.76%
+     - 468
    * - IE
-     - 0.66%
-     - 395
+     - 0.65%
+     - 399
    * - DK
-     - 0.66%
-     - 395
+     - 0.65%
+     - 397
    * - TW
-     - 0.60%
+     - 0.59%
      - 363
    * - IL
-     - 0.57%
+     - 0.56%
      - 341
    * - NL
-     - 0.49%
+     - 0.48%
      - 297
    * - ES
-     - 0.44%
+     - 0.43%
      - 262
    * - CH
      - 0.42%
-     - 254
+     - 255
    * - AE
      - 0.34%
-     - 207
+     - 209
    * - CZ
-     - 0.24%
+     - 0.23%
      - 144
    * - FI
      - 0.16%
-     - 97
+     - 99
    * - ZA
      - 0.15%
      - 89
    * - BR
      - 0.13%
      - 77
    * - PL
      - 0.10%
      - 61
-   * - CW
-     - 0.07%
-     - 44
    * - TR
      - 0.07%
+     - 46
+   * - CW
+     - 0.07%
      - 44
-   * - OM
+   * - IS
      - 0.07%
      - 42
-   * - IS
+   * - OM
      - 0.07%
      - 42
    * - RO
      - 0.04%
      - 24
    * - GF
      - 0.02%
@@ -464,29 +464,29 @@
      - 8
    * - CY
      - 0.01%
      - 6
    * - DZ
      - 0.01%
      - 4
-   * - EE
+   * - AR
      - 0.00%
      - 3
-   * - AR
+   * - EE
      - 0.00%
      - 3
    * - SK
      - 0.00%
      - 2
    * - MX
      - 0.00%
      - 1
-   * - PT
+   * - RS
      - 0.00%
      - 1
-   * - RS
+   * - PT
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **60,042**
+     - **61,352**
```

### Comparing `nrobo-2024.40.1/nrobo/__init__.py` & `nrobo-2024.40.2/nrobo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 nrobo module loads nRoBo globals.
 
 
 @author: Panchdev Singh Chauhan
 @email: erpanchdev@gmail.com
 """
 
-__version__ = '2024.40.1'
+__version__ = '2024.40.2'
 
 # install rich library
 import os
 from pathlib import Path
 
 
 class DB_CONNECTOR_TYPE:
```

### Comparing `nrobo-2024.40.1/nrobo/appium/__init__.py` & `nrobo-2024.40.2/nrobo/appium/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/browsers/chrome/__init__.py` & `nrobo-2024.40.2/nrobo/browsers/chrome/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/cli/__init__.py` & `nrobo-2024.40.2/nrobo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/cli/cli_constants.py` & `nrobo-2024.40.2/nrobo/cli/cli_constants.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/cli/detection/__init__.py` & `nrobo-2024.40.2/nrobo/cli/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/cli/formatting/__init__.py` & `nrobo-2024.40.2/nrobo/cli/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/cli/install/__init__.py` & `nrobo-2024.40.2/nrobo/cli/install/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/cli/install/requirements.txt` & `nrobo-2024.40.2/nrobo/cli/install/requirements.txt`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/cli/launcher.py` & `nrobo-2024.40.2/nrobo/cli/launcher.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/cli/ncodes/__init__.py` & `nrobo-2024.40.2/nrobo/cli/ncodes/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/cli/nglobals.py` & `nrobo-2024.40.2/nrobo/cli/nglobals.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/cli/nrobo_args/__init__.py` & `nrobo-2024.40.2/nrobo/cli/nrobo_args/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/cli/tools/__init__.py` & `nrobo-2024.40.2/nrobo/cli/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/cli/upgrade/__init__.py` & `nrobo-2024.40.2/nrobo/cli/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/conftest.py` & `nrobo-2024.40.2/nrobo/conftest.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/exceptions/__init__.py` & `nrobo-2024.40.2/nrobo/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/conftest-host.py` & `nrobo-2024.40.2/nrobo/framework/conftest-host.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/nrobo-config.yaml` & `nrobo-2024.40.2/nrobo/framework/nrobo-config.yaml`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/pages/PagePyPiHome.py` & `nrobo-2024.40.2/nrobo/framework/pages/PagePyPiHome.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/pages/__init__.py` & `nrobo-2024.40.2/nrobo/framework/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/test-data/nRoBo-Logo.png` & `nrobo-2024.40.2/nrobo/framework/test-data/nRoBo-Logo.png`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/tests/web/PyPi_home_page_test.py` & `nrobo-2024.40.2/nrobo/framework/tests/web/PyPi_home_page_test.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/tests/web/examples/__init__.py` & `nrobo-2024.40.2/nrobo/framework/tests/web/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/tests/web/gui/PyPi_home_page_test.py` & `nrobo-2024.40.2/nrobo/framework/tests/web/gui/PyPi_home_page_test.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py` & `nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py` & `nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py` & `nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py` & `nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py` & `nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py` & `nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/selenese/__init__.py` & `nrobo-2024.40.2/nrobo/selenese/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/util/commands/ncommands/__init__.py` & `nrobo-2024.40.2/nrobo/util/commands/ncommands/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/util/commands/posix/__init__.py` & `nrobo-2024.40.2/nrobo/util/commands/posix/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/util/commands/windows/__init__.py` & `nrobo-2024.40.2/nrobo/util/commands/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/util/common/__init__.py` & `nrobo-2024.40.2/nrobo/util/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/util/constants/__init__.py` & `nrobo-2024.40.2/nrobo/util/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/util/database/connectors.py` & `nrobo-2024.40.2/nrobo/util/database/connectors.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/util/filesystem/__init__.py` & `nrobo-2024.40.2/nrobo/util/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/util/network/__init__.py` & `nrobo-2024.40.2/nrobo/util/network/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/util/platform/__init__.py` & `nrobo-2024.40.2/nrobo/util/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/util/process/__init__.py` & `nrobo-2024.40.2/nrobo/util/process/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/util/python/__init__.py` & `nrobo-2024.40.2/nrobo/util/python/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/util/regex/__init__.py` & `nrobo-2024.40.2/nrobo/util/regex/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo/util/version/__init__.py` & `nrobo-2024.40.2/nrobo/util/version/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.1/nrobo.egg-info/PKG-INFO` & `nrobo-2024.40.2/nrobo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrobo
-Version: 2024.40.1
+Version: 2024.40.2
 Summary: Powerful! Yet, Easy to USE! Automated Testing Framework
 Author-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Maintainer-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/nrobo/
 Project-URL: GitHub Repo, https://github.com/pancht/ngrobo
 Project-URL: Bug Tracker, https://github.com/pancht/ngrobo/issues
 Project-URL: changelog, https://github.com/pancht/ngrobo/blob/master/CHANGELOG.md
@@ -384,113 +384,113 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 38.91%
-     - 23,363
+     - 39.12%
+     - 24,003
    * - CN
-     - 12.98%
-     - 7,792
+     - 12.84%
+     - 7,878
    * - DE
-     - 6.76%
-     - 4,057
+     - 6.98%
+     - 4,282
    * - SG
-     - 5.55%
-     - 3,332
+     - 5.48%
+     - 3,364
    * - RU
-     - 5.12%
-     - 3,075
+     - 5.22%
+     - 3,202
    * - HK
-     - 4.10%
-     - 2,462
+     - 4.05%
+     - 2,486
    * - JP
-     - 3.07%
-     - 1,842
+     - 3.01%
+     - 1,846
    * - FR
-     - 2.81%
-     - 1,685
+     - 2.80%
+     - 1,719
    * - KR
-     - 2.68%
-     - 1,611
+     - 2.69%
+     - 1,652
    * - CA
-     - 2.65%
-     - 1,591
+     - 2.62%
+     - 1,607
    * - NO
-     - 2.18%
-     - 1,307
+     - 2.16%
+     - 1,327
    * - GB
-     - 1.83%
-     - 1,096
+     - 1.79%
+     - 1,100
    * - AU
-     - 1.75%
-     - 1,048
+     - 1.74%
+     - 1,065
    * - IN
-     - 1.52%
-     - 911
+     - 1.50%
+     - 923
    * - SE
-     - 1.20%
-     - 718
+     - 1.18%
+     - 725
    * - TH
-     - 0.78%
-     - 469
+     - 0.77%
+     - 475
    * - HR
-     - 0.78%
-     - 466
+     - 0.76%
+     - 468
    * - IE
-     - 0.66%
-     - 395
+     - 0.65%
+     - 399
    * - DK
-     - 0.66%
-     - 395
+     - 0.65%
+     - 397
    * - TW
-     - 0.60%
+     - 0.59%
      - 363
    * - IL
-     - 0.57%
+     - 0.56%
      - 341
    * - NL
-     - 0.49%
+     - 0.48%
      - 297
    * - ES
-     - 0.44%
+     - 0.43%
      - 262
    * - CH
      - 0.42%
-     - 254
+     - 255
    * - AE
      - 0.34%
-     - 207
+     - 209
    * - CZ
-     - 0.24%
+     - 0.23%
      - 144
    * - FI
      - 0.16%
-     - 97
+     - 99
    * - ZA
      - 0.15%
      - 89
    * - BR
      - 0.13%
      - 77
    * - PL
      - 0.10%
      - 61
-   * - CW
-     - 0.07%
-     - 44
    * - TR
      - 0.07%
+     - 46
+   * - CW
+     - 0.07%
      - 44
-   * - OM
+   * - IS
      - 0.07%
      - 42
-   * - IS
+   * - OM
      - 0.07%
      - 42
    * - RO
      - 0.04%
      - 24
    * - GF
      - 0.02%
@@ -500,29 +500,29 @@
      - 8
    * - CY
      - 0.01%
      - 6
    * - DZ
      - 0.01%
      - 4
-   * - EE
+   * - AR
      - 0.00%
      - 3
-   * - AR
+   * - EE
      - 0.00%
      - 3
    * - SK
      - 0.00%
      - 2
    * - MX
      - 0.00%
      - 1
-   * - PT
+   * - RS
      - 0.00%
      - 1
-   * - RS
+   * - PT
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **60,042**
+     - **61,352**
```

### Comparing `nrobo-2024.40.1/nrobo.egg-info/SOURCES.txt` & `nrobo-2024.40.2/nrobo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 nrobo.egg-info/dependency_links.txt
 nrobo.egg-info/entry_points.txt
 nrobo.egg-info/requires.txt
 nrobo.egg-info/top_level.txt
 nrobo/appium/__init__.py
 nrobo/appium/android_capability.yaml
 nrobo/appium/ios_capability.yaml
+nrobo/aws/__init__.py
 nrobo/browserConfigs/__init__.py
 nrobo/browserConfigs/capability.yaml
 nrobo/browserConfigs/chrome_config.txt
 nrobo/browserConfigs/chrome_prefs.yaml
 nrobo/browserConfigs/markers.yaml
 nrobo/browsers/__init__.py
 nrobo/browsers/chrome/__init__.py
@@ -31,14 +32,15 @@
 nrobo/cli/formatting/__init__.py
 nrobo/cli/install/__init__.py
 nrobo/cli/install/requirements.txt
 nrobo/cli/ncodes/__init__.py
 nrobo/cli/nrobo_args/__init__.py
 nrobo/cli/tools/__init__.py
 nrobo/cli/upgrade/__init__.py
+nrobo/db/__init__.py
 nrobo/exceptions/__init__.py
 nrobo/framework/__init__.py
 nrobo/framework/conftest-host.py
 nrobo/framework/nrobo-config.yaml
 nrobo/framework/requirements.txt
 nrobo/framework/secrets.yaml
 nrobo/framework/pages/PagePyPiHome.py
```

### Comparing `nrobo-2024.40.1/pyproject.toml` & `nrobo-2024.40.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["setuptools >= 40.7.0",]
 build-backend = "setuptools.build_meta"
 
 # Project details
 [project]
 name = "nrobo"
-version = "2024.40.1"
+version = "2024.40.2"
 authors = [{name="Panchdev Singh Chauhan", email="erpanchdev@gmail.com"}]
 maintainers = [{name="Panchdev Singh Chauhan", email="erpanchdev@gmail.com"}]
 description = "Powerful! Yet, Easy to USE! Automated Testing Framework"
 readme = "README.rst"
 keywords = ["test automation", "test automation framework", "automated testing", "automation testing", "testing", "qa", "acceptance test", "automation"]
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
```

