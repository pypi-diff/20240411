# Comparing `tmp/inManage-1.0.0.tar.gz` & `tmp/inManage-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inManage-1.0.0.tar", last modified: Wed Nov  1 03:10:20 2023, max compression
+gzip compressed data, was "dist/inManage-1.0.1.tar", last modified: Thu Apr 11 02:31:46 2024, max compression
```

## Comparing `inManage-1.0.0.tar` & `inManage-1.0.1.tar`

### file list

```diff
@@ -1,88 +1,83 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 03:10:20.000000 inManage-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      975 2023-11-01 03:05:09.000000 inManage-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      894 2023-11-01 03:10:20.000000 inManage-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      229 2023-11-01 03:05:08.000000 inManage-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       25 2023-11-01 03:05:08.000000 inManage-1.0.0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 03:10:20.000000 inManage-1.0.0/inManage.egg-info/
--rw-r--r--   0 root         (0) root         (0)      894 2023-11-01 03:10:20.000000 inManage-1.0.0/inManage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2606 2023-11-01 03:10:20.000000 inManage-1.0.0/inManage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-01 03:10:20.000000 inManage-1.0.0/inManage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-11-01 03:10:20.000000 inManage-1.0.0/inManage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-11-01 03:10:20.000000 inManage-1.0.0/inManage.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5228 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 03:10:20.000000 inManage-1.0.0/inmanage_sdk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 03:10:20.000000 inManage-1.0.0/inmanage_sdk/command/
--rw-r--r--   0 root         (0) root         (0)    49818 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/IpmiFunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 03:10:20.000000 inManage-1.0.0/inmanage_sdk/command/M5Log/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/command/M5Log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/M5Log/biosPostEventStr.py
--rw-r--r--   0 root         (0) root         (0)    16391 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/M5Log/commonInfoStr.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/M5Log/eventLogString.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/M5Log/sensorEventStr.py
--rw-r--r--   0 root         (0) root         (0)    51098 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/M5Log/sensorSpecificEventStr.py
--rw-r--r--   0 root         (0) root         (0)     5698 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/command/M5Log/showSensorDesc.py
--rw-r--r--   0 root         (0) root         (0)    21216 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/command/RedfishFunc.py
--rw-r--r--   0 root         (0) root         (0)   299927 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/command/RestFunc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12150 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/backup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 03:10:20.000000 inManage-1.0.0/inmanage_sdk/command/bios/
--rw-r--r--   0 root         (0) root         (0)    44672 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/A7.xml
--rw-r--r--   0 root         (0) root         (0)    18001 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/M4.xml
--rw-r--r--   0 root         (0) root         (0)    54050 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/M5.xml
--rw-r--r--   0 root         (0) root         (0)    84400 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/M6-N.xml
--rw-r--r--   0 root         (0) root         (0)    81680 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/M6.xml
--rw-r--r--   0 root         (0) root         (0)    46082 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/M7.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/NF3180A6.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/NF3280A6.xml
--rw-r--r--   0 root         (0) root         (0)   354128 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/NF5180M5.xml
--rw-r--r--   0 root         (0) root         (0)   354211 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/NF5280M5.xml
--rw-r--r--   0 root         (0) root         (0)    36922 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/NF5468A5.xml
--rw-r--r--   0 root         (0) root         (0)    29961 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/NF5488A5.xml
--rw-r--r--   0 root         (0) root         (0)   354291 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/SA5112M5.xml
--rw-r--r--   0 root         (0) root         (0)   354213 2023-11-01 03:05:11.000000 inManage-1.0.0/inmanage_sdk/command/bios/SA5212M5.xml
--rw-r--r--   0 root         (0) root         (0)    66016 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/command/restore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 03:10:20.000000 inManage-1.0.0/inmanage_sdk/conf/
--rw-r--r--   0 root         (0) root         (0)     1613 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/conf/NF5180M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/conf/NF5280M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/conf/SA5112M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/conf/SA5212M5.yml
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/conf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 03:10:20.000000 inManage-1.0.0/inmanage_sdk/interface/
--rw-r--r--   0 root         (0) root         (0)    44314 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/interface/Base.py
--rw-r--r--   0 root         (0) root         (0)     2588 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/interface/CommonA5.py
--rw-r--r--   0 root         (0) root         (0)     3021 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/interface/CommonA6.py
--rw-r--r--   0 root         (0) root         (0)     6330 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/interface/CommonA7.py
--rw-r--r--   0 root         (0) root         (0)      315 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/interface/CommonA7_11308.py
--rw-r--r--   0 root         (0) root         (0)   744214 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/interface/CommonM5.py
--rw-r--r--   0 root         (0) root         (0)   604745 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/interface/CommonM6.py
--rw-r--r--   0 root         (0) root         (0)    18026 2023-11-01 03:05:10.000000 inManage-1.0.0/inmanage_sdk/interface/CommonM6_41401.py
--rw-r--r--   0 root         (0) root         (0)    16472 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/CommonM6_4140a.py
--rw-r--r--   0 root         (0) root         (0)   288624 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/CommonM7.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/CommonM7_13505.py
--rw-r--r--   0 root         (0) root         (0)    45789 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/I24M6.py
--rw-r--r--   0 root         (0) root         (0)     8558 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/IBase.py
--rw-r--r--   0 root         (0) root         (0)    14823 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/NF5180M5.py
--rw-r--r--   0 root         (0) root         (0)      338 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/NF5180M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    15213 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/NF5280M5.py
--rw-r--r--   0 root         (0) root         (0)      509 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/NF5280M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    59692 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/NF5280M5_435.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/NF5280M5_436.py
--rw-r--r--   0 root         (0) root         (0)    47112 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/NS5160M6.py
--rw-r--r--   0 root         (0) root         (0)   122296 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/ResEntity.py
--rw-r--r--   0 root         (0) root         (0)      511 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/SA5212M5Impl.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 03:10:20.000000 inManage-1.0.0/inmanage_sdk/route/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/route/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4904 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/route/route.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 03:10:20.000000 inManage-1.0.0/inmanage_sdk/util/
--rw-r--r--   0 root         (0) root         (0)     4716 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/util/HostTypeJudge.py
--rw-r--r--   0 root         (0) root         (0)     4788 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/util/RedfishClient.py
--rw-r--r--   0 root         (0) root         (0)    10339 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/util/RegularCheckUtil.py
--rw-r--r--   0 root         (0) root         (0)     7686 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/util/RequestClient.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7550 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/util/configUtil.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/util/fileUtil.py
--rw-r--r--   0 root         (0) root         (0)     7590 2023-11-01 03:05:09.000000 inManage-1.0.0/inmanage_sdk/util/parameterConversion.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-01 03:10:20.000000 inManage-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1438 2023-11-01 03:05:08.000000 inManage-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      785 2024-04-11 02:22:49.000000 inManage-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-11 02:31:46.000000 inManage-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      228 2024-04-11 02:22:49.000000 inManage-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-11 02:22:49.000000 inManage-1.0.1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inManage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-11 02:31:46.000000 inManage-1.0.1/inManage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-04-11 02:31:46.000000 inManage-1.0.1/inManage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 02:31:46.000000 inManage-1.0.1/inManage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2024-04-11 02:31:46.000000 inManage-1.0.1/inManage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-11 02:31:46.000000 inManage-1.0.1/inManage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/command/
+-rw-r--r--   0 root         (0) root         (0)    49818 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/IpmiFunc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/biosPostEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    16391 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/commonInfoStr.py
+-rw-r--r--   0 root         (0) root         (0)      693 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/eventLogString.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/sensorEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    51098 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/sensorSpecificEventStr.py
+-rw-r--r--   0 root         (0) root         (0)     5697 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/showSensorDesc.py
+-rw-r--r--   0 root         (0) root         (0)    21216 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/RedfishFunc.py
+-rw-r--r--   0 root         (0) root         (0)   304005 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/RestFunc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12150 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/backup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/command/bios/
+-rw-r--r--   0 root         (0) root         (0)    44672 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/A7.xml
+-rw-r--r--   0 root         (0) root         (0)    18001 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/M4.xml
+-rw-r--r--   0 root         (0) root         (0)    54050 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/M5.xml
+-rw-r--r--   0 root         (0) root         (0)    84400 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/M6-N.xml
+-rw-r--r--   0 root         (0) root         (0)    81680 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/M6.xml
+-rw-r--r--   0 root         (0) root         (0)    46082 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/M7.xml
+-rw-r--r--   0 root         (0) root         (0)   117980 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/M7_5.10.00.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/NF3180A6.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/NF3280A6.xml
+-rw-r--r--   0 root         (0) root         (0)   354128 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/NF5180M5.xml
+-rw-r--r--   0 root         (0) root         (0)   354211 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/bios/NF5280M5.xml
+-rw-r--r--   0 root         (0) root         (0)    36922 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/bios/NF5468A5.xml
+-rw-r--r--   0 root         (0) root         (0)    29961 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/bios/NF5488A5.xml
+-rw-r--r--   0 root         (0) root         (0)   354291 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/bios/SA5112M5.xml
+-rw-r--r--   0 root         (0) root         (0)   354213 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/bios/SA5212M5.xml
+-rw-r--r--   0 root         (0) root         (0)    66016 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/restore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/interface/
+-rw-r--r--   0 root         (0) root         (0)    44314 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/Base.py
+-rw-r--r--   0 root         (0) root         (0)     2588 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonA5.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonA6.py
+-rw-r--r--   0 root         (0) root         (0)     6330 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonA7.py
+-rw-r--r--   0 root         (0) root         (0)      315 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonA7_11308.py
+-rw-r--r--   0 root         (0) root         (0)   744214 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonM5.py
+-rw-r--r--   0 root         (0) root         (0)   608244 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonM6.py
+-rw-r--r--   0 root         (0) root         (0)    18026 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonM6_41401.py
+-rw-r--r--   0 root         (0) root         (0)    16472 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonM6_4140a.py
+-rw-r--r--   0 root         (0) root         (0)   271855 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonM7.py
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/CommonM7_13505.py
+-rw-r--r--   0 root         (0) root         (0)    45789 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/I24M6.py
+-rw-r--r--   0 root         (0) root         (0)     8558 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/IBase.py
+-rw-r--r--   0 root         (0) root         (0)    14823 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NF5180M5.py
+-rw-r--r--   0 root         (0) root         (0)      338 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NF5180M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    15213 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NF5280M5.py
+-rw-r--r--   0 root         (0) root         (0)      509 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NF5280M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    59692 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NF5280M5_435.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NF5280M5_436.py
+-rw-r--r--   0 root         (0) root         (0)    47112 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NS5160M6.py
+-rw-r--r--   0 root         (0) root         (0)   123026 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/ResEntity.py
+-rw-r--r--   0 root         (0) root         (0)      511 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/SA5212M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/route/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/route/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5516 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/route/route.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/util/
+-rw-r--r--   0 root         (0) root         (0)     4716 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/HostTypeJudge.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/RedfishClient.py
+-rw-r--r--   0 root         (0) root         (0)    10339 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/RegularCheckUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/RequestClient.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7550 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/configUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/fileUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/parameterConversion.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 02:31:46.000000 inManage-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1438 2024-04-11 02:22:49.000000 inManage-1.0.1/setup.py
```

### Comparing `inManage-1.0.0/PKG-INFO` & `inManage-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 1.1
 Name: inManage
-Version: 1.0.0
+Version: 1.0.1
 Summary: ieisystem server manager api
 Home-page: https://github.com/ieisystem/inManage
 Author: Wangbaoshan
 Author-email: wangbaoshan@ieisystem.com
 License: Expat License
