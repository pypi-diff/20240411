# Comparing `tmp/wiliot-core-5.4.3.tar.gz` & `tmp/wiliot-core-5.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-core-5.4.3.tar", last modified: Mon Jan 29 09:42:14 2024, max compression
+gzip compressed data, was "wiliot-core-5.5.8.tar", last modified: Thu Apr 11 12:51:09 2024, max compression
```

## Comparing `wiliot-core-5.4.3.tar` & `wiliot-core-5.5.8.tar`

### file list

```diff
@@ -1,67 +1,72 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:42:14.143332 wiliot-core-5.4.3/
--rw-rw-rw-   0 root         (0) root         (0)      258 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4726 2024-01-29 09:42:14.143332 wiliot-core-5.4.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4214 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7532 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      329 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-01-29 09:42:14.143332 wiliot-core-5.4.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1861 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:42:14.119332 wiliot-core-5.4.3/wiliot_core/
--rw-rw-rw-   0 root         (0) root         (0)     4665 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:42:14.123332 wiliot-core-5.4.3/wiliot_core/local_gateway/
--rw-rw-rw-   0 root         (0) root         (0)     4010 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15041 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/continuous_listener.py
--rw-rw-rw-   0 root         (0) root         (0)    12763 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/custom_energy_pattern.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:42:14.123332 wiliot-core-5.4.3/wiliot_core/local_gateway/examples/
--rw-rw-rw-   0 root         (0) root         (0)     4010 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7067 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/examples/local_gateway_basic_example.py
--rw-rw-rw-   0 root         (0) root         (0)    84994 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:42:14.139332 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/
--rw-rw-rw-   0 root         (0) root         (0)   253422 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   448599 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   122153 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.16_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   317338 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.16_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   122201 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.18_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   317386 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.18_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   122153 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.19_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   317338 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.19_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   229471 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   424656 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   125807 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.1.4_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   320992 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.1.4_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   130759 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.2.0_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   325944 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.2.0_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)  1242814 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex
--rw-rw-rw-   0 root         (0) root         (0)   881890 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.18.hex
--rw-rw-rw-   0 root         (0) root         (0)   881758 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.19.hex
--rw-rw-rw-   0 root         (0) root         (0)  1176930 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex
--rw-rw-rw-   0 root         (0) root         (0)   891838 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/wifi_4.1.4.hex
--rw-rw-rw-   0 root         (0) root         (0)   905450 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/wifi_4.2.0.hex
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:42:14.139332 wiliot-core-5.4.3/wiliot_core/packet_data/
--rw-rw-rw-   0 root         (0) root         (0)     4010 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/packet_data/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:42:14.139332 wiliot-core-5.4.3/wiliot_core/packet_data/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/packet_data/config_files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5021 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/packet_data/config_files/packet_flow_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    13146 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/packet_data/config_files/packet_map.py
--rw-rw-rw-   0 root         (0) root         (0)    26723 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/packet_data/packet.py
--rw-rw-rw-   0 root         (0) root         (0)    32367 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/packet_data/packet_list.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/packet_data/tag_collection.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:42:14.143332 wiliot-core-5.4.3/wiliot_core/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6185 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)     9296 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/utils/release_for_partners.py
--rw-rw-rw-   0 root         (0) root         (0)    14010 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/utils/update_wiliot_packages.py
--rw-rw-rw-   0 root         (0) root         (0)    15791 2024-01-29 09:41:57.000000 wiliot-core-5.4.3/wiliot_core/utils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-01-29 09:42:13.000000 wiliot-core-5.4.3/wiliot_core/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:42:14.123332 wiliot-core-5.4.3/wiliot_core.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4726 2024-01-29 09:42:13.000000 wiliot-core-5.4.3/wiliot_core.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2583 2024-01-29 09:42:14.000000 wiliot-core-5.4.3/wiliot_core.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-01-29 09:42:13.000000 wiliot-core-5.4.3/wiliot_core.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-01-29 09:42:13.000000 wiliot-core-5.4.3/wiliot_core.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-01-29 09:42:13.000000 wiliot-core-5.4.3/wiliot_core.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-01-29 09:42:13.000000 wiliot-core-5.4.3/wiliot_core.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:51:09.326946 wiliot-core-5.5.8/
+-rw-rw-rw-   0 root         (0) root         (0)      258 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     5371 2024-04-11 12:51:09.326946 wiliot-core-5.5.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4859 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7532 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      329 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-11 12:51:09.326946 wiliot-core-5.5.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1863 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:51:09.302946 wiliot-core-5.5.8/wiliot_core/
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:51:09.302946 wiliot-core-5.5.8/wiliot_core/local_gateway/
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15333 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/continuous_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)    12763 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/custom_energy_pattern.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:51:09.302946 wiliot-core-5.5.8/wiliot_core/local_gateway/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7616 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/examples/dual_gw_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     7067 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/examples/local_gateway_basic_example.py
+-rw-rw-rw-   0 root         (0) root         (0)    89635 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:51:09.322946 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/
+-rw-rw-rw-   0 root         (0) root         (0)   253422 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   448599 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   122153 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.16_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   317338 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.16_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   122201 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.18_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   317386 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.18_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   122153 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.19_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   317338 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.19_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   229471 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   424656 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   125807 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.1.4_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   320992 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.1.4_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   130759 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.2.0_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   325944 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.2.0_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   135079 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.3.3_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   330264 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.3.3_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)  1242814 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex
+-rw-rw-rw-   0 root         (0) root         (0)   881890 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.18.hex
+-rw-rw-rw-   0 root         (0) root         (0)   881758 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.19.hex
+-rw-rw-rw-   0 root         (0) root         (0)  1176930 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex
+-rw-rw-rw-   0 root         (0) root         (0)   891838 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.1.4.hex
+-rw-rw-rw-   0 root         (0) root         (0)   905450 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.2.0.hex
+-rw-rw-rw-   0 root         (0) root         (0)   917330 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.3.3.hex
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:51:09.322946 wiliot-core-5.5.8/wiliot_core/packet_data/
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/packet_data/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:51:09.326946 wiliot-core-5.5.8/wiliot_core/packet_data/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/packet_data/config_files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6368 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/packet_data/config_files/packet_flow_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    19254 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/packet_data/config_files/packet_map.py
+-rw-rw-rw-   0 root         (0) root         (0)     6352 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/packet_data/config_files/stat_calculation.py
+-rw-rw-rw-   0 root         (0) root         (0)    28175 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/packet_data/packet.py
+-rw-rw-rw-   0 root         (0) root         (0)    33444 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/packet_data/packet_list.py
+-rw-rw-rw-   0 root         (0) root         (0)    11013 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/packet_data/tag_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:51:09.326946 wiliot-core-5.5.8/wiliot_core/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6186 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     9296 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/utils/release_for_partners.py
+-rw-rw-rw-   0 root         (0) root         (0)    19966 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/utils/update_wiliot_packages.py
+-rw-rw-rw-   0 root         (0) root         (0)    15791 2024-04-11 12:50:59.000000 wiliot-core-5.5.8/wiliot_core/utils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-11 12:51:08.000000 wiliot-core-5.5.8/wiliot_core/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:51:09.302946 wiliot-core-5.5.8/wiliot_core.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     5371 2024-04-11 12:51:08.000000 wiliot-core-5.5.8/wiliot_core.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2893 2024-04-11 12:51:09.000000 wiliot-core-5.5.8/wiliot_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-11 12:51:08.000000 wiliot-core-5.5.8/wiliot_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-11 12:51:08.000000 wiliot-core-5.5.8/wiliot_core.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-04-11 12:51:08.000000 wiliot-core-5.5.8/wiliot_core.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-04-11 12:51:08.000000 wiliot-core-5.5.8/wiliot_core.egg-info/top_level.txt
```

### Comparing `wiliot-core-5.4.3/LICENSE` & `wiliot-core-5.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/PKG-INFO` & `wiliot-core-5.5.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-core
-Version: 5.4.3
+Version: 5.5.8
 Summary: A library for interacting with Wiliot's private core functions
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -57,14 +57,30 @@
 * [packet data](wiliot_core/packet_data) (at the end of each script)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 5.5.8:
+-----------------
+* update requirements
+* gateway core:
+  * add support to listen to two or more gw and merge data
+  * support auto time reset based on GW msg
+  * added support to connect to gw based on its name/uid
+  * added wrapper to get all gw responses similar to get packets
+  * added function of reconnect
+  * added function to control output signal (GPIO) from the GW
+  * added new firmware version
+* packets data core:
+  * support packets from cloud (payload)
+  * added new packet fields - gw clock, crc, adi (relevant to ble5 only) - effective only for the new firmware version
+  * add function to manipulate packets
+  
 Version 5.4.3:
 -----------------
 * gateway core:
   * Added new firmware version to local gateway
   * added the option to restart the gateway time based on command and control the log for buffer overload
 * packets data core:
   * Support Gen3 wiliot tags - tbp, per calculation
```

### Comparing `wiliot-core-5.4.3/README.md` & `wiliot-core-5.5.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,30 @@
 * [packet data](wiliot_core/packet_data) (at the end of each script)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 5.5.8:
+-----------------
+* update requirements
+* gateway core:
+  * add support to listen to two or more gw and merge data
+  * support auto time reset based on GW msg
+  * added support to connect to gw based on its name/uid
+  * added wrapper to get all gw responses similar to get packets
+  * added function of reconnect
+  * added function to control output signal (GPIO) from the GW
+  * added new firmware version
+* packets data core:
+  * support packets from cloud (payload)
+  * added new packet fields - gw clock, crc, adi (relevant to ble5 only) - effective only for the new firmware version
+  * add function to manipulate packets
+  
 Version 5.4.3:
 -----------------
 * gateway core:
   * Added new firmware version to local gateway
   * added the option to restart the gateway time based on command and control the log for buffer overload
 * packets data core:
   * Support Gen3 wiliot tags - tbp, per calculation
