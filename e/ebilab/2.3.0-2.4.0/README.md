# Comparing `tmp/ebilab-2.3.0.tar.gz` & `tmp/ebilab-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebilab-2.3.0.tar", last modified: Thu Apr 20 10:22:58 2023, max compression
+gzip compressed data, was "ebilab-2.4.0.tar", last modified: Thu Apr 11 10:04:27 2024, max compression
```

## Comparing `ebilab-2.3.0.tar` & `ebilab-2.4.0.tar`

### file list

```diff
@@ -1,111 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.885872 ebilab-2.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 10:22:43.000000 ebilab-2.3.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-20 10:22:43.000000 ebilab-2.3.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-20 10:22:43.000000 ebilab-2.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 10:22:43.000000 ebilab-2.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 10:22:43.000000 ebilab-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 10:22:43.000000 ebilab-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-20 10:22:43.000000 ebilab-2.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 10:22:58.893872 ebilab-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-20 10:22:43.000000 ebilab-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/ebilab.analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/ebilab.experiment.devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/ebilab.experiment.devices.visa.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/ebilab.experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/ebilab.project.rst
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/ebilab.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/changelog-v2.0.0-pre.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.885872 ebilab-2.3.0/docs/source/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.885872 ebilab-2.3.0/docs/source/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12691 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/api.po
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/changelog.po
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/index.po
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/installation.po
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/modules.po
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/tutorial.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/docs/source/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/tutorial/analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/tutorial/experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/tutorial/experiment_device.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/tutorial/version.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/ebilab/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/analysis/_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/analysis/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/analysis/_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.885872 ebilab-2.3.0/ebilab/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/data/project-template/
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.885872 ebilab-2.3.0/ebilab/data/project-template/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/data/project-template/data/input/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/data/input/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/data/project-template/data/original/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/data/original/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/data/project-template/data/output/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/data/output/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/data/project-template/data/plot/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/data/plot/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/ebilab.ini
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/_experiment_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    20758 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/_ui_tkinter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/experiment/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/experiment/devices/_visa/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/devices/_visa/A707.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/devices/_visa/E4980.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/devices/_visa/K34411A.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/devices/_visa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/devices/visa.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 10:22:58.000000 ebilab-2.3.0/ebilab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-20 10:22:58.000000 ebilab-2.3.0/ebilab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:22:58.000000 ebilab-2.3.0/ebilab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 10:22:58.000000 ebilab-2.3.0/ebilab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 10:22:58.000000 ebilab-2.3.0/ebilab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 10:22:58.000000 ebilab-2.3.0/ebilab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 10:22:43.000000 ebilab-2.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/sample/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 10:22:43.000000 ebilab-2.3.0/sample/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 10:22:43.000000 ebilab-2.3.0/sample/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-20 10:22:43.000000 ebilab-2.3.0/sample/cont_r.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-20 10:22:43.000000 ebilab-2.3.0/sample/multimeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-20 10:22:43.000000 ebilab-2.3.0/sample/random-walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-20 10:22:43.000000 ebilab-2.3.0/sample/voltage.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:22:58.893872 ebilab-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-20 10:22:43.000000 ebilab-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/tests/sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/tests/sample/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/tests/sample/data/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/tests/sample/data/input/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/tests/sample/data/original/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/tests/sample/data/original/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/tests/sample/data/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/tests/sample/data/output/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/tests/sample/ebilab.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/tests/sample/other_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/tests/sample/other_dir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-20 10:22:43.000000 ebilab-2.3.0/tests/test_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.055173 ebilab-2.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.063173 ebilab-2.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-11 10:04:17.000000 ebilab-2.4.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-11 10:04:17.000000 ebilab-2.4.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-11 10:04:17.000000 ebilab-2.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-11 10:04:17.000000 ebilab-2.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-11 10:04:17.000000 ebilab-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-11 10:04:17.000000 ebilab-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-11 10:04:17.000000 ebilab-2.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-11 10:04:27.075173 ebilab-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-11 10:04:17.000000 ebilab-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.063173 ebilab-2.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.063173 ebilab-2.4.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.063173 ebilab-2.4.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/ebilab.analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/ebilab.experiment.devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/ebilab.experiment.devices.visa.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/ebilab.experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/ebilab.project.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/ebilab.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/changelog-v2.0.0-pre.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.059173 ebilab-2.4.0/docs/source/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.059173 ebilab-2.4.0/docs/source/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.067173 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/api.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/changelog.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/index.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/installation.po
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/modules.po
+-rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/tutorial.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.067173 ebilab-2.4.0/docs/source/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/tutorial/analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/tutorial/experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/tutorial/experiment_device.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/tutorial/version.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.067173 ebilab-2.4.0/ebilab/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.067173 ebilab-2.4.0/ebilab/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/analysis/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/analysis/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/analysis/_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.059173 ebilab-2.4.0/ebilab/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/data/project-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.059173 ebilab-2.4.0/ebilab/data/project-template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/data/project-template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/data/input/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/data/project-template/data/original/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/data/original/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/data/project-template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/data/output/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/data/project-template/data/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/data/plot/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/ebilab.ini
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/_experiment_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/_ui_tkinter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/experiment/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/experiment/devices/_visa/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/devices/_visa/A707.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/devices/_visa/E4980.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/devices/_visa/K34411A.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/devices/_visa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/devices/visa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/ebilab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-11 10:04:26.000000 ebilab-2.4.0/ebilab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-11 10:04:27.000000 ebilab-2.4.0/ebilab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:04:26.000000 ebilab-2.4.0/ebilab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 10:04:26.000000 ebilab-2.4.0/ebilab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 10:04:26.000000 ebilab-2.4.0/ebilab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 10:04:26.000000 ebilab-2.4.0/ebilab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 10:04:17.000000 ebilab-2.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/cont_r.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/multimeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/random-walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/sample/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/recipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/recipes/do-nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/recipes/random-walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/voltage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 10:04:27.075173 ebilab-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-11 10:04:17.000000 ebilab-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/tests/sample/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.059173 ebilab-2.4.0/tests/sample/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/tests/sample/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/tests/sample/data/input/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/tests/sample/data/original/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/tests/sample/data/original/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/tests/sample/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/tests/sample/data/output/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/tests/sample/ebilab.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/tests/sample/other_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/tests/sample/other_dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-11 10:04:17.000000 ebilab-2.4.0/tests/test_paths.py
```

### Comparing `ebilab-2.3.0/.gitignore` & `ebilab-2.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/LICENSE` & `ebilab-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/README.md` & `ebilab-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/Makefile` & `ebilab-2.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/make.bat` & `ebilab-2.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/api/ebilab.analysis.rst` & `ebilab-2.4.0/docs/source/api/ebilab.analysis.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/changelog-v2.0.0-pre.rst` & `ebilab-2.4.0/docs/source/changelog-v2.0.0-pre.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/changelog.rst` & `ebilab-2.4.0/docs/source/changelog.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,33 @@
 ####################
 更新履歴
 ####################
 
 **************************