-Description: # ieisystemInManage
+Description: # InManage
         inManage is a support tool for ansible.ieisystem.inmanage
         
         ## External requirements
         
         Circumstance instruction:
         inManage relies on the Ipmitool tool.
         
         Main steps:
-        install inManage
-        yum install ipmitool
+        * pip install inManage
+        * yum install ipmitool
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `inManage-1.0.0/inManage.egg-info/PKG-INFO` & `inManage-1.0.1/inManage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 1.1
 Name: inManage
-Version: 1.0.0
+Version: 1.0.1
 Summary: ieisystem server manager api
 Home-page: https://github.com/ieisystem/inManage
 Author: Wangbaoshan
 Author-email: wangbaoshan@ieisystem.com
 License: Expat License
-Description: # ieisystemInManage
+Description: # InManage
         inManage is a support tool for ansible.ieisystem.inmanage
         
         ## External requirements
         
         Circumstance instruction:
         inManage relies on the Ipmitool tool.
         
         Main steps:
-        install inManage
-        yum install ipmitool
+        * pip install inManage
+        * yum install ipmitool
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `inManage-1.0.0/inManage.egg-info/SOURCES.txt` & `inManage-1.0.1/inManage.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,23 @@
 inmanage_sdk/command/M5Log/showSensorDesc.py
 inmanage_sdk/command/bios/A7.xml
 inmanage_sdk/command/bios/M4.xml
 inmanage_sdk/command/bios/M5.xml
 inmanage_sdk/command/bios/M6-N.xml
 inmanage_sdk/command/bios/M6.xml
 inmanage_sdk/command/bios/M7.xml
+inmanage_sdk/command/bios/M7_5.10.00.xml
 inmanage_sdk/command/bios/NF3180A6.xml
 inmanage_sdk/command/bios/NF3280A6.xml
 inmanage_sdk/command/bios/NF5180M5.xml
 inmanage_sdk/command/bios/NF5280M5.xml
 inmanage_sdk/command/bios/NF5468A5.xml
 inmanage_sdk/command/bios/NF5488A5.xml
 inmanage_sdk/command/bios/SA5112M5.xml
 inmanage_sdk/command/bios/SA5212M5.xml
-inmanage_sdk/conf/NF5180M5.yml
-inmanage_sdk/conf/NF5280M5.yml
-inmanage_sdk/conf/SA5112M5.yml
-inmanage_sdk/conf/SA5212M5.yml
-inmanage_sdk/conf/__init__.py
 inmanage_sdk/interface/Base.py
 inmanage_sdk/interface/CommonA5.py
 inmanage_sdk/interface/CommonA6.py
 inmanage_sdk/interface/CommonA7.py
 inmanage_sdk/interface/CommonA7_11308.py
 inmanage_sdk/interface/CommonM5.py
 inmanage_sdk/interface/CommonM6.py
```

### Comparing `inManage-1.0.0/inmanage.py` & `inManage-1.0.1/inmanage.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ImportError:
     INMANAGE_EXIST = False
 sys.path.append(os.path.join(sys.path[0], "interface"))
 current_time = time.strftime(
     '%Y-%m-%d   %H:%M:%S',
     time.localtime(
         time.time()))
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 
 ERR_dict = {
     'ERR_CODE_CMN_FAIL': 'data acquisition exception',
     'ERR_CODE_PARAM_NULL': 'parameter is null',
     'ERR_CODE_INPUT_ERROR': 'parameter error',
     'ERR_CODE_INTF_FAIL': 'create link exception',
```

### Comparing `inManage-1.0.0/inmanage_sdk/command/IpmiFunc.py` & `inManage-1.0.1/inmanage_sdk/command/IpmiFunc.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/M5Log/biosPostEventStr.py` & `inManage-1.0.1/inmanage_sdk/command/M5Log/biosPostEventStr.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/M5Log/commonInfoStr.py` & `inManage-1.0.1/inmanage_sdk/command/M5Log/commonInfoStr.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/M5Log/eventLogString.py` & `inManage-1.0.1/inmanage_sdk/command/M5Log/eventLogString.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/M5Log/sensorEventStr.py` & `inManage-1.0.1/inmanage_sdk/command/M5Log/sensorEventStr.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/M5Log/sensorSpecificEventStr.py` & `inManage-1.0.1/inmanage_sdk/command/M5Log/sensorSpecificEventStr.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/M5Log/showSensorDesc.py` & `inManage-1.0.1/inmanage_sdk/command/M5Log/showSensorDesc.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             if type == 0x0:
                 pass
             elif type == 0x6F:
                 offset = getbits(item.event_data1, 3, 0)
                 if m_Max_allowed_SensorSpecific_offset[item['sensor_type']] >= offset:
                     eventdesc = sensor_specific_event[item['sensor_type']][offset]
                 else:
-                    eventdesc = eventLogStrings.STR_EVENT_LOG_INVALID_OFFSET;
+                    eventdesc = eventLogStrings.STR_EVENT_LOG_INVALID_OFFSET
             elif (type >= 0x01) and (type <= 0x0C):
                 offset = getbits(item['event_data1'], 3, 0)
                 if m_Max_allowed_offset[type] >= offset:
                     eventdesc = sensorEvent_Str[type][offset]
                 else:
                     eventdesc = eventLogStrings['STR_EVENT_LOG_INVALID_OFFSET']
             else:
```

### Comparing `inManage-1.0.0/inmanage_sdk/command/RedfishFunc.py` & `inManage-1.0.1/inmanage_sdk/command/RedfishFunc.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/RestFunc.py` & `inManage-1.0.1/inmanage_sdk/command/RestFunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -2764,19 +2764,35 @@
                 data = {
                     "username": Encrypt(client.username),
                     "password": Encrypt(client.passcode),
                     "encrypt_flag": 1,
                     "login_tag": randomtag.json().get('random')
                 }
                 response = client.request("POST", "api/session", data=data)
-                if response is not None and response.status_code == 200:
+                if response is not None and response.status_code in range(200, 300):
+                    encrypt_type_flag = 2
                     headers = {
                         "X-CSRFToken": response.json()["CSRFToken"],
                         "Cookie": response.headers["set-cookie"]
                     }
+                else:
+                    # M6 好像也没有RSA加密方式
+                    data = {
+                        "username": encrypt_rsa(client.username),
+                        "password": encrypt_rsa(client.passcode),
+                        "encrypt_flag": 1,
+                        "login_tag": randomtag.json().get('random')
+                    }
+                    response = client.request("POST", "api/session", data=data)
+                    if response is not None and response.status_code in range(200, 300):
+                        encrypt_type_flag = 1
+                        headers = {
+                            "X-CSRFToken": response.json()["CSRFToken"],
+                            "Cookie": response.headers["set-cookie"]
+                        }
         else:
             data = {
                 "username": client.username,
                 "password": client.passcode,
             }
             response = client.request("POST", "api/session", data=data)
             if response is not None and response.status_code == 200:
@@ -2785,14 +2801,43 @@
                     "Cookie": response.headers["set-cookie"]
                 }
     except:
         headers = {}
     return headers
 
 
+def encrypt_rsa(sourceStr):
+    try:
+        if sourceStr is None or sourceStr == "":
+            return sourceStr
+        from Crypto.Cipher import PKCS1_v1_5
+        from Crypto.PublicKey import RSA
+        encrypt_key = "-----BEGIN PUBLIC KEY-----\nMIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEAvAIoJ+F0MiuinN903RNX\n"\
+                        "z4umR3b0OackykNmXP+d5qRmxfRS6ymjGwmS1hxBVkGNAulpoeqNDQ1oeilc6IOI\n"\
+                        "6QgsRDzSas4/cXY7/ndz1TK2ocBhh9bxwHfBa0STFyK8004lQ2FKjJj9zrUMC67w\n"\
+                        "U3qvU5np2pddqaIunEEExeU88ZVsNS7jBYDlN/XDdT6sqs0qAicley9ogfeRSh95\n"\
+                        "9KxCG3QnyMSNDk+Gf8Yp4z6hfc8ON1FYsQfFh3yVScvHp0UKbuhs+Mt7TjoyALel\n"\
+                        "cGY18eFt0evYT+n7arRRvdjsDfQz8mJTXYxBy5eTgIVt7s8hufuqtnVH3chkp5o1\n"\
+                        "32LiTTutoliyLsyr+uRitnYPH97vE+edESimql1112ozzs8Axjsh4ugX8YhU2jdA\n"\
+                        "BZSNz6AqfmnALbHRaaxoWinyuKRGA1LPMFSwW3pkbJ8RFqm7PJIza/IKmarqb1S1\n"\
+                        "2d9EqyWjIKD+KAnrsSRttfhgujf5qPCye3m0XhAIDC96JkRsv3x/erD8PQp69fdP\n"\
+                        "QdzTLnHTFSpzDE8KFyj3+YL99ejzxg3TW7/JAeJRX/XXAygRf/1GGOIxv1odXfOn\n"\
+                        "HOlA5ssqfj1Ch6zxEMuf/my6bz5M309pRQheNoEHBMDJlCRQPNeLN5ILw3n9c2cT\n"\
+                        "RUUIfwZlDzalqfR8zWNh0VUCAwEAAQ==\n-----END PUBLIC KEY-----"
+        if sourceStr is None:
+            return None
+        pub_key = RSA.importKey(encrypt_key)
+        pub_cipher = PKCS1_v1_5.new(pub_key)
+        cryptedStr = base64.b64encode(pub_cipher.encrypt(sourceStr.encode()))
+        cryptedStr = str(cryptedStr, encoding='utf-8')
+        return cryptedStr
+    except Exception as e:
+        return sourceStr
+
+
 def logout(client):
     try:
         responds = client.request("DELETE", "api/session", client.getHearder())
     except BaseException:
         return
     return
 
@@ -3776,17 +3821,41 @@
             JSON['data'] = formatError("api/diagnose/bmc-reset", response)
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/diagnose/bmc-reset", response)
     return JSON
 
 
-# 开机自检代码
+def resetBMCM7(client, type):
+    JSON = {}
+    if type.upper() != "BMC" and type.upper() != "KVM":
+        JSON['code'] = 1
+        JSON['data'] = 'reset BMC or KVM only.'
+    data = {
+        "reset": type.upper(),
+        "currentuserpassword": encrypt_rsa(client.passcode)
+    }
+    response = client.request("POST", "api/diagnose/bmc-reset", client.getHearder(), json=data)
+    if response is None:
+        JSON['code'] = 1
+        JSON['data'] = 'Failed to call BMC interface api/diagnose/bmc-reset ,response is none'
+    elif response.status_code in range(200, 300):
+        try:
+            JSON["code"] = 0
+            JSON["data"] = "reset " + type + " success"
+        except:
+            JSON['code'] = 1
+            JSON['data'] = formatError("api/diagnose/bmc-reset", response)
+    else:
+        JSON['code'] = 1
+        JSON['data'] = formatError("api/diagnose/bmc-reset", response)
+    return JSON
 
 
+# 开机自检代码
 def getBiosPostCode(client):
     JSON = {}
     response = client.request("GET", "api/diagnose/bios-post-code", client.getHearder())
     if response is None:
         JSON['code'] = 1
         JSON['data'] = 'Failed to call BMC interface api/diagnose/bios-post-code,response is none'
     elif response.status_code == 200:
@@ -7811,14 +7880,30 @@
             JSON['data'] = formatError("api/settings/snmp", response)
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/settings/snmp", response)
     return JSON
 
 
