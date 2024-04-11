# Comparing `tmp/erlab-2.1.2.tar.gz` & `tmp/erlab-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.1.2.tar", last modified: Thu Apr 11 01:29:22 2024, max compression
+gzip compressed data, was "erlab-2.1.3.tar", last modified: Thu Apr 11 03:07:02 2024, max compression
```

## Comparing `erlab-2.1.2.tar` & `erlab-2.1.3.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.202324 erlab-2.1.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.158324 erlab-2.1.2/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.162324 erlab-2.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-11 01:29:15.000000 erlab-2.1.2/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 root         (0) root         (0)      608 2024-04-11 01:29:15.000000 erlab-2.1.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.162324 erlab-2.1.2/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-11 01:29:15.000000 erlab-2.1.2/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-11 01:29:15.000000 erlab-2.1.2/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-11 01:29:15.000000 erlab-2.1.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-11 01:29:15.000000 erlab-2.1.2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      796 2024-04-11 01:29:15.000000 erlab-2.1.2/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   104651 2024-04-11 01:29:18.000000 erlab-2.1.2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-04-11 01:29:15.000000 erlab-2.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    47782 2024-04-11 01:29:22.202324 erlab-2.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-11 01:29:15.000000 erlab-2.1.2/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     4823 2024-04-11 01:29:15.000000 erlab-2.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.166324 erlab-2.1.2/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      655 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.170324 erlab-2.1.2/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    16011 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    14522 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      265 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.characterization.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     3806 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.174324 erlab-2.1.2/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   321080 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/flowchart_multiple.pdf
--rw-r--r--   0 root         (0) root         (0)   317804 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/flowchart_single.pdf
--rw-r--r--   0 root         (0) root         (0)   996803 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     3285 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.178324 erlab-2.1.2/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2578 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1344 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     2342 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.178324 erlab-2.1.2/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)     1261 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)     5063 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)    50371 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)   379705 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    16193 2024-04-11 01:29:15.000000 erlab-2.1.2/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-11 01:29:15.000000 erlab-2.1.2/environment.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-11 01:29:15.000000 erlab-2.1.2/environment_apple.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-11 01:29:15.000000 erlab-2.1.2/environment_nogit.yml
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-11 01:29:15.000000 erlab-2.1.2/environment_nogit_mkl.yml
--rw-r--r--   0 root         (0) root         (0)     4373 2024-04-11 01:29:15.000000 erlab-2.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-11 01:29:15.000000 erlab-2.1.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 01:29:22.202324 erlab-2.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.158324 erlab-2.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.178324 erlab-2.1.2/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-11 01:29:18.000000 erlab-2.1.2/src/erlab/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35543 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/accessors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.182324 erlab-2.1.2/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5514 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.182324 erlab-2.1.2/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      459 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.182324 erlab-2.1.2/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      839 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9632 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     6026 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)     9881 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1168 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    15448 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    17325 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10629 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.186324 erlab-2.1.2/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     5401 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8440 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     8658 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.186324 erlab-2.1.2/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      191 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.186324 erlab-2.1.2/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      540 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13953 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    20867 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    22451 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11443 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)     9458 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/exampledata.py
--rw-r--r--   0 root         (0) root         (0)    19072 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.190324 erlab-2.1.2/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    19396 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.190324 erlab-2.1.2/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51945 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114560 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27081 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    54122 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    13907 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25270 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    15835 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19382 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     3341 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    54143 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.190324 erlab-2.1.2/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     1937 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32013 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6905 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.190324 erlab-2.1.2/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3667 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     7594 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7804 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     6559 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.194324 erlab-2.1.2/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.194324 erlab-2.1.2/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     2026 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29010 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18284 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    32437 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    31070 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.198324 erlab-2.1.2/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-04-11 01:29:15.000000 erlab-2.1.2/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.198324 erlab-2.1.2/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    47782 2024-04-11 01:29:22.000000 erlab-2.1.2/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4675 2024-04-11 01:29:22.000000 erlab-2.1.2/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 01:29:22.000000 erlab-2.1.2/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      536 2024-04-11 01:29:22.000000 erlab-2.1.2/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-11 01:29:22.000000 erlab-2.1.2/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.198324 erlab-2.1.2/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-11 01:29:15.000000 erlab-2.1.2/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-04-11 01:29:15.000000 erlab-2.1.2/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-04-11 01:29:15.000000 erlab-2.1.2/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.162324 erlab-2.1.2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:29:22.198324 erlab-2.1.2/tests/analysis/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_fit_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_fit_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     5228 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_image.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     2423 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-11 01:29:15.000000 erlab-2.1.2/tests/analysis/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.820390 erlab-2.1.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.776389 erlab-2.1.3/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.784390 erlab-2.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-11 03:06:56.000000 erlab-2.1.3/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-11 03:06:56.000000 erlab-2.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.784390 erlab-2.1.3/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-11 03:06:56.000000 erlab-2.1.3/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-11 03:06:56.000000 erlab-2.1.3/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-11 03:06:56.000000 erlab-2.1.3/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-11 03:06:56.000000 erlab-2.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      796 2024-04-11 03:06:56.000000 erlab-2.1.3/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   104848 2024-04-11 03:06:59.000000 erlab-2.1.3/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-04-11 03:06:56.000000 erlab-2.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    47782 2024-04-11 03:07:02.820390 erlab-2.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-11 03:06:56.000000 erlab-2.1.3/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     4823 2024-04-11 03:06:56.000000 erlab-2.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.784390 erlab-2.1.3/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      655 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.788390 erlab-2.1.3/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    16011 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    14522 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.characterization.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     3806 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.792389 erlab-2.1.3/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   321080 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   317804 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     3285 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.796390 erlab-2.1.3/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2578 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.796390 erlab-2.1.3/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)     5063 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    50053 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)   379705 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    16193 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-11 03:06:56.000000 erlab-2.1.3/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-11 03:06:56.000000 erlab-2.1.3/environment_apple.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-11 03:06:56.000000 erlab-2.1.3/environment_nogit.yml
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-11 03:06:56.000000 erlab-2.1.3/environment_nogit_mkl.yml
+-rw-r--r--   0 root         (0) root         (0)     4373 2024-04-11 03:06:56.000000 erlab-2.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-11 03:06:56.000000 erlab-2.1.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 03:07:02.820390 erlab-2.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.776389 erlab-2.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.796390 erlab-2.1.3/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-11 03:06:59.000000 erlab-2.1.3/src/erlab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35543 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/accessors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.800390 erlab-2.1.3/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.800390 erlab-2.1.3/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      459 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.804390 erlab-2.1.3/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      839 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9632 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     6026 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)     9881 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    15448 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    17325 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10629 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.804390 erlab-2.1.3/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     5401 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8440 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     8658 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.804390 erlab-2.1.3/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.804390 erlab-2.1.3/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13953 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    20867 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    22451 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11443 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)     9458 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)    19072 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.808390 erlab-2.1.3/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    19705 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.808390 erlab-2.1.3/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51945 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114560 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27081 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    54122 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    13907 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25270 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    15835 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     3341 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    54143 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.808390 erlab-2.1.3/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31737 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.808390 erlab-2.1.3/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3672 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     7594 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7804 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     6777 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.812390 erlab-2.1.3/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.812390 erlab-2.1.3/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29010 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18284 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    32437 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    31070 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.816390 erlab-2.1.3/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.816390 erlab-2.1.3/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    47782 2024-04-11 03:07:02.000000 erlab-2.1.3/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4675 2024-04-11 03:07:02.000000 erlab-2.1.3/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 03:07:02.000000 erlab-2.1.3/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      536 2024-04-11 03:07:02.000000 erlab-2.1.3/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-11 03:07:02.000000 erlab-2.1.3/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.816390 erlab-2.1.3/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-11 03:06:56.000000 erlab-2.1.3/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-11 03:06:56.000000 erlab-2.1.3/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-11 03:06:56.000000 erlab-2.1.3/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.780390 erlab-2.1.3/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.816390 erlab-2.1.3/tests/analysis/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_fit_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_fit_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_utilities.py
```

### Comparing `erlab-2.1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `erlab-2.1.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/.github/workflows/pr.yml` & `erlab-2.1.3/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/.github/workflows/release.yml` & `erlab-2.1.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/.gitignore` & `erlab-2.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/.pre-commit-config.yaml` & `erlab-2.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/.readthedocs.yaml` & `erlab-2.1.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/CHANGELOG.md` & `erlab-2.1.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v2.1.3 (2024-04-11)
+
+### Fix
+
+* (**interactive**) update data load functions used in imagetool ([`c3abe35`](https://github.com/kmnhan/erlabpy/commit/c3abe3517046ed603a9221de38b22257322d3a51))
+
+
 ## v2.1.2 (2024-04-11)
 
 ### Documentation
 
 * update syntax ([`2b72991`](https://github.com/kmnhan/erlabpy/commit/2b7299150a50af38e6e05d5f9690558cbeb7a9ad))
 
 * improve intro pages ([`ec2a4f8`](https://github.com/kmnhan/erlabpy/commit/ec2a4f816e1ad0ed1ad154d6544e91bea1b5d9c5))
```