```

### Comparing `wiliot-core-5.4.3/bitbucket-pipelines.yml` & `wiliot-core-5.5.8/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/setup.py` & `wiliot-core-5.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,14 @@
                  install_requires=[
                      'setuptools_scm',
                      'pyserial',
                      'pc_ble_driver_py',
                      'nrfutil; sys_platform != "linux"',
                      'pandas',
                      'numpy<2',
-                     'PySimpleGUI',
+                     'PySimpleGUI<5',
                      'appdirs'
                  ],
                  zip_safe=False,
                  python_requires='>=3.6',
                  include_package_data=True,
                  )
```

### Comparing `wiliot-core-5.4.3/wiliot_core/__init__.py` & `wiliot-core-5.5.8/wiliot_core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 # gateway
 from wiliot_core.local_gateway.local_gateway_core import *
 
 # packet data
 from wiliot_core.packet_data.packet import *
 from wiliot_core.packet_data.packet_list import *
 from wiliot_core.packet_data.tag_collection import *
+from wiliot_core.packet_data.config_files.packet_map import *
 
 # utils
 from wiliot_core.utils.utils import *
 
 # package internal functions
 try:
     from wiliot_core.packet_data.extended.decrypted_packet import *
```

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/__init__.py` & `wiliot-core-5.5.8/wiliot_core/local_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/continuous_listener.py` & `wiliot-core-5.5.8/wiliot_core/local_gateway/continuous_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,9 +306,15 @@
         commands.put({'cmd': SerialProcessState.WRITE, 'data': {'gw_cmd': '!version'}})
         try:
             version_msg = gw_rsp.get(timeout=1)
             print('got rsp: {}'.format(version_msg))
         except Empty:
             print('empty')
         commands.put({'cmd': SerialProcessState.WRITE, 'data': {'gw_cmd': '!gateway_app'}})
+        time.sleep(5)
+        commands.put({'cmd': SerialProcessState.WRITE, 'data': {'gw_cmd': '!reset'}})
+        print(f'packet queue size: {packets.qsize()}')
+        for _ in range(packets.qsize()):
+            print(packets.get())
     else:
         print('problem during connection')
+        print(f'packet queue size: {packets.qsize()}')
```

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/custom_energy_pattern.py` & `wiliot-core-5.5.8/wiliot_core/local_gateway/custom_energy_pattern.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/examples/__init__.py` & `wiliot-core-5.5.8/wiliot_core/local_gateway/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/examples/local_gateway_basic_example.py` & `wiliot-core-5.5.8/wiliot_core/local_gateway/examples/local_gateway_basic_example.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_core.py` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,16 @@
     {'abs_power': 6, 'gw_output_power': 'neg12dBm', 'bypass_pa': '0'},
     {'abs_power': 10, 'gw_output_power': 'neg8dBm', 'bypass_pa': '0'},
     {'abs_power': 15, 'gw_output_power': 'neg4dBm', 'bypass_pa': '0'},
     {'abs_power': 20, 'gw_output_power': 'pos0dBm', 'bypass_pa': '0'},
     {'abs_power': 21, 'gw_output_power': 'pos2dBm', 'bypass_pa': '0'},
     {'abs_power': 22, 'gw_output_power': 'pos3dBm', 'bypass_pa': '0'}
 ]
-CMDS_WITHOUT_ACK = ['print', 'set_energizing_pattern', 'move_to_bootloader', 'version', 'pce', 'trigger_pl']
+CMDS_WITHOUT_ACK = ['print', 'set_energizing_pattern', 'move_to_bootloader', 'version', 'pce', 'trigger_pl', 'get_name']
+GW_START_APP_MSGS = ['Detected Low-to-High peak', 'Start Production Line GW']
 
 
 class ConfigParam:
     def __init__(self):
         self.energy_pattern = None
         self.received_channel = None
         self.time_profile_on = None
@@ -176,15 +177,15 @@
     :param auto_connect: If TRUE, connect automatically to the GW.
 
     :exception during open serial port process
     """
 
     def __init__(self, baud=921600, port=None, auto_connect=False, lock_print=None, logger_name=None, verbose=True,
                  socket_host='localhost', socket_port=8202, is_multi_processes=False, log_dir_for_multi_processes=None,
-                 mp_reset_time_upon_gw_start=None, np_max_packet_in_buffer_before_error=None):
+                 mp_reset_time_upon_gw_start=None, np_max_packet_in_buffer_before_error=None, device_name=None):
         """
         :type baud: int
         :param baud: the GW baud rate
         :type port: str
         :param port: The GW port if it is already know.
         :type auto_connect: bool
         :param auto_connect: If TRUE, connect automatically to the GW.
@@ -320,24 +321,35 @@
             self.available_ports = [s.name for s in serial.tools.list_ports.comports()
                                     if 'Silicon Labs' in s.description or 'CP210' in s.description]
             if len(self.available_ports) == 0:
                 self._printing_func("no serial ports were found. please check your connections", "init", True)
                 return
 
         # if user want to connect automatically - connecting to the first available COM with valid gw version
-        if auto_connect:
+        if auto_connect or device_name is not None:
             for p in self.available_ports:
                 try:
                     if self.open_port(p, self.baud):
                         self._printing_func("connection was established: {}={} , port {}".
                                             format(self.hw_version, self.sw_version, p), 'init')
                         self.connected = True
-                        break
+                        if device_name:
+                            cur_dev_name = self.write('!get_name', with_ack=True)
+                            if device_name.upper() in cur_dev_name['raw'].upper():
+                                break
+                            self.close_port()
+                            self.connected = False
+                            self._printing_func(f"connected to {p} but got wrong device name: {cur_dev_name},"
+                                                f" moving to the next port", 'init')
+                        else:
+                            break
                 except Exception as e:
                     self._printing_func("tried to connect {} but failed, moving to the next port".format(p), 'init')
+            if not self.connected:
+                self._printing_func("could not connect to the gateway", 'init')
 
     def set_logger(self, wanted_logger):
         self.logger = wanted_logger
 
     def set_verbosity(self, verbose=True):
         self.verbose = verbose
 
@@ -521,26 +533,30 @@
                     print('could not found a second/third row to gw respond {}'.format(e))
 
             if "unsupported" in data_in['raw'].lower():
                 is_ack = False
             else:
                 if isinstance(cmd, bytes):
                     cmd = cmd.decode()
-                is_ack = any([s in cmd for s in CMDS_WITHOUT_ACK]) or "command complete event" in data_in['raw'].lower()
+                is_ack = self.is_command_acknowledged(cmd=cmd, rsp=data_in['raw'])
 
             return data_in, is_ack
         else:
             is_ack = True
             data = self.readline_from_buffer()
             self._printing_func(
                 "GW write_get_response {} respond with {} is not supported "
                 "without continuous_listener_enabled".format(cmd, data),
                 "write_get_response")
             return {'raw': data, 'time': 0}, is_ack
 
+    @staticmethod
+    def is_command_acknowledged(cmd, rsp):
+        return any([s in cmd for s in CMDS_WITHOUT_ACK]) or "command complete event" in rsp.lower()
+
     def get_curr_timestamp_in_sec(self):
         return (datetime.datetime.now() - self.start_time).total_seconds()
 
     def read_specific_message(self, msg, read_timeout=1, clear=False):
         """
         search for specific message in the input buffer
         :type msg: str
@@ -720,15 +736,15 @@
         return is_stopped
 
     def config_gw(self, filter_val=None, pacer_val=None, energy_pattern_val=None, time_profile_val=None,
                   beacons_backoff_val=None, received_channel=None,
                   output_power_val=None, effective_output_power_val=None, sub1g_output_power_val=None,
                   bypass_pa_val=None, pl_delay_val=None, rssi_thr_val=None,
                   max_wait=1, check_validity=False, check_current_config_only=False, start_gw_app=True, with_ack=False,
-                  combined_msg=False):
+                  combined_msg=False, whitening_as_rx=False):
         """
         set all the input configuration
 
         :type filter_val: bool
         :param filter_val: set packet filter.
         :type pacer_val: int
         :param pacer_val: Set pacer interval
@@ -782,15 +798,15 @@
         # check the validity of the config parameters:
         if check_validity:
             self._printing_func("unavailable situation", 'config_gw')
             return
 
         # check if we can merge commands (channel, cycle time, transmit time, energizing pattern):
         if received_channel is not None and time_profile_val is not None and energy_pattern_val is not None \
-                and start_gw_app:
+                and start_gw_app and not whitening_as_rx:
             merge_msg = True
         else:
             merge_msg = False
 
         # stop gateway app before configuration:
         # if start_gw_app:
         #     self.write('!cancel')
@@ -920,16 +936,19 @@
                     self.config_param.pacer_val = pacer_val
 
         # set Received Channel
         if received_channel is not None and (not merge_msg or combined_msg):
             if combined_msg:
                 combined_msg_str += ' sc {}'.format(received_channel)
             else:
-                gateway_response = self.write('!scan_ch {}'.format(received_channel), with_ack=with_ack)
-                gateway_response['command'] = '!scan_ch {}'.format(received_channel)
+                cmd_str = f'!scan_ch {received_channel}'
+                if whitening_as_rx:
+                    cmd_str += f' {received_channel}'
+                gateway_response = self.write(cmd_str, with_ack=with_ack)
+                gateway_response['command'] = cmd_str
                 gateway_output.append(gateway_response)
                 if 'unsupported' in gateway_response['raw'].lower():
                     self.config_param.received_channel = None
                 else:
                     self.config_param.received_channel = received_channel
 
         # set Time Profile
@@ -1113,15 +1132,16 @@
             self.write('!move_to_bootloader')
             time.sleep(0.1)
             self.close_port()
 
             # run the nRF Util to burn the version:
             time.sleep(.1)
             # wait until burn was completed
-            self._printing_func("please wait for approx. 30 seconds...", 'update_version')
+            self._printing_func(f"update version from: {new_version_path}. please wait for approx. 30 seconds...",
+                                'update_version')
             command = 'nrfutil -v -v dfu serial  --package {} -p {} -fc 0 -b 115200 -t 10'.format(new_version_path,
                                                                                                   self.port)
             self.run_command(command)
 
             self._printing_func("Rebooting and opening serial port again...", 'update_version')
             time.sleep(5)
             for i in range(5):
@@ -1461,14 +1481,48 @@
 
     def reset_start_time(self):
         if self.multi_process:
             self.cmd_serial_process_q.put({'cmd': SerialProcessState.READ})
         with self.start_time_lock:
             self.start_time = datetime.datetime.now()
 
+    @staticmethod
+    def get_time_of_controlled_start_app(gw_rsp):
+        """
+        return the time when a start gw msg was received
+        :type gw_rsp list
+        :param gw_rsp list of all gw responses
+        : return the time of the start msg
+        :rtype float
+        """
+        for rsp in gw_rsp:
+            if any([start_msg in rsp['raw'] for start_msg in GW_START_APP_MSGS]):
+                return rsp['time']
+        return float('nan')
+
+    def get_gw_responses(self):
+        """
+        This function output all available gw responses and return it as a list of dict {'raw': '', 'time': 0}
+        """
+        if not self.continuous_listener_enabled and not self.multi_process:
+            raise ValueError("to use get_gw_responses please first call start_continuous_listener() "
+                             "or run using multi_process=True."
+                             "to stop the listener after usage call stop_continuous_listener()")
+
+        n_rsp = self.com_rsp_str_input_q.qsize()
+        all_rsp = []
+        for _ in range(n_rsp):
+            try:
+                data_in = self.com_rsp_str_input_q.get(timeout=0)
+                all_rsp.append(data_in)
+            except Exception as e:
+                self._printing_func(f'could not pull element from the response queue due to: {e}',
+                                    'get_gw_responses')
+        return all_rsp
+
     def get_packets(self, action_type=ActionType.FIRST_SAMPLES, num_of_packets=None, data_type=DataType.PACKET_LIST,
                     max_time=None, tag_inlay=None, is_blocking=True, send_to_additional_app=False, packet_version=None):
         """
         Extract packets from the queue, process according to data_type value.
                 action_type valid options:
                 all_samples: return all available packets.
                 first_samples: return all the X first packets (the oldest packets ) according to num_of_packages
@@ -1764,24 +1818,72 @@
             value = check_valid(value, HarvesterFlowValues)
         elif operation == MiniRxOperations.DEBUG_PACKET.value:
             value = check_valid(value, DebugPacketValues)
         elif operation == MiniRxOperations.HARVESTER_TYPE.value:
             value = check_valid(value, HarvesterTypeValues)
         elif operation == MiniRxOperations.BLE5_FREQ.value:
             value = check_valid(value, BleChannels)
+        elif operation == MiniRxOperations.EnterTestMode.value:
+            value = check_valid(value, EnterTestModeValues)
 
         beacons_train_cmd = '!beacons_train'
         beacons_train_cmd += f' {int(sub1g_energy)}'
         beacons_train_cmd += f' {get_mini_rx_sequence(x=operation, y=value)}'
         self.write(cmd=beacons_train_cmd, with_ack=True)
         if start_gw_app:
             self.write(cmd='!gateway_app', with_ack=True)
 
         return beacons_train_cmd
 
+    def reconnect(self):
+        is_connected = self.open_port(port=self.port, baud=self.baud)
+        if not is_connected:
+            raise Exception('gw-core: could not reconnect to GW')
+        self.reset_buffer()
+        return is_connected
+
+    # ######## GPIO Function #############
+
+    def set_gw_gpio(self, gpio_configs, is_send=False):
+        send_config_str = 'SEND' if is_send else 'SAVE'
+        for config in gpio_configs:
+            cmd = f'!cmd_gpio {send_config_str} {config["signal_num"]} {config["gpio"]} {config["signal_type"]} ' \
+                  f'{config["high_low"]}'
+            cmd += f' {config["pulse_time"]}' if 'pulse_time' in config else ''
+            rsp = self.write(cmd=cmd,  with_ack=True)
+            if rsp['raw'].lower() != 'command complete event':
+                raise Exception('gw-core: gpio config failed')
+
+    def gpio_state(self, gpio='',  state='ON', config=None):
+        if config is None:
+            config = {'signal_num': 1,
+                      'gpio': gpio.replace('.', '').upper(),
+                      'signal_type': 'static',
+                      'high_low': 1 if state.upper() == 'ON' else 0,
+                      }
+        self.set_gw_gpio(gpio_configs=[config], is_send=True)
+
+    def pulse(self, gpio='', pulse_duration_ms=None, config=None):
+        if config is None:
+            config = {'signal_num': 1,
+                      'gpio': gpio.replace('.', '').upper(),
+                      'signal_type': 'pulse',
+                      'high_low': 1,
+                      'pulse_time': pulse_duration_ms
+                      }
+        self.set_gw_gpio(gpio_configs=[config], is_send=True)
+
+    def gpio_send_signal(self, signal):
+        rsp = self.write(cmd=f'!cmd_gpio SEND {signal}', with_ack=True)
+        if rsp['raw'].lower() != 'command complete event':
+            raise Exception('gw-core: gpio state failed to send signal')
+
+    def __del__(self):
+        self.exit_gw_api()
+
 
 if __name__ == '__main__':
     print(datetime.datetime.now())
     gw = WiliotGateway(auto_connect=True, is_multi_processes=True)
     gw.send_mini_rx(operation=MiniRxOperations.HARVESTER_FLOW, value=HarvesterFlowValues.TRANSMIT_AT_MAX_DCO)
     gw.send_mini_rx(operation=MiniRxOperations.HARVESTER_TYPE, value=HarvesterTypeValues.X1)
     if gw.is_connected():
```

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.16_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.16_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.16_sd_bl_gw_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.16_sd_bl_gw_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.18_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.18_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.18_sd_bl_gw_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.18_sd_bl_gw_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.19_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.19_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.19_sd_bl_gw_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.19_sd_bl_gw_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.1.4_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.1.4_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.1.4_sd_bl_gw_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.1.4_sd_bl_gw_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.2.0_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.2.0_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/4.2.0_sd_bl_gw_app.zip` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/4.2.0_sd_bl_gw_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.18.hex` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.18.hex`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.19.hex` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.19.hex`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/wifi_4.1.4.hex` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.1.4.hex`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/local_gateway/local_gateway_versions/wifi_4.2.0.hex` & `wiliot-core-5.5.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.2.0.hex`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/packet_data/__init__.py` & `wiliot-core-5.5.8/wiliot_core/packet_data/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/packet_data/packet.py` & `wiliot-core-5.5.8/wiliot_core/packet_data/packet.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,37 +59,39 @@
 #  """
 import datetime
 import logging
 import numpy as np
 import pandas as pd
 import copy
 from enum import Enum
