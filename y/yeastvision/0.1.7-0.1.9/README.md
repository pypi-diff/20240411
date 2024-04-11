# Comparing `tmp/yeastvision-0.1.7.tar.gz` & `tmp/yeastvision-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeastvision-0.1.7.tar", last modified: Tue Jul 11 03:12:40 2023, max compression
+gzip compressed data, was "yeastvision-0.1.9.tar", last modified: Wed Jul 19 15:42:37 2023, max compression
```

## Comparing `yeastvision-0.1.7.tar` & `yeastvision-0.1.9.tar`

### file list

```diff
@@ -1,96 +1,100 @@
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.216730 yeastvision-0.1.7/
--rw-r--r--   0 berk       (502) staff       (20)     1467 2023-06-13 00:33:13.000000 yeastvision-0.1.7/LICENSE
--rw-r--r--   0 berk       (502) staff       (20)     3635 2023-07-11 03:12:40.216031 yeastvision-0.1.7/PKG-INFO
--rw-r--r--   0 berk       (502) staff       (20)     3287 2023-07-11 03:08:39.000000 yeastvision-0.1.7/README.md
--rw-r--r--   0 berk       (502) staff       (20)       38 2023-07-11 03:12:40.216921 yeastvision-0.1.7/setup.cfg
--rw-r--r--   0 berk       (502) staff       (20)     1798 2023-07-11 03:12:14.000000 yeastvision-0.1.7/setup.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.142601 yeastvision-0.1.7/yeastvision/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 01:16:17.000000 yeastvision-0.1.7/yeastvision/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)    81437 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/__main__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.149281 yeastvision-0.1.7/yeastvision/disk/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-01-09 00:08:51.000000 yeastvision-0.1.7/yeastvision/disk/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     1212 2023-06-22 04:39:33.000000 yeastvision-0.1.7/yeastvision/disk/io.py
--rw-r--r--   0 berk       (502) staff       (20)    13015 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/disk/reader.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.151588 yeastvision-0.1.7/yeastvision/flou/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-02-23 11:08:01.000000 yeastvision-0.1.7/yeastvision/flou/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     1676 2023-06-13 10:06:19.000000 yeastvision-0.1.7/yeastvision/flou/blob_detect.py
--rw-r--r--   0 berk       (502) staff       (20)     1374 2023-03-29 01:49:55.000000 yeastvision-0.1.7/yeastvision/flou/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.153324 yeastvision-0.1.7/yeastvision/ims/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     2688 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/im_funcs.py
--rw-r--r--   0 berk       (502) staff       (20)     3907 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/interpolate.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.162021 yeastvision-0.1.7/yeastvision/ims/rife_model/
--rw-r--r--   0 berk       (502) staff       (20)     4518 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/IFNet.py
--rw-r--r--   0 berk       (502) staff       (20)     4509 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/IFNet_2R.py
--rw-r--r--   0 berk       (502) staff       (20)     4716 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/IFNet_m.py
--rw-r--r--   0 berk       (502) staff       (20)     3518 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/RIFE.py
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     3850 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/interpolate.py
--rw-r--r--   0 berk       (502) staff       (20)     2187 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/laplacian.py
--rw-r--r--   0 berk       (502) staff       (20)     4641 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/loss.py
--rw-r--r--   0 berk       (502) staff       (20)     3219 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/refine.py
--rw-r--r--   0 berk       (502) staff       (20)     3286 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/refine_2R.py
--rw-r--r--   0 berk       (502) staff       (20)     1058 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/warplayer.py
--rw-r--r--   0 berk       (502) staff       (20)     2419 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/install_weights.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.168913 yeastvision-0.1.7/yeastvision/models/
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.173158 yeastvision-0.1.7/yeastvision/models/YeaZ/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:23:10.000000 yeastvision-0.1.7/yeastvision/models/YeaZ/__init__.py
--rw-rw-r--   0 berk       (502) staff       (20)     1919 2023-06-13 09:59:20.000000 yeastvision-0.1.7/yeastvision/models/YeaZ/model.py
--rw-rw-r--   0 berk       (502) staff       (20)     6145 2022-09-09 01:01:50.000000 yeastvision-0.1.7/yeastvision/models/YeaZ/segment.py
--rw-r--r--   0 berk       (502) staff       (20)     3665 2022-10-05 10:22:57.000000 yeastvision-0.1.7/yeastvision/models/YeaZ/unet.py
--rw-rw-r--   0 berk       (502) staff       (20)        0 2023-06-13 07:27:49.000000 yeastvision-0.1.7/yeastvision/models/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.174327 yeastvision-0.1.7/yeastvision/models/artilife/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-07 09:15:32.000000 yeastvision-0.1.7/yeastvision/models/artilife/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.175936 yeastvision-0.1.7/yeastvision/models/artilife/budSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-25 06:42:22.000000 yeastvision-0.1.7/yeastvision/models/artilife/budSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      590 2023-06-21 06:06:54.000000 yeastvision-0.1.7/yeastvision/models/artilife/budSeg/model.py
--rw-r--r--   0 berk       (502) staff       (20)     9519 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/models/artilife/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.177044 yeastvision-0.1.7/yeastvision/models/budNET/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:46.000000 yeastvision-0.1.7/yeastvision/models/budNET/__init__.py
--rw-rw-r--   0 berk       (502) staff       (20)     1334 2023-06-13 09:58:28.000000 yeastvision-0.1.7/yeastvision/models/budNET/model.py
--rw-r--r--   0 berk       (502) staff       (20)     3833 2023-06-27 20:12:02.000000 yeastvision-0.1.7/yeastvision/models/cp.py
--rw-r--r--   0 berk       (502) staff       (20)       21 2022-12-28 01:01:29.000000 yeastvision-0.1.7/yeastvision/models/eval.py
--rw-r--r--   0 berk       (502) staff       (20)      381 2023-01-19 00:50:23.000000 yeastvision-0.1.7/yeastvision/models/loss.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.178176 yeastvision-0.1.7/yeastvision/models/matSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:19.000000 yeastvision-0.1.7/yeastvision/models/matSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      164 2023-06-13 09:58:37.000000 yeastvision-0.1.7/yeastvision/models/matSeg/model.py
--rw-rw-r--   0 berk       (502) staff       (20)     1649 2023-06-13 10:00:05.000000 yeastvision-0.1.7/yeastvision/models/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.179368 yeastvision-0.1.7/yeastvision/models/tetradSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:27.000000 yeastvision-0.1.7/yeastvision/models/tetradSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      168 2023-06-13 09:58:44.000000 yeastvision-0.1.7/yeastvision/models/tetradSeg/model.py
--rw-rw-r--   0 berk       (502) staff       (20)    14546 2023-06-04 23:09:45.000000 yeastvision-0.1.7/yeastvision/models/unet.py
--rw-rw-r--   0 berk       (502) staff       (20)     6177 2023-06-13 10:04:25.000000 yeastvision-0.1.7/yeastvision/models/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.180471 yeastvision-0.1.7/yeastvision/models/vacNET/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:37.000000 yeastvision-0.1.7/yeastvision/models/vacNET/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      468 2023-06-13 09:58:56.000000 yeastvision-0.1.7/yeastvision/models/vacNET/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.186965 yeastvision-0.1.7/yeastvision/parts/
--rw-r--r--   0 berk       (502) staff       (20)    13220 2023-06-22 04:39:33.000000 yeastvision-0.1.7/yeastvision/parts/canvas.py
--rw-r--r--   0 berk       (502) staff       (20)    31747 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/parts/dialogs.py
--rw-r--r--   0 berk       (502) staff       (20)    12008 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/parts/guiparts.py
--rw-r--r--   0 berk       (502) staff       (20)     3724 2023-06-22 04:39:33.000000 yeastvision-0.1.7/yeastvision/parts/menu.py
--rw-r--r--   0 berk       (502) staff       (20)        5 2023-04-12 05:16:38.000000 yeastvision-0.1.7/yeastvision/parts/utils.py
--rw-r--r--   0 berk       (502) staff       (20)     3502 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/parts/workers.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.191258 yeastvision-0.1.7/yeastvision/plot/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 00:45:38.000000 yeastvision-0.1.7/yeastvision/plot/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     3461 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/plot/cell_table.py
--rw-r--r--   0 berk       (502) staff       (20)    12653 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/plot/plot.py
--rw-r--r--   0 berk       (502) staff       (20)     5056 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/plot/types.py
--rw-r--r--   0 berk       (502) staff       (20)      391 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/plot/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.211297 yeastvision-0.1.7/yeastvision/track/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 12:09:09.000000 yeastvision-0.1.7/yeastvision/track/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     6286 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/track/cell.py
--rw-r--r--   0 berk       (502) staff       (20)     8241 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/track/data.py
--rw-r--r--   0 berk       (502) staff       (20)     6820 2023-03-08 23:50:11.000000 yeastvision-0.1.7/yeastvision/track/hungarian_track.py
--rw-r--r--   0 berk       (502) staff       (20)        4 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/track/lc.py
--rw-r--r--   0 berk       (502) staff       (20)     8413 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/track/lineage.py
--rw-r--r--   0 berk       (502) staff       (20)    18443 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/track/mat.py
--rw-rw-r--   0 berk       (502) staff       (20)     5357 2023-06-20 19:14:02.000000 yeastvision-0.1.7/yeastvision/track/track.py
--rw-r--r--   0 berk       (502) staff       (20)     4574 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/track/utils.py
--rw-r--r--   0 berk       (502) staff       (20)     5523 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.147281 yeastvision-0.1.7/yeastvision.egg-info/
--rw-r--r--   0 berk       (502) staff       (20)     3635 2023-07-11 03:12:40.000000 yeastvision-0.1.7/yeastvision.egg-info/PKG-INFO
--rw-r--r--   0 berk       (502) staff       (20)     2364 2023-07-11 03:12:40.000000 yeastvision-0.1.7/yeastvision.egg-info/SOURCES.txt
--rw-r--r--   0 berk       (502) staff       (20)        1 2023-07-11 03:12:40.000000 yeastvision-0.1.7/yeastvision.egg-info/dependency_links.txt
--rw-r--r--   0 berk       (502) staff       (20)      116 2023-07-11 03:12:40.000000 yeastvision-0.1.7/yeastvision.egg-info/entry_points.txt
--rw-r--r--   0 berk       (502) staff       (20)      273 2023-07-11 03:12:40.000000 yeastvision-0.1.7/yeastvision.egg-info/requires.txt
--rw-r--r--   0 berk       (502) staff       (20)       12 2023-07-11 03:12:40.000000 yeastvision-0.1.7/yeastvision.egg-info/top_level.txt
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:37.005496 yeastvision-0.1.9/
+-rw-r--r--   0 berk       (502) staff       (20)     1467 2023-06-13 00:33:13.000000 yeastvision-0.1.9/LICENSE
+-rw-r--r--   0 berk       (502) staff       (20)     4566 2023-07-19 15:42:37.005128 yeastvision-0.1.9/PKG-INFO
+-rw-r--r--   0 berk       (502) staff       (20)     4238 2023-07-19 15:35:36.000000 yeastvision-0.1.9/README.md
+-rw-r--r--   0 berk       (502) staff       (20)       38 2023-07-19 15:42:37.005607 yeastvision-0.1.9/setup.cfg
+-rw-r--r--   0 berk       (502) staff       (20)     1928 2023-07-19 15:40:38.000000 yeastvision-0.1.9/setup.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.967485 yeastvision-0.1.9/yeastvision/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 01:16:17.000000 yeastvision-0.1.9/yeastvision/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)    82362 2023-07-18 17:30:38.000000 yeastvision-0.1.9/yeastvision/__main__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.971058 yeastvision-0.1.9/yeastvision/disk/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-01-09 00:08:51.000000 yeastvision-0.1.9/yeastvision/disk/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     1212 2023-06-22 04:39:33.000000 yeastvision-0.1.9/yeastvision/disk/io.py
+-rw-r--r--   0 berk       (502) staff       (20)    13016 2023-07-18 17:07:50.000000 yeastvision-0.1.9/yeastvision/disk/reader.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.972038 yeastvision-0.1.9/yeastvision/flou/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-02-23 11:08:01.000000 yeastvision-0.1.9/yeastvision/flou/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     1676 2023-06-13 10:06:19.000000 yeastvision-0.1.9/yeastvision/flou/blob_detect.py
+-rw-r--r--   0 berk       (502) staff       (20)     1374 2023-03-29 01:49:55.000000 yeastvision-0.1.9/yeastvision/flou/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.973358 yeastvision-0.1.9/yeastvision/ims/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/ims/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     2688 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/ims/im_funcs.py
+-rw-r--r--   0 berk       (502) staff       (20)     3981 2023-07-19 15:39:14.000000 yeastvision-0.1.9/yeastvision/ims/interpolate.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.976665 yeastvision-0.1.9/yeastvision/ims/rife_model/
+-rw-r--r--   0 berk       (502) staff       (20)     4518 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/ims/rife_model/IFNet.py
+-rw-r--r--   0 berk       (502) staff       (20)     4509 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/ims/rife_model/IFNet_2R.py
+-rw-r--r--   0 berk       (502) staff       (20)     4716 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/ims/rife_model/IFNet_m.py
+-rw-r--r--   0 berk       (502) staff       (20)     3539 2023-07-18 18:53:08.000000 yeastvision-0.1.9/yeastvision/ims/rife_model/RIFE.py
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/ims/rife_model/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     2187 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/ims/rife_model/laplacian.py
+-rw-r--r--   0 berk       (502) staff       (20)     4641 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/ims/rife_model/loss.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.976963 yeastvision-0.1.9/yeastvision/ims/rife_model/pytorch_msssim/
+-rw-r--r--   0 berk       (502) staff       (20)     6999 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/ims/rife_model/pytorch_msssim/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     3219 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/ims/rife_model/refine.py
+-rw-r--r--   0 berk       (502) staff       (20)     3286 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/ims/rife_model/refine_2R.py
+-rw-r--r--   0 berk       (502) staff       (20)     1058 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/ims/rife_model/warplayer.py
+-rw-r--r--   0 berk       (502) staff       (20)     2419 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/install_weights.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.979515 yeastvision-0.1.9/yeastvision/models/
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.991688 yeastvision-0.1.9/yeastvision/models/YeaZ/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:23:10.000000 yeastvision-0.1.9/yeastvision/models/YeaZ/__init__.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1919 2023-06-13 09:59:20.000000 yeastvision-0.1.9/yeastvision/models/YeaZ/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)     6145 2022-09-09 01:01:50.000000 yeastvision-0.1.9/yeastvision/models/YeaZ/segment.py
+-rw-r--r--   0 berk       (502) staff       (20)     3665 2022-10-05 10:22:57.000000 yeastvision-0.1.9/yeastvision/models/YeaZ/unet.py
+-rw-rw-r--   0 berk       (502) staff       (20)        0 2023-06-13 07:27:49.000000 yeastvision-0.1.9/yeastvision/models/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.992477 yeastvision-0.1.9/yeastvision/models/artiBud/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-07-18 17:07:50.000000 yeastvision-0.1.9/yeastvision/models/artiBud/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      165 2023-07-18 17:07:50.000000 yeastvision-0.1.9/yeastvision/models/artiBud/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.993109 yeastvision-0.1.9/yeastvision/models/artilife/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-07 09:15:32.000000 yeastvision-0.1.9/yeastvision/models/artilife/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.993927 yeastvision-0.1.9/yeastvision/models/artilife/budSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-25 06:42:22.000000 yeastvision-0.1.9/yeastvision/models/artilife/budSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      590 2023-06-21 06:06:54.000000 yeastvision-0.1.9/yeastvision/models/artilife/budSeg/model.py
+-rw-r--r--   0 berk       (502) staff       (20)     9519 2023-06-29 18:12:58.000000 yeastvision-0.1.9/yeastvision/models/artilife/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.994807 yeastvision-0.1.9/yeastvision/models/budNET/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:46.000000 yeastvision-0.1.9/yeastvision/models/budNET/__init__.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1334 2023-06-13 09:58:28.000000 yeastvision-0.1.9/yeastvision/models/budNET/model.py
+-rw-r--r--   0 berk       (502) staff       (20)     3833 2023-06-27 20:12:02.000000 yeastvision-0.1.9/yeastvision/models/cp.py
+-rw-r--r--   0 berk       (502) staff       (20)       21 2022-12-28 01:01:29.000000 yeastvision-0.1.9/yeastvision/models/eval.py
+-rw-r--r--   0 berk       (502) staff       (20)      381 2023-01-19 00:50:23.000000 yeastvision-0.1.9/yeastvision/models/loss.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.995486 yeastvision-0.1.9/yeastvision/models/matSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:19.000000 yeastvision-0.1.9/yeastvision/models/matSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      164 2023-06-13 09:58:37.000000 yeastvision-0.1.9/yeastvision/models/matSeg/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1649 2023-06-13 10:00:05.000000 yeastvision-0.1.9/yeastvision/models/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.996145 yeastvision-0.1.9/yeastvision/models/tetradSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:27.000000 yeastvision-0.1.9/yeastvision/models/tetradSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      168 2023-06-13 09:58:44.000000 yeastvision-0.1.9/yeastvision/models/tetradSeg/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)    14546 2023-06-04 23:09:45.000000 yeastvision-0.1.9/yeastvision/models/unet.py
+-rw-rw-r--   0 berk       (502) staff       (20)     6177 2023-06-13 10:04:25.000000 yeastvision-0.1.9/yeastvision/models/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.996859 yeastvision-0.1.9/yeastvision/models/vacNET/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:37.000000 yeastvision-0.1.9/yeastvision/models/vacNET/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      468 2023-06-13 09:58:56.000000 yeastvision-0.1.9/yeastvision/models/vacNET/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.998982 yeastvision-0.1.9/yeastvision/parts/
+-rw-r--r--   0 berk       (502) staff       (20)    13220 2023-06-22 04:39:33.000000 yeastvision-0.1.9/yeastvision/parts/canvas.py
+-rw-r--r--   0 berk       (502) staff       (20)    31747 2023-06-29 18:12:58.000000 yeastvision-0.1.9/yeastvision/parts/dialogs.py
+-rw-r--r--   0 berk       (502) staff       (20)    12008 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/parts/guiparts.py
+-rw-r--r--   0 berk       (502) staff       (20)     3724 2023-06-22 04:39:33.000000 yeastvision-0.1.9/yeastvision/parts/menu.py
+-rw-r--r--   0 berk       (502) staff       (20)        5 2023-04-12 05:16:38.000000 yeastvision-0.1.9/yeastvision/parts/utils.py
+-rw-r--r--   0 berk       (502) staff       (20)     3502 2023-07-11 03:02:20.000000 yeastvision-0.1.9/yeastvision/parts/workers.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:37.000939 yeastvision-0.1.9/yeastvision/plot/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 00:45:38.000000 yeastvision-0.1.9/yeastvision/plot/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     3461 2023-06-29 18:12:58.000000 yeastvision-0.1.9/yeastvision/plot/cell_table.py
+-rw-r--r--   0 berk       (502) staff       (20)    12653 2023-06-29 18:12:58.000000 yeastvision-0.1.9/yeastvision/plot/plot.py
+-rw-r--r--   0 berk       (502) staff       (20)     5056 2023-06-29 18:12:58.000000 yeastvision-0.1.9/yeastvision/plot/types.py
+-rw-r--r--   0 berk       (502) staff       (20)      391 2023-06-29 18:12:58.000000 yeastvision-0.1.9/yeastvision/plot/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:37.004681 yeastvision-0.1.9/yeastvision/track/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 12:09:09.000000 yeastvision-0.1.9/yeastvision/track/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     6286 2023-06-29 18:12:58.000000 yeastvision-0.1.9/yeastvision/track/cell.py
+-rw-r--r--   0 berk       (502) staff       (20)     8241 2023-06-29 18:12:58.000000 yeastvision-0.1.9/yeastvision/track/data.py
+-rw-r--r--   0 berk       (502) staff       (20)     6820 2023-03-08 23:50:11.000000 yeastvision-0.1.9/yeastvision/track/hungarian_track.py
+-rw-r--r--   0 berk       (502) staff       (20)        4 2023-06-29 18:12:58.000000 yeastvision-0.1.9/yeastvision/track/lc.py
+-rw-r--r--   0 berk       (502) staff       (20)     8413 2023-06-29 18:12:58.000000 yeastvision-0.1.9/yeastvision/track/lineage.py
+-rw-r--r--   0 berk       (502) staff       (20)    18354 2023-07-18 17:07:50.000000 yeastvision-0.1.9/yeastvision/track/mat.py
+-rw-rw-r--   0 berk       (502) staff       (20)     5357 2023-06-20 19:14:02.000000 yeastvision-0.1.9/yeastvision/track/track.py
+-rw-r--r--   0 berk       (502) staff       (20)     4574 2023-06-29 18:12:58.000000 yeastvision-0.1.9/yeastvision/track/utils.py
+-rw-r--r--   0 berk       (502) staff       (20)     5523 2023-06-29 18:12:58.000000 yeastvision-0.1.9/yeastvision/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-19 15:42:36.970152 yeastvision-0.1.9/yeastvision.egg-info/
+-rw-r--r--   0 berk       (502) staff       (20)     4566 2023-07-19 15:42:36.000000 yeastvision-0.1.9/yeastvision.egg-info/PKG-INFO
+-rw-r--r--   0 berk       (502) staff       (20)     2451 2023-07-19 15:42:36.000000 yeastvision-0.1.9/yeastvision.egg-info/SOURCES.txt
+-rw-r--r--   0 berk       (502) staff       (20)        1 2023-07-19 15:42:36.000000 yeastvision-0.1.9/yeastvision.egg-info/dependency_links.txt
+-rw-r--r--   0 berk       (502) staff       (20)      115 2023-07-19 15:42:36.000000 yeastvision-0.1.9/yeastvision.egg-info/entry_points.txt
+-rw-r--r--   0 berk       (502) staff       (20)      275 2023-07-19 15:42:36.000000 yeastvision-0.1.9/yeastvision.egg-info/requires.txt
+-rw-r--r--   0 berk       (502) staff       (20)       12 2023-07-19 15:42:36.000000 yeastvision-0.1.9/yeastvision.egg-info/top_level.txt
```

### Comparing `yeastvision-0.1.7/LICENSE` & `yeastvision-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/PKG-INFO` & `yeastvision-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: yeastvision
-Version: 0.1.7
+Version: 0.1.9
 Summary: Deep learning-enabled image analysis of the yeast full life cycle
 Home-page: https://github.com/berkyalcinkaya/yeastvision
 Author: Berk Yalcinkaya
 Author-email: berkyalcinkaya55@gmail.com
 License: BSD
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <p>  <b>YeastVision </b> </p>
 
 
 # Installation