+v2.4.0 (Apr 11, 2024)
+**************************
+
+Features
+=====================
+
+* experiment discovery 機能を追加しました。
+  * 特定のフォルダを指定することで、そのフォルダに含まれる実験ファイルを自動で認識してウィンドウが起動します。
+  * `python -m ebilab experiment <directory>` にて実行が可能です。
+* `ebilab.experiment` で起動するウィンドウのレイアウトを変更しました。
+  * タブを活用することで、各種情報をより広いスペースで閲覧することができるようになりました。
+* `ExperimentProtocol` をまとめる `ExperimentGroup` を追加しました。
+* `ExperimentProtocol` の `register_plotter` にて、 `plotter_classes` を登録できるようにしました。
+* `ebilab.experiment` で起動するウィンドウにアイコンを追加しました。
+
+Bug fixes
+=====================
+
+* gitがインストールされていない環境で、gitを利用しないにも関わらずエラーとなるバグを修正しました。
+
+**************************
 v2.3.0 (Apr 20, 2023)
 **************************
 
 Features
 =====================
 
 * ebilab.experimentのOptionFieldにおいて、 `IntField` と `StrField` を追加しました。 (`#7 <https://github.com/ebiyuu1121/ebilab/pull/7/>`_)
```

### Comparing `ebilab-2.3.0/docs/source/conf.py` & `ebilab-2.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/index.rst` & `ebilab-2.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/installation.rst` & `ebilab-2.4.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/api.po` & `ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/api.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/changelog.po` & `ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/changelog.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/index.po` & `ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/installation.po` & `ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/installation.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/modules.po` & `ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/modules.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/tutorial.po` & `ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/tutorial.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/tutorial/analysis.rst` & `ebilab-2.4.0/docs/source/tutorial/analysis.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/tutorial/experiment.rst` & `ebilab-2.4.0/docs/source/tutorial/experiment.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/tutorial/experiment_device.rst` & `ebilab-2.4.0/docs/source/tutorial/experiment_device.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/docs/source/tutorial/version.rst` & `ebilab-2.4.0/docs/source/tutorial/version.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/ebilab/__init__.py` & `ebilab-2.4.0/ebilab/__init__.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/ebilab/analysis/_actions.py` & `ebilab-2.4.0/ebilab/analysis/_actions.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/ebilab/analysis/_preprocess.py` & `ebilab-2.4.0/ebilab/analysis/_preprocess.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/ebilab/analysis/_process.py` & `ebilab-2.4.0/ebilab/analysis/_process.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,32 @@
 
 import re
 import os
 from pathlib import Path
 from typing import Union, List
 
 import pandas as pd
+import matplotlib.pyplot as plt
 
 from ebilab.project import get_current_project
 from ._actions import DfAction, DfPlotter, AggregatedDfPlotter
 
 class ProcessingData:
     _df: pd.DataFrame
     _key: str
     _use_cache = True
+    _plot_ctx: dict
+    _plot_ctx_label = ""
+
     def __init__(self, df: pd.DataFrame, key: str, *, save=True):
         self._df = df
         self._key = key
         if save:
             self._save()
+        self._plot_ctx = {}
 
     def apply(self, action: DfAction):
         self._key += "__" + action.key
         cache = self._load_csv()
         if cache is None:
             self._df = action.handler(self._df)
             self._save()
@@ -61,56 +66,71 @@
         dir = get_current_project().path.data_output
         self._df.to_csv(dir / (self._key + ".csv"), index=False)
         return self
 
     def plot(self, plotter: DfPlotter):
 
         dir = get_current_project().path.data_plot
-        filename = dir / (self._key + "__" + plotter.key + ".png")
+        filename = dir / (self._key + "__" + plotter.key + self._plot_ctx_label + ".png")
 
         # cache
         if self._use_cache and filename.exists():
             if os.environ.get("EBILAB_SOURCE") != "WATCH":
                 print(f"Plot already exists: {filename.name}")
         else:
-            plotter.handler(self._df, filename)
+            with plt.rc_context(self._plot_ctx):
+                plotter.handler(self._df, filename)
             print(f"Saved plot: {filename.name}")
 
         return self
 