+def getgpu(client):
+    JSON = {}
+    response = client.request("GET", "api/gpu/gpu_info", client.getHearder(), None, None, None, None)
+    if response is None:
+        JSON['code'] = 1
+        JSON['data'] = 'Failed to call BMC interface api/gpu/gpu_info, response is none'
+    elif response.status_code in range(200, 300):
+        result = response.json()
+        JSON['code'] = 0
+        JSON['data'] = result
+    else:
+        JSON['code'] = 1
+        JSON['data'] = formatError("api/gpu/gpu_info", response)
+    return JSON
+
+
 class NF5280M5_SensorDesc():
 
     def __init__(self):
         command_path = os.path.dirname(os.path.realpath(__file__))
         ipmi_path = os.path.join(command_path, "M5Log")
         sys.path.append(ipmi_path)
```

### Comparing `inManage-1.0.0/inmanage_sdk/command/backup.py` & `inManage-1.0.1/inmanage_sdk/command/backup.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/A7.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/A7.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/M4.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/M4.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/M5.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/M5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/M6-N.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/M6-N.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/M6.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/M6.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/M7.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/M7.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/NF3180A6.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/NF3180A6.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/NF3280A6.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/NF3280A6.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/NF5180M5.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/NF5180M5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/NF5280M5.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/NF5280M5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/NF5468A5.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/NF5468A5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/NF5488A5.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/NF5488A5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/SA5112M5.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/SA5112M5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/bios/SA5212M5.xml` & `inManage-1.0.1/inmanage_sdk/command/bios/SA5212M5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/command/restore.py` & `inManage-1.0.1/inmanage_sdk/command/restore.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/Base.py` & `inManage-1.0.1/inmanage_sdk/interface/Base.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/CommonA5.py` & `inManage-1.0.1/inmanage_sdk/interface/CommonA5.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/CommonA6.py` & `inManage-1.0.1/inmanage_sdk/interface/CommonA6.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/CommonA7.py` & `inManage-1.0.1/inmanage_sdk/interface/CommonA7.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/CommonM5.py` & `inManage-1.0.1/inmanage_sdk/interface/CommonM5.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/CommonM6.py` & `inManage-1.0.1/inmanage_sdk/interface/CommonM6.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,17 @@
     NCSIBean,
     DNSBean,
     SessionBean,
     SensorBean,
     Sensor,
     FruBean,
     PowerConsumptionBean,
-    SuspendBean)
+    SuspendBean,
+    HBABean,
+    HBAPost)
 retry_count = 0
 
 
 class CommonM6(Base):
 
     def getcapabilities(self, client, args):
         res = ResultBean()
@@ -909,52 +911,68 @@
                 errorinfo = ",".join(errorlist)
                 errordict[bios_dict.get(bioskey)]=errorinfo
         if errordict == {}:
             return True, None
         else:
             return False, errordict
 
-    def setbios(self, client, args):
-        def update_infoList(infoList):
-            flag = False
-            attr_result = RedfishFunc.getBIOSAttrByRedfish(client, login_header)
-            if "code" in attr_result and attr_result.get('code') == 0 and attr_result.get('data') != "":
-                json_url = attr_result.get('data')
-                json_result = RedfishFunc.getBIOSAttrJsonByRedfish(client, login_header, json_url)
-                if "code" in json_result and json_result.get('code') == 0 and json_result.get('data') != {}:
-                    flag = True
-                    json_data = json_result.get('data')
-                    if "UefiBootOrder1" in json_data.keys():
-                        item_value = json_data.get("UefiBootOrder1")
-                        for item_1 in infoList:
-                            if item_1.get('getter') == "UefiBootOrder1" or \
-                                    item_1.get('getter') == "UefiBootOrder2" or \
-                                    item_1.get('getter') == "UefiBootOrder3" or \
-                                    item_1.get('getter') == "UefiBootOrder4":
-                                setter_list = []
-                                for item_2 in item_value:
-                                    setter_list.append(
-                                        {"cmd": item_2.get("ValueName"), "value": item_2.get("ValueName")})
-                                item_1['setter'] = setter_list
-                    elif "LegacyBootOrder1" in json_data.keys():
-                        item_value = json_data.get("LegacyBootOrder1")
-                        for item_1 in infoList:
-                            if item_1.get('getter') == "LegacyBootOrder1" or \
-                                    item_1.get('getter') == "LegacyBootOrder2" or \
-                                    item_1.get('getter') == "LegacyBootOrder3" or \
-                                    item_1.get('getter') == "LegacyBootOrder4":
-                                setter_list = []
-                                for item_2 in item_value:
-                                    setter_list.append(
-                                        {"cmd": item_2.get("ValueName"), "value": item_2.get("ValueName")})
-                                item_1['setter'] = setter_list
-            return flag, infoList
+    def getXmlFileName(self, res):
+        xml_path = os.path.join(IpmiFunc.command_path, "bios") + os.path.sep
+        if "IioVmdOnStackPch" in res.keys():
+            xmlfilepath = xml_path + "M6-N.xml"
+        else:
+            xmlfilepath = xml_path + "M6.xml"
+        return xmlfilepath
+
+    def update_xmlinfo(self, client, login_header, xmlhelp):
+        Bios_result = ResultBean()
+        attr_result = RedfishFunc.getBIOSAttrByRedfish(client, login_header)
+        if attr_result.get('code') == 0:
+            json_url = attr_result.get('data')
+            json_result = RedfishFunc.getBIOSAttrJsonByRedfish(client, login_header, json_url)
+            if json_result.get('code') == 0:
+                json_data = json_result.get('data')
+                if "UefiBootOrder1" in json_data.keys():
+                    item_value = json_data.get("UefiBootOrder1")
+                    for item_1 in xmlhelp:
+                        if item_1.get('getter') == "UefiBootOrder1" or \
+                                item_1.get('getter') == "UefiBootOrder2" or \
+                                item_1.get('getter') == "UefiBootOrder3" or \
+                                item_1.get('getter') == "UefiBootOrder4":
+                            setter_list = []
+                            for item_2 in item_value:
+                                setter_list.append(
+                                    {"cmd": item_2.get("ValueName"), "value": item_2.get("ValueName")})
+                            item_1['setter'] = setter_list
+                elif "LegacyBootOrder1" in json_data.keys():
+                    item_value = json_data.get("LegacyBootOrder1")
+                    for item_1 in xmlhelp:
+                        if item_1.get('getter') == "LegacyBootOrder1" or \
+                                item_1.get('getter') == "LegacyBootOrder2" or \
+                                item_1.get('getter') == "LegacyBootOrder3" or \
+                                item_1.get('getter') == "LegacyBootOrder4":
+                            setter_list = []
+                            for item_2 in item_value:
+                                setter_list.append(
+                                    {"cmd": item_2.get("ValueName"), "value": item_2.get("ValueName")})
+                            item_1['setter'] = setter_list
+                Bios_result.State('Success')
+                Bios_result.Message([xmlhelp])
+            else:
+                Bios_result.State('Failure')
+                Bios_result.Message([str(json_result.get('data'))])
+        else:
+            Bios_result.State('Failure')
+            Bios_result.Message([str(attr_result.get('data'))])
 
+        return Bios_result
+
+    def setbios(self, client, args):
         Bios_result = ResultBean()
-        # args.list = False
+        # 不输入-L
         if 'list' not in args or ('list' in args and args.list is False):
             if args.attribute is None and args.value is None and args.fileurl is None:
                 Bios_result.Message(['please input a command at least.'])
                 Bios_result.State('Failure')
                 return Bios_result
             elif args.attribute is None and args.value is None and args.fileurl is not None:
                 if not os.path.exists(args.fileurl) or not os.path.isfile(args.fileurl):
@@ -984,34 +1002,29 @@
             Bios_result.Message(['login session service failed, please check username/password/host/port'])
             return Bios_result
         data = {'Attributes': {}}
         result = RedfishFunc.getBiosV1ByRedfish(client, login_header)
         boot_option = ['UEFIBootOption1', 'UEFIBootOption2', 'UEFIBootOption3', 'UEFIBootOption4', 'LegacyBootOption1',
                        'LegacyBootOption2', 'LegacyBootOption3', 'LegacyBootOption4']
         if result.get('code') == 0 and result.get('data') is not None:
-            xml_path = os.path.join(IpmiFunc.command_path, "bios") + os.path.sep
-            if "IioVmdOnStackPch" in result.get('data').keys():
-                xmlfilepath = xml_path + "M6-N.xml"
-                xmlfilename = "M6-N.xml"
-            else:
-                xmlfilepath = xml_path + "M6.xml"
-                xmlfilename = "M6.xml"
+            xmlfilepath = self.getXmlFileName(result.get('data'))
             if os.path.exists(xmlfilepath) is False:
-                Bios_result.Message([str(xmlfilename) + ' file not exist.'])
+                Bios_result.Message([os.path.basename(xmlfilepath) + ' file not exist.'])
                 Bios_result.State('Failure')
                 RedfishFunc.logout(client, login_id, login_header)
                 return Bios_result
             biosconfutil = configUtil.configUtil()  # 实例化类对象
             blongtoSet, descriptionList, infoList = biosconfutil.getSetOption(xmlfilepath)  # 读取xml文件，返回信息
-            flag, infoList = update_infoList(infoList)
-            if not flag:
+            updateresult = self.update_xmlinfo(client, login_header, infoList)
+            if updateresult.State != "Success":
                 Bios_result.Message(["get BIOS attribute failed."])
                 Bios_result.State('Failure')
                 RedfishFunc.logout(client, login_id, login_header)
-                return Bios_result
+                return updateresult
+            infoList = updateresult.Message[0]
             if 'list' in args and args.list:
                 help_list = []
                 for info in infoList:
                     help_list.append('{:<35}: {}'.format(info['description'], list(item.get('value') for item in info.get('setter'))))
                 Bios_result.Message(help_list)
                 Bios_result.State('Success')
                 RedfishFunc.logout(client, login_id, login_header)
@@ -1027,77 +1040,112 @@
 
             if args.attribute is None and args.value is None and args.fileurl is not None:
                 for key, value in biosJson.items():
                     if str(value).lower() == "enable":
                         value = "Enabled"
                     if str(value).lower() == "disable":
                         value = "Disabled"
-                    if judgeAttInList(key.replace(" ", ""), descriptionList) is False:
+                    if self.judgeAttInListM5(key.replace(" ", ""), descriptionList) is False:
                         Bios_result.State('Failure')
                         Bios_result.Message(["Please check your attribute spell of '{0}' by -L parameter!".format(key)])
                         # logout
                         RedfishFunc.logout(client, login_id, login_header)
                         return Bios_result
                     # 执行单个设置 先读取文件，判断-a -v是否在列表中
-                    if judgeAttInList(des_key[key.replace(" ", "")], result.get('data').keys()) is False:
+                    if self.judgeAttInListM5(des_key[key.replace(" ", "")], result.get('data').keys()) is False:
                         Bios_result.State('Failure')
                         Bios_result.Message(["'{0}' is not in set options.".format(key)])
                         # logout
                         RedfishFunc.logout(client, login_id, login_header)
                         return Bios_result
                     if key in boot_option:
                         for item in des_value[key.replace(" ", "")]:
                             if str(item).startswith(value):
                                 value = item
                                 break
