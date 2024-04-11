# Comparing `tmp/erlab-2.1.0.tar.gz` & `tmp/erlab-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.1.0.tar", last modified: Tue Apr  9 15:36:25 2024, max compression
+gzip compressed data, was "erlab-2.1.1.tar", last modified: Wed Apr 10 12:00:58 2024, max compression
```

## Comparing `erlab-2.1.0.tar` & `erlab-2.1.1.tar`

### file list

```diff
@@ -1,171 +1,174 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.373746 erlab-2.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.329746 erlab-2.1.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.337746 erlab-2.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-09 15:36:19.000000 erlab-2.1.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 root         (0) root         (0)      608 2024-04-09 15:36:19.000000 erlab-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.337746 erlab-2.1.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-09 15:36:19.000000 erlab-2.1.0/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-09 15:36:19.000000 erlab-2.1.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-09 15:36:19.000000 erlab-2.1.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-09 15:36:19.000000 erlab-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      796 2024-04-09 15:36:19.000000 erlab-2.1.0/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   102069 2024-04-09 15:36:21.000000 erlab-2.1.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-04-09 15:36:19.000000 erlab-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    47662 2024-04-09 15:36:25.373746 erlab-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-09 15:36:19.000000 erlab-2.1.0/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     4703 2024-04-09 15:36:19.000000 erlab-2.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.337746 erlab-2.1.0/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      655 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.341746 erlab-2.1.0/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    13912 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    14522 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      265 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.characterization.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     3806 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.349746 erlab-2.1.0/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   996803 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     2665 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.349746 erlab-2.1.0/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2578 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1344 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     2356 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.349746 erlab-2.1.0/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)     1222 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)     7084 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)     5606 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)   379533 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    15761 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-09 15:36:19.000000 erlab-2.1.0/environment.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-09 15:36:19.000000 erlab-2.1.0/environment_apple.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-09 15:36:19.000000 erlab-2.1.0/environment_nogit.yml
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-09 15:36:19.000000 erlab-2.1.0/environment_nogit_mkl.yml
--rw-r--r--   0 root         (0) root         (0)     4637 2024-04-09 15:36:19.000000 erlab-2.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-09 15:36:19.000000 erlab-2.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 15:36:25.373746 erlab-2.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.333746 erlab-2.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.353746 erlab-2.1.0/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-09 15:36:21.000000 erlab-2.1.0/src/erlab/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35543 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/accessors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.353746 erlab-2.1.0/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5514 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.357746 erlab-2.1.0/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      459 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.357746 erlab-2.1.0/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      839 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9632 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     6026 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)     9818 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1168 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    15394 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    17319 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10359 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.357746 erlab-2.1.0/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     2775 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7809 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     8659 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.357746 erlab-2.1.0/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      191 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)     2115 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.361746 erlab-2.1.0/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      540 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13943 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    20867 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    22451 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11371 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)     9458 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/exampledata.py
--rw-r--r--   0 root         (0) root         (0)    19072 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.361746 erlab-2.1.0/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    19391 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.361746 erlab-2.1.0/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52076 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114751 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27081 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    54122 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    13907 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25375 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    15728 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19382 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     3341 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    54144 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.361746 erlab-2.1.0/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     1937 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30408 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6780 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.365746 erlab-2.1.0/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3674 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     7448 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7745 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     6278 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.365746 erlab-2.1.0/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.369746 erlab-2.1.0/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     1858 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29010 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18275 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    32411 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    31070 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.369746 erlab-2.1.0/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.369746 erlab-2.1.0/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    47662 2024-04-09 15:36:25.000000 erlab-2.1.0/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4530 2024-04-09 15:36:25.000000 erlab-2.1.0/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 15:36:25.000000 erlab-2.1.0/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      536 2024-04-09 15:36:25.000000 erlab-2.1.0/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-09 15:36:25.000000 erlab-2.1.0/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.369746 erlab-2.1.0/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-09 15:36:19.000000 erlab-2.1.0/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-04-09 15:36:19.000000 erlab-2.1.0/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-04-09 15:36:19.000000 erlab-2.1.0/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.369746 erlab-2.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_fit_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_fit_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     5228 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_image.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     2419 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.389099 erlab-2.1.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.345099 erlab-2.1.1/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.349099 erlab-2.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-10 12:00:52.000000 erlab-2.1.1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-10 12:00:52.000000 erlab-2.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.349099 erlab-2.1.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-10 12:00:52.000000 erlab-2.1.1/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-10 12:00:52.000000 erlab-2.1.1/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-10 12:00:52.000000 erlab-2.1.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-10 12:00:52.000000 erlab-2.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      796 2024-04-10 12:00:52.000000 erlab-2.1.1/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   103668 2024-04-10 12:00:54.000000 erlab-2.1.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-04-10 12:00:52.000000 erlab-2.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    47662 2024-04-10 12:00:58.389099 erlab-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-10 12:00:52.000000 erlab-2.1.1/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     4703 2024-04-10 12:00:52.000000 erlab-2.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.353099 erlab-2.1.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      655 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.357099 erlab-2.1.1/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    16011 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    14522 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.characterization.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     3806 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.361099 erlab-2.1.1/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   294466 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   291044 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     2665 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.365099 erlab-2.1.1/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2578 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.365099 erlab-2.1.1/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)     1222 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)     5063 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    18148 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)   379543 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    15771 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-10 12:00:52.000000 erlab-2.1.1/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-10 12:00:52.000000 erlab-2.1.1/environment_apple.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-10 12:00:52.000000 erlab-2.1.1/environment_nogit.yml
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-10 12:00:52.000000 erlab-2.1.1/environment_nogit_mkl.yml
+-rw-r--r--   0 root         (0) root         (0)     4373 2024-04-10 12:00:52.000000 erlab-2.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-10 12:00:52.000000 erlab-2.1.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 12:00:58.389099 erlab-2.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.345099 erlab-2.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.365099 erlab-2.1.1/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-10 12:00:54.000000 erlab-2.1.1/src/erlab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35543 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/accessors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.369099 erlab-2.1.1/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.369099 erlab-2.1.1/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      459 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.369099 erlab-2.1.1/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      839 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9632 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     6026 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)     9881 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    15448 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    17325 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10629 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.369099 erlab-2.1.1/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     5401 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8440 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     8658 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.373099 erlab-2.1.1/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.373099 erlab-2.1.1/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13953 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    20867 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    22451 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11443 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)     9458 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)    19072 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.377099 erlab-2.1.1/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    19396 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.377099 erlab-2.1.1/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51945 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114560 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27081 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    54122 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    13907 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25270 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    15835 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     3341 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    54143 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.377099 erlab-2.1.1/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31715 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.377099 erlab-2.1.1/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3667 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7804 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     6559 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.381099 erlab-2.1.1/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.381099 erlab-2.1.1/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29010 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18284 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    32437 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    31070 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.385099 erlab-2.1.1/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.385099 erlab-2.1.1/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    47662 2024-04-10 12:00:58.000000 erlab-2.1.1/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4675 2024-04-10 12:00:58.000000 erlab-2.1.1/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 12:00:58.000000 erlab-2.1.1/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      536 2024-04-10 12:00:58.000000 erlab-2.1.1/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-10 12:00:58.000000 erlab-2.1.1/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.385099 erlab-2.1.1/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-10 12:00:52.000000 erlab-2.1.1/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-10 12:00:52.000000 erlab-2.1.1/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-10 12:00:52.000000 erlab-2.1.1/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.349099 erlab-2.1.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.385099 erlab-2.1.1/tests/analysis/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_fit_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_fit_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_utilities.py
```

### Comparing `erlab-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `erlab-2.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/.github/workflows/pr.yml` & `erlab-2.1.1/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/.github/workflows/release.yml` & `erlab-2.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/.gitignore` & `erlab-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/.pre-commit-config.yaml` & `erlab-2.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/.readthedocs.yaml` & `erlab-2.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/CHANGELOG.md` & `erlab-2.1.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,46 @@
 # CHANGELOG
 
 
 
+## v2.1.1 (2024-04-10)
+
+### Documentation
+
+* (**io**) improve docstrings and user guide ([`8e69abb`](https://github.com/kmnhan/erlabpy/commit/8e69abb37a99818081bf2e03453d64e1b48b16ab))
+
+* update io documentation ([`b0d2d01`](https://github.com/kmnhan/erlabpy/commit/b0d2d01d0dec2ec8180cb5d7da2034900d0d0aba))
+
+* change reference format ([`44e159a`](https://github.com/kmnhan/erlabpy/commit/44e159af6102f42182e4f705c18bacff1add7972))
+
+* add missing type annotations and docstrings ([`b8c7471`](https://github.com/kmnhan/erlabpy/commit/b8c747111663c07b441a3cbf0e11652c2f5cac49))
+
+### Fix
+
+* (**io**) enable specifying data_dir in loader context manager ([`37913b8`](https://github.com/kmnhan/erlabpy/commit/37913b80a1d7c6313a5b6cc4a3ab614565274c81))
+
+* (**io**) allow loader_class aliases to be None ([`7eae2eb`](https://github.com/kmnhan/erlabpy/commit/7eae2ebf13f972d368ddb9922a71fd3bbed014e5))
+
+### Refactor
+
+* remove igor2 import checking ([`b64d8f7`](https://github.com/kmnhan/erlabpy/commit/b64d8f7fe22ebc1c4818e26f93f864fd402bbd05))
+
+* (**io**) default to always_single=True ([`007bb3b`](https://github.com/kmnhan/erlabpy/commit/007bb3b2703a647856c0a85e89075cf6572d263a))
+
+### Style
+
+* sort __all__ and change linter configuration ([`c07262e`](https://github.com/kmnhan/erlabpy/commit/c07262eb647f17638eec77829a12a223f88b09d5))
+
+* apply perf lint and more ([`9cb4242`](https://github.com/kmnhan/erlabpy/commit/9cb424222e75360cf7240ce3325a63169ea67911))
+
+### Test
+
+* refactor directory structure ([`895ea0d`](https://github.com/kmnhan/erlabpy/commit/895ea0da46b4ed1ddcb81ff5dbff15ed20c7377b))
+
+
 ## v2.1.0 (2024-04-09)
 
 ### Chore
 
 * update changelog template ([`46a79e5`](https://github.com/kmnhan/erlabpy/commit/46a79e53c3bd6ce358d0fbf1a632d947671444c1))
 
 ### Ci
```

### Comparing `erlab-2.1.0/LICENSE` & `erlab-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/PKG-INFO` & `erlab-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.1.0/PythonInterface.ipf` & `erlab-2.1.1/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/README.md` & `erlab-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/Makefile` & `erlab-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/environment.yml` & `erlab-2.1.1/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/make.bat` & `erlab-2.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/source/conf.py` & `erlab-2.1.1/docs/source/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -145,36 +145,47 @@
 # -- Bibliography settings ---------------------------------------------------
 
 pybtex.style.formatting.unsrt.date = pybtex.style.template.words(sep="")[
     "(", pybtex.style.template.field("year"), ")"
 ]
 
 