+    def plot_context(self, label, ctx: dict):
+        self._plot_ctx.update(ctx)
+        self._plot_ctx_label += "-" + label
+        return self
+
     def __del__(self):
         # ここでplt.closeすると show() メソッドが作れるかも
         pass
 
     @classmethod
     def fromCsv(cls, filename: Union[str, Path]):
         path = Path(filename)
         df = pd.read_csv(path)
         return cls(df, path.stem, save=False)
 
 class AggregatedProcessingData:
     _dfs: List[pd.DataFrame]
     _keys: List[str]
     _use_cache = True
+    _plot_ctx: dict
+    _plot_ctx_label = ""
 
     def __init__(self, data: List[ProcessingData]):
         self._dfs = list(map(lambda d:d._df, data))
         self._keys = list(map(lambda d:d._key, data))
         self._use_cache = all(map(lambda d:d._use_cache, data))
+        self._plot_ctx = {}
+
+    def plot_context(self, label, ctx: dict):
+        self._plot_ctx.update(ctx)
+        self._plot_ctx_label += "-" + label
+        return self
 
     def plot(self, plotter: AggregatedDfPlotter):
         dir = get_current_project().path.data_plot
-        filename = dir / (f"[{','.join(self._keys)}]__{plotter.key}.png")
+        filename = dir / (f"[{','.join(self._keys)}]__{plotter.key}{self._plot_ctx_label}.png")
 
         # cache
         if self._use_cache and filename.exists():
             if os.environ.get("EBILAB_SOURCE") != "WATCH":
                 print(f"Plot already exists: {filename.name}")
         else:
-            plotter.handler(self._dfs, filename)
+            with plt.rc_context(self._plot_ctx):
+                plotter.handler(self._dfs, filename)
             print(f"Saved plot: {filename.name}")
 
         return self  
 
     def combine(self, varname: str, values: list):
         dfs_copy = [df.copy() for df in self._dfs]
         for df, val in zip(dfs_copy, values):
```

### Comparing `ebilab-2.3.0/ebilab/data/project-template/.gitignore` & `ebilab-2.4.0/ebilab/data/project-template/.gitignore`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/ebilab/experiment/_experiment_controller.py` & `ebilab-2.4.0/ebilab/experiment/_experiment_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,22 +84,34 @@
     @abc.abstractmethod
     def update(self, df, ctx: PlotterContext):
         raise NotImplementedError()
 
 class ExperimentProtocol(metaclass=abc.ABCMeta):
     name: str
     columns: List[str]
-    plotter_classes: List[Type[ExperimentPlotter]]
+    plotter_classes: List[Type[ExperimentPlotter]] = None
 
     options: Optional[Dict[str, OptionField]] = None
 
     @abc.abstractmethod
     def steps(self, ctx: ExperimentContext) -> None:
         raise NotImplementedError()
 
+    @classmethod
+    def register_plotter(cls, plotter):
+        if cls.plotter_classes is None:
+            cls.plotter_classes = []
+        cls.plotter_classes.append(plotter)
+
+@dataclasses.dataclass(frozen=True)
+class ExperimentProtocolGroup:
+    name: str
+    protocols: List[Type[ExperimentProtocol]]
+
+
 class ExperimentUIDelegate(metaclass=abc.ABCMeta):
     # UI -> Coreの操作
     @abc.abstractmethod
     def handle_ui_start(self, experiment_index: int):
         raise NotImplementedError
 
     @abc.abstractmethod
@@ -143,25 +155,37 @@
     def get_options(self) -> dict:
         raise NotImplementedError()
 
     @property
     def experiment_label(self) -> str:
         raise NotImplementedError()
 
+def prepare_experiments(experiments):
+    for experiment in experiments:
+        if isinstance(experiment, ExperimentProtocolGroup):
+            prepare_experiments(experiment.protocols)
+            continue
+
+        if experiment.plotter_classes is None:
+            experiment.plotter_classes = []
+
 class ExperimentController(ExperimentContextDelegate, ExperimentUIDelegate):
     _experiments: List[Type[ExperimentProtocol]]
     _ui: IExperimentUI
     _ctx: ExperimentContext
     _running = False
     _file = None
     _log_file = None
 
     _experiment_thread = None
 
     def __init__(self, *, experiments: List[Type[ExperimentProtocol]], ui: IExperimentUI):
+        # fix plotter_classes in experiments
+        prepare_experiments(experiments)
+
         self._experiments = experiments
 
         self._ui = ui
         self._ui.delegate = self
         self._ui.experiments = experiments
 
     def launch(self):
@@ -179,21 +203,20 @@
 
         comment_str = ""
         comment_str += f"# {exp_name} experiment: Ran at {date} in {pc_name}\n"
         comment_str += f"# {options_str}\n"
         comment_str += f"#\n"
         return comment_str
 
-    def _run(self, experiment_index: int):
+    def _run(self, experiment: Type[ExperimentProtocol]):
         logger.info(f"starting experiment")
 
         self._ui.update_state("running")
 
-        self._running_experiment_idx = experiment_index
-        self._running_experiment_class = self._experiments[experiment_index]
+        self._running_experiment_class = experiment
         self._running_experiment = self._running_experiment_class()
 
         self._ui.reset_data()
 
         self._options = self._ui.get_options()
 
         self._ctx = ExperimentContext(delegate=self)
@@ -293,16 +316,16 @@
         return self._options
 
     def experiment_ctx_delegate_loop(self) -> None:
         if not self._running:
             sys.exit()
 
     # ExperimentUIDelegate
-    def handle_ui_start(self, experiment_index: int):
-        self._run(experiment_index)
+    def handle_ui_start(self, experiment: Type[ExperimentProtocol]):
+        self._run(experiment)
 
     def handle_ui_stop(self):
         self._stop()
 
     def __del__(self):
         if self._file is not None:
             self._file.close()
```

