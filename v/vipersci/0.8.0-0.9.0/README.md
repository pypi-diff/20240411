# Comparing `tmp/vipersci-0.8.0.tar.gz` & `tmp/vipersci-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipersci-0.8.0.tar", last modified: Wed Feb 21 21:16:53 2024, max compression
+gzip compressed data, was "vipersci-0.9.0.tar", last modified: Wed Apr 10 21:25:25 2024, max compression
```

## Comparing `vipersci-0.8.0.tar` & `vipersci-0.9.0.tar`

### file list

```diff
@@ -1,151 +1,153 @@
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.804102 vipersci-0.8.0/
--rw-r--r--   0 rbeyer     (503) staff       (20)      614 2023-09-25 00:36:59.000000 vipersci-0.8.0/AUTHORS.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)    12197 2024-02-21 21:13:54.000000 vipersci-0.8.0/CHANGELOG.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)     7942 2024-02-07 01:56:52.000000 vipersci-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)    11357 2021-10-25 21:26:36.000000 vipersci-0.8.0/LICENSE
--rw-r--r--   0 rbeyer     (503) staff       (20)      264 2021-10-25 21:34:05.000000 vipersci-0.8.0/MANIFEST.in
--rw-r--r--   0 rbeyer     (503) staff       (20)    16625 2024-02-21 21:16:53.803774 vipersci-0.8.0/PKG-INFO
--rw-r--r--   0 rbeyer     (503) staff       (20)     3295 2023-07-26 18:46:41.000000 vipersci-0.8.0/README.rst
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.580915 vipersci-0.8.0/docs/
--rw-r--r--   0 rbeyer     (503) staff       (20)      609 2021-10-25 21:48:39.000000 vipersci-0.8.0/docs/Makefile
--rw-r--r--   0 rbeyer     (503) staff       (20)       28 2021-03-28 21:36:13.000000 vipersci-0.8.0/docs/authors.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)       30 2022-10-06 00:17:46.000000 vipersci-0.8.0/docs/changelog.rst
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     4895 2022-11-01 14:54:30.000000 vipersci-0.8.0/docs/conf.py
--rw-r--r--   0 rbeyer     (503) staff       (20)       33 2021-03-28 21:36:13.000000 vipersci-0.8.0/docs/contributing.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      307 2022-10-06 00:17:46.000000 vipersci-0.8.0/docs/index.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      716 2022-10-06 00:17:46.000000 vipersci-0.8.0/docs/installation.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      770 2021-10-25 21:48:14.000000 vipersci-0.8.0/docs/make.bat
--rw-r--r--   0 rbeyer     (503) staff       (20)       61 2022-10-05 23:23:34.000000 vipersci-0.8.0/docs/modules.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)       27 2021-03-28 21:36:13.000000 vipersci-0.8.0/docs/readme.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)       71 2021-10-25 21:48:27.000000 vipersci-0.8.0/docs/usage.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      260 2022-10-05 23:15:23.000000 vipersci-0.8.0/docs/vipersci.pds.data.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      201 2022-10-05 23:15:23.000000 vipersci-0.8.0/docs/vipersci.pds.data.template.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      927 2022-10-05 23:15:23.000000 vipersci-0.8.0/docs/vipersci.pds.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      511 2022-10-05 23:23:34.000000 vipersci-0.8.0/docs/vipersci.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      465 2022-10-05 23:15:23.000000 vipersci-0.8.0/docs/vipersci.vis.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      356 2023-05-05 04:04:23.000000 vipersci-0.8.0/pyproject.toml
--rw-r--r--   0 rbeyer     (503) staff       (20)     3070 2024-02-21 21:16:53.806008 vipersci-0.8.0/setup.cfg
--rw-r--r--   0 rbeyer     (503) staff       (20)       86 2022-11-08 00:15:45.000000 vipersci-0.8.0/setup.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.439440 vipersci-0.8.0/src/
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.703825 vipersci-0.8.0/src/vipersci/
--rw-r--r--   0 rbeyer     (503) staff       (20)      130 2024-02-21 21:15:23.000000 vipersci-0.8.0/src/vipersci/__init__.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.739042 vipersci-0.8.0/src/vipersci/carto/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-11-14 18:58:15.000000 vipersci-0.8.0/src/vipersci/carto/__init__.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     3731 2023-04-11 20:22:14.000000 vipersci-0.8.0/src/vipersci/carto/accrual.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3454 2023-03-01 16:59:24.000000 vipersci-0.8.0/src/vipersci/carto/bounds.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)    12418 2024-02-07 01:56:52.000000 vipersci-0.8.0/src/vipersci/carto/colorforge.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     3718 2022-11-10 16:51:53.000000 vipersci-0.8.0/src/vipersci/carto/dice_buffer.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     2325 2022-11-10 16:51:53.000000 vipersci-0.8.0/src/vipersci/carto/dissolve_dice.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3463 2023-03-01 16:59:24.000000 vipersci-0.8.0/src/vipersci/carto/dotmap.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     5171 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/carto/get_position.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    20383 2023-07-26 18:42:09.000000 vipersci-0.8.0/src/vipersci/carto/heatmap.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     5959 2022-11-10 16:51:53.000000 vipersci-0.8.0/src/vipersci/carto/msolo_simulator.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     6644 2022-11-10 16:51:53.000000 vipersci-0.8.0/src/vipersci/carto/nirvss_simulator.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     3061 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/carto/nss_modeler.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     7540 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/carto/nss_simulator.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.739911 vipersci-0.8.0/src/vipersci/carto/pds/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2023-04-23 00:01:47.000000 vipersci-0.8.0/src/vipersci/carto/pds/__init__.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.740490 vipersci-0.8.0/src/vipersci/carto/pds/data/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2023-04-23 00:03:38.000000 vipersci-0.8.0/src/vipersci/carto/pds/data/__init__.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     3733 2024-02-07 01:56:52.000000 vipersci-0.8.0/src/vipersci/carto/traverse_interpolator.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)    11429 2023-07-26 18:42:09.000000 vipersci-0.8.0/src/vipersci/carto/tri2gpkg.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1434 2022-11-01 14:54:30.000000 vipersci-0.8.0/src/vipersci/msolo.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1382 2022-11-01 14:54:30.000000 vipersci-0.8.0/src/vipersci/nirvss.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    10898 2023-06-06 20:26:52.000000 vipersci-0.8.0/src/vipersci/nss.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.744193 vipersci-0.8.0/src/vipersci/pds/
--rw-r--r--   0 rbeyer     (503) staff       (20)     2035 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/pds/__init__.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     5234 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/pds/bundle_install.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     2901 2023-10-27 17:08:28.000000 vipersci-0.8.0/src/vipersci/pds/datetime.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.747536 vipersci-0.8.0/src/vipersci/pds/labelmaker/
--rw-r--r--   0 rbeyer     (503) staff       (20)     9858 2024-02-07 01:56:52.000000 vipersci-0.8.0/src/vipersci/pds/labelmaker/__init__.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     4267 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/pds/labelmaker/bundle.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1755 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/pds/labelmaker/cli.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     4747 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/pds/labelmaker/collection.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1975 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/pds/labelmaker/generic.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2290 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/pds/labelmaker/inventory.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)    16452 2024-02-21 21:07:21.000000 vipersci-0.8.0/src/vipersci/pds/pid.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     2030 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/pds/xml.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2566 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/util.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.752885 vipersci-0.8.0/src/vipersci/vis/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.8.0/src/vipersci/vis/__init__.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     5421 2023-10-05 22:33:13.000000 vipersci-0.8.0/src/vipersci/vis/anaglyph.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2537 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/vis/anom_pixel.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    12800 2024-02-21 03:54:05.000000 vipersci-0.8.0/src/vipersci/vis/create_image.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     7758 2024-02-21 21:07:21.000000 vipersci-0.8.0/src/vipersci/vis/create_mmgis_pano.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    11737 2024-01-31 17:28:33.000000 vipersci-0.8.0/src/vipersci/vis/create_pano.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2031 2023-08-09 00:22:12.000000 vipersci-0.8.0/src/vipersci/vis/create_tif.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.760252 vipersci-0.8.0/src/vipersci/vis/db/
--rw-r--r--   0 rbeyer     (503) staff       (20)     1093 2023-07-26 18:42:09.000000 vipersci-0.8.0/src/vipersci/vis/db/__init__.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     5674 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/vis/db/create_vis_dbs.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    28411 2024-02-21 21:07:21.000000 vipersci-0.8.0/src/vipersci/vis/db/image_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    10446 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/vis/db/image_requests.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1888 2023-08-09 00:22:12.000000 vipersci-0.8.0/src/vipersci/vis/db/image_stats.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2148 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/vis/db/image_tags.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1877 2023-10-24 18:52:44.000000 vipersci-0.8.0/src/vipersci/vis/db/junc_image_pano.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2045 2023-09-21 04:19:35.000000 vipersci-0.8.0/src/vipersci/vis/db/junc_image_record_tags.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2704 2023-10-24 18:52:44.000000 vipersci-0.8.0/src/vipersci/vis/db/junc_image_req_ldst.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1680 2023-09-23 17:38:22.000000 vipersci-0.8.0/src/vipersci/vis/db/ldst.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3752 2023-10-24 18:52:44.000000 vipersci-0.8.0/src/vipersci/vis/db/light_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     9404 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/vis/db/pano_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3291 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/vis/db/ptu_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1951 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/vis/db/validators.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3192 2023-08-09 00:22:12.000000 vipersci-0.8.0/src/vipersci/vis/header.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     4322 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/vis/image_statistics.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     9243 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/vis/pano_check.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.762714 vipersci-0.8.0/src/vipersci/vis/pds/
--rw-r--r--   0 rbeyer     (503) staff       (20)     2701 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/vis/pds/__init__.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     5178 2024-02-07 01:56:52.000000 vipersci-0.8.0/src/vipersci/vis/pds/create_browse.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     7341 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/vis/pds/create_pano_product.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    12931 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/vis/pds/create_raw.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.763196 vipersci-0.8.0/src/vipersci/vis/pds/data/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.8.0/src/vipersci/vis/pds/data/__init__.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     5342 2024-01-26 00:56:09.000000 vipersci-0.8.0/src/vipersci/vis/viseer.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.802982 vipersci-0.8.0/src/vipersci.egg-info/
--rw-r--r--   0 rbeyer     (503) staff       (20)    16625 2024-02-21 21:16:53.000000 vipersci-0.8.0/src/vipersci.egg-info/PKG-INFO
--rw-r--r--   0 rbeyer     (503) staff       (20)     3836 2024-02-21 21:16:53.000000 vipersci-0.8.0/src/vipersci.egg-info/SOURCES.txt
--rw-r--r--   0 rbeyer     (503) staff       (20)        1 2024-02-21 21:16:53.000000 vipersci-0.8.0/src/vipersci.egg-info/dependency_links.txt
--rw-r--r--   0 rbeyer     (503) staff       (20)     1344 2024-02-21 21:16:53.000000 vipersci-0.8.0/src/vipersci.egg-info/entry_points.txt
--rw-r--r--   0 rbeyer     (503) staff       (20)        1 2024-02-21 21:16:53.000000 vipersci-0.8.0/src/vipersci.egg-info/not-zip-safe
--rw-r--r--   0 rbeyer     (503) staff       (20)      121 2024-02-21 21:16:53.000000 vipersci-0.8.0/src/vipersci.egg-info/requires.txt
--rw-r--r--   0 rbeyer     (503) staff       (20)        9 2024-02-21 21:16:53.000000 vipersci-0.8.0/src/vipersci.egg-info/top_level.txt
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-02-21 21:16:53.802127 vipersci-0.8.0/tests/
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     2301 2023-08-09 00:22:12.000000 vipersci-0.8.0/tests/datetime_sqlite.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     6112 2023-09-06 15:17:57.000000 vipersci-0.8.0/tests/test_anaglyph.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1682 2022-11-30 20:55:10.000000 vipersci-0.8.0/tests/test_area_bin.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    11820 2023-05-05 04:04:23.000000 vipersci-0.8.0/tests/test_colorforge.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    11937 2024-02-21 21:07:21.000000 vipersci-0.8.0/tests/test_create_image.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     9001 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_create_pano.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     8441 2024-02-21 21:07:21.000000 vipersci-0.8.0/tests/test_create_pano_product.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     6123 2024-02-21 21:07:21.000000 vipersci-0.8.0/tests/test_create_raw.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1636 2023-08-09 00:22:12.000000 vipersci-0.8.0/tests/test_create_tif.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2848 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_create_vis_dbs.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1644 2022-11-30 20:55:10.000000 vipersci-0.8.0/tests/test_datetime.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     8388 2023-07-26 18:42:09.000000 vipersci-0.8.0/tests/test_density_heatmap.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3895 2023-02-24 03:28:58.000000 vipersci-0.8.0/tests/test_dotmap.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2526 2023-02-24 03:28:58.000000 vipersci-0.8.0/tests/test_heatmap_helpers.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    22487 2024-02-21 21:07:21.000000 vipersci-0.8.0/tests/test_image_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3835 2023-09-23 17:38:22.000000 vipersci-0.8.0/tests/test_image_requests.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2602 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_image_statistics.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1300 2023-08-09 00:22:12.000000 vipersci-0.8.0/tests/test_image_stats.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1192 2023-09-21 04:19:35.000000 vipersci-0.8.0/tests/test_image_tags.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    11202 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_labelmaker.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     5619 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_labelmaker_bundle.py
--rw-r--r--   0 rbeyer     (503) staff       (20)      571 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_labelmaker_cli.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     6289 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_labelmaker_collection.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1588 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_labelmaker_generic.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1549 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_labelmaker_inventory.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1773 2023-10-24 18:52:44.000000 vipersci-0.8.0/tests/test_light_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1646 2022-11-01 14:54:30.000000 vipersci-0.8.0/tests/test_msolo.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2278 2023-02-24 03:28:58.000000 vipersci-0.8.0/tests/test_msolo_simulator.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1649 2022-11-01 14:54:30.000000 vipersci-0.8.0/tests/test_nirvss.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2387 2023-02-24 03:28:58.000000 vipersci-0.8.0/tests/test_nirvss_simulator.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3737 2022-11-01 14:54:30.000000 vipersci-0.8.0/tests/test_nss.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1782 2022-11-30 20:55:10.000000 vipersci-0.8.0/tests/test_nss_modeler.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2727 2022-11-30 20:55:10.000000 vipersci-0.8.0/tests/test_nss_simulator.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     4591 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_pano_check.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3807 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_pano_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    13805 2024-02-21 21:07:21.000000 vipersci-0.8.0/tests/test_pid.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1589 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_util.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2333 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_validators.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2588 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_vis_pds.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2826 2024-01-26 00:56:09.000000 vipersci-0.8.0/tests/test_xml.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.280402 vipersci-0.9.0/
+-rw-r--r--   0 rbeyer     (503) staff       (20)      614 2023-09-25 00:36:59.000000 vipersci-0.9.0/AUTHORS.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)    12993 2024-04-10 21:24:13.000000 vipersci-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)     7942 2024-02-07 01:56:52.000000 vipersci-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11357 2021-10-25 21:26:36.000000 vipersci-0.9.0/LICENSE
+-rw-r--r--   0 rbeyer     (503) staff       (20)      264 2021-10-25 21:34:05.000000 vipersci-0.9.0/MANIFEST.in
+-rw-r--r--   0 rbeyer     (503) staff       (20)    17421 2024-04-10 21:25:25.280007 vipersci-0.9.0/PKG-INFO
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3295 2023-07-26 18:46:41.000000 vipersci-0.9.0/README.rst
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.163195 vipersci-0.9.0/docs/
+-rw-r--r--   0 rbeyer     (503) staff       (20)      609 2021-10-25 21:48:39.000000 vipersci-0.9.0/docs/Makefile
+-rw-r--r--   0 rbeyer     (503) staff       (20)       28 2021-03-28 21:36:13.000000 vipersci-0.9.0/docs/authors.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)       30 2022-10-06 00:17:46.000000 vipersci-0.9.0/docs/changelog.rst
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     4895 2022-11-01 14:54:30.000000 vipersci-0.9.0/docs/conf.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)       33 2021-03-28 21:36:13.000000 vipersci-0.9.0/docs/contributing.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      307 2022-10-06 00:17:46.000000 vipersci-0.9.0/docs/index.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      716 2022-10-06 00:17:46.000000 vipersci-0.9.0/docs/installation.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      770 2021-10-25 21:48:14.000000 vipersci-0.9.0/docs/make.bat
+-rw-r--r--   0 rbeyer     (503) staff       (20)       61 2022-10-05 23:23:34.000000 vipersci-0.9.0/docs/modules.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)       27 2021-03-28 21:36:13.000000 vipersci-0.9.0/docs/readme.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)       71 2021-10-25 21:48:27.000000 vipersci-0.9.0/docs/usage.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      260 2022-10-05 23:15:23.000000 vipersci-0.9.0/docs/vipersci.pds.data.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      201 2022-10-05 23:15:23.000000 vipersci-0.9.0/docs/vipersci.pds.data.template.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      927 2022-10-05 23:15:23.000000 vipersci-0.9.0/docs/vipersci.pds.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      511 2022-10-05 23:23:34.000000 vipersci-0.9.0/docs/vipersci.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      465 2022-10-05 23:15:23.000000 vipersci-0.9.0/docs/vipersci.vis.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      356 2023-05-05 04:04:23.000000 vipersci-0.9.0/pyproject.toml
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3070 2024-04-10 21:25:25.281942 vipersci-0.9.0/setup.cfg
+-rw-r--r--   0 rbeyer     (503) staff       (20)       86 2022-11-08 00:15:45.000000 vipersci-0.9.0/setup.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.134917 vipersci-0.9.0/src/
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.168346 vipersci-0.9.0/src/vipersci/
+-rw-r--r--   0 rbeyer     (503) staff       (20)      130 2024-04-10 21:24:13.000000 vipersci-0.9.0/src/vipersci/__init__.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.190219 vipersci-0.9.0/src/vipersci/carto/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-11-14 18:58:15.000000 vipersci-0.9.0/src/vipersci/carto/__init__.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     3731 2023-04-11 20:22:14.000000 vipersci-0.9.0/src/vipersci/carto/accrual.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3454 2023-03-01 16:59:24.000000 vipersci-0.9.0/src/vipersci/carto/bounds.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)    12418 2024-02-07 01:56:52.000000 vipersci-0.9.0/src/vipersci/carto/colorforge.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     3718 2022-11-10 16:51:53.000000 vipersci-0.9.0/src/vipersci/carto/dice_buffer.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     2325 2022-11-10 16:51:53.000000 vipersci-0.9.0/src/vipersci/carto/dissolve_dice.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3463 2023-03-01 16:59:24.000000 vipersci-0.9.0/src/vipersci/carto/dotmap.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     6244 2024-04-10 21:24:13.000000 vipersci-0.9.0/src/vipersci/carto/get_position.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    20383 2023-07-26 18:42:09.000000 vipersci-0.9.0/src/vipersci/carto/heatmap.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     5959 2022-11-10 16:51:53.000000 vipersci-0.9.0/src/vipersci/carto/msolo_simulator.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     6644 2022-11-10 16:51:53.000000 vipersci-0.9.0/src/vipersci/carto/nirvss_simulator.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     3061 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/carto/nss_modeler.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     7540 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/carto/nss_simulator.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.191502 vipersci-0.9.0/src/vipersci/carto/pds/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2023-04-23 00:01:47.000000 vipersci-0.9.0/src/vipersci/carto/pds/__init__.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.192206 vipersci-0.9.0/src/vipersci/carto/pds/data/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2023-04-23 00:03:38.000000 vipersci-0.9.0/src/vipersci/carto/pds/data/__init__.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     3733 2024-02-07 01:56:52.000000 vipersci-0.9.0/src/vipersci/carto/traverse_interpolator.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)    11429 2024-04-01 23:27:57.000000 vipersci-0.9.0/src/vipersci/carto/tri2gpkg.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1434 2022-11-01 14:54:30.000000 vipersci-0.9.0/src/vipersci/msolo.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1382 2022-11-01 14:54:30.000000 vipersci-0.9.0/src/vipersci/nirvss.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    10898 2023-06-06 20:26:52.000000 vipersci-0.9.0/src/vipersci/nss.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.197425 vipersci-0.9.0/src/vipersci/pds/
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2035 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/pds/__init__.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     5234 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/pds/bundle_install.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     2901 2023-10-27 17:08:28.000000 vipersci-0.9.0/src/vipersci/pds/datetime.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.203800 vipersci-0.9.0/src/vipersci/pds/labelmaker/
+-rw-r--r--   0 rbeyer     (503) staff       (20)     9858 2024-02-07 01:56:52.000000 vipersci-0.9.0/src/vipersci/pds/labelmaker/__init__.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     4267 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/pds/labelmaker/bundle.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1755 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/pds/labelmaker/cli.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     4747 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/pds/labelmaker/collection.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1975 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/pds/labelmaker/generic.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2290 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/pds/labelmaker/inventory.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)    16452 2024-02-21 21:07:21.000000 vipersci-0.9.0/src/vipersci/pds/pid.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     2030 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/pds/xml.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2566 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/util.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.214445 vipersci-0.9.0/src/vipersci/vis/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.9.0/src/vipersci/vis/__init__.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     5421 2023-10-05 22:33:13.000000 vipersci-0.9.0/src/vipersci/vis/anaglyph.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2537 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/vis/anom_pixel.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    12800 2024-02-21 03:54:05.000000 vipersci-0.9.0/src/vipersci/vis/create_image.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     7817 2024-04-10 21:24:13.000000 vipersci-0.9.0/src/vipersci/vis/create_mmgis_pano.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11737 2024-01-31 17:28:33.000000 vipersci-0.9.0/src/vipersci/vis/create_pano.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2031 2023-08-09 00:22:12.000000 vipersci-0.9.0/src/vipersci/vis/create_tif.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.229392 vipersci-0.9.0/src/vipersci/vis/db/
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1093 2023-07-26 18:42:09.000000 vipersci-0.9.0/src/vipersci/vis/db/__init__.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     5674 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/vis/db/create_vis_dbs.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    29400 2024-04-10 21:24:13.000000 vipersci-0.9.0/src/vipersci/vis/db/image_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    10446 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/vis/db/image_requests.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1888 2023-08-09 00:22:12.000000 vipersci-0.9.0/src/vipersci/vis/db/image_stats.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2148 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/vis/db/image_tags.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1877 2023-10-24 18:52:44.000000 vipersci-0.9.0/src/vipersci/vis/db/junc_image_pano.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2045 2023-09-21 04:19:35.000000 vipersci-0.9.0/src/vipersci/vis/db/junc_image_record_tags.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2704 2023-10-24 18:52:44.000000 vipersci-0.9.0/src/vipersci/vis/db/junc_image_req_ldst.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1680 2023-09-23 17:38:22.000000 vipersci-0.9.0/src/vipersci/vis/db/ldst.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3752 2023-10-24 18:52:44.000000 vipersci-0.9.0/src/vipersci/vis/db/light_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     9404 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/vis/db/pano_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3291 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/vis/db/ptu_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1951 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/vis/db/validators.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3192 2023-08-09 00:22:12.000000 vipersci-0.9.0/src/vipersci/vis/header.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     4322 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/vis/image_statistics.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     9073 2024-04-10 21:24:13.000000 vipersci-0.9.0/src/vipersci/vis/pano_check.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.233506 vipersci-0.9.0/src/vipersci/vis/pds/
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2701 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/vis/pds/__init__.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     5178 2024-02-07 01:56:52.000000 vipersci-0.9.0/src/vipersci/vis/pds/create_browse.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     7341 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/vis/pds/create_pano_product.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    12865 2024-04-10 21:24:13.000000 vipersci-0.9.0/src/vipersci/vis/pds/create_raw.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.234269 vipersci-0.9.0/src/vipersci/vis/pds/data/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.9.0/src/vipersci/vis/pds/data/__init__.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     5342 2024-01-26 00:56:09.000000 vipersci-0.9.0/src/vipersci/vis/viseer.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.278923 vipersci-0.9.0/src/vipersci.egg-info/
+-rw-r--r--   0 rbeyer     (503) staff       (20)    17421 2024-04-10 21:25:24.000000 vipersci-0.9.0/src/vipersci.egg-info/PKG-INFO
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3897 2024-04-10 21:25:25.000000 vipersci-0.9.0/src/vipersci.egg-info/SOURCES.txt
+-rw-r--r--   0 rbeyer     (503) staff       (20)        1 2024-04-10 21:25:24.000000 vipersci-0.9.0/src/vipersci.egg-info/dependency_links.txt
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1344 2024-04-10 21:25:24.000000 vipersci-0.9.0/src/vipersci.egg-info/entry_points.txt
+-rw-r--r--   0 rbeyer     (503) staff       (20)        1 2024-04-10 21:25:24.000000 vipersci-0.9.0/src/vipersci.egg-info/not-zip-safe
+-rw-r--r--   0 rbeyer     (503) staff       (20)      121 2024-04-10 21:25:24.000000 vipersci-0.9.0/src/vipersci.egg-info/requires.txt
+-rw-r--r--   0 rbeyer     (503) staff       (20)        9 2024-04-10 21:25:24.000000 vipersci-0.9.0/src/vipersci.egg-info/top_level.txt
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 21:25:25.277656 vipersci-0.9.0/tests/
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     2301 2023-08-09 00:22:12.000000 vipersci-0.9.0/tests/datetime_sqlite.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     6112 2023-09-06 15:17:57.000000 vipersci-0.9.0/tests/test_anaglyph.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1682 2022-11-30 20:55:10.000000 vipersci-0.9.0/tests/test_area_bin.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    14596 2024-04-10 21:24:13.000000 vipersci-0.9.0/tests/test_bundle_install.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11820 2023-05-05 04:04:23.000000 vipersci-0.9.0/tests/test_colorforge.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11937 2024-02-21 21:07:21.000000 vipersci-0.9.0/tests/test_create_image.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     5015 2024-04-10 21:24:13.000000 vipersci-0.9.0/tests/test_create_mmgis_pano.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     9001 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_create_pano.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     8441 2024-02-21 21:07:21.000000 vipersci-0.9.0/tests/test_create_pano_product.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     6123 2024-02-21 21:07:21.000000 vipersci-0.9.0/tests/test_create_raw.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1636 2023-08-09 00:22:12.000000 vipersci-0.9.0/tests/test_create_tif.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2848 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_create_vis_dbs.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1644 2022-11-30 20:55:10.000000 vipersci-0.9.0/tests/test_datetime.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     8388 2023-07-26 18:42:09.000000 vipersci-0.9.0/tests/test_density_heatmap.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3895 2023-02-24 03:28:58.000000 vipersci-0.9.0/tests/test_dotmap.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2526 2023-02-24 03:28:58.000000 vipersci-0.9.0/tests/test_heatmap_helpers.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    22535 2024-04-10 21:24:13.000000 vipersci-0.9.0/tests/test_image_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3835 2023-09-23 17:38:22.000000 vipersci-0.9.0/tests/test_image_requests.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2602 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_image_statistics.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1300 2023-08-09 00:22:12.000000 vipersci-0.9.0/tests/test_image_stats.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1192 2023-09-21 04:19:35.000000 vipersci-0.9.0/tests/test_image_tags.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11202 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_labelmaker.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     5619 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_labelmaker_bundle.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)      571 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_labelmaker_cli.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     6289 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_labelmaker_collection.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1588 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_labelmaker_generic.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1549 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_labelmaker_inventory.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1773 2023-10-24 18:52:44.000000 vipersci-0.9.0/tests/test_light_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1646 2022-11-01 14:54:30.000000 vipersci-0.9.0/tests/test_msolo.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2278 2023-02-24 03:28:58.000000 vipersci-0.9.0/tests/test_msolo_simulator.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1649 2022-11-01 14:54:30.000000 vipersci-0.9.0/tests/test_nirvss.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2387 2023-02-24 03:28:58.000000 vipersci-0.9.0/tests/test_nirvss_simulator.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3737 2022-11-01 14:54:30.000000 vipersci-0.9.0/tests/test_nss.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1782 2022-11-30 20:55:10.000000 vipersci-0.9.0/tests/test_nss_modeler.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2727 2022-11-30 20:55:10.000000 vipersci-0.9.0/tests/test_nss_simulator.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     4591 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_pano_check.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3807 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_pano_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    13805 2024-02-21 21:07:21.000000 vipersci-0.9.0/tests/test_pid.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1589 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_util.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2333 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_validators.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2588 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_vis_pds.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2826 2024-01-26 00:56:09.000000 vipersci-0.9.0/tests/test_xml.py
```

### Comparing `vipersci-0.8.0/AUTHORS.rst` & `vipersci-0.9.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/CHANGELOG.rst` & `vipersci-0.9.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,35 @@
 underlined with dashes under Unreleased_ with the version number
 and the release date, in year-month-day format (see examples below).
 
 
 Unreleased
 ----------
 