-                    if value not in des_value[key.replace(" ", "")]:
-                        Bios_result.State('Failure')
-                        Bios_result.Message(["{0} does not support setting to {1}!".format(key, value)])
-                        # logout
-                        RedfishFunc.logout(client, login_id, login_header)
-                        return Bios_result
-                    # if str(value).isdigit():
-                    #     data['Attributes'][des_key[key.replace(" ", "")]] = int(value)
-                    # else:
-                    #     data['Attributes'][des_key[key.replace(" ", "")]] = value
-                    data['Attributes'][des_key[key.replace(" ", "")]] = value
+
+                    values = des_value.get(key.replace(" ", ""), [])
+                    if len(values) == 1:
+                        valuestr = values[0]
+                        if "~" in valuestr:
+                            min = valuestr.split("~")[0]
+                            max = valuestr.split("~")[1]
+                        elif "-" in valuestr:
+                            min = valuestr.split("-")[0]
+                            max = valuestr.split("-")[1]
+                        if int(value) < int(min) or int(value) > int(max):
+                            Bios_result.State('Failure')
+                            Bios_result.Message(["The scope of {0} is {1}!".format(key, valuestr)])
+                            # logout
+                            RedfishFunc.logout(client, login_id, login_header)
+                            return Bios_result
+
+                    else:
+                        if str(value) not in des_value[key.replace(" ", "")]:
+                            Bios_result.State('Failure')
+                            Bios_result.Message(["{0} does not support setting to {1}!".format(key, value)])
+                            # logout
+                            RedfishFunc.logout(client, login_id, login_header)
+                            return Bios_result
+                        data['Attributes'][des_key[key.replace(" ", "")]] = str(value)
             elif args.attribute is not None and args.value is not None and args.fileurl is None:
                 if str(args.value).lower() == "enable":
                     args.value = "Enabled"
                 if str(args.value).lower() == "disable":
                     args.value = "Disabled"
-                if judgeAttInList(args.attribute.replace(" ", ""), descriptionList) is False:
+                if self.judgeAttInListM5(args.attribute.replace(" ", ""), descriptionList) is False:
                     Bios_result.State('Failure')
                     Bios_result.Message(
                         ["Please check your attribute spell of '{0}' by -L parameter!".format(args.attribute)])
                     # logout
                     RedfishFunc.logout(client, login_id, login_header)
                     return Bios_result
-                if judgeAttInList(des_key[args.attribute.replace(" ", "")], result.get('data').keys()) is False:
+                if self.judgeAttInListM5(des_key[args.attribute.replace(" ", "")], result.get('data').keys()) is False:
                     Bios_result.State('Failure')
                     Bios_result.Message(["'{0}' is not in set options.".format(args.attribute)])
                     # logout
                     RedfishFunc.logout(client, login_id, login_header)
                     return Bios_result
                 if args.attribute in boot_option:
                     for item in des_value[args.attribute.replace(" ", "")]:
                         if str(item).startswith(args.value):
                             args.value = item
                             break
-                if args.value not in des_value[args.attribute.replace(" ", "")]:
-                    Bios_result.State('Failure')
-                    Bios_result.Message(["{0} does not support setting to {1}!".format(args.attribute, args.value)])
-                    # logout
-                    RedfishFunc.logout(client, login_id, login_header)
-                    return Bios_result
-                data['Attributes'][des_key[args.attribute.replace(" ", "")]] = args.value
+
+                values = des_value.get(args.attribute.replace(" ", ""), [])
+                if len(values) == 1:
+                    valuestr = values[0]
+                    if "~" in valuestr:
+                        min = valuestr.split("~")[0]
+                        max = valuestr.split("~")[1]
+                    elif "-" in valuestr:
+                        min = valuestr.split("-")[0]
+                        max = valuestr.split("-")[1]
+                    if int(args.value) < int(min) or int(args.value) > int(max):
+                        Bios_result.State('Failure')
+                        Bios_result.Message(["The scope of {0} is {1}!".format(args.attribute, valuestr)])
+                        # logout
+                        RedfishFunc.logout(client, login_id, login_header)
+                        return Bios_result
+
+                    data['Attributes'][des_key[args.attribute.replace(" ", "")]] = int(args.value)
+                else:
+                    if str(args.value) not in values:
+                        Bios_result.State('Failure')
+                        Bios_result.Message(["{0} does not support setting to {1}!".format(args.attribute, args.value)])
+                        # logout
+                        RedfishFunc.logout(client, login_id, login_header)
+                        return Bios_result
+                    data['Attributes'][des_key[args.attribute.replace(" ", "")]] = str(args.value)
+
             # 获取future
             future_result = RedfishFunc.getBiosFuture(client, login_header)
             # 检查前置项
-            conditionflag, conditionmessage = self.judgeCondition(data['Attributes'], future_result.get('data'), result.get('data'), infoList)
+            conditionflag, conditionmessage = self.judgeCondition(data['Attributes'], future_result.get('data'),
+                                                                  result.get('data'), infoList)
             if not conditionflag:
                 Bios_result.State('Failure')
                 Bios_result.Message([conditionmessage])
                 # logout
                 RedfishFunc.logout(client, login_id, login_header)
                 return Bios_result
 
@@ -5925,15 +5973,15 @@
                 session_result.UserPrivilege(item.get('user_privilege', None))
                 seList.append(session_result.dict)
             result.State('Success')
             result.Message(seList)
         else:
             result.State("Failure")
             result.Message(
-                ["get power status error, error code " + str(info.get('code'))])
+                ["get sessions info error, error code " + str(info.get('code'))])
 
         RestFunc.logout(client)
         return result
 
     def delsession(self, client, args):
         result = ResultBean()
         headers = RestFunc.login_M6(client)
@@ -6064,20 +6112,26 @@
                 if cpu.get('proc_status') == 1:
                     # 在位
                     name = 'CPU' + str(cpu.get('proc_id', 0))
                     cpu_singe.CommonName(name)
                     cpu_singe.Location('mainboard')
                     if 'proc_name' in cpu:
                         cpu_singe.Model(cpu.get('proc_name'))
+                    else:
+                        cpu_singe.Model(cpu.get(None))
+                    if "Manufacturer" in cpu:
+                        cpu_singe.Manufacturer(cpu.get('Manufacturer', None))
+                    elif 'proc_name' in cpu:
                         if 'Intel' in cpu.get('proc_name'):
-                            cpu_singe.Manufacturer('Intel')
+                            cpu_singe.Manufacturer('Intel(R) Corporation')
+                        elif 'AMD' in cpu.get('proc_name'):
+                            cpu_singe.Manufacturer('AMD')
                         else:
                             cpu_singe.Manufacturer(None)
                     else:
-                        cpu_singe.Model(cpu.get(None))
                         cpu_singe.Manufacturer(None)
 
                     cpu_singe.L1CacheKiB(cpu.get('proc_l1cache_size', None))
                     cpu_singe.L2CacheKiB(cpu.get('proc_l2cache_size', None))
                     cpu_singe.L3CacheKiB(cpu.get('proc_l3cache_size', None))
                     # 通过sensor获取cpu_DTS_Temp
                     sensor = IpmiFunc.getSensorByNameByIpmi(
@@ -6221,17 +6275,15 @@
                                 'mem_mod_socket_num', 0))
                     else:
                         name = memory.get('mem_mod_slot', None)
                     memory_singe.CommonName(name)
                     memory_singe.Location('mainboard')
                     memory_singe.Manufacturer(
                         memory.get('mem_mod_vendor', None))
