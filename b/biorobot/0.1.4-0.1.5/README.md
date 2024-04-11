# Comparing `tmp/biorobot-0.1.4.tar.gz` & `tmp/biorobot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biorobot-0.1.4.tar", last modified: Wed Mar 27 10:56:27 2024, max compression
+gzip compressed data, was "biorobot-0.1.5.tar", last modified: Wed Apr 10 15:32:17 2024, max compression
```

## Comparing `biorobot-0.1.4.tar` & `biorobot-0.1.5.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.735893 biorobot-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-27 10:56:23.000000 biorobot-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-27 10:56:23.000000 biorobot-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-03-27 10:56:27.735893 biorobot-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-03-27 10:56:23.000000 biorobot-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.723893 biorobot-0.1.4/biorobot/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.723893 biorobot-0.1.4/biorobot/brittle_star/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.723893 biorobot-0.1.4/biorobot/brittle_star/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.727893 biorobot-0.1.4/biorobot/brittle_star/environment/directed_locomotion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/directed_locomotion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/directed_locomotion/dual.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/directed_locomotion/mjc_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/directed_locomotion/mjx_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/directed_locomotion/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.727893 biorobot-0.1.4/biorobot/brittle_star/environment/light_escape/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/light_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/light_escape/dual.py
--rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/light_escape/mjc_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/light_escape/mjx_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/light_escape/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.727893 biorobot-0.1.4/biorobot/brittle_star/environment/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/shared/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/shared/mjc_observables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/shared/mjx_observables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.727893 biorobot-0.1.4/biorobot/brittle_star/environment/undirected_locomotion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/undirected_locomotion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/undirected_locomotion/dual.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/undirected_locomotion/mjc_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/undirected_locomotion/mjx_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/environment/undirected_locomotion/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.727893 biorobot-0.1.4/biorobot/brittle_star/mjcf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/mjcf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.727893 biorobot-0.1.4/biorobot/brittle_star/mjcf/arena/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/mjcf/arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/mjcf/arena/aquarium.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.727893 biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/morphology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.731893 biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/parts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/parts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/parts/arm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/parts/arm_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/parts/disk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.731893 biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/specification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/specification/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/specification/specification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.731893 biorobot-0.1.4/biorobot/brittle_star/usage_examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/usage_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/usage_examples/directed_locomotion_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/usage_examples/light_escape_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/usage_examples/light_escape_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/brittle_star/usage_examples/undirected_locomotion_single.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.731893 biorobot-0.1.4/biorobot/toy_example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.731893 biorobot-0.1.4/biorobot/toy_example/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13905 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/environment/mjc_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/environment/mjx_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.731893 biorobot-0.1.4/biorobot/toy_example/mjcf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/mjcf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.731893 biorobot-0.1.4/biorobot/toy_example/mjcf/arena/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/mjcf/arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/mjcf/arena/arena.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/mjcf/arena/target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.731893 biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/morphology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.731893 biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/parts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/parts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/parts/arm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/parts/arm_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/parts/torso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.735893 biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/specification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/specification/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/specification/specification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.735893 biorobot-0.1.4/biorobot/toy_example/usage_examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/usage_examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.735893 biorobot-0.1.4/biorobot/toy_example/usage_examples/mjc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/usage_examples/mjc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/usage_examples/mjc/example_usage_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/usage_examples/mjc/example_usage_vectorized.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.735893 biorobot-0.1.4/biorobot/toy_example/usage_examples/mjx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/usage_examples/mjx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/usage_examples/mjx/example_usage_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/toy_example/usage_examples/mjx/example_usage_vectorized.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.735893 biorobot-0.1.4/biorobot/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/utils/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-27 10:56:23.000000 biorobot-0.1.4/biorobot/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:56:27.735893 biorobot-0.1.4/biorobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-03-27 10:56:27.000000 biorobot-0.1.4/biorobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-03-27 10:56:27.000000 biorobot-0.1.4/biorobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 10:56:27.000000 biorobot-0.1.4/biorobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-27 10:56:27.000000 biorobot-0.1.4/biorobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 10:56:27.000000 biorobot-0.1.4/biorobot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-27 10:56:23.000000 biorobot-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-27 10:56:23.000000 biorobot-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 10:56:27.735893 biorobot-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-27 10:56:23.000000 biorobot-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.775164 biorobot-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 15:32:12.000000 biorobot-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 15:32:12.000000 biorobot-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-10 15:32:17.775164 biorobot-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-10 15:32:12.000000 biorobot-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.763163 biorobot-0.1.5/biorobot/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.763163 biorobot-0.1.5/biorobot/brittle_star/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.763163 biorobot-0.1.5/biorobot/brittle_star/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.767163 biorobot-0.1.5/biorobot/brittle_star/environment/directed_locomotion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/directed_locomotion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/directed_locomotion/dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/directed_locomotion/mjc_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/directed_locomotion/mjx_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/directed_locomotion/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.767163 biorobot-0.1.5/biorobot/brittle_star/environment/light_escape/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/light_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/light_escape/dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/light_escape/mjc_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/light_escape/mjx_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/light_escape/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.767163 biorobot-0.1.5/biorobot/brittle_star/environment/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/shared/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/shared/mjc_observables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/shared/mjx_observables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.767163 biorobot-0.1.5/biorobot/brittle_star/environment/undirected_locomotion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/undirected_locomotion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/undirected_locomotion/dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/undirected_locomotion/mjc_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/undirected_locomotion/mjx_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/environment/undirected_locomotion/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.767163 biorobot-0.1.5/biorobot/brittle_star/mjcf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/mjcf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.767163 biorobot-0.1.5/biorobot/brittle_star/mjcf/arena/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/mjcf/arena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/mjcf/arena/aquarium.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.767163 biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/morphology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.771164 biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/parts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/parts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/parts/arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/parts/arm_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/parts/disk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.771164 biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/specification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/specification/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/specification/specification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.771164 biorobot-0.1.5/biorobot/brittle_star/usage_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/usage_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/usage_examples/directed_locomotion_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/usage_examples/light_escape_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/usage_examples/light_escape_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/brittle_star/usage_examples/undirected_locomotion_single.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.771164 biorobot-0.1.5/biorobot/toy_example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.771164 biorobot-0.1.5/biorobot/toy_example/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13905 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/environment/mjc_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/environment/mjx_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.771164 biorobot-0.1.5/biorobot/toy_example/mjcf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/mjcf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.771164 biorobot-0.1.5/biorobot/toy_example/mjcf/arena/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/mjcf/arena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/mjcf/arena/arena.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/mjcf/arena/target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.771164 biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/morphology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.775164 biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/parts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/parts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/parts/arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/parts/arm_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/parts/torso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.775164 biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/specification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/specification/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/specification/specification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.775164 biorobot-0.1.5/biorobot/toy_example/usage_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/usage_examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.775164 biorobot-0.1.5/biorobot/toy_example/usage_examples/mjc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/usage_examples/mjc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/usage_examples/mjc/example_usage_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/usage_examples/mjc/example_usage_vectorized.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.775164 biorobot-0.1.5/biorobot/toy_example/usage_examples/mjx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/usage_examples/mjx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/usage_examples/mjx/example_usage_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/toy_example/usage_examples/mjx/example_usage_vectorized.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.775164 biorobot-0.1.5/biorobot/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/utils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-10 15:32:12.000000 biorobot-0.1.5/biorobot/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:32:17.775164 biorobot-0.1.5/biorobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-10 15:32:17.000000 biorobot-0.1.5/biorobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-10 15:32:17.000000 biorobot-0.1.5/biorobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 15:32:17.000000 biorobot-0.1.5/biorobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-10 15:32:17.000000 biorobot-0.1.5/biorobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 15:32:17.000000 biorobot-0.1.5/biorobot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-10 15:32:12.000000 biorobot-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-10 15:32:12.000000 biorobot-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:32:17.775164 biorobot-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-10 15:32:12.000000 biorobot-0.1.5/setup.py
```

### Comparing `biorobot-0.1.4/LICENSE` & `biorobot-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/PKG-INFO` & `biorobot-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biorobot
-Version: 0.1.4
+Version: 0.1.5
 Summary: The Bio-inspired Robotics Testbed (BRT).
 Home-page: https://github.com/Co-Evolve/brb
 Author-email: Dries Marzougui <dries.marzougui@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Co-Evolve/brt
 Project-URL: Repository, https://github.com/Co-Evolve/brt
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biorobot Version: 0.1.4 Summary: The Bio-inspired
+Metadata-Version: 2.1 Name: biorobot Version: 0.1.5 Summary: The Bio-inspired
 Robotics Testbed (BRT). Home-page: https://github.com/Co-Evolve/brb Author-
 email: Dries Marzougui
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/Co-Evolve/brt
 Project-URL: Repository, https://github.com/Co-Evolve/brt Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