### Comparing `ebilab-2.3.0/ebilab/experiment/_ui_tkinter.py` & `ebilab-2.4.0/ebilab/experiment/_ui_tkinter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,80 @@
 from logging import getLogger
 import queue
 import time
+from pathlib import Path
 from typing import List, Optional, Type, Dict
 import tkinter as tk
 from tkinter import ttk
 import tkinter.font as tkf
 
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 
-from ._experiment_controller import ExperimentPlotter, IExperimentUI, ExperimentProtocol, PlotterContext
+from ._experiment_controller import ExperimentPlotter, IExperimentUI, ExperimentProtocol, PlotterContext, ExperimentProtocolGroup
 from .options import OptionField, FloatField, SelectField, IntField, StrField
 
 logger = getLogger(__name__)
 
 # windows dpi workaround
 try:
     import ctypes
     ctypes.windll.shcore.SetProcessDpiAwareness(2) 
 except:
     try:
         ctypes.windll.user32.SetProcessDPIAware()
     except:
         pass
 
+class ProtocolTree(ttk.Treeview):
+    def __init__(self, master):
+        super().__init__(master, padding=10, selectmode="browse")
+        self.bind("<<TreeviewSelect>>", self._on_change)
+        self.experiments = []
+
+    def update_experiments(self, experiments):
+        """
+        Update protocol list (tree)
+        """
+        self._insert_experiments("", experiments, "")
+        self.experiments = experiments
+
+    def _insert_experiments(self, parent, experiments, key):
+        for i, experiment in enumerate(experiments):
+            new_key = f"{key}.{i}"
+            if isinstance(experiment, ExperimentProtocolGroup):
+                id = self.insert(parent, "end", text=experiment.name, iid=new_key, open=True)
+                self._insert_experiments(id, experiment.protocols, new_key)
+                continue
+            else:
+                self.insert(parent, "end", text=experiment.name, iid=new_key)
+
+    def _on_change(self, *args, **kwargs):
+        self.event_generate("<<ExperimentChange>>")
+
+    def _get_experiment_from_list(self, experiments, ids):
+        for i in ids:
+            experiment = experiments[int(i)]
+            if not isinstance(experiment, ExperimentProtocolGroup):
+                return experiment
+            experiments = experiment.protocols
+        return None
+
+    @property
+    def selected_experiment(self):
+        """
+        Active experiment
+        """
+        selection = self.selection()
+        if len(selection) == 0:
+            return None
+        ids = selection[0].split(".")
+        return self._get_experiment_from_list(self.experiments, ids[1:])
+
 class OptionsPane(ttk.Frame):
     __label: str
     __fields: Dict[str, OptionField]
     __enabled = True
     __options: dict
     __is_valid = True
 
@@ -204,117 +250,116 @@
         else:
             for widget in self._options_widget:
                 widget["state"] = "disabled"
 
 class ExperimentUITkinter(IExperimentUI):
     _data_queue: queue.Queue
     log_queue: queue.Queue
+    _log_cnt = 0
 
     _state: str = "stopped"
     _plotter: Optional[ExperimentPlotter] = None
     _update_experiment_loop_id: Optional[str] = None
     _protocol_options_pane: OptionsPane
     _plotter_options_pane: OptionsPane
 
     def __init__(self) -> None:
         super().__init__()
 
     def _create_ui(self):
         self._root = tk.Tk()
+        self._root.iconbitmap(default=str(Path(__file__).parent.parent / "icon.ico"))
         self._root.state("zoomed")
-        self._root.columnconfigure(0, weight=1)
         self._root.rowconfigure(0, weight=1)
+        self._root.columnconfigure(0, minsize=300)
+        self._root.columnconfigure(1, weight=1)
 