+0.9.0 (2024-04-08)
+------------------
+
+Added
+^^^^^
+- get_position.py - Now has support for http basic auth and can now handle returns
+  from the REST service that could be either a sequence of elements or a single
+  element.
+- create_raw.py - Updated to accommodate the icer_minloss and icer_byte_quota properties
+  of an ImageRecord.
+- image_records.py - Added properties for the new image_nickname and waypoint_id
+  properties, and updated the concept of capture_id to be a combination of the
+  waypoint_id and the locally unique_capture_id, instead of a combination of the
+  locally unique_capture_id and the image_request_id.
+
+Fixed
+^^^^^
+- pano_check.py - removed a redundant argument.
+- create_mmgis_pano.py - outpaths for saving the pano and thumbnail were being
+  incorrectly generated.
+
 
 0.8.0 (2024-02-21)
 ------------------
 
 Changed
 ^^^^^^^
 - The instrument_name() function in pid.py now can deal with alias names that are
```

### Comparing `vipersci-0.8.0/CONTRIBUTING.rst` & `vipersci-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/LICENSE` & `vipersci-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/PKG-INFO` & `vipersci-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vipersci
-Version: 0.8.0
+Version: 0.9.0
 Summary: The VIPER Science package is software to support the activities of the Volatiles Investigating Polar Exploration Rover (VIPER) Science Team.
 Home-page: https://github.com/NeoGeographyToolkit/vipersci
 Author: vipersci Developers
 Author-email: Ross.A.Beyer@nasa.gov
 License: Apache 2
 Keywords: VIPER
 Classifier: Programming Language :: Python :: 3.7