```

### Comparing `biorobot-0.1.4/README.md` & `biorobot-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/directed_locomotion/dual.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/directed_locomotion/dual.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/directed_locomotion/mjc_env.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/directed_locomotion/mjc_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/directed_locomotion/mjx_env.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/directed_locomotion/mjx_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/directed_locomotion/shared.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/directed_locomotion/shared.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/light_escape/dual.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/light_escape/dual.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/light_escape/mjc_env.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/light_escape/mjc_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/light_escape/mjx_env.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/light_escape/mjx_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/light_escape/shared.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/light_escape/shared.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/shared/base.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/shared/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
         joint_randomization_noise_scale: float = 0.0,
         color_contacts: bool = False,
         *args,
         **kwargs,
     ):
         super().__init__(
             disable_eulerdamp=True,
-            solver_iterations=1,
-            solver_ls_iterations=1,
+            solver_iterations=10,
+            solver_ls_iterations=10,
             *args,
             **kwargs,
         )
         self.joint_randomization_noise_scale = joint_randomization_noise_scale
         self.color_contacts = color_contacts
```

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/shared/mjc_observables.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/shared/mjc_observables.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/shared/mjx_observables.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/shared/mjx_observables.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/undirected_locomotion/dual.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/undirected_locomotion/dual.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/undirected_locomotion/mjc_env.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/undirected_locomotion/mjc_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/undirected_locomotion/mjx_env.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/undirected_locomotion/mjx_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/environment/undirected_locomotion/shared.py` & `biorobot-0.1.5/biorobot/brittle_star/environment/undirected_locomotion/shared.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/mjcf/arena/aquarium.py` & `biorobot-0.1.5/biorobot/brittle_star/mjcf/arena/aquarium.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/morphology.py` & `biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/morphology.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/parts/arm.py` & `biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/parts/arm.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/parts/arm_segment.py` & `biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/parts/arm_segment.py`

 * *Files 22% similar despite different names*