@@ -24,19 +23,19 @@
 ### Instructions 
 
 If you have an older `yeastvision` environment you should remove it with `conda env remove -n yeastvision` before creating a new one. 
 
 Yeastvision is ready to go for cpu-usage as soon as it downloaded. GPU-usage requires some additional steps after download. To download:
 
 1. Install an [Anaconda](https://www.anaconda.com/products/distribution) distribution of Python. Note you might need to use an anaconda prompt if you did not add anaconda to the path.
-2. Open an anaconda prompt / command prompt which has `conda` for **python 3** in the path
-3. Create a new environment with `conda create --name yeastvision python=3.10.o`. 
+2. Open an anaconda prompt/command prompt
+3. Create a new environment with `conda create --name yeastvision python=3.10.0`. 
 4. Activate this new environment by running `conda activate yeastvision`
 5. Run `python -m pip install yeastvision` to download our package plus all dependencies
-6. Download the weights [online](https://drive.google.com/file/d/1Zl3b00eSbe3wbxpYOknEP5q0A86XtEfL/view?usp=sharing). 
+6. Download the weights [online](https://drive.google.com/file/d/1sxYyiRmLxykJcb3PXxa7p4iGEOa96APk/view?usp=sharing). 
 7. Run `install-weights` in the same directory as the *yeastvision_weights.zip* file
 
 
 You should upgrade yeastvision (package [here](https://pypi.org/project/yeastvision/)) periodically as it is still in development. To do so, run the following in the environment:
 
 ~~~sh
 python -m pip install yeastvision --upgrade
@@ -48,36 +47,51 @@
 
 To use your NVIDIA GPU with python, you will first need to install the NVIDIA driver for your GPU, check out this [website](https://www.nvidia.com/Download/index.aspx?lang=en-us) to download it. Ensure it is downloaded and your GPU is detected by running `nvidia-smi` in the terminal.
 
 Next we need to remove the CPU version of torch:
 ~~~
 pip uninstall torch
 ~~~
-
-To install the GPU version of torch, follow the instructions [here](https://pytorch.org/get-started/locally/). The conda install is strongly recommended, and then choose the CUDA version that is supported by your GPU (newer GPUs may need newer CUDA versions > 10.2). For instance this command will install the 11.6 version on Linux and Windows (note the `torchvision` and `torchaudio` commands are removed because yeastvision doesn't require them):
+And the cpu version of torchvision:
 ~~~
-conda install pytorch pytorch-cuda=11.6 -c pytorch -c nvidia
+pip uninstall torchvision
 ~~~
 
-If you are unable to install the package using the command above, try an older version like cuda 11.3:
+To install the GPU version of torch and torchvision, first ensure you have downloaded the proper nvidia drivers for your GPU. Then for pytorch and torchvision, follow the instructions [here](https://pytorch.org/get-started/locally/). The conda install is strongly recommended, and then choose the CUDA version that is supported by your GPU (newer GPUs may need newer CUDA versions > 10.2). You can check the highest version of CUDA that your nvidia driver supports by running: 
+~~~
+nvidia-smi
+~~~
+For instance this command will install the 11.6 version on Linux and Windows (note the `torchaudio` commands are removed because yeastvision doesn't require them):
 ~~~
-conda install pytorch==1.12.0 cudatoolkit=11.3 -c pytorch
+conda install pytorch==1.12.0 torchvision==0.13.0 pytorch-cuda=11.6 -c pytorch -c nvidia
+~~~
+The 11.6 configuration is recommended as this system was thoroughly tested with this system.  However, for some GPUs which do not support CUDA 11.6 or later, the above command will timeout. In that case, you can quickly try an older version like cuda 11.3:
+~~~
+conda install pytorch==1.12.0 torchvision==0.13.0 cudatoolkit=11.3 -c pytorch
 ~~~~
 Info on how to install several older versions is available [here](https://pytorch.org/get-started/previous-versions/). 
 
 After install you can check `conda list` for `pytorch`, and its version info should have `cuXX.X`, not `cpu`.
 
+## Common Installation Problems
+
+You may receive the following error upon upgrading `torch` and `torchvision`:
+~~~
+AttributeError: partially initialized module 'charset_normalizer' has no attribute 'md__mypyc' (most likely due to a circular import)
+~~~
+This is solved by upgrading the charselt_normalizer package with the following command: `AttributeError: partially initialized module 'charset_normalizer' has no attribute 'md__mypyc' (most likely due to a circular import)`
+
+Report any other installation errors.
+
 # Run yeastvision locally
 
 The quickest way to start is to open the GUI from a command line terminal. Activate the correct conda environment, then run:
 ~~~~
 yeastvision
 ~~~~
 
 To get started, drop an image or directory of images into the GUI. 
 
 **Masks can be loaded by dropping them into the top half of the screen.**
 
 
 
-
-
```

### Comparing `yeastvision-0.1.7/README.md` & `yeastvision-0.1.9/yeastvision.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: yeastvision
+Version: 0.1.9
+Summary: Deep learning-enabled image analysis of the yeast full life cycle
+Home-page: https://github.com/berkyalcinkaya/yeastvision
+Author: Berk Yalcinkaya
+Author-email: berkyalcinkaya55@gmail.com
+License: BSD
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # <p>  <b>YeastVision </b> </p>
 
 
 # Installation
 
 ## Local installation (< 2 minutes)
 
@@ -12,19 +23,19 @@
 ### Instructions 
 
 If you have an older `yeastvision` environment you should remove it with `conda env remove -n yeastvision` before creating a new one. 
 
 Yeastvision is ready to go for cpu-usage as soon as it downloaded. GPU-usage requires some additional steps after download. To download:
 
 1. Install an [Anaconda](https://www.anaconda.com/products/distribution) distribution of Python. Note you might need to use an anaconda prompt if you did not add anaconda to the path.
-2. Open an anaconda prompt / command prompt which has `conda` for **python 3** in the path
-3. Create a new environment with `conda create --name yeastvision python=3.10.o`. 
+2. Open an anaconda prompt/command prompt
+3. Create a new environment with `conda create --name yeastvision python=3.10.0`. 
 4. Activate this new environment by running `conda activate yeastvision`
 5. Run `python -m pip install yeastvision` to download our package plus all dependencies
-6. Download the weights [online](https://drive.google.com/file/d/1Zl3b00eSbe3wbxpYOknEP5q0A86XtEfL/view?usp=sharing). 
+6. Download the weights [online](https://drive.google.com/file/d/1sxYyiRmLxykJcb3PXxa7p4iGEOa96APk/view?usp=sharing). 
 7. Run `install-weights` in the same directory as the *yeastvision_weights.zip* file
 
 
 You should upgrade yeastvision (package [here](https://pypi.org/project/yeastvision/)) periodically as it is still in development. To do so, run the following in the environment:
 
 ~~~sh
 python -m pip install yeastvision --upgrade
@@ -36,28 +47,45 @@
 
 To use your NVIDIA GPU with python, you will first need to install the NVIDIA driver for your GPU, check out this [website](https://www.nvidia.com/Download/index.aspx?lang=en-us) to download it. Ensure it is downloaded and your GPU is detected by running `nvidia-smi` in the terminal.
 
 Next we need to remove the CPU version of torch:
 ~~~
 pip uninstall torch
 ~~~
-
-To install the GPU version of torch, follow the instructions [here](https://pytorch.org/get-started/locally/). The conda install is strongly recommended, and then choose the CUDA version that is supported by your GPU (newer GPUs may need newer CUDA versions > 10.2). For instance this command will install the 11.6 version on Linux and Windows (note the `torchvision` and `torchaudio` commands are removed because yeastvision doesn't require them):
+And the cpu version of torchvision:
 ~~~
-conda install pytorch pytorch-cuda=11.6 -c pytorch -c nvidia
+pip uninstall torchvision
 ~~~
 
-If you are unable to install the package using the command above, try an older version like cuda 11.3:
+To install the GPU version of torch and torchvision, first ensure you have downloaded the proper nvidia drivers for your GPU. Then for pytorch and torchvision, follow the instructions [here](https://pytorch.org/get-started/locally/). The conda install is strongly recommended, and then choose the CUDA version that is supported by your GPU (newer GPUs may need newer CUDA versions > 10.2). You can check the highest version of CUDA that your nvidia driver supports by running: 
+~~~
+nvidia-smi
+~~~
+For instance this command will install the 11.6 version on Linux and Windows (note the `torchaudio` commands are removed because yeastvision doesn't require them):
+~~~
+conda install pytorch==1.12.0 torchvision==0.13.0 pytorch-cuda=11.6 -c pytorch -c nvidia
+~~~
+The 11.6 configuration is recommended as this system was thoroughly tested with this system.  However, for some GPUs which do not support CUDA 11.6 or later, the above command will timeout. In that case, you can quickly try an older version like cuda 11.3:
 ~~~
-conda install pytorch==1.12.0 cudatoolkit=11.3 -c pytorch
+conda install pytorch==1.12.0 torchvision==0.13.0 cudatoolkit=11.3 -c pytorch
 ~~~~
 Info on how to install several older versions is available [here](https://pytorch.org/get-started/previous-versions/). 
 
 After install you can check `conda list` for `pytorch`, and its version info should have `cuXX.X`, not `cpu`.
 
+## Common Installation Problems
+
+You may receive the following error upon upgrading `torch` and `torchvision`:
+~~~
+AttributeError: partially initialized module 'charset_normalizer' has no attribute 'md__mypyc' (most likely due to a circular import)
+~~~
+This is solved by upgrading the charselt_normalizer package with the following command: `AttributeError: partially initialized module 'charset_normalizer' has no attribute 'md__mypyc' (most likely due to a circular import)`
+
+Report any other installation errors.
+
 # Run yeastvision locally
 
 The quickest way to start is to open the GUI from a command line terminal. Activate the correct conda environment, then run:
 ~~~~
 yeastvision
 ~~~~
```

### Comparing `yeastvision-0.1.7/setup.py` & `yeastvision-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 requires = ["cellpose==2.1.0",
 "matplotlib==3.6.0",
 "munkres==1.1.4",
 "numpy==1.23.3",
 "opencv_python_headless==4.6.0.66",
 "pandas==1.5.0",
 "patchify==0.2.3",
-"Pillow==9.5.0",
 "PyQt5==5.15.9",
 "pyqtgraph==0.13.0",
 "scikit_image==0.19.3",
 "scikit_learn==1.2.2",
 "scipy==1.9.1",
 "tensorflow==2.10.0",
-"torch==1.12.1",
+"torch==1.12.0",
 "tqdm==4.65.0",
-"trackpy==0.5.0"]
+"trackpy==0.5.0",
+"torchvision==0.13.0",
+"memory-profiler"]
 
 try:
     import torch
     a = torch.ones(2, 3)
     major_version, minor_version, _ = torch.__version__.split(".")
     if major_version == "2" or int(minor_version) >= 12:
-        requires.remove("torch==1.12.1")
+        requires.remove("torch==1.12.0")
+        requires.remove("torchvision==0.13.0")
 except:
     pass
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 packages = ["yeastvision", "yeastvision.plot", "yeastvision.track", "yeastvision.models", "yeastvision.ims", "yeastvision.ims.rife_model",
-            "yeastvision.parts", "yeastvision.flou", "yeastvision.disk", 
-            "yeastvision.models.artilife", "yeastvision.models.artilife.budSeg",
+            "yeastvision.ims.rife_model.pytorch_msssim", "yeastvision.parts", "yeastvision.flou", "yeastvision.disk", 
+            "yeastvision.models.artilife", "yeastvision.models.artilife.budSeg", "yeastvision.models.artiBud",
             "yeastvision.models.matSeg", "yeastvision.models.tetradSeg", "yeastvision.models.budNET", 
             "yeastvision.models.vacNET", "yeastvision.models.YeaZ"]
 
 
-
-
 setup(
     name = "yeastvision",
-    version = "0.1.7",
+    version = "0.1.9",
     description = "Deep learning-enabled image analysis of the yeast full life cycle",
     author = "Berk Yalcinkaya",
     url = "https://github.com/berkyalcinkaya/yeastvision",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author_email="berkyalcinkaya55@gmail.com",
     license = "BSD",
```

### Comparing `yeastvision-0.1.7/yeastvision/__main__.py` & `yeastvision-0.1.9/yeastvision/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from functools import partial
 
 
 class MainWindow(QtWidgets.QMainWindow):
     def __init__(self, thread, imPaths = None, labelPaths = None):
         super(MainWindow, self).__init__()
         pg.setConfigOption('imageAxisOrder', 'row-major')
-        self.setGeometry(50, 50, 1300, 1300)
+        self.setGeometry(100, 100, 900, 1000)
         self.setAcceptDrops(True)
 
         #self.idealThreadCount  = thread.idealThreadCount()//2
         self.idealThreadCount = 2
 
         self.sessionId = self.getCurrTimeStr()
         
@@ -99,16 +99,16 @@
         self.currImDtype = "uint8"
 
         self.threads = []
         self.workers = []
         
         self.setEmptyDisplay(initial=True)
         self.build_widgets()
-        self.l.setHorizontalSpacing(8)
-        self.l.setVerticalSpacing(8)
+        self.l.setHorizontalSpacing(15)
+        self.l.setVerticalSpacing(15)
         
         self.drawType = ""
         self.cellToChange = 0
 
         self.annotationList = []
 
         self.addRegionStrokes = []
@@ -250,17 +250,15 @@
         self.maskOn = True
         self.contourOn = False
         self.probOn = False
         self.maskZ = -1
         self.currMask = np.zeros((512,512), dtype = np.uint8)
         self.pg_mask.setImage(self.currMask, autolevels  =False, levels =[0,0], lut = self.maskColors)
 
-        
-
-
+    
         self.cellData = [] 
         self.mother_daughters = []
 
         if not initial:
             self.labelSelect.clear()
             self.maskTypeSelect.uncheckAll()
             self.contourButton.setChecked(False)
@@ -429,15 +427,15 @@
         self.dataDisplay = QLabel("")
         self.dataDisplay.setMinimumWidth(300)
         # self.dataDisplay.setMaximumWidth(300)
         self.dataDisplay.setStyleSheet(self.labelstyle)
         self.dataDisplay.setFont(self.smallfont)
         self.dataDisplay.setAlignment(QtCore.Qt.AlignLeft | QtCore.Qt.AlignBottom)
         self.updateDataDisplay()
-        self.l.addWidget(self.dataDisplay, rowspace-1,cspace+1,1,20)
+        self.l.addWidget(self.dataDisplay, rowspace-1,cspace-1,1,20)
 
         label = QLabel('Drawing:')#[\u2191 \u2193]')
         label.setStyleSheet(self.headings)
         label.setFont(self.boldfont)
         self.l.addWidget(label, rowspace,1,1,5)
 
         label = QLabel("Brush Type:")
@@ -912,19 +910,40 @@
         else:
             if isinstance(self.cellData[cellI], TimeSeriesData):
                 life = self.cellData[cellI].life_data
                 cell_data = self.cellData[cellI].cell_data
             else:
                 life, cell_data = None, None
 
-            self.cellData[cellI] = LineageData(cellI, cells, necks, cell_data=cell_data, life_data=life)
+            self.cellData[cellI] = LineageData(cellI, cells, buds = necks, cell_data=cell_data, life_data=life)
+
+        self.saveData()
+        self.checkDataAvailibility()
+    
+    def getMatingLineages(self, cellI, matingI):
+        mating = self.maskData.channels[matingI][0,:,:,:]
+        cells = self.maskData.channels[cellI][0,:,:,:]
+
+        if isinstance(self.cellData[cellI], LineageData):
+            self.cellData[cellI].add_mating(cells, mating)
+        else:
+            if isinstance(self.cellData[cellI], TimeSeriesData):
+                life = self.cellData[cellI].life_data
+                cell_data = self.cellData[cellI].cell_data
+            else:
+                life, cell_data = None, None
+
+            self.cellData[cellI] = LineageData(cellI, cells, mating = mating, cell_data=cell_data, life_data=life)
 
         self.saveData()
         self.checkDataAvailibility()
     
+
+        
+    
     def getCellDataLabelProps(self):
         label_props = LABEL_PROPS.copy()
         label_props.remove("label")
         return sorted(label_props)
 
     def getCellDataImProperties(self, i = None):
         if not i:
@@ -1552,15 +1571,14 @@
                 error_dialog  = QErrorMessage()
                 error_dialog.showMessage(f"Cannot Segment Until Other Processes are Finished")
                 self.activateButton(self.segButton)
                 return
         else:
             return
 
-        
     def getModels(self):
         for modelName in self.modelNames:
             if os.path.exists(os.path.join("models",modelName,"model.py")):
                 importlib.import_module(self.getPkgString(modelName))
     
     def getPkgString(self, string):
         return f"yeastvision.models.{string}.model"
@@ -1672,16 +1690,14 @@
         if len(self.modelNames)==0:
             self.showError("Weights Have Not Been Downloaded. Find the weights at https://drive.google.com/file/d/1J3R4JKILkQNM0Ap-MKxqv61oAxObSjBo/view?usp=drive_link. Then run install-weights in the same directory as the downloaded zip file.")
 
 
     def segment(self, output, modelClass, ims, params, weightPath, modelType):
 
         tStart, tStop = int(params["T Start"]), int(params["T Stop"])
-
-
         imName = params["Channel"]
 
         if modelType == "artilife":
             counter = 0
             for labelName, outputTup in output.items():
                 if type(outputTup[0]) == np.ndarray:
                     counter += 1
@@ -1689,16 +1705,23 @@
                     for i in [0,1]:
                         template = np.zeros_like(ims, dtype = outputTup[i].dtype)
                         template[tStart:tStop+1] = outputTup[i]
                         templates.append(template)
                     outputTup = (templates[0], templates[1])
                     self.loadMasks(outputTup, name = f"{imName}_{labelName}")
             if params["Time Series"]:
+                if params["Mating Cells"]:
+                    mating_idx = self.maskZ -1
+                    cell_idx = self.maskZ
+                    self.getMatingLineage(cell_idx, mating_idx)
+
                 idx = self.maskZ - counter
                 self.updateCellData(idx = idx)
+
+
         else:
             templates = []
             for i in [0,1]:
                 template = np.zeros_like(ims, dtype = output[i].dtype)
                 template[tStart:tStop+1] = output[i]
                 templates.append(template)
             outputTup = (templates[0], templates[1])
```

### Comparing `yeastvision-0.1.7/yeastvision/disk/io.py` & `yeastvision-0.1.9/yeastvision/disk/io.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/disk/reader.py` & `yeastvision-0.1.9/yeastvision/disk/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,16 @@
         names.append(all_files[i].split("_")[-1])
         for n in range(i,num_ims, num_channels):
             channels[n,:,:,i] = imread(all_files[n])
             files[i].append(all_files[n])
 
     return channels, files, names
 
+
+
 def get_channel_files_from_dir(dir, num_channels):
     '''Loads images seperately by channel 
     
     Parameters
     ----------
     
     dir: string 
@@ -299,15 +301,15 @@
     def labelIms(self, ims):
         return np.array([label((im>0).astype(ims.dtype)) for im in ims])
 
     def isBinary(self, mask):
         return np.array_equal(mask, mask.astype(bool))
     
     def isFloat(self,im):
-        return im.dtype.kind ==  "f" and np.all(im<=1.0)
+        return im.dtype.kind == "f" and np.all(im<=1.0)
     
     def addZ(self,imData, pred = False, contours = None):
     
         hasFloats = False
         if type(imData) is tuple:
             ims,floats = imData
             hasFloats = True
```

### Comparing `yeastvision-0.1.7/yeastvision/flou/blob_detect.py` & `yeastvision-0.1.9/yeastvision/flou/blob_detect.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/flou/utils.py` & `yeastvision-0.1.9/yeastvision/flou/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/ims/im_funcs.py` & `yeastvision-0.1.9/yeastvision/ims/im_funcs.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/ims/interpolate.py` & `yeastvision-0.1.9/yeastvision/ims/interpolate.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import torch
 import numpy as np
 from yeastvision.ims.rife_model.pytorch_msssim import ssim_matlab
 from queue import Queue, Empty
 from skimage.util import img_as_ubyte
 from .rife_model.RIFE import Model
 import os
+from yeastvision.ims import rife_model
 
+RIFE_DIR = rife_model.__path__[0]
 
 def interpolate(ims: np.ndarray, exp: int)->np.ndarray:
     scale = 1
     
     def make_inference(I0, I1, n):
         middle = model.inference(I0, I1, scale)
         if n == 1:
@@ -44,23 +46,24 @@
 
     ims = ims = [reformat(im) for im in ims]
     lastframe = ims[0]
     h,w,_ = lastframe.shape
     ims = ims[1:]
 
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    torch.set_grad_enabled(False)
     if torch.cuda.is_available():
         torch.backends.cudnn.enabled = True
         torch.backends.cudnn.benchmark = True
     
     model = Model()
-    print(os.getcwd())
-    model.load_model("yeastvision/ims/train_log")
+    model.load_model(RIFE_DIR, -1)
     model.eval()
     model.device()
+    
 
     write_buffer = []
     read_buffer = make_read_buffer(ims)
 
     I1 = torch.from_numpy(np.transpose(lastframe, (2,0,1))).to(device, non_blocking=True).unsqueeze(0).float() / 255.
     I1 = pad_image(I1)
     temp = None # save lastframe when processing static frame
```

### Comparing `yeastvision-0.1.7/yeastvision/ims/rife_model/IFNet.py` & `yeastvision-0.1.9/yeastvision/ims/rife_model/IFNet.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/ims/rife_model/IFNet_2R.py` & `yeastvision-0.1.9/yeastvision/ims/rife_model/IFNet_2R.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/ims/rife_model/IFNet_m.py` & `yeastvision-0.1.9/yeastvision/ims/rife_model/IFNet_m.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/ims/rife_model/RIFE.py` & `yeastvision-0.1.9/yeastvision/ims/rife_model/RIFE.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             return {
             k.replace("module.", ""): v
                 for k, v in param.items()
                 if "module." in k
             }
             
         if rank <= 0:
-            self.flownet.load_state_dict(convert(torch.load('{}/flownet.pkl'.format(path))))
+            self.flownet.load_state_dict(convert(torch.load('{}/flownet.pkl'.format(path), map_location=device)))
         
     def save_model(self, path, rank=0):
         if rank == 0:
             torch.save(self.flownet.state_dict(),'{}/flownet.pkl'.format(path))
 
     def inference(self, img0, img1, scale=1, scale_list=[4, 2, 1], TTA=False, timestep=0.5):
         for i in range(3):
```

### Comparing `yeastvision-0.1.7/yeastvision/ims/rife_model/laplacian.py` & `yeastvision-0.1.9/yeastvision/ims/rife_model/laplacian.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/ims/rife_model/loss.py` & `yeastvision-0.1.9/yeastvision/ims/rife_model/loss.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/ims/rife_model/refine.py` & `yeastvision-0.1.9/yeastvision/ims/rife_model/refine.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/ims/rife_model/refine_2R.py` & `yeastvision-0.1.9/yeastvision/ims/rife_model/refine_2R.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/ims/rife_model/warplayer.py` & `yeastvision-0.1.9/yeastvision/ims/rife_model/warplayer.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/install_weights.py` & `yeastvision-0.1.9/yeastvision/install_weights.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/models/YeaZ/model.py` & `yeastvision-0.1.9/yeastvision/models/YeaZ/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/models/YeaZ/segment.py` & `yeastvision-0.1.9/yeastvision/models/YeaZ/segment.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/models/YeaZ/unet.py` & `yeastvision-0.1.9/yeastvision/models/YeaZ/unet.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/models/artilife/budSeg/model.py` & `yeastvision-0.1.9/yeastvision/models/artilife/budSeg/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/models/artilife/model.py` & `yeastvision-0.1.9/yeastvision/models/artilife/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/models/budNET/model.py` & `yeastvision-0.1.9/yeastvision/models/budNET/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/models/cp.py` & `yeastvision-0.1.9/yeastvision/models/cp.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/models/model.py` & `yeastvision-0.1.9/yeastvision/models/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/models/unet.py` & `yeastvision-0.1.9/yeastvision/models/unet.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/models/utils.py` & `yeastvision-0.1.9/yeastvision/models/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/parts/canvas.py` & `yeastvision-0.1.9/yeastvision/parts/canvas.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/parts/dialogs.py` & `yeastvision-0.1.9/yeastvision/parts/dialogs.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/parts/guiparts.py` & `yeastvision-0.1.9/yeastvision/parts/guiparts.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/parts/menu.py` & `yeastvision-0.1.9/yeastvision/parts/menu.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/parts/workers.py` & `yeastvision-0.1.9/yeastvision/parts/workers.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/plot/cell_table.py` & `yeastvision-0.1.9/yeastvision/plot/cell_table.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/plot/plot.py` & `yeastvision-0.1.9/yeastvision/plot/plot.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/plot/types.py` & `yeastvision-0.1.9/yeastvision/plot/types.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/track/cell.py` & `yeastvision-0.1.9/yeastvision/track/cell.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/track/data.py` & `yeastvision-0.1.9/yeastvision/track/data.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/track/hungarian_track.py` & `yeastvision-0.1.9/yeastvision/track/hungarian_track.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/track/lineage.py` & `yeastvision-0.1.9/yeastvision/track/lineage.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/track/mat.py` & `yeastvision-0.1.9/yeastvision/track/mat.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,15 @@
 import yeastvision.track.utils as f
 from yeastvision.utils import showCellNums
 import statistics as stats
 import matplotlib.pyplot as plt
 from skimage.morphology import thin, skeletonize, opening, dilation, erosion, square
 from skimage.measure import regionprops, label
 from tqdm import tqdm
-
-def get_mating_data(mating, cells):
-    mating_tracks = correct_mat_tracks(track_mating(mating))
-    return merge(cells, mating_tracks)
-
+from yeastvision.track.cell import getBirthFrame
 
 def track_mating(mating_masks, visualize = False):
     cell_margin = 20
     numbM = len(mating_masks)
     MATC = [[[] for _ in range(numbM)] for _ in range(2)]
     
     # First loop, for leading cell number one
```

### Comparing `yeastvision-0.1.7/yeastvision/track/track.py` & `yeastvision-0.1.9/yeastvision/track/track.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/track/utils.py` & `yeastvision-0.1.9/yeastvision/track/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision/utils.py` & `yeastvision-0.1.9/yeastvision/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.7/yeastvision.egg-info/PKG-INFO` & `yeastvision-0.1.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: yeastvision
-Version: 0.1.7
-Summary: Deep learning-enabled image analysis of the yeast full life cycle
-Home-page: https://github.com/berkyalcinkaya/yeastvision
-Author: Berk Yalcinkaya
-Author-email: berkyalcinkaya55@gmail.com
-License: BSD
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # <p>  <b>YeastVision </b> </p>
 
 
 # Installation
 
 ## Local installation (< 2 minutes)
 
@@ -24,19 +12,19 @@
 ### Instructions 
 
 If you have an older `yeastvision` environment you should remove it with `conda env remove -n yeastvision` before creating a new one. 
 
 Yeastvision is ready to go for cpu-usage as soon as it downloaded. GPU-usage requires some additional steps after download. To download:
 
 1. Install an [Anaconda](https://www.anaconda.com/products/distribution) distribution of Python. Note you might need to use an anaconda prompt if you did not add anaconda to the path.
-2. Open an anaconda prompt / command prompt which has `conda` for **python 3** in the path
-3. Create a new environment with `conda create --name yeastvision python=3.10.o`. 
+2. Open an anaconda prompt/command prompt
+3. Create a new environment with `conda create --name yeastvision python=3.10.0`. 
 4. Activate this new environment by running `conda activate yeastvision`
 5. Run `python -m pip install yeastvision` to download our package plus all dependencies
-6. Download the weights [online](https://drive.google.com/file/d/1Zl3b00eSbe3wbxpYOknEP5q0A86XtEfL/view?usp=sharing). 
+6. Download the weights [online](https://drive.google.com/file/d/1sxYyiRmLxykJcb3PXxa7p4iGEOa96APk/view?usp=sharing). 
 7. Run `install-weights` in the same directory as the *yeastvision_weights.zip* file
 
 
 You should upgrade yeastvision (package [here](https://pypi.org/project/yeastvision/)) periodically as it is still in development. To do so, run the following in the environment:
 
 ~~~sh
 python -m pip install yeastvision --upgrade
@@ -48,36 +36,51 @@
 
 To use your NVIDIA GPU with python, you will first need to install the NVIDIA driver for your GPU, check out this [website](https://www.nvidia.com/Download/index.aspx?lang=en-us) to download it. Ensure it is downloaded and your GPU is detected by running `nvidia-smi` in the terminal.
 
 Next we need to remove the CPU version of torch:
 ~~~
 pip uninstall torch
 ~~~
-
-To install the GPU version of torch, follow the instructions [here](https://pytorch.org/get-started/locally/). The conda install is strongly recommended, and then choose the CUDA version that is supported by your GPU (newer GPUs may need newer CUDA versions > 10.2). For instance this command will install the 11.6 version on Linux and Windows (note the `torchvision` and `torchaudio` commands are removed because yeastvision doesn't require them):
+And the cpu version of torchvision:
 ~~~
-conda install pytorch pytorch-cuda=11.6 -c pytorch -c nvidia
+pip uninstall torchvision
 ~~~
 
-If you are unable to install the package using the command above, try an older version like cuda 11.3:
+To install the GPU version of torch and torchvision, first ensure you have downloaded the proper nvidia drivers for your GPU. Then for pytorch and torchvision, follow the instructions [here](https://pytorch.org/get-started/locally/). The conda install is strongly recommended, and then choose the CUDA version that is supported by your GPU (newer GPUs may need newer CUDA versions > 10.2). You can check the highest version of CUDA that your nvidia driver supports by running: 
+~~~
+nvidia-smi
+~~~
+For instance this command will install the 11.6 version on Linux and Windows (note the `torchaudio` commands are removed because yeastvision doesn't require them):
 ~~~
-conda install pytorch==1.12.0 cudatoolkit=11.3 -c pytorch
+conda install pytorch==1.12.0 torchvision==0.13.0 pytorch-cuda=11.6 -c pytorch -c nvidia
+~~~
+The 11.6 configuration is recommended as this system was thoroughly tested with this system.  However, for some GPUs which do not support CUDA 11.6 or later, the above command will timeout. In that case, you can quickly try an older version like cuda 11.3:
+~~~
+conda install pytorch==1.12.0 torchvision==0.13.0 cudatoolkit=11.3 -c pytorch
 ~~~~
 Info on how to install several older versions is available [here](https://pytorch.org/get-started/previous-versions/). 
 
 After install you can check `conda list` for `pytorch`, and its version info should have `cuXX.X`, not `cpu`.
 
+## Common Installation Problems
+
+You may receive the following error upon upgrading `torch` and `torchvision`:
+~~~
+AttributeError: partially initialized module 'charset_normalizer' has no attribute 'md__mypyc' (most likely due to a circular import)
+~~~
+This is solved by upgrading the charselt_normalizer package with the following command: `AttributeError: partially initialized module 'charset_normalizer' has no attribute 'md__mypyc' (most likely due to a circular import)`
+
+Report any other installation errors.
+
 # Run yeastvision locally
 
 The quickest way to start is to open the GUI from a command line terminal. Activate the correct conda environment, then run:
 ~~~~
 yeastvision
 ~~~~
 
 To get started, drop an image or directory of images into the GUI. 
 
 **Masks can be loaded by dropping them into the top half of the screen.**
 
 
 
-
-
```

### Comparing `yeastvision-0.1.7/yeastvision.egg-info/SOURCES.txt` & `yeastvision-0.1.9/yeastvision.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -21,31 +21,33 @@
 yeastvision/ims/im_funcs.py
 yeastvision/ims/interpolate.py
 yeastvision/ims/rife_model/IFNet.py
 yeastvision/ims/rife_model/IFNet_2R.py
 yeastvision/ims/rife_model/IFNet_m.py
 yeastvision/ims/rife_model/RIFE.py
 yeastvision/ims/rife_model/__init__.py
-yeastvision/ims/rife_model/interpolate.py
 yeastvision/ims/rife_model/laplacian.py
 yeastvision/ims/rife_model/loss.py
 yeastvision/ims/rife_model/refine.py
 yeastvision/ims/rife_model/refine_2R.py
 yeastvision/ims/rife_model/warplayer.py
+yeastvision/ims/rife_model/pytorch_msssim/__init__.py
 yeastvision/models/__init__.py
 yeastvision/models/cp.py
 yeastvision/models/eval.py
 yeastvision/models/loss.py
 yeastvision/models/model.py
 yeastvision/models/unet.py
 yeastvision/models/utils.py
 yeastvision/models/YeaZ/__init__.py
 yeastvision/models/YeaZ/model.py
 yeastvision/models/YeaZ/segment.py
 yeastvision/models/YeaZ/unet.py
+yeastvision/models/artiBud/__init__.py
+yeastvision/models/artiBud/model.py
 yeastvision/models/artilife/__init__.py
 yeastvision/models/artilife/model.py
 yeastvision/models/artilife/budSeg/__init__.py
 yeastvision/models/artilife/budSeg/model.py
 yeastvision/models/budNET/__init__.py
 yeastvision/models/budNET/model.py
 yeastvision/models/matSeg/__init__.py
```

