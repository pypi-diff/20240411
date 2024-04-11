# Comparing `tmp/mly-1.0.0.tar.gz` & `tmp/mly-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly-1.0.0.tar", last modified: Fri Jan 19 15:12:45 2024, max compression
+gzip compressed data, was "mly-1.0.3.tar", last modified: Thu Apr 11 09:05:40 2024, max compression
```

## Comparing `mly-1.0.0.tar` & `mly-1.0.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-01-19 15:12:45.115186 mly-1.0.0/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      106 2024-01-12 11:29:08.000000 mly-1.0.0/.gitignore
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1673 2023-07-18 09:16:42.000000 mly-1.0.0/.gitlab-ci.yml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:19.000000 mly-1.0.0/LICENSE
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      698 2024-01-19 15:12:45.114186 mly-1.0.0/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2021-01-11 16:48:33.000000 mly-1.0.0/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-01-19 15:12:45.074185 mly-1.0.0/mly/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  3493542 2023-09-11 15:21:17.000000 mly-1.0.0/mly/SRD.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:15:39.000000 mly-1.0.0/mly/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      411 2024-01-19 15:12:44.000000 mly-1.0.0/mly/_version.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10331 2023-11-22 17:14:48.000000 mly-1.0.0/mly/createFileSystem.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-01-19 15:12:45.083185 mly-1.0.0/mly/datatools/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      155 2023-07-18 09:16:42.000000 mly-1.0.0/mly/datatools/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22332 2023-07-18 09:16:42.000000 mly-1.0.0/mly/datatools/core.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28224 2023-12-07 11:49:40.000000 mly-1.0.0/mly/datatools/datatools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    95588 2023-12-07 11:40:41.000000 mly-1.0.0/mly/datatools/generator.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-01-19 15:12:45.086185 mly-1.0.0/mly/datatools/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-07-18 09:16:42.000000 mly-1.0.0/mly/datatools/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3438 2023-07-18 09:16:42.000000 mly-1.0.0/mly/datatools/tests/test_core.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      441 2023-07-18 09:16:42.000000 mly-1.0.0/mly/datatools/tests/test_datatools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5075 2023-09-11 15:21:17.000000 mly-1.0.0/mly/datatools/tests/test_generator.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19065 2023-11-22 17:13:37.000000 mly-1.0.0/mly/exceptions.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7314 2023-11-01 17:24:53.000000 mly-1.0.0/mly/offlinefar.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7796 2023-09-11 15:21:12.000000 mly-1.0.0/mly/plugins.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10595 2023-12-06 19:17:38.000000 mly-1.0.0/mly/projectwave.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8913 2022-03-15 16:16:40.000000 mly-1.0.0/mly/simulateddetectornoise.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    32530 2024-01-05 10:44:20.000000 mly-1.0.0/mly/skymap_utils.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-01-19 15:12:45.090185 mly-1.0.0/mly/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      653 2021-10-07 09:34:45.000000 mly-1.0.0/mly/tests/README.md
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      728 2021-10-07 09:34:45.000000 mly-1.0.0/mly/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1601 2021-10-08 08:22:16.000000 mly-1.0.0/mly/tests/test_init.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5258 2022-03-02 09:58:19.000000 mly-1.0.0/mly/tests/test_tools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13037 2023-07-18 09:16:42.000000 mly-1.0.0/mly/tools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   132149 2023-12-01 17:23:44.000000 mly-1.0.0/mly/validators.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    40367 2024-01-11 15:28:31.000000 mly-1.0.0/mly/waveforms.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-01-19 15:12:45.113186 mly-1.0.0/mly.egg-info/
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      698 2024-01-19 15:12:44.000000 mly-1.0.0/mly.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1281 2024-01-19 15:12:45.000000 mly-1.0.0/mly.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2024-01-19 15:12:44.000000 mly-1.0.0/mly.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      189 2024-01-19 15:12:44.000000 mly-1.0.0/mly.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2024-01-19 15:12:44.000000 mly-1.0.0/mly.egg-info/top_level.txt
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-01-19 15:12:45.051185 mly-1.0.0/pages/
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-01-19 15:12:45.092185 mly-1.0.0/pages/docs/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      638 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/Makefile
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      804 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/make.bat
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-01-19 15:12:45.111186 mly-1.0.0/pages/docs/source/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  4149543 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/GeneratorTutorial.ipynb
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       56 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/api.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2143 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/conf.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-01-19 15:12:45.112186 mly-1.0.0/pages/docs/source/generated/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       84 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/generated/mly.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      719 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/index.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      122 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/install.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1081 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/mly.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       46 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/modules.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   102698 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/timeseriesexample.png
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1445 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/tutorials.generator.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       60 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/tutorials.plugins.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      928 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/tutorials.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       62 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/tutorials.training.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       66 2022-08-19 14:30:26.000000 mly-1.0.0/pages/docs/source/tutorials.validation.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1238 2024-01-16 15:44:19.000000 mly-1.0.0/pyproject.toml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2024-01-19 15:12:45.115186 mly-1.0.0/setup.cfg
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:05:40.115414 mly-1.0.3/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      106 2024-01-12 11:29:08.000000 mly-1.0.3/.gitignore
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1621 2024-04-11 09:02:42.000000 mly-1.0.3/.gitlab-ci.yml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:19.000000 mly-1.0.3/LICENSE
+-rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      698 2024-04-11 09:05:40.113414 mly-1.0.3/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2021-01-11 16:48:33.000000 mly-1.0.3/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:05:39.782410 mly-1.0.3/mly/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  3493542 2023-09-11 15:21:17.000000 mly-1.0.3/mly/SRD.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:15:39.000000 mly-1.0.3/mly/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      411 2024-04-11 09:05:39.000000 mly-1.0.3/mly/_version.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10331 2023-11-22 17:14:48.000000 mly-1.0.3/mly/createFileSystem.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:05:39.812411 mly-1.0.3/mly/datatools/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      155 2023-07-18 09:16:42.000000 mly-1.0.3/mly/datatools/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22332 2023-07-18 09:16:42.000000 mly-1.0.3/mly/datatools/core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28224 2023-12-07 11:49:40.000000 mly-1.0.3/mly/datatools/datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    95588 2024-03-20 11:52:07.000000 mly-1.0.3/mly/datatools/generator.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:05:39.827411 mly-1.0.3/mly/datatools/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-07-18 09:16:42.000000 mly-1.0.3/mly/datatools/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3438 2023-07-18 09:16:42.000000 mly-1.0.3/mly/datatools/tests/test_core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      441 2023-07-18 09:16:42.000000 mly-1.0.3/mly/datatools/tests/test_datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5075 2023-09-11 15:21:17.000000 mly-1.0.3/mly/datatools/tests/test_generator.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19065 2024-03-20 11:52:07.000000 mly-1.0.3/mly/exceptions.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7314 2023-11-01 17:24:53.000000 mly-1.0.3/mly/offlinefar.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7827 2024-04-11 09:02:43.000000 mly-1.0.3/mly/plugins.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10595 2023-12-06 19:17:38.000000 mly-1.0.3/mly/projectwave.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8913 2022-03-15 16:16:40.000000 mly-1.0.3/mly/simulateddetectornoise.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    39362 2024-04-11 09:02:43.000000 mly-1.0.3/mly/skymap_utils.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:05:39.838411 mly-1.0.3/mly/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      653 2021-10-07 09:34:45.000000 mly-1.0.3/mly/tests/README.md
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      728 2021-10-07 09:34:45.000000 mly-1.0.3/mly/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1601 2021-10-08 08:22:16.000000 mly-1.0.3/mly/tests/test_init.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5258 2022-03-02 09:58:19.000000 mly-1.0.3/mly/tests/test_tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13037 2023-07-18 09:16:42.000000 mly-1.0.3/mly/tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   132149 2023-12-01 17:23:44.000000 mly-1.0.3/mly/validators.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    40367 2024-01-11 15:28:31.000000 mly-1.0.3/mly/waveforms.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:05:40.109414 mly-1.0.3/mly.egg-info/
+-rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      698 2024-04-11 09:05:39.000000 mly-1.0.3/mly.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1281 2024-04-11 09:05:39.000000 mly-1.0.3/mly.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2024-04-11 09:05:39.000000 mly-1.0.3/mly.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      189 2024-04-11 09:05:39.000000 mly-1.0.3/mly.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2024-04-11 09:05:39.000000 mly-1.0.3/mly.egg-info/top_level.txt
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:05:39.633409 mly-1.0.3/pages/
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:05:39.862411 mly-1.0.3/pages/docs/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      638 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/Makefile
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      804 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/make.bat
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:05:40.102414 mly-1.0.3/pages/docs/source/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  4149543 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/GeneratorTutorial.ipynb
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       56 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/api.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2143 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/conf.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:05:40.106414 mly-1.0.3/pages/docs/source/generated/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       84 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/generated/mly.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      719 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/index.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      122 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/install.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1081 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/mly.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       46 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/modules.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   102698 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/timeseriesexample.png
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1445 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/tutorials.generator.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       60 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/tutorials.plugins.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      928 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/tutorials.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       62 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/tutorials.training.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       66 2022-08-19 14:30:26.000000 mly-1.0.3/pages/docs/source/tutorials.validation.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1238 2024-01-16 15:44:19.000000 mly-1.0.3/pyproject.toml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2024-04-11 09:05:40.115414 mly-1.0.3/setup.cfg
```

### Comparing `mly-1.0.0/.gitlab-ci.yml` & `mly-1.0.3/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -46,28 +46,24 @@
     INSTALL_TARGET: "mly-*.tar.*"
     # point pytest at the installed package
     PYTEST_OPTIONS: "--pyargs mly"
 
 # actually run the tests for each python version we support
 test:3.7:
   extends: [.test]
