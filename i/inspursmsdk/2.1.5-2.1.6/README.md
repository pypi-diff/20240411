# Comparing `tmp/inspursmsdk-2.1.5.tar.gz` & `tmp/inspursmsdk-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inspursmsdk-2.1.5.tar", last modified: Mon Oct  9 03:26:54 2023, max compression
+gzip compressed data, was "dist/inspursmsdk-2.1.6.tar", last modified: Thu Apr 11 02:29:18 2024, max compression
```

## Comparing `inspursmsdk-2.1.5.tar` & `inspursmsdk-2.1.6.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 03:26:54.000000 inspursmsdk-2.1.5/
--rw-r--r--   0 root         (0) root         (0)      991 2023-10-09 03:23:12.000000 inspursmsdk-2.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      888 2023-10-09 03:26:54.000000 inspursmsdk-2.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      222 2023-10-09 03:23:12.000000 inspursmsdk-2.1.5/README.md
--rw-r--r--   0 root         (0) root         (0)       20 2023-10-09 03:23:11.000000 inspursmsdk-2.1.5/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 03:26:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-09 03:22:53.000000 inspursmsdk-2.1.5/inspur_sm_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 03:26:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/
--rw-r--r--   0 root         (0) root         (0)    49818 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/IpmiFunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 03:26:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/biosPostEventStr.py
--rw-r--r--   0 root         (0) root         (0)    16391 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/commonInfoStr.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/eventLogString.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/sensorEventStr.py
--rw-r--r--   0 root         (0) root         (0)    51098 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py
--rw-r--r--   0 root         (0) root         (0)     5698 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/showSensorDesc.py
--rw-r--r--   0 root         (0) root         (0)    21216 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/RedfishFunc.py
--rw-r--r--   0 root         (0) root         (0)   300270 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/RestFunc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12152 2023-10-09 03:22:57.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/backup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 03:26:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/
--rw-r--r--   0 root         (0) root         (0)    44672 2023-10-09 03:22:57.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/A7.xml
--rw-r--r--   0 root         (0) root         (0)    18131 2023-10-09 03:22:57.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/M4.xml
--rw-r--r--   0 root         (0) root         (0)    54444 2023-10-09 03:22:57.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/M5.xml
--rw-r--r--   0 root         (0) root         (0)    84520 2023-10-09 03:22:57.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/M6-N.xml
--rw-r--r--   0 root         (0) root         (0)    81800 2023-10-09 03:22:57.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/M6.xml
--rw-r--r--   0 root         (0) root         (0)    46178 2023-10-09 03:22:57.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/M7.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2023-10-09 03:22:57.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/NF3180A6.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2023-10-09 03:22:57.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/NF3280A6.xml
--rw-r--r--   0 root         (0) root         (0)   360127 2023-10-09 03:22:57.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/NF5180M5.xml
--rw-r--r--   0 root         (0) root         (0)   360210 2023-10-09 03:22:57.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/NF5280M5.xml
--rw-r--r--   0 root         (0) root         (0)    36922 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/NF5468A5.xml
--rw-r--r--   0 root         (0) root         (0)    29961 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/NF5488A5.xml
--rw-r--r--   0 root         (0) root         (0)   360290 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/SA5112M5.xml
--rw-r--r--   0 root         (0) root         (0)   360210 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/SA5212M5.xml
--rw-r--r--   0 root         (0) root         (0)    66019 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/command/restore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 03:26:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/conf/
--rw-r--r--   0 root         (0) root         (0)     1613 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/conf/NF5180M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/conf/NF5280M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/conf/SA5112M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-10-09 03:22:56.000000 inspursmsdk-2.1.5/inspur_sm_sdk/conf/SA5212M5.yml
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/conf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 03:26:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/
--rw-r--r--   0 root         (0) root         (0)    44318 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/Base.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonA5.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonA6.py
--rw-r--r--   0 root         (0) root         (0)     6333 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonA7.py
--rw-r--r--   0 root         (0) root         (0)      316 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonA7_11308.py
--rw-r--r--   0 root         (0) root         (0)   744218 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonM5.py
--rw-r--r--   0 root         (0) root         (0)   604752 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonM6.py
--rw-r--r--   0 root         (0) root         (0)    18029 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonM6_41401.py
--rw-r--r--   0 root         (0) root         (0)    16476 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonM6_4140a.py
--rw-r--r--   0 root         (0) root         (0)   288628 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonM7.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonM7_13505.py
--rw-r--r--   0 root         (0) root         (0)    45791 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/I24M6.py
--rw-r--r--   0 root         (0) root         (0)     8558 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/IBase.py
--rw-r--r--   0 root         (0) root         (0)    14826 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/NF5180M5.py
--rw-r--r--   0 root         (0) root         (0)      339 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/NF5180M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    15217 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/NF5280M5.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/NF5280M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    59696 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/NF5280M5_435.py
--rw-r--r--   0 root         (0) root         (0)     2193 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/NF5280M5_436.py
--rw-r--r--   0 root         (0) root         (0)    47115 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/NS5160M6.py
--rw-r--r--   0 root         (0) root         (0)   122296 2023-10-09 03:22:55.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/ResEntity.py
--rw-r--r--   0 root         (0) root         (0)      512 2023-10-09 03:22:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/SA5212M5Impl.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-09 03:22:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 03:26:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/route/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-09 03:22:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/route/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4904 2023-10-09 03:22:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/route/route.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 03:26:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/util/
--rw-r--r--   0 root         (0) root         (0)     4718 2023-10-09 03:22:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/util/HostTypeJudge.py
--rw-r--r--   0 root         (0) root         (0)     4788 2023-10-09 03:22:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/util/RedfishClient.py
--rw-r--r--   0 root         (0) root         (0)    10339 2023-10-09 03:22:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/util/RegularCheckUtil.py
--rw-r--r--   0 root         (0) root         (0)     7686 2023-10-09 03:22:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/util/RequestClient.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-09 03:22:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7550 2023-10-09 03:22:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/util/configUtil.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-10-09 03:22:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/util/fileUtil.py
--rw-r--r--   0 root         (0) root         (0)     7590 2023-10-09 03:22:54.000000 inspursmsdk-2.1.5/inspur_sm_sdk/util/parameterConversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 03:26:54.000000 inspursmsdk-2.1.5/inspursmsdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      888 2023-10-09 03:26:53.000000 inspursmsdk-2.1.5/inspursmsdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2682 2023-10-09 03:26:53.000000 inspursmsdk-2.1.5/inspursmsdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-09 03:26:53.000000 inspursmsdk-2.1.5/inspursmsdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-10-09 03:26:53.000000 inspursmsdk-2.1.5/inspursmsdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-10-09 03:26:53.000000 inspursmsdk-2.1.5/inspursmsdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5216 2023-10-09 03:23:12.000000 inspursmsdk-2.1.5/ism.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-09 03:26:54.000000 inspursmsdk-2.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2023-10-09 03:23:12.000000 inspursmsdk-2.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/
+-rw-r--r--   0 root         (0) root         (0)      991 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      896 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      230 2024-04-11 02:26:45.000000 inspursmsdk-2.1.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-11 02:26:45.000000 inspursmsdk-2.1.6/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/
+-rw-r--r--   0 root         (0) root         (0)    49818 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/IpmiFunc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/biosPostEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    16391 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/commonInfoStr.py
+-rw-r--r--   0 root         (0) root         (0)      693 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/eventLogString.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/sensorEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    51098 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py
+-rw-r--r--   0 root         (0) root         (0)     5698 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/showSensorDesc.py
+-rw-r--r--   0 root         (0) root         (0)    21216 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/RedfishFunc.py
+-rw-r--r--   0 root         (0) root         (0)   300270 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/RestFunc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12152 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/backup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/
+-rw-r--r--   0 root         (0) root         (0)    44672 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/A7.xml
+-rw-r--r--   0 root         (0) root         (0)    18131 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M4.xml
+-rw-r--r--   0 root         (0) root         (0)    54444 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M5.xml
+-rw-r--r--   0 root         (0) root         (0)    84520 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M6-N.xml
+-rw-r--r--   0 root         (0) root         (0)    81800 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M6.xml
+-rw-r--r--   0 root         (0) root         (0)    46178 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M7.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF3180A6.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF3280A6.xml
+-rw-r--r--   0 root         (0) root         (0)   360127 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5180M5.xml
+-rw-r--r--   0 root         (0) root         (0)   360210 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5280M5.xml
+-rw-r--r--   0 root         (0) root         (0)    36922 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5468A5.xml
+-rw-r--r--   0 root         (0) root         (0)    29961 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5488A5.xml
+-rw-r--r--   0 root         (0) root         (0)   360290 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/SA5112M5.xml
+-rw-r--r--   0 root         (0) root         (0)   360210 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/SA5212M5.xml
+-rw-r--r--   0 root         (0) root         (0)    66019 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/restore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/conf/
+-rw-r--r--   0 root         (0) root         (0)     1613 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/conf/NF5180M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/conf/NF5280M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/conf/SA5112M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/conf/SA5212M5.yml
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/conf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/
+-rw-r--r--   0 root         (0) root         (0)    44318 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/Base.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA5.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA6.py
+-rw-r--r--   0 root         (0) root         (0)     6333 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA7.py
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA7_11308.py
+-rw-r--r--   0 root         (0) root         (0)   744218 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM5.py
+-rw-r--r--   0 root         (0) root         (0)   604752 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM6.py
+-rw-r--r--   0 root         (0) root         (0)    18029 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM6_41401.py
+-rw-r--r--   0 root         (0) root         (0)    16476 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM6_4140a.py
+-rw-r--r--   0 root         (0) root         (0)   288628 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM7.py
+-rw-r--r--   0 root         (0) root         (0)      312 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM7_13505.py
+-rw-r--r--   0 root         (0) root         (0)    45791 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/I24M6.py
+-rw-r--r--   0 root         (0) root         (0)     8558 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/IBase.py
+-rw-r--r--   0 root         (0) root         (0)    14826 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5180M5.py
+-rw-r--r--   0 root         (0) root         (0)      339 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5180M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    15217 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5.py
+-rw-r--r--   0 root         (0) root         (0)      510 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    59696 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5_435.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5_436.py
+-rw-r--r--   0 root         (0) root         (0)    47115 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NS5160M6.py
+-rw-r--r--   0 root         (0) root         (0)   122296 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/ResEntity.py
+-rw-r--r--   0 root         (0) root         (0)      512 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/SA5212M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/route/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/route/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5311 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/route/route.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/
+-rw-r--r--   0 root         (0) root         (0)     4718 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/HostTypeJudge.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/RedfishClient.py
+-rw-r--r--   0 root         (0) root         (0)    10339 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/RegularCheckUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/RequestClient.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7550 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/configUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/fileUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/parameterConversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspursmsdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      896 2024-04-11 02:29:17.000000 inspursmsdk-2.1.6/inspursmsdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2682 2024-04-11 02:29:17.000000 inspursmsdk-2.1.6/inspursmsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 02:29:17.000000 inspursmsdk-2.1.6/inspursmsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2024-04-11 02:29:17.000000 inspursmsdk-2.1.6/inspursmsdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-11 02:29:17.000000 inspursmsdk-2.1.6/inspursmsdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5216 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/ism.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-04-11 02:26:45.000000 inspursmsdk-2.1.6/setup.py
```

### Comparing `inspursmsdk-2.1.5/MANIFEST.in` & `inspursmsdk-2.1.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/PKG-INFO` & `inspursmsdk-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 1.1
 Name: inspursmsdk