-        frm = ttk.Frame(self._root, padding=10, relief="solid")
-        frm.grid(sticky="nsew")
-        frm.columnconfigure(0, weight=1)
-        frm.rowconfigure(1, weight=1)
-        frm.rowconfigure(2, weight=1)
-        frm.rowconfigure(3, weight=1)
-
-        ctrl_frm = ttk.Frame(frm, padding=10, relief="solid")
-        ctrl_frm.grid(column=0, row=0, sticky="new")
-        ctrl_frm.rowconfigure(0, weight=1)
-        ctrl_frm.columnconfigure(0, weight=1)
-        ctrl_frm.columnconfigure(1, weight=1)
-        ctrl_frm.columnconfigure(2, weight=1)
-        ctrl_frm.columnconfigure(3, weight=1)
-
-        experiment_list_pane = ttk.Frame(ctrl_frm, padding=10, relief="solid")
-        experiment_list_pane.grid(column=0, row=0, sticky=tk.NSEW)
-        experiment_list_pane.columnconfigure(0, weight=1)
-        experiment_list_pane.rowconfigure(1, weight=1)
-        tk.Label(experiment_list_pane, justify="center", text="Experiment List").grid(column=0, row=0, sticky=tk.N)
-
-        self._experiment_list_var = tk.StringVar(value=[])
-        self._experiment_list = tk.Listbox(experiment_list_pane, listvariable=self._experiment_list_var, exportselection=False, height=5)
-        self._experiment_list.grid(column=0, row=1, sticky=tk.NSEW)
-        self._experiment_list.bind("<<ListboxSelect>>", self._handle_experiment_change)
-
-        # options pane
-        self._protocol_options_pane = OptionsPane(ctrl_frm, "Experiment options")
-        self._protocol_options_pane.grid(column=1, row=0, sticky=tk.NSEW)
-
-        plotter_list_pane = ttk.Frame(ctrl_frm, padding=10, relief="solid")
-        plotter_list_pane.grid(column=2, row=0, sticky=tk.NSEW)
-        plotter_list_pane.columnconfigure(0, weight=1)
-        plotter_list_pane.rowconfigure(1, weight=1)
-        tk.Label(plotter_list_pane, justify="center", text="Plotter List").grid(column=0, row=0, sticky=tk.N)
-
-        self._plotter_list_var = tk.StringVar(value=[])
-        self._plotter_list = tk.Listbox(plotter_list_pane, listvariable=self._plotter_list_var, exportselection=False, height=5)
-        self._plotter_list.grid(column=0, row=1, sticky=tk.NSEW)
-        self._plotter_list.bind("<<ListboxSelect>>", self._handle_plotter_change)
-
-        # options pane
-        self._plotter_options_pane = OptionsPane(ctrl_frm, "Plot options")
-        self._plotter_options_pane.grid(column=3, row=0, sticky=tk.NSEW)
-
-        buttons_pane = ttk.Frame(ctrl_frm, padding=10, relief="solid")
-        buttons_pane.grid(column=4, row=0, sticky="nes")
+        # frames
+        sidebar_frm = ttk.Frame(self._root, padding=10, relief="solid")
+        sidebar_frm.grid(row=0, column=0, sticky=tk.NSEW)
+        main_frm = ttk.Frame(self._root, padding=10, relief="solid")
+        main_frm.grid(row=0, column=1, sticky=tk.NSEW)
+
+        # experiment list pane
+        experiment_list_pane = ttk.Frame(sidebar_frm, padding=10, relief="solid")
+        experiment_list_pane.pack(side=tk.TOP, fill=tk.BOTH, expand=True)
+
+        tk.Label(experiment_list_pane, justify="center", text="Experiments") \
+            .pack(side=tk.TOP, fill=tk.Y, expand=False)
+
+        self._protocol_tree = ProtocolTree(experiment_list_pane)
+        self._protocol_tree.pack(side=tk.TOP, fill=tk.BOTH, expand=True)
+        self._protocol_tree.bind("<<ExperimentChange>>", self._handle_experiment_change)
+
+        # plotter options pane
+        self._protocol_options_pane = OptionsPane(sidebar_frm, "Experiment options")
+        self._protocol_options_pane.pack(side=tk.TOP, fill=tk.BOTH, expand=True)
+
+        # buttons pane
+        buttons_pane = ttk.Frame(sidebar_frm, padding=10, relief="solid")
+        buttons_pane.pack(side=tk.TOP, fill=tk.BOTH)
 
         self._experiment_label_var = tk.StringVar(value="")
         self._experiment_label_var.trace("w", self._validate_options_and_update_ui)
-        tk.Label(buttons_pane, justify=tk.LEFT, text="Filename:").grid(column=0, row=0, sticky=tk.W)
+        tk.Label(buttons_pane, justify=tk.LEFT, text="Filename:") \
+            .pack(side=tk.TOP, fill=tk.X, expand=False)
         self._experiment_label_entry = tk.Entry(buttons_pane, textvariable=self._experiment_label_var)
-        self._experiment_label_entry.grid(column=0, row=1)
+        self._experiment_label_entry.pack(side=tk.TOP, fill=tk.X, expand=False)
 
         self._start_button = ttk.Button(buttons_pane, text="Start", command=self._handle_start_experiment, state="disabled")
-        self._start_button.grid(column=0, row=2)
+        self._start_button.pack(side=tk.TOP, fill=tk.X, expand=False)
         self._stop_button = ttk.Button(buttons_pane, text="Stop", command=self._handle_stop_experiment, state="disabled")
-        self._stop_button.grid(column=0, row=3)
+        self._stop_button.pack(side=tk.TOP, fill=tk.X, expand=False)
         self._quit_button = ttk.Button(buttons_pane, text="Quit", command=self._handle_quit)
-        self._quit_button.grid(column=0, row=4)
+        self._quit_button.pack(side=tk.TOP, fill=tk.X, expand=False)
+
+        self._plotter_nb = ttk.Notebook(main_frm)
+        tab1 = tk.Frame(self._plotter_nb)
+        self._plotter_nb.pack(side=tk.TOP, fill=tk.BOTH)
+
+        # タブに表示する文字列の設定
+        self._plotter_nb.add(tab1, text='-')
+        self._plotter_nb.bind("<<NotebookTabChanged>>", self._handle_plotter_change)
+
+
+        # plot range
+        plot_frm = ttk.Frame(main_frm, padding=10, relief="solid")
+        plot_frm.pack(side=tk.TOP, fill=tk.BOTH, expand=True)
 
-        plot_frm = ttk.Frame(frm, padding=10, relief="solid")
-        plot_frm.grid(column=0, row=1, sticky=tk.NSEW)
-        plot_frm.columnconfigure(0, weight=1)
         plot_frm.rowconfigure(0, weight=1)
+        plot_frm.columnconfigure(0, weight=1)
+        plot_frm.columnconfigure(1, minsize=300)
 
         self._fig = plt.figure(figsize=(6, 3), dpi=100, constrained_layout=True)
         self._canvas = FigureCanvasTkAgg(self._fig, master=plot_frm)