-from wiliot_core.packet_data.config_files.packet_map import parse_packet, gw_result_dict
+from wiliot_core.packet_data.config_files.packet_map import parse_packet, gw_result_dict, construct_packet_from_fields
 from wiliot_core.utils.utils import valid_packet_start
 from wiliot_core.packet_data.config_files.packet_flow_parameters import get_flow_param
 
 
 FULL_PACKET_PREFIX = 'full_packet'
 LEGACY_PACKET_PREFIX = 'process_packet'
 
 
 packet_tag_length = 74
 MAX_STAT_PARAM_VAL = 65535  # 2 bytes
+MAX_GW_CLOCK = 32767  # 7 bits
 
 
 class InlayTypes(Enum):
     TEO_086 = '086'
     TIKI_096 = '096'
     TIKI_099 = '099'
     BATTERY_107 = '107'
     TIKI_117 = '117'
     TIKI_118 = '118'
     TIKI_121 = '121'
     TIKI_122 = '122'
     TIKI_136 = '136'
+    TIKI_H_160 = '160'
 
 
 class Packet(object):
     """
     Wiliot Packet Object
 
         :param raw_packet: the raw packet to create a Packet object
@@ -159,27 +161,19 @@
             self.custom_data = custom_data
         else:
             self.custom_data = {}
         self.custom_data['timestamp'] = datetime.datetime.now().timestamp()
         self.inlay_type = inlay_type
 
         if self.is_valid_packet:
-            # TODO need to understand if this section supports everything - START
-            if int(self.packet_data['data_uid'], 16) == 5:
-                # TX LPM\HPM:
-                tx_lpm_hpm = int(self.packet_data['decrypted_packet_type']) & 1
-                self.decoded_data['tx_lpm_hpm'] = tx_lpm_hpm
-                if tx_lpm_hpm == 0:
-                    self.decoded_data['tx_lpm_hpm_str'] = 'LPM'
-                else:
-                    self.decoded_data['tx_lpm_hpm_str'] = 'HPM'
-                # battery mode:
-                battery_tag_ind = (int(self.packet_data['decrypted_packet_type']) & 2) >> 1
-                self.decoded_data['battery_tag_ind'] = battery_tag_ind
-            # TODO - END
+            # clear adi from packet and add it to custom data
+            if self.packet_data['ble_type'] != 'LEGACY':
+                self.custom_data['adi_per_packet'] = [self.packet_data['adi']]
+                self.packet_data['raw_packet'] = construct_packet_from_fields(packet_data=self.packet_data,
+                                                                              fields_to_zero=['adi'])
 
     def __len__(self):
         """
         gets number of sprinkler occurrences in packet
         """
         return self.gw_data['rssi'].size
 
@@ -211,14 +205,17 @@
     def get_payload(self):
         if self.is_valid_packet:
             return self.packet_data['data_uid'] + self.packet_data['raw_group_id'] + self.packet_data['nonce'] + \
                    self.packet_data['enc_uid'] + self.packet_data['mic'] + self.packet_data['enc_payload']
         else:
             return ''
 
+    def get_group_id(self):
+        return self.packet_data['group_id']
+
     def set_inlay_type(self, inlay_type):
         inlay_type = inlay_type if isinstance(inlay_type, str) else inlay_type.value
         self.inlay_type = inlay_type
 
     def is_in(self, packet):
         """
         is packet contains another packet