+@pybtex.style.template.node
+def top_level(children, data):
+    return pybtex.style.template.sentence(sep=", ")[children].format_data(data)
+
+
 class APSStyle(pybtex.style.formatting.unsrt.Style):
     """
     APS style for BibTeX formatting, adapted from the conf.py file of the `mitiq
     library<https://github.com/unitaryfund/mitiq>`_.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.abbreviate_names = True
 
-    def format_title(self, e, which_field, as_sentence=True):
+    def format_names(self, role, as_sentence=False):
+        return super().format_names(role, as_sentence=as_sentence)
+
+    def format_volume_and_series(self, e, as_sentence=False):
+        return super().format_volume_and_series(e, as_sentence=as_sentence)
+
+    def format_title(self, e, which_field, as_sentence=False):
         formatted_title = pybtex.style.template.field(
             which_field, apply_func=lambda text: text.capitalize()
         )
 
         formatted_title = pybtex.style.template.tag("em")[formatted_title]
         if as_sentence:
             return pybtex.style.template.sentence[formatted_title]
         else:
             return formatted_title
 
-    def format_editor(self, e, as_sentence=True):
+    def format_editor(self, e, as_sentence=False):
         editors = self.format_names("editor", as_sentence=False)
         if "editor" not in e.persons:
             return editors
         result = pybtex.style.template.join(sep=" ")["edited by", editors]
         if as_sentence:
             return pybtex.style.template.sentence[result]
         else:
@@ -202,15 +213,28 @@
             pybtex.style.template.join(sep=", ")[
                 organization,
                 pybtex.style.template.optional_field("publisher"),
                 pybtex.style.template.field("year"),
             ],
         ]
 
-    def get_article_template(self, e):
+    def format_web_refs(self, e):
+        return pybtex.style.template.sentence(add_period=False)[
+            pybtex.style.template.optional[
+                self.format_url(e),
+                pybtex.style.template.optional[
+                    " (visited on ", pybtex.style.template.field("urldate"), ")"
+                ],
+            ],
+            pybtex.style.template.optional[self.format_eprint(e)],
+            pybtex.style.template.optional[self.format_pubmed(e)],
+            pybtex.style.template.optional[self.format_doi(e)],
+        ]
+
+    def format_journal_volume_page(self, e):
         volume_and_pages = pybtex.style.template.first_of[
             # volume and pages
             pybtex.style.template.optional[
                 pybtex.style.template.join[
                     " ",
                     pybtex.style.template.tag("strong")[
                         pybtex.style.template.field("volume")
@@ -226,51 +250,82 @@
             pybtex.style.template.words[
                 "pages",
                 pybtex.style.template.field(
                     "pages", apply_func=pybtex.style.formatting.unsrt.dashify
                 ),
             ],
         ]
-        template = pybtex.style.formatting.toplevel[
+        journal_volume_page = pybtex.style.template.sentence(sep=" ", add_period=False)[
+            pybtex.style.template.field("journal"),
+            pybtex.style.template.optional[volume_and_pages],
+            pybtex.style.formatting.unsrt.date,
+        ]
+        if "eprint" in e.fields:
+            return pybtex.style.template.href[
+                pybtex.style.template.join[
+                    "https://arxiv.org/abs/",
+                    pybtex.style.template.field("eprint", raw=True),
+                ],
+                journal_volume_page,
+            ]
+        elif "url" in e.fields:
+            return pybtex.style.template.href[
+                pybtex.style.template.field("url", raw=True), journal_volume_page
+            ]
+        elif "pubmed" in e.fields:
+            return pybtex.style.template.href[
+                pybtex.style.template.join[
+                    "https://www.ncbi.nlm.nih.gov/pubmed/",
+                    pybtex.style.template.field("pubmed", raw=True),
+                ],
+                journal_volume_page,
+            ]
+        elif "doi" in e.fields:
+            return pybtex.style.template.href[
+                pybtex.style.template.join[
+                    "https://doi.org/", pybtex.style.template.field("doi", raw=True)
+                ],
+                journal_volume_page,
+            ]
+        else:
+            return journal_volume_page
+
+    def get_article_template(self, e):
+        template = top_level[
             self.format_names("author"),
             self.format_title(e, "title"),
-            pybtex.style.template.sentence(sep=" ")[
-                pybtex.style.template.field("journal"),
-                pybtex.style.template.optional[volume_and_pages],
-                pybtex.style.formatting.unsrt.date,
-            ],
-            self.format_web_refs(e),
+            self.format_journal_volume_page(e),
         ]
         return template
 
     def get_book_template(self, e):
-        template = pybtex.style.formatting.toplevel[
+        template = top_level[
             self.format_author_or_editor(e),
             self.format_btitle(e, "title"),
             self.format_volume_and_series(e),
-            pybtex.style.template.sentence(sep=" ")[
+            pybtex.style.template.sentence(sep=" ", add_period=True)[
                 pybtex.style.template.sentence(add_period=False)[
                     pybtex.style.template.field("publisher"),
                     pybtex.style.template.optional_field("address"),
                     self.format_edition(e),
                 ],
                 pybtex.style.formatting.unsrt.date,
             ],
             pybtex.style.template.optional[
-                pybtex.style.template.sentence[self.format_isbn(e)]
+                pybtex.style.template.sentence(add_period=False)[self.format_isbn(e)]
             ],
-            pybtex.style.template.sentence[
+            pybtex.style.template.sentence(add_period=False)[
                 pybtex.style.template.optional_field("note")
             ],
             self.format_web_refs(e),
         ]
         return template
 
     def get_incollection_template(self, e):
-        template = pybtex.style.formatting.toplevel[
+        template = top_level[
             pybtex.style.template.sentence[self.format_names("author")],
             self.format_title(e, "title"),
             pybtex.style.template.words[
                 "In",
                 pybtex.style.template.sentence[
                     pybtex.style.template.optional[
                         self.format_editor(e, as_sentence=False)
@@ -289,37 +344,36 @@
                 pybtex.style.formatting.unsrt.date,
             ],
             self.format_web_refs(e),
         ]
         return template
 
     def get_inproceedings_template(self, e):
-        template = pybtex.style.formatting.toplevel[
+        template = top_level[
             pybtex.style.template.sentence[self.format_names("author")],
             self.format_title(e, "title"),
             pybtex.style.template.words[
                 "in",
-                pybtex.style.template.sentence[
+                pybtex.style.template.sentence(add_period=False)[
                     self.format_btitle(e, "booktitle", as_sentence=False),
                     # self.format_volume_and_series(e, as_sentence=False),
                     # self.format_chapter_and_pages(e),
                     pybtex.style.template.field("year"),
                     pybtex.style.template.sentence(add_period=False, sep=" ")[
                         pybtex.style.template.optional[
                             self.format_editor(e, as_sentence=False)
                         ],
                         pybtex.style.template.words(sep="")[
                             "(", self.format_address_organization_publisher_date(e), ")"
                         ],
                     ],
-                    pybtex.style.template.sentence(add_period=True, sep=". ")[
-                        "p",
-                        pybtex.style.formatting.unsrt.pages,
-                        pybtex.style.template.optional_field("note"),
+                    pybtex.style.template.join(sep=" ")[
+                        "p.", pybtex.style.formatting.unsrt.pages
                     ],
+                    pybtex.style.template.optional_field("note"),
                 ],
             ],
             self.format_web_refs(e),
         ]
         return template
```

### Comparing `erlab-2.1.0/docs/source/contributing.rst` & `erlab-2.1.1/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/source/getting-started.rst` & `erlab-2.1.1/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/source/images/imagetool_dark.png` & `erlab-2.1.1/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/source/images/imagetool_light.png` & `erlab-2.1.1/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/source/images/ktool_1_dark.png` & `erlab-2.1.1/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/source/images/ktool_1_light.png` & `erlab-2.1.1/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/source/images/ktool_2_dark.png` & `erlab-2.1.1/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/source/images/ktool_2_light.png` & `erlab-2.1.1/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/source/index.rst` & `erlab-2.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/source/pyplots/norms.py` & `erlab-2.1.1/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/source/reference.rst` & `erlab-2.1.1/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/source/refs.bib` & `erlab-2.1.1/docs/source/refs.bib`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,14 @@
   year    = {2017},
   type    = {Journal Article}
 }
 
 @article{hoyer2017xarray,
   title     = {xarray: {N-D} labeled arrays and datasets in {Python}},
   author    = {Hoyer, S. and J. Hamman},
-  journal   = {Journal of Open Research Software},
+  journal   = {J. Open Res. Softw.},
   volume    = {5},
   number    = {1},
   year      = {2017},
   publisher = {Ubiquity Press},
   doi       = {10.5334/jors.148}
 }
```

### Comparing `erlab-2.1.0/docs/source/user-guide/index.rst` & `erlab-2.1.1/docs/source/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/docs/source/user-guide/kconv.ipynb` & `erlab-2.1.1/docs/source/user-guide/kconv.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999621212121212%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(13, '\\n')]}}}"}*

```diff
@@ -61,14 +61,15 @@
                 "#   are kept when performing operations such as sum and mean. Since parameters for\n",
                 "#   momentum conversion such as angle offsets and inner potential are stored as\n",
                 "#   attributes, this is important.\n",
                 "%config InlineBackend.figure_formats = [\"svg\", \"pdf\"]\n",
                 "plt.rcParams[\"figure.dpi\"] = 96\n",
                 "\n",
                 "import xarray\n",
+                "\n",
                 "_ = xarray.set_options(display_expand_data=False, keep_attrs=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "editable": true,
```

### Comparing `erlab-2.1.0/docs/source/user-guide/plotting.ipynb` & `erlab-2.1.1/docs/source/user-guide/plotting.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999436936936936%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(3, '\\n')]}}}"}*

```diff
@@ -48,14 +48,15 @@
                 "nbsphinx": "hidden"
             },
             "outputs": [],
             "source": [
                 "%config InlineBackend.figure_formats = [\"svg\", \"pdf\"]\n",
                 "plt.rcParams[\"figure.dpi\"] = 96\n",
                 "import xarray as xr\n",
+                "\n",
                 "xr.set_options(display_expand_data=False)\n",
                 "nb_execution_mode = \"cache\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
```

### Comparing `erlab-2.1.0/environment.yml` & `erlab-2.1.1/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/environment_apple.yml` & `erlab-2.1.1/environment_apple.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/environment_nogit.yml` & `erlab-2.1.1/environment_nogit.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/environment_nogit_mkl.yml` & `erlab-2.1.1/environment_nogit_mkl.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/pyproject.toml` & `erlab-2.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -147,60 +147,40 @@
 dist_glob_patterns = ["dist/*"]
 upload_to_vcs_release = true
 
 
 [tool.ruff]
 line-length = 88
 indent-width = 4
-exclude = [
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".git-rewrite",
-    ".hg",
-    ".ipynb_checkpoints",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".pyenv",
-    ".pytest_cache",
-    ".pytype",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    ".vscode",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "site-packages",
-    "venv",
-]
 
 [tool.ruff.lint]
 select = [
     "E4",
     "E7",
     "E9",
     "F",
     "B",
     "C4",
     "FA",
     "ICN",
     "PIE",
+    "PT",
+    "Q",
     "RSE",
+    "TID",
     "TCH",
+    # "PTH",
+    # "FIX",
+    "TRY",
+    "FLY",
     "NPY",
+    "PERF",
     "RUF",
 ]
-ignore = ["B905", "ICN001", "RUF001", "RUF002", "RUF003", "RUF012"]
+ignore = ["B905", "ICN001", "TRY003", "RUF001", "RUF002", "RUF003", "RUF012"]
 extend-select = [
     "UP", # pyupgrade
 ]
 
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
@@ -209,8 +189,10 @@
 docstring-code-format = true
 docstring-code-line-length = "dynamic"
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
+addopts = ["--import-mode=importlib"]
+pythonpath = "src"
 testpaths = "tests"
```

### Comparing `erlab-2.1.0/src/erlab/accessors.py` & `erlab-2.1.1/src/erlab/accessors.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 data analysis and visualization.
 
 .. currentmodule:: erlab.accessors
 
 """
 
 __all__ = [
-    "PlotAccessor",
     "ImageToolAccessor",
-    "SelectionAccessor",
     "MomentumAccessor",
     "OffsetView",
+    "PlotAccessor",
+    "SelectionAccessor",
 ]
 
 import functools
 import time
 import warnings
 from collections.abc import Callable, ItemsView, Iterable, Iterator
 from typing import Literal
