# Comparing `tmp/dissect.volume-3.9.tar.gz` & `tmp/dissect.volume-3.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.volume-3.9.tar", last modified: Thu Mar  7 15:23:40 2024, max compression
+gzip compressed data, was "dissect.volume-3.9.dev1.tar", last modified: Wed Jan 31 14:21:28 2024, max compression
```

## Comparing `dissect.volume-3.9.tar` & `dissect.volume-3.9.dev1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.804804 dissect.volume-3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-03-07 15:23:31.000000 dissect.volume-3.9/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-07 15:23:31.000000 dissect.volume-3.9/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-07 15:23:31.000000 dissect.volume-3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-07 15:23:31.000000 dissect.volume-3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-03-07 15:23:40.800804 dissect.volume-3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-07 15:23:31.000000 dissect.volume-3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.776804 dissect.volume-3.9/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.780804 dissect.volume-3.9/dissect/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.780804 dissect.volume-3.9/dissect/volume/ddf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/ddf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/ddf/c_ddf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/ddf/ddf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.780804 dissect.volume-3.9/dissect/volume/disk/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/disk/disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/disk/partition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.784804 dissect.volume-3.9/dissect/volume/disk/schemes/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/disk/schemes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/disk/schemes/apm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16101 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/disk/schemes/bsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/disk/schemes/gpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/disk/schemes/mbr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.784804 dissect.volume-3.9/dissect/volume/dm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/dm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/dm/btree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/dm/c_dm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/dm/thin.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/ldm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.784804 dissect.volume-3.9/dissect/volume/lvm/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/lvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/lvm/c_lvm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/lvm/lvm2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16491 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/lvm/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/lvm/physical.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.784804 dissect.volume-3.9/dissect/volume/md/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/md/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/md/c_md.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/md/md.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.784804 dissect.volume-3.9/dissect/volume/raid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/raid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/raid/raid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15836 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/raid/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    21549 2024-03-07 15:23:31.000000 dissect.volume-3.9/dissect/volume/vss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.800804 dissect.volume-3.9/dissect.volume.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-03-07 15:23:40.000000 dissect.volume-3.9/dissect.volume.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-03-07 15:23:40.000000 dissect.volume-3.9/dissect.volume.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 15:23:40.000000 dissect.volume-3.9/dissect.volume.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-07 15:23:40.000000 dissect.volume-3.9/dissect.volume.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-07 15:23:40.000000 dissect.volume-3.9/dissect.volume.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-07 15:23:31.000000 dissect.volume-3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 15:23:40.804804 dissect.volume-3.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.788804 dissect.volume-3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.792804 dissect.volume-3.9/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/apm.bin
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/bsd.bin
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/bsd64.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.796804 dissect.volume-3.9/tests/data/ddf/
--rw-r--r--   0 runner    (1001) docker     (127)    46699 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid0-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    46703 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid0-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    44381 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid0-3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    43948 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid0-raid1-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    43945 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid0-raid1-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    43314 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid1-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    43318 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid1-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42891 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid10-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42895 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid10-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42899 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid10-3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42899 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid10-4.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    43327 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid4-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    43327 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid4-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42616 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid5-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42870 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid5-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42612 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid5-3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42707 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid6-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42928 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid6-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42674 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid6-3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42997 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/ddf/ddf-raid6-4.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.796804 dissect.volume-3.9/tests/data/dm/
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/dm/dm-thin-data.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/dm/dm-thin-metadata.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/gpt.bin
--rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/gpt_4k.bin
--rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/gpt_esxi.bin
--rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/gpt_hybrid.bin
--rw-r--r--   0 runner    (1001) docker     (127)    17920 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/gpt_no_name_xff.bin
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/lvm-mirror-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/lvm-mirror-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    24933 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/lvm-thin.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/lvm.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/mbr.bin
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.800804 dissect.volume-3.9/tests/data/md/
--rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-90-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-90-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-90-raid1-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-90-raid1-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-linear-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-linear-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid0-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid0-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid0-3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid1-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid1-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid10-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid10-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid4-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid4-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid4-3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid5-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid5-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid5-3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid6-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid6-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid6-3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/data/md/md-raid6-4.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:23:40.800804 dissect.volume-3.9/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/test_apm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/test_bsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/test_ddf.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/test_dm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/test_gpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/test_lvm.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/test_mbr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-03-07 15:23:31.000000 dissect.volume-3.9/tests/test_md.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-07 15:23:31.000000 dissect.volume-3.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.425190 dissect.volume-3.9.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-01-31 14:21:28.425190 dissect.volume-3.9.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.393190 dissect.volume-3.9.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.401190 dissect.volume-3.9.dev1/dissect/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.401190 dissect.volume-3.9.dev1/dissect/volume/ddf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/ddf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/ddf/c_ddf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/ddf/ddf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.401190 dissect.volume-3.9.dev1/dissect/volume/disk/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/disk/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/disk/partition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.401190 dissect.volume-3.9.dev1/dissect/volume/disk/schemes/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/disk/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/disk/schemes/apm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16101 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/disk/schemes/bsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/disk/schemes/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/disk/schemes/mbr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.405190 dissect.volume-3.9.dev1/dissect/volume/dm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/dm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/dm/btree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/dm/c_dm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/dm/thin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/ldm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.405190 dissect.volume-3.9.dev1/dissect/volume/lvm/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/lvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/lvm/c_lvm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/lvm/lvm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16491 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/lvm/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/lvm/physical.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.405190 dissect.volume-3.9.dev1/dissect/volume/md/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/md/c_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/md/md.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.405190 dissect.volume-3.9.dev1/dissect/volume/raid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/raid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/raid/raid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15836 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/raid/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21549 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/dissect/volume/vss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.421190 dissect.volume-3.9.dev1/dissect.volume.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-01-31 14:21:28.000000 dissect.volume-3.9.dev1/dissect.volume.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-01-31 14:21:28.000000 dissect.volume-3.9.dev1/dissect.volume.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 14:21:28.000000 dissect.volume-3.9.dev1/dissect.volume.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-31 14:21:28.000000 dissect.volume-3.9.dev1/dissect.volume.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-31 14:21:28.000000 dissect.volume-3.9.dev1/dissect.volume.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-01-31 14:21:19.000000 dissect.volume-3.9.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 14:21:28.425190 dissect.volume-3.9.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.409190 dissect.volume-3.9.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.409190 dissect.volume-3.9.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/apm.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/bsd.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/bsd64.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.417190 dissect.volume-3.9.dev1/tests/data/ddf/
+-rw-r--r--   0 runner    (1001) docker     (127)    46699 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid0-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    46703 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid0-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    44381 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid0-3.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    43948 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid0-raid1-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    43945 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid0-raid1-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    43314 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid1-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    43318 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid1-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42891 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid10-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42895 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid10-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42899 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid10-3.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42899 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid10-4.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    43327 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid4-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    43327 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid4-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42616 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid5-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42870 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid5-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42612 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid5-3.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42707 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid6-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42928 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid6-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42674 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid6-3.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42997 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid6-4.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.417190 dissect.volume-3.9.dev1/tests/data/dm/
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/dm/dm-thin-data.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/dm/dm-thin-metadata.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/gpt.bin
+-rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/gpt_4k.bin
+-rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/gpt_esxi.bin
+-rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/gpt_hybrid.bin
+-rw-r--r--   0 runner    (1001) docker     (127)    17920 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/gpt_no_name_xff.bin
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/lvm-mirror-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/lvm-mirror-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    24933 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/lvm-thin.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/lvm.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/mbr.bin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.421190 dissect.volume-3.9.dev1/tests/data/md/
+-rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-90-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-90-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-90-raid1-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-90-raid1-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-linear-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-linear-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid0-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid0-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid0-3.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid1-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid1-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid10-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid10-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid4-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid4-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid4-3.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid5-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid5-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid5-3.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid6-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid6-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid6-3.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/data/md/md-raid6-4.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:28.421190 dissect.volume-3.9.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/test_apm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/test_bsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/test_ddf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/test_dm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/test_gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/test_lvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/test_mbr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tests/test_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-01-31 14:21:16.000000 dissect.volume-3.9.dev1/tox.ini
```

### Comparing `dissect.volume-3.9/.gitattributes` & `dissect.volume-3.9.dev1/.gitattributes`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/LICENSE` & `dissect.volume-3.9.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/PKG-INFO` & `dissect.volume-3.9.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.volume
-Version: 3.9
+Version: 3.9.dev1
 Summary: A Dissect module implementing a parser for different disk volume and partition systems, for example LVM2, GPT and MBR
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.volume
 Project-URL: repository, https://github.com/fox-it/dissect.volume
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.volume-3.9/README.md` & `dissect.volume-3.9.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/ddf/c_ddf.py` & `dissect.volume-3.9.dev1/dissect/volume/ddf/c_ddf.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/ddf/ddf.py` & `dissect.volume-3.9.dev1/dissect/volume/ddf/ddf.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/disk/disk.py` & `dissect.volume-3.9.dev1/dissect/volume/disk/disk.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/disk/partition.py` & `dissect.volume-3.9.dev1/dissect/volume/disk/partition.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/disk/schemes/apm.py` & `dissect.volume-3.9.dev1/dissect/volume/disk/schemes/apm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/disk/schemes/bsd.py` & `dissect.volume-3.9.dev1/dissect/volume/disk/schemes/bsd.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/disk/schemes/gpt.py` & `dissect.volume-3.9.dev1/dissect/volume/disk/schemes/gpt.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/disk/schemes/mbr.py` & `dissect.volume-3.9.dev1/dissect/volume/disk/schemes/mbr.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/dm/btree.py` & `dissect.volume-3.9.dev1/dissect/volume/dm/btree.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/dm/c_dm.py` & `dissect.volume-3.9.dev1/dissect/volume/dm/c_dm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/dm/thin.py` & `dissect.volume-3.9.dev1/dissect/volume/dm/thin.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/ldm.py` & `dissect.volume-3.9.dev1/dissect/volume/ldm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/lvm/c_lvm2.py` & `dissect.volume-3.9.dev1/dissect/volume/lvm/c_lvm2.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/lvm/lvm2.py` & `dissect.volume-3.9.dev1/dissect/volume/lvm/lvm2.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/lvm/metadata.py` & `dissect.volume-3.9.dev1/dissect/volume/lvm/metadata.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/lvm/physical.py` & `dissect.volume-3.9.dev1/dissect/volume/lvm/physical.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/md/c_md.py` & `dissect.volume-3.9.dev1/dissect/volume/md/c_md.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/md/md.py` & `dissect.volume-3.9.dev1/dissect/volume/md/md.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/raid/raid.py` & `dissect.volume-3.9.dev1/dissect/volume/raid/raid.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/raid/stream.py` & `dissect.volume-3.9.dev1/dissect/volume/raid/stream.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect/volume/vss.py` & `dissect.volume-3.9.dev1/dissect/volume/vss.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/dissect.volume.egg-info/PKG-INFO` & `dissect.volume-3.9.dev1/dissect.volume.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.volume
-Version: 3.9
+Version: 3.9.dev1
 Summary: A Dissect module implementing a parser for different disk volume and partition systems, for example LVM2, GPT and MBR
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.volume
 Project-URL: repository, https://github.com/fox-it/dissect.volume
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.volume-3.9/dissect.volume.egg-info/SOURCES.txt` & `dissect.volume-3.9.dev1/dissect.volume.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/pyproject.toml` & `dissect.volume-3.9.dev1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -46,7 +46,8 @@
 [tool.setuptools]
 license-files = ["LICENSE", "COPYRIGHT"]
 
 [tool.setuptools.packages.find]
 include = ["dissect.*"]
 
 [tool.setuptools_scm]
+local_scheme = "no-local-version"
```

