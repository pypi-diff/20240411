# Comparing `tmp/peutils-0.0.98.tar.gz` & `tmp/peutils-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peutils-0.0.98.tar", last modified: Tue Jan 30 07:45:01 2024, max compression
+gzip compressed data, was "peutils-0.0.99.tar", last modified: Thu Feb  1 09:44:02 2024, max compression
```

## Comparing `peutils-0.0.98.tar` & `peutils-0.0.99.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.562095 peutils-0.0.98/
--rw-r--r--   0 root         (0) jenkins   (1000)      358 2024-01-30 07:45:01.562095 peutils-0.0.98/PKG-INFO
--rw-r--r--   0 root         (0) jenkins   (1000)      589 2024-01-30 07:23:35.000000 peutils-0.0.98/README.md
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.557095 peutils-0.0.98/peutils/
--rw-r--r--   0 root         (0) jenkins   (1000)      114 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/__init__.py
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.558095 peutils-0.0.98/peutils/a9_process/
--rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/a9_process/__init__.py
--rw-r--r--   0 root         (0) jenkins   (1000)     6861 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/a9_process/v1.py
--rw-r--r--   0 root         (0) jenkins   (1000)     8441 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/comutil.py
--rw-r--r--   0 root         (0) jenkins   (1000)     2433 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/datautil.py
--rw-r--r--   0 root         (0) jenkins   (1000)     5960 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/fileutil.py
--rw-r--r--   0 root         (0) jenkins   (1000)     4647 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/image_util.py
--rw-r--r--   0 root         (0) jenkins   (1000)     1461 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/mailutil.py
--rw-r--r--   0 root         (0) jenkins   (1000)      337 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/matrix_util.py
--rw-r--r--   0 root         (0) jenkins   (1000)    12081 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/ossutil.py
--rw-r--r--   0 root         (0) jenkins   (1000)    29907 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/pcd_py3.py
--rw-r--r--   0 root         (0) jenkins   (1000)     2960 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/pcd_util.py
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.558095 peutils-0.0.98/peutils/process/
--rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/process/__init__.py
--rw-r--r--   0 root         (0) jenkins   (1000)     7027 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/process/v1.py
--rw-r--r--   0 root         (0) jenkins   (1000)    11830 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/storage_util.py
--rw-r--r--   0 root         (0) jenkins   (1000)     1649 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/test_collect.py
--rw-r--r--   0 root         (0) jenkins   (1000)     1919 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/textutil.py
--rw-r--r--   0 root         (0) jenkins   (1000)      693 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/toolutil.py
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.558095 peutils-0.0.98/peutils/transform/
--rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/__init__.py
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.559095 peutils-0.0.98/peutils/transform/v1/
--rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/__init__.py
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.559095 peutils-0.0.98/peutils/transform/v1/audio_seg/
--rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/audio_seg/__init__.py
--rw-r--r--   0 root         (0) jenkins   (1000)     4376 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/audio_seg/parser.py
--rw-r--r--   0 root         (0) jenkins   (1000)     2035 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/audio_seg/pre_parser.py
--rw-r--r--   0 root         (0) jenkins   (1000)    27181 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/base.py
--rw-r--r--   0 root         (0) jenkins   (1000)     2458 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/case_test.py
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.559095 peutils-0.0.98/peutils/transform/v1/img_com/
--rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/img_com/__init__.py
--rw-r--r--   0 root         (0) jenkins   (1000)    10067 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/img_com/parser.py
--rw-r--r--   0 root         (0) jenkins   (1000)     7085 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/img_com/pre_parser.py
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.560095 peutils-0.0.98/peutils/transform/v1/lidar_box/
--rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/lidar_box/__init__.py
--rw-r--r--   0 root         (0) jenkins   (1000)    23875 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/lidar_box/parser.py
--rw-r--r--   0 root         (0) jenkins   (1000)     5789 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/lidar_box/pre_parser.py
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.560095 peutils-0.0.98/peutils/transform/v1/lidar_manifest/
--rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/lidar_manifest/__init__.py
--rw-r--r--   0 root         (0) jenkins   (1000)     2659 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/lidar_manifest/parser.py
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.560095 peutils-0.0.98/peutils/transform/v1/lidar_point/
--rw-r--r--   0 root         (0) jenkins   (1000)      114 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/lidar_point/__init__.py
--rw-r--r--   0 root         (0) jenkins   (1000)    12021 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/lidar_point/parser.py
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.561095 peutils-0.0.98/peutils/transform/v1/report/
--rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/report/__init__.py
--rw-r--r--   0 root         (0) jenkins   (1000)     7033 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/report/executor.py
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.561095 peutils-0.0.98/peutils/transform/v1/task/
--rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/task/__init__.py
--rw-r--r--   0 root         (0) jenkins   (1000)     5099 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/task/executor.py
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.561095 peutils-0.0.98/peutils/transform/v1/tools/
--rw-r--r--   0 root         (0) jenkins   (1000)      115 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/tools/__init__.py
--rw-r--r--   0 root         (0) jenkins   (1000)    19040 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/tools/lidar.py
--rw-r--r--   0 root         (0) jenkins   (1000)     5723 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/tools/lidar_cal_point.py
--rw-r--r--   0 root         (0) jenkins   (1000)     2280 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transform/v1/tools/lidar_point.py
--rw-r--r--   0 root         (0) jenkins   (1000)     1037 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/transutil.py
--rw-r--r--   0 root         (0) jenkins   (1000)     6905 2024-01-30 07:23:35.000000 peutils-0.0.98/peutils/wooeyutil.py
-drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-01-30 07:45:01.558095 peutils-0.0.98/peutils.egg-info/
--rw-r--r--   0 root         (0) jenkins   (1000)      358 2024-01-30 07:45:01.000000 peutils-0.0.98/peutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) jenkins   (1000)     1588 2024-01-30 07:45:01.000000 peutils-0.0.98/peutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) jenkins   (1000)        1 2024-01-30 07:45:01.000000 peutils-0.0.98/peutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) jenkins   (1000)        8 2024-01-30 07:45:01.000000 peutils-0.0.98/peutils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) jenkins   (1000)       38 2024-01-30 07:45:01.562095 peutils-0.0.98/setup.cfg
--rw-r--r--   0 root         (0) jenkins   (1000)      701 2024-01-30 07:23:35.000000 peutils-0.0.98/setup.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.207776 peutils-0.0.99/
+-rw-r--r--   0 root         (0) jenkins   (1000)      358 2024-02-01 09:44:02.207776 peutils-0.0.99/PKG-INFO
+-rw-r--r--   0 root         (0) jenkins   (1000)      589 2024-01-30 07:23:35.000000 peutils-0.0.99/README.md
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.201776 peutils-0.0.99/peutils/
+-rw-r--r--   0 root         (0) jenkins   (1000)      114 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/__init__.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.202776 peutils-0.0.99/peutils/a9_process/
+-rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/a9_process/__init__.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     6861 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/a9_process/v1.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     8441 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/comutil.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     2433 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/datautil.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     5960 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/fileutil.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     4647 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/image_util.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     1461 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/mailutil.py
+-rw-r--r--   0 root         (0) jenkins   (1000)      337 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/matrix_util.py
+-rw-r--r--   0 root         (0) jenkins   (1000)    12081 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/ossutil.py
+-rw-r--r--   0 root         (0) jenkins   (1000)    29907 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/pcd_py3.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     2960 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/pcd_util.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.203776 peutils-0.0.99/peutils/process/
+-rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/process/__init__.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     7027 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/process/v1.py
+-rw-r--r--   0 root         (0) jenkins   (1000)    11830 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/storage_util.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     1649 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/test_collect.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     1919 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/textutil.py
+-rw-r--r--   0 root         (0) jenkins   (1000)      693 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/toolutil.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.203776 peutils-0.0.99/peutils/transform/
+-rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/__init__.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.203776 peutils-0.0.99/peutils/transform/v1/
+-rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/__init__.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.204776 peutils-0.0.99/peutils/transform/v1/audio_seg/
+-rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/audio_seg/__init__.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     4376 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/audio_seg/parser.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     2035 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/audio_seg/pre_parser.py
+-rw-r--r--   0 root         (0) jenkins   (1000)    27450 2024-02-01 09:43:54.000000 peutils-0.0.99/peutils/transform/v1/base.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     2458 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/case_test.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.204776 peutils-0.0.99/peutils/transform/v1/img_com/
+-rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/img_com/__init__.py
+-rw-r--r--   0 root         (0) jenkins   (1000)    10067 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/img_com/parser.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     7085 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/img_com/pre_parser.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.205776 peutils-0.0.99/peutils/transform/v1/lidar_box/
+-rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/lidar_box/__init__.py
+-rw-r--r--   0 root         (0) jenkins   (1000)    23875 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/lidar_box/parser.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     5789 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/lidar_box/pre_parser.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.205776 peutils-0.0.99/peutils/transform/v1/lidar_manifest/
+-rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/lidar_manifest/__init__.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     2659 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/lidar_manifest/parser.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.205776 peutils-0.0.99/peutils/transform/v1/lidar_point/
+-rw-r--r--   0 root         (0) jenkins   (1000)      114 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/lidar_point/__init__.py
+-rw-r--r--   0 root         (0) jenkins   (1000)    12021 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/lidar_point/parser.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.205776 peutils-0.0.99/peutils/transform/v1/report/
+-rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/report/__init__.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     7033 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/report/executor.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.206776 peutils-0.0.99/peutils/transform/v1/task/
+-rw-r--r--   0 root         (0) jenkins   (1000)        0 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/task/__init__.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     5099 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/task/executor.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.206776 peutils-0.0.99/peutils/transform/v1/tools/
+-rw-r--r--   0 root         (0) jenkins   (1000)      115 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/tools/__init__.py
+-rw-r--r--   0 root         (0) jenkins   (1000)    19040 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/tools/lidar.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     5723 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/tools/lidar_cal_point.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     2280 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transform/v1/tools/lidar_point.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     1037 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/transutil.py
+-rw-r--r--   0 root         (0) jenkins   (1000)     6905 2024-01-30 07:23:35.000000 peutils-0.0.99/peutils/wooeyutil.py
+drwxr-sr-x   0 root         (0) jenkins   (1000)        0 2024-02-01 09:44:02.202776 peutils-0.0.99/peutils.egg-info/
+-rw-r--r--   0 root         (0) jenkins   (1000)      358 2024-02-01 09:44:02.000000 peutils-0.0.99/peutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) jenkins   (1000)     1588 2024-02-01 09:44:02.000000 peutils-0.0.99/peutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) jenkins   (1000)        1 2024-02-01 09:44:02.000000 peutils-0.0.99/peutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) jenkins   (1000)        8 2024-02-01 09:44:02.000000 peutils-0.0.99/peutils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) jenkins   (1000)       38 2024-02-01 09:44:02.207776 peutils-0.0.99/setup.cfg
+-rw-r--r--   0 root         (0) jenkins   (1000)      701 2024-02-01 09:43:54.000000 peutils-0.0.99/setup.py
```

### Comparing `peutils-0.0.98/README.md` & `peutils-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/a9_process/v1.py` & `peutils-0.0.99/peutils/a9_process/v1.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/comutil.py` & `peutils-0.0.99/peutils/comutil.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/datautil.py` & `peutils-0.0.99/peutils/datautil.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/fileutil.py` & `peutils-0.0.99/peutils/fileutil.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/image_util.py` & `peutils-0.0.99/peutils/image_util.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/mailutil.py` & `peutils-0.0.99/peutils/mailutil.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/ossutil.py` & `peutils-0.0.99/peutils/ossutil.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/pcd_py3.py` & `peutils-0.0.99/peutils/pcd_py3.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/pcd_util.py` & `peutils-0.0.99/peutils/pcd_util.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/process/v1.py` & `peutils-0.0.99/peutils/process/v1.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/storage_util.py` & `peutils-0.0.99/peutils/storage_util.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/test_collect.py` & `peutils-0.0.99/peutils/test_collect.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/textutil.py` & `peutils-0.0.99/peutils/textutil.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/toolutil.py` & `peutils-0.0.99/peutils/toolutil.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/audio_seg/parser.py` & `peutils-0.0.99/peutils/transform/v1/audio_seg/parser.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/audio_seg/pre_parser.py` & `peutils-0.0.99/peutils/transform/v1/audio_seg/pre_parser.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/base.py` & `peutils-0.0.99/peutils/transform/v1/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,18 +257,24 @@
             "rotation": self.rotation if self.rotation else None,
             "rotation2": self.rotation2 if self.rotation2 else None,
             "quaternion": self.quaternion if self.quaternion else None,
             "dimension": self.dimension,
             # "labels": "" if self.lidar_attr else json.dumps(self.lidar_attr, ensure_ascii=False),
             "labels": json.dumps(self.lidar_attr, ensure_ascii=False) if self.lidar_attr else "",
         }
