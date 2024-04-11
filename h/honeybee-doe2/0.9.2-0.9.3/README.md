# Comparing `tmp/honeybee-doe2-0.9.2.tar.gz` & `tmp/honeybee-doe2-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-doe2-0.9.2.tar", last modified: Tue Aug 29 19:29:48 2023, max compression
+gzip compressed data, was "dist/honeybee-doe2-0.9.3.tar", last modified: Thu Sep  7 19:24:04 2023, max compression
```

## Comparing `honeybee-doe2-0.9.2.tar` & `honeybee-doe2-0.9.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (999)      279 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (999)      445 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (999)    34523 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      172 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     1499 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      921 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (999)      262 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/honeybee_doe2/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       43 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)       74 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)      297 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/_base.py
--rw-r--r--   0 runner    (1001) docker     (999)     1771 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/_extend_honeybee_doe2.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/honeybee_doe2/cli/
--rw-r--r--   0 runner    (1001) docker     (999)      316 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1234 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/cli/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/honeybee_doe2/geometry/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2938 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/geometry/polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1856 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/adiabaticfloor.py
--rw-r--r--   0 runner    (1001) docker     (999)     1930 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/adiabaticroof.py
--rw-r--r--   0 runner    (1001) docker     (999)     1787 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/aperture.py
--rw-r--r--   0 runner    (1001) docker     (999)     3871 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/constructions.py
--rw-r--r--   0 runner    (1001) docker     (999)     1739 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/door.py
--rw-r--r--   0 runner    (1001) docker     (999)     1736 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/exposedfloor.py
--rw-r--r--   0 runner    (1001) docker     (999)      790 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/face.py
--rw-r--r--   0 runner    (1001) docker     (999)     1578 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/groundcontact.py
--rw-r--r--   0 runner    (1001) docker     (999)     2610 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/hvac.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/inputils/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/inputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     7307 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/inputils/blocks.py
--rw-r--r--   0 runner    (1001) docker     (999)     1247 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/inputils/compliance.py
--rw-r--r--   0 runner    (1001) docker     (999)     1437 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/inputils/glass_types.py
--rw-r--r--   0 runner    (1001) docker     (999)     1382 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/inputils/run_period.py
--rw-r--r--   0 runner    (1001) docker     (999)      852 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/inputils/sitebldg.py
--rw-r--r--   0 runner    (1001) docker     (999)      369 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/inputils/title.py
--rw-r--r--   0 runner    (1001) docker     (999)     1793 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/interiorfloor.py
--rw-r--r--   0 runner    (1001) docker     (999)     4307 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/materials.py
--rw-r--r--   0 runner    (1001) docker     (999)     3855 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (999)     1643 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/roof.py
--rw-r--r--   0 runner    (1001) docker     (999)     6428 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/room.py
--rw-r--r--   0 runner    (1001) docker     (999)     3773 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/shades.py
--rw-r--r--   0 runner    (1001) docker     (999)     3774 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/story.py
--rw-r--r--   0 runner    (1001) docker     (999)     3265 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/properties/wall.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/honeybee_doe2/utils/
--rw-r--r--   0 runner    (1001) docker     (999)       19 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2719 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/utils/doe_formatters.py
--rw-r--r--   0 runner    (1001) docker     (999)      116 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (999)     5807 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/honeybee_doe2/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/honeybee_doe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     1499 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/honeybee_doe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1726 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/honeybee_doe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/honeybee_doe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       57 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/honeybee_doe2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       25 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/honeybee_doe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       14 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/honeybee_doe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       25 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)      102 2023-08-29 19:29:48.000000 honeybee-doe2-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1108 2023-08-29 19:28:50.000000 honeybee-doe2-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/honeybee_doe2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/_extend_honeybee_doe2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/honeybee_doe2/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/cli/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/honeybee_doe2/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/geometry/polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/adiabaticfloor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/adiabaticroof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/constructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/door.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/exposedfloor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/groundcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/hvac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/inputils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/inputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/inputils/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/inputils/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/inputils/glass_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/inputils/run_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/inputils/sitebldg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/inputils/title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/interiorfloor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/roof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/shades.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/story.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/properties/wall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/honeybee_doe2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/utils/doe_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/honeybee_doe2/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/honeybee_doe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/honeybee_doe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/honeybee_doe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/honeybee_doe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/honeybee_doe2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/honeybee_doe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/honeybee_doe2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-09-07 19:24:04.000000 honeybee-doe2-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-09-07 19:22:46.000000 honeybee-doe2-0.9.3/setup.py
```

### Comparing `honeybee-doe2-0.9.2/LICENSE` & `honeybee-doe2-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/PKG-INFO` & `honeybee-doe2-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.9.2
+Version: 0.9.3
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-doe2-0.9.2/README.md` & `honeybee-doe2-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/_extend_honeybee_doe2.py` & `honeybee-doe2-0.9.3/honeybee_doe2/_extend_honeybee_doe2.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/cli/translate.py` & `honeybee-doe2-0.9.3/honeybee_doe2/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/geometry/polygon.py` & `honeybee-doe2-0.9.3/honeybee_doe2/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/adiabaticfloor.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/adiabaticfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/adiabaticroof.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/adiabaticroof.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/aperture.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/constructions.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/constructions.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/door.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/door.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/exposedfloor.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/exposedfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/face.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/groundcontact.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/groundcontact.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/hvac.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/hvac.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/inputils/blocks.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/inputils/blocks.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/inputils/compliance.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/inputils/compliance.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/inputils/glass_types.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/inputils/glass_types.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/inputils/run_period.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/inputils/run_period.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/inputils/sitebldg.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/inputils/sitebldg.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/interiorfloor.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/interiorfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/materials.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/materials.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/model.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/model.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/roof.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/roof.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/room.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/room.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/shades.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/shades.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/story.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/story.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/properties/wall.py` & `honeybee-doe2-0.9.3/honeybee_doe2/properties/wall.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/utils/doe_formatters.py` & `honeybee-doe2-0.9.3/honeybee_doe2/utils/doe_formatters.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2/writer.py` & `honeybee-doe2-0.9.3/honeybee_doe2/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,17 +22,26 @@
     sb_data = sbd()
 
     hb_model = hb_model.duplicate()
 
     if hb_model.units != 'Feet':
         hb_model.convert_to_units(units='Feet')
     hb_model.remove_degenerate_geometry()
-    hb_model.rectangularize_apertures(
-        subdivision_distance=0.5, max_separation=0.0, merge_all=True
-    )
+
+    try:
+        hb_model.rectangularize_apertures(
+            subdivision_distance=0.5, max_separation=0.0, merge_all=True,
+            resolve_adjacency=True
+        )
+    except AssertionError:
+        # try without resolving adjacency that can create errors
+        hb_model.rectangularize_apertures(
+            subdivision_distance=0.5, max_separation=0.0, merge_all=True,
+            resolve_adjacency=False
+        )
 
     room_names = {}
     face_names = {}
     for room in hb_model.rooms:
         room.display_name = clean_string(room.display_name).replace('..', '_')
         room.display_name = short_name(room.display_name)
         if room.display_name in room_names:
```

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2.egg-info/PKG-INFO` & `honeybee-doe2-0.9.3/honeybee_doe2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.9.2
+Version: 0.9.3
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-doe2-0.9.2/honeybee_doe2.egg-info/SOURCES.txt` & `honeybee-doe2-0.9.3/honeybee_doe2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.9.2/setup.py` & `honeybee-doe2-0.9.3/setup.py`

 * *Files identical despite different names*