-Version: 2.1.5
+Version: 2.1.6
 Summary: inspur server manager api
 Home-page: https://github.com/ISIB-Group/inspursmsdk
 Author: Wangbaoshan
 Author-email: wangbaoshan@inspur.com
 License: Expat License
 Description: # inspursmsdk
         inspursmsdk is a support tool for ansible.inspur.sm
         
         ## External requirements
         
         Circumstance instruction:
         inspursmsdk relies on the Ipmitool tool.
         
         Main steps:
-        install inspursmsdk
-        yum istall ipmitool
+        * pip install inspursmsdk
+        * yum istall ipmitool
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/IpmiFunc.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/IpmiFunc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/biosPostEventStr.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/biosPostEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/commonInfoStr.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/commonInfoStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/eventLogString.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/eventLogString.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/sensorEventStr.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/sensorEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/M5Log/showSensorDesc.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/showSensorDesc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/RedfishFunc.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/RedfishFunc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/RestFunc.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/RestFunc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/backup.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/backup.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/A7.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/A7.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/M4.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M4.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/M5.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/M6-N.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M6-N.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/M6.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/M7.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M7.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/NF3180A6.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF3180A6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/NF3280A6.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF3280A6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/NF5180M5.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5180M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/NF5280M5.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5280M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/NF5468A5.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5468A5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/NF5488A5.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5488A5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/SA5112M5.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/SA5112M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/bios/SA5212M5.xml` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/SA5212M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/command/restore.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/command/restore.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/conf/NF5180M5.yml` & `inspursmsdk-2.1.6/inspur_sm_sdk/conf/NF5180M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/conf/NF5280M5.yml` & `inspursmsdk-2.1.6/inspur_sm_sdk/conf/NF5280M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/conf/SA5112M5.yml` & `inspursmsdk-2.1.6/inspur_sm_sdk/conf/SA5112M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/conf/SA5212M5.yml` & `inspursmsdk-2.1.6/inspur_sm_sdk/conf/SA5212M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/Base.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/Base.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonA5.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonA6.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonA7.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA7.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonM5.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonM6.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonM6_41401.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM6_41401.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonM6_4140a.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM6_4140a.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/CommonM7.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM7.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/I24M6.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/I24M6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/IBase.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/IBase.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/NF5180M5.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5180M5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/NF5280M5.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/NF5280M5_435.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5_435.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/NF5280M5_436.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5_436.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/NS5160M6.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/NS5160M6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/ResEntity.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/ResEntity.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/interface/SA5212M5Impl.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/interface/SA5212M5Impl.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/route/route.yml` & `inspursmsdk-2.1.6/inspur_sm_sdk/route/route.yml`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,17 @@
     1.1308: CommonA7_11308
 NF5468A7:
     common: CommonA7
     1.1308: CommonA7_11308
 NF5688A7:
     common: CommonA7
     1.1308: CommonA7_11308