-        self._canvas.get_tk_widget().grid(column=0, row=0, sticky=tk.NSEW)
+        self._canvas.get_tk_widget().grid(row=0, column=0, sticky=tk.NSEW)
+
+        # plotter options pane
+        self._plotter_options_pane = OptionsPane(plot_frm, "Plot options")
+        self._plotter_options_pane.grid(row=0, column=1, sticky=tk.NSEW)
+
+        # bottom notebook
+        self._bottom_nb = ttk.Notebook(main_frm)
+        self._bottom_nb.pack(side=tk.TOP, fill=tk.BOTH, expand=True)
+
+        table_frm = ttk.Frame(self._bottom_nb, padding=10)
+        table_frm.pack(side=tk.LEFT, fill=tk.BOTH, expand=True)
+        log_frm = ttk.Frame(self._bottom_nb, padding=10)
+        log_frm.pack(side=tk.LEFT, fill=tk.BOTH, expand=True)
 
-        table_frm = ttk.Frame(frm, padding=10, relief="solid")
-        table_frm.grid(column=0, row=2, sticky="wes")
-        table_frm.columnconfigure(0, weight=1)
-        table_frm.rowconfigure(0, weight=1)
+        self._bottom_nb.add(table_frm, text="Result")
+        self._bottom_nb.add(log_frm, text="Log")
 
         self._result_tree = ttk.Treeview(table_frm)
         self._result_tree.column("#0", width=0)
-        self._result_tree.grid(row=0, column=0, sticky=tk.NSEW)
-
-        log_frm = ttk.Frame(frm, padding=10, relief="solid")
-        log_frm.grid(column=0, row=3, sticky="wes")
-        log_frm.columnconfigure(0, weight=1)
-        log_frm.rowconfigure(0, weight=1)
+        self._result_tree.pack(side=tk.TOP, fill=tk.BOTH, expand=True)
 
         self._log_tree = ttk.Treeview(log_frm)
+        self._log_tree.pack(side=tk.TOP, fill=tk.BOTH, expand=True) 
         self._log_tree.column("#0", width=0, stretch=False)
-        self._log_tree.grid(row=0, column=0, sticky=tk.NSEW)
         self._log_tree["columns"] = ["t", "time", "message"]
         self._log_tree.heading("message", text="message")
         self._log_tree.heading("time", text="time")
         self._log_tree.column("time", width=100, stretch=False)
         self._log_tree.heading("t", text="t")
         self._log_tree.column("t", width=150, stretch=False)
 
@@ -324,75 +369,79 @@
 
     def _handle_quit(self):
         if self._update_experiment_loop_id is not None:
             self._root.after_cancel(self._update_experiment_loop_id)
         self._root.quit()
         self._root.destroy()
 
-    def _get_current_experiment(self) -> Type[ExperimentProtocol]:
-        idx = self._experiment_list.curselection()[0]
-        return self.experiments[idx]
-
     def _handle_experiment_change(self, _):
-        if not self._experiment_list.curselection():
+        experiment = self._protocol_tree.selected_experiment
+        if not experiment:
             return
 
         self.reset_data()
 
-        idx = self._experiment_list.curselection()[0]
-        self._plotter_list_var.set(list(map(lambda cls:cls.name, self.experiments[idx].plotter_classes)))
-        self._plotter_list.select_clear(0, tk.END)
-        self._plotter_list.selection_set(0)
+        # update plotter list (tab)
+        for tab in self._plotter_nb.tabs():
+            self._plotter_nb.forget(tab)
+        for name in map(lambda cls:cls.name, experiment.plotter_classes):
+            tab = tk.Frame(self._plotter_nb)
+            self._plotter_nb.add(tab, text=name)
+        if len(experiment.plotter_classes) == 0:
+            tab = tk.Frame(self._plotter_nb)
+            self._plotter_nb.add(tab, text="-")
+
         self._handle_plotter_change()
 
         # update cols
-        Experiment = self.experiments[idx]
-        columns = ["t", "time"] + Experiment.columns
+        columns = ["t", "time"] + experiment.columns
         self._result_tree["columns"] = columns
         self._result_tree.column("#0", width=0, stretch=False)
         self._result_tree.heading("time", text="time")
         self._result_tree.column("time", width=100, stretch=False)
         self._result_tree.heading("t", text="t")
         self._result_tree.column("t", width=150, stretch=False)
 
         for col in columns[2:]:
             self._result_tree.heading(col, text=col)
             self._result_tree.column(col, minwidth=100, anchor='center', stretch=True)
 
 
-        self._experiment_label_var.set(Experiment.name)
+        self._experiment_label_var.set(experiment.name)
 
-        self._protocol_options_pane.fields = Experiment.options or {}
+        self._protocol_options_pane.fields = experiment.options or {}
 
         self._validate_options_and_update_ui()
+        self._update_ui_from_state()
 
     def _validate_options_and_update_ui(self, *_):
         if self._state != "stopped":
             return
         if self._protocol_options_pane.is_valid and self._experiment_label_var.get() != "":
             self._start_button["state"] = "normal"
         else:
             self._start_button["state"] = "disabled"
 
     def _handle_plotter_change(self, *args, **kwargs):
         try:
-            exp_idx = self._experiment_list.curselection()[0]
-            Experiment = self.experiments[exp_idx]
-            plotter_idx = self._plotter_list.curselection()[0]
-            Plotter = Experiment.plotter_classes[plotter_idx]
+            experiment = self._protocol_tree.selected_experiment
+            if experiment is None:
+                return
+            plotter_idx = self._plotter_nb.index(self._plotter_nb.select())
+            Plotter = experiment.plotter_classes[plotter_idx]
         except IndexError:
             return
         self._plotter_options_pane.fields = Plotter.options or {}
         self._reset_plotter()
 
     def launch(self):
         self._create_ui()
 
         # insert data