@@ -673,14 +673,48 @@
     def offsets(self, offset_dict: dict[str, float]):
         if not hasattr(self, "_offsetview"):
             self._offsetview = OffsetView(self._obj)
 
         self._offsetview.reset()
         self._offsetview.update(offset_dict)
 
+    @property
+    @only_angles
+    def best_kp_resolution(self) -> float:
+        r"""
+        Estimates the minimum in-plane momentum resolution based on the kinetic energy
+        and angular resolution:
+
+        .. math:: \Delta k_{\parallel} \sim \sqrt{2 m_e E_k/\hbar^2} \cos(\alpha) \Delta\alpha
+
+        """
+        min_Ek = np.amin(self._kinetic_energy)
+        max_angle = max(np.abs(self._obj["alpha"].values))
+        return (
+            rel_kconv
+            * np.sqrt(min_Ek)
+            * np.cos(np.deg2rad(max_angle))
+            * np.deg2rad(self.angle_resolution)
+        )
+
+    @property
+    @only_angles
+    def best_kz_resolution(self) -> float:
+        r"""
+        Estimates the minimum out-of-plane momentum resolution based on the mean free
+        path :cite:p:`seah1979imfp` and the kinetic energy.
+
+        .. math:: \Delta k_z \sim 1/\lambda
+
+        """
+        kin = self._kinetic_energy.flatten()
+        c1, c2 = 641.0, 0.096
+        imfp = (c1 / (kin**2) + c2 * np.sqrt(kin)) * 10
+        return np.amin(1 / imfp)
+
     def estimate_bounds(self) -> dict[str, tuple[float, float]]:
         """
         Estimates the bounds of the data in momentum space based on the available
         parameters.
 
         Returns
         -------
@@ -770,48 +804,14 @@
         if from_numpoints:
             return float((lims[1] - lims[0]) / len(self._obj[dim]))
         elif axis == "kz":
             return self.best_kz_resolution
         else:
             return self.best_kp_resolution
 
-    @property
-    @only_angles
-    def best_kp_resolution(self) -> float:
-        r"""
-        Estimates the minimum in-plane momentum resolution based on the kinetic energy
-        and angular resolution:
-
-        .. math:: \Delta k_{\parallel} \sim \sqrt{2 m_e E_k/\hbar^2} \cos(\alpha) \Delta\alpha
-
-        """
-        min_Ek = np.amin(self._kinetic_energy)
-        max_angle = max(np.abs(self._obj["alpha"].values))
-        return (
-            rel_kconv
-            * np.sqrt(min_Ek)
-            * np.cos(np.deg2rad(max_angle))
-            * np.deg2rad(self.angle_resolution)
-        )
-
-    @property
-    @only_angles
-    def best_kz_resolution(self) -> float:
-        r"""
-        Estimates the minimum out-of-plane momentum resolution based on the mean free
-        path :cite:p:`seah1979imfp` and the kinetic energy.
-
-        .. math:: \Delta k_z \sim 1/\lambda
-
-        """
-        kin = self._kinetic_energy.flatten()
-        c1, c2 = 641.0, 0.096
-        imfp = (c1 / (kin**2) + c2 * np.sqrt(kin)) * 10
-        return np.amin(1 / imfp)
-
     def _forward_func_raw(self, alpha, beta):
         return get_kconv_func(
             self._kinetic_energy, self.configuration, self.angle_params
         )[0](alpha, beta)
 
     def _inverse_func_raw(self, kx, ky, kz=None):
         return get_kconv_func(
```

### Comparing `erlab-2.1.0/src/erlab/analysis/__init__.py` & `erlab-2.1.1/src/erlab/analysis/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,21 +18,21 @@
    kspace
    transform
    utilities
 
 """
 
 __all__ = [
+    "correct_with_edge",
+    "mask_with_hex_bz",
     "mask_with_polygon",
     "polygon_mask",
     "polygon_mask_points",
-    "mask_with_hex_bz",
     "rotateinplane",
     "rotatestackinplane",
-    "correct_with_edge",
 ]
 
 from erlab.analysis import correlation, fit, gold, interpolate, kspace  # noqa: F401
 from erlab.analysis.mask import (
     mask_with_hex_bz,
     mask_with_polygon,
     polygon_mask,
```

### Comparing `erlab-2.1.0/src/erlab/analysis/correlation.py` & `erlab-2.1.1/src/erlab/analysis/correlation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Macros for correlation analysis."""
 
-__all__ = ["acf2stack", "acf2", "match_dims", "xcorr1d"]
+__all__ = ["acf2", "acf2stack", "match_dims", "xcorr1d"]
 
 
 import itertools
 
 import joblib
 import numpy as np
 import scipy.signal
```

### Comparing `erlab-2.1.0/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.1.1/src/erlab/analysis/fit/functions/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,26 +11,26 @@
    dynamic
    general
 
 """
 
 __all__ = [
     "TINY",
+    "FermiEdge2dFunction",
+    "MultiPeakFunction",
+    "PolynomialFunction",
     "do_convolve",
     "do_convolve_y",
-    "gaussian_wh",
-    "lorentzian_wh",
     "fermi_dirac",
     "fermi_dirac_linbkg",
     "fermi_dirac_linbkg_broad",
-    "step_linbkg_broad",
+    "gaussian_wh",
+    "lorentzian_wh",
     "step_broad",
-    "PolynomialFunction",
-    "MultiPeakFunction",
-    "FermiEdge2dFunction",
+    "step_linbkg_broad",
 ]
 
 from erlab.analysis.fit.functions.dynamic import (
     FermiEdge2dFunction,
     MultiPeakFunction,
     PolynomialFunction,
 )
```

### Comparing `erlab-2.1.0/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.1.1/src/erlab/analysis/fit/functions/dynamic.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Class-based dynamic functions for fitting.
 
 These functions are not limited to a single function form, and can be used to create
 complex models.
 """
 
 __all__ = [
-    "get_args_kwargs",
     "DynamicFunction",
-    "PolynomialFunction",
-    "MultiPeakFunction",
     "FermiEdge2dFunction",
+    "MultiPeakFunction",
+    "PolynomialFunction",
+    "get_args_kwargs",
 ]
 import functools
 import inspect
 from collections.abc import Callable
 
 import numpy as np
 import numpy.typing as npt
```

### Comparing `erlab-2.1.0/src/erlab/analysis/fit/functions/general.py` & `erlab-2.1.1/src/erlab/analysis/fit/functions/general.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 Many functions are `numba`-compiled for speed.
 """
 
 __all__ = [
     "TINY",
     "do_convolve",
     "do_convolve_y",
-    "gaussian_wh",
-    "lorentzian_wh",
     "fermi_dirac",
     "fermi_dirac_linbkg",
     "fermi_dirac_linbkg_broad",
-    "step_linbkg_broad",
+    "gaussian_wh",
+    "lorentzian_wh",
     "step_broad",
+    "step_linbkg_broad",
 ]
 
 from collections.abc import Callable
 
 import numba
 import numpy as np
 import numpy.typing as npt
```

### Comparing `erlab-2.1.0/src/erlab/analysis/fit/minuit.py` & `erlab-2.1.1/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/analysis/fit/models.py` & `erlab-2.1.1/src/erlab/analysis/fit/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Models for fitting data."""
 
 __all__ = [
     "ExtendedAffineBroadenedFD",
-    "StepEdgeModel",
-    "PolynomialModel",
-    "MultiPeakModel",
     "FermiEdge2dModel",
+    "MultiPeakModel",
+    "PolynomialModel",
+    "StepEdgeModel",
 ]
 
 import lmfit
 import numba
 import numpy as np
 import numpy.typing as npt
 import scipy.ndimage
@@ -157,15 +157,19 @@
     __init__.doc = lmfit.models.COMMON_INIT_DOC
     guess.__doc__ = lmfit.models.COMMON_GUESS_DOC
 
 
 class StepEdgeModel(lmfit.Model):
     def __init__(self, independent_vars=("x",), prefix="", missing="raise", **kwargs):
         kwargs.update(
-            {"prefix": prefix, "missing": missing, "independent_vars": independent_vars}
+            {
+                "prefix": prefix,
+                "missing": missing,
+                "independent_vars": independent_vars,
+            }
         )
         super().__init__(step_linbkg_broad, **kwargs)
         self.set_param_hint("sigma", min=0.0)
 
     def guess(self, data, x, **kwargs):
         pars = self.make_params()
```

### Comparing `erlab-2.1.0/src/erlab/analysis/fit/spline.py` & `erlab-2.1.1/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/analysis/gold.py` & `erlab-2.1.1/src/erlab/analysis/gold.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Fermi edge fitting."""
 
 __all__ = [
     "edge",
     "poly",
     "poly_from_edge",
-    "spline_from_edge",
     "resolution",
     "resolution_roi",
+    "spline_from_edge",
 ]
 
 from collections.abc import Sequence
 
 import joblib
 import lmfit.model
 import matplotlib
@@ -212,15 +212,15 @@
 
 def _plot_gold_fit(fig, gold, angle_range, eV_range, center_arr, center_stderr, res):
     if isinstance(res, lmfit.model.ModelResult):
         is_callable = False
     elif callable(res):
         is_callable = True
     else:
-        raise ValueError
+        raise TypeError("res must be a callable or a lmfit.model.ModelResult")
 
     if not isinstance(fig, plt.Figure):
         fig = plt.figure(figsize=figwh(0.75, wscale=1.75))
 
     gs = fig.add_gridspec(2, 2, height_ratios=[1, 3])
     ax0 = fig.add_subplot(gs[:, 0])
     ax1 = fig.add_subplot(gs[0, 1])
```

### Comparing `erlab-2.1.0/src/erlab/analysis/image.py` & `erlab-2.1.1/src/erlab/analysis/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         [20, 22, 24, 25, 27],
         [29, 31, 33, 34, 36],
         [36, 38, 40, 41, 43]])
     Dimensions without coordinates: x, y
 
     """
     if np.isscalar(sigma):
-        sigma = {d: sigma for d in darr.dims}
+        sigma = dict.fromkeys(darr.dims, sigma)
     elif not isinstance(sigma, dict):
         sigma = dict(zip(darr.dims, sigma))
 
     # Get the axis indices to apply the filter
     axes = tuple(darr.get_axis_num(d) for d in sigma.keys())
 
     # Convert arguments to tuples acceptable by scipy
@@ -113,15 +113,15 @@
     if isinstance(mode, dict):
         mode = tuple(mode[d] for d in sigma.keys())
     if radius is not None:
         if len(radius) != len(sigma):
             raise ValueError("`radius` does not match dimensions of `sigma`")
 
         if np.isscalar(radius):
-            radius = {d: radius for d in sigma.keys()}
+            radius = dict.fromkeys(sigma.keys(), radius)
         elif not isinstance(radius, dict):
             radius = dict(zip(sigma.keys(), radius))
 
         # Calculate radius in pixels
         radius: tuple[int, ...] = tuple(
             round(r / (darr[d].values[1] - darr[d].values[0]))
             for d, r in radius.items()
@@ -192,15 +192,15 @@
 
     See Also
     --------
     :func:`scipy.ndimage.gaussian_laplace` : The underlying function used to apply the
         filter.
     """
     if np.isscalar(sigma):