-  image: python:3.7
+  image: python:3.8
 
 test:3.9:
   extends: [.test]
   image: python:3.9
 
 test:3.10:
   extends: [.test]
   image: python:3.10
 
-test:3.11:
-  extends: [.test]
-  image: python:3.11
-
 # -- lint -------------------
 #
 # Check the code for style
 # issues with flake8
 #
 
 lint:
```

### Comparing `mly-1.0.0/LICENSE` & `mly-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/PKG-INFO` & `mly-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly
-Version: 1.0.0
+Version: 1.0.3
 Summary: Toolkit package to run GW search using ML.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly-1.0.0/mly/SRD.py` & `mly-1.0.3/mly/SRD.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/createFileSystem.py` & `mly-1.0.3/mly/createFileSystem.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/datatools/core.py` & `mly-1.0.3/mly/datatools/core.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/datatools/datatools.py` & `mly-1.0.3/mly/datatools/datatools.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/datatools/generator.py` & `mly-1.0.3/mly/datatools/generator.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/datatools/tests/test_core.py` & `mly-1.0.3/mly/datatools/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/datatools/tests/test_generator.py` & `mly-1.0.3/mly/datatools/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/exceptions.py` & `mly-1.0.3/mly/exceptions.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/offlinefar.py` & `mly-1.0.3/mly/offlinefar.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/plugins.py` & `mly-1.0.3/mly/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,17 +144,18 @@
         window=int(0.043*fs)
     correlations=[]
     for i in range(len(detectors)):
         for j in range(1+i,len(detectors)):
             correlations.append(correlate(strain[i],strain[j],window).tolist())
     return(np.array(correlations))
     