-        self._experiment_list_var.set(list(map(lambda cls:cls.name, self.experiments)))
+        self._protocol_tree.update_experiments(self.experiments)
 
         self._update_experiment_loop_id = self._root.after(30, self._update_experiment_loop)
         self._root.mainloop()
 
     def _get_data_from_queue(self, queue_):
         d = []
         while True:
@@ -405,16 +454,16 @@
         self._update_ui_from_state()
         if self._state != "stopped":
             data = self._get_data_from_queue(self._data_queue)
 
             for d in data:
                 self._data.append(d)
 
-                experiment_idx = self._experiment_list.curselection()[0]
-                columns = self.experiments[experiment_idx].columns
+                experiment = self._protocol_tree.selected_experiment
+                columns = experiment.columns
 
                 # insert to table
                 row_list = [str(d["t"]), str(d["time"])]
                 for col in columns:
                     if col in d:
                         row_list.append(str(d[col]))
                     else:
@@ -424,30 +473,31 @@
             self._draw_plot()
 
             # update logs
             logs = self._get_data_from_queue(self.log_queue)
             for log in logs:
                 self._log_tree.insert("", tk.END, values=[log["t"], log["time"], log["message"]])
                 self._log_tree.yview_moveto(1)
+                self._log_cnt += 1
+                self._bottom_nb.tab(1, text=f"Log ({self._log_cnt})")
 
         self._update_experiment_loop_id = self._root.after(30, self._update_experiment_loop)
 
     def _draw_plot(self):
         if len(self._data) > 0 and self._plotter:
             df = pd.DataFrame(self._data)
             time_before_plot = time.perf_counter()
             self._plotter.update(df, self._get_plotter_context())
             logger.debug(f"Plotter.update took {time.perf_counter() - time_before_plot} s")
             time_before_draw = time.perf_counter()
             self._canvas.draw()
             logger.debug(f"canvas.draw took {time.perf_counter() - time_before_draw} s")
 
     def _handle_start_experiment(self):
-        experiment_idx = self._experiment_list.curselection()[0]
-        self.delegate.handle_ui_start(experiment_idx)
+        self.delegate.handle_ui_start(self._protocol_tree.selected_experiment)
 
     def _handle_stop_experiment(self):
         self.delegate.handle_ui_stop()
 
     @property
     def data_queue(self) -> queue.Queue:
         return self._data_queue
@@ -460,54 +510,55 @@
     def _update_ui_from_state(self):
         if self._state == "running":
             self._start_button["state"] = "disabled"
             self._stop_button["state"] = "normal"
             self._quit_button["state"] = "disabled"
             self._stop_button["text"] = "Stop"
             self._experiment_label_entry["state"] = "disabled"
-            self._experiment_list["state"] = "disabled"
+            self._protocol_tree.state(("disabled", ))
             self._protocol_options_pane.enabled = False
         elif self._state == "stopping":
             self._start_button["state"] = "disabled"
             self._stop_button["state"] = "normal"
             self._quit_button["state"] = "normal"
             self._stop_button["text"] = "Stopping..."
             self._experiment_label_entry["state"] = "disabled"
-            self._experiment_list["state"] = "disabled"
+            self._protocol_tree.state(("disabled", ))
             self._protocol_options_pane.enabled = False
         else:
-            if self._experiment_list.curselection():
+            if self._protocol_tree.selected_experiment:
                 self._start_button["state"] = "normal"
                 self._validate_options_and_update_ui()
             else:
                 self._start_button["state"] = "disabled"
             self._experiment_label_entry["state"] = "normal"
-            self._experiment_list["state"] = "normal"
+            self._protocol_tree.state(("!disabled", ))
             self._protocol_options_pane.enabled = True
             self._stop_button["state"] = "disabled"
             self._quit_button["state"] = "enabled"
             self._stop_button["text"] = "Stop"
 
     def update_state(self, state: str):
         self._state = state
 
     def reset_data(self):
         self._data = []
         self._data_queue = queue.Queue()
         self.log_queue = queue.Queue()
+        self._log_cnt = 0
+        self._bottom_nb.tab(1, text=f"Log")
         self._result_tree.delete(*self._result_tree.get_children())
         self._reset_plotter()
 
     def _reset_plotter(self):
         self._fig.clf()
 
         try:
-            exp_idx = self._experiment_list.curselection()[0]
-            Experiment = self.experiments[exp_idx]
-            plotter_idx = self._plotter_list.curselection()[0]
+            Experiment = self._protocol_tree.selected_experiment
+            plotter_idx = self._plotter_nb.index(self._plotter_nb.select())
             Plotter = Experiment.plotter_classes[plotter_idx]
         except IndexError:
             self._plotter = None
             return
 
         self._plotter = Plotter()
         self._plotter.fig = self._fig
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ebilab-2.3.0/ebilab/experiment/devices/_visa/A707.py` & `ebilab-2.4.0/ebilab/experiment/devices/_visa/A707.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/ebilab/experiment/devices/_visa/E4980.py` & `ebilab-2.4.0/ebilab/experiment/devices/_visa/E4980.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/ebilab/experiment/devices/_visa/K34411A.py` & `ebilab-2.4.0/ebilab/experiment/devices/_visa/K34411A.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/ebilab/experiment/devices/visa.py` & `ebilab-2.4.0/ebilab/experiment/devices/visa.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/ebilab/experiment/options.py` & `ebilab-2.4.0/ebilab/experiment/options.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/ebilab/project.py` & `ebilab-2.4.0/ebilab/project.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/ebilab.egg-info/SOURCES.txt` & `ebilab-2.4.0/ebilab.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 docs/source/tutorial/analysis.rst
 docs/source/tutorial/experiment.rst
 docs/source/tutorial/experiment_device.rst
 docs/source/tutorial/version.rst
 ebilab/__init__.py
 ebilab/__main__.py
 ebilab/_cli.py