### Comparing `erlab-2.1.2/LICENSE` & `erlab-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/PKG-INFO` & `erlab-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.1.2/PythonInterface.ipf` & `erlab-2.1.3/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/README.md` & `erlab-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/Makefile` & `erlab-2.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/environment.yml` & `erlab-2.1.3/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/make.bat` & `erlab-2.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/conf.py` & `erlab-2.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/contributing.rst` & `erlab-2.1.3/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/getting-started.rst` & `erlab-2.1.3/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/images/flowchart_multiple.pdf` & `erlab-2.1.3/docs/source/images/flowchart_multiple.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/images/flowchart_single.pdf` & `erlab-2.1.3/docs/source/images/flowchart_single.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/images/imagetool_dark.png` & `erlab-2.1.3/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/images/imagetool_light.png` & `erlab-2.1.3/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/images/ktool_1_dark.png` & `erlab-2.1.3/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/images/ktool_1_light.png` & `erlab-2.1.3/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/images/ktool_2_dark.png` & `erlab-2.1.3/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/images/ktool_2_light.png` & `erlab-2.1.3/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/index.rst` & `erlab-2.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/pyplots/norms.py` & `erlab-2.1.3/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/reference.rst` & `erlab-2.1.3/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/refs.bib` & `erlab-2.1.3/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/user-guide/index.rst` & `erlab-2.1.3/docs/source/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/user-guide/indexing.ipynb` & `erlab-2.1.3/docs/source/user-guide/indexing.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/user-guide/io.ipynb` & `erlab-2.1.3/docs/source/user-guide/io.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998885918003565%*

 * *Differences: {"'cells'": "{12: {'source': {insert: [(9, 'as a loader. This is useful for base classes that are "*

 * *            "not meant to be used directly.\\n')], delete: [12, 11, 10, 9]}}}"}*