-def plotcorrerlaion(strain,detectors,fs,data=None):
+def plotcorrerlaion(strain,detectors,fs,data=None,ax=None):
     
-    f,ax = plt.subplots(figsize=(15,7))#,facecolor='lightslategray')
+    if ax is None:
+        f,ax = plt.subplots(figsize=(15,7))#,facecolor='lightslategray')
     ax.set_xlabel('Time Shift')
     ax.set_ylabel('Pearson Correlation')
     tlength=len(data[0])/fs
     tarray=np.arange(-tlength/2,tlength/2,1/fs)
     count_=0
     for i in np.arange(len(detectors)):
         for j in np.arange(i+1,len(detectors)):
```

### Comparing `mly-1.0.0/mly/projectwave.py` & `mly-1.0.3/mly/projectwave.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/simulateddetectornoise.py` & `mly-1.0.3/mly/simulateddetectornoise.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/skymap_utils.py` & `mly-1.0.3/mly/skymap_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from pycbc.detector import Detector
 from math import *
 import numpy as np
 from .plugins import *
 from .datatools import *
 from scipy.signal import welch
 from scipy.signal import iirnotch, lfilter, butter
+from gwpy.timeseries import TimeSeries
 
 # GPS > GPS, GMST > GMST, ra = RA, dec = declination
 
 
 def GPStoGMST(GPS):
 
     # Function to convert a time in GPS seconds to Greenwich Mean Sidereal Time
@@ -143,55 +144,188 @@
         antenna_response_rms[pixel_index] = (np.sum(totalResponse))**0.5
 
     #print(antenna_response_rms)
     #print('antenna_response_rms', antenna_response_rms.shape)
 
     return antenna_response_rms
 
-def mask_window_tf(data_length, fs, start_time, end_time, ramp_duration):
+
+def mask_window_tf(T, fs, start_time, end_time, ramp_duration,ramp_centre, duration_limit = 1/32):
     """
     Creates a windowed mask for a given time series.
     
     Parameters:
-    - data_length: Length of the data series.
+    - T: Duration of the final data series.
     - fs: Sampling frequency.
     - start_time: Starting time of the window.
     - end_time: Ending time of the window.
     - ramp_duration: Duration of the ramp (smooth transition) in the window.
-    
+    - ramp_centre: Where will the center of the ramp be in respect of start and end time [0,1]
+                    0 corresponds for the center to be -0.5*ramp_duration away from the signal 
+                    1 corresponds for the center to be +0.5*ramp_duration in the signal (dumping the edge)
     Returns:
     - A windowed mask with values between 0 and 1.
     """
+    start_time = tf.cast(start_time, tf.float32)
+    end_time = tf.cast(end_time, tf.float32)
+    ramp_duration = tf.cast(ramp_duration, tf.float32)
+    ramp_centre = tf.cast(ramp_centre, tf.float32)
+    duration_limit = tf.cast(duration_limit, tf.float32)
+    fs = tf.cast(fs, tf.float32)
     tnp = tf.experimental.numpy
-    pi = tnp.pi 
-    PI_HALF = pi / 2
+    PI = tnp.pi 
+    PI = tf.cast( PI, tf.float32)
+    
+    # Duration limit is used as limiter on the duration of signals
+    # also it is used for the edges so that they are smooth and they
+    # do not fold on the other side.
+    if end_time - start_time < duration_limit:
+
+        diff = duration_limit - (end_time - start_time)
+        
+        start_time = start_time -diff/2
+        end_time = end_time + diff/2
+
+        print(f"Duration smaller than duration limit, and it was adjusted by {diff} s")
+
+    if start_time < ramp_duration:
+        # The first 32 ms will be folded to the end so we move the start time 
+        # enough to avoid that.
+        start_time = ramp_duration + duration_limit 
+        print("Start time close too close to the biggining")
+
+        # Adjusting duration in case the above adjustment 
+        # made duration negative or too small
+        if end_time-start_time < duration_limit: # Max difference between detectors
+            end_time = start_time + duration_limit
+            print("End time too close to start time, changed to start_time + 0.032")
+
+    if T-end_time < ramp_duration:
+        # The last 32 ms will be folded to the end so we move the start time 
+        # enough to avoid that.
+        end_time = T - ramp_duration - duration_limit
+        print("End time close too close to the biggining")
+        # Adjusting duration in case the above adjustment 
+        # made duration negative or too small
+        if end_time-start_time < duration_limit: # Max difference between detectors
+            start_time = end_time - duration_limit
+            print("Start time too close to end time, changed to end_time - 0.032")
+
+
+    signal_duration = end_time - start_time
+    
+    # Check that ramp_duration is a power of two:
+    # if not (ramp_duration != 0 
+    #     and ramp_duration<T/2 
+    #     and tf.subtract(tf.experimental.numpy.log2(ramp_duration) , tf.math.round(tf.experimental.numpy.log2(ramp_duration))).numpy() == 0.0):
+
+    #     raise ValueError("Ramp duration must be a power of two"
+    #                      ", and one fourth of the duration")
+
+    # Adjusting the ramp_duration when signals are too small
+    # Note: Possibly adjust this with the duration of the signal
+    #       to include cases where signal is small and at the edge.
+    while signal_duration <= 2 * ramp_duration * ramp_centre:
+
+        ramp_duration = ramp_duration/2
+
+        print(f"Ramp duration changed to 1/{int(fs/(ramp_duration*fs))}")
+
+        if ramp_duration == 1/128:
+            print("Ramp duration reached minimum value of 1/128")
+            break
+
+    # Creating the central platoe
+    centre_lentgh = int(( signal_duration - 2 * ramp_duration * ramp_centre ) * fs )
+    centre = tf.ones( centre_lentgh)
+
+    # Creating the ramps
+    t = tf.range( 0 , ramp_duration, 1/fs )
+    left_ramp  = tf.math.sin( PI * t * (1/ramp_duration) - PI/2 )/2 + 0.5
+    right_ramp = tf.math.sin( PI * t * (1/ramp_duration) + PI/2 )/2 + 0.5
+
+    # Creating the pads
+    #print(start_time, ramp_centre,ramp_duration,fs)
+    
+
+    left_pad =  tf.zeros( tf.cast(tf.math.ceil((start_time - (1 - ramp_centre) * ramp_duration) * fs),tf.int32) )
+    right_pad = tf.zeros( tf.cast(tf.math.ceil((T - end_time - (1 - ramp_centre) * ramp_duration) * fs ),tf.int32))
+
+    # print(len(left_pad),len(left_ramp),len(centre),len(right_ramp),len(right_pad))
+    # print(len(left_pad)+len(left_ramp)+len(centre)+len(right_ramp)+len(right_pad))
+
+    # Adjusting the length when sometimes a pixel or two missing due to the use of int and ceil.
+    
+    thesum = tf.cast(len(left_pad)+len(left_ramp)+len(centre)+len(right_ramp)+len(right_pad),tf.float32)
+
+    if thesum < T*fs:
+        diff = tf.cast( T*fs - thesum , tf.int32 ) 
+
+        centre = tf.concat([centre, tf.ones(diff)],0)
+    
+    elif thesum > T*fs:
+
+        diff = tf.cast( thesum - T*fs , tf.int32 )
 