```diff
@@ -112,55 +112,44 @@
     def _is_first_segment(self) -> bool:
         return self._segment_index == 0
 
     def _is_last_segment(self) -> bool:
         number_of_segments = len(self._arm_specification.segment_specifications)
         return self._segment_index == number_of_segments - 1
 
-    @property
-    def volume(self) -> float:
-        radius = self._segment_specification.radius.value
-        length = self._segment_specification.length.value
-
-        sphere_volume = 4 / 3 * np.pi * radius**3
-        cylinder_volume = np.pi * radius**2 * length
-
-        return sphere_volume + cylinder_volume
-
-    def _get_p_control_kp(self, joint: _ElementImpl) -> float:
-        kp = self.volume * 500_000
-        return kp
+    def _get_strength(self, joint: _ElementImpl) -> float:
+        strength = self._segment_specification.radius.value * 200
+        return strength
 
     def _configure_p_control_actuator(self, joint: _ElementImpl) -> None:
         self.mjcf_model.actuator.add(
             "position",
             name=f"{joint.name}_p_control",
             joint=joint,
-            kp=self._get_p_control_kp(joint),
+            kp=50,
             ctrllimited=True,
             ctrlrange=joint.range,
+            forcelimited=True,
+            forcerange=[-self._get_strength(joint), self._get_strength(joint)],
         )
 
     def _configure_p_control_actuators(self) -> None:
         if self.morphology_specification.actuation_specification.use_p_control.value:
             self._configure_p_control_actuator(self._in_plane_joint)
             self._configure_p_control_actuator(self._out_of_plane_joint)
 
-    def _get_torque_control_gear(self, joint: _ElementImpl) -> float:
-        gear = self.volume * 200_000
-        return gear
-
     def _configure_torque_control_actuator(self, joint: _ElementImpl) -> None:
         self.mjcf_model.actuator.add(
             "motor",
             name=f"{joint.name}_torque_control",
             joint=joint,
-            gear=[self._get_torque_control_gear(joint)],
             ctrllimited=True,
-            ctrlrange=[-1, 1],
+            ctrlrange=[-self._get_strength(joint), self._get_strength(joint)],
+            forcelimited=True,
+            forcerange=[-self._get_strength(joint), self._get_strength(joint)],
         )
 
     def _configure_torque_control_actuators(self) -> None:
         if (
             self.morphology_specification.actuation_specification.use_torque_control.value
         ):
             self._configure_torque_control_actuator(self._in_plane_joint)
```