@@ -150,14 +150,35 @@
 underlined with dashes under Unreleased_ with the version number
 and the release date, in year-month-day format (see examples below).
 
 
 Unreleased
 ----------
 
+0.9.0 (2024-04-08)
+------------------
+
+Added
+^^^^^
+- get_position.py - Now has support for http basic auth and can now handle returns
+  from the REST service that could be either a sequence of elements or a single
+  element.
+- create_raw.py - Updated to accommodate the icer_minloss and icer_byte_quota properties
+  of an ImageRecord.
+- image_records.py - Added properties for the new image_nickname and waypoint_id
+  properties, and updated the concept of capture_id to be a combination of the
+  waypoint_id and the locally unique_capture_id, instead of a combination of the
+  locally unique_capture_id and the image_request_id.
+
+Fixed
+^^^^^
+- pano_check.py - removed a redundant argument.
+- create_mmgis_pano.py - outpaths for saving the pano and thumbnail were being
+  incorrectly generated.
+
 
 0.8.0 (2024-02-21)
 ------------------
 
 Changed
 ^^^^^^^
 - The instrument_name() function in pid.py now can deal with alias names that are
```

### Comparing `vipersci-0.8.0/README.rst` & `vipersci-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/docs/Makefile` & `vipersci-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/docs/conf.py` & `vipersci-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/docs/installation.rst` & `vipersci-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/docs/make.bat` & `vipersci-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/docs/vipersci.pds.rst` & `vipersci-0.9.0/docs/vipersci.pds.rst`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/setup.cfg` & `vipersci-0.9.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.0
+current_version = 0.9.0
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
 	{major}.{minor}.{patch}
```