### Comparing `dissect.volume-3.9/tests/conftest.py` & `dissect.volume-3.9.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/apm.bin` & `dissect.volume-3.9.dev1/tests/data/apm.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/bsd.bin` & `dissect.volume-3.9.dev1/tests/data/bsd.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/bsd64.bin.gz` & `dissect.volume-3.9.dev1/tests/data/bsd64.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid0-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid0-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid0-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid0-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid0-3.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid0-3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid0-raid1-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid0-raid1-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid0-raid1-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid0-raid1-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid1-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid1-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid1-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid1-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid10-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid10-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid10-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid10-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid10-3.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid10-3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid10-4.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid10-4.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid4-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid4-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid4-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid4-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid5-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid5-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid5-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid5-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid5-3.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid5-3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid6-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid6-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid6-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid6-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid6-3.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid6-3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/ddf/ddf-raid6-4.bin.gz` & `dissect.volume-3.9.dev1/tests/data/ddf/ddf-raid6-4.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/dm/dm-thin-data.bin.gz` & `dissect.volume-3.9.dev1/tests/data/dm/dm-thin-data.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/dm/dm-thin-metadata.bin.gz` & `dissect.volume-3.9.dev1/tests/data/dm/dm-thin-metadata.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/gpt.bin` & `dissect.volume-3.9.dev1/tests/data/gpt.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/gpt_4k.bin` & `dissect.volume-3.9.dev1/tests/data/gpt_4k.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/gpt_esxi.bin` & `dissect.volume-3.9.dev1/tests/data/gpt_esxi.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/gpt_hybrid.bin` & `dissect.volume-3.9.dev1/tests/data/gpt_hybrid.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/gpt_no_name_xff.bin` & `dissect.volume-3.9.dev1/tests/data/gpt_no_name_xff.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/lvm-mirror-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/lvm-mirror-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/lvm-mirror-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/lvm-mirror-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/lvm-thin.bin.gz` & `dissect.volume-3.9.dev1/tests/data/lvm-thin.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/lvm.bin.gz` & `dissect.volume-3.9.dev1/tests/data/lvm.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/mbr.bin` & `dissect.volume-3.9.dev1/tests/data/mbr.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-90-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-90-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-90-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-90-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-90-raid1-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-90-raid1-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-90-raid1-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-90-raid1-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-linear-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-linear-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-linear-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-linear-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid0-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid0-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid0-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid0-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid0-3.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid0-3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid1-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid1-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid1-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid1-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid10-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid10-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid10-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid10-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid4-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid4-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid4-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid4-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid4-3.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid4-3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid5-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid5-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid5-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid5-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid5-3.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid5-3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid6-1.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid6-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid6-2.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid6-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid6-3.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid6-3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/data/md/md-raid6-4.bin.gz` & `dissect.volume-3.9.dev1/tests/data/md/md-raid6-4.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/docs/Makefile` & `dissect.volume-3.9.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/docs/conf.py` & `dissect.volume-3.9.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/test_apm.py` & `dissect.volume-3.9.dev1/tests/test_apm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/test_bsd.py` & `dissect.volume-3.9.dev1/tests/test_bsd.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/test_ddf.py` & `dissect.volume-3.9.dev1/tests/test_ddf.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/test_dm.py` & `dissect.volume-3.9.dev1/tests/test_dm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/test_gpt.py` & `dissect.volume-3.9.dev1/tests/test_gpt.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/test_lvm.py` & `dissect.volume-3.9.dev1/tests/test_lvm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/test_mbr.py` & `dissect.volume-3.9.dev1/tests/test_mbr.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tests/test_md.py` & `dissect.volume-3.9.dev1/tests/test_md.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.9/tox.ini` & `dissect.volume-3.9.dev1/tox.ini`

 * *Files identical despite different names*