-        sigma = {d: sigma for d in darr.dims}
+        sigma = dict.fromkeys(darr.dims, sigma)
     elif not isinstance(sigma, dict):
         sigma = dict(zip(darr.dims, sigma))
 
     if len(sigma) != darr.ndim:
         raise ValueError(
             "`sigma` must be provided for every dimension of the DataArray"
         )
```

### Comparing `erlab-2.1.0/src/erlab/analysis/interpolate.py` & `erlab-2.1.1/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/analysis/kspace.py` & `erlab-2.1.1/src/erlab/analysis/kspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,36 @@
     Type2DA = 4
 
 
 def _sinc(x):
     return np.sin(x) / (x + 1e-15)
 
 
-def kz_func_inv(kz, inner_potential, kx, ky):
+def _kz_func_inv(kz, inner_potential, kx, ky):
     k_perp_sq = kx**2 + ky**2
     k_z_sq = kz**2
     return k_perp_sq + k_z_sq - inner_potential / erlab.constants.rel_kzconv
 
 
+def _kperp_func(k_tot_sq, kx, ky):
+    r""":math:`\sqrt{k^2 - k_x^2 - k_y^2}`"""
+    return np.sqrt(np.clip(k_tot_sq - kx**2 - ky**2, a_min=0, a_max=None))
+
+
 def kz_func(kinetic_energy, inner_potential, kx, ky):
+    r"""
+    Calculate :math:`k_z` from the given kinetic energy, inner potential, and
+    :math:`k_x`, :math:`k_y` with
+
+    .. math::
+
+        k_z = \sqrt{k^2 - k_x^2 - k_y^2 + \frac{2 m_e V_0}{\hbar^2}}
+
+    where :math:`k = \frac{\sqrt{2 m_e E_k}}{\hbar}`.
+    """
     k_tot = erlab.constants.rel_kconv * np.sqrt(kinetic_energy)
     k_perp_sq = k_tot**2 - kx**2 - ky**2
     k_z_sq = k_perp_sq + inner_potential / erlab.constants.rel_kzconv
     return np.sqrt(np.clip(k_z_sq, a_min=0, a_max=None))
 
 
 def get_kconv_func(
@@ -116,19 +131,14 @@
             func = _kconv_func_type2_da
         case _:
             ValueError(f"Invalid configuration {configuration}")
 
     return func(k_tot, **angle_params)
 
 
-def _kperp_func(k_tot_sq, kx, ky):
-    r""":math:`\sqrt{k^2 - k_x^2 - k_y^2}`"""
-    return np.sqrt(np.clip(k_tot_sq - kx**2 - ky**2, a_min=0, a_max=None))
-
-
 def _kconv_func_type1(
     k_tot: np.floating | npt.NDArray,
     delta: np.floating = 0.0,
     xi: np.floating = 0.0,
     xi0: np.floating = 0.0,
     beta0: np.floating = 0.0,
 ):
```

### Comparing `erlab-2.1.0/src/erlab/analysis/mask/polygon.py` & `erlab-2.1.1/src/erlab/analysis/mask/polygon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Polygon mask generation code adapted from the `CGAL C++ library
+Point-in-polygon algorithm adapted from the `CGAL C++ library
 <https://doc.cgal.org/5.3.2/Polygon/index.html>`_.
 
 """
 
 from __future__ import annotations
 
 import enum
@@ -65,15 +65,15 @@
     Parameters
     ----------
     points
         Input array of polygon vertices.
 
     Returns
     -------
-    int
+    index : int
 
     """
     ind = _get_argmin_all(points[:, 0].astype(np.float32))
     return ind[np.argmin(points[ind][:, 1])]
 
 
 @numba.njit(nogil=True, cache=True)
@@ -130,40 +130,62 @@
                 return int(low_x_comp_res != Comparison.EQUAL)
 
     return _orientation(points[low], point, points[high])
 
 
 @numba.njit(nogil=True, cache=True)
 def bounded_side_bool(
-    points: npt.NDArray[np.float64], point: tuple[float, float], boundary=True
-):
+    points: npt.NDArray[np.float64], point: tuple[float, float], boundary: bool = True
+) -> bool:
+    """Computes whether a point lies inside a polygon using `bounded_side`.
+
+    Parameters
+    ----------
+    points
+        (N, 2) input array of polygon vertices.
+    point
+        2-tuple of float specifying point of interest.
+    boundary
+        Whether to consider points on the boundary to be inside the polygon. Default is
+        `True`.
+
+    Returns
+    -------
+    bool
+        `True` if the point is on the bounded side of the polygon, `False` otherwise.
+    """
     match bounded_side(points, point):
         case Side.ON_UNBOUNDED_SIDE:
             return False
         case Side.ON_BOUNDED_SIDE:
             return True
         case Side.ON_BOUNDARY:
             return boundary
 
 
 @numba.njit(nogil=True, cache=True)
-def bounded_side(points: npt.NDArray[np.float64], point: tuple[float, float]):
-    """Computes if a point lies inside a polygon.
+def bounded_side(points: npt.NDArray[np.float64], point: tuple[float, float]) -> Side:
+    """Computes if a point is inside, outside, or on the boundary of a polygon.
 
     The polygon is defined by the sequence of points [first,last). Being inside is
     defined by the odd-even rule. If the point is on a polygon edge, a special value is
     returned. A simple polygon divides the plane in an unbounded and a bounded region.
     According to the definition points in the bounded region are inside the polygon.
 
     Parameters
     ----------
     points
         (N, 2) input array of polygon vertices.
     point
-        2-tuple specifying point of interest
+        2-tuple of float specifying point of interest.
+
+    Returns
+    -------
+    Side
+        Enum indicating the location of the point.
 
     Note
     ----
     We shoot a horizontal ray from the point to the right and count the number of
     intersections with polygon segments. If the number of intersections is odd, the
     point is inside. We don't count intersections with horizontal segments. With
     non-horizontal segments, the top vertex is considered to be part of the segment, but
```

### Comparing `erlab-2.1.0/src/erlab/analysis/transform.py` & `erlab-2.1.1/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/analysis/utilities.py` & `erlab-2.1.1/src/erlab/analysis/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__all__ = ["shift", "correct_with_edge"]
+__all__ = ["correct_with_edge", "shift"]
 
 import itertools
 from collections.abc import Callable
 
 import lmfit
 import matplotlib.pyplot as plt
 import numpy as np
@@ -202,15 +202,15 @@
             raise ValueError(
                 "Length of modelresult must be equal to the length of alpha in data"
             )
         else:
             edge_quad = modelresult
 
     else:
-        raise ValueError(
+        raise TypeError(
             "modelresult must be one of "
             "lmfit.model.ModelResult, "
             "and np.ndarray or a callable"
         )
 
     if isinstance(edge_quad, np.ndarray):
         edge_quad = xr.DataArray(
```

### Comparing `erlab-2.1.0/src/erlab/characterization/resistance.py` & `erlab-2.1.1/src/erlab/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/characterization/xrd.py` & `erlab-2.1.1/src/erlab/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/constants.py` & `erlab-2.1.1/src/erlab/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,18 +38,17 @@
 #: :math:`hc`  (eV·m)
 hc_eV: float = 1.2398419843320028e-6
 #: Dirac constant :math:`\hbar` (eV·s)
 hbar_eV: float = 6.582119569509067e-16
 #: :math:`\hbar^2` (eV²·s²)
 hbarsq_eV: float = 4.332429802731423e-31
 
-#: :math:`hc`  (eV·nm)
+#: :math:`hc`  (eV·nm), Used in energy-wavelength conversion
 rel_eV_nm: float = 1239.8419843320028
 
-
 #: :math:`\frac{\sqrt{2 m_e}}{\hbar}`, Used in momentum conversion
 rel_kconv: float = 0.512316721967493
 #: :math:`\frac{\hbar^2}{2 m_e}`, Used in momentum conversion
 rel_kzconv: float = 3.8099821161548606
 
 #: Boltzmann constant :math:`k_B` (J/K)
 kb: float = 1.380649e-23
```

### Comparing `erlab-2.1.0/src/erlab/interactive/__init__.py` & `erlab-2.1.1/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/interactive/bzplot.py` & `erlab-2.1.1/src/erlab/interactive/bzplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,20 +298,20 @@
         self.sigChanged.emit(self.bvec_val)
 
     def set_latt(self, a, b, c, alpha, beta, gamma):
         self.params_latt.set_values(a=a, b=b, c=c, alpha=alpha, beta=beta, gamma=gamma)
 
     def set_avec(self, avec):
         self.params_avec.set_values(
-            **{f"a{i+1}{('x', 'y', 'z')[j]}": v for (i, j), v in np.ndenumerate(avec)}
+            **{f"a{i + 1}{('x', 'y', 'z')[j]}": v for (i, j), v in np.ndenumerate(avec)}
         )
 
     def set_bvec(self, bvec):
         self.params_bvec.set_values(
-            **{f"b{i+1}{('x', 'y', 'z')[j]}": v for (i, j), v in np.ndenumerate(bvec)}
+            **{f"b{i + 1}{('x', 'y', 'z')[j]}": v for (i, j), v in np.ndenumerate(bvec)}
         )
 
     @property
     def latt_vals(self):
         return tuple(
             self.params_latt.widgets[k].value()
             for k in ("a", "b", "c", "alpha", "beta", "gamma")
@@ -364,19 +364,19 @@
             mew=0,
             clip_on=False,
         )[0]
 
         # plot reciprocal lattice vectors
         self._bvecs = []
         for i, b in enumerate(bvec):
-            p = self.ax.plot(*[(0, bi) for bi in b], "-", c=f"C{i+1}", clip_on=False)
+            p = self.ax.plot(*[(0, bi) for bi in b], "-", c=f"C{i + 1}", clip_on=False)
             t = self.ax.text(
                 *(b + 0.15 * b / np.linalg.norm(b)),
-                f"$b_{i+1}$",
-                c=f"C{i+1}",
+                f"$b_{i + 1}$",
+                c=f"C{i + 1}",
                 ha="center",
                 va="center_baseline",
             )
             self._bvecs.append((p[0], t))
 
         # plot origin
         self.ax.plot(0, 0, 0, ".", color="k", mew=0)
```

### Comparing `erlab-2.1.0/src/erlab/interactive/colors.py` & `erlab-2.1.1/src/erlab/interactive/colors.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Functions for manipulating colors in Qt."""
 
 from __future__ import annotations
 
 __all__ = [
+    "BetterColorBarItem",
+    "BetterImageItem",
     "ColorMapComboBox",
     "ColorMapGammaWidget",
-    "BetterImageItem",
-    "BetterColorBarItem",
     "color_to_QColor",
-    "pg_colormap_names",
     "pg_colormap_from_name",
+    "pg_colormap_names",
     "pg_colormap_powernorm",
     "pg_colormap_to_QPixmap",
 ]
 
 import weakref
 from collections.abc import Iterable, Sequence
 from typing import Literal
```

### Comparing `erlab-2.1.0/src/erlab/interactive/curvefittingtool.py` & `erlab-2.1.1/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/interactive/derivative.py` & `erlab-2.1.1/src/erlab/interactive/derivative.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,25 +241,27 @@
                             for s in (self.sx_spin, self.sy_spin)
                         ],
                     )
                 )
             }
             lines.append(f"_processed = {data_name}.copy()")
             data_name = "_processed"
-            lines.append(f"for _ in range({self.sn_spin.value()}):")
-            lines.append(
-                "\t"
-                + gen_function_code(
-                    copy=False,
-                    **{
-                        "_processed = era.image.gaussian_filter": [
-                            f"|{data_name}|",
-                            arg_dict,
-                        ]
-                    },
+            lines.extend(
+                (
+                    f"for _ in range({self.sn_spin.value()}):",
+                    "\t"
+                    + gen_function_code(
+                        copy=False,
+                        **{
+                            "_processed = era.image.gaussian_filter": [
+                                f"|{data_name}|",
+                                arg_dict,
+                            ]
+                        },
+                    ),
                 )
             )
             data_name = "_processed"
 
         if self.tab_widget.currentIndex() == 0:
             dim = self.xdim if self.x_radio.isChecked() else self.ydim
             lines.append(f"{data_name}.differentiate('{dim}').differentiate('{dim}')")
```

### Comparing `erlab-2.1.0/src/erlab/interactive/dtool.ui` & `erlab-2.1.1/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/interactive/exampledata.py` & `erlab-2.1.1/src/erlab/interactive/exampledata.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/interactive/fermiedge.py` & `erlab-2.1.1/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.1.1/src/erlab/interactive/imagetool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    fastbinning
    controls
 
 """
 
 from __future__ import annotations
 
-__all__ = ["itool", "ImageTool"]
+__all__ = ["ImageTool", "itool"]
 
 import gc
 import sys
 from typing import TYPE_CHECKING
 
 import xarray as xr
 from qtpy import QtCore, QtWidgets
@@ -128,15 +128,15 @@
         except NameError:
             pass
     if execute:
         qapp.exec()
         del win
         gc.collect()
 
-        return
+        return None
     return win
 
 
 class BaseImageTool(QtWidgets.QMainWindow):
     def __init__(self, data=None, parent=None, **kwargs):
         super().__init__(parent=parent)
         self.slicer_area = ImageSlicerArea(self, data, **kwargs)
```

### Comparing `erlab-2.1.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.1.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,15 @@
 
         if self.useblit and not self.canvas.supports_blit:
             raise RuntimeError(
                 "Canvas does not support blit. "
                 "If running in ipython, add `%matplotlib qt`."
             )
         for ax in self.axes:
-            for _loc, spine in ax.spines.items():
+            for spine in ax.spines.values():
                 spine.set_position(("outward", 1))
         self.cursorprops = cursorprops
         self.lineprops = lineprops
         self.fermilineprops = fermilineprops
         self.improps = improps
         self.cursorprops.update(
             {
@@ -1029,15 +1029,14 @@
         elif i == 14:
             self.all[i].set_ydata((self.cursor_pos[2], self.cursor_pos[2]))
 
     def _drawpath(self):
         # ld = LineDrawer(self.canvas, self.axes[0])
         # points = ld.draw_line()
         # print(points)
-        # TODO
         pass
 
     def _onselectpath(self, verts):
         print(verts)
 
 
 class ImageToolNavBar(NavigationToolbar2QT):
@@ -1065,19 +1064,15 @@
             "filesave": qta.icon("msc.save"),
             "home": qta.icon("msc.debug-step-back"),
             "move": qta.icon("msc.move"),
             "qt4_editor_options": qta.icon("msc.graph-line"),
             "zoom_to_rect": qta.icon("msc.search"),
             "subplots": qta.icon("msc.editor-layout"),
         }
-        try:
-            return icons_dict[name]
-        except BaseException as e:
-            print(name)
-            raise Exception from e
+        return icons_dict[name]
         # name = name.replace('.png', '_large.png')
         # pm = QtGui.QPixmap(str(cbook._get_data_path('images', name)))
         # _setDevicePixelRatio(pm, _devicePixelRatioF(self))
         # if self.palette().color(self.backgroundRole()).value() < 128:
         # icon_color = self.palette().color(self.foregroundRole())
         # mask = pm.createMaskFromColor(
         # QtGui.QColor('black'),
```

### Comparing `erlab-2.1.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.1.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -1382,52 +1382,50 @@
             totalspan = (2, 1)
         elif axis in bottom_right:
             group = bottom_right
             totalspan = (1, 2)
         elif axis in top_right:
             group = top_right
             totalspan = (2, 2)
+        elif not toggle:
+            self.removeItem(target)
+            return
         else:
-            if not toggle:
-                self.removeItem(target)
-                return
-            else:
-                self.addItem(target, *ref_dims[axis])
-                return
+            self.addItem(target, *ref_dims[axis])
+            return
 
         anchors = tuple(ref_dims[i][:2] for i in group)
         other_index = [
             x for x in group if x != axis and self.axes[x] in self.ci.items.keys()
         ]
         other = [self.axes[i] for i in other_index]
         unique = True if len(other) == 0 else False
         if not toggle:
             self.removeItem(target)
             if not unique:
                 for o in other:
                     self.removeItem(o)
                     self.addItem(o, *anchors[0], *totalspan)
+        elif unique:
+            self.addItem(target, *anchors[0], *totalspan)
         else:
-            if unique:
-                self.addItem(target, *anchors[0], *totalspan)
-            else:
-                # for i, o, oi in enumerate(zip(other, other_index)):
-                # self.removeItem(o)
-                # for o, oi in zip(other, other_index):
-                #     self.removeItem(o)
-                # self.addItem(self.axes[group[0]], *ref_dims[axis])
-                # for o, oi in zip(other, other_index):
-                #     self.addItem(o, *ref_dims[oi])
-                # for a in group:
-                #     ax = self.axes[a]
-                #     if ax in self.ci.items.keys():
-                #         self.removeItem(ax)
-                #     self.addItem(ax, *ref_dims[a])
-                self.addItem(self.axes[group[0]], *anchors[0], *ref_dims[axis][2:])
-                self.addItem(self.axes[group[1]], *anchors[1], *ref_dims[axis][2:])
+            # for i, o, oi in enumerate(zip(other, other_index)):
+            # self.removeItem(o)
+            # for o, oi in zip(other, other_index):
+            #     self.removeItem(o)
+            # self.addItem(self.axes[group[0]], *ref_dims[axis])
+            # for o, oi in zip(other, other_index):
+            #     self.addItem(o, *ref_dims[oi])
+            # for a in group:
+            #     ax = self.axes[a]
+            #     if ax in self.ci.items.keys():
+            #         self.removeItem(ax)
+            #     self.addItem(ax, *ref_dims[a])
+            self.addItem(self.axes[group[0]], *anchors[0], *ref_dims[axis][2:])
+            self.addItem(self.axes[group[1]], *anchors[1], *ref_dims[axis][2:])
 
     def set_labels(self, labels=None):
         """labels: list or tuple of str"""
         if labels is None:
             labels = self.data_dims
         # 0: default, 1: svg, 2: pixmap
         labelmode = ItoolAxisItem.LabelType.TextLabel
@@ -1843,15 +1841,15 @@
             return
         D = [v is not None for v in V]
         if not any(D):
             return
         for i in range(self.data_ndim):
             if D[i]:
                 ind = self.get_index_of_value(i, V[i])
-                if self.snap and (ind == self._last_ind[i]) or self.axis_locked[i]:
+                if (self.snap and (ind == self._last_ind[i])) or self.axis_locked[i]:
                     D[i] = False
                 else:
                     self._last_ind[i] = ind
             if not D[i]:
                 V[i] = self.cursor_pos[i]
         if not any(D):
             return
@@ -2118,15 +2116,14 @@
             self.update()
         super().changeEvent(evt)
 
     def _drawpath(self):
         # ld = LineDrawer(self.canvas, self.axes[0])
         # points = ld.draw_line()
         # print(points)
-        # TODO
         pass
 
     def _onselectpath(self, verts):
         print(verts)
 
 
 class ImageToolColors(QtWidgets.QDialog):
@@ -3204,15 +3201,14 @@
         pass
         # if i == self.tabwidget.indexOf(self.tab3):
         # lazy loading
         # self.tab3.initialize_functions()
 
 
 def itool_(data, execute=None, *args, **kwargs):
-    # TODO: implement multiple windows, equal aspect settings
     qapp = QtWidgets.QApplication.instance()
     if not qapp:
         qapp = QtWidgets.QApplication(sys.argv)
     qapp.setStyle("Fusion")
 
     if isinstance(data, list | tuple):
         win = ()
```

### Comparing `erlab-2.1.0/src/erlab/interactive/imagetool/controls.py` & `erlab-2.1.1/src/erlab/interactive/imagetool/controls.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 __all__ = [
-    "ItoolCrosshairControls",
     "ColorControls",
-    "ItoolColormapControls",
     "ItoolBinningControls",
+    "ItoolColormapControls",
+    "ItoolCrosshairControls",
 ]
 
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pyqtgraph as pg
 import qtawesome as qta
```

### Comparing `erlab-2.1.0/src/erlab/interactive/imagetool/core.py` & `erlab-2.1.1/src/erlab/interactive/imagetool/core.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.1.1/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.1.1/src/erlab/interactive/imagetool/slicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,26 +26,25 @@
         numba.int64,
         numba.int64,
         numba.types.UniTuple(numba.types.UniTuple(numba.float32, 2), i),
         numba.types.UniTuple(numba.float32, i),
     )
     for i in VALID_NDIM
 ]
-_signature_index_of_value = []
-for ftype in (numba.float32, numba.float64):
-    for i in VALID_NDIM:
-        _signature_index_of_value.append(
-            numba.int64(
-                numba.int64,
-                ftype,
-                numba.types.UniTuple(numba.types.UniTuple(ftype, 2), i),
-                numba.types.UniTuple(ftype, i),
-                numba.types.UniTuple(numba.int64, i),
-            )
-        )
+_signature_index_of_value = [
+    numba.int64(
+        numba.int64,
+        ftype,
+        numba.types.UniTuple(numba.types.UniTuple(ftype, 2), i),
+        numba.types.UniTuple(ftype, i),
+        numba.types.UniTuple(numba.int64, i),
+    )
+    for ftype in (numba.float32, numba.float64)
+    for i in VALID_NDIM
+]
 
 
 @numba.njit(_signature_array_rect, cache=True, fastmath=True)
 def _array_rect(
     i: int,
     j: int,
     lims: tuple[tuple[np.float32, np.float32], ...],
```

### Comparing `erlab-2.1.0/src/erlab/interactive/kspace.py` & `erlab-2.1.1/src/erlab/interactive/kspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,19 +282,21 @@
         out_lines: list[str] = []
 
         if self.data.kspace.has_hv:
             out_lines.append(
                 f"{input_name}.kspace.inner_potential"
                 f" = {self._offset_spins['V0'].value()}"
             )
-        out_lines.append(f"{input_name}.kspace.offsets = {self.offset_dict}")
-        out_lines.append(
-            gen_function_code(
-                copy=False,
-                **{f"{input_name}_kconv = {input_name}.kspace.convert": [arg_dict]},
+        out_lines.extend(
+            (
+                f"{input_name}.kspace.offsets = {self.offset_dict}",
+                gen_function_code(
+                    copy=False,
+                    **{f"{input_name}_kconv = {input_name}.kspace.convert": [arg_dict]},
+                ),
             )
         )
 
         copy_to_clipboard(out_lines)
 
     @property
     def bounds(self) -> dict[str, tuple[float, float]] | None:
@@ -393,15 +395,18 @@
                 avec,
                 reciprocal=self.reciprocal_check.isChecked(),
                 extend=(self.n1_spin.value(), self.n2_spin.value()),
             )
 
             if rot != 0.0:
                 rotmat = np.array(
-                    [[np.cos(rot), -np.sin(rot)], [np.sin(rot), np.cos(rot)]]
+                    [
+                        [np.cos(rot), -np.sin(rot)],
+                        [np.sin(rot), np.cos(rot)],
+                    ]
                 )
                 lines = (rotmat @ lines.transpose(1, 2, 0)).transpose(2, 0, 1)
                 vertices = (rotmat @ vertices.T).T
 
         return lines, vertices
 
     def closeEvent(self, event: QtGui.QCloseEvent):
```

### Comparing `erlab-2.1.0/src/erlab/interactive/ktool.ui` & `erlab-2.1.1/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/interactive/masktool.py` & `erlab-2.1.1/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/interactive/utilities.py` & `erlab-2.1.1/src/erlab/interactive/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 import xarray as xr
 from qtpy import QtCore, QtGui, QtWidgets
 from superqt import QDoubleSlider
 
 from erlab.interactive.colors import BetterImageItem, pg_colormap_powernorm
 
 __all__ = [
-    "parse_data",
-    "copy_to_clipboard",
-    "gen_single_function_code",
-    "gen_function_code",
-    "BetterSpinBox",
-    "BetterAxisItem",
-    "xImageItem",
-    "ParameterGroup",
     "AnalysisWidgetBase",
     "AnalysisWindow",
+    "BetterAxisItem",
+    "BetterSpinBox",
     "DictMenuBar",
+    "ParameterGroup",
+    "copy_to_clipboard",
+    "gen_function_code",
+    "gen_single_function_code",
+    "parse_data",
+    "xImageItem",
 ]
 
 
 def parse_data(data):
     if isinstance(data, xr.Dataset):
         raise TypeError(
             "input argument data must be a xarray.DataArray or a "
@@ -847,15 +847,15 @@
                     self.untracked.append(k)
                 self.widgets[k] = self.getParameterWidget(**v)
             elif isinstance(v, QtWidgets.QWidget):
                 showlabel = k
                 ind_eff = 1
                 self.widgets[k] = v
             else:
-                raise ValueError(
+                raise TypeError(
                     "Each value must be a QtWidgets.QWidget instance"
                     "or a dictionary of keyword arguments to getParameterWidget."
                 )
 
             self.labels.append(QtWidgets.QLabel(str(showlabel)))
             self.labels[i].setBuddy(self.widgets[k])
             if showlabel:
```

### Comparing `erlab-2.1.0/src/erlab/io/__init__.py` & `erlab-2.1.1/src/erlab/io/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -37,27 +37,27 @@
 
   >>> dat = erlab.io.loaders["merlin"].load(...)
 
 
 """
 
 __all__ = [
-    "loaders",
-    "set_loader",
-    "loader_context",
-    "set_data_dir",
     "load",
-    "summarize",
     "load_experiment",
-    "load_wave",
+    "load_hdf5",
     "load_live",
+    "load_wave",
+    "loader_context",
+    "loaders",
     "open_hdf5",
-    "load_hdf5",
     "save_as_hdf5",
     "save_as_netcdf",
+    "set_data_dir",
+    "set_loader",
+    "summarize",
 ]
 
 import warnings
 
 from erlab.io.dataloader import (
     load,
     loader_context,
```

### Comparing `erlab-2.1.0/src/erlab/io/dataloader.py` & `erlab-2.1.1/src/erlab/io/dataloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 loaders are plugins used to load data from various file formats. Each data loader that
 subclasses `LoaderBase` is registered on import in `loaders`.
 
 Loaded ARPES data must contain several attributes and coordinates. See the
 implementation of `LoaderBase.validate` for details.
 
 For any data loader plugin subclassing `LoaderBase`, the following attributes and
-methods must be defined: `LoaderBase.name`, `LoaderBase.aliases`,
-`LoaderBase.name_map`, `LoaderBase.coordinate_attrs`, `LoaderBase.additional_attrs`,
+methods must be defined: `LoaderBase.name`, `LoaderBase.aliases`, `LoaderBase.name_map`,
+`LoaderBase.coordinate_attrs`, `LoaderBase.additional_attrs`,
 `LoaderBase.always_single`, `LoaderBase.skip_validate`, :func:`LoaderBase.load_single`,
 :func:`LoaderBase.identify`, :func:`LoaderBase.infer_index`, and
 :func:`LoaderBase.generate_summary`.
 
+A detailed guide on how to implement a data loader can be found in
+:doc:`../user-guide/io`.
+
 If additional post-processing is required, the :func:`LoaderBase.post_process` method
 can be extended to include the necessary functionality.
 
 """
 
 from __future__ import annotations
 
@@ -85,15 +88,15 @@
     given here, both before and after renaming, will be removed from attrs for
     consistency.
     """
 
     additional_attrs: dict[str, str | int | float] = {}
     """Additional attributes to be added to the data."""
 
-    always_single: bool = False
+    always_single: bool = True
     """
     If `True`, this indicates that all individual scans always lead to a single data
     file. No concatenation of data from multiple files will be performed.
     """
 
     skip_validate: bool = False
     """If `True`, validation checks will be skipped."""
@@ -145,15 +148,15 @@
         if not cls.name.startswith("_"):
             LoaderRegistry.instance().register(cls)
 
     @classmethod
     def formatter(cls, val: object):
         """Format the given value based on its type.
 
-        This method is used when formtting the cells of the summary dataframe.
+        This method is used when formatting the cells of the summary dataframe.
 
         Parameters
         ----------
         val
             The value to be formatted.
 
         Returns
@@ -355,15 +358,15 @@
                 )
             elif len(file_paths) == 1:
                 # Single file resolved
                 data = self.load_single(file_paths[0])
             else:
                 # Multiple files resolved
                 data = self.combine_multiple(
-                    self._load_multiple_parallel(file_paths), coord_dict
+                    self.load_multiple_parallel(file_paths), coord_dict
                 )
         else:
             if data_dir is not None:
                 # Generate full path to file
                 identifier = os.path.join(data_dir, identifier)
 
             if not single:
@@ -396,25 +399,25 @@
         self, data_dir: str | os.PathLike, usecache: bool = True, **kwargs
     ) -> pandas.DataFrame:
         """
         Takes a path to a directory and summarizes the data in the directory to a
         `pandas.DataFrame`, much like a log file. This is useful for quickly inspecting
         the contents of a directory.
 
-        The dataframe is formatted using `get_styler` and displayed in the IPython
-        shell. Results are cached in a pickle file in the directory. If the pickle file
-        is not found, the summary is generated with `generate_summary` and cached.
+        The dataframe is formatted using the style from :meth:`get_styler
+        <erlab.io.dataloader.LoaderBase.get_styler>` and displayed in the IPython shell.
+        Results are cached in a pickle file in the directory.
 
         Parameters
         ----------
         data_dir
             Directory to summarize.
         usecache
             Whether to use the cached summary if available. If `False`, the summary will
-            be regenerated and cached.
+            be regenerated and the cache will be updated.
         **kwargs
             Additional keyword arguments to be passed to `generate_summary`.
 
         Returns
         -------
         pandas.DataFrame
             Summary of the data in the directory.
@@ -456,15 +459,15 @@
         Any scan-specific postprocessing should be implemented in this method. When the
         single file contains many regions, the method should return a single dataset
         whenever the data can be merged with `xarray.merge` without conflicts.
         Otherwise, a list of `xarray.DataArray`\ s should be returned.
 
         Parameters
         ----------
-        file_paths
+        file_path
             Full path to the file to be loaded.
 
         Returns
         -------
         xarray.DataArray or xarray.Dataset or list of xarray.DataArray
             The loaded data.
 
@@ -473,15 +476,18 @@
 
     def identify(
         self, num: int, data_dir: str | os.PathLike
     ) -> tuple[list[str], dict[str, Iterable]]:
         """Identify the files and coordinates for a given scan number.
 
         This method takes a scan index and transforms it into a list of file paths and
-        coordinates.
+        coordinates. For scans spread over multiple files, the coordinates must be a
+        dictionary mapping scan axes names to scan coordinates. For single file scans,
+        the list should contain only one file path and coordinates must be an empty
+        dictionary.
 
         Parameters
         ----------
         num
             The index of the scan to identify.
         data_dir
             The directory containing the data.
@@ -498,14 +504,17 @@
 
         """
         raise NotImplementedError("method must be implemented in the subclass")
 
     def infer_index(self, name: str) -> int | None:
         """Infer the index for the given file name.
 
+        This method takes a file name and tries to infer the scan index from it. If the
+        index can be inferred, it is returned; otherwise, `None` should be returned.
+
         Parameters
         ----------
         name
             The base name of the file without the path and extension.
 
         Returns
         -------
@@ -650,33 +659,48 @@
             if data.attrs["configuration"] not in (3, 4):
                 cls._raise_or_warn(
                     f"Invalid configuration {data.attrs['configuration']}"
                 )
             elif "chi" not in data.coords:
                 cls._raise_or_warn("Missing coordinate chi")
 
+    def load_multiple_parallel(
+        self, file_paths: list[str], n_jobs: int | None = None
+    ) -> list[xr.DataArray | xr.Dataset]:
+        """Load multiple files in parallel.
+
+        Parameters
+        ----------
+        file_paths
+            A list of file paths to load.
+        n_jobs
+            The number of jobs to run in parallel. If `None`, the number of jobs is set
+            to 1 for less than 15 files and to -1 (all CPU cores) for 15 or more files.
+
+        Returns
+        -------
+        A list of the loaded data.
+        """
+        if n_jobs is None:
+            if len(file_paths) < 15:
+                n_jobs = 1
+            else:
+                n_jobs = -1
+
+        return joblib.Parallel(n_jobs=n_jobs)(
+            joblib.delayed(self.load_single)(f) for f in file_paths
+        )
+
     @classmethod
     def _raise_or_warn(cls, msg: str):
         if cls.strict_validation:
             raise ValidationError(msg)
         else:
             warnings.warn(msg, ValidationWarning, stacklevel=2)
 
-    def _load_multiple_parallel(
-        self, file_paths: list[str]
-    ) -> list[xr.DataArray | xr.Dataset]:
-        if len(file_paths) < 15:
-            n_jobs = 1
-        else:
-            n_jobs = -1
-
-        return joblib.Parallel(n_jobs=n_jobs)(
-            joblib.delayed(self.load_single)(f) for f in file_paths
-        )
-
 
 class RegistryBase:
     """Base class for the loader registry.
 
     This class implements the singleton pattern, ensuring that only one instance of the
     registry is created and used throughout the application.
     """
@@ -709,16 +733,17 @@
 
     def register(self, loader_class: type[LoaderBase]):
         # Add class to loader
         self.loaders[loader_class.name] = loader_class
 
         # Add aliases to mapping
         self.alias_mapping[loader_class.name] = loader_class.name
-        for alias in loader_class.aliases:
-            self.alias_mapping[alias] = loader_class.name
+        if loader_class.aliases is not None:
+            for alias in loader_class.aliases:
+                self.alias_mapping[alias] = loader_class.name
 
     def get(self, key: str) -> LoaderBase:
         loader_name = self.alias_mapping.get(key)
         loader = self.loaders.get(loader_name)
 
         if loader is None:
             raise KeyError(f"Loader for {key} not found")
@@ -760,15 +785,15 @@
         """
         if isinstance(loader, str):
             self.current_loader = self.get(loader)
         else:
             self.current_loader = loader
 
     @contextlib.contextmanager
-    def loader_context(self, loader: str):
+    def loader_context(self, loader: str, data_dir: str | os.PathLike | None = None):
         """Context manager for temporarily changing the current data loader.
 
         The loader set here will only be used within the context manager.
 
         Parameters
         ----------
         loader
@@ -786,21 +811,29 @@
           >>> erlab.io.set_loader("ssrl52")
           >>> dat_ssrl_1 = erlab.io.load(...)
           >>> with erlab.io.loader_context("merlin"):
           ...     dat_merlin = erlab.io.load(...)
           >>> dat_ssrl_2 = erlab.io.load(...)
 
         """
-        old_loader: LoaderBase = self.current_loader
+        old_loader: LoaderBase | None = self.current_loader
         self.set_loader(loader)
+
+        if data_dir is not None:
+            old_data_dir = self.default_data_dir
+            self.set_data_dir(data_dir)
+
         try:
             yield self.current_loader
         finally:
             self.set_loader(old_loader)
 
+            if data_dir is not None:
+                self.set_data_dir(old_data_dir)
+
     def set_data_dir(self, data_dir: str | os.PathLike):
         """Set the default data directory for the data loader.
 
         All subsequent calls to `load` will use the `data_dir` set here unless
         specified.
 
         Parameters
```

### Comparing `erlab-2.1.0/src/erlab/io/igor.py` & `erlab-2.1.1/src/erlab/io/igor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 import os
 
 import h5netcdf
+import igor2.binarywave
+import igor2.packed
+import igor2.record
 import numpy as np
 import xarray as xr
 
-try:
-    import igor2.binarywave
-    import igor2.packed
-    import igor2.record
-
-except ImportError:
-    import warnings
-
-    warnings.warn(
-        "igor2 is not installed. Some functions may not work.",
-        ImportWarning,
-        stacklevel=1,
-    )
-
-__all__ = ["load_experiment", "load_h5", "load_wave", "load_pxp", "load_ibw"]
+__all__ = ["load_experiment", "load_igor_hdf5", "load_wave"]
 
 
 def _load_experiment_raw(
     filename: str | os.PathLike,
     folder: str | None = None,
     *,
     prefix: str | None = None,
@@ -109,15 +98,28 @@
             ignore=ignore,
             recursive=recursive,
             **kwargs,
         )
     )
 
 
-def load_h5(filename):
+def load_igor_hdf5(filename: str | os.PathLike) -> xr.Dataset:
+    """Load a HDF5 file exported by Igor Pro into an `xarray.Dataset`.
+
+    Parameters
+    ----------
+    filename
+        The path to the file.
+
+    Returns
+    -------
+    xarray.Dataset
+        The loaded data.
+
+    """
     ncf = h5netcdf.File(filename, mode="r", phony_dims="sort")
     ds = xr.open_dataset(xr.backends.H5NetCDFStore(ncf))
     for dv in ds.data_vars:
         wavescale = ds[dv].attrs["IGORWaveScaling"]
         ds = ds.assign_coords(
             {
                 dim: wavescale[i + 1, 1]
@@ -125,15 +127,15 @@
                 for i, dim in enumerate(ds[dv].dims)
             }
         )
     return ds
 
 
 def load_wave(
-    wave,  #: dict | igor2.record.WaveRecord | str | os.PathLike,
+    wave: dict | igor2.record.WaveRecord | str | os.PathLike,
     data_dir: str | os.PathLike | None = None,
 ) -> xr.DataArray:
     """Load a wave from Igor binary format.
 
     Parameters
     ----------
     wave
@@ -233,8 +235,11 @@
 
     return xr.DataArray(
         d["wData"], dims=coords.keys(), coords=coords, attrs=attrs
     ).rename(wave_header["bname"].decode())
 
 
 load_pxp = load_experiment
+"""Alias for :func:`load_experiment`."""
+
 load_ibw = load_wave
+"""Alias for :func:`load_wave`."""
```

### Comparing `erlab-2.1.0/src/erlab/io/plugins/__init__.py` & `erlab-2.1.1/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/io/plugins/da30.py` & `erlab-2.1.1/src/erlab/io/plugins/da30.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,21 +53,20 @@
 
         return data
 
 
 def load_zip(
     filename: str | os.PathLike,
 ) -> xr.DataArray | xr.Dataset | list[xr.DataArray]:
-    regions: list[str] = []
-
     with zipfile.ZipFile(filename) as z:
-        for fn in z.namelist():
-            if fn.startswith("Spectrum_") and fn.endswith(".bin"):
-                regions.append(fn[9:-4])
-
+        regions: list[str] = [
+            fn[9:-4]
+            for fn in z.namelist()
+            if fn.startswith("Spectrum_") and fn.endswith(".bin")
+        ]
         out = []
         for region in regions:
             with tempfile.TemporaryDirectory() as tmp_dir:
                 z.extract(f"Spectrum_{region}.ini", tmp_dir)
                 z.extract(f"{region}.ini", tmp_dir)
                 z.extract(f"Spectrum_{region}.bin", tmp_dir)
```

### Comparing `erlab-2.1.0/src/erlab/io/plugins/kriss.py` & `erlab-2.1.1/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/io/plugins/merlin.py` & `erlab-2.1.1/src/erlab/io/plugins/merlin.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         "polarization",
         "photon_flux",
     )
     additional_attrs: dict[str, str | int | float] = {
         "configuration": 1,
         "sample_workfunction": 4.44,
     }
+    always_single: bool = False
 
     def load_single(self, file_path: str | os.PathLike) -> xr.DataArray:
         data = load_experiment(file_path)
         # One file always corresponds to single region, so assume only one data variable
         data: xr.DataArray = data.data_vars[next(iter(data.data_vars.keys()))]
 
         return self.process_keys(data)
```

### Comparing `erlab-2.1.0/src/erlab/io/plugins/ssrl52.py` & `erlab-2.1.1/src/erlab/io/plugins/ssrl52.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,18 @@
 
         data_info = []
 
         for name, path in files.items():
             data = self.load(path)
 
             data_info.append(
-                [datetime.datetime.fromtimestamp(data.attrs["CreationTimeStamp"]), name]
+                [
+                    datetime.datetime.fromtimestamp(data.attrs["CreationTimeStamp"]),
+                    name,
+                ]
             )
 
             for k, v in summary_attrs.items():
                 try:
                     val = data.attrs[v]
                 except KeyError:
                     try:
```

### Comparing `erlab-2.1.0/src/erlab/io/utilities.py` & `erlab-2.1.1/src/erlab/io/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = [
-    "showfitsinfo",
     "get_files",
-    "open_hdf5",
     "load_hdf5",
+    "open_hdf5",
     "save_as_hdf5",
     "save_as_netcdf",
+    "showfitsinfo",
 ]
 
 import os
 import warnings
 from collections.abc import Sequence
 
 import numpy as np
@@ -164,31 +164,38 @@
     Parameters
     ----------
     data
         `xarray.DataArray` to save.
     filename
         Target file name.
     igor_compat
-        Make the resulting file compatible with Igor's `HDF5OpenFile`.
+        (*Experimental*) Make the resulting file compatible with Igor's `HDF5OpenFile` for DataArrays
+        with up to 4 dimensions. A convenient Igor procedure is `included in the
+        repository <https://github.com/kmnhan/erlabpy/blob/main/PythonInterface.ipf>`_.
+        Default is `True`.
     **kwargs
         Extra arguments to `xarray.DataArray.to_netcdf`: refer to the `xarray`
         documentation for a list of all possible arguments.
 
     """
     kwargs.setdefault("engine", "h5netcdf")
     kwargs.setdefault("invalid_netcdf", True)
 
     data = data.copy(deep=True)
     for k, v in data.attrs.items():
         if v is None:
             data = data.assign_attrs({k: "None"})
         if isinstance(v, dict):
             data = data.assign_attrs({k: str(v)})
+
     if isinstance(data, xr.Dataset):
         igor_compat = False
+    elif data.ndim > 4:
+        igor_compat = False
+
     if igor_compat:
         # IGORWaveScaling order: chunk row column layer
         scaling = [[1, 0]]
         for i in range(data.ndim):
             coord = data[data.dims[i]].values
             delta = coord[1] - coord[0]
             scaling.append([delta, coord[0]])
```

### Comparing `erlab-2.1.0/src/erlab/lattice.py` & `erlab-2.1.1/src/erlab/lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Tools related to the real and reciprocal lattice.
 
 .. currentmodule:: erlab.lattice
 
 """
 
-__all__ = ["angle_between", "abc2avec", "avec2abc", "to_reciprocal", "to_real"]
+__all__ = ["abc2avec", "angle_between", "avec2abc", "to_real", "to_reciprocal"]
 
 
 import numpy as np
 import numpy.typing as npt
 
 
 def angle_between(v1: npt.NDArray[np.float64], v2: npt.NDArray[np.float64]) -> float:
```

### Comparing `erlab-2.1.0/src/erlab/parallel.py` & `erlab-2.1.1/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.1.1/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.1.1/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.1.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.1.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.1.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.1.1/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.1.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.1.1/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.1.1/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.1.1/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/__init__.py` & `erlab-2.1.1/src/erlab/plotting/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,35 +46,44 @@
     importlib.import_module("cmasher")
 if importlib.util.find_spec("cmocean"):
     importlib.import_module("cmocean")
 if importlib.util.find_spec("colorcet"):
     importlib.import_module("colorcet")
 
 
-def load_igor_ct(fname, name):
+def load_igor_ct(fname: str, name: str) -> None:
+    """Load a Igor CT wave file (`.ibw`) and register as a matplotlib colormap.
+
+    Parameters
+    ----------
+    fname
+        Path to the Igor CT wave file.
+    name
+        The name to register the colormap as.
+
+    """
     file = pkgutil.get_data(__package__, "IgorCT/" + fname)
     if fname.endswith(".txt"):
         values = np.genfromtxt(io.StringIO(file.decode()))
     elif fname.endswith(".ibw"):
         values = erlab.io.load_wave(io.BytesIO(file)).values
 
     cmap = matplotlib.colors.LinearSegmentedColormap.from_list(name, values / 65535)
     matplotlib.colormaps.register(cmap)
     matplotlib.colormaps.register(cmap.reversed())
 
 
-if importlib.util.find_spec("igor2"):
-    load_igor_ct("CTBlueWhite.ibw", "BuWh")
-    load_igor_ct("CTRainbowLIght.ibw", "RainbowLight")
-    # load_igor_ct("CTRedTemperature.ibw", "RedTemperature")
-    load_igor_ct("ColdWarm.ibw", "ColdWarm")
-    load_igor_ct("BlueHot.ibw", "BlueHot")
-    # load_igor_ct("PlanetEarth.ibw", "PlanetEarth")
-    # load_igor_ct("ametrine.ibw", "ametrine")
-    # load_igor_ct("isolum.ibw", "isolum")
-    # load_igor_ct("morgenstemning.ibw", "morgenstemning")
+load_igor_ct("CTBlueWhite.ibw", "BuWh")
+load_igor_ct("CTRainbowLIght.ibw", "RainbowLight")
+# load_igor_ct("CTRedTemperature.ibw", "RedTemperature")
+load_igor_ct("ColdWarm.ibw", "ColdWarm")
+load_igor_ct("BlueHot.ibw", "BlueHot")
+# load_igor_ct("PlanetEarth.ibw", "PlanetEarth")
+# load_igor_ct("ametrine.ibw", "ametrine")
+# load_igor_ct("isolum.ibw", "isolum")
+# load_igor_ct("morgenstemning.ibw", "morgenstemning")
 
 
 matplotlib.style.core.USER_LIBRARY_PATHS.append(
     os.path.join(os.path.dirname(__file__), "stylelib")
 )
 matplotlib.style.core.reload_library()
```

### Comparing `erlab-2.1.0/src/erlab/plotting/annotations.py` & `erlab-2.1.1/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/atoms.py` & `erlab-2.1.1/src/erlab/plotting/atoms.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,27 +383,31 @@
             masked_atom_pos[k] = np.asarray(
                 [p for i, p in enumerate(v) if i in valid[k][0]]
             )
         return masked_atom_pos
 
     @property
     def _color_array(self) -> tuple[npt.NDArray[np.str_]]:
-        clr_arr = []
-        for k, v in self.atom_pos.items():
-            for _ in range(len(v)):
-                clr_arr.append(self.atom_color[k])
-        return np.asarray(clr_arr)
+        return np.asarray(
+            [
+                self.atom_color[k]
+                for k, v in self.atom_pos.items()
+                for _ in range(len(v))
+            ]
+        )
 
     @property
     def _size_array(self) -> tuple[npt.NDArray[np.float64]]:
-        sz_arr = []
-        for k, v in self.atom_pos.items():
-            for _ in range(len(v)):
-                sz_arr.append(self.atom_radii[k])
-        return np.asarray(sz_arr)
+        return np.asarray(
+            [
+                self.atom_radii[k]
+                for k, v in self.atom_pos.items()
+                for _ in range(len(v))
+            ]
+        )
 
     @property
     def _atom_pos_array(self) -> npt.NDArray[np.float64]:
         return np.r_[*list(self.atom_pos.values())]
 
     def clear_bonds(self) -> None:
         self.segments.clear()
```

### Comparing `erlab-2.1.0/src/erlab/plotting/bz.py` & `erlab-2.1.1/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/colors.py` & `erlab-2.1.1/src/erlab/plotting/colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,30 +22,30 @@
    :width: 65 %
 
    Demonstration of `CenteredPowerNorm` and `CenteredInversePowerNorm`.
 
 """
 
 __all__ = [
-    "InversePowerNorm",
-    "TwoSlopePowerNorm",
+    "CenteredInversePowerNorm",
     "CenteredPowerNorm",
+    "InversePowerNorm",
     "TwoSlopeInversePowerNorm",
-    "CenteredInversePowerNorm",
-    "get_mappable",
-    "unify_clim",
-    "proportional_colorbar",
-    "nice_colorbar",
+    "TwoSlopePowerNorm",
+    "axes_textcolor",
+    "close_to_white",
+    "color_distance",
     "flatten_transparency",
     "gen_2d_colormap",
-    "color_distance",
-    "close_to_white",
-    "prominent_color",
+    "get_mappable",
     "image_is_light",
-    "axes_textcolor",
+    "nice_colorbar",
+    "prominent_color",
+    "proportional_colorbar",
+    "unify_clim",
 ]
 
 from collections.abc import Iterable, Sequence
 from numbers import Number
 from typing import Literal
 
 import matplotlib
@@ -467,24 +467,26 @@
         If `False`, raises a `RuntimeError`. If `True`, silently returns `None`.
 
     Returns
     -------
     matplotlib.cm.ScalarMappable or None
 
     """
-    try:
-        if not image_only:
+    if not image_only:
+        try:
             mappable = ax.collections[-1]
-        else:
-            raise AttributeError
-    except (IndexError, AttributeError):
+        except (IndexError, AttributeError):
+            mappable = None
+
+    if image_only or mappable is None:
         try:
             mappable = ax.get_images()[-1]
         except (IndexError, AttributeError):
             mappable = None
+
     if not silent and mappable is None:
         raise RuntimeError(
             "No mappable was found to use for colorbar "
             "creation. First define a mappable such as "
             "an image (with imshow) or a contour set ("
             "with contourf)."
         )
```

### Comparing `erlab-2.1.0/src/erlab/plotting/erplot.py` & `erlab-2.1.1/src/erlab/plotting/erplot.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """Convenient access to various plotting functions."""
 
 __all__ = [
+    "CenteredInversePowerNorm",
+    "CenteredPowerNorm",
+    "InversePowerNorm",
+    "TwoSlopeInversePowerNorm",
+    "TwoSlopePowerNorm",
+    "autoscale_to",
     "copy_mathtext",
     "fancy_labels",
+    "fermiline",
+    "figwh",
+    "flatten_transparency",
+    "get_bz_edge",
+    "get_mappable",
+    "gradient_fill",
+    "image_is_light",
     "label_subplot_properties",
     "label_subplots",
     "label_subplots_nature",
     "mark_points",
     "mark_points_outside",
+    "nice_colorbar",
+    "place_inset",
+    "plot_array",
+    "plot_array_2d",
+    "plot_hex_bz",
     "plot_hv_text",
+    "plot_slices",
     "property_label",
+    "proportional_colorbar",
     "scale_units",
     "set_titles",
     "set_xlabels",
     "set_ylabels",
     "sizebar",
-    "get_bz_edge",
-    "plot_hex_bz",
-    "InversePowerNorm",
-    "TwoSlopePowerNorm",
-    "CenteredPowerNorm",
-    "TwoSlopeInversePowerNorm",
-    "CenteredInversePowerNorm",
-    "get_mappable",
     "unify_clim",
-    "flatten_transparency",
-    "image_is_light",
-    "nice_colorbar",
-    "proportional_colorbar",
-    "fermiline",
-    "figwh",
-    "autoscale_to",
-    "place_inset",
-    "plot_array",
-    "plot_array_2d",
-    "gradient_fill",
-    "plot_slices",
 ]
 
 import numpy as np
 
 from erlab.plotting.annotations import (
     copy_mathtext,
     fancy_labels,
```

### Comparing `erlab-2.1.0/src/erlab/plotting/general.py` & `erlab-2.1.1/src/erlab/plotting/general.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """General plotting utilities."""
 
 from __future__ import annotations
 
 __all__ = [
-    "figwh",
+    "LabeledCursor",
     "autoscale_off",
     "autoscale_to",
-    "LabeledCursor",
+    "fermiline",
+    "figwh",
+    "gradient_fill",
     "place_inset",
     "plot_array",
     "plot_array_2d",
-    "gradient_fill",
     "plot_slices",
-    "fermiline",
 ]
 
 import contextlib
 import copy
 from typing import TYPE_CHECKING, Literal
 
 import matplotlib
```

### Comparing `erlab-2.1.0/src/erlab/plotting/plot3d.py` & `erlab-2.1.1/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.1.1/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.1.1/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.1.1/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.1.1/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.1.1/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.1.1/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/src/erlab.egg-info/PKG-INFO` & `erlab-2.1.1/src/erlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.1.0/src/erlab.egg-info/SOURCES.txt` & `erlab-2.1.1/src/erlab.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 docs/source/erlab.lattice.rst
 docs/source/erlab.parallel.rst
 docs/source/erlab.plotting.rst
 docs/source/getting-started.rst
 docs/source/index.rst
 docs/source/reference.rst
 docs/source/refs.bib
+docs/source/images/flowchart_multiple.pdf
+docs/source/images/flowchart_single.pdf
 docs/source/images/imagetool_dark.png
 docs/source/images/imagetool_light.png
 docs/source/images/ktool_1_dark.png
 docs/source/images/ktool_1_light.png
 docs/source/images/ktool_2_dark.png
 docs/source/images/ktool_2_light.png
 docs/source/pyplots/norms.py
@@ -129,14 +131,14 @@
 src/erlab/plotting/stylelib/khan.mplstyle
 src/erlab/plotting/stylelib/nature.mplstyle
 src/erlab/plotting/stylelib/poster.mplstyle
 src/erlab/plotting/stylelib/times.mplstyle
 templates/.macros.j2
 templates/.release_notes.md.j2
 templates/CHANGELOG.md.j2
-tests/test_fastbinning.py
-tests/test_fit_functions_dynamic.py
-tests/test_fit_functions_general.py
-tests/test_image.py
-tests/test_interpolate.py
-tests/test_kspace.py
-tests/test_utilities.py
+tests/analysis/test_fastbinning.py
+tests/analysis/test_fit_functions_dynamic.py
+tests/analysis/test_fit_functions_general.py
+tests/analysis/test_image.py
+tests/analysis/test_interpolate.py
+tests/analysis/test_kspace.py
+tests/analysis/test_utilities.py
```

### Comparing `erlab-2.1.0/src/erlab.egg-info/requires.txt` & `erlab-2.1.1/src/erlab.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/templates/.macros.j2` & `erlab-2.1.1/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/tests/test_fastbinning.py` & `erlab-2.1.1/tests/analysis/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/tests/test_fit_functions_dynamic.py` & `erlab-2.1.1/tests/analysis/test_fit_functions_dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/tests/test_fit_functions_general.py` & `erlab-2.1.1/tests/analysis/test_fit_functions_general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/tests/test_image.py` & `erlab-2.1.1/tests/analysis/test_image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/tests/test_interpolate.py` & `erlab-2.1.1/tests/analysis/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.0/tests/test_kspace.py` & `erlab-2.1.1/tests/analysis/test_kspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,23 +47,23 @@
 
         kx, ky = forward_func(*inverse_func(0.1, 0.2))
         assert kx.size == ky.size == k_tot.size
         assert np.allclose(kx, 0.1)
         assert np.allclose(ky, 0.2)
 
 
-@pytest.fixture
+@pytest.fixture()
 def angle_data():
     return generate_data_angles(shape=(10, 10, 10))
 
 
 def test_offsets(angle_data):
     angle_data.kspace.offsets.reset()
     angle_data.kspace.offsets = {"xi": 10.0}
-    answer = {k: 0.0 for k in angle_data.kspace.valid_offset_keys}
+    answer = dict.fromkeys(angle_data.kspace.valid_offset_keys, 0.0)
     answer["xi"] = 10.0
     assert dict(angle_data.kspace.offsets) == answer
 
 
 def test_kconv(angle_data):
     for conf in erlab.analysis.kspace.AxesConfiguration:
         angle_data.kspace.configuration = conf
```

### Comparing `erlab-2.1.0/tests/test_utilities.py` & `erlab-2.1.1/tests/analysis/test_utilities.py`

 * *Files identical despite different names*