### Comparing `vipersci-0.8.0/src/vipersci/carto/accrual.py` & `vipersci-0.9.0/src/vipersci/carto/accrual.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/carto/bounds.py` & `vipersci-0.9.0/src/vipersci/carto/bounds.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/carto/colorforge.py` & `vipersci-0.9.0/src/vipersci/carto/colorforge.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/carto/dice_buffer.py` & `vipersci-0.9.0/src/vipersci/carto/dice_buffer.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/carto/dissolve_dice.py` & `vipersci-0.9.0/src/vipersci/carto/dissolve_dice.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/carto/dotmap.py` & `vipersci-0.9.0/src/vipersci/carto/dotmap.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/carto/get_position.py` & `vipersci-0.9.0/src/vipersci/carto/get_position.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,35 +21,40 @@
 #
 # Reuse is permitted under the terms of the license.
 # The AUTHORS file and the LICENSE file are at the
 # top level of this library.
 
 import argparse
 import csv
+from collections.abc import Sequence
 from datetime import datetime, timezone
+import getpass
 import logging
 from pathlib import Path
 import sys
 
+import http.client as http_client
+
 import pandas as pd
 import requests
+from requests.auth import HTTPBasicAuth
 
 from vipersci import util
 
 logger = logging.getLogger(__name__)
 
 
 def arg_parser():
     parser = argparse.ArgumentParser(
         description=__doc__, parents=[util.parent_parser()]
     )
     parser.add_argument(
         "-s",
         "--start",
-        default=datetime(2020, 1, 1, tz=timezone.utc),
+        default=datetime(2020, 1, 1, tzinfo=timezone.utc),
         help="An ISO8601 datetime to start the query at.",
     )
     parser.add_argument(
         "-e",
         "--end",
         default=datetime.now(tz=timezone.utc),
         help="An ISO8601 datetime to end the query at.",
@@ -64,39 +69,59 @@
     parser.add_argument(
         "-u",
         "--url",
         required=True,
         help="URL to which event_times may be posted and for which location and "
         "orientation will be returned.",
     )
+    parser.add_argument("--user", help="Username to authenticate to URL with.")
+    parser.add_argument(
+        "-p",
+        "--password",
+        action="store_true",
+        help="If given will trigger asking for a password.",
+    )
     parser.add_argument(
         "-o", "--output", type=Path, help="Output path for CSV file output."
     )
     return parser
 
 
 def main():
     parser = arg_parser()
     args = parser.parse_args()
     util.set_logger(args.verbose)
 
+    if args.verbose >= 2:
+        http_client.HTTPConnection.debuglevel = 1
+
+    basic_auth = None
+    if args.password:
+        if args.user:
+            username = args.user
+        else:
+            username = getpass.getuser()
+
+        print(f"For username {username}")
+        basic_auth = HTTPBasicAuth(username, getpass.getpass())
+
     t_start = datetime.fromisoformat(args.start)
     t_end = datetime.fromisoformat(args.end)
 
     if args.frequency:
         times = pd.date_range(t_start, t_end, freq=args.frequency).tolist()
 
         unix_times = []
         for t in times:
             unix_times.append(t.timestamp())
 
-        tpp = get_position_and_pose(unix_times, args.url)
+        tpp = get_position_and_pose(unix_times, args.url, auth=basic_auth)
     else:
         tpp = get_position_and_pose_range(
-            t_start.timestamp(), t_end.timestamp(), args.url
+            t_start.timestamp(), t_end.timestamp(), args.url, auth=basic_auth
         )
 
     if args.output is not None:
         with open(args.output, "w", newline="") as csvfile:
             writer = csv.writer(csvfile)
             writer.writerow(["UTC datetime", "x", "y", "yaw"])
             for row in tpp:
@@ -105,15 +130,15 @@
                     [
                         dt.isoformat(),
                     ]
                     + list(row[1:])
                 )
 
 
