# Comparing `tmp/erlab-2.1.1.tar.gz` & `tmp/erlab-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.1.1.tar", last modified: Wed Apr 10 12:00:58 2024, max compression
+gzip compressed data, was "erlab-2.1.2.tar", last modified: Thu Apr 11 01:29:22 2024, max compression
```

## Comparing `erlab-2.1.1.tar` & `erlab-2.1.2.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.389099 erlab-2.1.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.345099 erlab-2.1.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.349099 erlab-2.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-10 12:00:52.000000 erlab-2.1.1/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 root         (0) root         (0)      608 2024-04-10 12:00:52.000000 erlab-2.1.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.349099 erlab-2.1.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-10 12:00:52.000000 erlab-2.1.1/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-10 12:00:52.000000 erlab-2.1.1/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-10 12:00:52.000000 erlab-2.1.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-10 12:00:52.000000 erlab-2.1.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      796 2024-04-10 12:00:52.000000 erlab-2.1.1/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   103668 2024-04-10 12:00:54.000000 erlab-2.1.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-04-10 12:00:52.000000 erlab-2.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    47662 2024-04-10 12:00:58.389099 erlab-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-10 12:00:52.000000 erlab-2.1.1/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     4703 2024-04-10 12:00:52.000000 erlab-2.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.353099 erlab-2.1.1/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      655 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.357099 erlab-2.1.1/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    16011 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    14522 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      265 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.characterization.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     3806 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.361099 erlab-2.1.1/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   294466 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/flowchart_multiple.pdf
--rw-r--r--   0 root         (0) root         (0)   291044 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/flowchart_single.pdf
--rw-r--r--   0 root         (0) root         (0)   996803 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     2665 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.365099 erlab-2.1.1/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2578 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1344 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     2342 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.365099 erlab-2.1.1/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)     1222 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)     5063 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)    18148 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)   379543 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    15771 2024-04-10 12:00:52.000000 erlab-2.1.1/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-10 12:00:52.000000 erlab-2.1.1/environment.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-10 12:00:52.000000 erlab-2.1.1/environment_apple.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-10 12:00:52.000000 erlab-2.1.1/environment_nogit.yml
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-10 12:00:52.000000 erlab-2.1.1/environment_nogit_mkl.yml
--rw-r--r--   0 root         (0) root         (0)     4373 2024-04-10 12:00:52.000000 erlab-2.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-10 12:00:52.000000 erlab-2.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 12:00:58.389099 erlab-2.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.345099 erlab-2.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.365099 erlab-2.1.1/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-10 12:00:54.000000 erlab-2.1.1/src/erlab/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35543 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/accessors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.369099 erlab-2.1.1/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5514 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.369099 erlab-2.1.1/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      459 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.369099 erlab-2.1.1/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      839 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9632 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     6026 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)     9881 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1168 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    15448 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    17325 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10629 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.369099 erlab-2.1.1/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     5401 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8440 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     8658 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.373099 erlab-2.1.1/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      191 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.373099 erlab-2.1.1/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      540 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13953 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    20867 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    22451 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11443 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)     9458 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/exampledata.py
--rw-r--r--   0 root         (0) root         (0)    19072 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.377099 erlab-2.1.1/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    19396 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.377099 erlab-2.1.1/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51945 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114560 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27081 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    54122 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    13907 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25270 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    15835 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19382 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     3341 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    54143 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.377099 erlab-2.1.1/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     1937 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31715 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6905 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.377099 erlab-2.1.1/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3667 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     7480 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7804 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     6559 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.381099 erlab-2.1.1/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.381099 erlab-2.1.1/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     2026 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29010 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18284 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    32437 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    31070 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.385099 erlab-2.1.1/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-04-10 12:00:52.000000 erlab-2.1.1/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.385099 erlab-2.1.1/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    47662 2024-04-10 12:00:58.000000 erlab-2.1.1/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4675 2024-04-10 12:00:58.000000 erlab-2.1.1/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 12:00:58.000000 erlab-2.1.1/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      536 2024-04-10 12:00:58.000000 erlab-2.1.1/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-10 12:00:58.000000 erlab-2.1.1/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.385099 erlab-2.1.1/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-10 12:00:52.000000 erlab-2.1.1/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-04-10 12:00:52.000000 erlab-2.1.1/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-04-10 12:00:52.000000 erlab-2.1.1/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.349099 erlab-2.1.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:00:58.385099 erlab-2.1.1/tests/analysis/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_fit_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_fit_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     5228 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_image.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     2423 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-10 12:00:52.000000 erlab-2.1.1/tests/analysis/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.202324 erlab-2.1.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.158324 erlab-2.1.2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.162324 erlab-2.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-11 01:29:15.000000 erlab-2.1.2/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-11 01:29:15.000000 erlab-2.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.162324 erlab-2.1.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-11 01:29:15.000000 erlab-2.1.2/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-11 01:29:15.000000 erlab-2.1.2/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-11 01:29:15.000000 erlab-2.1.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-11 01:29:15.000000 erlab-2.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      796 2024-04-11 01:29:15.000000 erlab-2.1.2/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   104651 2024-04-11 01:29:18.000000 erlab-2.1.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-04-11 01:29:15.000000 erlab-2.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    47782 2024-04-11 01:29:22.202324 erlab-2.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-11 01:29:15.000000 erlab-2.1.2/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     4823 2024-04-11 01:29:15.000000 erlab-2.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.166324 erlab-2.1.2/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      655 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.170324 erlab-2.1.2/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    16011 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    14522 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.characterization.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     3806 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.174324 erlab-2.1.2/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   321080 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   317804 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     3285 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.178324 erlab-2.1.2/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2578 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.178324 erlab-2.1.2/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)     5063 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    50371 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)   379705 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    16193 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-11 01:29:15.000000 erlab-2.1.2/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-11 01:29:15.000000 erlab-2.1.2/environment_apple.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-11 01:29:15.000000 erlab-2.1.2/environment_nogit.yml
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-11 01:29:15.000000 erlab-2.1.2/environment_nogit_mkl.yml
+-rw-r--r--   0 root         (0) root         (0)     4373 2024-04-11 01:29:15.000000 erlab-2.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-11 01:29:15.000000 erlab-2.1.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 01:29:22.202324 erlab-2.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.158324 erlab-2.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.178324 erlab-2.1.2/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-11 01:29:18.000000 erlab-2.1.2/src/erlab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35543 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/accessors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.182324 erlab-2.1.2/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.182324 erlab-2.1.2/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      459 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.182324 erlab-2.1.2/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      839 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9632 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     6026 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)     9881 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    15448 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    17325 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10629 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.186324 erlab-2.1.2/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     5401 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8440 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     8658 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.186324 erlab-2.1.2/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.186324 erlab-2.1.2/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13953 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    20867 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    22451 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11443 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)     9458 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)    19072 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.190324 erlab-2.1.2/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    19396 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.190324 erlab-2.1.2/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51945 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114560 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27081 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    54122 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    13907 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25270 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    15835 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     3341 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    54143 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.190324 erlab-2.1.2/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32013 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.190324 erlab-2.1.2/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3667 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     7594 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7804 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     6559 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.194324 erlab-2.1.2/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.194324 erlab-2.1.2/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29010 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18284 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    32437 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    31070 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.198324 erlab-2.1.2/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.198324 erlab-2.1.2/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    47782 2024-04-11 01:29:22.000000 erlab-2.1.2/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4675 2024-04-11 01:29:22.000000 erlab-2.1.2/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 01:29:22.000000 erlab-2.1.2/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      536 2024-04-11 01:29:22.000000 erlab-2.1.2/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-11 01:29:22.000000 erlab-2.1.2/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.198324 erlab-2.1.2/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-11 01:29:15.000000 erlab-2.1.2/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-11 01:29:15.000000 erlab-2.1.2/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-11 01:29:15.000000 erlab-2.1.2/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.162324 erlab-2.1.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.198324 erlab-2.1.2/tests/analysis/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_fit_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_fit_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_utilities.py
```

### Comparing `erlab-2.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `erlab-2.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/.github/workflows/pr.yml` & `erlab-2.1.2/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/.github/workflows/release.yml` & `erlab-2.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/.gitignore` & `erlab-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/.pre-commit-config.yaml` & `erlab-2.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/.readthedocs.yaml` & `erlab-2.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/CHANGELOG.md` & `erlab-2.1.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # CHANGELOG
 
 
 
+## v2.1.2 (2024-04-11)
+
+### Documentation
+
+* update syntax ([`2b72991`](https://github.com/kmnhan/erlabpy/commit/2b7299150a50af38e6e05d5f9690558cbeb7a9ad))
+
+* improve intro pages ([`ec2a4f8`](https://github.com/kmnhan/erlabpy/commit/ec2a4f816e1ad0ed1ad154d6544e91bea1b5d9c5))
+
+* (**io**) add complete data loading examples ([`63e88c4`](https://github.com/kmnhan/erlabpy/commit/63e88c40b14584214cd45bd0258f8ef7a32d716c))
+
+* (**io**) simplify flowchart ([`355d023`](https://github.com/kmnhan/erlabpy/commit/355d02374e11f7a78b87f8d3159f288a1d15d22d))
+
+### Fix
+
+* (**io**) prevent specifying invalid data_dir ([`701b011`](https://github.com/kmnhan/erlabpy/commit/701b011339ecba657a0f4a14e2fef19adeb4bf2b))
+
+* (**io**) fixes merlin summary data type resolving ([`a91ad3d`](https://github.com/kmnhan/erlabpy/commit/a91ad3d4387a23d25ac1b208cba8217e67efbec0))
+
+* (**io**) fix summary loading ([`a5dd84a`](https://github.com/kmnhan/erlabpy/commit/a5dd84af9eec0f835b3116bc7c470e57ef3f3e02))
+
+
 ## v2.1.1 (2024-04-10)
 
 ### Documentation
 
 * (**io**) improve docstrings and user guide ([`8e69abb`](https://github.com/kmnhan/erlabpy/commit/8e69abb37a99818081bf2e03453d64e1b48b16ab))
 
 * update io documentation ([`b0d2d01`](https://github.com/kmnhan/erlabpy/commit/b0d2d01d0dec2ec8180cb5d7da2034900d0d0aba))
```