+NF5688-A7-A0-R0-00:
+    common: CommonA7
+    1.1308: CommonA7_11308
 TS860-M7-A0-R0-00:
     common: CommonM7
     1.3505: CommonM7_13505
 TS860M7:
     common: CommonM7
     1.3505: CommonM7_13505
 NF8480M7:
@@ -223,7 +226,22 @@
     common: CommonM7
     1.3505: CommonM7_13505
 NF5466-M7-C0-R0-00:
     common: CommonM7
     1.3505: CommonM7_13505
 NF5280A6:
     common: CommonA6
+NF5476M7:
+    common: CommonM7
+    1.3505: CommonM7_13505
+NF5476-M7-A0-R0-00:
+    common: CommonM7
+    1.3505: CommonM7_13505
+NF5476-M7--A0-F0-00:
+    common: CommonM7
+    1.3505: CommonM7_13505
+NF5298M7:
+    common: CommonM7
+    1.3505: CommonM7_13505
+NF5298-M7-C0-R0-00:
+    common: CommonM7
+    1.3505: CommonM7_13505
```

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/util/HostTypeJudge.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/util/HostTypeJudge.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/util/RedfishClient.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/util/RedfishClient.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/util/RegularCheckUtil.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/util/RegularCheckUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/util/RequestClient.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/util/RequestClient.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/util/configUtil.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/util/configUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/util/fileUtil.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/util/fileUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspur_sm_sdk/util/parameterConversion.py` & `inspursmsdk-2.1.6/inspur_sm_sdk/util/parameterConversion.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/inspursmsdk.egg-info/PKG-INFO` & `inspursmsdk-2.1.6/inspursmsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 1.1
 Name: inspursmsdk
-Version: 2.1.5
+Version: 2.1.6
 Summary: inspur server manager api
 Home-page: https://github.com/ISIB-Group/inspursmsdk
 Author: Wangbaoshan
 Author-email: wangbaoshan@inspur.com
 License: Expat License
 Description: # inspursmsdk
         inspursmsdk is a support tool for ansible.inspur.sm
         
         ## External requirements
         
         Circumstance instruction:
         inspursmsdk relies on the Ipmitool tool.
         
         Main steps:
-        install inspursmsdk
-        yum istall ipmitool
+        * pip install inspursmsdk
+        * yum istall ipmitool
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `inspursmsdk-2.1.5/inspursmsdk.egg-info/SOURCES.txt` & `inspursmsdk-2.1.6/inspursmsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.5/ism.py` & `inspursmsdk-2.1.6/ism.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ImportError:
     ISM_EXIST = False
 sys.path.append(os.path.join(sys.path[0], "interface"))
 current_time = time.strftime(
     '%Y-%m-%d   %H:%M:%S',
     time.localtime(
         time.time()))
-__version__ = '2.1.5'
+__version__ = '2.1.6'
 
 
 ERR_dict = {
     'ERR_CODE_CMN_FAIL': 'data acquisition exception',
     'ERR_CODE_PARAM_NULL': 'parameter is null',
     'ERR_CODE_INPUT_ERROR': 'parameter error',
     'ERR_CODE_INTF_FAIL': 'create link exception',
```

### Comparing `inspursmsdk-2.1.5/setup.py` & `inspursmsdk-2.1.6/setup.py`

 * *Files identical despite different names*