-def get_position_and_pose(times: list, url: str, crs: str = "VIPER:910101"):
+def get_position_and_pose(times: list, url: str, crs: str = "VIPER:910101", auth=None):
     """
     Given a list of unix times and a URL that requests can be made against,
     return a list of two-tuples whose first element is the time and
     whose second element is a three-tuple of x-location, y-location,
     and yaw.
     """
 
@@ -129,27 +154,29 @@
                 "format": "xyyaw",  # Could also be xyyaw_uncertainty
                 "time_format": "unix_seconds",
                 "source": "ROVER",
                 "limit": 0,
                 "crs_code": crs,
             },
             verify=False,
+            auth=auth,
         )
+        logger.debug(position_result)
         rj = position_result.json()
         logger.info(rj)
 
         tpp.append(
-            (rj["event_seconds"], (rj["location"][0], rj["location"][1], rj["yaw"]))
+            (rj["event_seconds"], rj["location"][0], rj["location"][1], rj["yaw"])
         )
 
     return tpp
 
 
 def get_position_and_pose_range(
-    start_time, stop_time, url: str, crs: str = "VIPER:910101"
+    start_time, stop_time, url: str, crs: str = "VIPER:910101", auth=None
 ):
     tpp = list()
 
     track_result = requests.get(
         url,
         params={
             "min_time": start_time,
@@ -160,18 +187,26 @@
             "time_format": "unix_seconds",
             "source": "ROVER",
             "start_end_only": False,
             "simplify": False,
             "order": "asc",
         },
         verify=False,
+        auth=auth,
     )