@@ -258,15 +255,15 @@
     def copy(self):
         return copy.deepcopy(self)
 
     def sort(self):
         """
         sort gw_data lists according to gw_time
         """
-        isort = np.argsort(self.gw_data['stat_param'])
+        isort = np.argsort(self.gw_data['gw_clock'])
         for key in self.gw_data.keys():
             self.gw_data[key] = self.gw_data[key][isort]
 
     def get_average_rssi(self):
         return np.average(self.gw_data['rssi'])
 
     def get_packet_size(self):
@@ -332,36 +329,38 @@
                 keys = keys + list(dict_temp[k].keys())
         return keys
 
     def is_same_sprinkler(self, packet):
         raw_packet = packet.packet_data['raw_packet']
         if raw_packet == self.packet_data['raw_packet']:
             return True
-        if self.packet_data['test_mode'] and self.packet_data['ble_type'] != 'LEGACY':
-            if ((raw_packet[0:20] + raw_packet[24:]) ==
-                    (self.packet_data['raw_packet'][0:20] + self.packet_data['raw_packet'][24:])):
-                return True
         return False
 
-    def append_to_sprinkler(self, packet, output_log=True):
+    def append_to_sprinkler(self, packet, output_log=True, do_sort=False):
         status = True
         if self.is_same_sprinkler(packet):
             for i in range(len(packet)):
                 try:
                     # stat param should be unique (time + rssi for same packet)- we make sure no duplications are added.
-                    if np.take(packet.gw_data['stat_param'], i).item() not in self.gw_data['stat_param'] or \
+                    if np.take(packet.gw_data['gw_clock'], i).item() not in self.gw_data['gw_clock'] or \
                             np.take(packet.gw_data['time_from_start'], i).item() not in self.gw_data['time_from_start']:
                         for key in gw_result_dict.keys():
                             self.gw_data[key] = np.append(self.gw_data[key], np.take(packet.gw_data[key], i))
                         for key in self.custom_data.keys():
                             if key in packet.custom_data.keys():
                                 self.custom_data[key] = np.append(self.custom_data[key],
                                                                   np.take(packet.custom_data[key], i))
                             else:
                                 self.custom_data[key] = np.append(self.custom_data[key], [None])
+                        if do_sort:
+                            sort_idx = self.gw_data['time_from_start'].argsort()
+                            for k, v in self.gw_data.items():
+                                self.gw_data[k] = v[sort_idx]
+                            for k, v in self.custom_data.items():
+                                self.custom_data[k] = v[sort_idx]
                     else:
                         if output_log:
                             self.printing_and_logging('Tried to add duplicated packet to sprinkler {}'.format(packet))
                 except Exception as e:
                     self.printing_and_logging('Failed to add packet {} to sprinkler, exception: {}'
                                               .format(packet, str(e)))
         else:
@@ -381,14 +380,20 @@
                 sprinkler_gw_data[gw_attr] = np.take(self.gw_data[gw_attr], sprinkler_index)
             for custom_attr in self.custom_data.keys():
                 custom_data[custom_attr] = np.take(self.custom_data[custom_attr], sprinkler_index)
             dict_len = 1
         else:
             dict_len = len(self)
             for k, v in packet_data.items():
+                if k == 'raw_packet' and 'adi_per_packet' in custom_data.keys():
+                    original_raw_packets = [construct_packet_from_fields(
+                        packet_data=self.packet_data,
+                        fields_to_convert={'adi': adi_per_packet}) for adi_per_packet in custom_data['adi_per_packet']]
+                    packet_data[k] = original_raw_packets
+                    continue
                 packet_data[k] = [v] * dict_len
 
         data = {**packet_data, **sprinkler_gw_data, **custom_data}
         data['gw_process'] = [self.gw_process] * dict_len  # bool should be a list for pd.DataFrame.from_dict(data)
         data['is_valid_packet'] = [self.is_valid_packet] * dict_len  # bool should be a list
         data['inlay_type'] = [self.inlay_type] * dict_len
         return data
@@ -402,15 +407,19 @@
     def get_per(self, expected_sprinkler_count=None):
         """
         Calculates the packet per at the sprinkler
         @param expected_sprinkler_count - The number of packet per sprinkler
         @return packet per at percentage
         """
         if expected_sprinkler_count is None:
-            expected_sprinkler_count = get_flow_param(flow_in=self.packet_data['flow_ver'], param_name='sprinkler_num')
+            if self.packet_data['test_mode']:
+                expected_sprinkler_count = 6
+            else:
+                expected_sprinkler_count = get_flow_param(flow_in=self.packet_data['flow_ver'],
+                                                          param_name='sprinkler_num')
         return 100 * (1 - len(self) / expected_sprinkler_count)
 
     def get_tbp(self):
         """
         calculates the rate of packets from the same sprinkler
         :return: min_times_found - in msec
         :rtype: int
@@ -448,19 +457,19 @@
             #     ind += counts
 
             times_list_sorted = times_list_sorted[fix_sort_idx]
             dt = []
             for i, t_hw in enumerate(zip(times_list_sorted[1::], times_list_sorted[:-1])):
                 dt_tmp = t_hw[0] - t_hw[1]
                 dt_pc = round((pc_time_list_sorted[i + 1] - pc_time_list_sorted[i]) * 1000)
-                if dt_pc >= MAX_STAT_PARAM_VAL:
+                if dt_pc >= MAX_GW_CLOCK:
                     # HW timing was zeroing during the same packets sprinkler
                     dt_tmp = dt_pc
                 elif dt_tmp < 0:
-                    dt_tmp += MAX_STAT_PARAM_VAL
+                    dt_tmp += MAX_GW_CLOCK
 
                 dt.append(dt_tmp)
 
             return dt
 
         def check_if_nan(lst):
             is_nan = pd.isnull(lst)
@@ -468,19 +477,22 @@
                 return is_nan
             if isinstance(is_nan.tolist(), bool):
                 return is_nan.tolist()
             if isinstance(is_nan, np.ndarray):
                 return any(is_nan)
             return False
 
-        if check_if_nan(self.gw_data['time_from_start']) or check_if_nan(self.gw_data['stat_param']):
+        if check_if_nan(self.gw_data['time_from_start']) or check_if_nan(self.gw_data['gw_clock']):
             return None
 
-        sprinkler_num = get_flow_param(flow_in=self.packet_data['flow_ver'], param_name='sprinkler_num')
-        estimate_diff_time = estimate_diff_packet_time(self.gw_data['stat_param'], self.gw_data['time_from_start'])
+        if self.packet_data['test_mode']:
+            sprinkler_num = 6
+        else:
+            sprinkler_num = get_flow_param(flow_in=self.packet_data['flow_ver'], param_name='sprinkler_num')
+        estimate_diff_time = estimate_diff_packet_time(self.gw_data['gw_clock'], self.gw_data['time_from_start'])
         if estimate_diff_time is None:
             return None
         elif len(self) == sprinkler_num/2 and sprinkler_num == 6:
             if triad_ratio_logic(estimate_diff_time[0], estimate_diff_time[1], ratio=1):
                 return None
             else:
                 for ratio in [2, 3, 4]:
@@ -557,17 +569,29 @@
                                               ' the number of packets')
             else:
                 self.custom_data[key] = self.__len__() * [custom_data[key]]
 
 
 if __name__ == '__main__':
 
+    # test mode packets with different adi, same sprinkler:
+    testing_82_tm_adi0 = Packet(
+        'full_packet("4731090906D03E34CD8200001EFF000505000060750774415ACDFFFBD069756C550DB1FD75E7B127312C21F3B10A03B1CB12AF2D45AC")')
+    testing_82_tm_adi1 = Packet(
+        'full_packet("4731090906D03E34CD8200011EFF000505000060750774415ACDFFFBD069756C550DB1FD75E7B127312C21F3B10A03B1CB12AF2D45CE")')
+    testing_82_tm_adi2 = Packet(
+        'full_packet("4731090906D03E34CD8200031EFF000505000060750774415ACDFFFBD069756C550DB1FD75E7B127312C21F3B10A03B1CB12AF2D4615")')
+    testing_82_tm_adi0.append_to_sprinkler(testing_82_tm_adi1)
+    testing_82_tm_adi0.append_to_sprinkler(testing_82_tm_adi2)
+    print(f'packet len: {len(testing_82_tm_adi0)} with the following adi: '
+          f'{testing_82_tm_adi0.custom_data["adi_per_packet"]}')
+
     packet_1 = {'packet': '03B28DCD99201EFF0005FE0000E0210FFF93B635EBFF1DB118C6D782DC2ED98C404200486436AE8F',
                 'is_valid_tag_packet': True, 'adv_address': '03B28DCD9920', 'group_id': 'FE0000', 'rssi': 54,
-                'stat_param': 44687,
+                'stat_param': 30687,
                 'time_from_start': 1.528374, 'counter_tag': 1}
     packet_2 = '03B28DCD99201EFF0005FE0000E0210FFF93B635EBFF1DB118C6D782DC2ED98C404200486436AE82'
 
     p1 = Packet(packet_1)
 
     print(p1.get_packet_content('03B28DCD99201EFF0005FE0000E0210FFF93B635EBFF1DB118C6D782DC2ED98C404200486436AE82', get_gw_data=True),)
```

### Comparing `wiliot-core-5.4.3/wiliot_core/packet_data/packet_list.py` & `wiliot-core-5.5.8/wiliot_core/packet_data/packet_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,20 +56,21 @@
 #     CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE);
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
 import logging
 
 import numpy as np
-import pandas
 import pandas as pd
 import copy
+import inspect
 
 from wiliot_core.packet_data.packet import Packet, InlayTypes
-from wiliot_core.packet_data.config_files.packet_map import packet_length_types
+from wiliot_core.packet_data.config_files.packet_map import packet_length_types, convert_cloud_to_packet
+from wiliot_core.packet_data.config_files.stat_calculation import StatisticsCalc
 
 
 class PacketList(list):
     def __init__(self, packet_obj_type=Packet, packet_list_obj_type=None, list_custom_data=None, logger_name=None):
         """
         :param packet_obj_type:
         :param packet_list_obj_type:
@@ -185,37 +186,37 @@
         Total amount of packets, sprinklers count individually
         """
         packet_list_size = 0
         for packet in self.packet_list:
             packet_list_size += len(packet)
         return packet_list_size
 
-    def append(self, packet: Packet, ignore_sprinkler=False):
+    def append(self, packet: Packet, ignore_sprinkler=False, sort_by_time=False):
         """
         Adds single Packet to PacketList
 
         :type packet: Packet
         :param packet: packet to be added to packet_list
         :type ignore_sprinkler: Bool
         :param ignore_sprinkler: allow duplicates packets from different sprinkler
+        :type sort_by_time: bool
+        :param sort_by_time: if true append to sprinkler based on the time from start
 
         :return: packet_list
         """
         if packet.is_valid_packet:
             self.is_df_changed = True
             raw_packet = packet.get_packet()
-            if packet.packet_data['test_mode'] and packet.packet_data['ble_type'] != 'LEGACY':
-                raw_packet = raw_packet[0:20] + raw_packet[24:]
             if raw_packet not in self.raw_packet_map_list.keys():
                 self.packet_list = np.append(self.packet_list, packet)
                 raw_packet_list_index = self.packet_list.size - 1
                 self.raw_packet_map_list[raw_packet] = raw_packet_list_index
             else:
                 raw_packet_list_index = self.raw_packet_map_list[raw_packet]
-                self.packet_list[raw_packet_list_index].append_to_sprinkler(packet)
+                self.packet_list[raw_packet_list_index].append_to_sprinkler(packet=packet, do_sort=sort_by_time)
 
     def get_sprinkler(self, packet):
         """
         @param packet: a packet data type. Needs to be appended before using this function.
         @return: A packet sprinkler of this packet.
         """
         raw_packet = packet.get_packet()
@@ -324,15 +325,15 @@
         :return: Dataframe - sprinkler_df
         """
         packet_list = self.import_packet_df(packet_df=packet_df)
         sprinkler_df = packet_list.get_df(sprinkler_filter=True, add_sprinkler_info=True)
 
         return sprinkler_df
 
-    def sort_df_by(self, column='stat_param'):
+    def sort_df_by(self, column='gw_clock'):
         """
         returns dataframe sorted by column
         :type column: str
         :param column: the column to filter by
 
         :return: Dataframe
         """
@@ -433,27 +434,30 @@
         if len(tbp_list) == 0:
             return None
         avg_tbp = round(tbp_list.mean(), 4)
         if ignore_outliers:
             avg_tbp = round(reject_outliers(tbp_list).mean(), 4)
         return avg_tbp
 
-    def to_csv(self, path, append=False, export_packet_id=True, columns=None, add_sprinkler_info=False):
+    def to_csv(self, path, append=False, export_packet_id=True, columns=None, add_sprinkler_info=False,
+               is_overwrite=False):
         """
         export entire PacketList to csv
 
         :type path: str
         :param path: path to save csv
         :type append: bool
         :param append: to append the df to an existing csv file
 
         :return: bool - export status
         """
 