### Comparing `erlab-2.1.1/LICENSE` & `erlab-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/PKG-INFO` & `erlab-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -742,49 +742,50 @@
 [![Workflow Status](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml/badge.svg)](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml)
 [![Documentation Status](https://readthedocs.org/projects/erlabpy/badge/)](https://erlabpy.readthedocs.io/)
 [![License](https://img.shields.io/pypi/l/erlab)](https://github.com/kmnhan/erlabpy/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/kmnhan/erlabpy/main.svg)](https://results.pre-commit.ci/latest/github/kmnhan/erlabpy/main)
 
 A library that provides a set of tools and utilities to handle, manipulate, and
-visualize data from condensed matter physics experiments, with a focus on
-angle-resolved photoemission spectroscopy (ARPES).
+visualize data from condensed matter physics experiments, with a focus on angle-resolved
+photoemission spectroscopy (ARPES).
 
 *ERLabPy* is built on top of the popular scientific computing libraries
 [*numpy*](https://numpy.org/), [*scipy*](https://scipy.org/), and
-[*xarray*](https://xarray.pydata.org/), and is designed to be easy to use and
-integrate with existing scientific Python workflows. It is also designed to be
-extensible, allowing users to easily add custom functionality and analysis
-tools.
+[*xarray*](https://xarray.pydata.org/), and is designed to be easy to use and integrate
+with existing scientific Python workflows so that you can quickly get started with your
+data analysis. The package is still under development, so if you have any questions or
+suggestions, please feel free to contact us. We hope you find ERLabPy useful for your
+research!
 
 *ERLabPy* is developed and maintained by the electronic structure research
 laboratory at Korea Advanced Institute of Science and Technology (KAIST).
 
 ## Features
 
-- **Data Loading**: A flexible and extensible data loading system is included,
-  capable of handling various data formats.
+- **Data Loading**: A flexible and extensible data loading system is included, capable
+  of handling various data formats.
 - **Data Manipulation**: A set of tools for manipulating and transforming data,
   including interpolation, masking and symmetrization is provided.
-- **Plotting**: ERLabPy provides many different plotting functions for
-  visualizing image data, including 2D and 3D plots. Publication-quality plots
-  can be generated with minimal effort.
-- **Fitting**: Several functions and models are implemented for fitting various
-  types of data, including broadened Fermi-Dirac distributions, momentum
-  distribution curves (MDCs), and energy distribution curves (EDCs).
+- **Plotting**: ERLabPy provides many different plotting functions for visualizing image
+  data, including 2D and 3D plots. Publication-quality plots can be generated with
+  minimal effort.
+- **Fitting**: Several functions and models are implemented for fitting various types of
+  data, including broadened Fermi-Dirac distributions, momentum distribution curves
+  (MDCs), and energy distribution curves (EDCs).
 - **Interactive Data Visualization**: ERLabPy includes many interactive plotting
-  routines that resemble panels in Igor Pro that are very responsive and easy to
-  use. See screenshots below.
+  routines that resemble panels in Igor Pro that are very responsive and easy to use.
+  See screenshots below.
 - **Active Development**: ERLabPy is actively developed and maintained, with new
   features and improvements being added regularly.
 
 ## Screenshots
 
-Most interactive windows support dark mode. Viewing this page from a supported
-browser with dark mode enabled will show the dark mode screenshots.
+Most interactive windows support dark mode. Viewing this page from a supported browser
+with dark mode enabled will show the dark mode screenshots.
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/imagetool_dark.png?raw=true">
   <source media="(prefers-color-scheme: light)" srcset="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/imagetool_light.png?raw=true">
   <img alt="Imagetool in action." src="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/imagetool_light.png?raw=true">
 </picture>
 
@@ -801,18 +802,18 @@
 
 ## Documentation
 
 The full documentation for ERLabPy is available on [Read the Docs](https://erlabpy.readthedocs.io/).
 
 ## Contributing
 
-ERLabPy is an open-source project and we welcome contributions from the
-community. If you find any bugs, issues, or have any suggestions, please open an
-issue [here](https://github.com/kmnhan/erlabpy/issues). If you would like to add
-a new feature or fix a bug yourself, we would love to have your contribution.
-Feel free to fork the repository and submit a pull request with your changes.
+ERLabPy is an open-source project and we welcome contributions from the community. If
+you find any bugs, issues, or have any suggestions, please open an issue
+[here](https://github.com/kmnhan/erlabpy/issues). If you would like to add a new feature
+or fix a bug yourself, we would love to have your contribution. Feel free to fork the
+repository and submit a pull request with your changes.
 
 For more information on contributing, see our [Contributing page](https://erlabpy.readthedocs.io/en/stable/contributing.html).
 
 ## License
 
 This project is licensed under the terms of the [GPL-3.0 License](LICENSE).
```

### Comparing `erlab-2.1.1/PythonInterface.ipf` & `erlab-2.1.2/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/README.md` & `erlab-2.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,49 +5,50 @@
 [![Workflow Status](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml/badge.svg)](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml)
 [![Documentation Status](https://readthedocs.org/projects/erlabpy/badge/)](https://erlabpy.readthedocs.io/)
 [![License](https://img.shields.io/pypi/l/erlab)](https://github.com/kmnhan/erlabpy/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/kmnhan/erlabpy/main.svg)](https://results.pre-commit.ci/latest/github/kmnhan/erlabpy/main)
 
 A library that provides a set of tools and utilities to handle, manipulate, and
-visualize data from condensed matter physics experiments, with a focus on
-angle-resolved photoemission spectroscopy (ARPES).
+visualize data from condensed matter physics experiments, with a focus on angle-resolved
+photoemission spectroscopy (ARPES).
 
 *ERLabPy* is built on top of the popular scientific computing libraries
 [*numpy*](https://numpy.org/), [*scipy*](https://scipy.org/), and
-[*xarray*](https://xarray.pydata.org/), and is designed to be easy to use and
-integrate with existing scientific Python workflows. It is also designed to be
-extensible, allowing users to easily add custom functionality and analysis
-tools.
+[*xarray*](https://xarray.pydata.org/), and is designed to be easy to use and integrate
+with existing scientific Python workflows so that you can quickly get started with your
+data analysis. The package is still under development, so if you have any questions or
+suggestions, please feel free to contact us. We hope you find ERLabPy useful for your
+research!
 
 *ERLabPy* is developed and maintained by the electronic structure research
 laboratory at Korea Advanced Institute of Science and Technology (KAIST).
 
 ## Features
 
-- **Data Loading**: A flexible and extensible data loading system is included,
-  capable of handling various data formats.
+- **Data Loading**: A flexible and extensible data loading system is included, capable
+  of handling various data formats.
 - **Data Manipulation**: A set of tools for manipulating and transforming data,
   including interpolation, masking and symmetrization is provided.
-- **Plotting**: ERLabPy provides many different plotting functions for
-  visualizing image data, including 2D and 3D plots. Publication-quality plots
-  can be generated with minimal effort.
-- **Fitting**: Several functions and models are implemented for fitting various
-  types of data, including broadened Fermi-Dirac distributions, momentum
-  distribution curves (MDCs), and energy distribution curves (EDCs).
+- **Plotting**: ERLabPy provides many different plotting functions for visualizing image
+  data, including 2D and 3D plots. Publication-quality plots can be generated with
+  minimal effort.
+- **Fitting**: Several functions and models are implemented for fitting various types of
+  data, including broadened Fermi-Dirac distributions, momentum distribution curves
+  (MDCs), and energy distribution curves (EDCs).
 - **Interactive Data Visualization**: ERLabPy includes many interactive plotting
-  routines that resemble panels in Igor Pro that are very responsive and easy to
-  use. See screenshots below.
+  routines that resemble panels in Igor Pro that are very responsive and easy to use.
+  See screenshots below.
 - **Active Development**: ERLabPy is actively developed and maintained, with new
   features and improvements being added regularly.
 
 ## Screenshots
 
-Most interactive windows support dark mode. Viewing this page from a supported
-browser with dark mode enabled will show the dark mode screenshots.
+Most interactive windows support dark mode. Viewing this page from a supported browser
+with dark mode enabled will show the dark mode screenshots.
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/imagetool_dark.png?raw=true">
   <source media="(prefers-color-scheme: light)" srcset="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/imagetool_light.png?raw=true">
   <img alt="Imagetool in action." src="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/imagetool_light.png?raw=true">
 </picture>
 
@@ -64,18 +65,18 @@
 
 ## Documentation
 
 The full documentation for ERLabPy is available on [Read the Docs](https://erlabpy.readthedocs.io/).
 
 ## Contributing
 
-ERLabPy is an open-source project and we welcome contributions from the
-community. If you find any bugs, issues, or have any suggestions, please open an
-issue [here](https://github.com/kmnhan/erlabpy/issues). If you would like to add
-a new feature or fix a bug yourself, we would love to have your contribution.
-Feel free to fork the repository and submit a pull request with your changes.
+ERLabPy is an open-source project and we welcome contributions from the community. If
+you find any bugs, issues, or have any suggestions, please open an issue
+[here](https://github.com/kmnhan/erlabpy/issues). If you would like to add a new feature
+or fix a bug yourself, we would love to have your contribution. Feel free to fork the
+repository and submit a pull request with your changes.
 
 For more information on contributing, see our [Contributing page](https://erlabpy.readthedocs.io/en/stable/contributing.html).
 
 ## License
 
 This project is licensed under the terms of the [GPL-3.0 License](LICENSE).
```

### Comparing `erlab-2.1.1/docs/Makefile` & `erlab-2.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/environment.yml` & `erlab-2.1.2/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/make.bat` & `erlab-2.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/conf.py` & `erlab-2.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/contributing.rst` & `erlab-2.1.2/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/getting-started.rst` & `erlab-2.1.2/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/images/flowchart_multiple.pdf` & `erlab-2.1.2/docs/source/images/flowchart_multiple.pdf`

 * *Files 11% similar despite different names*

#### Comparing `erlab-2.1.1/docs/source/images/flowchart_multiple.pdf` & `erlab-2.1.2/docs/source/images/flowchart_multiple.pdf`

 * *Document info*

```diff
@@ -1,6 +1,6 @@
-CreationDate: "D:20240410143522+09'00'"
+CreationDate: "D:20240411075630+09'00'"
 Creator: 'Adobe Illustrator 28.4 (Macintosh)'
 CreatorVersion: '21.0.0'
-ModDate: "D:20240410143522+09'00'"
+ModDate: "D:20240411075630+09'00'"
 Producer: 'Adobe PDF library 17.00'
 Title: 'flowchart_multiple'
```

#### pdftotext {} -

```diff
@@ -1,43 +1,43 @@
 load(identifier, data_dir, single)
 
 Loader base class methods
 
 Loader methods (requires overriding)
 construct file path from
+identifier & data_dir
 
 False
 
-identifier & data_dir
-
 is identifier an integer?
 True
 
-False
-
 single ?
 
-infer_index
+False
 
+infer_index
 identify
 
 True
+
+failed to infer?
+True
+
 False
 
-resolved index integer?
+single file?
+
 True
 
 load_single
 
 post_process
 
-False
+loaded data
 
-multiple files?
-True
+False
 
 load_multiple_parallel
-loaded data
-
 combine_multiple
```

### Comparing `erlab-2.1.1/docs/source/images/flowchart_single.pdf` & `erlab-2.1.2/docs/source/images/flowchart_single.pdf`

 * *Files 11% similar despite different names*

#### Comparing `erlab-2.1.1/docs/source/images/flowchart_single.pdf` & `erlab-2.1.2/docs/source/images/flowchart_single.pdf`

 * *Document info*

```diff
@@ -1,6 +1,6 @@
-CreationDate: "D:20240410143522+09'00'"
+CreationDate: "D:20240411075630+09'00'"
 Creator: 'Adobe Illustrator 28.4 (Macintosh)'
 CreatorVersion: '21.0.0'
-ModDate: "D:20240410143522+09'00'"
+ModDate: "D:20240411075630+09'00'"
 Producer: 'Adobe PDF library 17.00'
 Title: 'flowchart_single'
```

### Comparing `erlab-2.1.1/docs/source/images/imagetool_dark.png` & `erlab-2.1.2/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/images/imagetool_light.png` & `erlab-2.1.2/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/images/ktool_1_dark.png` & `erlab-2.1.2/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/images/ktool_1_light.png` & `erlab-2.1.2/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/images/ktool_2_dark.png` & `erlab-2.1.2/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/images/ktool_2_light.png` & `erlab-2.1.2/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/index.rst` & `erlab-2.1.2/docs/source/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -28,55 +28,67 @@
        :target: https://results.pre-commit.ci/latest/github/kmnhan/erlabpy/main
        :alt: pre-commit.ci status
 
 A library that provides a set of tools and utilities to handle, manipulate, and
 visualize data from condensed matter physics experiments, with a focus on
 angle-resolved photoemission spectroscopy (ARPES).
 
-.. grid:: 1 1 2 2
-    :gutter: 2
+*ERLabPy* is built on top of the popular scientific python libraries `numpy
+<https://numpy.org>`_, `scipy <https://scipy.org>`_, and `xarray
+<https://xarray.pydata.org>`_, and is designed to be easy to use and integrate with
+existing scientific Python workflows so that you can quickly get started with your data
+analysis. The package is still under development, so if you have any questions or
+suggestions, please feel free to contact us. We hope you find ERLabPy useful for your
+research!
+
+.. only:: format_html
+
+   .. grid:: 1 1 2 2
+       :gutter: 2
+
+       .. grid-item-card:: Getting started
+           :link: getting-started
+           :link-type: doc
+
+            The getting started guide provides installation instructions and an
+            overview on the dependencies.
+
+       .. grid-item-card::  User guide
+           :link: user-guide/index
+           :link-type: doc
+
+            The user guide provides some tutorials and examples on how to use
+            ERLabPy.
+
+       .. grid-item-card::  API reference
+           :link: reference
+           :link-type: doc
+
+            The reference guide provides detailed information of the API, including
+            descriptions of most available methods and parameters.
+
+       .. grid-item-card::  Contributing guide
+           :link: contributing
+           :link-type: doc
 
-    .. grid-item-card:: Getting started
-        :link: getting-started
-        :link-type: doc
-
-         The getting started guide provides installation instructions and an
-         overview on the dependencies.
-
-    .. grid-item-card::  User guide
-        :link: user-guide/index
-        :link-type: doc
-
-         The user guide provides some tutorials and examples on how to use
-         ERLabPy.
-
-    .. grid-item-card::  API reference
-        :link: reference
-        :link-type: doc
-
-         The reference guide provides detailed information of the API, including
-         descriptions of most available methods and parameters.
-
-    .. grid-item-card::  Contributing guide
-        :link: contributing
-        :link-type: doc
-
-         The contributing guide contains information on how to contribute to the
-         project.
+            The contributing guide contains information on how to contribute to the
+            project.
 
 
 .. image:: images/imagetool_light.png
     :align: center
     :alt: Imagetool
     :class: only-light
 
-.. image:: images/imagetool_dark.png
-    :align: center
-    :alt: Imagetool
-    :class: only-dark
+.. only:: format_html
+
+    .. image:: images/imagetool_dark.png
+        :align: center
+        :alt: Imagetool
+        :class: only-dark
 
 .. toctree::
    :maxdepth: 3
    :hidden:
    :caption: Contents
 
    getting-started
```

### Comparing `erlab-2.1.1/docs/source/pyplots/norms.py` & `erlab-2.1.2/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/reference.rst` & `erlab-2.1.2/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/refs.bib` & `erlab-2.1.2/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/user-guide/index.rst` & `erlab-2.1.2/docs/source/user-guide/index.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 **********
 User Guide
 **********
 
 .. admonition:: Work in Progress
    :class: warning
 
-   The user guide is incomplete. For the full list of packages and modules
-   provided by ERLabPy, see :doc:`../reference`.
-
-This section contains some examples for getting started with ARPES data analysis
-and visualization.
-
+   The user guide is incomplete. For the full list of packages and modules provided by
+   ERLabPy, see :doc:`../reference`.
 
 Introduction
 ============
 
-The following documentation assumes basic python programming experience.
+Welcome to the ERLabPy user guide! This guide provides an overview of ERLabPy and its
+core features.
 
-If you are new to scientific programming in python altogether, `Scientific
-Python Lectures <https://github.com/jrjohansson/scientific-python-lectures>`_ is
-a great resource to get started.
-
-Data in ERLabPy are mostly represented by :mod:`xarray` objects
-:cite:p:`hoyer2017xarray`. The `xarray user guide
-<https://docs.xarray.dev/en/stable/index.html>`_ and the `xarray tutorial
-<https://tutorial.xarray.dev/>`_ are great resources to get started with xarray.
+If you are new to programming with python, `Scientific Python Lectures
+<https://github.com/jrjohansson/scientific-python-lectures>`_ is a great place to start.
+
+Data structures in ERLabPy are represented using `xarray <https://docs.xarray.dev/>`_\
+:cite:p:`hoyer2017xarray`, which provides a powerful data structure for working with
+multi-dimensional arrays. Visit the `xarray tutorial <https://tutorial.xarray.dev/>`_
+and the `xarray user guide <https://docs.xarray.dev/en/stable/index.html>`_ to get
+familiar with xarray.
 
 .. toctree::
+   :caption: Table of Contents
+   :maxdepth: 2
+
    io
    indexing
    plotting
    kconv
 
 Further reading
 ===============
```

### Comparing `erlab-2.1.1/docs/source/user-guide/indexing.ipynb` & `erlab-2.1.2/docs/source/user-guide/indexing.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/docs/source/user-guide/kconv.ipynb` & `erlab-2.1.2/docs/source/user-guide/kconv.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993801652892562%*

 * *Differences: {"'cells'": "{18: {'metadata': {'vscode': OrderedDict([('languageId', 'raw')])}, 'source': "*

 * *            "{insert: [(12, '.. only:: format_html\\n'), (13, '\\n'), (14, '    .. image:: "*

 * *            "../images/ktool_1_dark.png\\n'), (15, '        :align: center\\n'), (16, '        "*

 * *            ":alt: KspaceTool 1\\n'), (17, '        :class: only-dark\\n'), (26, '.. only:: "*

 * *            "format_html\\n'), (27, '\\n'), (28, '    .. image:: ../images/ktool_2_dark.png\\n'), "*

 * *            "(29, '        :align:  […]*

```diff
@@ -4060,45 +4060,52 @@
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
-                "tags": []
+                "tags": [],
+                "vscode": {
+                    "languageId": "raw"
+                }
             },
             "source": [
                 "Interactive conversion\n",
                 "----------------------\n",
                 "\n",
                 "For three dimensional momentum conversion like maps or photon energy scans, an interactive window can be opened where you can adjust the parameters and see the effect right away.\n",
                 "\n",
                 "The GUI is divided into two tabs.\n",
                 "\n",
                 ".. image:: ../images/ktool_1_light.png\n",
                 "    :align: center\n",
                 "    :alt: KspaceTool 1\n",
                 "    :class: only-light\n",
                 "\n",
-                ".. image:: ../images/ktool_1_dark.png\n",
-                "    :align: center\n",
-                "    :alt: KspaceTool 1\n",
-                "    :class: only-dark\n",
+                ".. only:: format_html\n",
+                "\n",
+                "    .. image:: ../images/ktool_1_dark.png\n",
+                "        :align: center\n",
+                "        :alt: KspaceTool 1\n",
+                "        :class: only-dark\n",
                 "\n",
                 "The first tab is for setting momentum conversion parameters. The image is updated in real time as you change the parameters. Clicking the \"Copy code\" button will copy the code for conversion to the clipboard. The \"Open in ImageTool\" button performs a full three-dimensional conversion and opens the result in the ImageTool. \n",
                 "\n",
                 ".. image:: ../images/ktool_2_light.png\n",
                 "    :align: center\n",
                 "    :alt: KspaceTool 2\n",
                 "    :class: only-light\n",
                 "\n",
-                ".. image:: ../images/ktool_2_dark.png\n",
-                "    :align: center\n",
-                "    :alt: KspaceTool 2\n",
-                "    :class: only-dark\n",
+                ".. only:: format_html\n",
+                "\n",
+                "    .. image:: ../images/ktool_2_dark.png\n",
+                "        :align: center\n",
+                "        :alt: KspaceTool 2\n",
+                "        :class: only-dark\n",
                 "\n",
                 "The second tab provides visualization options. You can overlay Brillouin zones and high symmetry points on the result, adjust colors, and apply binning.\n",
                 "\n",
                 "There are two ways to invoke the GUI. The first one is to call the ``interactive`` method on the accessor: "
             ]
         },
         {
```

### Comparing `erlab-2.1.1/docs/source/user-guide/plotting.ipynb` & `erlab-2.1.2/docs/source/user-guide/plotting.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9932109557109556%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(0, 'cut = dat.qsel(ky=0.3)\\n')], delete: [0]}}, 19: "*

 * *            "{'source': {insert: [(5, '    const_energy_surface = dat.qsel(eV=energy)\\n')], "*

 * *            "delete: [5]}}, 33: {'source': {insert: [(4, '| khan       | Personal preferences of "*

 * *            "the package author.                                                         |\\n')], "*

 * *            "delete: [4]}}, insert: [(22, OrderedDict([('cell_type', 'markdown'), ('metadata', "*

 * *            "OrderedDict()) […]*

```diff
@@ -118,15 +118,15 @@
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "cut = dat.sel(ky=0.3, method=\"nearest\")\n",
+                "cut = dat.qsel(ky=0.3)\n",
                 "cut"
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
@@ -306,15 +306,15 @@
             "outputs": [],
             "source": [
                 "energies = [-0.4, -0.2, 0.0]\n",
                 "\n",
                 "fig, axs = plt.subplots(1, 3, layout=\"compressed\", sharey=True)\n",
                 "\n",
                 "for energy, ax in zip(energies, axs):\n",
-                "    const_energy_surface = dat.sel(eV=energy, method=\"nearest\")\n",
+                "    const_energy_surface = dat.qsel(eV=energy)\n",
                 "    eplt.plot_array(const_energy_surface, ax=ax, gamma=0.5, aspect=\"equal\")\n",
                 "\n",
                 "eplt.clean_labels(axs)  # removes shared y labels\n",
                 "eplt.label_subplot_properties(axs, values=dict(Eb=energies))  # annotates energy"
             ]
         },
         {
@@ -351,14 +351,32 @@
                 "fig, axs = eplt.plot_slices([dat], eV=[-0.4, -0.2, 0.0], gamma=0.5, axis=\"image\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "We can also plot the data integrated over an energy window, in this case with a width of 200 meV by adding the `eV_width` argument:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "fig, axs = eplt.plot_slices(\n",
+                "    [dat], eV=[-0.4, -0.2, 0.0], eV_width=0.2, gamma=0.5, axis=\"image\"\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "Cuts along constant $k_y$ can be plotted analogously."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -468,15 +486,15 @@
                 "tags": []
             },
             "source": [
                 "You can control the look and feel of matplotlib figures with [*style sheets* and *rcParams*](https://matplotlib.org/stable/users/explain/customizing.html). In addition to the [options provided by matplotlib](https://matplotlib.org/stable/gallery/style_sheets/style_sheets_reference.html), ERLabPy provides some style sheets that are listed below. Note that style sheets that change the default font requires the font to be installed on the system. To see how each one looks, try running [the code provided by matplotlib](https://matplotlib.org/stable/gallery/style_sheets/style_sheets_reference.html).\n",
                 "\n",
                 "| Style Name | Description                                                                                         |\n",
                 "|------------|-----------------------------------------------------------------------------------------------------|\n",
-                "| khan       | Personal preferences.                                                                               |\n",
+                "| khan       | Personal preferences of the package author.                                                         |\n",
                 "| fira       | Changes the default font to Fira Sans.                                                              |\n",
                 "| firalight  | Changes the default font to Fira Sans Light.                                                        |\n",
                 "| times      | Changes the default font to Times New Roman.                                                        |\n",
                 "| nature     | Changes the default font to Arial, and tweaks some aspects such as padding and default figure size. |\n"
             ]
         },
         {
```

### Comparing `erlab-2.1.1/environment.yml` & `erlab-2.1.2/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/environment_apple.yml` & `erlab-2.1.2/environment_apple.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/environment_nogit.yml` & `erlab-2.1.2/environment_nogit.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/environment_nogit_mkl.yml` & `erlab-2.1.2/environment_nogit_mkl.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/pyproject.toml` & `erlab-2.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/accessors.py` & `erlab-2.1.2/src/erlab/accessors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/__init__.py` & `erlab-2.1.2/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/correlation.py` & `erlab-2.1.2/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.1.2/src/erlab/analysis/fit/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.1.2/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/fit/functions/general.py` & `erlab-2.1.2/src/erlab/analysis/fit/functions/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/fit/minuit.py` & `erlab-2.1.2/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/fit/models.py` & `erlab-2.1.2/src/erlab/analysis/fit/models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/fit/spline.py` & `erlab-2.1.2/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/gold.py` & `erlab-2.1.2/src/erlab/analysis/gold.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/image.py` & `erlab-2.1.2/src/erlab/analysis/image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/interpolate.py` & `erlab-2.1.2/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/kspace.py` & `erlab-2.1.2/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/mask/__init__.py` & `erlab-2.1.2/src/erlab/analysis/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/mask/polygon.py` & `erlab-2.1.2/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/transform.py` & `erlab-2.1.2/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/analysis/utilities.py` & `erlab-2.1.2/src/erlab/analysis/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/characterization/resistance.py` & `erlab-2.1.2/src/erlab/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/characterization/xrd.py` & `erlab-2.1.2/src/erlab/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/constants.py` & `erlab-2.1.2/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/__init__.py` & `erlab-2.1.2/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/bzplot.py` & `erlab-2.1.2/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/colors.py` & `erlab-2.1.2/src/erlab/interactive/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/curvefittingtool.py` & `erlab-2.1.2/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/derivative.py` & `erlab-2.1.2/src/erlab/interactive/derivative.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/dtool.ui` & `erlab-2.1.2/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/exampledata.py` & `erlab-2.1.2/src/erlab/interactive/exampledata.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/fermiedge.py` & `erlab-2.1.2/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.1.2/src/erlab/interactive/imagetool/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.1.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.1.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/imagetool/controls.py` & `erlab-2.1.2/src/erlab/interactive/imagetool/controls.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/imagetool/core.py` & `erlab-2.1.2/src/erlab/interactive/imagetool/core.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.1.2/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.1.2/src/erlab/interactive/imagetool/slicer.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/kspace.py` & `erlab-2.1.2/src/erlab/interactive/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/ktool.ui` & `erlab-2.1.2/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/masktool.py` & `erlab-2.1.2/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/interactive/utilities.py` & `erlab-2.1.2/src/erlab/interactive/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/io/__init__.py` & `erlab-2.1.2/src/erlab/io/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/io/dataloader.py` & `erlab-2.1.2/src/erlab/io/dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,15 +325,16 @@
             used.
         single
             For some setups, data for a single scan is saved over multiple files. This
             argument is only used for such setups. When `identifier` is resolved to a
             single file within a multiple file scan, the default behavior when `single`
             is `False` is to return a single concatenated array that contains data from
             all files in the same scan. If `single` is set to `True`, only the data from
-            the file given is returned.
+            the file given is returned. This argument is ignored when `identifier` is a
+            number.
         **kwargs
             Additional keyword arguments are passed to `identify`.
 
         Returns
         -------
         xarray.DataArray or xarray.Dataset or list of xarray.DataArray
             The loaded data.
@@ -419,24 +420,26 @@
 
         Returns
         -------
         pandas.DataFrame
             Summary of the data in the directory.
 
         """
+        if not os.path.isdir(data_dir):
+            raise FileNotFoundError(f"Directory {data_dir} not found")
+
         pkl_path = os.path.join(data_dir, ".summary.pkl")
         df = None
         if usecache:
             try:
                 df = pandas.read_pickle(pkl_path)
+                df = df.head(len(df))
             except FileNotFoundError:
                 pass
 
-        df = df.head(len(df))
-
         if df is None:
             df = self.generate_summary(data_dir, **kwargs)
             df.to_pickle(pkl_path)
 
         try:
             shell = get_ipython().__class__.__name__  # type: ignore
             if shell in ["ZMQInteractiveShell", "TerminalInteractiveShell"]:
@@ -843,14 +846,16 @@
 
         Note
         ----
         This will only affect `load`. If the loader's ``load`` method is called
         directly, it will not use the default data directory.
 
         """
+        if not os.path.isdir(data_dir):
+            raise FileNotFoundError(f"Directory {data_dir} not found")
         self.default_data_dir = data_dir
 
     def load(
         self,
         identifier: str | os.PathLike | int | None,
         data_dir: str | os.PathLike | None = None,
         **kwargs: dict,
```

### Comparing `erlab-2.1.1/src/erlab/io/igor.py` & `erlab-2.1.2/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/io/plugins/__init__.py` & `erlab-2.1.2/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/io/plugins/da30.py` & `erlab-2.1.2/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/io/plugins/kriss.py` & `erlab-2.1.2/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/io/plugins/merlin.py` & `erlab-2.1.2/src/erlab/io/plugins/merlin.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,17 @@
                 data = self.load_live(path)
                 if "beta" in data.dims:
                     data_type = "LP"
                 else:
                     data_type = "LXY"
             else:
                 data = self.load(path)
+                data_type = "core"
+                if "alpha" in data.dims:
+                    data_type = "cut"
                 if "beta" in data.dims:
                     data_type = "map"
                 if "hv" in data.dims:
                     data_type = "hvdep"
 
             data_info.append(
                 [
```

### Comparing `erlab-2.1.1/src/erlab/io/plugins/ssrl52.py` & `erlab-2.1.2/src/erlab/io/plugins/ssrl52.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/io/utilities.py` & `erlab-2.1.2/src/erlab/io/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/lattice.py` & `erlab-2.1.2/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/parallel.py` & `erlab-2.1.2/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.1.2/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.1.2/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.1.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.1.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.1.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.1.2/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.1.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.1.2/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.1.2/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.1.2/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/__init__.py` & `erlab-2.1.2/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/annotations.py` & `erlab-2.1.2/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/atoms.py` & `erlab-2.1.2/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/bz.py` & `erlab-2.1.2/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/colors.py` & `erlab-2.1.2/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/erplot.py` & `erlab-2.1.2/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/general.py` & `erlab-2.1.2/src/erlab/plotting/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/plot3d.py` & `erlab-2.1.2/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.1.2/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.1.2/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.1.2/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.1.2/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.1.2/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.1.2/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab.egg-info/PKG-INFO` & `erlab-2.1.2/src/erlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -742,49 +742,50 @@
 [![Workflow Status](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml/badge.svg)](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml)
 [![Documentation Status](https://readthedocs.org/projects/erlabpy/badge/)](https://erlabpy.readthedocs.io/)
 [![License](https://img.shields.io/pypi/l/erlab)](https://github.com/kmnhan/erlabpy/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/kmnhan/erlabpy/main.svg)](https://results.pre-commit.ci/latest/github/kmnhan/erlabpy/main)
 
 A library that provides a set of tools and utilities to handle, manipulate, and
-visualize data from condensed matter physics experiments, with a focus on
-angle-resolved photoemission spectroscopy (ARPES).
+visualize data from condensed matter physics experiments, with a focus on angle-resolved
+photoemission spectroscopy (ARPES).
 
 *ERLabPy* is built on top of the popular scientific computing libraries
 [*numpy*](https://numpy.org/), [*scipy*](https://scipy.org/), and
-[*xarray*](https://xarray.pydata.org/), and is designed to be easy to use and
-integrate with existing scientific Python workflows. It is also designed to be
-extensible, allowing users to easily add custom functionality and analysis
-tools.
+[*xarray*](https://xarray.pydata.org/), and is designed to be easy to use and integrate
+with existing scientific Python workflows so that you can quickly get started with your
+data analysis. The package is still under development, so if you have any questions or
+suggestions, please feel free to contact us. We hope you find ERLabPy useful for your
+research!
 
 *ERLabPy* is developed and maintained by the electronic structure research
 laboratory at Korea Advanced Institute of Science and Technology (KAIST).
 
 ## Features
 
-- **Data Loading**: A flexible and extensible data loading system is included,
-  capable of handling various data formats.
+- **Data Loading**: A flexible and extensible data loading system is included, capable
+  of handling various data formats.
 - **Data Manipulation**: A set of tools for manipulating and transforming data,
   including interpolation, masking and symmetrization is provided.
-- **Plotting**: ERLabPy provides many different plotting functions for
-  visualizing image data, including 2D and 3D plots. Publication-quality plots
-  can be generated with minimal effort.
-- **Fitting**: Several functions and models are implemented for fitting various
-  types of data, including broadened Fermi-Dirac distributions, momentum
-  distribution curves (MDCs), and energy distribution curves (EDCs).
+- **Plotting**: ERLabPy provides many different plotting functions for visualizing image
+  data, including 2D and 3D plots. Publication-quality plots can be generated with
+  minimal effort.
+- **Fitting**: Several functions and models are implemented for fitting various types of
+  data, including broadened Fermi-Dirac distributions, momentum distribution curves
+  (MDCs), and energy distribution curves (EDCs).
 - **Interactive Data Visualization**: ERLabPy includes many interactive plotting
-  routines that resemble panels in Igor Pro that are very responsive and easy to
-  use. See screenshots below.
+  routines that resemble panels in Igor Pro that are very responsive and easy to use.
+  See screenshots below.
 - **Active Development**: ERLabPy is actively developed and maintained, with new
   features and improvements being added regularly.
 
 ## Screenshots
 
-Most interactive windows support dark mode. Viewing this page from a supported
-browser with dark mode enabled will show the dark mode screenshots.
+Most interactive windows support dark mode. Viewing this page from a supported browser
+with dark mode enabled will show the dark mode screenshots.
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/imagetool_dark.png?raw=true">
   <source media="(prefers-color-scheme: light)" srcset="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/imagetool_light.png?raw=true">
   <img alt="Imagetool in action." src="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/imagetool_light.png?raw=true">
 </picture>
 
@@ -801,18 +802,18 @@
 
 ## Documentation
 
 The full documentation for ERLabPy is available on [Read the Docs](https://erlabpy.readthedocs.io/).
 
 ## Contributing
 
-ERLabPy is an open-source project and we welcome contributions from the
-community. If you find any bugs, issues, or have any suggestions, please open an
-issue [here](https://github.com/kmnhan/erlabpy/issues). If you would like to add
-a new feature or fix a bug yourself, we would love to have your contribution.
-Feel free to fork the repository and submit a pull request with your changes.
+ERLabPy is an open-source project and we welcome contributions from the community. If
+you find any bugs, issues, or have any suggestions, please open an issue
+[here](https://github.com/kmnhan/erlabpy/issues). If you would like to add a new feature
+or fix a bug yourself, we would love to have your contribution. Feel free to fork the
+repository and submit a pull request with your changes.
 
 For more information on contributing, see our [Contributing page](https://erlabpy.readthedocs.io/en/stable/contributing.html).
 
 ## License
 
 This project is licensed under the terms of the [GPL-3.0 License](LICENSE).
```

### Comparing `erlab-2.1.1/src/erlab.egg-info/SOURCES.txt` & `erlab-2.1.2/src/erlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/src/erlab.egg-info/requires.txt` & `erlab-2.1.2/src/erlab.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/templates/.macros.j2` & `erlab-2.1.2/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/tests/analysis/test_fastbinning.py` & `erlab-2.1.2/tests/analysis/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/tests/analysis/test_fit_functions_dynamic.py` & `erlab-2.1.2/tests/analysis/test_fit_functions_dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/tests/analysis/test_fit_functions_general.py` & `erlab-2.1.2/tests/analysis/test_fit_functions_general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/tests/analysis/test_image.py` & `erlab-2.1.2/tests/analysis/test_image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/tests/analysis/test_interpolate.py` & `erlab-2.1.2/tests/analysis/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/tests/analysis/test_kspace.py` & `erlab-2.1.2/tests/analysis/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.1/tests/analysis/test_utilities.py` & `erlab-2.1.2/tests/analysis/test_utilities.py`

 * *Files identical despite different names*