```diff
@@ -650,18 +650,15 @@
                 "\n",
                 "It is easy to add new loaders to the framework. Any class that subclasses\n",
                 ":class:`LoaderBase <erlab.io.dataloader.LoaderBase>` is automatically registered as a\n",
                 "loader upon its definition. The class must have a valid ``name`` attribute, which is\n",
                 "used to access the loader.\n",
                 "\n",
                 "If the ``name`` attribute is prefixed with an underscore, the loader is not registered\n",
-                "as a loader. This is useful for base classes that are not meant to be used directly. One\n",
-                "example is :class:`DA30Loader <erlab.io.plugins.da30.DA30Loader>`, which only implements\n",
-                "the ``load_single`` method and serves as a base class for implementing loaders for\n",
-                "setups using the Scienta Omicron DA30 hemispherical analyzer with ``SES.exe``.\n",
+                "as a loader. This is useful for base classes that are not meant to be used directly.\n",
                 "\n",
                 "ARPES data from a single experiment are usually stored in one folder, with files that\n",
                 "look like ``file_0001.h5``, ``file_0002.h5``, etc. If the naming scheme does not deviate\n",
                 "from this pattern, only two methods need to be implemented: :meth:`identify\n",
                 "<erlab.io.dataloader.LoaderBase.identify>` and :meth:`load_single\n",
                 "<erlab.io.dataloader.LoaderBase.load_single>`. The following flowchart shows the process\n",
                 "of loading data from a single scan, given either a file path or a sequence number:\n",