-    # Convert times to indices and ensure they are float32
-    window_start_idx = tf.cast((start_time - ramp_duration) * fs, tf.float32)
-    window_end_idx = tf.cast((end_time + ramp_duration) * fs, tf.float32)
-    start_idx = tf.cast(start_time * fs, tf.float32)
-    end_idx = tf.cast(end_time * fs, tf.float32)
+        centre = centre[:-diff]
     
-    indices = tf.range(data_length, dtype=tf.float32)
+    else:
+        diff = 0
+
+    # Putting the mask together.
+    mask = tf.concat([ left_pad, left_ramp , centre, right_ramp, right_pad ],0)
+
+    return(mask)
+
+
+
+
+
+
+# def mask_window_tf_old(data_length, fs, start_time, end_time, ramp_duration):
+#     """
+#     Creates a windowed mask for a given time series.
     
-    # Create the rolling mask for the main windowed region
-    main_mask = tf.where((indices >= start_idx) & (indices < end_idx), 1., indices * 0.)
+#     Parameters:
+#     - data_length: Length of the data series.
+#     - fs: Sampling frequency.
+#     - start_time: Starting time of the window.
+#     - end_time: Ending time of the window.
+#     - ramp_duration: Duration of the ramp (smooth transition) in the window.
     
-    # Create the ramp-up transition
-    ramp_up = 0.5 * (1 + tf.math.sin(-PI_HALF + (indices - window_start_idx) / (start_idx - window_start_idx) * pi))
-    mask_on = tf.where((indices >= window_start_idx) & (indices < start_idx), ramp_up, 0.)
+#     Returns:
+#     - A windowed mask with values between 0 and 1.
+#     """
+#     tnp = tf.experimental.numpy
+#     pi = tnp.pi 
+#     PI_HALF = pi / 2
 
-    # Create the ramp-down transition
-    ramp_down = 0.5 * (1 + tf.math.sin(PI_HALF + (indices - end_idx) / (window_end_idx - end_idx) * pi))
-    mask_off = tf.where((indices >= end_idx) & (indices < window_end_idx), ramp_down, 0.)
+#     # Convert times to indices and ensure they are float32
+#     window_start_idx = tf.cast((start_time - ramp_duration) * fs, tf.float32)
+#     window_end_idx = tf.cast((end_time + ramp_duration) * fs, tf.float32)
+#     start_idx = tf.cast(start_time * fs, tf.float32)
+#     end_idx = tf.cast(end_time * fs, tf.float32)
+    
+#     indices = tf.range(data_length, dtype=tf.float32)
+    
+#     # Create the rolling mask for the main windowed region
+#     main_mask = tf.where((indices >= start_idx) & (indices < end_idx), 1., indices * 0.)
+    
+#     # Create the ramp-up transition
+#     ramp_up = 0.5 * (1 + tf.math.sin(-PI_HALF + (indices - window_start_idx) / (start_idx - window_start_idx) * pi))
+#     mask_on = tf.where((indices >= window_start_idx) & (indices < start_idx), ramp_up, 0.)
 
-    # Combine the masks
-    windowed_data = main_mask + mask_on + mask_off
+#     # Create the ramp-down transition
+#     ramp_down = 0.5 * (1 + tf.math.sin(PI_HALF + (indices - end_idx) / (window_end_idx - end_idx) * pi))
+#     mask_off = tf.where((indices >= end_idx) & (indices < window_end_idx), ramp_down, 0.)
 
