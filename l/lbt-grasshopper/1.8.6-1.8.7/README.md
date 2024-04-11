# Comparing `tmp/lbt-grasshopper-1.8.6.tar.gz` & `tmp/lbt-grasshopper-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbt-grasshopper-1.8.6.tar", last modified: Sat Apr  6 05:29:30 2024, max compression
+gzip compressed data, was "dist/lbt-grasshopper-1.8.7.tar", last modified: Thu Apr 11 14:00:33 2024, max compression
```

## Comparing `lbt-grasshopper-1.8.6.tar` & `lbt-grasshopper-1.8.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:29:30.000000 lbt-grasshopper-1.8.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:29:30.000000 lbt-grasshopper-1.8.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:29:30.000000 lbt-grasshopper-1.8.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/CI_STATUS.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-06 05:29:30.000000 lbt-grasshopper-1.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/ci-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)   730519 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/gradients.png
--rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/installer.gh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:29:30.000000 lbt-grasshopper-1.8.6/lbt_grasshopper/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/lbt_grasshopper/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:29:30.000000 lbt-grasshopper-1.8.6/lbt_grasshopper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-06 05:29:30.000000 lbt-grasshopper-1.8.6/lbt_grasshopper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-06 05:29:30.000000 lbt-grasshopper-1.8.6/lbt_grasshopper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 05:29:30.000000 lbt-grasshopper-1.8.6/lbt_grasshopper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-06 05:29:30.000000 lbt-grasshopper-1.8.6/lbt_grasshopper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 05:29:30.000000 lbt-grasshopper-1.8.6/lbt_grasshopper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/pass_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/ruby-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-06 05:29:30.000000 lbt-grasshopper-1.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-06 05:28:28.000000 lbt-grasshopper-1.8.6/uninstaller.gh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:00:33.000000 lbt-grasshopper-1.8.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:00:33.000000 lbt-grasshopper-1.8.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:00:33.000000 lbt-grasshopper-1.8.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/CI_STATUS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-11 14:00:33.000000 lbt-grasshopper-1.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/ci-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   730519 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/gradients.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/installer.gh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:00:33.000000 lbt-grasshopper-1.8.7/lbt_grasshopper/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/lbt_grasshopper/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:00:33.000000 lbt-grasshopper-1.8.7/lbt_grasshopper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-11 14:00:33.000000 lbt-grasshopper-1.8.7/lbt_grasshopper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-11 14:00:33.000000 lbt-grasshopper-1.8.7/lbt_grasshopper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:00:33.000000 lbt-grasshopper-1.8.7/lbt_grasshopper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 14:00:33.000000 lbt-grasshopper-1.8.7/lbt_grasshopper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:00:33.000000 lbt-grasshopper-1.8.7/lbt_grasshopper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/pass_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/ruby-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 14:00:33.000000 lbt-grasshopper-1.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-11 13:59:26.000000 lbt-grasshopper-1.8.7/uninstaller.gh
```

### Comparing `lbt-grasshopper-1.8.6/.github/workflows/ci.yaml` & `lbt-grasshopper-1.8.7/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.6/.github/workflows/dependency-release.yaml` & `lbt-grasshopper-1.8.7/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.6/CI_STATUS.md` & `lbt-grasshopper-1.8.7/CI_STATUS.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 # Ladybug Tools Continuous Integration Status
 
 Status of all repositories that make up the Ladybug Tools SDK.
 
 ### Ladybug Libraries
 