-        return self.export_packet_df(packet_df=self.get_df(add_sprinkler_info=add_sprinkler_info), path=path,
+        return self.export_packet_df(packet_df=self.get_df(add_sprinkler_info=add_sprinkler_info,
+                                                           is_overwrite=is_overwrite),
+                                     path=path,
                                      append=append,
                                      export_packet_id=export_packet_id, columns=columns)
 
     def export_packet_df(self, packet_df, path, append=False, export_packet_id=True, columns=None):
         """
         export given dataframe to csv
 
@@ -476,14 +480,19 @@
             else:
                 packet_df.to_csv(path, index=False, columns=columns)
             return True
         except Exception as e:
 
             raise Exception('problem during export packet df {}'.format(e))
 
+    def packet_string_to_object(self, packet_in, time_from_start, configs=None, custom_data=None, inlay_type=None):
+        packet_obj = Packet(packet_in, float(time_from_start), custom_data=custom_data, inlay_type=inlay_type,
+                            logger_name=self.logger.name if self.logger is not None else None)
+        return packet_obj
+
     def import_packet_df(self, path=None, packet_df=None, custom_data_attr=None, import_all=False,
                          list_custom_data=None, verbose=True, inlay_type=None):
         """
         import from a csv of dataframe
         :type path: str
         :param path: the message or part of the message that needed to be read
         :type packet_df: DataFrame
@@ -519,53 +528,69 @@
                         reconstructed_packet = str(raw_packet) + str(gw_data)
                 elif 'encryptedPacket' in row.keys():
                     reconstructed_packet = row['encryptedPacket']
                 elif 'decrypted_full_packet' in row.keys():
                     reconstructed_packet = row['decrypted_full_packet']
                 elif 'encrypted_packet' in row.keys():
                     reconstructed_packet = row['encrypted_packet']
+                elif 'rawPacket' in row.keys() and 'packetVersion' in row.keys():
+                    cloud_packet = row['rawPacket']
+                    reconstructed_packet = convert_cloud_to_packet(cloud_packet=cloud_packet)
+                    if reconstructed_packet == cloud_packet:
+                        non_packets_rows.append(index)
+                        continue
                 else:
-                    non_packets_rows.append(index)
-                    continue
+                    raise Exception('dataframe/file must contains one of the following columns conventions:\n'
+                                    '1. raw_packet AND gw_packet\n'
+                                    '2. encryptedPacket\n'
+                                    '3. decrypted_full_packet\n'
+                                    '4. encrypted_packet\n'
+                                    '5. rawPacket AND packetVersion\n')
                 if reconstructed_packet == '' or pd.isnull(reconstructed_packet):
                     non_packets_rows.append(index)
                     continue
             except Exception as e:
                 non_packets_rows.append(index)
                 continue
 
             if 'time_from_start' in row.keys():
                 time_from_start = row['time_from_start']
             elif 'time' in row.keys():
                 time_from_start = row['time']
             else:
                 time_from_start = float('nan')
-            if time_from_start == '' or time_from_start is None:
+
+            try:
+                time_from_start = float(time_from_start)
+            except ValueError:
                 time_from_start = float('nan')
 
             # adding custom data
             custom_data = {}
             if import_all:
                 try:
-                    p_tmp = self.packet_obj_type(reconstructed_packet, float(time_from_start),
-                                                 logger_name=self.logger.name if self.logger is not None else None)
+                    p_tmp = self.packet_string_to_object(packet_in=reconstructed_packet,
+                                                         time_from_start=time_from_start,
+                                                         configs=row)
                     static_keys_list = p_tmp.get_packet_data_names()
                     for k in row.keys():
                         if k not in static_keys_list and k != 'packet_id':
                             custom_data[k] = row[k]
                 except Exception as e:
                     self.printing_and_logging('exception raised during extracting custom data in import df: {}'.format(e))
             elif custom_data_attr is not None:
                 for k in custom_data_attr:
                     if k in row.keys():
                         custom_data[k] = row[k]
             try:
-                p = self.packet_obj_type(reconstructed_packet, float(time_from_start), custom_data=custom_data,
-                                         inlay_type=inlay_type,
-                                         logger_name=self.logger.name if self.logger is not None else None)
+                p = self.packet_string_to_object(packet_in=reconstructed_packet,
+                                                 time_from_start=time_from_start,
+                                                 configs=row,
+                                                 custom_data=custom_data,
+                                                 inlay_type=inlay_type)
                 import_packet_list.append(p)
             except Exception as e:
                 self.printing_and_logging('exception raised during import df: {}'.format(e))
 
         if len(non_packets_rows) and verbose:
             self.printing_and_logging('the following {} rows could not be imported '
                                       'to the packet list:{}'.format(len(non_packets_rows), non_packets_rows))
@@ -613,18 +638,19 @@
 
     def get_num_packets(self):
         """
         Total amount of packets, sprinklers packets count separately
         """
         return len(self.packet_list)
 
-    def get_df_statistics(self, packet_df=None):
+    def get_df_statistics(self, packet_df=None, stat_calc=StatisticsCalc):
         """
         Calculates statistics from packetList DF.
         @param packet_df - dataframe generated by packetList
+        @param stat_calc - object to calc the statistics
         @return dictionary with predefined statistics of the packetList.
         """
         statistics = {}
         if (packet_df is not None and packet_df.shape[0] == 0) or (packet_df is None and self.size() == 0):
             statistics = {'num_packets': 0, 'num_cycles': 0}
             return statistics
 
@@ -632,63 +658,58 @@
         if packet_df is None:
             packet_df = self.get_df(add_sprinkler_info=True)
         if 'sprinkler_counter' in packet_df.keys():
             sprinkler_df = packet_df[packet_df['sprinkler_counter'] == 1]
         else:
             sprinkler_df = self.packet_df_to_sprinkler_df(packet_df)
 
-        statistics['num_packets'] = packet_df.shape[0]
-        statistics['num_cycles'] = sprinkler_df.shape[0]
+        s = stat_calc(packet_df, sprinkler_df)
+        stat_attr = (getattr(s, name) for name in dir(s) if not name.startswith('_'))
+        stat_methods = [a for a in stat_attr if inspect.ismethod(a)]
+        statistics = {}
+        for method in stat_methods:
+            calc_stat = method()
+            statistics = {**statistics, **calc_stat}
 
-        sprinkler_counter_arr = pandas.to_numeric(sprinkler_df['num_packets_per_sprinkler'], errors='coerce')
-        statistics['sprinkler_counter_mean'] = np.mean(sprinkler_counter_arr)
-        statistics['sprinkler_counter_std'] = np.std(sprinkler_counter_arr)
-        statistics['sprinkler_counter_min'] = np.min(sprinkler_counter_arr)
-        statistics['sprinkler_counter_max'] = np.max(sprinkler_counter_arr)
-
-        tbp_arr = pandas.to_numeric(sprinkler_df.loc[sprinkler_df['tbp'] > 0]['tbp'], errors='coerce')
-        if len(tbp_arr) == 0:
-            tbp_arr = [-1]
-        statistics['tbp_mean'] = np.mean(tbp_arr)
-        statistics['tbp_std'] = np.std(tbp_arr)
-        statistics['tbp_min'] = np.min(tbp_arr)
-        statistics['tbp_max'] = np.max(tbp_arr)
-        statistics['tbp_num_vals'] = np.size(tbp_arr)
-
-        per_arr = pandas.to_numeric(sprinkler_df['per'], errors='coerce')
-        statistics['per_mean'] = np.mean(per_arr)
-        statistics['per_std'] = np.std(per_arr)
-
-        rssi_arr = pandas.to_numeric(packet_df['rssi'], errors='coerce')
-        statistics['rssi_mean'] = np.mean(rssi_arr)
-        statistics['rssi_std'] = np.std(rssi_arr)
-        statistics['rssi_min'] = np.min(rssi_arr)
-        statistics['rssi_max'] = np.max(rssi_arr)
-
-        time_arr = pandas.to_numeric(packet_df['time_from_start'], errors='coerce')
-        # statistics['start_time'] = np.min(time_arr)
-        statistics['ttfp'] = np.min(time_arr)
-        statistics['end_time'] = np.max(time_arr)
-        statistics['duration'] = statistics['end_time'] - statistics['ttfp']
-        if statistics['duration'] > 0:
-            statistics['rx_rate_normalized'] = statistics['num_packets'] / statistics['duration']
-            statistics['rx_rate'] = statistics['num_packets'] / statistics['end_time']
-        else:
-            statistics['rx_rate'] = 0
-            statistics['rx_rate_normalized'] = 0
         return statistics
 
     def to_tag_list(self):
         # import here to avoid infinte loop (packet_list calls tag_list and tags_list calls packet_list)
         from wiliot_core.packet_data.tag_collection import TagCollection
         tag_list = TagCollection()
         for packet in self.packet_list:
             tag_list.append(packet)
         return tag_list
 
+    def sync_packet_list(self, new_packet_list, time_sync_new, my_source_name='original', new_source_name='new',
+                         do_sort=False):
+        """
+        This function merge one packet list to the self packet list. if time_sync_list is specified it sync the data based on
+        the time sync list
+        """
+        if pd.isnull(time_sync_new):
+            raise Exception(f'cannot sync packet list due to time sync new id null: {time_sync_new}')
+
+        for p in self.packet_list:
+            p.add_custom_data({'source': my_source_name})
+
+        for p in new_packet_list:
+            p.gw_data['time_from_start'] = np.array(p.gw_data['time_from_start'] - time_sync_new)
+            p.add_custom_data({'source': new_source_name})
+            self.append(p, sort_by_time=do_sort)
+
+        if do_sort:
+            min_time_from_start = []
+            for p in self.packet_list:
+                min_time_from_start.append(np.min(p.gw_data['time_from_start']))
+
+            min_time_from_start = np.array(min_time_from_start)
+            idx = min_time_from_start.argsort()
+            self.packet_list = self.packet_list[idx]
+
     @staticmethod
     def get_generic_df_cols(ble_packet_type='LEGACY'):
         len_packet = None
         for v in packet_length_types.values():
             if v['name'].upper() == ble_packet_type.upper():
                 len_packet = v['packet_tag_length']
         if len_packet is None:
```

### Comparing `wiliot-core-5.4.3/wiliot_core/packet_data/tag_collection.py` & `wiliot-core-5.5.8/wiliot_core/packet_data/tag_collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,26 @@
 
 class TagCollection(dict):
     def __init__(self, packet_list_obj=PacketList):
         self.tags = {}  # key is adv_address, value is Packet_list
         self.metadata = {}
         self.packet_list_obj = packet_list_obj
 
+    def items(self):
+        return self.tags.items()
+
+    def keys(self):
+        return self.tags.keys()
+
+    def values(self):
+        return self.tags.values()
+
+    def __getitem__(self, key):
+        return self.tags[key]
+
     def __len__(self):
         """
         Amount of tags
         """
         return len(self.tags)
 
     def __add__(self, other_multi_tag):
@@ -188,16 +200,16 @@
         :type id: str
         :param id: adv_address or tag id of wanted tag
 
         :return: average tbp for tag
         """
         return self.tags[id].get_avg_tbp(ignore_outliers=ignore_outliers)
 
-    def to_csv(self, path, val='time_from_start', add_sprinkler_info=False):
-        multi_tag_df = self.get_df(val=val, add_sprinkler_info=add_sprinkler_info)
+    def to_csv(self, path, val='time_from_start', add_sprinkler_info=False, is_overwrite=False):
+        multi_tag_df = self.get_df(val=val, add_sprinkler_info=add_sprinkler_info, is_overwrite=is_overwrite)
         multi_tag_df.to_csv(path, index=False)
 
     def get_statistics(self, id_name='adv_address'):
         statistics_df = pd.DataFrame()
         for id in self.tags.keys():
             id_statistics = self.get_statistics_by_id(id)
             id_statistics[id_name] = id
@@ -239,15 +251,15 @@
         return packet_list
 
 
 if __name__ == '__main__':
     import os
 
     try:
-        df_path = os.path.abspath('../../internal/data_samples_for_tests/offline_tester@packets_data.csv')
+        df_path = os.path.abspath('../internal/tests/data_samples_for_tests/offline_tester@packets_data.csv')
         packet_list = PacketList()
         packet_list = packet_list.import_packet_df(path=df_path, import_all=True)
         tag_list = packet_list.to_tag_list()
         t = tag_list.get_by_index([1, 30])
-    except:
+    except Exception as e:
         pass
     print('done')
```

### Comparing `wiliot-core-5.4.3/wiliot_core/utils/get_version.py` & `wiliot-core-5.5.8/wiliot_core/utils/get_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
             ver_arr[2] = 0
             ver_arr[1] = 0
             ver_arr[0] = int(ver_arr[0]) + 1
         return f"{ver_arr[0]}.{ver_arr[1]}.{ver_arr[2]}"
 
 
 if __name__ == '__main__':
+
     num_args = len(sys.argv)
     if num_args == 1:
         type = 'current'
     else:
         type = sys.argv[1]
 
     __version__ = get_version(type)
```

### Comparing `wiliot-core-5.4.3/wiliot_core/utils/release_for_partners.py` & `wiliot-core-5.5.8/wiliot_core/utils/release_for_partners.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core/utils/update_wiliot_packages.py` & `wiliot-core-5.5.8/wiliot_core/utils/update_wiliot_packages.py`

 * *Files 18% similar despite different names*

```diff
@@ -59,42 +59,48 @@
 #  """
 
 import shutil
 from os import popen
 from os.path import join, isdir
 from sys import platform
 from enum import Enum
+import os
+import json
+import PySimpleGUI as sg
+from tkinter import messagebox
 
 
 class WiliotPackages(Enum):
     CLOUD = ['pywiliot-api']
     CORE = ['pywiliot-core', 'pywiliot-api']
     TOOLS = ['pywiliot-tools', 'pywiliot-core', 'pywiliot-api']
     DEPLOYMENT = ['pywiliot-deployment-tools', 'pywiliot-tools', 'pywiliot-core', 'pywiliot-api']
     TESTERS = ['pywiliot-testers', 'pywiliot-tools', 'pywiliot-core', 'pywiliot-api']
 
 
 def update_internal_wiliot_packages(wiliot_repo=WiliotPackages.CLOUD, branch_name='master',
                                     overwrite=False, no_wiliot_dep=False,
                                     username_bitbucket=None, password_bitbucket=None,
-                                    install_from_local_folder='', branch_name_for_dep='master'):
+                                    install_from_local_folder='', install_from_git_folder='',
+                                    branch_name_for_dep='master'):
     # check platform command prefix
     python_ver = ''
     if platform == "darwin" or platform == 'linux':
         # macos or linux
         python_ver = '3'
     # install pywiliot and requirements:
     # update dependencies
     print("----------------------------------\nupdate pip:\n----------------------------------")
     p = popen(f'python{python_ver} -m pip install --upgrade pip')
     rsp = p.read()
     print(rsp)
     pkg_versions = []
     req_status = []
     for repo_num, repo_name in enumerate(wiliot_repo.value):