-    return windowed_data
+#     # Combine the masks
+#     windowed_data = main_mask + mask_on + mask_off
+
+#     return windowed_data
 
 
 mask_window_tf = tf.function(mask_window_tf)
 
 
 #this is a tensorflow graph
 def EnergySkyMapsGRF(
@@ -200,15 +334,15 @@
     noise_psd,
     time_delay,
     null_coefficient,
     antenna_response_rms,
     num_pixels,
     num_detectors,
     fs,
-    window_parameter = None
+    window_parameter = None,
 ):
     """
     THIS FUNCTION IS A TENSORFLOW GRAPH AND CONVERTS APPLE TO ORANGE 
 
     Parameters
     ----------
 
@@ -250,22 +384,22 @@
     #Calculating spectral density of background noise
     noise_psd = tf.math.reduce_sum(tf.math.multiply(
         tf.math.square(null_coefficient), noise_psd), axis=1)
     
     if window_parameter is not None:
         print('activate window', window_parameter)
 
-        start_time, end_time, ramp_duration = window_parameter
+        start_time, end_time, ramp_duration, ramp_centre, duration_limit ,fmin, fmax = window_parameter
         
         # data_shape = tf.shape(strain)
         # num_det = data_shape[1]
         # data_len = data_shape[2]
         
         # Apply mask_window_tf function on strain data
-        windowed_data = mask_window_tf(fs, fs, start_time, end_time, ramp_duration)
+        windowed_data = mask_window_tf(1.0, fs, start_time, end_time, ramp_duration, ramp_centre, duration_limit = duration_limit)
         # print('windowed_data', windowed_data.shape)
         # print ('strain shape', strain.shape)
         # print('start_time_util', start_time)
         # print('end_time_until', start_time)
     
         
         # Reshape windowed_data to match the shape of strain
@@ -434,140 +568,147 @@
     
 
     return (coherentNullEnergy, incoherentNullEnergy)
 
 
 
 
-def bandpass(data, fs, f_min, f_max, filter_order=10):
+def gwpy_bandpass(data, fs, f_min, f_max):
+    
+    f_max = min(f_max , 480.0)
+    f_min = max(f_min , 32)
 
-    # ---- Construct bandpass filter.
-    b, a = butter(filter_order, [f_min, f_max], btype='bandpass', output='ba', fs=fs)
+    bandpassed_data = list( TimeSeries(data[i],sample_rate = fs).bandpass(
+                            f_min, f_max, fstop = (31,481)
+                            , gpass=2 , gstop=30 , type='iir') for i in range(len(data)) )
 
-    # ---- Assign storage for bandpassed data. Remove samples_to_crop samples from 
-    #      each end to avoid filter transients. 
-    samples_to_crop = 1 * fs  # 1 second at each end
-    bandpassed_data = np.zeros((data.shape[0], data.shape[1] - 2*samples_to_crop))
-    for index in range(data.shape[0]):    
-        # ---- Apply the filter.
-        filtered_data = lfilter(b, a, data[index])
-        # ---- Crop the ends and store.
-        bandpassed_data[index] = filtered_data[samples_to_crop:-samples_to_crop]
-        # # Crop the ends
-        # cropped_data = filtered_data[samples_to_crop:-samples_to_crop]
-        # # Store the cropped data
-        # bandpassed_data[index] = cropped_data
+    # # ---- Construct bandpass filter.
+    # b, a = butter(filter_order, [f_min, f_max], btype='bandpass', output='ba', fs=fs)
+
+    # # ---- Assign storage for bandpassed data. Remove samples_to_crop samples from 
+    # #      each end to avoid filter transients. 
+    # samples_to_crop = 1 * fs  # 1 second at each end
+    # bandpassed_data = np.zeros((data.shape[0], data.shape[1] - 2*samples_to_crop))
+    # for index in range(data.shape[0]):    
+    #     # ---- Apply the filter.
+    #     filtered_data = lfilter(b, a, data[index])
+    #     # ---- Crop the ends and store.
+    #     bandpassed_data[index] = filtered_data[samples_to_crop:-samples_to_crop]
+    #     # # Crop the ends
+    #     # cropped_data = filtered_data[samples_to_crop:-samples_to_crop]
+    #     # # Store the cropped data
+    #     # bandpassed_data[index] = cropped_data
         
-    return bandpassed_data
+    return np.asarray(bandpassed_data)
 
 
 
-def remove_lines(data, fs, f_min, f_max, Q=30.0, factor=10.0, smoothing=9.0):
+# def remove_lines(data, fs, f_min, f_max, Q=30.0, factor=10.0, smoothing=9.0):
 
-    # data  FORMAT? Timeseries data.
-    # fs  Integer. Sample rate [Hz] of timeseries data.
-    # f_min  Float. Minimum frequency [Hz] for bandpassing.
-    # f_max  Float. Maximum frequency [Hz] for bandpassing.
-    # Q  Float. Notch filter quality factor. Default 30.0.
-    # factor  Float. Minimum line height above median PSD. Default 10.0.
-    # smoothing  Float. Width [Hz] for smoothing. Default 9.0.
+#     # data  FORMAT? Timeseries data.
+#     # fs  Integer. Sample rate [Hz] of timeseries data.
+#     # f_min  Float. Minimum frequency [Hz] for bandpassing.
+#     # f_max  Float. Maximum frequency [Hz] for bandpassing.
+#     # Q  Float. Notch filter quality factor. Default 30.0.
+#     # factor  Float. Minimum line height above median PSD. Default 10.0.
+#     # smoothing  Float. Width [Hz] for smoothing. Default 9.0.
 
-    # ---- Parameters for line removal.
-    smoothingWindowHz = smoothing
-    minLineHeightFactor = factor
+#     # ---- Parameters for line removal.
+#     smoothingWindowHz = smoothing
+#     minLineHeightFactor = factor
     
-    # ---- FFT length. 
-    Nfft = 4 * fs    # FFT resolution 0.25 Hz
+#     # ---- FFT length. 
+#     Nfft = 4 * fs    # FFT resolution 0.25 Hz
 
-    # ---- Bandpass the data.
-    data = bandpass(data, fs, f_min, f_max)
+#     # ---- Bandpass the data.
+#     data = bandpass(data, fs, f_min, f_max)
     
-    confirmed_clean = False
+#     confirmed_clean = False
 
-    while confirmed_clean == False:
+#     while confirmed_clean == False:
 
-        notch_centre_bin = []
-        notch_width_bins = []
-        notch_height     = []  # really depth ...
+#         notch_centre_bin = []
+#         notch_width_bins = []
+#         notch_height     = []  # really depth ...
 
-        # ---- Check all timeseries for lines.
+#         # ---- Check all timeseries for lines.
 
-        # ---- Loop through the rows in the data (each row is a separate time series).
-        for ifo in range(data.shape[0]):
+#         # ---- Loop through the rows in the data (each row is a separate time series).
+#         for ifo in range(data.shape[0]):
 
-            # ---- Compute the PSD of the data.
-            frequency, psd = welch(data[ifo], fs=fs, nperseg=Nfft)
+#             # ---- Compute the PSD of the data.
+#             frequency, psd = welch(data[ifo], fs=fs, nperseg=Nfft)
         
-            # ---- Construct and plot the "smoothed" PSD.
-            smoothingWindowBins = int(smoothingWindowHz / (fs/Nfft))
-            median_psd = np.zeros_like(psd)
-            for bins in range(len(psd)):
-                start = max(0, bins - smoothingWindowBins)
-                end = min(len(psd), bins + smoothingWindowBins)
-                median_psd[bins] = np.median(psd[start:end])
+#             # ---- Construct and plot the "smoothed" PSD.
+#             smoothingWindowBins = int(smoothingWindowHz / (fs/Nfft))
+#             median_psd = np.zeros_like(psd)
+#             for bins in range(len(psd)):
+#                 start = max(0, bins - smoothingWindowBins)
+#                 end = min(len(psd), bins + smoothingWindowBins)
+#                 median_psd[bins] = np.median(psd[start:end])
             
-            # ---- Identify lines.
-            line_centre_bin = []
-            line_width_bins = []
-            line_height     = []
-            prev_bin = False
-            for j in range(len(psd)):
-                if (psd[j] > minLineHeightFactor*median_psd[j]) and (frequency[j] >= f_min) and (frequency[j] <= f_max):
-                    #print(frequency[j])
-                    if prev_bin==False:
-                        width_bins = 1
-                        max_height = psd[j] / median_psd[j]
-                        centre_bin = j
-                    else:
-                        width_bins = width_bins+1
-                        if psd[j] / median_psd[j] > max_height:
-                            max_height = psd[j] / median_psd[j]
-                            centre_bin = j
-                    prev_bin = True
-                else:
-                    if prev_bin==True:
-                        line_centre_bin.append(centre_bin)
-                        line_width_bins.append(width_bins)
-                        line_height.append(max_height)
-                        prev_bin = False
-            notch_centre_bin.append(line_centre_bin)
-            notch_width_bins.append(line_width_bins)
-            notch_height.append(line_height)
-
-        # ---- Remove the lines.
-        confirmed_clean = True
-        for ifo in range(data.shape[0]):
-            frequencies_to_remove = frequency[notch_centre_bin[ifo]]
-            if notch_centre_bin[ifo]:
-                print('notches found for detector',ifo,':')
-                print(notch_centre_bin[ifo])
-                confirmed_clean = False # resets to loop again if any lines found
-            # ---- Copy the original data.
-            filtered_data = np.copy(data[ifo])
-            # ---- Loop over frequencies and apply notch filter.
-            for f0 in frequencies_to_remove:
-                # ---- Create and apply a notch filter.
-                b, a = iirnotch(f0, Q, fs)
-                filtered_data = lfilter(b, a, filtered_data)
-            # ---- Replace background timeseries in the pod.
-            data[ifo] = filtered_data            
-
-    # ---- Return central 1 second of notched data.
-    # w = int(data.shape[1]/fs)
-    # # print('w =',w)
-    # # print('original shape of notched data:',notched_data.shape)
-    # data = data[:,int(((w-1)/2)*fs):int(((w+1)/2)*fs)]
-    # # print('shape of notched data:',notched_data.shape)
-    return data
+#             # ---- Identify lines.
+#             line_centre_bin = []
+#             line_width_bins = []
+#             line_height     = []
+#             prev_bin = False
+#             for j in range(len(psd)):
+#                 if (psd[j] > minLineHeightFactor*median_psd[j]) and (frequency[j] >= f_min) and (frequency[j] <= f_max):
+#                     #print(frequency[j])
+#                     if prev_bin==False:
+#                         width_bins = 1
+#                         max_height = psd[j] / median_psd[j]
+#                         centre_bin = j
+#                     else:
+#                         width_bins = width_bins+1
+#                         if psd[j] / median_psd[j] > max_height:
+#                             max_height = psd[j] / median_psd[j]
+#                             centre_bin = j
+#                     prev_bin = True
+#                 else:
+#                     if prev_bin==True:
+#                         line_centre_bin.append(centre_bin)
+#                         line_width_bins.append(width_bins)
+#                         line_height.append(max_height)
+#                         prev_bin = False
+#             notch_centre_bin.append(line_centre_bin)
+#             notch_width_bins.append(line_width_bins)
+#             notch_height.append(line_height)
+
+#         # ---- Remove the lines.
+#         confirmed_clean = True
+#         for ifo in range(data.shape[0]):
+#             frequencies_to_remove = frequency[notch_centre_bin[ifo]]
+#             if notch_centre_bin[ifo]:
+#                 print('notches found for detector',ifo,':')
+#                 print(notch_centre_bin[ifo])
+#                 confirmed_clean = False # resets to loop again if any lines found
+#             # ---- Copy the original data.
+#             filtered_data = np.copy(data[ifo])
+#             # ---- Loop over frequencies and apply notch filter.
+#             for f0 in frequencies_to_remove:
+#                 # ---- Create and apply a notch filter.
+#                 b, a = iirnotch(f0, Q, fs)
+#                 filtered_data = lfilter(b, a, filtered_data)
+#             # ---- Replace background timeseries in the pod.
+#             data[ifo] = filtered_data            
+
+#     # ---- Return central 1 second of notched data.
+#     # w = int(data.shape[1]/fs)
+#     # # print('w =',w)
+#     # # print('original shape of notched data:',notched_data.shape)
+#     # data = data[:,int(((w-1)/2)*fs):int(((w+1)/2)*fs)]
+#     # # print('shape of notched data:',notched_data.shape)
+#     return data
 
 def remove_line(data, fs, f_min, f_max, Q=30.0, factor=10.0):
     
     # print('shape of raw data:',data.shape)
 
-    data = bandpass(data, fs, f_min, f_max)
+    data = gwpy_bandpass(data, fs, f_min, f_max)
     
     # print('shape of bandpassed data:',data.shape)
 
     # FFT length chosen 4 times the sample frequency (FFT resolution 0.25 Hz)
     Nfft = 4 * fs  
     notched_data = np.zeros_like(data)  # Array to hold the smoothed time series
     # originalPSD = []
@@ -696,20 +837,29 @@
     
     #print('td shape:',time_delay_map.shape)
 
     frequency_axis = np.fft.rfftfreq(fs, d=1/fs)
 
     # < ------------------------------------------
     
-    notched_strain = remove_line(uwstrain, fs, f_min=20, f_max=480, Q=30.0, factor=10)
+    notched_strain = remove_line(uwstrain, fs, f_min=window_parameter[-2], f_max=window_parameter[-1], Q=30.0, factor=10)
+    from gwpy.timeseries import TimeSeries
 
+    # HARDCODED ###
+    notched_strain_white = np.asarray([TimeSeries(notched_strain[0],sample_rate = fs).whiten(
+                                                  4,2,fduration=4,method = 'welch', highpass=20).value
+                                      ,TimeSeries(notched_strain[1],sample_rate = fs).whiten(
+                                                  4,2,fduration=4,method = 'welch', highpass=20).value])
+                                                  
     w = int(notched_strain.shape[1]/fs)
 
-    notched_strain= notched_strain[:,int(((w-1)/2)*fs):int(((w+1)/2)*fs)]
+    notched_strain_white = notched_strain_white[:,int(((w-1)/2)*fs):int(((w+1)/2)*fs)]
+    ###
 
+    notched_strain= notched_strain[:,int(((w-1)/2)*fs):int(((w+1)/2)*fs)]
     start = time.time()
     sky_map = EnergySkyMaps(notched_strain,
                             time_delay_map, 
                             frequency_axis,
                             psd,
                             num_pixels, 
                             len(detectors), 
@@ -731,17 +881,17 @@
 
     prob_map_total = np.array(prob_map)
     Lsky_array = np.array(Lsky)
 
     containment_region_50 = containment_region(prob_map,threshold=0.5)
     containment_region_90 = containment_region(prob_map,threshold=0.9)
 
-    return [ prob_map_total, Lsky_array, antenna_response_rms , containment_region_50, containment_region_90]
+    return [ prob_map_total, Lsky_array, antenna_response_rms , containment_region_50, containment_region_90,notched_strain_white]
 
-def skymap_plot_function(strain,data=None):
+def skymap_plot_function(strain,data=None,ax = None):
         
     """
     Function to format and display a LIGO skymap plot.
 
     Parameters
     ----------
     probmap: A HEALPix probability map to be plotted.