### Comparing `biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/parts/disk.py` & `biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/parts/disk.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/specification/default.py` & `biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/specification/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 def linear_interpolation(alpha: float, start: float, stop: float) -> float:
     return start + alpha * (stop - start)
 
 
 def default_joint_specification(range: float) -> BrittleStarJointSpecification:
     joint_specification = BrittleStarJointSpecification(
-        range=range, stiffness=1.1084, damping=5.5084, armature=0.45
+        range=range, stiffness=0.1, damping=0.5, armature=0.02
     )
 
     return joint_specification
 
 
 def default_arm_segment_specification(
     alpha: float,
```

### Comparing `biorobot-0.1.4/biorobot/brittle_star/mjcf/morphology/specification/specification.py` & `biorobot-0.1.5/biorobot/brittle_star/mjcf/morphology/specification/specification.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/usage_examples/directed_locomotion_single.py` & `biorobot-0.1.5/biorobot/brittle_star/usage_examples/directed_locomotion_single.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/usage_examples/light_escape_single.py` & `biorobot-0.1.5/biorobot/brittle_star/usage_examples/light_escape_single.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/usage_examples/light_escape_vectorized.py` & `biorobot-0.1.5/biorobot/brittle_star/usage_examples/light_escape_vectorized.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/brittle_star/usage_examples/undirected_locomotion_single.py` & `biorobot-0.1.5/biorobot/brittle_star/usage_examples/undirected_locomotion_single.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 )
 
 
 def create_env(
     backend: str, render_mode: str
 ) -> BrittleStarUndirectedLocomotionEnvironment:
     morphology_spec = default_brittle_star_morphology_specification(
-        num_arms=5, num_segments_per_arm=5, use_p_control=True
+        num_arms=5, num_segments_per_arm=5, use_p_control=True, use_torque_control=False
     )
     morphology = MJCFBrittleStarMorphology(morphology_spec)
     arena_config = AquariumArenaConfiguration()
     arena = MJCFAquariumArena(configuration=arena_config)
 
     env_config = BrittleStarUndirectedLocomotionEnvironmentConfiguration(
         render_mode=render_mode,
@@ -42,15 +42,15 @@
     env = BrittleStarUndirectedLocomotionEnvironment.from_morphology_and_arena(
         morphology=morphology, arena=arena, configuration=env_config, backend=backend
     )
     return env
 
 
 if __name__ == "__main__":
-    BACKEND = "MJC"
+    BACKEND = "MJX"
     RENDER_MODE = "human"
 
     env = create_env(backend=BACKEND, render_mode=RENDER_MODE)
 
     if BACKEND == "MJC":
         env_rng, action_rng = np.random.RandomState(0), None
         step_fn = env.step
@@ -70,12 +70,9 @@
             return env.action_space.sample(rng=sub_rng), rng
 
     state = reset_fn(env_rng)
     while True:
         action, action_rng = action_sample_fn(action_rng)
         state = step_fn(state=state, action=action)
         print(state.observations["joint_position"])
-        print(state.observations["joint_velocity"])
-        print(state.observations["joint_actuator_force"])
-        print()
         env.render(state=state)
     env.close()
```

### Comparing `biorobot-0.1.4/biorobot/toy_example/environment/mjc_env.py` & `biorobot-0.1.5/biorobot/toy_example/environment/mjc_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/toy_example/environment/mjx_env.py` & `biorobot-0.1.5/biorobot/toy_example/environment/mjx_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/toy_example/mjcf/arena/arena.py` & `biorobot-0.1.5/biorobot/toy_example/mjcf/arena/arena.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/morphology.py` & `biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/morphology.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/parts/arm.py` & `biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/parts/arm.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/parts/arm_segment.py` & `biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/parts/arm_segment.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/parts/torso.py` & `biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/parts/torso.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/specification/default.py` & `biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/specification/default.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/toy_example/mjcf/morphology/specification/specification.py` & `biorobot-0.1.5/biorobot/toy_example/mjcf/morphology/specification/specification.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/toy_example/usage_examples/mjc/example_usage_single.py` & `biorobot-0.1.5/biorobot/toy_example/usage_examples/mjc/example_usage_single.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/toy_example/usage_examples/mjc/example_usage_vectorized.py` & `biorobot-0.1.5/biorobot/toy_example/usage_examples/mjc/example_usage_vectorized.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/toy_example/usage_examples/mjx/example_usage_single.py` & `biorobot-0.1.5/biorobot/toy_example/usage_examples/mjx/example_usage_single.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/toy_example/usage_examples/mjx/example_usage_vectorized.py` & `biorobot-0.1.5/biorobot/toy_example/usage_examples/mjx/example_usage_vectorized.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/utils/colors.py` & `biorobot-0.1.5/biorobot/utils/colors.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/utils/noise.py` & `biorobot-0.1.5/biorobot/utils/noise.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot/utils/video.py` & `biorobot-0.1.5/biorobot/utils/video.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/biorobot.egg-info/PKG-INFO` & `biorobot-0.1.5/biorobot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biorobot
-Version: 0.1.4
+Version: 0.1.5
 Summary: The Bio-inspired Robotics Testbed (BRT).
 Home-page: https://github.com/Co-Evolve/brb
 Author-email: Dries Marzougui <dries.marzougui@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Co-Evolve/brt
 Project-URL: Repository, https://github.com/Co-Evolve/brt
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biorobot Version: 0.1.4 Summary: The Bio-inspired
+Metadata-Version: 2.1 Name: biorobot Version: 0.1.5 Summary: The Bio-inspired
 Robotics Testbed (BRT). Home-page: https://github.com/Co-Evolve/brb Author-
 email: Dries Marzougui
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/Co-Evolve/brt
 Project-URL: Repository, https://github.com/Co-Evolve/brt Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
```

### Comparing `biorobot-0.1.4/biorobot.egg-info/SOURCES.txt` & `biorobot-0.1.5/biorobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.4/pyproject.toml` & `biorobot-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "biorobot"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
     { name = "Dries Marzougui", email = "dries.marzougui@gmail.com" },
 ]
 description = "The Bio-inspired Robotics Testbed (BRT)."
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { text = "MIT" }
 classifiers = [
```

### Comparing `biorobot-0.1.4/setup.py` & `biorobot-0.1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     license = f.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
         name='biorobot',
-        version='0.1.4',
+        version='0.1.5',
         description='The Bio-inspired Robotics Testbed.',
         long_description=readme,
         url='https://github.com/Co-Evolve/brb',
         license=license,
         packages=find_packages(exclude=('tests', 'docs')),
         install_requires=required
         )
```