+        need_to_install = True
         package_name = repo_name.replace('py', '')
         folder_name = package_name.replace('-', '_')
         print('check if package already exist')
         p = popen(f'pip{python_ver} show {package_name}')
         rsp = p.read()
         print(rsp)
         if package_name in rsp:
@@ -109,72 +115,80 @@
                       f'--------------------------------------------------------------------\n')
                 p = popen(f'pip{python_ver} uninstall {package_name}')
             rsp = p.read()
             print(rsp)
         print(f'--------------------------------------------------------------------\n'
               f'update wiliot package: {package_name}\n'
               f'--------------------------------------------------------------------')
-        if install_from_local_folder:
-            local_repo_path = join(install_from_local_folder, repo_name)
-            if not isdir(local_repo_path):
-                print(f'{repo_name} does not exist in local folder, skip installation')
-                pkg_versions.append('')
-                req_status.append(False)
-                continue
-            p = popen(f'pip{python_ver} install -e {local_repo_path}')
-            rsp = p.read()
-            print(rsp)
-        elif username_bitbucket is None and password_bitbucket is None:
-            if repo_num == 0:
-                p = popen(f'pip{python_ver} install git+ssh://git@bitbucket.org/wiliot/{repo_name}.git'
-                          f'@{branch_name}#egg={folder_name} --upgrade')
+        if install_from_local_folder or install_from_git_folder:
+            local_repo_path = join(install_from_local_folder if install_from_local_folder else install_from_git_folder,
+                                   repo_name)
+            if isdir(local_repo_path):
+                p = popen(f'pip{python_ver} install -e {local_repo_path}  --upgrade')
+                rsp = p.read()
+                print(rsp)
+                need_to_install = False
             else:
-                p = popen(f'pip{python_ver} install git+ssh://git@bitbucket.org/wiliot/{repo_name}.git'
-                          f'@{branch_name_for_dep}#egg={folder_name} --upgrade')
-            rsp = p.read()
-            print(rsp)
-            if 'Successfully installed' not in rsp.split('\n')[-2]:
-                print(f'problem with ssh key credentials. Please rerun the script using username (-u) and password (-p).'
-                      f'\nTo extract Attlasian username and password go to '
-                      f'https://wiliot.atlassian.net/wiki/spaces/SW/pages/2890662124/'
-                      f'PyWiliot+Installation+Guidelines+-+Private#using-username-and-password%3A')
-                return
-        elif username_bitbucket is not None and password_bitbucket is not None:
-            if repo_num == 0:
-                p = popen(f'pip{python_ver} install git+https://{username_bitbucket}:{password_bitbucket}@bitbucket.org'
-                          f'/wiliot/{repo_name}.git@{branch_name}#egg={folder_name} --upgrade')
+                print(f'{repo_name} does not exist in local folder, try to install from bitbucket')
+
+        if need_to_install:
+            if username_bitbucket is None and password_bitbucket is None:
+                if repo_num == 0:
+                    p = popen(f'pip{python_ver} install git+ssh://git@bitbucket.org/wiliot/{repo_name}.git'
+                              f'@{branch_name}#egg={folder_name} --upgrade')
+                else:
+                    p = popen(f'pip{python_ver} install git+ssh://git@bitbucket.org/wiliot/{repo_name}.git'
+                              f'@{branch_name_for_dep}#egg={folder_name} --upgrade')
+                rsp = p.read()
+                print(rsp)
+                if 'Successfully installed' not in rsp.split('\n')[-2]:
+                    print(
+                        f'problem with ssh key credentials. Please rerun the script using username (-u) and password (-p).'
+                        f'\nTo extract Attlasian username and password go to '
+                        f'https://wiliot.atlassian.net/wiki/spaces/SW/pages/2890662124/'
+                        f'PyWiliot+Installation+Guidelines+-+Private#using-username-and-password%3A')
+                    return
+            elif username_bitbucket is not None and password_bitbucket is not None:
+                if repo_num == 0:
+                    p = popen(
+                        f'pip{python_ver} install git+https://{username_bitbucket}:{password_bitbucket}@bitbucket.org'
+                        f'/wiliot/{repo_name}.git@{branch_name}#egg={folder_name} --upgrade')
+                else:
+                    p = popen(
+                        f'pip{python_ver} install git+https://{username_bitbucket}:{password_bitbucket}@bitbucket.org'
+                        f'/wiliot/{repo_name}.git@{branch_name_for_dep}#egg={folder_name} --upgrade')
+                rsp = p.read()
+                print(rsp)
             else:
-                p = popen(f'pip{python_ver} install git+https://{username_bitbucket}:{password_bitbucket}@bitbucket.org'
-                          f'/wiliot/{repo_name}.git#egg={folder_name} --upgrade')
-            rsp = p.read()
-            print(rsp)
-        else:
-            print('you Must specified both username and password or do NOT specified neither '
-                  'for installation using SSH key')
-            return
+                print('you Must specified both username and password or do NOT specified neither '
+                      'for installation using SSH key')
+                return
 
         print(f'check wiliot package: {package_name}')
         p = popen(f'pip{python_ver} show {package_name}')
         rsp = p.read()
         print(rsp)
         if 'Location' in rsp:
             pkg_versions.append(rsp.split('Version: ')[1].split('\n')[0])
             req_path = rsp.split('Location: ')[-1].split('\n')[0]
-            if install_from_local_folder:
+            if install_from_git_folder:
+                if 'Editable project location: ' in rsp:
+                    req_path = rsp.split('Editable project location: ')[-1].split('\n')[0]
+            elif install_from_local_folder:
                 site_packages_path = join(req_path, folder_name)
                 if isdir(site_packages_path):
                     shutil.rmtree(site_packages_path)
                 shutil.copytree(join(install_from_local_folder, repo_name, folder_name), site_packages_path)
                 req_path = join(install_from_local_folder, repo_name)
 
             print("--------------------------------------------------------------------\n"
                   "update dependencies:\n"
                   "--------------------------------------------------------------------")
             requirements_path = join(req_path, folder_name, 'requirements.txt')
-            p = popen(f'pip{python_ver} install -r {requirements_path}')
+            p = popen(f'pip{python_ver} install -r "{requirements_path}"')
             rsp = p.read()
             print(rsp)
             req_status.append('ERROR' not in rsp)
         else:
             pkg_versions.append('')
             req_status.append(False)
 
@@ -191,55 +205,172 @@
         sum_str = f'{package_name} was {is_installed}'
         if is_installed:
             req_is_installed = 'installed' if req_status[i] else 'NOT installed'
             sum_str += f'and the dependencies were {req_is_installed}'
         print(sum_str)
         if no_wiliot_dep:
             break
+def simple_gui():
+    background_color = '#78ebff'  # Light blue color, for example
+    text_color = '#3a3c3c'  # White color for text for good contrast
+    input_background_color = '#ffffff'  # Light input fields to stand out on the darker background
+    button_color = ('#ffffff', '#0073e6')  # Text, Background
+
+    custom_theme = {
+        'BACKGROUND': background_color,
+        'TEXT': text_color,
+        'INPUT': input_background_color,
+        'TEXT_INPUT': None,  # Default text color for input fields
+        'SCROLL': None,  # Default scroll color
+        'BUTTON': (text_color, background_color),
+        'PROGRESS': None,  # Default progress bar color
+        'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
+    }
+
+    sg.LOOK_AND_FEEL_TABLE['wiliotTheme'] = custom_theme
+
+    sg.theme('wiliotTheme')
+
+    wiliot_folder = os.path.join(os.getenv('LOCALAPPDATA'), 'wiliot', "update_wiliot_packages")
+    if not os.path.exists(wiliot_folder):
+        os.makedirs(wiliot_folder, exist_ok=True)
+
+    credentials_file = os.path.join(wiliot_folder, "user_config.json")
+    if os.path.isfile(credentials_file):
+        if os.path.getsize(credentials_file) > 0:
+            try:
+                with open(credentials_file, 'r') as file:
+                    json_data = json.load(file)
+                    bitbucket_username = json_data.get('bitbucket_username', '')
+                    bitbucket_password = json_data.get('bitbucket_password', '')
+                    print("Username and password loaded successfully.")
+            except json.JSONDecodeError:
+                print("JSON file is empty or corrupt.")
+                bitbucket_username = None
+                bitbucket_password = None
+        else:
+            bitbucket_username = ''
+            bitbucket_password = ''
+            with open(credentials_file, 'w') as file:
+                json.dump({'bitbucket_username': bitbucket_username, 'bitbucket_password': bitbucket_password}, file)
+    else:
+        bitbucket_username = None
+        bitbucket_password = None
+        with open(credentials_file, 'w') as file:
+            json.dump({'bitbucket_username': bitbucket_username, 'bitbucket_password': bitbucket_password}, file)
+
+    package_dict = {package.value[0]: package.name for package in WiliotPackages}
+
+    package_names = list(package_dict.keys())
+
+    # Define the layout
+    layout = [
+        [sg.Text('Select a package:')],
+        [sg.DropDown(package_names, default_value='pywiliot-tools', key='-PACKAGE_DROPDOWN-', size=(20, 1))],
+        [sg.Text('Branch:'), sg.InputText(default_text='master', key='-BRANCH_TEXT-', size=(10, 1))],
+        [sg.Text('Bitbucket Username:'), sg.InputText(default_text=bitbucket_username, key='-BITBUCKET_USERNAME-',
+                                                      size=(20, 1))],
+        [sg.Text('Bitbucket Password:'), sg.InputText(default_text=bitbucket_password, key='-BITBUCKET_PASSWORD-'
+                                                      , password_char='*', size=(20, 1))],
+        [sg.Checkbox(text="Overwrite installed files?", default=True, key='-OVERWRITE-')],
+        [sg.Checkbox(text="Install package without wiliot dependencies", default=False, key='-wiliot_DEP-')],
+
+        [sg.Button('OK'), sg.Button('Cancel')]
+
+    ]
+
+    window = sg.Window('wiliot package updater', layout)
+
+    while True:
+        event, values = window.read()
+        if event == sg.WINDOW_CLOSED or event == 'Cancel':
+            break
+        elif event == 'OK':
+            window.close()
+            selected_package_name = values['-PACKAGE_DROPDOWN-']
+            selected_package_enum = package_dict[selected_package_name]
+            selected_branch = values['-BRANCH_TEXT-']
+            bitbucket_username = values['-BITBUCKET_USERNAME-']
+            bitbucket_password = values['-BITBUCKET_PASSWORD-']
+
+            if selected_branch != "develop":
+                dep_branch = "master"
+            else:
+                dep_branch = "develop"
+            json_data['bitbucket_username'] = bitbucket_username
+            json_data['bitbucket_password'] = bitbucket_password
+            with open(credentials_file, 'w') as file:
+                json.dump(json_data, file)
+
+            update_internal_wiliot_packages(
+                wiliot_repo=WiliotPackages[selected_package_enum],
+                branch_name=selected_branch,
+                username_bitbucket=bitbucket_username,
+                password_bitbucket=bitbucket_password,
+                overwrite=values['-OVERWRITE-'],
+                no_wiliot_dep=values['-wiliot_DEP-'],
+                branch_name_for_dep=dep_branch
+
+
+            )
+            messagebox.showinfo("wiliot package updater", "wiliot package updated successfully!")
+
+    window.close()
+
 
 
 if __name__ == '__main__':
     import argparse