@@ -760,32 +910,37 @@
     containment_region_50 = data[3]
     containment_region_90 = data[4]
     # Plot settings
     projection='astro hours mollweide'
     nested=True
     cmap='cylon'
 
-    fig = plt.figure(figsize=(10, 5))
-    ax = fig.add_subplot(111, projection=projection)
+    if ax is None:
+        fig = plt.figure(figsize=(10, 5))
+        ax = fig.add_subplot(111, projection=projection)
+    else:
+        print('For skymaps you need projection = \'astro hours mollweide\'')
 
     # Plot the sky map
     img = ax.imshow_hpx(probmap, nested=nested, cmap=cmap)
 
     # Add grid lines
     ax.grid(True, which='major', color='k', linestyle='-', linewidth=0)
 
-    ax.text(0.8, 1, f"50% area: {containment_region_50:.3f} deg²", weight='bold', transform=ax.transAxes)  
-    ax.text(0.8, 0.95, f"90% area: {containment_region_90:.3f} deg²", weight='bold', transform=ax.transAxes) 
+    ax.text(0.8, 1, f"50% area: {containment_region_50:.1f} deg²", weight='bold', transform=ax.transAxes)  
+    ax.text(0.8, 0.95, f"90% area: {containment_region_90:.1f} deg²", weight='bold', transform=ax.transAxes) 
 
     c = 100 * postprocess.find_greedy_credible_levels(probmap)
     cs = ax.contour_hpx(c, nested=True, colors='k', linewidths=0.5, levels=[50,90])
     plt.clabel(cs, fmt='%g%%', fontsize=6, inline=True)
 