```

### Comparing `erlab-2.1.2/docs/source/user-guide/kconv.ipynb` & `erlab-2.1.3/docs/source/user-guide/kconv.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/docs/source/user-guide/plotting.ipynb` & `erlab-2.1.3/docs/source/user-guide/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/environment.yml` & `erlab-2.1.3/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/environment_apple.yml` & `erlab-2.1.3/environment_apple.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/environment_nogit.yml` & `erlab-2.1.3/environment_nogit.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/environment_nogit_mkl.yml` & `erlab-2.1.3/environment_nogit_mkl.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/pyproject.toml` & `erlab-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/accessors.py` & `erlab-2.1.3/src/erlab/accessors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/__init__.py` & `erlab-2.1.3/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/correlation.py` & `erlab-2.1.3/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.1.3/src/erlab/analysis/fit/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.1.3/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/fit/functions/general.py` & `erlab-2.1.3/src/erlab/analysis/fit/functions/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/fit/minuit.py` & `erlab-2.1.3/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/fit/models.py` & `erlab-2.1.3/src/erlab/analysis/fit/models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/fit/spline.py` & `erlab-2.1.3/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/gold.py` & `erlab-2.1.3/src/erlab/analysis/gold.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/image.py` & `erlab-2.1.3/src/erlab/analysis/image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/interpolate.py` & `erlab-2.1.3/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/kspace.py` & `erlab-2.1.3/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/mask/__init__.py` & `erlab-2.1.3/src/erlab/analysis/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/mask/polygon.py` & `erlab-2.1.3/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/transform.py` & `erlab-2.1.3/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/analysis/utilities.py` & `erlab-2.1.3/src/erlab/analysis/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/characterization/resistance.py` & `erlab-2.1.3/src/erlab/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/characterization/xrd.py` & `erlab-2.1.3/src/erlab/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/constants.py` & `erlab-2.1.3/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/__init__.py` & `erlab-2.1.3/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/bzplot.py` & `erlab-2.1.3/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/colors.py` & `erlab-2.1.3/src/erlab/interactive/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/curvefittingtool.py` & `erlab-2.1.3/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/derivative.py` & `erlab-2.1.3/src/erlab/interactive/derivative.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/dtool.ui` & `erlab-2.1.3/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/exampledata.py` & `erlab-2.1.3/src/erlab/interactive/exampledata.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/fermiedge.py` & `erlab-2.1.3/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.1.3/src/erlab/interactive/imagetool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     ItoolColormapControls,
     ItoolCrosshairControls,
 )
 from erlab.interactive.imagetool.core import ImageSlicerArea, SlicerLinkProxy
 from erlab.interactive.utilities import DictMenuBar, copy_to_clipboard
 
 if TYPE_CHECKING:
-    from collections.abc import Sequence
+    from collections.abc import Callable, Sequence
 
     import numpy as np
     import numpy.typing as npt
 
     from erlab.interactive.imagetool.slicer import ArraySlicer
 
 
@@ -417,50 +417,54 @@
     def _copy_cursor_val(self):
         copy_to_clipboard(str(self.slicer_area.array_slicer._values))
 
     def _copy_cursor_idx(self):
         copy_to_clipboard(str(self.slicer_area.array_slicer._indices))
 
     def _open_file(self):