-        if self.pointCount:
+        if self.pointCount is None:
+            _data_dict["pointCount"] = {}
+        elif isinstance(self.pointCount, int):
             _data_dict["pointCount"] = {
                 "lidar": self.pointCount
             }
+        elif isinstance(self.pointCount, dict):
+            _data_dict["pointCount"] = self.pointCount
+        else:
+            raise ValueError(f'pointCount参数error')
         return _data_dict
 
 
 class Lidar3dCamCube():
     def __init__(self, frameNum, id, number, category, position, dimension, rotation=None, rotation2=None,
                  camCubeAttr=None, quaternion=None, pointCount=None, vertices=None, type=None, imageNum=None):
         self.frameNum = frameNum
```

### Comparing `peutils-0.0.98/peutils/transform/v1/case_test.py` & `peutils-0.0.99/peutils/transform/v1/case_test.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/img_com/parser.py` & `peutils-0.0.99/peutils/transform/v1/img_com/parser.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/img_com/pre_parser.py` & `peutils-0.0.99/peutils/transform/v1/img_com/pre_parser.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/lidar_box/parser.py` & `peutils-0.0.99/peutils/transform/v1/lidar_box/parser.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/lidar_box/pre_parser.py` & `peutils-0.0.99/peutils/transform/v1/lidar_box/pre_parser.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/lidar_manifest/parser.py` & `peutils-0.0.99/peutils/transform/v1/lidar_manifest/parser.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/lidar_point/parser.py` & `peutils-0.0.99/peutils/transform/v1/lidar_point/parser.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/report/executor.py` & `peutils-0.0.99/peutils/transform/v1/report/executor.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/task/executor.py` & `peutils-0.0.99/peutils/transform/v1/task/executor.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/tools/lidar.py` & `peutils-0.0.99/peutils/transform/v1/tools/lidar.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/tools/lidar_cal_point.py` & `peutils-0.0.99/peutils/transform/v1/tools/lidar_cal_point.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transform/v1/tools/lidar_point.py` & `peutils-0.0.99/peutils/transform/v1/tools/lidar_point.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/transutil.py` & `peutils-0.0.99/peutils/transutil.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils/wooeyutil.py` & `peutils-0.0.99/peutils/wooeyutil.py`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/peutils.egg-info/SOURCES.txt` & `peutils-0.0.99/peutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peutils-0.0.98/setup.py` & `peutils-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from setuptools import setup, find_packages
 
 
 
 
 setup(
     name = "peutils",
-    version = '0.0.98',
+    version = '0.0.99',
     keywords = ("pip3", "peutils",'henry'),
     description = "utils for text,audio,video,excel,file and so on.",
     long_description = "utils for text,audio,video,excel,file and so on,more details please visit gitlab.",
     license = "MIT Licence",
     url = "https://github.com/yunsansheng/peutils",
     author = "henry.wang",
     author_email = "shanandone@qq.com",
```