+    return ax
 
-def skymap_plot_function_with_inj(strain,RA,declination,data=None):
+
+def skymap_plot_function_with_inj(strain,RA,declination,data=None,ax = None):
         
     """
     Function to format and display a LIGO skymap plot.
 
     Parameters
     ----------
     probmap: A HEALPix probability map to be plotted.
@@ -807,27 +962,29 @@
     projection='astro hours mollweide'
     nested=True
     cmap='viridis'
     xlabel='Right Ascension'
     ylabel='Declination'
 
     # Create a new figure and subplot with a Mollweide projection
-    fig = plt.figure(figsize=(10, 5))
-    ax = fig.add_subplot(111, projection=projection)
-
+    if ax is None:
+        fig = plt.figure(figsize=(10, 5))
+        ax = fig.add_subplot(111, projection=projection)
+    else:
+        print('For skymaps you need projection = \'astro hours mollweide\'')
     # Plot the sky map
     img = ax.imshow_hpx(probmap, nested=nested, cmap=cmap)
 
     # Add grid lines
     ax.grid(True, which='major', color='white', linestyle='-', linewidth=0.2)
 
     ax.text(0, 0, xlabel, ha='center', va='center', transform=ax.transAxes)  
     ax.set_ylabel(ylabel)
-    ax.text(0.8, 1, f"50% area: {containment_region_50:.3f} deg²", weight='bold', transform=ax.transAxes)  
-    ax.text(0.8, 0.95, f"90% area: {containment_region_90:.3f} deg²", weight='bold', transform=ax.transAxes) 
+    ax.text(0.8, 1, f"50% area: {containment_region_50:.1f} deg²", weight='bold', transform=ax.transAxes)  
+    ax.text(0.8, 0.95, f"90% area: {containment_region_90:.1f} deg²", weight='bold', transform=ax.transAxes) 
     # Add color bar
     cbar = plt.colorbar(img, ax=ax, orientation='horizontal', fraction=0.05, pad=0.1)
     cbar.set_label('Probability')
 
     c = 100 * postprocess.find_greedy_credible_levels(probmap)
     cs = ax.contour_hpx(c, nested=True, colors='k', linewidths=0.5, levels=[50,90])
     plt.clabel(cs, fmt='%g%%', fontsize=6, inline=True)
@@ -835,16 +992,17 @@
     # Plot injection location if injection is present
     ax.plot(np.degrees(RA), np.degrees(declination),
         transform=ax.get_transform('world'),
         marker=ligo.skymap.plot.reticle(),
         markersize=30,
         markeredgewidth=3)
 
+    return ax
     
-def skymap_plugin(alpha = 0.75, beta=0.128, sigma = 64*1024, nside =64, window_parameter = None, injection = False):
+def skymap_plugin(alpha = None, beta=None, sigma = None, nside =None, window_parameter = None, injection = False):
 
     if injection:
 
         return PlugIn('sky_map', genFunction=skymap_gen_function , attributes= ['strain','fs', 'uwstrain', 'psd', 'gps', 'detectors','PE'],
                         plotFunction=skymap_plot_function_with_inj, plotAttributes=['strain','RA','declination'], alpha = alpha, beta = beta, sigma = sigma, nside = nside, window_parameter = window_parameter)
     else:
```

### Comparing `mly-1.0.0/mly/tests/README.md` & `mly-1.0.3/mly/tests/README.md`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/tests/__init__.py` & `mly-1.0.3/mly/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/tests/test_init.py` & `mly-1.0.3/mly/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/tests/test_tools.py` & `mly-1.0.3/mly/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/tools.py` & `mly-1.0.3/mly/tools.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/validators.py` & `mly-1.0.3/mly/validators.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly/waveforms.py` & `mly-1.0.3/mly/waveforms.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/mly.egg-info/PKG-INFO` & `mly-1.0.3/mly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly
-Version: 1.0.0
+Version: 1.0.3
 Summary: Toolkit package to run GW search using ML.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly-1.0.0/mly.egg-info/SOURCES.txt` & `mly-1.0.3/mly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/pages/docs/Makefile` & `mly-1.0.3/pages/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/pages/docs/make.bat` & `mly-1.0.3/pages/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/pages/docs/source/GeneratorTutorial.ipynb` & `mly-1.0.3/pages/docs/source/GeneratorTutorial.ipynb`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/pages/docs/source/conf.py` & `mly-1.0.3/pages/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/pages/docs/source/index.rst` & `mly-1.0.3/pages/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/pages/docs/source/mly.rst` & `mly-1.0.3/pages/docs/source/mly.rst`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/pages/docs/source/timeseriesexample.png` & `mly-1.0.3/pages/docs/source/timeseriesexample.png`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/pages/docs/source/tutorials.generator.rst` & `mly-1.0.3/pages/docs/source/tutorials.generator.rst`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/pages/docs/source/tutorials.rst` & `mly-1.0.3/pages/docs/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `mly-1.0.0/pyproject.toml` & `mly-1.0.3/pyproject.toml`

 * *Files identical despite different names*