-        valid_files = {
-            "xarray HDF5 Files (*.h5)": (xr.load_dataarray, {"engine": "h5netcdf"}),
-            "ALS BL4.0.3 Raw Data (*.pxt)": (erlab.io.merlin.load, {}),
-            "ALS BL4.0.3 Live (*.ibw)": (erlab.io.merlin.load_live, {}),
-            "DA30 Raw Data (*.ibw *.pxt *.zip)": (erlab.io.da30.load, {}),
-            "SSRL BL5-2 Raw Data (*.h5)": (erlab.io.ssrl52.load, {}),
+        valid_loaders: dict[str, tuple[Callable, dict]] = {
+            "xarray HDF5 Files (*.h5)": (erlab.io.load_hdf5, {}),
+            "ALS BL4.0.3 Raw Data (*.pxt)": (erlab.io.loaders["merlin"].load, {}),
+            "ALS BL4.0.3 Live (*.ibw)": (erlab.io.loaders["merlin"].load_live, {}),
+            "DA30 Raw Data (*.ibw *.pxt *.zip)": (erlab.io.loaders["da30"].load, {}),
+            "SSRL BL5-2 Raw Data (*.h5)": (erlab.io.loaders["ssrl52"].load, {}),
             "NetCDF Files (*.nc *.nc4 *.cdf)": (xr.load_dataarray, {}),
         }
 
         dialog = QtWidgets.QFileDialog(self)
         dialog.setAcceptMode(QtWidgets.QFileDialog.AcceptMode.AcceptOpen)
         dialog.setFileMode(QtWidgets.QFileDialog.FileMode.ExistingFile)
-        dialog.setNameFilters(valid_files.keys())
+        dialog.setNameFilters(valid_loaders.keys())
         # dialog.setOption(QtWidgets.QFileDialog.Option.DontUseNativeDialog)
 
         if dialog.exec():
             files = dialog.selectedFiles()
-            fn, kargs = valid_files[dialog.selectedNameFilter()]
+            fn, kargs = valid_loaders[dialog.selectedNameFilter()]
             # !TODO: handle ambiguous datasets
             self.slicer_area.set_data(fn(files[0], **kargs))
             self.slicer_area.view_all()
 
     def _export_file(self):
         if self.slicer_area._data is None:
             raise ValueError("Data is Empty!")
         dialog = QtWidgets.QFileDialog(self)
         dialog.setAcceptMode(QtWidgets.QFileDialog.AcceptMode.AcceptSave)
         dialog.setFileMode(QtWidgets.QFileDialog.FileMode.AnyFile)
-        dialog.setNameFilter(
-            "xarray HDF5 Files (*.h5)",
-        )
+
+        valid_savers: dict[str, tuple[Callable, dict]] = {
+            "xarray HDF5 Files (*.h5)": (erlab.io.save_as_hdf5, {}),
+            "NetCDF Files (*.nc *.nc4 *.cdf)": (erlab.io.save_as_netcdf, {}),
+        }
+        dialog.setNameFilters(valid_savers.keys())
         dialog.setDirectory(f"{self.slicer_area._data.name}.h5")
         # dialog.setOption(QtWidgets.QFileDialog.Option.DontUseNativeDialog)
         if dialog.exec():
             files = dialog.selectedFiles()
-            erlab.io.save_as_hdf5(self.slicer_area._data, files[0])
+            fn, kargs = valid_savers[dialog.selectedNameFilter()]
+            fn(self.slicer_area._data, files[0], **kargs)
 
 
 if __name__ == "__main__":
     # import gc
     # import linecache
     # import tracemalloc
 
@@ -501,17 +505,17 @@
     #     for line in stat.traceback.format():
     #         print(line)
 
     # tracemalloc.start()
     data = xr.load_dataarray(
         #     # "~/Documents/ERLab/TiSe2/kxy10.nc",
         #     # "~/Documents/ERLab/TiSe2/221213_SSRL_BL5-2/fullmap_kconv_.h5",
-        #     # "~/Documents/ERLab/CsV3Sb5/2021_Dec_ALS_CV3Sb5/Data/cvs_kxy_small.nc",
-        #     "~/Documents/ERLab/CsV3Sb5/2021_Dec_ALS_CV3Sb5/Data/cvs_kxy.nc",
-        "~/Documents/ERLab/TiSe2/220410_ALS_BL4/map_mm_4d_.nc",
+        "~/Documents/ERLab/CsV3Sb5/2021_Dec_ALS_CV3Sb5/Data/cvs_kxy_small.nc",
+        # "~/Documents/ERLab/CsV3Sb5/2021_Dec_ALS_CV3Sb5/Data/cvs_kxy.nc",
+        # "~/Documents/ERLab/TiSe2/220410_ALS_BL4/map_mm_4d_.nc",
         # engine="h5netcdf",
     )
 
     # win = itool(data, bench=True)
     # win = itool(data)
     # del data
```

### Comparing `erlab-2.1.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.1.3/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.1.3/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/imagetool/controls.py` & `erlab-2.1.3/src/erlab/interactive/imagetool/controls.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/imagetool/core.py` & `erlab-2.1.3/src/erlab/interactive/imagetool/core.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.1.3/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.1.3/src/erlab/interactive/imagetool/slicer.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/kspace.py` & `erlab-2.1.3/src/erlab/interactive/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/ktool.ui` & `erlab-2.1.3/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/masktool.py` & `erlab-2.1.3/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/interactive/utilities.py` & `erlab-2.1.3/src/erlab/interactive/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/io/__init__.py` & `erlab-2.1.3/src/erlab/io/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,29 +54,35 @@
     "set_data_dir",
     "set_loader",
     "summarize",
 ]
 
 import warnings
 