+    logger.debug(track_result)
     rj = track_result.json()
+    logger.info(rj)
 
-    for time, loc, yaw in zip(rj["event_seconds"], rj["location"], rj["yaw"]):
-        tpp.append((time, loc[0], loc[1], yaw))
+    if isinstance(rj["event_seconds"], Sequence):
+        for time, loc, yaw in zip(rj["event_seconds"], rj["location"], rj["yaw"]):
+            tpp.append((time, loc[0], loc[1], yaw))
+    else:
+        tpp.append(
+            (rj["event_seconds"], rj["location"][0], rj["location"][1], rj["yaw"])
+        )
 
     return tpp
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `vipersci-0.8.0/src/vipersci/carto/heatmap.py` & `vipersci-0.9.0/src/vipersci/carto/heatmap.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/carto/msolo_simulator.py` & `vipersci-0.9.0/src/vipersci/carto/msolo_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/carto/nirvss_simulator.py` & `vipersci-0.9.0/src/vipersci/carto/nirvss_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/carto/nss_modeler.py` & `vipersci-0.9.0/src/vipersci/carto/nss_modeler.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/carto/nss_simulator.py` & `vipersci-0.9.0/src/vipersci/carto/nss_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/carto/traverse_interpolator.py` & `vipersci-0.9.0/src/vipersci/carto/traverse_interpolator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/carto/tri2gpkg.py` & `vipersci-0.9.0/src/vipersci/carto/tri2gpkg.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/msolo.py` & `vipersci-0.9.0/src/vipersci/msolo.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/nirvss.py` & `vipersci-0.9.0/src/vipersci/nirvss.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/nss.py` & `vipersci-0.9.0/src/vipersci/nss.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/pds/__init__.py` & `vipersci-0.9.0/src/vipersci/pds/__init__.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/pds/bundle_install.py` & `vipersci-0.9.0/src/vipersci/pds/bundle_install.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/pds/datetime.py` & `vipersci-0.9.0/src/vipersci/pds/datetime.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/pds/labelmaker/__init__.py` & `vipersci-0.9.0/src/vipersci/pds/labelmaker/__init__.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/pds/labelmaker/bundle.py` & `vipersci-0.9.0/src/vipersci/pds/labelmaker/bundle.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/pds/labelmaker/cli.py` & `vipersci-0.9.0/src/vipersci/pds/labelmaker/cli.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/pds/labelmaker/collection.py` & `vipersci-0.9.0/src/vipersci/pds/labelmaker/collection.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/pds/labelmaker/generic.py` & `vipersci-0.9.0/src/vipersci/pds/labelmaker/generic.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/pds/labelmaker/inventory.py` & `vipersci-0.9.0/src/vipersci/pds/labelmaker/inventory.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/pds/pid.py` & `vipersci-0.9.0/src/vipersci/pds/pid.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/pds/xml.py` & `vipersci-0.9.0/src/vipersci/pds/xml.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/util.py` & `vipersci-0.9.0/src/vipersci/util.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/anaglyph.py` & `vipersci-0.9.0/src/vipersci/vis/anaglyph.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/anom_pixel.py` & `vipersci-0.9.0/src/vipersci/vis/anom_pixel.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/create_image.py` & `vipersci-0.9.0/src/vipersci/vis/create_image.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/create_mmgis_pano.py` & `vipersci-0.9.0/src/vipersci/vis/create_mmgis_pano.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,56 +177,59 @@
 
     # Convert to PNG
     image = equalize_adapthist(imread(str(source_path)))
     image8 = rescale_intensity(image, in_range="image", out_range="uint8").astype(
         "uint8"
     )
 
-    outpath = outdir / longname(source_path).with_suffix(".png").name
+    outpath = outdir / Path(longname(source_path)).with_suffix(".png").name
 
     imsave(str(outpath), image8, check_contrast=False)
 
     d = mmgis_data(pano, yaw)
     # Decided not to include the URL key in the JSON this program outputs
     # as the process that takes these data and publishes them are what
     # should set that.
     # d["url"] = "not/sure/what/the/path/should/be/to/" + outpath.name
 
     # Make JPG thumbnail
     if thumbsize is not None:
-        if isinstance(int, thumbsize):
+        if isinstance(thumbsize, int):
             max_dim = max(np.shape(image8))
             if max_dim > thumbsize:
                 scale = max_dim / thumbsize
                 new_shape = tuple(int(x / scale) for x in np.shape(image8))
         elif len(thumbsize) == 2:
             if thumbsize[0] is not None:
                 raise ValueError(
                     "Not sure how to handle a non-None first element for thumbsize."
                 )
             scale = np.shape(image8)[1] / thumbsize[1]
             new_shape = tuple(int(x / scale) for x in np.shape(image8))
 
         image8 = rescale_intensity(
-            resize(image8, new_shape), in_range="image8", out_range="uint8"
+            resize(image8, new_shape), in_range="image", out_range="uint8"
         )
-        outthumb = outpath.with_suffix("") + "_thumb.jpeg"
+        outthumb = outpath.with_name(outpath.stem + "_thumb.jpeg")
         imsave(outthumb, image8, check_contrast=False)
 
     with open(outpath.stem + ".json", "w") as f:
         json.dump(d, f, indent=2, sort_keys=True)
 
     return
 
 
 def longname(path):
     """Returns a longer iso8601-esque filename."""
     # YYYY-MM-DDTHH-mm-ss.SSS-pan
     vid = pds.PanoID(path.name)
-    return vid.date.isoformat() + "T" + vid.time.isformat().replace(":", "-") + "-pan"
+    vdt = vid.datetime()
+    return (
+        vdt.date().isoformat() + "T" + vdt.time().isoformat().replace(":", "-") + "-pan"
+    )
 
 
 def mmgis_data(pano_data: dict, yaw=0.0):
     d = {
         "azmax": yaw + pano_data["rover_pan_max"],
         "azmin": yaw + pano_data["rover_pan_min"],
         "columns": pano_data["samples"],
```