+
     parser = argparse.ArgumentParser(description='Update Wiliot Internal Packages')
     parser.add_argument('-p', '--package_name', help='The package name. valid option(wiliot-api, wiliot-core, '
                                                      'wiliot-tools, wiliot-testers, wiliot-deployment-tools')
     parser.add_argument('-b', '--branch_name', help='The branch name you want to use. the default is master',
                         default='master')
     parser.add_argument('-w', '--overwrite', help='If specified, all wiliot existed packages will be overwrite '
                                                   'with the new installation', default=False, action='store_true')
     parser.add_argument('-n', '--no_wiliot_dep', help='If specified, install the main package without wiliot '
                                                       'dependencies packages', default=False, action='store_true')
     parser.add_argument('-u', '--username', help='If specified, install based username and password and not SHH key',
                         default=None)
     parser.add_argument('-pass', '--password', help='If specified, install based username and password and not SHH key',
                         default=None)
     parser.add_argument('-l', '--local_folder', help='If specified, install packages from the specified local folder')
+    parser.add_argument('-g', '--git_folder', help='FOR DEVELOPERS. If specified, install packages from the specified'
+                                                   'folder, which assumed to be your git workspace')
     parser.add_argument('-b-for-dep', '--branch_for_dependencies',
                         help='if specified, all wiliot package dependencies will be installed for this branch '
                              '(default master)', default='master')
     args = parser.parse_args()
     package_name = args.package_name
     branch_name = args.branch_name
     is_overwrite = args.overwrite
     is_no_wiliot_dep = args.no_wiliot_dep
     username = args.username
     password = args.password
     local_folder = args.local_folder
+    git_folder = args.git_folder
     branch_for_dep = args.branch_for_dependencies
     err_msg = 'please add package name, e.g. update_wiliot_packages.py -p wiliot-api.\n' \
               'The valid packages names are: wiliot-api, wiliot-core, wiliot-tools, wiliot-testers, ' \
               'wiliot-deployment-tools'
-    try:
-        repo_name = None
-        for package in WiliotPackages.__members__.values():
-            if package_name in package.value[0]:
-                repo_name = package
-                break
-        if repo_name is None:
-            print(err_msg)
-        else:
-            update_internal_wiliot_packages(wiliot_repo=repo_name, branch_name=branch_name,
-                                            overwrite=is_overwrite, no_wiliot_dep=is_no_wiliot_dep,
-                                            username_bitbucket=username, password_bitbucket=password,
-                                            install_from_local_folder=local_folder, branch_name_for_dep=branch_for_dep)
-    except Exception as e:
-        print('Error during update packages  [ERROR: {}]'.format(e))
+    if package_name != None:
+        try:
+            repo_name = None
+            for package in WiliotPackages.__members__.values():
+                if package_name in package.value[0]:
+                    repo_name = package
+                    break
+            if repo_name is None:
+                print(err_msg)
+            else:
+                update_internal_wiliot_packages(wiliot_repo=repo_name, branch_name=branch_name,
+                                                overwrite=is_overwrite, no_wiliot_dep=is_no_wiliot_dep,
+                                                username_bitbucket=username, password_bitbucket=password,
+                                                install_from_local_folder=local_folder,
+                                                install_from_git_folder=git_folder,
+                                                branch_name_for_dep=branch_for_dep)
+        except Exception as e:
+            print('Error during update packages  [ERROR: {}]'.format(e))
+
+    else:
+        simple_gui()
```

### Comparing `wiliot-core-5.4.3/wiliot_core/utils/utils.py` & `wiliot-core-5.5.8/wiliot_core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-5.4.3/wiliot_core.egg-info/PKG-INFO` & `wiliot-core-5.5.8/wiliot_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-core
-Version: 5.4.3
+Version: 5.5.8
 Summary: A library for interacting with Wiliot's private core functions
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -57,14 +57,30 @@
 * [packet data](wiliot_core/packet_data) (at the end of each script)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 5.5.8:
+-----------------
+* update requirements
+* gateway core:
+  * add support to listen to two or more gw and merge data
+  * support auto time reset based on GW msg
+  * added support to connect to gw based on its name/uid
+  * added wrapper to get all gw responses similar to get packets
+  * added function of reconnect
+  * added function to control output signal (GPIO) from the GW
+  * added new firmware version
+* packets data core:
+  * support packets from cloud (payload)
+  * added new packet fields - gw clock, crc, adi (relevant to ble5 only) - effective only for the new firmware version
+  * add function to manipulate packets
+  
 Version 5.4.3:
 -----------------
 * gateway core:
   * Added new firmware version to local gateway
   * added the option to restart the gateway time based on command and control the log for buffer overload
 * packets data core:
   * Support Gen3 wiliot tags - tbp, per calculation
```

### Comparing `wiliot-core-5.4.3/wiliot_core.egg-info/SOURCES.txt` & `wiliot-core-5.5.8/wiliot_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 wiliot_core.egg-info/requires.txt
 wiliot_core.egg-info/top_level.txt
 wiliot_core/local_gateway/__init__.py
 wiliot_core/local_gateway/continuous_listener.py
 wiliot_core/local_gateway/custom_energy_pattern.py
 wiliot_core/local_gateway/local_gateway_core.py
 wiliot_core/local_gateway/examples/__init__.py
+wiliot_core/local_gateway/examples/dual_gw_example.py
 wiliot_core/local_gateway/examples/local_gateway_basic_example.py
 wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip
 wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip
 wiliot_core/local_gateway/local_gateway_versions/4.0.16_app.zip
 wiliot_core/local_gateway/local_gateway_versions/4.0.16_sd_bl_gw_app.zip
 wiliot_core/local_gateway/local_gateway_versions/4.0.18_app.zip
 wiliot_core/local_gateway/local_gateway_versions/4.0.18_sd_bl_gw_app.zip
@@ -31,26 +32,30 @@
 wiliot_core/local_gateway/local_gateway_versions/4.0.19_sd_bl_gw_app.zip
 wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip
 wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip
 wiliot_core/local_gateway/local_gateway_versions/4.1.4_app.zip
 wiliot_core/local_gateway/local_gateway_versions/4.1.4_sd_bl_gw_app.zip
 wiliot_core/local_gateway/local_gateway_versions/4.2.0_app.zip
 wiliot_core/local_gateway/local_gateway_versions/4.2.0_sd_bl_gw_app.zip
+wiliot_core/local_gateway/local_gateway_versions/4.3.3_app.zip
+wiliot_core/local_gateway/local_gateway_versions/4.3.3_sd_bl_gw_app.zip
 wiliot_core/local_gateway/local_gateway_versions/__init__.py
 wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex
 wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.18.hex
 wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.19.hex
 wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex
 wiliot_core/local_gateway/local_gateway_versions/wifi_4.1.4.hex
 wiliot_core/local_gateway/local_gateway_versions/wifi_4.2.0.hex
+wiliot_core/local_gateway/local_gateway_versions/wifi_4.3.3.hex
 wiliot_core/packet_data/__init__.py
 wiliot_core/packet_data/packet.py
 wiliot_core/packet_data/packet_list.py
 wiliot_core/packet_data/tag_collection.py
 wiliot_core/packet_data/config_files/__init__.py
 wiliot_core/packet_data/config_files/packet_flow_parameters.py
 wiliot_core/packet_data/config_files/packet_map.py
+wiliot_core/packet_data/config_files/stat_calculation.py
 wiliot_core/utils/__init__.py
 wiliot_core/utils/get_version.py
 wiliot_core/utils/release_for_partners.py
 wiliot_core/utils/update_wiliot_packages.py
 wiliot_core/utils/utils.py
```