-from erlab.io.dataloader import (
-    load,
-    loader_context,
-    loaders,
-    set_data_dir,
-    set_loader,
-    summarize,
-)
+from erlab.io.dataloader import LoaderRegistry
 from erlab.io.igor import load_experiment, load_wave
 from erlab.io.utilities import load_hdf5, open_hdf5, save_as_hdf5, save_as_netcdf
 
 # Import plugins last
 # isort: off
 import erlab.io.plugins  # noqa: F401
 
+loaders = LoaderRegistry.instance()
+"""
+Global instance of :class:`LoaderRegistry <erlab.io.dataloader.LoaderRegistry>`.
+
+:meta hide-value:
+"""
+
+load = loaders.load
+loader_context = loaders.loader_context
+set_data_dir = loaders.set_data_dir
+set_loader = loaders.set_loader
+summarize = loaders.summarize
+
 merlin = loaders["merlin"]
 ssrl52 = loaders["ssrl52"]
 
 
 def load_igor_ibw(*args, **kwargs):
     warnings.warn("Use `erlab.io.load_wave` instead", DeprecationWarning, stacklevel=2)
     return load_wave(*args, **kwargs)
```

### Comparing `erlab-2.1.2/src/erlab/io/dataloader.py` & `erlab-2.1.3/src/erlab/io/dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -932,17 +932,7 @@
             )
         out += "</tbody></table>"
 
         return out
 
     load.__doc__ = LoaderBase.load.__doc__
     summarize.__doc__ = LoaderBase.summarize.__doc__
-
-
-loaders: LoaderRegistry = LoaderRegistry.instance()
-"""Global instance of `LoaderRegistry`\n\n:meta hide-value:"""
-
-set_loader = loaders.set_loader
-loader_context = loaders.loader_context
-set_data_dir = loaders.set_data_dir
-load = loaders.load
-summarize = loaders.summarize
```

### Comparing `erlab-2.1.2/src/erlab/io/igor.py` & `erlab-2.1.3/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/io/plugins/__init__.py` & `erlab-2.1.3/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/io/plugins/da30.py` & `erlab-2.1.3/src/erlab/io/plugins/da30.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import xarray as xr
 
 from erlab.io.dataloader import LoaderBase
 from erlab.io.igor import load_experiment, load_wave
 
 
 class DA30Loader(LoaderBase):
-    name: str = "_da30"
-    aliases: list[str] = []
+    name: str = "da30"
+    aliases: list[str] = ["DA30"]
 
     name_map: dict[str, str] = {
         "eV": ["Kinetic Energy [eV]", "Energy [eV]"],
         "alpha": ["Y-Scale [deg]", "Thetax [deg]"],
         "beta": ["Thetay [deg]"],
         "hv": ["BL Energy", "Excitation Energy"],
     }
```

### Comparing `erlab-2.1.2/src/erlab/io/plugins/kriss.py` & `erlab-2.1.3/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/io/plugins/merlin.py` & `erlab-2.1.3/src/erlab/io/plugins/merlin.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/io/plugins/ssrl52.py` & `erlab-2.1.3/src/erlab/io/plugins/ssrl52.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/io/utilities.py` & `erlab-2.1.3/src/erlab/io/utilities.py`

 * *Files 9% similar despite different names*

```diff
@@ -107,54 +107,60 @@
                 warnings.warn(
                     f"The attribute {key} with invalid type {dt} will be removed",
                     stacklevel=1,
                 )
     return da
 
 
-def open_hdf5(filename: str | os.PathLike) -> xr.DataArray | xr.Dataset:
+def open_hdf5(filename: str | os.PathLike, **kwargs: dict) -> xr.DataArray | xr.Dataset:
     """Open data from an HDF5 file saved with `save_as_hdf5`.
 
     This is a thin wrapper around `xarray.open_dataarray` and `xarray.open_dataset`.
 
     Parameters
     ----------
     filename
         The path to the HDF5 file.
+    **kwargs
+        Extra arguments to `xarray.open_dataarray` or `xarray.open_dataset`.
 
     Returns
     -------
     xarray.DataArray or xarray.Dataset
         The opened data.
     """