-[![Build Status](https://github.com/ladybug-tools/lbt-ladybug/workflows/CI/badge.svg)](https://github.com/ladybug-tools/lbt-ladybug/actions) lbt-ladybug
+[![Build Status](https://github.com/ladybug-tools/lbt-ladybug/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/lbt-ladybug/actions) lbt-ladybug
 
-[![Build Status](https://github.com/ladybug-tools/ladybug-geometry/workflows/CI/badge.svg)](https://github.com/ladybug-tools/ladybug-geometry/actions) ladybug-geometry
+[![Build Status](https://github.com/ladybug-tools/ladybug-geometry/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/ladybug-geometry/actions) ladybug-geometry
 
-[![Build Status](https://github.com/ladybug-tools/ladybug-geometry-polyskel/workflows/CI/badge.svg)](https://github.com/ladybug-tools/ladybug-geometry-polyskel/actions) ladybug-geometry-polyskel
+[![Build Status](https://github.com/ladybug-tools/ladybug-geometry-polyskel/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/ladybug-geometry-polyskel/actions) ladybug-geometry-polyskel
 
-[![Build Status](https://github.com/ladybug-tools/ladybug/workflows/CI/badge.svg)](https://github.com/ladybug-tools/ladybug/actions) ladybug
+[![Build Status](https://github.com/ladybug-tools/ladybug/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/ladybug/actions) ladybug
 
-[![Build Status](https://github.com/ladybug-tools/ladybug-comfort/workflows/CI/badge.svg)](https://github.com/ladybug-tools/ladybug-comfort/actions) ladybug-comfort
+[![Build Status](https://github.com/ladybug-tools/ladybug-comfort/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/ladybug-comfort/actions) ladybug-comfort
 
-[![Build Status](https://github.com/ladybug-tools/ladybug-radiance/workflows/CI/badge.svg)](https://github.com/ladybug-tools/ladybug-radiance/actions) ladybug-radiance
+[![Build Status](https://github.com/ladybug-tools/ladybug-radiance/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/ladybug-radiance/actions) ladybug-radiance
 
-[![Build Status](https://github.com/ladybug-tools/ladybug-display/workflows/CI/badge.svg)](https://github.com/ladybug-tools/ladybug-display/actions) ladybug-display
+[![Build Status](https://github.com/ladybug-tools/ladybug-display/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/ladybug-display/actions) ladybug-display
 
-[![Build Status](https://github.com/ladybug-tools/ladybug-display-schema/workflows/CI/badge.svg)](https://github.com/ladybug-tools/ladybug-display-schema/actions) ladybug-display-schema
+[![Build Status](https://github.com/ladybug-tools/ladybug-display-schema/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/ladybug-display-schema/actions) ladybug-display-schema
 
 ### Honeybee Libraries
 
-[![Build Status](https://github.com/ladybug-tools/lbt-honeybee/workflows/CI/badge.svg)](https://github.com/ladybug-tools/lbt-honeybee/actions) lbt-honeybee
+[![Build Status](https://github.com/ladybug-tools/lbt-honeybee/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/lbt-honeybee/actions) lbt-honeybee
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-core/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-core/actions) honeybee-core
+[![Build Status](https://github.com/ladybug-tools/honeybee-core/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-core/actions) honeybee-core
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-display/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-display/actions) honeybee-display
+[![Build Status](https://github.com/ladybug-tools/honeybee-display/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-display/actions) honeybee-display
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-energy/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-energy/actions) honeybee-energy
+[![Build Status](https://github.com/ladybug-tools/honeybee-energy/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-energy/actions) honeybee-energy
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-openstudio-gem/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-openstudio-gem/actions) honeybee-openstudio-gem
+[![Build Status](https://github.com/ladybug-tools/honeybee-openstudio-gem/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-openstudio-gem/actions) honeybee-openstudio-gem
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-radiance/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-radiance/actions) honeybee-radiance
+[![Build Status](https://github.com/ladybug-tools/honeybee-radiance/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-radiance/actions) honeybee-radiance
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-radiance-folder/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-radiance-folder/actions) honeybee-radiance-folder
+[![Build Status](https://github.com/ladybug-tools/honeybee-radiance-folder/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-radiance-folder/actions) honeybee-radiance-folder
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-radiance-command/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-radiance-command/actions) honeybee-radiance-command
+[![Build Status](https://github.com/ladybug-tools/honeybee-radiance-command/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-radiance-command/actions) honeybee-radiance-command
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-radiance-postprocess/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-radiance-postprocess/actions) honeybee-radiance-postprocess
+[![Build Status](https://github.com/ladybug-tools/honeybee-radiance-postprocess/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-radiance-postprocess/actions) honeybee-radiance-postprocess
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-schema/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-schema/actions) honeybee-schema
+[![Build Status](https://github.com/ladybug-tools/honeybee-schema/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-schema/actions) honeybee-schema
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-standards/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-standards/actions) honeybee-standards
+[![Build Status](https://github.com/ladybug-tools/honeybee-standards/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-standards/actions) honeybee-standards
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-energy-standards/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-energy-standards/actions) honeybee-energy-standards
+[![Build Status](https://github.com/ladybug-tools/honeybee-energy-standards/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-energy-standards/actions) honeybee-energy-standards
 
 ### Dragonfly Libraries
 
-[![Build Status](https://github.com/ladybug-tools/lbt-dragonfly/workflows/CI/badge.svg)](https://github.com/ladybug-tools/lbt-dragonfly/actions) lbt-dragonfly
+[![Build Status](https://github.com/ladybug-tools/lbt-dragonfly/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/lbt-dragonfly/actions) lbt-dragonfly
 
-[![Build Status](https://github.com/ladybug-tools/dragonfly-core/workflows/CI/badge.svg)](https://github.com/ladybug-tools/dragonfly-core/actions) dragonfly-core
+[![Build Status](https://github.com/ladybug-tools/dragonfly-core/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/dragonfly-core/actions) dragonfly-core
 
-[![Build Status](https://github.com/ladybug-tools/dragonfly-energy/workflows/CI/badge.svg)](https://github.com/ladybug-tools/dragonfly-energy/actions) dragonfly-energy
+[![Build Status](https://github.com/ladybug-tools/dragonfly-energy/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/dragonfly-energy/actions) dragonfly-energy
 
-[![Build Status](https://github.com/ladybug-tools/dragonfly-radiance/workflows/CI/badge.svg)](https://github.com/ladybug-tools/dragonfly-radiance/actions) dragonfly-radiance
+[![Build Status](https://github.com/ladybug-tools/dragonfly-radiance/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/dragonfly-radiance/actions) dragonfly-radiance
 
-[![Build Status](https://github.com/ladybug-tools/dragonfly-uwg/workflows/CI/badge.svg)](https://github.com/ladybug-tools/dragonfly-uwg/actions) dragonfly-uwg
+[![Build Status](https://github.com/ladybug-tools/dragonfly-uwg/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/dragonfly-uwg/actions) dragonfly-uwg
 
-[![Build Status](https://github.com/ladybug-tools/dragonfly-schema/workflows/CI/badge.svg)](https://github.com/ladybug-tools/dragonfly-schema/actions) dragonfly-schema
+[![Build Status](https://github.com/ladybug-tools/dragonfly-schema/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/dragonfly-schema/actions) dragonfly-schema
 
 ### Recipe Libraries
 
-[![Build Status](https://github.com/ladybug-tools/lbt-recipes/workflows/CI/badge.svg)](https://github.com/ladybug-tools/lbt-recipes/actions) lbt-recipes
+[![Build Status](https://github.com/ladybug-tools/lbt-recipes/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/lbt-recipes/actions) lbt-recipes
 
-[![Build Status](https://github.com/pollination/handlers-python/workflows/CI/badge.svg)](https://github.com/pollination/handlers-python/actions) pollination-handlers
+[![Build Status](https://github.com/pollination/handlers-python/actions/workflows/ci.yaml/badge.svg)](https://github.com/pollination/handlers-python/actions) pollination-handlers
 
 ### Rhino/Grasshopper Libraries
 
-[![Build Status](https://github.com/ladybug-tools/lbt-grasshopper/workflows/CI/badge.svg)](https://github.com/ladybug-tools/lbt-grasshopper/actions) lbt-grasshopper
+[![Build Status](https://github.com/ladybug-tools/lbt-grasshopper/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/lbt-grasshopper/actions) lbt-grasshopper
 
-[![Build Status](https://github.com/ladybug-tools/ladybug-rhino/workflows/CI/badge.svg)](https://github.com/ladybug-tools/ladybug-rhino/actions) ladybug-rhino
+[![Build Status](https://github.com/ladybug-tools/ladybug-rhino/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/ladybug-rhino/actions) ladybug-rhino
 
-[![Build Status](https://github.com/ladybug-tools/ladybug-grasshopper/workflows/CI/badge.svg)](https://github.com/ladybug-tools/ladybug-grasshopper/actions) ladybug-grasshopper
+[![Build Status](https://github.com/ladybug-tools/ladybug-grasshopper/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/ladybug-grasshopper/actions) ladybug-grasshopper
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-grasshopper-core/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-grasshopper-core/actions) honeybee-grasshopper-core
+[![Build Status](https://github.com/ladybug-tools/honeybee-grasshopper-core/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-grasshopper-core/actions) honeybee-grasshopper-core
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-grasshopper-energy/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-grasshopper-energy/actions) honeybee-grasshopper-energy
+[![Build Status](https://github.com/ladybug-tools/honeybee-grasshopper-energy/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-grasshopper-energy/actions) honeybee-grasshopper-energy
 
-[![Build Status](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/actions) honeybee-grasshopper-radiance
+[![Build Status](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/actions) honeybee-grasshopper-radiance
 
-[![Build Status](https://github.com/ladybug-tools/dragonfly-grasshopper/workflows/CI/badge.svg)](https://github.com/ladybug-tools/dragonfly-grasshopper/actions) dragonfly-grasshopper
+[![Build Status](https://github.com/ladybug-tools/dragonfly-grasshopper/actions/workflows/ci.yaml/badge.svg)](https://github.com/ladybug-tools/dragonfly-grasshopper/actions) dragonfly-grasshopper
```

### Comparing `lbt-grasshopper-1.8.6/LICENSE` & `lbt-grasshopper-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.6/PKG-INFO` & `lbt-grasshopper-1.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbt-grasshopper
-Version: 1.8.6
+Version: 1.8.7
 Summary: Collection of all Ladybug Tools plugins for Grasshopper
 Home-page: https://github.com/ladybug-tools/lbt-grasshopper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: Implementation :: IronPython
```

### Comparing `lbt-grasshopper-1.8.6/README.md` & `lbt-grasshopper-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.6/gradients.png` & `lbt-grasshopper-1.8.7/gradients.png`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.6/installer.gh` & `lbt-grasshopper-1.8.7/installer.gh`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.6/lbt_grasshopper.egg-info/PKG-INFO` & `lbt-grasshopper-1.8.7/lbt_grasshopper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbt-grasshopper
-Version: 1.8.6
+Version: 1.8.7
 Summary: Collection of all Ladybug Tools plugins for Grasshopper
 Home-page: https://github.com/ladybug-tools/lbt-grasshopper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: Implementation :: IronPython
```

### Comparing `lbt-grasshopper-1.8.6/setup.py` & `lbt-grasshopper-1.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.6/uninstaller.gh` & `lbt-grasshopper-1.8.7/uninstaller.gh`

 * *Files identical despite different names*