### Comparing `vipersci-0.8.0/src/vipersci/vis/create_pano.py` & `vipersci-0.9.0/src/vipersci/vis/create_pano.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/create_tif.py` & `vipersci-0.9.0/src/vipersci/vis/create_tif.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/__init__.py` & `vipersci-0.9.0/src/vipersci/vis/db/__init__.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/create_vis_dbs.py` & `vipersci-0.9.0/src/vipersci/vis/db/create_vis_dbs.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/image_records.py` & `vipersci-0.9.0/src/vipersci/vis/db/image_records.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,21 @@
     )
     image_id = mapped_column(
         Integer,
         nullable=False,
         doc="The IMG_ID from the MCSE Image Header used for CCU storage and "
         "retrieval.",
     )
+    image_nickname = mapped_column(
+        String,
+        nullable=True,
+        doc="This was designed to be a unique nickname for the waypoint+camera. It has "
+        "the form: <camera>-<waypoint>-<index>, where the index is represented as "
+        "letters A, B, C, ..., Z, AA, AB, ...",
+    )
     # This image_request_id column and image_request relationship allow a many
     # ImageRecords to one ImageRequest relationship, and the nullable allows it to be
     # optional.  So an ImageRecord may be connected to an ImageRequest, but it may not.
     image_request_id = mapped_column(ForeignKey("image_requests.id"), nullable=True)
     image_request = relationship("ImageRequest", back_populates="image_records")
 
     # The image_tags and image_tag_associations allow a many ImageTag to many
@@ -175,14 +182,15 @@
         viewonly=True,
     )
     image_tag_associations = relationship(
         "JuncImageRecordTag", back_populates="image_record"
     )
     imageHeight = synonym("lines")
     imageId = synonym("image_id")
+    imageNickname = synonym("image_nickname")
     imageWidth = synonym("samples")
     instrument_name = mapped_column(
         String, nullable=False, doc="The full name of the instrument."
     )
     instrument_temperature = mapped_column(
         Float,
         nullable=False,
@@ -262,14 +270,15 @@
         Integer,
         nullable=False,
         doc="The processingInfo parameter from the Yamcs imageHeader. This integer "
         "value must correspond to a valid value of ProcessingStage, and indicates "
         "what onboard processing occurred.",
     )
     processingInfo = synonym("processing_info")
+    requestId = synonym("image_request_id")
     samples = mapped_column(
         Integer,
         nullable=False,
         doc="The imageWidth parameter from the Yamcs imageHeader.",
     )
     # slog = mapped_column(
     #     Boolean,
@@ -284,14 +293,22 @@
         Boolean,
         nullable=False,
         doc="The stereo parameter from the Yamcs imageHeader.",
         # TODO: learn more about stereo to provide better doc here.
     )
     stop_time = mapped_column(DateTime(timezone=True), nullable=False)
     temperature = synonym("instrument_temperature")
+    unique_capture_id = mapped_column(
+        Integer,
+        nullable=True,
+        doc="The unique portion from the lower 16 bits of the captureId.  Ironically, "
+        "this isn't guaranteed to be a mission-long globally unique value, only "
+        "locally unique in time.  It gets set and linearly increases, but can "
+        "be reset to zero.",
+    )
     verification_notes = mapped_column(
         String,
         nullable=True,
         doc="Any notes about the verification of this image by the VIS Operator.",
     )
     verification_purpose = mapped_column(
         Enum(Purpose), nullable=True, doc="Purpose of Observation, as defined by PDS."
@@ -310,14 +327,19 @@
     )
     voltage_ramp = mapped_column(
         Integer,
         nullable=False,
         doc="The VOLTAGE_RAMP parameter from the MCSE Image Header.",
     )
     voltageRamp = synonym("voltage_ramp")
+    waypoint_id = mapped_column(
+        Integer,
+        nullable=True,
+        doc="The waypoint id extracted from the upper 16 bits of the captureId.",
+    )
     yamcs_generation_time = mapped_column(
         DateTime(timezone=True),
         nullable=False,
         doc="The generation time of the source record from Yamcs.",
     )
     yamcs_name = mapped_column(
         String,
@@ -545,15 +567,16 @@
             )
 
         self._pid = str(pid)
 
         if self.capture_id is not None and self.capture_id > int(
             "1111111111111111", base=2
         ):  # 65535
-            self.image_request_id = int(bin(self.capture_id)[-16:], base=2)
+            self.waypoint_id = int(bin(self.capture_id)[:-16], base=2)
+            self.unique_capture_id = int(bin(self.capture_id)[-16:], base=2)
 
         # Is this really a good idea?  Not sure.  This instance variable plus
         # label_dict() and update() allow other key/value pairs to be carried around
         # in this object, which is handy.  If these are well enough known, perhaps
         # they should just be pre-defined properties and not left to chance?
         self.labelmeta = otherargs
```

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/image_requests.py` & `vipersci-0.9.0/src/vipersci/vis/db/image_requests.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/image_stats.py` & `vipersci-0.9.0/src/vipersci/vis/db/image_stats.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/image_tags.py` & `vipersci-0.9.0/src/vipersci/vis/db/image_tags.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/junc_image_pano.py` & `vipersci-0.9.0/src/vipersci/vis/db/junc_image_pano.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/junc_image_record_tags.py` & `vipersci-0.9.0/src/vipersci/vis/db/junc_image_record_tags.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/junc_image_req_ldst.py` & `vipersci-0.9.0/src/vipersci/vis/db/junc_image_req_ldst.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/ldst.py` & `vipersci-0.9.0/src/vipersci/vis/db/ldst.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/light_records.py` & `vipersci-0.9.0/src/vipersci/vis/db/light_records.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/pano_records.py` & `vipersci-0.9.0/src/vipersci/vis/db/pano_records.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/ptu_records.py` & `vipersci-0.9.0/src/vipersci/vis/db/ptu_records.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/db/validators.py` & `vipersci-0.9.0/src/vipersci/vis/db/validators.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/header.py` & `vipersci-0.9.0/src/vipersci/vis/header.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/image_statistics.py` & `vipersci-0.9.0/src/vipersci/vis/image_statistics.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/pano_check.py` & `vipersci-0.9.0/src/vipersci/vis/pano_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,20 +56,14 @@
         "-d",
         "--dburl",
         help="Database with an image_records table to read from. "
         "If not given, no database will be written to.  Example: "
         "postgresql://postgres:NotTheDefault@localhost/visdb",
     )
     parser.add_argument(
-        "-m",
-        "--mapserver",
-        help="URL that will respond to requests when given an event_time and "
-        "a crs_code.",
-    )
-    parser.add_argument(
         "-s",
         "--since",
         default=0,
         help="An ISO8601 datetime after which should be searched for images "
         "in the database.",
     )
     parser.add_argument(
```

### Comparing `vipersci-0.8.0/src/vipersci/vis/pds/__init__.py` & `vipersci-0.9.0/src/vipersci/vis/pds/__init__.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/pds/create_browse.py` & `vipersci-0.9.0/src/vipersci/vis/pds/create_browse.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/pds/create_pano_product.py` & `vipersci-0.9.0/src/vipersci/vis/pds/create_pano_product.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci/vis/pds/create_raw.py` & `vipersci-0.9.0/src/vipersci/vis/pds/create_raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,17 +304,16 @@
         inst_lid=f"{lids['instrument']}",
         gain_number=(ir.adc_gain * ir.pga_gain),
         exposure_type="Auto" if ir.auto_exposure else "Manual",
         image_filters="",
         led_wavelength=453,  # nm
         luminaires={},
         compression_class=pid.compression_class(),