+ebilab/icon.ico
 ebilab/project.py
 ebilab.egg-info/PKG-INFO
 ebilab.egg-info/SOURCES.txt
 ebilab.egg-info/dependency_links.txt
 ebilab.egg-info/entry_points.txt
 ebilab.egg-info/requires.txt
 ebilab.egg-info/top_level.txt
@@ -66,13 +67,16 @@
 ebilab/experiment/devices/_visa/__init__.py
 sample/.gitignore
 sample/README.md
 sample/cont_r.py
 sample/multimeter.py
 sample/random-walk.py
 sample/voltage.py
+sample/recipes/__init__.py
+sample/recipes/do-nothing.py
+sample/recipes/random-walk.py
 tests/test_paths.py
 tests/sample/ebilab.ini
 tests/sample/data/input/.gitkeep
 tests/sample/data/original/.gitkeep
 tests/sample/data/output/.gitkeep
 tests/sample/other_dir/.gitkeep
```

### Comparing `ebilab-2.3.0/sample/cont_r.py` & `ebilab-2.4.0/sample/cont_r.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/sample/random-walk.py` & `ebilab-2.4.0/sample/recipes/random-walk.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,19 @@
 # sample of GUI app
 import time
 import random
 
 from ebilab.experiment import ExperimentProtocol, ExperimentPlotter, ExperimentContext, PlotterContext, launch_experiment
 from ebilab.experiment.options import FloatField, SelectField
 
-#  class to decide how to plot during experiment
-class MyPlotter(ExperimentPlotter):
-    name = "simple"
-    def prepare(self, ctx: PlotterContext):
-        # this method is executed before starting experiment
-        # e.g. adding Axes to Figure
-        # figure is stored in `self.fig`
-
-        self._ax = self.fig.add_subplot(111)
-
-    def update(self, df, ctx: PlotterContext):
-        # this method is executed many times during experiment
-        # df is pandas.DataFrame which has experiment data
-
-        self._ax.cla()
-
-        self._ax.plot(df["t"], df["v"])
-        self._ax.set_xlabel("Time")
-        self._ax.set_ylabel("Voltage")
-        self._ax.grid()
 
 # class to decide steps of experiment
 class RandomWalkExperiment(ExperimentProtocol):
     columns = ["v", "v2"] # please specify columns to write csv file
     name = "random-walk" # filename is suffixed by datetime
-    plotter_classes = [MyPlotter]
 
     # available in GUI
     options = {
         "initial": FloatField(default=2),
         "step": SelectField(choices=[1, 2, 4], default_index=1),
     }
 
@@ -47,10 +26,53 @@
             ctx.send_row({"v": v})
 
             time.sleep(0.2)
             v += step if random.random() < 0.5 else -step
 
             ctx.loop() # you must run ctx.loop() in every loop
 
-if __name__ == "__main__":
-    launch_experiment([RandomWalkExperiment])
+#  class to decide how to plot during experiment
+@RandomWalkExperiment.register_plotter
+class TransientPlotter(ExperimentPlotter):
+    name = "transient"
+    def prepare(self, ctx: PlotterContext):
+        # this method is executed before starting experiment
+        # e.g. adding Axes to Figure
+        # figure is stored in `self.fig`
+
+        self._ax = self.fig.add_subplot(111)
 
+    def update(self, df, ctx: PlotterContext):
+        # this method is executed many times during experiment
+        # df is pandas.DataFrame which has experiment data
+
+        self._ax.cla()
+
+        self._ax.plot(df["t"], df["v"])
+        self._ax.set_xlabel("Time")
+        self._ax.set_ylabel("Voltage")
+        self._ax.grid()
+
+#  class to decide how to plot during experiment
+@RandomWalkExperiment.register_plotter
+class HistgramPlotter(ExperimentPlotter):
+    name = "histgram"
+    options = {
+        "bins": FloatField(default=10),
+    }
+    def prepare(self, ctx: PlotterContext):
+        # this method is executed before starting experiment
+        # e.g. adding Axes to Figure
+        # figure is stored in `self.fig`
+
+        self._ax = self.fig.add_subplot(111)
+
+    def update(self, df, ctx: PlotterContext):
+        # this method is executed many times during experiment
+        # df is pandas.DataFrame which has experiment data
+
+        self._ax.cla()
+
+        self._ax.hist(df["v"], bins=int(ctx.plotter_options["bins"]))
+        self._ax.set_xlabel("Value")
+        self._ax.set_ylabel("Count")
+        self._ax.grid()
```

### Comparing `ebilab-2.3.0/sample/voltage.py` & `ebilab-2.4.0/sample/voltage.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.3.0/setup.py` & `ebilab-2.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 setup(
     name="ebilab",
     author="Yusuke Ebihara",
     author_email="yusuke@ebihara.me",
     url="https://ebilab.readthedocs.io/",
     description="Python package for my research",
+    long_description_content_type="text/markdown",
     install_requires=[
         "tqdm",
         "numpy",
         "pandas",
         "matplotlib",
         "watchdog",
         "click",
```

### Comparing `ebilab-2.3.0/tests/test_paths.py` & `ebilab-2.4.0/tests/test_paths.py`

 * *Files identical despite different names*