+    kwargs.setdefault("engine", "h5netcdf")
     try:
-        return xr.open_dataarray(filename, engine="h5netcdf")
+        return xr.open_dataarray(filename, **kwargs)
     except ValueError:
-        return xr.open_dataset(filename, engine="h5netcdf")
+        return xr.open_dataset(filename, **kwargs)
 
 
-def load_hdf5(filename: str | os.PathLike) -> xr.DataArray | xr.Dataset:
+def load_hdf5(filename: str | os.PathLike, **kwargs: dict) -> xr.DataArray | xr.Dataset:
     """Load data from an HDF5 file saved with `save_as_hdf5`.
 
     This is a thin wrapper around `xarray.load_dataarray` and `xarray.load_dataset`.
 
     Parameters
     ----------
     filename
         The path to the HDF5 file.
+    **kwargs
+        Extra arguments to `xarray.load_dataarray` or `xarray.load_dataset`.
 
     Returns
     -------
     xarray.DataArray or xarray.Dataset
         The loaded data.
     """
+    kwargs.setdefault("engine", "h5netcdf")
     try:
-        return xr.load_dataarray(filename, engine="h5netcdf")
+        return xr.load_dataarray(filename, **kwargs)
     except ValueError:
-        return xr.load_dataset(filename, engine="h5netcdf")
+        return xr.load_dataset(filename, **kwargs)
 
 
 def save_as_hdf5(
     data: xr.DataArray | xr.Dataset,
     filename: str | os.PathLike,
     igor_compat: bool = True,
     **kwargs: dict,
@@ -223,15 +229,14 @@
     filename
         Target file name.
     **kwargs
         Extra arguments to `xarray.DataArray.to_netcdf`: refer to the `xarray`
         documentation for a list of all possible arguments.
 
     """
-    # data = data.assign_attrs(provenance="")
     kwargs.setdefault("engine", "h5netcdf")
     fix_attr_format(data).to_netcdf(
         filename,
         encoding={var: {"zlib": True, "complevel": 5} for var in data.coords},
         **kwargs,
     )
```

### Comparing `erlab-2.1.2/src/erlab/lattice.py` & `erlab-2.1.3/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/parallel.py` & `erlab-2.1.3/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.1.3/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.1.3/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.1.3/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.1.3/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.1.3/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.1.3/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.1.3/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.1.3/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.1.3/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.1.3/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/__init__.py` & `erlab-2.1.3/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/annotations.py` & `erlab-2.1.3/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/atoms.py` & `erlab-2.1.3/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/bz.py` & `erlab-2.1.3/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/colors.py` & `erlab-2.1.3/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/erplot.py` & `erlab-2.1.3/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/general.py` & `erlab-2.1.3/src/erlab/plotting/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/plot3d.py` & `erlab-2.1.3/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.1.3/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.1.3/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.1.3/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.1.3/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.1.3/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.1.3/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab.egg-info/PKG-INFO` & `erlab-2.1.3/src/erlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.1.2/src/erlab.egg-info/SOURCES.txt` & `erlab-2.1.3/src/erlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/src/erlab.egg-info/requires.txt` & `erlab-2.1.3/src/erlab.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/templates/.macros.j2` & `erlab-2.1.3/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/tests/analysis/test_fastbinning.py` & `erlab-2.1.3/tests/analysis/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/tests/analysis/test_fit_functions_dynamic.py` & `erlab-2.1.3/tests/analysis/test_fit_functions_dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/tests/analysis/test_fit_functions_general.py` & `erlab-2.1.3/tests/analysis/test_fit_functions_general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/tests/analysis/test_image.py` & `erlab-2.1.3/tests/analysis/test_image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/tests/analysis/test_interpolate.py` & `erlab-2.1.3/tests/analysis/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/tests/analysis/test_kspace.py` & `erlab-2.1.3/tests/analysis/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.2/tests/analysis/test_utilities.py` & `erlab-2.1.3/tests/analysis/test_utilities.py`

 * *Files identical despite different names*