-                    memory_singe.CapacityMiB(
-                        memory.get('mem_mod_size') *
-                        1024 if 'mem_mod_size' in memory else None)
+                    memory_singe.CapacityGiB(memory.get('mem_mod_size') if 'mem_mod_size' in memory else None)
                     memory_singe.OperatingSpeedMhz(
                         memory.get('mem_mod_frequency', None))
                     memory_singe.CurrentSpeedMhz(memory.get('mem_mod_current_frequency', None))
                     memory_singe.AssetTag(memory.get('mem_mod_asset_tag', None))
                     memory_singe.SerialNumber(
                         memory.get('mem_mod_serial_num', None))
                     memory_singe.MemoryDeviceType(
@@ -6431,15 +6483,15 @@
         hard_info = RestFunc.getHardDiskInfoByRest(client)
         if hard_info == {}:
             result.State('Failure')
             result.Message(['get hard disk info failed'])
         elif hard_info.get('code') == 0 and hard_info.get('data') is not None:
             hard_data = hard_info.get('data')
             hard_dict = {0: 'No', 1: 'Yes'}
-            FrontRear_dict = {1: 'Front', 0: 'Rear'}
+            FrontRear_dict = {1: 'Front', 0: 'Rear', 2: 'Onboard', 3: 'Inner'}
             hardList = []
             idx = 0
             while idx < len(hard_data):
                 hard_result = HardBackBean()
                 hsrd_info = hard_data[idx]
                 hard_result.Id(hsrd_info.get('h_id', None))
                 hard_result.Present(hard_dict.get(hsrd_info.get('present', 0)))
@@ -6549,16 +6601,22 @@
                     hdd_dict['Model'] = str(item['model']).strip()
                 if "SN" in item:
                     hdd_dict['SN'] = str(item['SN']).strip()
                 if "firmware" in item:
                     hdd_dict['Firmware'] = str(item['firmware']).strip()
                 if "location" in item:
                     hdd_dict['Location'] = str(item['location']).strip()
+                    # 比M6多位置字段
+                if "locationstring" in item:
+                    hdd_dict['Location'] = str(item['locationstring']).strip()
                 if "manufacture" in item:
                     hdd_dict['Manufacture'] = str(item['manufacture']).strip()
+                if "capablespeed" in item:
+                    # 比M6多最大速率字段
+                    hdd_dict['CapableSpeed'] = str(item['capablespeed']).strip()
                 hdd_list.append(hdd_dict)
             result.State("Success")
             result.Message(hdd_list)
         else:
             result.State("Failure")
             result.Message(["get hard disk info error, error info: " + str(hdd_info.get('data'))])
         RestFunc.logout(client)
@@ -6583,15 +6641,18 @@
             back_data = back_info.get('data')
             back_dict = {0: 'No', 1: 'Yes'}
             backList = []
             idx = 0
             while idx < len(back_data):
                 back_result = BackplaneBean()
                 back_info = back_data[idx]
-                back_result.Id(back_info.get('backplane_index', None))
+                if "backplane_index" in back_info:
+                    back_result.Id(back_info.get('backplane_index', None))
+                else:
+                    back_result.Id(back_info.get('id', None))
                 back_result.Present(back_dict.get(back_info.get('present', 0)))
                 back_result.CPLDVersion(back_info.get('cpld_version', None))
                 back_result.PortCount(back_info.get('port_count', 0))
                 back_result.DriverCount(back_info.get('driver_count', 0))
                 back_result.Temperature(back_info.get('temperature', None))
                 back_result.Location(back_info.get('front', None))
                 idx += 1
@@ -6603,14 +6664,19 @@
             result.Message(
                 ["get disk back plane info error, error code " + str(back_info.get('code'))])
 
         RestFunc.logout(client)
         return result
 
     def getpcie(self, client, args):
+        def gethex(id):
+            if id:
+                return hex(id)
+            else:
+                return None
         headers = RestFunc.login_M6(client)
         if headers == {}:
             login_res = ResultBean()
             login_res.State("Failure")
             login_res.Message(
                 ["login error, please check username/password/host/port"])
             return login_res
@@ -6628,27 +6694,34 @@
             List = []
             for i in range(size):
                 if data[i] == {}:
                     continue
                 pcie = Pcie()
                 pcie.Id(data[i].get('id', i))
                 pcie.CommonName(data[i].get('DeviceLocator'))
-                pcie.Location('mainboard')
+                pcie.Location(data[i].get('DeviceLocator'))
                 if data[i].get('present', None) == 1:
                     pcie.Type(ListPCIEDevType[data[i].get('dev_type')] if data[i].get(
                         'dev_type') is not None else None)
                     pcie.SlotBus(hex(data[i].get('bus_num'))
                                  if 'bus_num' in data[i] else None)
                     pcie.SlotDevice(
                         hex(data[i].get('dev_num')) if 'dev_num' in data[i] else None)
                     pcie.SlotFunction(
                         hex(data[i].get('func_num')) if 'func_num' in data[i] else None)
                     pcie.State('Enabled')
                     pcie.DeviceID(data[i].get('device_name', None))
                     pcie.VendorID(data[i].get('vendor_name', None))
+                    pcie.State('Present')
+                    pcie.DeviceName(data[i].get('device_name', None))
+                    pcie.DeviceID(gethex(data[i].get('device_id', None)))
+                    pcie.SubDeviceID(gethex(data[i].get('sub_device_id', None)))
+                    pcie.VendorName(data[i].get('vendor_name', None))
+                    pcie.VendorID(gethex(data[i].get('vendor_id', None)))
+                    pcie.SubVendorID(gethex(data[i].get('sub_vendor_id', None)))
                     pcie.RatedLinkSpeed("GEN" +
                                         str(data[i].get('max_link_speed', 0)))
                     pcie.RatedLinkWidth("X" +
                                         str(data[i].get('max_link_width', 0)))
                     pcie.CurrentLinkSpeed(
                         "GEN" + str(data[i].get('current_link_speed', 0)))
                     pcie.CurrentLinkWidth(
@@ -6709,19 +6782,19 @@
                 "Unknown": "NA",
                 255: "NA"}
             nicRes.State("Success")
             PCIElist = []
             data = res.get('data')['sys_adapters']
             for ada in data:
                 PCIEinfo = NICBean()
-                PCIEinfo.CommonName(ada['location'])
+                PCIEinfo.CommonName(ada.get('location', 'NA'))
                 PCIEinfo.Location("mainboard")
                 adapterinfo = NICController()
                 adapterinfo.Id(ada['id'])
-                adapterinfo.Location(ada['location'])
+                adapterinfo.Location(ada.get('location', 'NA'))
                 if ada['vendor'] == "":
                     adapterinfo.Manufacturer(None)
                     PCIEinfo.Manufacturer(None)
                 else:
                     if "0x" in ada['vendor']:
                         maf = PCI_IDS_LIST.get(
                             int(ada['vendor'], 16), ada['vendor'])
@@ -11403,15 +11476,15 @@
                         return res
                 set_res = IpmiFunc.setPsuConfigByIpmi(client, set_cmd)
                 if set_res.get('code') == 0:
                     res.State("Success")
                     res.Message(["set psu config success."])
                 else:
                     res.State("Failure")
-                    res.Message(["set psu config failed."])
+                    res.Message([str(set_res.get('data'))])
             else:
                 res.State("Failure")
                 res.Message(["get psu count failed."])
         except Exception as e:
             res.State("Failure")
             res.Message([str(e)])
         return res
@@ -11673,15 +11746,15 @@
 
         res = ResultBean()
         try:
             login_header, login_id = RedfishFunc.login(client)
             if login_header == {} or "login error" in login_id or login_id == '':
                 res.State("Failure")
                 res.Message(['login session service failed.'])
-                return
+                return res
 
             local_time = ftime()
             file_name_init = str(args.host) + "_bios_" + str(local_time) + ".conf"
             if args.fileurl == ".":
                 file_name = file_name_init
                 file_path = os.path.abspath(".")
             elif args.fileurl == "..":
@@ -13328,15 +13401,15 @@
                     args.access = 1
                 user_old["access"] = args.access
                 user_old["group_name"] = args.group
             user_old["UserOperation"] = 1
             user_old["changepassword"] = 0
             user_old["confirm_password"] = ""
             user_old["password"] = ""
-            user_old["session_confirm"] = ""
+            user_old["session_confirm"] = client.passcode
 
             user_old["password_size"] = "bytes_16"
             user_old["email_format"] = "ami_format"
             if args.email is not None:
                 user_old["email_id"] = args.email
             else:
                 user_old["email_id"] = ''
```

### Comparing `inManage-1.0.0/inmanage_sdk/interface/CommonM6_41401.py` & `inManage-1.0.1/inmanage_sdk/interface/CommonM6_41401.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/CommonM6_4140a.py` & `inManage-1.0.1/inmanage_sdk/interface/CommonM6_4140a.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/CommonM7.py` & `inManage-1.0.1/inmanage_sdk/interface/CommonM7.py`

 * *Files 2% similar despite different names*

```diff
@@ -458,25 +458,26 @@
         # get
         # res=RestFunc.getAdapterByRest(client)
         res = RestFunc.getAdapterByRest(client)
         if res == {}:
             nicRes.State("Failure")
             nicRes.Message(["cannot get information"])
         elif res.get('code') == 0 and res.get('data') is not None:
-            port_status_dict = {0: "Not Linked", 1: "Linked", 2: "NA", "Unknown": "NA", 255: "NA"}
+            # port_status_dict = {0: "Not Linked", 1: "Linked", 2: "NA", "Unknown": "NA", 255: "NA"}
             nicRes.State("Success")
             PCIElist = []
             data = res.get('data')['sys_adapters']
             for ada in data:
                 PCIEinfo = NICBean()
                 PCIEinfo.CommonName(ada['location'])
                 PCIEinfo.Location("mainboard")
                 adapterinfo = NICController()
                 adapterinfo.Id(ada['id'])
-                adapterinfo.Location(ada['location'])
+                adapterinfo.Location(ada.get('location', 'NA'))
+                adapterinfo.PortType(ada.get('port_type', 'NA'))
                 if ada['vendor'] == "":
                     adapterinfo.Manufacturer(None)
                     PCIEinfo.Manufacturer(None)
                 else:
                     if "0x" in ada['vendor']:
                         maf = PCI_IDS_LIST.get(int(ada['vendor'], 16), ada['vendor'])
                         adapterinfo.Manufacturer(maf)
@@ -502,15 +503,16 @@
                 ports = ada.get('ports', [])
                 adapterinfo.PortCount(len(ports))
                 portlist = []
                 for port in ports:
                     portBean = NicPort()
                     portBean.Id(port['id'])
                     portBean.MACAddress(port['mac_addr'])
-                    portBean.LinkStatus(port_status_dict.get(port['status'], port['status']))
+                    # portBean.LinkStatus(port_status_dict.get(port['status'], port['status']))
+                    portBean.LinkStatus(port.get('LinkStatus', "N/A"))
                     portBean.MediaType(None)
                     portlist.append(portBean.dict)
                 adapterinfo.Port(portlist)
                 controllerList = []
                 controllerList.append(adapterinfo.dict)
                 # PCIEinfo.Serialnumber(ada['serial_num'])
                 if 'serial_num' in ada:
@@ -533,15 +535,15 @@
         else:
             nicRes.State("Failure")
             nicRes.Message(["get information error, error code " + str(res.get('code'))])
 
         RestFunc.logout(client)
         return nicRes
 
-    def getgpu(self, client, args):
+    def getgpu1(self, client, args):
         res = ResultBean()
         state = "Failure"
         gpu_device_class_type = ["DisplayController", "ProcessingAccelerator"]
         id_res = RedfishFunc.getChassisID(client)
         if id_res.get('code') == 0 and id_res.get('data') is not None:
             id_data = id_res.get('data')
             id_url = None
@@ -575,14 +577,36 @@
                 message = "No chassis id."
         else:
             message = "Cannot get chassis id."
         res.State(state)
         res.Message([message])
         return res
 
+    def getgpu(self, client, args):
+        headers = RestFunc.login_M6(client)
+        if headers == {}:
+            login_res = ResultBean()
+            login_res.State("Failure")
+            login_res.Message(["login error, please check username/password/host/port"])
+            return login_res
+        client.setHearder(headers)
+        res = ResultBean()
+
+        gpures = RestFunc.getgpu(client)
+        if gpures.get('code') == 0:
+            res.State('Success')
+            gpurawinfo = gpures.get('data')
+            res.Message([gpurawinfo])
+        else:
+            res.State('Failure')
+            res.Message(['get gpu information failed.' + str(gpures.get('date'))])
+        # logout
+        RestFunc.logout(client)
+        return res
+
     def setpowerbudget(self, client, args):
         import collections
 
         def getSuspend(start, end, week_str):
             if start is not None and end is not None and week_str is not None:
                 if start > 24 or start < 0:
                     value = 'Invalid start, start range from 0-24'
@@ -853,14 +877,17 @@
                     res.Message([""])
             except Exception as e:
                 res.State("Failure")
                 res.Message(["File content must be in json format."])
             return res
 
     def getbios(self, client, args):
+        #获取bios版本 放在args里面
+        self._get_bios_version(client, args)
+
         bios_result = ResultBean()
         login_header, login_id = RedfishFunc.login(client)
         if not login_header or not login_id or 'login error' in login_id:
             bios_result.State('Failure')
             bios_result.Message(['login session service failed, please check username/password/host/port'])
             return bios_result
         args.Attribute = None
@@ -958,17 +985,23 @@
                 index = int(user_key[-1:]) - 1
                 return value_map.get(origin_value[index], origin_value[index])
             else:
                 return [value_map.get(str(value), str(value)) for value in origin_value]
         elif isinstance(origin_value, dict):
             return {k: value_map.get(str(v), str(v)) for k, v in origin_value}
         else:
-            return value_map.get(str(origin_value), None)
+            if len(value_map) == 1:
+                return origin_value
+            else:
+                return value_map.get(str(origin_value), None)
 
     def setbios(self, client, args):
+        #获取bios版本 放在args里面
+        self._get_bios_version(client, args)
+
         res = ResultBean()
         attr_dict = {}
         # 读取映射文件
         mapper_result = self._get_xml_mapper(args, 'value', 'cmd')
         # args.list = False
         if mapper_result[0]:
             if 'list' in args and args.list:  # 打印信息
@@ -1014,15 +1047,15 @@
                 return res
             # 校验值并转换
             item_dict = attr_dict[key.lower().replace(" ","")]
             attr = item_dict['getter']
             attr_setter = item_dict['setter']
             attr_parent = item_dict['parent']
             #list的3种处理方式 {0:"x", 1:"y"} [x,y,...] x
-            if item_dict['type'] == 'list':
+            if item_dict.get('list') > 0:
                 if isinstance(value, dict):
                     for k, v in value.items():  # 根据目前支持的配置项，值统一处理为str
                         user_bios[attr + str(k)] = str(attr_setter[v])
                 elif isinstance(value, list):
                     for i in range(len(value)):
                         user_bios[attr + str(i)] = str(attr_setter[value[i]])
                 elif isinstance(value, str):
@@ -1038,23 +1071,44 @@
                             return res
                     elif "[" in value:
                         valueinlist = value[1:-1].split(",")
                         for i in range(len(valueinlist)):
                             user_bios[attr + str(i)] = str(attr_setter[valueinlist[i]])
 
             else:
-                if item_dict['match'] and value not in attr_setter:
-                    res.Message(['[{}] is invalid value for bios option [{}], and valid values are [{}].'
-                                .format(value, key, ', '.join(list(attr_setter.keys())))])
-                    res.State('Failure')
-                    return res
+                if len(attr_setter) == 1:
+                    #类型
+                    for valuerange in attr_setter.keys():
+                        if "-" in valuerange:
+                            min = int(valuerange.split("-")[0])
+                            max = int(valuerange.split("-")[1])
+                        elif "~" in valuerange:
+                            min = int(valuerange.split("~")[0])
+                            max = int(valuerange.split("~")[1])
+                        else:
+                            res.Message([
+                                            '[{}] is invalid range value for bios option [{}], range should be a~b or a-b.'
+                                        .format(valuerange, key)])
+                            res.State('Failure')
+                            return res
+                        if int(value) < min or int(value) > max:
+                            res.Message(
+                                ['[{}] is invalid value for bios option [{}], and valid values are [{}].'
+                                .format(value, key, valuerange)])
+                            res.State('Failure')
+                            return res
 
-                if item_dict['type'] == 'int':  # 根据目前支持的配置项，处理int、str两种类型
-                    user_bios[attr] = int(attr_setter.get(value, value))
+                        user_bios[attr] = int(value)
                 else:
+                    if item_dict['match'] and value not in attr_setter:
+                        res.Message(['[{}] is invalid value for bios option [{}], and valid values are [{}].'
+                                    .format(value, key, ', '.join(list(attr_setter.keys())))])
+                        res.State('Failure')
+                        return res
+
                     user_bios[attr] = str(attr_setter.get(value, value))
 
         # 调用接口设置
         login_header, login_id = RedfishFunc.login(client)
         if not login_header or not login_id or 'login error' in login_id:
             res.Message(['login session service failed, please check username/password/host/port'])
             res.State('Failure')
@@ -1137,45 +1191,81 @@
             res.State('Failure')
         RedfishFunc.logout(client, login_id, login_header)
         return res
 
     def formatBiosPatchBody(self, user_bios):
         return user_bios
 
-    def _get_xml_file(self):
+    def _get_bios_version(self, client, args):
+        biosversion = None
+        # login
+        headers = RestFunc.login_M6(client)
+        if headers == {}:
+            args.biosversion = biosversion
+            return biosversion
+        client.setHearder(headers)
+        # get
+        res = RestFunc.getFwVersion(client)
+        if res.get('code') == 0 and res.get('data') is not None:
+            data = res.get('data')
+
+            for fwinfo in data:
+                name_raw = fwinfo.get('dev_name')
+                if name_raw != "BIOS":
+                    continue
+                else:
+                    index_version = fwinfo.get('dev_version').find('(')
+                    if index_version == -1:
+                        biosversion = None if fwinfo.get('dev_version') == '' else fwinfo.get('dev_version')
+                    else:
+                        biosversion = None if fwinfo.get('dev_version') == '' else fwinfo.get('dev_version')[:index_version].strip()
+                    break
+        args.biosversion = biosversion
+        RestFunc.logout(client)
+        return biosversion
+
+    def _get_xml_file(self, args):
         xml_path = os.path.join(IpmiFunc.command_path, "bios") + os.path.sep
+        if args.biosversion:
+            #M7 5.10.00 开始 bios里面替换为 XCradle
+            b1=args.biosversion.split(".")[0]
+            b2=args.biosversion.split(".")[1]
+            b3=args.biosversion.split(".")[2]
+            biosformat = float(b1 + "." + b2 + b3)
+            if biosformat >= 5.1000:
+                return xml_path + 'M7_5.10.00.xml'
         return xml_path + 'M7.xml'
 
     def _get_xml_mapper(self, args, key, value):
         """
             {
                 'descriptionName': {
                     'description': 'descriptionName',
-                    'type': 'int/str/list/dict',
+                    'list': 64,
                     'match': True/False,
                     'parent': 'server_bios_parent_key',
                     'getter': 'server_bios_key',
                     'setter': {
                         'cmd': 'value' 或 'value': 'cmd' 根据参数确定
                     }
                 }
             }
         """
         try:
             #xml_filepath = sys.path[0] + '/mappers/bios/M7.xml'
-            xml_filepath = self._get_xml_file()
+            xml_filepath = self._get_xml_file(args)
             import xml.etree.ElementTree as ET
             tree = ET.parse(xml_filepath)
             server = tree.getroot()
             map_dict = {}
             for items in server:
                 for item in items:
                     map_dict[item.find('name').find('description').text.lower().replace(" ", "")] = {
                         'description': item.find('name').find('description').text,
-                        'type': 'str' if item.find('type') is None else item.find('type').text,
+                        'list': 0 if item.find('list') is None else int(item.find('list').text),
                         'match': True if item.find('match') is None else False if item.find(
                             'match').text == 'False' else True,
                         'parent': None if item.find('parent') is None else item.find('parent').text,
                         'getter': item.find('getter').text,
                         'setter': {
                             setter.find(key).text: setter.find(value).text for setter in item.find('setters')
                         },
@@ -1203,15 +1293,15 @@
                         'getter': 'cmd'
                     }
                 }
             }
         """
         try:
             #xml_filepath = sys.path[0] + '/mappers/bios/M7.xml'
-            xml_filepath = self._get_xml_file()
+            xml_filepath = self._get_xml_file(args)
             import xml.etree.ElementTree as ET
             tree = ET.parse(xml_filepath)
             server = tree.getroot()
             map_dict = {}
             for items in server:
                 for item in items:
                     map_dict[item.find('getter').text] = {
@@ -1257,17 +1347,30 @@
         condition_dict = {}
         # getter: description
         bios_dict = {}
         # getter: {cmd: value}
         bios_value_dict = {}
         errordict={}
         for bioskey, biosvalue in bios_set.items():
-            conditions = bios_all_info.get(bioskey).get("conditions")
+            conditions = bios_all_info.get(bioskey, {}).get("conditions", {})
             errorlist = []
             errorinfo = ""
+            #如果和当前值相等 不需要考虑condition
+            bioskeyparent = bios_all_info.get(bioskey, {}).get("parent")
+            if bioskeyparent:
+                if bioskeyparent == "FixedBootPriorities":
+                    #如果是启动项，可能获取方式有区别
+                    bioskeylistname = bioskey[0:-1]
+                    bioskeylistid = bioskey[-1]
+                    if bios_set.get(bioskey) == bios_cur.get(bioskeyparent, {}).get(bioskeylistname, [])[int(bioskeylistid)]:
+                        continue
+                else:
+                    if bios_cur.get(bioskeyparent, {}).get(bioskey) == bios_set.get(bioskey):
+                        continue
+
             for conditionkey,conditionvalue in conditions.items():
                 condition_bios_info = bios_all_info.get(conditionkey)
                 #condition 的 isrest 展示 key
                 conditionkeyshow = condition_bios_info.get("description")
                 #{bmc value: isrest value}
                 conditionvaluedict = condition_bios_info.get("setter")
                 conditionvalueshow = conditionvaluedict.get(conditionvalue, conditionvalue)
@@ -1294,14 +1397,15 @@
                     if conditonvalue_future:
                         if conditionvalue == conditonvalue_future:
                             continue
                         else:
                             errorlist.append(self.formatCondition(conditionkeyshow, conditionvalueshow, conditionvaluedict.get(conditonvalue_future), 2))
                             continue
                 #比较当前值
+                conditonvalue_current = None
                 if bios_cur.get(conditionkey):
                     conditonvalue_current = bios_cur.get(conditionkey)
                 elif bios_cur.get(conditionparent):
                     conditonvalue_current = bios_cur.get(conditionparent).get(conditionkey)
                 if conditonvalue_current:
                     if conditionvalue == conditonvalue_current:
                         continue
@@ -2484,17 +2588,19 @@
                         'Automatic' if mode.get('data').get('control_mode') == 'auto' else 'Manual')
                 else:
                     fan_Info.FanSpeedAdjustmentMode(None)
             # 通过sensor获取Fan_Power
             sensor = IpmiFunc.getSensorByNameByIpmi(client, 'Fan_Power')
             if sensor and sensor.get('code') == 0:
                 temp = sensor.get('data')[0].get('value')
-                fan_Info.FanTotalPowerWatts(float(temp) if (temp is not None and temp != 'na') else None)
-            else:
-                fan_Info.FanTotalPowerWatts(None)
+                if temp is not None and temp != 'na':
+                    fan_Info.FanTotalPowerWatts(float(temp))
+            #     fan_Info.FanTotalPowerWatts(float(temp) if (temp is not None and temp != 'na') else None)
+            # else:
+            #     fan_Info.FanTotalPowerWatts(None)
             fan_Info.FanManualModeTimeoutSeconds(None)
             fan_Info.Fan(list)
             result.State('Success')
             result.Message([fan_Info.dict])
         elif res.get('code') != 0 and res.get('data') is not None:
             result.State("Failure")
             result.Message(["get fan information error, " + res.get('data')])
@@ -4654,551 +4760,14 @@
         else:
             result.State("Failure")
             result.Message([set_res.get('data')])
 
         RestFunc.logout(client)
         return result
 
-    #2023年1月29日 大概是PFR专用 暂时删除
-    '''
-    def getldapgroup(self, client, args):
-        result = ResultBean()
-        # login
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-
-        res = RestFunc.getLDAPgroupM6(client)
-        if res.get('code') == 0 and res.get('data') is not None:
-            ldap_group = res.get('data')
-            ldap_group_list = []
-            for group in ldap_group:
-                ldap_res = collections.OrderedDict()
-                ldap_res['Id'] = group['id']
-                ldap_res['Name'] = group['role_group_name']
-                ldap_res['Domain'] = group['role_group_domain']
-                ldap_res['Privilege'] = group['role_group_withoem_privilege']
-                ldap_res['KVM Access'] = "Enabled" if group['role_group_kvm_privilege'] == 1 else "Disabled"
-                ldap_res['VMedia Access'] = "Enabled" if group['role_group_vmedia_privilege'] == 1 else "Disabled"
-                ldap_group_list.append(ldap_res)
-            result.State("Success")
-            result.Message([{"LDAPgroup": ldap_group_list}])
-        else:
-            result.State("Failure")
-            result.Message([res.get('data')])
-
-        RestFunc.logout(client)
-        return result
-
-    def addldapgroup(self, client, args):
-        def checkGroupName(name):
-            # 角色组名称是一个64字母数字组成的字串。
-            # 允许特殊字符如连字符和下划线。
-            dn = '^[\da-zA-Z\-_]{1,64}$'
-            if re.search(dn, name, re.I):
-                return True
-            return False
-
-        def checkDoamin(s):
-            # 域名名称是一个64字母数字组成的字串。
-            # 开头字符必须是字母。
-            # 允许特殊字符如点(.)，逗号(,)，连字符(-)，下划线(_)，等于号(=)。
-            # 范例: cn=manager,ou=login, dc=domain,dc=com
-            dn = '^[a-zA-Z][a-zA-Z\-_\.\,\=]{4,64}$'
-            if re.search(dn, s, re.I):
-                return True
-            return False
-
-        result = ResultBean()
-
-        if args.name is not None:
-            if not checkGroupName(args.name):
-                result.State("Failure")
-                result.Message([
-                    'Group name is a string of less than 64 alpha-numeric characters, and hyphen and underscore are also allowed.'])
-                return result
-
-        if args.domain is not None:
-            if not checkDoamin(args.domain):
-                result.State("Failure")
-                result.Message([
-                    'Domain Name is a string of 4 to 64 alpha-numeric characters.It must start with an alphabetical character.Special Symbols like dot(.), comma(,), hyphen(-), underscore(_), equal-to(=) are allowed.Example: cn=manager,ou=login,dc=domain,dc=com'])
-                return result
-
-        # login
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-
-        name_exist_flag = False
-        add_flag = False
-        res = RestFunc.getLDAPgroupM6(client)
-        if res.get('code') == 0 and res.get('data') is not None:
-            for item in res.get('data'):
-                name = item.get('role_group_name', "unknown")
-                if name == args.name:
-                    name_exist_flag = True
-                    break
-                if name == "":
-                    add_flag = True
-                    args.id = item.get('id', 0)
-                    break
-        else:
-            result.State("Failure")
-            result.Message([res.get('data')])
-            RestFunc.logout(client)
-            return result
-
-        if name_exist_flag:
-            result.State("Failure")
-            result.Message(['Group ' + args.name + ' is already exist.'])
-            RestFunc.logout(client)
-            return result
-
-        if not add_flag:
-            result.State("Failure")
-            result.Message(['LDAP role group is full.'])
-            RestFunc.logout(client)
-            return result
-
-        kvm_vm = {"enable": 1, "disable": 0}
-        # priv administrator user operator oem none
-        ldapgroup = {
-            'id': args.id,
-            'role_group_domain': args.domain,
-            'role_group_kvm_privilege': kvm_vm.get(args.kvm.lower()),
-            'role_group_name': args.name,
-            'role_group_withoem_privilege': args.pri,
-            'role_group_vmedia_privilege': kvm_vm.get(args.vm.lower()),
-            'role_group_privilege': "none"
-        }
-        # print(ldapgroup)
-        set_res = RestFunc.setLDAPgroupM6(client, ldapgroup)
-        if set_res.get('code') == 0 and set_res.get('data') is not None:
-            result.State("Success")
-            result.Message(["Add LDAP group success."])
-        else:
-            result.State("Failure")
-            result.Message([set_res.get('data')])
-
-        RestFunc.logout(client)
-        return result
-
-    def setldapgroup(self, client, args):
-
-        def checkGroupName(name):
-            # 角色组名称是一个64字母数字组成的字串。
-            # 允许特殊字符如连字符和下划线。
-            dn = '^[\da-zA-Z\-_]{1,64}$'
-            if re.search(dn, name, re.I):
-                return True
-            return False
-
-        def checkDoamin(s):
-            # 域名名称是一个64字母数字组成的字串。
-            # 开头字符必须是字母。
-            # 允许特殊字符如点(.)，逗号(,)，连字符(-)，下划线(_)，等于号(=)。
-            # 范例: cn=manager,ou=login, dc=domain,dc=com
-            dn = '^[a-zA-Z][a-zA-Z\-_\.\,\=]{4,64}$'
-            if re.search(dn, s, re.I):
-                return True
-            return False
-
-        result = ResultBean()
-        # login
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-
-        name_exist_flag = False
-        res = RestFunc.getLDAPgroupM6(client)
-        ldapgroup = None
-        if res.get('code') == 0 and res.get('data') is not None:
-            for item in res.get('data'):
-                id = str(item.get('id', 0))
-                if id == args.id:
-                    ldapgroup = item
-                else:
-                    name = item.get('role_group_name', "unknown")
-                    if name == args.name:
-                        name_exist_flag = True
-                        break
-        else:
-            result.State("Failure")
-            result.Message([res.get('data')])
-            RestFunc.logout(client)
-            return result
-
-        if name_exist_flag:
-            result.State("Failure")
-            result.Message(['Group ' + args.name + ' is already exist.'])
-            RestFunc.logout(client)
-            return result
-
-        if ldapgroup is None:
-            result.State("Failure")
-            result.Message(['Group id is not exist.' + res.get('data')])
-            RestFunc.logout(client)
-            return result
-
-        if args.name is not None:
-            if checkGroupName(args.name):
-                ldapgroup['role_group_name'] = args.name
-            else:
-                result.State("Failure")
-                result.Message([
-                    'Group name is a string of less than 64 alpha-numeric characters, and hyphen and underscore are also allowed.'])
-                RestFunc.logout(client)
-                return result
-        if ldapgroup['role_group_name'] == "":
-            result.State("Failure")
-            result.Message(['Group name is needed.'])
-            RestFunc.logout(client)
-            return result
-
-        if args.domain is not None:
-            if checkDoamin(args.domain):
-                ldapgroup['role_group_domain'] = args.domain
-            else:
-                result.State("Failure")
-                result.Message([
-                    'Domain Name is a string of 4 to 64 alpha-numeric characters.It must start with an alphabetical character.Special Symbols like dot(.), comma(,), hyphen(-), underscore(_), equal-to(=) are allowed.Example: cn=manager,ou=login,dc=domain,dc=com'])
-                RestFunc.logout(client)
-                return result
-        if ldapgroup['role_group_domain'] == "":
-            result.State("Failure")
-            result.Message(['Group domain is needed.'])
-            RestFunc.logout(client)
-            return result
-
-        if args.pri is not None:
-            ldapgroup['role_group_withoem_privilege'] = args.pri
-        if ldapgroup['role_group_withoem_privilege'] == "":
-            result.State("Failure")
-            result.Message(['Group privilege is needed.'])
-            RestFunc.logout(client)
-            return result
-
-        kvm_vm = {"enable": 1, "disable": 0}
-        if args.kvm is not None:
-            ldapgroup['role_group_kvm_privilege'] = kvm_vm.get(args.kvm.lower())
-
-        if args.vm is not None:
-            ldapgroup['role_group_vmedia_privilege'] = kvm_vm.get(args.vm.lower())
-
-        # print(ldapgroup)
-        set_res = RestFunc.setLDAPgroupM6(client, ldapgroup)
-        if set_res.get('code') == 0 and set_res.get('data') is not None:
-            result.State("Success")
-            result.Message(["Set LDAP group success."])
-        else:
-            result.State("Failure")
-            result.Message([set_res.get('data')])
-
-        RestFunc.logout(client)
-        return result
-
-    def getadgroup(self, client, args):
-        result = ResultBean()
-        # login
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-
-        res = RestFunc.getADgroupM6(client)
-        if res.get('code') == 0 and res.get('data') is not None:
-            ldap_group = res.get('data')
-            ldap_group_list = []
-            for group in ldap_group:
-                ldap_res = collections.OrderedDict()
-                ldap_res['Id'] = group['id']
-                ldap_res['Name'] = group['role_group_name']
-                ldap_res['Domain'] = group['role_group_domain']
-                ldap_res['Privilege'] = group['role_group_withoem_privilege']
-                ldap_res['KVM Access'] = "Enabled" if group['role_group_kvm_privilege'] == 1 else "Disabled"
-                ldap_res['VMedia Access'] = "Enabled" if group['role_group_vmedia_privilege'] == 1 else "Disabled"
-                ldap_group_list.append(ldap_res)
-            result.State("Success")
-            result.Message([{"ADgroup": ldap_group_list}])
-        else:
-            result.State("Failure")
-            result.Message([res.get('data')])
-
-        RestFunc.logout(client)
-        return result
-
-    def addadgroup(self, client, args):
-        def checkGroupName(name):
-            # 角色组名称是一个64字母数字组成的字串。
-            # 允许特殊字符如连字符和下划线。
-            dn = '^[\da-zA-Z\-_]{1,64}$'
-            if re.search(dn, name, re.I):
-                return True
-            return False
-
-        # def checkDoamin(s):
-        #     # 域名名称是一个64字母数字组成的字串。
-        #     # 开头字符必须是字母。
-        #     # 允许特殊字符如点(.)，逗号(,)，连字符(-)，下划线(_)，等于号(=)。
-        #     # 范例: cn=manager,ou=login, dc=domain,dc=com
-        #     dn = '^[a-zA-Z][a-zA-Z\-_\.\,\=]{4,64}$'
-        #     if re.search(dn, s, re.I):
-        #         return True
-        #     return False
-        def checkDoamin(s):
-            dn = '^([\da-zA-Z]+[\w\-]*\.)*([\da-zA-Z]+[\w\-]*)+\.([\da-zA-Z]+[\w\-]*)+$'
-            dnd = '^([\d]+\.)*[\d]+\.[\d]+$'
-            if re.search(dn, s, re.I) and not re.search(dnd, s, re.I):
-                return True
-            return False
-
-        result = ResultBean()
-        if args.name is not None:
-            if not checkGroupName(args.name):
-                result.State("Failure")
-                result.Message([
-                    'Group name is a string of less than 64 alpha-numeric characters, and hyphen and underscore are also allowed.'])
-                return result
-
-        if args.domain is not None:
-            if not checkDoamin(args.domain):
-                result.State("Failure")
-                result.Message([
-                    'Domain Name is a string of less than 255 alpha-numeric characters. '
-                    'It must start with an alphabetical character. '
-                    'Special Symbols like dot(.), hyphen(-), underscore(_) are allowed.'])
-                return result
-
-        # login
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-        result = ResultBean()
-
-        id_exist_flag = False
-        name_exist_flag = False
-        # add_flag = False
-        res = RestFunc.getADgroupM6(client)
-        if res.get('code') == 0 and res.get('data') is not None:
-            for item in res.get('data'):
-                name = item.get('role_group_name', "unknown")
-                if name == args.name:
-                    name_exist_flag = True
-                    break
-                id = item.get('id', "unknown")
-                if str(id) == args.id and name != "":
-                    id_exist_flag = True
-                    break
-                # if name == "":
-                #     add_flag = True
-                #     args.id = item.get('id', 0)
-                #     break
-        else:
-            result.State("Failure")
-            result.Message([res.get('data')])
-            RestFunc.logout(client)
-            return result
-
-        if id_exist_flag:
-            result.State("Failure")
-            result.Message(['the ID has group info already, please use "setADgroup" to edit it.'])
-            RestFunc.logout(client)
-            return result
-
-        if name_exist_flag:
-            result.State("Failure")
-            result.Message(['Group ' + args.name + ' is already exist.'])
-            RestFunc.logout(client)
-            return result
-
-        # if not add_flag:
-        #     result.State("Failure")
-        #     result.Message(['AD role group is full.'])
-        #     RestFunc.logout(client)
-        #     return result
-
-        kvm_vm = {"enable": 1, "disable": 0}
-        # priv administrator user operator none
-        adgroup = {
-            'id': args.id,
-            'role_group_domain': args.domain,
-            'role_group_kvm_privilege': kvm_vm.get(args.kvm.lower()),
-            'role_group_name': args.name,
-            'role_group_withoem_privilege': args.pri,
-            'role_group_vmedia_privilege': kvm_vm.get(args.vm.lower()),
-            'role_group_privilege': "none"
-        }
-        # print(adgroup)
-        set_res = RestFunc.setADgroupM6(client, adgroup)
-        if set_res.get('code') == 0 and set_res.get('data') is not None:
-            result.State("Success")
-            result.Message(["Add AD group success."])
-        else:
-            result.State("Failure")
-            result.Message([set_res.get('data')])
-
-        RestFunc.logout(client)
-        return result
-
-    def setadgroup(self, client, args):
-
-        def checkGroupName(name):
-            # 角色组名称是一个64字母数字组成的字串。
-            # 允许特殊字符如连字符和下划线。
-            dn = '^[\da-zA-Z\-_]{1,64}$'
-            if re.search(dn, name, re.I):
-                return True
-            return False
-
-        # def checkDoamin(s):
-        #     # 域名名称是一个64字母数字组成的字串。
-        #     # 开头字符必须是字母。
-        #     # 允许特殊字符如点(.)，逗号(,)，连字符(-)，下划线(_)，等于号(=)。
-        #     # 范例: cn=manager,ou=login, dc=domain,dc=com
-        #     dn = '^[a-zA-Z][a-zA-Z\-_\.\,\=]{4,64}$'
-        #     if re.search(dn, s, re.I):
-        #         return True
-        #     return False
-        def checkDoamin(s):
-            dn = '^([\da-zA-Z]+[\w\-]*\.)*([\da-zA-Z]+[\w\-]*)+\.([\da-zA-Z]+[\w\-]*)+$'
-            dnd = '^([\d]+\.)*[\d]+\.[\d]+$'
-            if re.search(dn, s, re.I) and not re.search(dnd, s, re.I):
-                return True
-            return False
-
-        result = ResultBean()
-        # login
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-
-        name_exist_flag = False
-        id_not_exit_flag = False
-        res = RestFunc.getADgroupM6(client)
-        adgroup = None
-        if res.get('code') == 0 and res.get('data') is not None:
-            for item in res.get('data'):
-                id = str(item.get('id', 0))
-                if id == args.id:
-                    name = item.get('role_group_name', "unknown")
-                    if name == "":
-                        id_not_exit_flag = True
-                        break
-                    adgroup = item
-                else:
-                    name = item.get('role_group_name', "unknown")
-                    if name == args.name:
-                        name_exist_flag = True
-                        break
-        else:
-            result.State("Failure")
-            result.Message([res.get('data')])
-            RestFunc.logout(client)
-            return result
-
-        if id_not_exit_flag:
-            result.State("Failure")
-            result.Message(['the ID has no group info yet, please use "addADgroup" to add it'])
-            RestFunc.logout(client)
-            return result
-
-        if name_exist_flag:
-            result.State("Failure")
-            result.Message(['Group ' + args.name + ' is already exist.'])
-            RestFunc.logout(client)
-            return result
-
-        if adgroup is None:
-            result.State("Failure")
-            result.Message(['Group id is not exist.' + res.get('data')])
-            RestFunc.logout(client)
-            return result
-
-        if args.name is not None:
-            if checkGroupName(args.name):
-                adgroup['role_group_name'] = args.name
-            else:
-                result.State("Failure")
-                result.Message([
-                    'Group name is a string of less than 64 alpha-numeric characters, and hyphen and underscore are also allowed.'])
-                RestFunc.logout(client)
-                return result
-        if adgroup['role_group_name'] == "":
-            result.State("Failure")
-            result.Message(['Group name is needed.'])
-            RestFunc.logout(client)
-            return result
-
-        if args.domain is not None:
-            if checkDoamin(args.domain):
-                adgroup['role_group_domain'] = args.domain
-            else:
-                result.State("Failure")
-                result.Message([
-                    'Domain Name is a string of 4 to 64 alpha-numeric characters.It must start with an alphabetical character.Special Symbols like dot(.), comma(,), hyphen(-), underscore(_), equal-to(=) are allowed.Example: cn=manager,ou=login,dc=domain,dc=com'])
-                RestFunc.logout(client)
-                return result
-        if adgroup['role_group_domain'] == "":
-            result.State("Failure")
-            result.Message(['Group domain is needed.'])
-            RestFunc.logout(client)
-            return result
-
-        if args.pri is not None:
-            adgroup['role_group_withoem_privilege'] = args.pri
-        if adgroup['role_group_withoem_privilege'] == "":
-            result.State("Failure")
-            result.Message(['Group privilege is needed.'])
-            RestFunc.logout(client)
-            return result
-
-        kvm_vm = {"enable": 1, "disable": 0}
-        if args.kvm is not None:
-            adgroup['role_group_kvm_privilege'] = kvm_vm.get(args.kvm.lower())
-
-        if args.vm is not None:
-            adgroup['role_group_vmedia_privilege'] = kvm_vm.get(args.vm.lower())
-
-        # print(adgroup)
-        set_res = RestFunc.setADgroupM6(client, adgroup)
-        if set_res.get('code') == 0 and set_res.get('data') is not None:
-            result.State("Success")
-            result.Message(["Set AD group success."])
-        else:
-            result.State("Failure")
-            result.Message([set_res.get('data')])
-
-        RestFunc.logout(client)
-        return result
-
-    '''
     def getmediainstance(self, client, args):
         result = ResultBean()
         # login
         headers = RestFunc.login_M6(client)
         if headers == {}:
             login_res = ResultBean()
             login_res.State("Failure")
@@ -5211,14 +4780,15 @@
             gs = res.get('data')
             media_instance = collections.OrderedDict()
             media_instance["CDNum"] = gs.get("num_cd")
             media_instance["HDNum"] = gs.get("num_hd")
             media_instance["KVMCDNum"] = gs.get("kvm_num_cd")
             media_instance["KVMHDNum"] = gs.get("kvm_num_hd")
             media_instance["SDMedia"] = "Enable" if gs.get("sd_media") == 1 else "Disable"
+            media_instance["SecureChannel"] = "Enable" if gs.get("secure_channel") == 1 else "Disable"
             media_instance["PowerSaveMode"] = "Enable" if gs.get("power_save_mode") == 1 else "Disable"
             result.State("Success")
             result.Message([{"Instance": media_instance}])
         else:
             result.State("Failure")
             result.Message([res.get('data')])
 
@@ -5310,15 +4880,15 @@
             login_res = ResultBean()
             login_res.State("Failure")
             login_res.Message(["login error, please check username/password/host/port"])
             return login_res
         client.setHearder(headers)
 
         RestFunc.securityCheckByRest(client)
-        res = RestFunc.resetBMCM6(client, args.type)
+        res = RestFunc.resetBMCM7(client, args.type)
         if res.get('code') == 0 and res.get('data') is not None:
             result.State("Success")
             result.Message([res.get('data')])
         else:
             result.State("Failure")
             result.Message([res.get('data')])
 
@@ -5470,15 +5040,18 @@
                     psu_Info.OverallHealth('OK')
                 else:
                     psu_Info.OverallHealth(overalhealth.get('data').get('psu').capitalize())
             else:
                 psu_Info.OverallHealth(None)
             psu_allInfo = res.get('data')
             psu_Info.PsuPresentTotalPower(psu_allInfo.get('present_power_reading', None))
-            psu_Info.PsuRatedPower(psu_allInfo.get('rated_power', None))
+            # 2023年3月27日
+            rate_power = psu_allInfo.get('rated_power', 'N/A')
+            if rate_power != "N/A":
+                psu_Info.PsuRatedPower(psu_allInfo.get('rated_power', 'N/A'))
             psu_Info.PsuStatus(status_dict.get(psu_allInfo.get('power_supplies_redundant', 0)))
             temp = psu_allInfo.get('power_supplies', [])
             size = len(temp)
             Num = IpmiFunc.getM6DeviceNumByIpmi(client, '0x00')
             if Num and Num.get('code') == 0:
                 DevConfNum = Num.get('data').get('DevNum')
                 psu_Info.Maximum(DevConfNum)
@@ -5505,19 +5078,23 @@
                     psu.PowerInputWatts(temp[i].get('ps_in_power') if 'ps_in_power' in temp[i] else None)
                     psu.OutputAmperage(
                         temp[i].get('ps_out_current') if 'ps_out_current' in temp[i] else None)
                     psu.PartNumber(None if temp[i].get('part_num', None) == '' else temp[i].get('part_num', None))
                     psu.PowerSupplyType(temp[i].get('input_type', 'Unknown'))
                     psu.LineInputVoltage(temp[i].get('ps_in_volt') if 'ps_in_volt' in temp[i] else None)
                     # psu.PowerCapacityWatts(temp[i].get('ps_out_power_max', None))
-                    # 2023年3月27日 
+                    # 2023年3月27日
                     psu.PowerCapacityWatts(temp[i].get('rated_power', None))
                     psu.FirmwareVersion(None if temp[i].get('fw_ver', None) == '' else temp[i].get('fw_ver', None))
                     psu.SerialNumber(temp[i].get('serial_num', None))
-                    psu.Temperature(temp[i].get('ambient_temperature', None))
+
+                    if "temperature" in temp[i]:
+                        psu.Temperature(temp[i].get('temperature', None))
+                    else:
+                        psu.Temperature(temp[i].get('psu_max_temperature', None))
                     if 'status' in temp[i]:
                         psu.Health(
                             'OK' if temp[i].get('status').upper() == 'OK' else temp[i].get('status').capitalize())
                     else:
                         if 'power_status' in temp[i]:
                             psu.Health('OK' if temp[i].get('power_status') == 0 else 'Critical')
                         else:
```

### Comparing `inManage-1.0.0/inmanage_sdk/interface/I24M6.py` & `inManage-1.0.1/inmanage_sdk/interface/I24M6.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/IBase.py` & `inManage-1.0.1/inmanage_sdk/interface/IBase.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/NF5180M5.py` & `inManage-1.0.1/inmanage_sdk/interface/NF5180M5.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/NF5280M5.py` & `inManage-1.0.1/inmanage_sdk/interface/NF5280M5.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/NF5280M5_435.py` & `inManage-1.0.1/inmanage_sdk/interface/NF5280M5_435.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/NF5280M5_436.py` & `inManage-1.0.1/inmanage_sdk/interface/NF5280M5_436.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/NS5160M6.py` & `inManage-1.0.1/inmanage_sdk/interface/NS5160M6.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/interface/ResEntity.py` & `inManage-1.0.1/inmanage_sdk/interface/ResEntity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1727,14 +1727,20 @@
 
     def Id(self):
         return self.dict['Id']
 
     def Id(self, value):
         self.dict['Id'] = value
 
+    def PortType(self):
+        return self.dict['PortType']
+
+    def PortType(self, value):
+        self.dict['PortType'] = value
+
     def Manufacturer(self):
         return self.dict['Manufacturer']
 
     def Manufacturer(self, value):
         self.dict['Manufacturer'] = value
 
     def Model(self):
@@ -2113,14 +2119,38 @@
 
     def VendorID(self):
         return self.dict['VendorID']
 
     def VendorID(self, value):
         self.dict['VendorID'] = value
 
+    def DeviceName(self):
+        return self.dict['DeviceName']
+
+    def DeviceName(self, value):
+        self.dict['DeviceName'] = value
+
+    def VendorName(self):
+        return self.dict['VendorName']
+
+    def VendorName(self, value):
+        self.dict['VendorName'] = value
+
+    def SubDeviceID(self):
+        return self.dict['SubDeviceID']
+
+    def SubDeviceID(self, value):
+        self.dict['SubDeviceID'] = value
+
+    def SubVendorID(self):
+        return self.dict['SubVendorID']
+
+    def SubVendorID(self, value):
+        self.dict['SubVendorID'] = value
+
     def RatedLinkSpeed(self):
         return self.dict['RatedLinkSpeed']
 
     def RatedLinkSpeed(self, value):
         self.dict['RatedLinkSpeed'] = value
 
     def RatedLinkWidth(self):
```

### Comparing `inManage-1.0.0/inmanage_sdk/route/route.yml` & `inManage-1.0.1/inmanage_sdk/route/route.yml`

 * *Files 3% similar despite different names*

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
@@ -223,7 +226,32 @@
     common: CommonM7
     1.3505: CommonM7_13505
 NF5466-M7-C0-R0-00:
     common: CommonM7
     1.3505: CommonM7_13505
 NF5280A6:
     common: CommonA6
+NE5260M7:
+    common: CommonM7
+    1.3505: CommonM7_13505
+NF5688-M7-C0-R0-00:
+    common: CommonM7
+    1.3505: CommonM7_13505
+NF5468-M7-A0-F0-00:
+    common: CommonM7
+    1.3505: CommonM7_13505
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
+
```

### Comparing `inManage-1.0.0/inmanage_sdk/util/HostTypeJudge.py` & `inManage-1.0.1/inmanage_sdk/util/HostTypeJudge.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/util/RedfishClient.py` & `inManage-1.0.1/inmanage_sdk/util/RedfishClient.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/util/RegularCheckUtil.py` & `inManage-1.0.1/inmanage_sdk/util/RegularCheckUtil.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/util/RequestClient.py` & `inManage-1.0.1/inmanage_sdk/util/RequestClient.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/util/configUtil.py` & `inManage-1.0.1/inmanage_sdk/util/configUtil.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/util/fileUtil.py` & `inManage-1.0.1/inmanage_sdk/util/fileUtil.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/inmanage_sdk/util/parameterConversion.py` & `inManage-1.0.1/inmanage_sdk/util/parameterConversion.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.0/setup.py` & `inManage-1.0.1/setup.py`

 * *Files identical despite different names*