-        minloss=0 if pid.compression_class() == "Lossless" else 12,
         observational_intent={},
-        onboard_compression_ratio=pds.vis_compression[pid.compression],
+        onboard_compression_ratio=ir.icer_byte_quota / (2048 * 2048 * 2),
         onboard_compression_type="ICER",
         sample_bits=12,
         sample_bit_mask="2#0000111111111111",
     )
     for k, v in lights.items():
         d["luminaires"][k] = onoff[v]
```

### Comparing `vipersci-0.8.0/src/vipersci/vis/viseer.py` & `vipersci-0.9.0/src/vipersci/vis/viseer.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/src/vipersci.egg-info/PKG-INFO` & `vipersci-0.9.0/src/vipersci.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vipersci
-Version: 0.8.0
+Version: 0.9.0
 Summary: The VIPER Science package is software to support the activities of the Volatiles Investigating Polar Exploration Rover (VIPER) Science Team.
 Home-page: https://github.com/NeoGeographyToolkit/vipersci
 Author: vipersci Developers
 Author-email: Ross.A.Beyer@nasa.gov
 License: Apache 2
 Keywords: VIPER
 Classifier: Programming Language :: Python :: 3.7
@@ -150,14 +150,35 @@
 underlined with dashes under Unreleased_ with the version number
 and the release date, in year-month-day format (see examples below).
 
 
 Unreleased
 ----------
 
+0.9.0 (2024-04-08)
+------------------
+
+Added
+^^^^^
+- get_position.py - Now has support for http basic auth and can now handle returns
+  from the REST service that could be either a sequence of elements or a single
+  element.
+- create_raw.py - Updated to accommodate the icer_minloss and icer_byte_quota properties
+  of an ImageRecord.
+- image_records.py - Added properties for the new image_nickname and waypoint_id
+  properties, and updated the concept of capture_id to be a combination of the
+  waypoint_id and the locally unique_capture_id, instead of a combination of the
+  locally unique_capture_id and the image_request_id.
+
+Fixed
+^^^^^
+- pano_check.py - removed a redundant argument.
+- create_mmgis_pano.py - outpaths for saving the pano and thumbnail were being
+  incorrectly generated.
+
 
 0.8.0 (2024-02-21)
 ------------------
 
 Changed
 ^^^^^^^
 - The instrument_name() function in pid.py now can deal with alias names that are
```

### Comparing `vipersci-0.8.0/src/vipersci.egg-info/SOURCES.txt` & `vipersci-0.9.0/src/vipersci.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,18 @@
 src/vipersci/vis/pds/create_browse.py
 src/vipersci/vis/pds/create_pano_product.py
 src/vipersci/vis/pds/create_raw.py
 src/vipersci/vis/pds/data/__init__.py
 tests/datetime_sqlite.py
 tests/test_anaglyph.py
 tests/test_area_bin.py
+tests/test_bundle_install.py
 tests/test_colorforge.py
 tests/test_create_image.py
+tests/test_create_mmgis_pano.py
 tests/test_create_pano.py
 tests/test_create_pano_product.py
 tests/test_create_raw.py
 tests/test_create_tif.py
 tests/test_create_vis_dbs.py
 tests/test_datetime.py
 tests/test_density_heatmap.py
```

### Comparing `vipersci-0.8.0/src/vipersci.egg-info/entry_points.txt` & `vipersci-0.9.0/src/vipersci.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/datetime_sqlite.py` & `vipersci-0.9.0/tests/datetime_sqlite.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_anaglyph.py` & `vipersci-0.9.0/tests/test_anaglyph.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_area_bin.py` & `vipersci-0.9.0/tests/test_area_bin.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_colorforge.py` & `vipersci-0.9.0/tests/test_colorforge.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_create_image.py` & `vipersci-0.9.0/tests/test_create_image.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_create_pano.py` & `vipersci-0.9.0/tests/test_create_pano.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_create_pano_product.py` & `vipersci-0.9.0/tests/test_create_pano_product.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_create_raw.py` & `vipersci-0.9.0/tests/test_create_raw.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_create_tif.py` & `vipersci-0.9.0/tests/test_create_tif.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_create_vis_dbs.py` & `vipersci-0.9.0/tests/test_create_vis_dbs.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_datetime.py` & `vipersci-0.9.0/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_density_heatmap.py` & `vipersci-0.9.0/tests/test_density_heatmap.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_dotmap.py` & `vipersci-0.9.0/tests/test_dotmap.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_heatmap_helpers.py` & `vipersci-0.9.0/tests/test_heatmap_helpers.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_image_records.py` & `vipersci-0.9.0/tests/test_image_records.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,16 @@
         d.update(self.extras)
         rpl = trp.ImageRecord(**d)
         self.assertEqual("220127-000000-ncl-c", str(rpl.product_id))
 
         d = self.d.copy()
         d["capture_id"] = 65537
         ir_ci = trp.ImageRecord(**d)
-        self.assertEqual(1, ir_ci.image_request_id)
+        self.assertEqual(1, ir_ci.waypoint_id)
+        self.assertEqual(1, ir_ci.unique_capture_id)
 
     def test_init_slog(self):
         d_slog = {
             "adcGain": 0,
             "autoExposure": 0,
             "cameraId": 0,
             "captureId": 1,
```

### Comparing `vipersci-0.8.0/tests/test_image_requests.py` & `vipersci-0.9.0/tests/test_image_requests.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_image_statistics.py` & `vipersci-0.9.0/tests/test_image_statistics.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_image_stats.py` & `vipersci-0.9.0/tests/test_image_stats.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_image_tags.py` & `vipersci-0.9.0/tests/test_image_tags.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_labelmaker.py` & `vipersci-0.9.0/tests/test_labelmaker.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_labelmaker_bundle.py` & `vipersci-0.9.0/tests/test_labelmaker_bundle.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_labelmaker_cli.py` & `vipersci-0.9.0/tests/test_labelmaker_cli.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_labelmaker_collection.py` & `vipersci-0.9.0/tests/test_labelmaker_collection.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_labelmaker_generic.py` & `vipersci-0.9.0/tests/test_labelmaker_generic.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_labelmaker_inventory.py` & `vipersci-0.9.0/tests/test_labelmaker_inventory.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_light_records.py` & `vipersci-0.9.0/tests/test_light_records.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_msolo.py` & `vipersci-0.9.0/tests/test_msolo.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_msolo_simulator.py` & `vipersci-0.9.0/tests/test_msolo_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_nirvss.py` & `vipersci-0.9.0/tests/test_nirvss.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_nirvss_simulator.py` & `vipersci-0.9.0/tests/test_nirvss_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_nss.py` & `vipersci-0.9.0/tests/test_nss.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_nss_modeler.py` & `vipersci-0.9.0/tests/test_nss_modeler.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_nss_simulator.py` & `vipersci-0.9.0/tests/test_nss_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_pano_check.py` & `vipersci-0.9.0/tests/test_pano_check.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_pano_records.py` & `vipersci-0.9.0/tests/test_pano_records.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_pid.py` & `vipersci-0.9.0/tests/test_pid.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_util.py` & `vipersci-0.9.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_validators.py` & `vipersci-0.9.0/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_vis_pds.py` & `vipersci-0.9.0/tests/test_vis_pds.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.8.0/tests/test_xml.py` & `vipersci-0.9.0/tests/test_xml.py`

 * *Files identical despite different names*

