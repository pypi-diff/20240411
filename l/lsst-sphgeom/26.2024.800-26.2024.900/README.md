# Comparing `tmp/lsst-sphgeom-26.2024.800.tar.gz` & `tmp/lsst-sphgeom-26.2024.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-sphgeom-26.2024.800.tar", last modified: Thu Feb 22 10:43:17 2024, max compression
+gzip compressed data, was "lsst-sphgeom-26.2024.900.tar", last modified: Thu Feb 29 10:20:52 2024, max compression
```

## Comparing `lsst-sphgeom-26.2024.800.tar` & `lsst-sphgeom-26.2024.900.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:17.432690 lsst-sphgeom-26.2024.800/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-02-22 10:43:17.432690 lsst-sphgeom-26.2024.800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/bsd_license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/gpl-v3.0.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:17.404690 lsst-sphgeom-26.2024.800/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:17.404690 lsst-sphgeom-26.2024.800/include/lsst/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:17.416690 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Angle.h
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/AngleInterval.h
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/BigInteger.h
--rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Box.h
--rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Box3d.h
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Chunker.h
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Circle.h
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/CompoundRegion.h
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/ConvexPolygon.h
--rw-r--r--   0 runner    (1001) docker     (127)    12953 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Ellipse.h
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/HtmPixelization.h
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Interval.h
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Interval1d.h
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/LonLat.h
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Matrix3d.h
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Mq3cPixelization.h
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/NormalizedAngle.h
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/NormalizedAngleInterval.h
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Pixelization.h
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Q3cPixelization.h
--rw-r--r--   0 runner    (1001) docker     (127)    22374 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/RangeSet.h
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Region.h
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Relationship.h
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/UnitVector3d.h
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Vector3d.h
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/codec.h
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/constants.h
--rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/curve.h
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/orientation.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:17.416690 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/python/
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/python/interval.h
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/python/relationship.h
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/python/utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/python.h
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/include/lsst/sphgeom/utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:17.408690 lsst-sphgeom-26.2024.800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:17.416690 lsst-sphgeom-26.2024.800/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:17.420690 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_angle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_angleInterval.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_box.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_box3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_chunker.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_circle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_compoundRegion.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_convexPolygon.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_curve.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_ellipse.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_healpixPixelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_htmPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_interval1d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_lonLat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_matrix3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_mq3cPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_normalizedAngle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_normalizedAngleInterval.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_orientation.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_pixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_q3cPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_rangeSet.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_region.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_relationship.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_sphgeom.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_unitVector3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_vector3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/pixelization_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 10:43:17.000000 lsst-sphgeom-26.2024.800/python/lsst/sphgeom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:17.432690 lsst-sphgeom-26.2024.800/python/lsst_sphgeom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-02-22 10:43:17.000000 lsst-sphgeom-26.2024.800/python/lsst_sphgeom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-02-22 10:43:17.000000 lsst-sphgeom-26.2024.800/python/lsst_sphgeom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:43:17.000000 lsst-sphgeom-26.2024.800/python/lsst_sphgeom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:43:16.000000 lsst-sphgeom-26.2024.800/python/lsst_sphgeom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-22 10:43:17.000000 lsst-sphgeom-26.2024.800/python/lsst_sphgeom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 10:43:17.000000 lsst-sphgeom-26.2024.800/python/lsst_sphgeom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-22 10:43:17.432690 lsst-sphgeom-26.2024.800/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:17.428690 lsst-sphgeom-26.2024.800/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/Angle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/AngleInterval.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9495 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/BigInteger.cc
--rw-r--r--   0 runner    (1001) docker     (127)    19939 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/Box.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/Box3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/Chunker.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/Circle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/CompoundRegion.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/ConvexPolygon.cc
--rw-r--r--   0 runner    (1001) docker     (127)    16322 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/ConvexPolygonImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/Ellipse.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/HtmPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/Interval1d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/LonLat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/Matrix3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/Mq3cPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/NormalizedAngle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/NormalizedAngleInterval.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/PixelFinder.h
--rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/Q3cPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/Q3cPixelizationImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/RangeSet.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/Region.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/UnitVector3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/Vector3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/orientation.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/src/utils.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:17.432690 lsst-sphgeom-26.2024.800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_Angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_AngleIntervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_Box.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_Box3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_Chunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_Circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_CompoundRegion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_ConvexPolygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_Ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_HealpixPixelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_HtmPixelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_Interval1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_LonLat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_Matrix3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_Mq3cPixelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_NormalizedAngle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_Q3cPixelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_RangeSet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_UnitVector3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-02-22 10:42:59.000000 lsst-sphgeom-26.2024.800/tests/test_Vector3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:52.458335 lsst-sphgeom-26.2024.900/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-02-29 10:20:52.454336 lsst-sphgeom-26.2024.900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/bsd_license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/gpl-v3.0.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:52.434336 lsst-sphgeom-26.2024.900/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:52.434336 lsst-sphgeom-26.2024.900/include/lsst/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:52.442336 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Angle.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/AngleInterval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/BigInteger.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Box.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Box3d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Chunker.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Circle.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/CompoundRegion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/ConvexPolygon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12953 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Ellipse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/HtmPixelization.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Interval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Interval1d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/LonLat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Matrix3d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Mq3cPixelization.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/NormalizedAngle.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/NormalizedAngleInterval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Pixelization.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Q3cPixelization.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22374 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/RangeSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Region.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Relationship.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/UnitVector3d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Vector3d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/codec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/curve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/orientation.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:52.442336 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/python/interval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/python/relationship.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/python/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/python.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/include/lsst/sphgeom/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:52.434336 lsst-sphgeom-26.2024.900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:52.442336 lsst-sphgeom-26.2024.900/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:52.446336 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_angle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_angleInterval.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_box.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_box3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_chunker.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_circle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_compoundRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_convexPolygon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_curve.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_ellipse.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_healpixPixelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_htmPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_interval1d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_lonLat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_matrix3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_mq3cPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_normalizedAngle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_normalizedAngleInterval.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_orientation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_pixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_q3cPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_rangeSet.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_region.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_relationship.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_sphgeom.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_unitVector3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_vector3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/pixelization_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:52.000000 lsst-sphgeom-26.2024.900/python/lsst/sphgeom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:52.454336 lsst-sphgeom-26.2024.900/python/lsst_sphgeom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-02-29 10:20:52.000000 lsst-sphgeom-26.2024.900/python/lsst_sphgeom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-02-29 10:20:52.000000 lsst-sphgeom-26.2024.900/python/lsst_sphgeom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:52.000000 lsst-sphgeom-26.2024.900/python/lsst_sphgeom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:51.000000 lsst-sphgeom-26.2024.900/python/lsst_sphgeom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-29 10:20:52.000000 lsst-sphgeom-26.2024.900/python/lsst_sphgeom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:20:52.000000 lsst-sphgeom-26.2024.900/python/lsst_sphgeom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-29 10:20:52.458335 lsst-sphgeom-26.2024.900/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:52.454336 lsst-sphgeom-26.2024.900/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/Angle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/AngleInterval.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9495 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/BigInteger.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    19939 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/Box.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/Box3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/Chunker.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/Circle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/CompoundRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/ConvexPolygon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    16322 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/ConvexPolygonImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/Ellipse.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/HtmPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/Interval1d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/LonLat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/Matrix3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/Mq3cPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/NormalizedAngle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/NormalizedAngleInterval.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/PixelFinder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/Q3cPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/Q3cPixelizationImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/RangeSet.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/Region.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/UnitVector3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/Vector3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/orientation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/src/utils.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:52.454336 lsst-sphgeom-26.2024.900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_Angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_AngleIntervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_Box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_Box3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_Chunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_Circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_CompoundRegion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_ConvexPolygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_Ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_HealpixPixelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_HtmPixelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_Interval1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_LonLat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_Matrix3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_Mq3cPixelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_NormalizedAngle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_Q3cPixelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_RangeSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_UnitVector3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-02-29 10:20:36.000000 lsst-sphgeom-26.2024.900/tests/test_Vector3d.py
```

### Comparing `lsst-sphgeom-26.2024.800/PKG-INFO` & `lsst-sphgeom-26.2024.900/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-sphgeom
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: A spherical geometry library.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/sphgeom
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-sphgeom-26.2024.800/README.md` & `lsst-sphgeom-26.2024.900/README.md`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/bsd_license.txt` & `lsst-sphgeom-26.2024.900/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/gpl-v3.0.txt` & `lsst-sphgeom-26.2024.900/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Angle.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Angle.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/AngleInterval.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/AngleInterval.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/BigInteger.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/BigInteger.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Box.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Box.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Box3d.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Box3d.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Chunker.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Chunker.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Circle.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Circle.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/CompoundRegion.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/CompoundRegion.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/ConvexPolygon.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/ConvexPolygon.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Ellipse.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Ellipse.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/HtmPixelization.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/HtmPixelization.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Interval.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Interval.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Interval1d.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Interval1d.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/LonLat.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/LonLat.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Matrix3d.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Matrix3d.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Mq3cPixelization.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Mq3cPixelization.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/NormalizedAngle.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/NormalizedAngle.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/NormalizedAngleInterval.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/NormalizedAngleInterval.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Pixelization.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Pixelization.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Q3cPixelization.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Q3cPixelization.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/RangeSet.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/RangeSet.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Region.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Region.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Relationship.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Relationship.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/UnitVector3d.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/UnitVector3d.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/Vector3d.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/Vector3d.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/codec.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/codec.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/constants.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/constants.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/curve.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/curve.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/orientation.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/orientation.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/python/interval.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/python/interval.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/python/relationship.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/python/relationship.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/python/utils.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/python/utils.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/python.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/python.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/include/lsst/sphgeom/utils.h` & `lsst-sphgeom-26.2024.900/include/lsst/sphgeom/utils.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/pyproject.toml` & `lsst-sphgeom-26.2024.900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/__init__.py` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_angle.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_angle.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_angleInterval.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_angleInterval.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_box.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_box.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_box3d.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_box3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_chunker.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_chunker.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_circle.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_circle.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_compoundRegion.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_compoundRegion.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_convexPolygon.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_convexPolygon.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_curve.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_curve.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_ellipse.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_ellipse.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_healpixPixelization.py` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_healpixPixelization.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_htmPixelization.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_htmPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_interval1d.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_interval1d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_lonLat.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_lonLat.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_matrix3d.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_matrix3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_mq3cPixelization.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_mq3cPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_normalizedAngle.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_normalizedAngle.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_normalizedAngleInterval.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_normalizedAngleInterval.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_orientation.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_orientation.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_pixelization.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_pixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_q3cPixelization.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_q3cPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_rangeSet.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_rangeSet.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_region.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_region.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_relationship.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_relationship.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_sphgeom.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_sphgeom.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_unitVector3d.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_unitVector3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_utils.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_utils.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_vector3d.cc` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_vector3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/_yaml.py` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/_yaml.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst/sphgeom/pixelization_abc.py` & `lsst-sphgeom-26.2024.900/python/lsst/sphgeom/pixelization_abc.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/python/lsst_sphgeom.egg-info/PKG-INFO` & `lsst-sphgeom-26.2024.900/python/lsst_sphgeom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-sphgeom
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: A spherical geometry library.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/sphgeom
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-sphgeom-26.2024.800/python/lsst_sphgeom.egg-info/SOURCES.txt` & `lsst-sphgeom-26.2024.900/python/lsst_sphgeom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/setup.py` & `lsst-sphgeom-26.2024.900/setup.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/Angle.cc` & `lsst-sphgeom-26.2024.900/src/Angle.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/AngleInterval.cc` & `lsst-sphgeom-26.2024.900/src/AngleInterval.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/BigInteger.cc` & `lsst-sphgeom-26.2024.900/src/BigInteger.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/Box.cc` & `lsst-sphgeom-26.2024.900/src/Box.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/Box3d.cc` & `lsst-sphgeom-26.2024.900/src/Box3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/Chunker.cc` & `lsst-sphgeom-26.2024.900/src/Chunker.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/Circle.cc` & `lsst-sphgeom-26.2024.900/src/Circle.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/CompoundRegion.cc` & `lsst-sphgeom-26.2024.900/src/CompoundRegion.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/ConvexPolygon.cc` & `lsst-sphgeom-26.2024.900/src/ConvexPolygon.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/ConvexPolygonImpl.h` & `lsst-sphgeom-26.2024.900/src/ConvexPolygonImpl.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/Ellipse.cc` & `lsst-sphgeom-26.2024.900/src/Ellipse.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/HtmPixelization.cc` & `lsst-sphgeom-26.2024.900/src/HtmPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/Interval1d.cc` & `lsst-sphgeom-26.2024.900/src/Interval1d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/LonLat.cc` & `lsst-sphgeom-26.2024.900/src/LonLat.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/Matrix3d.cc` & `lsst-sphgeom-26.2024.900/src/Matrix3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/Mq3cPixelization.cc` & `lsst-sphgeom-26.2024.900/src/Mq3cPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/NormalizedAngle.cc` & `lsst-sphgeom-26.2024.900/src/NormalizedAngle.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/NormalizedAngleInterval.cc` & `lsst-sphgeom-26.2024.900/src/NormalizedAngleInterval.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/PixelFinder.h` & `lsst-sphgeom-26.2024.900/src/PixelFinder.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/Q3cPixelization.cc` & `lsst-sphgeom-26.2024.900/src/Q3cPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/Q3cPixelizationImpl.h` & `lsst-sphgeom-26.2024.900/src/Q3cPixelizationImpl.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/RangeSet.cc` & `lsst-sphgeom-26.2024.900/src/RangeSet.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/Region.cc` & `lsst-sphgeom-26.2024.900/src/Region.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/UnitVector3d.cc` & `lsst-sphgeom-26.2024.900/src/UnitVector3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/Vector3d.cc` & `lsst-sphgeom-26.2024.900/src/Vector3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/orientation.cc` & `lsst-sphgeom-26.2024.900/src/orientation.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/src/utils.cc` & `lsst-sphgeom-26.2024.900/src/utils.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_Angle.py` & `lsst-sphgeom-26.2024.900/tests/test_Angle.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_AngleIntervals.py` & `lsst-sphgeom-26.2024.900/tests/test_AngleIntervals.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_Box.py` & `lsst-sphgeom-26.2024.900/tests/test_Box.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_Box3d.py` & `lsst-sphgeom-26.2024.900/tests/test_Box3d.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_Chunker.py` & `lsst-sphgeom-26.2024.900/tests/test_Chunker.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_Circle.py` & `lsst-sphgeom-26.2024.900/tests/test_Circle.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_CompoundRegion.py` & `lsst-sphgeom-26.2024.900/tests/test_CompoundRegion.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_ConvexPolygon.py` & `lsst-sphgeom-26.2024.900/tests/test_ConvexPolygon.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_Ellipse.py` & `lsst-sphgeom-26.2024.900/tests/test_Ellipse.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_HealpixPixelization.py` & `lsst-sphgeom-26.2024.900/tests/test_HealpixPixelization.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_HtmPixelization.py` & `lsst-sphgeom-26.2024.900/tests/test_HtmPixelization.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_Interval1d.py` & `lsst-sphgeom-26.2024.900/tests/test_Interval1d.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_LonLat.py` & `lsst-sphgeom-26.2024.900/tests/test_LonLat.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_Matrix3d.py` & `lsst-sphgeom-26.2024.900/tests/test_Matrix3d.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_Mq3cPixelization.py` & `lsst-sphgeom-26.2024.900/tests/test_Mq3cPixelization.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_NormalizedAngle.py` & `lsst-sphgeom-26.2024.900/tests/test_NormalizedAngle.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_Q3cPixelization.py` & `lsst-sphgeom-26.2024.900/tests/test_Q3cPixelization.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_RangeSet.py` & `lsst-sphgeom-26.2024.900/tests/test_RangeSet.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_UnitVector3d.py` & `lsst-sphgeom-26.2024.900/tests/test_UnitVector3d.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.2024.800/tests/test_Vector3d.py` & `lsst-sphgeom-26.2024.900/tests/test_Vector3d.py`

 * *Files identical despite different names*

