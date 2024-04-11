# Comparing `tmp/simulariumio-1.9.0.tar.gz` & `tmp/simulariumio-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulariumio-1.9.0.tar", last modified: Mon Oct 30 19:37:48 2023, max compression
+gzip compressed data, was "simulariumio-1.9.1.tar", last modified: Thu Nov  2 18:02:48 2023, max compression
```

## Comparing `simulariumio-1.9.0.tar` & `simulariumio-1.9.1.tar`

### file list

```diff
@@ -1,332 +1,332 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.539883 simulariumio-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-10-30 19:37:35.000000 simulariumio-1.9.0/.cookiecutter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-30 19:37:35.000000 simulariumio-1.9.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.479884 simulariumio-1.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-10-30 19:37:35.000000 simulariumio-1.9.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.479884 simulariumio-1.9.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2023-10-30 19:37:35.000000 simulariumio-1.9.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-10-30 19:37:35.000000 simulariumio-1.9.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-10-30 19:37:35.000000 simulariumio-1.9.0/.github/ISSUE_TEMPLATE/maintenance_task.md
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-10-30 19:37:35.000000 simulariumio-1.9.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-10-30 19:37:35.000000 simulariumio-1.9.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.479884 simulariumio-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2023-10-30 19:37:35.000000 simulariumio-1.9.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      324 2023-10-30 19:37:35.000000 simulariumio-1.9.0/.github/workflows/create-issue.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-10-30 19:37:35.000000 simulariumio-1.9.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2023-10-30 19:37:35.000000 simulariumio-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-10-30 19:37:35.000000 simulariumio-1.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2023-10-30 19:37:35.000000 simulariumio-1.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-10-30 19:37:35.000000 simulariumio-1.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2023-10-30 19:37:35.000000 simulariumio-1.9.0/Justfile
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2023-10-30 19:37:35.000000 simulariumio-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13006 2023-10-30 19:37:48.539883 simulariumio-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10325 2023-10-30 19:37:35.000000 simulariumio-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.479884 simulariumio-1.9.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-10-30 19:37:35.000000 simulariumio-1.9.0/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-30 19:37:35.000000 simulariumio-1.9.0/benchmarks/TEST_RESOURCES_HASH.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2023-10-30 19:37:35.000000 simulariumio-1.9.0/benchmarks/benchmark_simulariumio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2023-10-30 19:37:35.000000 simulariumio-1.9.0/benchmarks/download_benchmark_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2023-10-30 19:37:35.000000 simulariumio-1.9.0/benchmarks/upload_benchmark_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.483883 simulariumio-1.9.0/docs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5362 2023-10-30 19:37:35.000000 simulariumio-1.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-10-30 19:37:35.000000 simulariumio-1.9.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-30 19:37:35.000000 simulariumio-1.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2023-10-30 19:37:35.000000 simulariumio-1.9.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-10-30 19:37:35.000000 simulariumio-1.9.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-30 19:37:35.000000 simulariumio-1.9.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.483883 simulariumio-1.9.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/Tutorial_cellpack.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/Tutorial_custom.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9449 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/Tutorial_cytosim.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/Tutorial_filters.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/Tutorial_mcell.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/Tutorial_md.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/Tutorial_medyan.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/Tutorial_physicell.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/Tutorial_plots.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/Tutorial_readdy.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/Tutorial_smoldyn.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/Tutorial_springsalad.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.483883 simulariumio-1.9.0/examples/img/
--rw-r--r--   0 runner    (1001) docker     (127)  3109823 2023-10-30 19:37:35.000000 simulariumio-1.9.0/examples/img/drag_drop.gif
--rw-r--r--   0 runner    (1001) docker     (127)    13911 2023-10-30 19:37:35.000000 simulariumio-1.9.0/file_format.md
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2023-10-30 19:37:35.000000 simulariumio-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 19:37:48.539883 simulariumio-1.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.487883 simulariumio-1.9.0/simulariumio/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.487883 simulariumio-1.9.0/simulariumio/cellpack/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/cellpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15754 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/cellpack/cellpack_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/cellpack/cellpack_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.487883 simulariumio-1.9.0/simulariumio/cytosim/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/cytosim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13081 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/cytosim/cytosim_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/cytosim/cytosim_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/cytosim/cytosim_object_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.491883 simulariumio-1.9.0/simulariumio/data_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29455 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/agent_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/binary_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/camera_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/dimension_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/display_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/frame_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/histogram_plot_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/input_file_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/json_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/model_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/scatter_plot_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/simularium_file_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/trajectory_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/data_objects/unit_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/file_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.491883 simulariumio-1.9.0/simulariumio/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/filters/add_agents_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/filters/every_nth_agent_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/filters/every_nth_subpoint_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/filters/every_nth_timestep_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/filters/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/filters/multiply_space_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/filters/multiply_time_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/filters/transform_spatial_axes_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/filters/translate_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.491883 simulariumio-1.9.0/simulariumio/mcell/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/mcell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15510 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/mcell/mcell_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/mcell/mcell_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.491883 simulariumio-1.9.0/simulariumio/md/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/md/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8671 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/md/md_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/md/md_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.491883 simulariumio-1.9.0/simulariumio/medyan/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/medyan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12548 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/medyan/medyan_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/medyan/medyan_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.491883 simulariumio-1.9.0/simulariumio/package_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/package_data/jmolcolors.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.495884 simulariumio-1.9.0/simulariumio/physicell/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/physicell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.495884 simulariumio-1.9.0/simulariumio/physicell/dep/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/physicell/dep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21762 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/physicell/dep/pyMCDS.py
--rw-r--r--   0 runner    (1001) docker     (127)    16502 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/physicell/physicell_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/physicell/physicell_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.495884 simulariumio-1.9.0/simulariumio/plot_readers/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/plot_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/plot_readers/histogram_plot_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/plot_readers/plot_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/plot_readers/scatter_plot_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.495884 simulariumio-1.9.0/simulariumio/readdy/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/readdy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/readdy/readdy_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/readdy/readdy_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.495884 simulariumio-1.9.0/simulariumio/readers/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/readers/binary_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9134 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/readers/simularium_binary_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.495884 simulariumio-1.9.0/simulariumio/smoldyn/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/smoldyn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/smoldyn/smoldyn_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/smoldyn/smoldyn_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.495884 simulariumio-1.9.0/simulariumio/springsalad/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/springsalad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/springsalad/springsalad_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/springsalad/springsalad_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.495884 simulariumio-1.9.0/simulariumio/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.495884 simulariumio-1.9.0/simulariumio/tests/buffer/
--rw-r--r--   0 runner    (1001) docker     (127)    13522 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/buffer/test_buffer_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/buffer/test_buffer_size.py
--rw-r--r--   0 runner    (1001) docker     (127)    49341 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.499884 simulariumio-1.9.0/simulariumio/tests/converters/
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/converters/test_cellpack_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/converters/test_cytosim_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11048 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/converters/test_mcell_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/converters/test_md_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19860 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/converters/test_medyan_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    25088 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/converters/test_physicell_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12797 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/converters/test_readdy_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18199 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/converters/test_smoldyn_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16134 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/converters/test_springsalad_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    41763 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/converters/test_trajectory_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.475884 simulariumio-1.9.0/simulariumio/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.499884 simulariumio-1.9.0/simulariumio/tests/data/binary/
--rw-r--r--   0 runner    (1001) docker     (127)  1979356 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/binary/50filaments_motor_linker_binary.binary
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/binary/binary_test.binary
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.499884 simulariumio-1.9.0/simulariumio/tests/data/cellpack/
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cellpack/example_2D_recipe.json
--rw-r--r--   0 runner    (1001) docker     (127)    18827 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cellpack/example_2D_results.json
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cellpack/mock_recipe.json
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cellpack/mock_results.json
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cellpack/two_ingredients_recipe.json
--rw-r--r--   0 runner    (1001) docker     (127)    15676 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cellpack/two_ingredients_results.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.475884 simulariumio-1.9.0/simulariumio/tests/data/cytosim/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.499884 simulariumio-1.9.0/simulariumio/tests/data/cytosim/3_fibers_3_frames/
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/3_fibers_3_frames/fiber_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      815 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/3_fibers_3_frames/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.511883 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/aster_pull3D_couple_actin_solid.cym
--rw-r--r--   0 runner    (1001) docker     (127)  2076304 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/couples.txt
--rw-r--r--   0 runner    (1001) docker     (127)  8485882 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/fiber_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1461550 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/singles.txt
--rw-r--r--   0 runner    (1001) docker     (127)    68842 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/solids.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.515883 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couple_actin_solid.cym
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames.json
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames_small.json
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/couples.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/fiber_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/singles.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/solids.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.515883 simulariumio-1.9.0/simulariumio/tests/data/cytosim/fiber_test/
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/cytosim/fiber_test/fiber_points.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.515883 simulariumio-1.9.0/simulariumio/tests/data/malformed_data/
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/malformed_data/malformed_cytosim.txt
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/malformed_data/malformed_medyan.traj
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/malformed_data/malformed_smoldyn.txt
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/malformed_data/springsalad_broken_link.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.515883 simulariumio-1.9.0/simulariumio/tests/data/mcell/
--rw-r--r--   0 runner    (1001) docker     (127)  1033648 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example.blend
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.515883 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.515883 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/data_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.515883 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/
--rw-r--r--   0 runner    (1001) docker     (127)   157373 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.geometry.mdl
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.initialization.mdl
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.instantiation.mdl
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.main.mdl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.mod_surf_regions.mdl
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.molecules.mdl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.parameters.mdl
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.reactions.mdl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.release_patterns.mdl
--rw-r--r--   0 runner    (1001) docker     (127)      302 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.rxn_output.mdl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.surface_classes.mdl
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.viz_output.mdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.475884 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.519883 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/a.World.dat
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/b.World.dat
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/c.World.dat
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/d.World.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.475884 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.519883 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/Scene.cellbin.0.dat
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/Scene.cellbin.1.dat
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/Scene.cellbin.2.dat
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/start_time.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.519883 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_viz_output/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.cellbin.0.dat
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.cellbin.1.dat
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.cellbin.2.dat
--rw-r--r--   0 runner    (1001) docker     (127)   297563 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.data_model.00.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.519883 simulariumio-1.9.0/simulariumio/tests/data/md/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/md/example.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.519883 simulariumio-1.9.0/simulariumio/tests/data/medyan/
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/medyan/snapshot.traj
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/medyan/test.traj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.475884 simulariumio-1.9.0/simulariumio/tests/data/physicell/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.519883 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/initial.xml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/initial_cells.mat
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/initial_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (127)    80024 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/initial_mesh0.mat
--rw-r--r--   0 runner    (1001) docker     (127)   100047 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/initial_microenvironment0.mat
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000000.xml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000000_cells.mat
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000000_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (127)   100047 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000000_microenvironment0.mat
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000001.xml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000001_cells.mat
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000001_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (127)   100047 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000001_microenvironment0.mat
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000002.xml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000002_cells.mat
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000002_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (127)   100047 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000002_microenvironment0.mat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.527883 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/initial.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/initial_cells.mat
--rw-r--r--   0 runner    (1001) docker     (127)    11449 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/initial_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (127)   776184 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/initial_mesh0.mat
--rw-r--r--   0 runner    (1001) docker     (127)   970247 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/initial_microenvironment0.mat
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000000.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000000_cells.mat
--rw-r--r--   0 runner    (1001) docker     (127)    11673 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000000_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (127)   970247 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000000_microenvironment0.mat
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000001.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000001_cells.mat
--rw-r--r--   0 runner    (1001) docker     (127)    11449 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000001_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (127)   970247 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000001_microenvironment0.mat
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000002.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000002_cells.mat
--rw-r--r--   0 runner    (1001) docker     (127)    11449 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000002_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (127)   970247 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000002_microenvironment0.mat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.527883 simulariumio-1.9.0/simulariumio/tests/data/readdy/
--rw-r--r--   0 runner    (1001) docker     (127)    88121 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/readdy/test.h5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.527883 simulariumio-1.9.0/simulariumio/tests/data/smoldyn/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/smoldyn/example_2D.txt
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/smoldyn/example_3D.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/smoldyn/example_data.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.527883 simulariumio-1.9.0/simulariumio/tests/data/springsalad/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/springsalad/Simulation0_SIM_VIEW_Run0.txt
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/data/springsalad/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.531883 simulariumio-1.9.0/simulariumio/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (127)    11948 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/filters/test_add_agents_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26508 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/filters/test_every_nth_agent_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    31715 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/filters/test_every_nth_subpoint_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    25395 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/filters/test_every_nth_timestep_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/filters/test_multiply_space_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14420 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/filters/test_multiply_time_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/filters/test_transform_spatial_axes_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9672 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/filters/test_translate_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11703 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/filters/test_translate_filter_sphere_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.531883 simulariumio-1.9.0/simulariumio/tests/plot_readers/
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/plot_readers/test_histogram_plot_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/plot_readers/test_scatter_plot_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.531883 simulariumio-1.9.0/simulariumio/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/readers/test_binary_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8814 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/test_agents_from_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     9953 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/test_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/test_input_file_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/test_simularium_file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.531883 simulariumio-1.9.0/simulariumio/tests/writers/
--rw-r--r--   0 runner    (1001) docker     (127)    32766 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/tests/writers/test_binary_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17939 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/trajectory_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.531883 simulariumio-1.9.0/simulariumio/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/writers/binary_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/writers/binary_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    16185 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/writers/binary_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/writers/json_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2023-10-30 19:37:35.000000 simulariumio-1.9.0/simulariumio/writers/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.487883 simulariumio-1.9.0/simulariumio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13006 2023-10-30 19:37:48.000000 simulariumio-1.9.0/simulariumio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14083 2023-10-30 19:37:48.000000 simulariumio-1.9.0/simulariumio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 19:37:48.000000 simulariumio-1.9.0/simulariumio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 19:37:47.000000 simulariumio-1.9.0/simulariumio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-10-30 19:37:48.000000 simulariumio-1.9.0/simulariumio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-30 19:37:48.000000 simulariumio-1.9.0/simulariumio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.531883 simulariumio-1.9.0/ui-templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/base_types.json
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/cellpack_data.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 19:37:48.531883 simulariumio-1.9.0/ui-templates/custom-types/
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/custom-types/camera_data.json
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/custom-types/coordinates_xyz.json
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/custom-types/cytosim_object_info.json
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/custom-types/display_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/custom-types/meta_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/custom-types/model_meta_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/custom-types/space_unit_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/custom-types/time_unit_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/cytosim_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/medyan_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/smoldyn_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-10-30 19:37:35.000000 simulariumio-1.9.0/ui-templates/springsalad_data.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.850817 simulariumio-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2023-11-02 18:02:36.000000 simulariumio-1.9.1/.cookiecutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2023-11-02 18:02:36.000000 simulariumio-1.9.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.766817 simulariumio-1.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2023-11-02 18:02:36.000000 simulariumio-1.9.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.766817 simulariumio-1.9.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2023-11-02 18:02:36.000000 simulariumio-1.9.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2023-11-02 18:02:36.000000 simulariumio-1.9.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2023-11-02 18:02:36.000000 simulariumio-1.9.1/.github/ISSUE_TEMPLATE/maintenance_task.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-11-02 18:02:36.000000 simulariumio-1.9.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2023-11-02 18:02:36.000000 simulariumio-1.9.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.766817 simulariumio-1.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2023-11-02 18:02:36.000000 simulariumio-1.9.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2023-11-02 18:02:36.000000 simulariumio-1.9.1/.github/workflows/create-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-11-02 18:02:36.000000 simulariumio-1.9.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2023-11-02 18:02:36.000000 simulariumio-1.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2023-11-02 18:02:36.000000 simulariumio-1.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2023-11-02 18:02:36.000000 simulariumio-1.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-11-02 18:02:36.000000 simulariumio-1.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2023-11-02 18:02:36.000000 simulariumio-1.9.1/Justfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2023-11-02 18:02:36.000000 simulariumio-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2023-11-02 18:02:48.850817 simulariumio-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10325 2023-11-02 18:02:36.000000 simulariumio-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.770817 simulariumio-1.9.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-11-02 18:02:36.000000 simulariumio-1.9.1/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-11-02 18:02:36.000000 simulariumio-1.9.1/benchmarks/TEST_RESOURCES_HASH.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2023-11-02 18:02:36.000000 simulariumio-1.9.1/benchmarks/benchmark_simulariumio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2023-11-02 18:02:36.000000 simulariumio-1.9.1/benchmarks/download_benchmark_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2023-11-02 18:02:36.000000 simulariumio-1.9.1/benchmarks/upload_benchmark_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.770817 simulariumio-1.9.1/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5362 2023-11-02 18:02:36.000000 simulariumio-1.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-02 18:02:36.000000 simulariumio-1.9.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2023-11-02 18:02:36.000000 simulariumio-1.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2023-11-02 18:02:36.000000 simulariumio-1.9.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-02 18:02:36.000000 simulariumio-1.9.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-11-02 18:02:36.000000 simulariumio-1.9.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.770817 simulariumio-1.9.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/Tutorial_cellpack.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/Tutorial_custom.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9449 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/Tutorial_cytosim.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/Tutorial_filters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/Tutorial_mcell.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/Tutorial_md.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/Tutorial_medyan.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/Tutorial_physicell.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/Tutorial_plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/Tutorial_readdy.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/Tutorial_smoldyn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/Tutorial_springsalad.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.770817 simulariumio-1.9.1/examples/img/
+-rw-r--r--   0 runner    (1001) docker     (127)  3109823 2023-11-02 18:02:36.000000 simulariumio-1.9.1/examples/img/drag_drop.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    13911 2023-11-02 18:02:36.000000 simulariumio-1.9.1/file_format.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2023-11-02 18:02:36.000000 simulariumio-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-02 18:02:48.850817 simulariumio-1.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.778817 simulariumio-1.9.1/simulariumio/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.778817 simulariumio-1.9.1/simulariumio/cellpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/cellpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15754 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/cellpack/cellpack_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/cellpack/cellpack_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.778817 simulariumio-1.9.1/simulariumio/cytosim/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/cytosim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13081 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/cytosim/cytosim_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/cytosim/cytosim_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/cytosim/cytosim_object_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.782817 simulariumio-1.9.1/simulariumio/data_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29455 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/agent_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/binary_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/camera_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/dimension_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/display_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/frame_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/histogram_plot_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/input_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/json_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/model_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/scatter_plot_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/simularium_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/trajectory_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/data_objects/unit_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/file_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.782817 simulariumio-1.9.1/simulariumio/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/filters/add_agents_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/filters/every_nth_agent_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/filters/every_nth_subpoint_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/filters/every_nth_timestep_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/filters/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/filters/multiply_space_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/filters/multiply_time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/filters/transform_spatial_axes_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/filters/translate_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.782817 simulariumio-1.9.1/simulariumio/mcell/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/mcell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15510 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/mcell/mcell_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/mcell/mcell_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.782817 simulariumio-1.9.1/simulariumio/md/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8671 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/md/md_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/md/md_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.786817 simulariumio-1.9.1/simulariumio/medyan/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/medyan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12548 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/medyan/medyan_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/medyan/medyan_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.786817 simulariumio-1.9.1/simulariumio/package_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/package_data/jmolcolors.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.786817 simulariumio-1.9.1/simulariumio/physicell/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/physicell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.786817 simulariumio-1.9.1/simulariumio/physicell/dep/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/physicell/dep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21762 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/physicell/dep/pyMCDS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16502 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/physicell/physicell_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/physicell/physicell_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.786817 simulariumio-1.9.1/simulariumio/plot_readers/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/plot_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/plot_readers/histogram_plot_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/plot_readers/plot_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/plot_readers/scatter_plot_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.786817 simulariumio-1.9.1/simulariumio/readdy/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/readdy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/readdy/readdy_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/readdy/readdy_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.786817 simulariumio-1.9.1/simulariumio/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/readers/binary_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9134 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/readers/simularium_binary_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.786817 simulariumio-1.9.1/simulariumio/smoldyn/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/smoldyn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/smoldyn/smoldyn_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/smoldyn/smoldyn_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.790817 simulariumio-1.9.1/simulariumio/springsalad/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/springsalad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/springsalad/springsalad_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/springsalad/springsalad_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.790817 simulariumio-1.9.1/simulariumio/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.790817 simulariumio-1.9.1/simulariumio/tests/buffer/
+-rw-r--r--   0 runner    (1001) docker     (127)    13522 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/buffer/test_buffer_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/buffer/test_buffer_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49341 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.790817 simulariumio-1.9.1/simulariumio/tests/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/converters/test_cellpack_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/converters/test_cytosim_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11048 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/converters/test_mcell_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/converters/test_md_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19860 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/converters/test_medyan_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25088 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/converters/test_physicell_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12797 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/converters/test_readdy_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18199 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/converters/test_smoldyn_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16134 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/converters/test_springsalad_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41763 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/converters/test_trajectory_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.762817 simulariumio-1.9.1/simulariumio/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.794817 simulariumio-1.9.1/simulariumio/tests/data/binary/
+-rw-r--r--   0 runner    (1001) docker     (127)  1979356 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/binary/50filaments_motor_linker_binary.binary
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/binary/binary_test.binary
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.794817 simulariumio-1.9.1/simulariumio/tests/data/cellpack/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cellpack/example_2D_recipe.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18827 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cellpack/example_2D_results.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cellpack/mock_recipe.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cellpack/mock_results.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cellpack/two_ingredients_recipe.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15676 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cellpack/two_ingredients_results.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.758817 simulariumio-1.9.1/simulariumio/tests/data/cytosim/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.794817 simulariumio-1.9.1/simulariumio/tests/data/cytosim/3_fibers_3_frames/
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/3_fibers_3_frames/fiber_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/3_fibers_3_frames/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.810817 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/aster_pull3D_couple_actin_solid.cym
+-rw-r--r--   0 runner    (1001) docker     (127)  2076304 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/couples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  8485882 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/fiber_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1461550 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/singles.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    68842 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/solids.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.814817 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couple_actin_solid.cym
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames_small.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/couples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/fiber_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/singles.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/solids.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.814817 simulariumio-1.9.1/simulariumio/tests/data/cytosim/fiber_test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/cytosim/fiber_test/fiber_points.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.814817 simulariumio-1.9.1/simulariumio/tests/data/malformed_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/malformed_data/malformed_cytosim.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/malformed_data/malformed_medyan.traj
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/malformed_data/malformed_smoldyn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/malformed_data/springsalad_broken_link.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.814817 simulariumio-1.9.1/simulariumio/tests/data/mcell/
+-rw-r--r--   0 runner    (1001) docker     (127)  1033648 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example.blend
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.818817 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.818817 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/data_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.818817 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   157373 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.geometry.mdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.initialization.mdl
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.instantiation.mdl
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.main.mdl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.mod_surf_regions.mdl
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.molecules.mdl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.parameters.mdl
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.reactions.mdl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.release_patterns.mdl
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.rxn_output.mdl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.surface_classes.mdl
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.viz_output.mdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.762817 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.818817 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/a.World.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/b.World.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/c.World.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/d.World.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.762817 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.822817 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/Scene.cellbin.0.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/Scene.cellbin.1.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/Scene.cellbin.2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/start_time.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.822817 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_viz_output/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.cellbin.0.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.cellbin.1.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.cellbin.2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   297563 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.data_model.00.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.822817 simulariumio-1.9.1/simulariumio/tests/data/md/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/md/example.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.822817 simulariumio-1.9.1/simulariumio/tests/data/medyan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/medyan/snapshot.traj
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/medyan/test.traj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.762817 simulariumio-1.9.1/simulariumio/tests/data/physicell/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.826817 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/initial.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/initial_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/initial_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (127)    80024 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/initial_mesh0.mat
+-rw-r--r--   0 runner    (1001) docker     (127)   100047 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/initial_microenvironment0.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000000.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000000_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000000_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (127)   100047 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000000_microenvironment0.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000001.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000001_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000001_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (127)   100047 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000001_microenvironment0.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000002.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000002_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000002_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (127)   100047 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000002_microenvironment0.mat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.834817 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/initial.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/initial_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/initial_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (127)   776184 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/initial_mesh0.mat
+-rw-r--r--   0 runner    (1001) docker     (127)   970247 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/initial_microenvironment0.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000000.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000000_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (127)    11673 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000000_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (127)   970247 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000000_microenvironment0.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000001.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000001_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000001_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (127)   970247 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000001_microenvironment0.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000002.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000002_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000002_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (127)   970247 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000002_microenvironment0.mat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.838817 simulariumio-1.9.1/simulariumio/tests/data/readdy/
+-rw-r--r--   0 runner    (1001) docker     (127)    88121 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/readdy/test.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.838817 simulariumio-1.9.1/simulariumio/tests/data/smoldyn/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/smoldyn/example_2D.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/smoldyn/example_3D.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/smoldyn/example_data.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.838817 simulariumio-1.9.1/simulariumio/tests/data/springsalad/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/springsalad/Simulation0_SIM_VIEW_Run0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/data/springsalad/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.838817 simulariumio-1.9.1/simulariumio/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/filters/test_add_agents_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26508 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/filters/test_every_nth_agent_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31715 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/filters/test_every_nth_subpoint_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25395 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/filters/test_every_nth_timestep_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/filters/test_multiply_space_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14420 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/filters/test_multiply_time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/filters/test_transform_spatial_axes_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9672 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/filters/test_translate_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11703 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/filters/test_translate_filter_sphere_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.842817 simulariumio-1.9.1/simulariumio/tests/plot_readers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/plot_readers/test_histogram_plot_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/plot_readers/test_scatter_plot_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.842817 simulariumio-1.9.1/simulariumio/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/readers/test_binary_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8814 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/test_agents_from_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9953 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/test_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/test_input_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/test_simularium_file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.842817 simulariumio-1.9.1/simulariumio/tests/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)    32766 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/tests/writers/test_binary_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17939 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/trajectory_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.842817 simulariumio-1.9.1/simulariumio/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/writers/binary_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/writers/binary_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16185 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/writers/binary_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/writers/json_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2023-11-02 18:02:36.000000 simulariumio-1.9.1/simulariumio/writers/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.778817 simulariumio-1.9.1/simulariumio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2023-11-02 18:02:48.000000 simulariumio-1.9.1/simulariumio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14083 2023-11-02 18:02:48.000000 simulariumio-1.9.1/simulariumio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 18:02:48.000000 simulariumio-1.9.1/simulariumio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 18:02:48.000000 simulariumio-1.9.1/simulariumio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2023-11-02 18:02:48.000000 simulariumio-1.9.1/simulariumio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-02 18:02:48.000000 simulariumio-1.9.1/simulariumio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.842817 simulariumio-1.9.1/ui-templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/base_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/cellpack_data.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 18:02:48.846817 simulariumio-1.9.1/ui-templates/custom-types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/custom-types/camera_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/custom-types/coordinates_xyz.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/custom-types/cytosim_object_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/custom-types/display_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/custom-types/meta_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/custom-types/model_meta_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/custom-types/space_unit_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/custom-types/time_unit_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/cytosim_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/medyan_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/smoldyn_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-11-02 18:02:36.000000 simulariumio-1.9.1/ui-templates/springsalad_data.json
```

### Comparing `simulariumio-1.9.0/.github/PULL_REQUEST_TEMPLATE.md` & `simulariumio-1.9.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/.github/workflows/ci.yml` & `simulariumio-1.9.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/.github/workflows/docs.yml` & `simulariumio-1.9.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/.gitignore` & `simulariumio-1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/CODE_OF_CONDUCT.md` & `simulariumio-1.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/CONTRIBUTING.md` & `simulariumio-1.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/Justfile` & `simulariumio-1.9.1/Justfile`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/LICENSE` & `simulariumio-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/PKG-INFO` & `simulariumio-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulariumio
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python package that converts simulation outputs to the format consumed by the Simularium viewer website
 Author-email: Blair Lyons <blairl@alleninstitute.org>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://github.com/Simularium/simulariumio
 Project-URL: Bug Tracker, https://github.com/Simularium/simulariumio/issues
 Project-URL: Documentation, https://Simularium.github.io/simulariumio
 Project-URL: User Support, https://github.com/Simularium/simulariumio/issues
```

### Comparing `simulariumio-1.9.0/README.md` & `simulariumio-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/benchmarks/README.md` & `simulariumio-1.9.1/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/benchmarks/benchmark_simulariumio.py` & `simulariumio-1.9.1/benchmarks/benchmark_simulariumio.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/benchmarks/download_benchmark_resources.py` & `simulariumio-1.9.1/benchmarks/download_benchmark_resources.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/benchmarks/upload_benchmark_resources.py` & `simulariumio-1.9.1/benchmarks/upload_benchmark_resources.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/docs/conf.py` & `simulariumio-1.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/docs/installation.rst` & `simulariumio-1.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/examples/Tutorial_cellpack.ipynb` & `simulariumio-1.9.1/examples/Tutorial_cellpack.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/examples/Tutorial_custom.ipynb` & `simulariumio-1.9.1/examples/Tutorial_custom.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/examples/Tutorial_cytosim.ipynb` & `simulariumio-1.9.1/examples/Tutorial_cytosim.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/examples/Tutorial_filters.ipynb` & `simulariumio-1.9.1/examples/Tutorial_filters.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/examples/Tutorial_mcell.ipynb` & `simulariumio-1.9.1/examples/Tutorial_mcell.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/examples/Tutorial_md.ipynb` & `simulariumio-1.9.1/examples/Tutorial_md.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/examples/Tutorial_medyan.ipynb` & `simulariumio-1.9.1/examples/Tutorial_medyan.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/examples/Tutorial_physicell.ipynb` & `simulariumio-1.9.1/examples/Tutorial_physicell.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/examples/Tutorial_plots.ipynb` & `simulariumio-1.9.1/examples/Tutorial_plots.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/examples/Tutorial_readdy.ipynb` & `simulariumio-1.9.1/examples/Tutorial_readdy.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/examples/Tutorial_smoldyn.ipynb` & `simulariumio-1.9.1/examples/Tutorial_smoldyn.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/examples/Tutorial_springsalad.ipynb` & `simulariumio-1.9.1/examples/Tutorial_springsalad.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/examples/img/drag_drop.gif` & `simulariumio-1.9.1/examples/img/drag_drop.gif`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/file_format.md` & `simulariumio-1.9.1/file_format.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/pyproject.toml` & `simulariumio-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/__init__.py` & `simulariumio-1.9.1/simulariumio/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,13 +18,17 @@
     HistogramPlotData,
     InputFileData,
     MetaData,
     ModelMetaData,
     ScatterPlotData,
     TrajectoryData,
     UnitData,
+    FrameData,
+    SimulariumFileData,
+    JsonData,
+    BinaryData,
 )
 # DO NOT ISORT DISPLAY_TYPE, CAUSES CIRCULAR DEP
-from .constants import DISPLAY_TYPE  # noqa: F401
+from .constants import BINARY_SETTINGS, DISPLAY_TYPE  # noqa: F401
 from .file_converter import FileConverter  # noqa: F401
 from .trajectory_converter import TrajectoryConverter  # noqa: F401
 from .writers import BinaryWriter, JsonWriter  # noqa: F401
```

### Comparing `simulariumio-1.9.0/simulariumio/cellpack/cellpack_converter.py` & `simulariumio-1.9.1/simulariumio/cellpack/cellpack_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/cellpack/cellpack_data.py` & `simulariumio-1.9.1/simulariumio/cellpack/cellpack_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/constants.py` & `simulariumio-1.9.1/simulariumio/constants.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/cytosim/cytosim_converter.py` & `simulariumio-1.9.1/simulariumio/cytosim/cytosim_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/cytosim/cytosim_data.py` & `simulariumio-1.9.1/simulariumio/cytosim/cytosim_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/cytosim/cytosim_object_info.py` & `simulariumio-1.9.1/simulariumio/cytosim/cytosim_object_info.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/__init__.py` & `simulariumio-1.9.1/simulariumio/data_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/agent_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/agent_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/binary_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/binary_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/camera_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/camera_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/dimension_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/dimension_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/display_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/display_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/frame_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/frame_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/histogram_plot_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/histogram_plot_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/input_file_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/input_file_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/json_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/json_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/meta_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/meta_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/model_meta_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/model_meta_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/scatter_plot_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/scatter_plot_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/simularium_file_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/simularium_file_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/trajectory_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/trajectory_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/data_objects/unit_data.py` & `simulariumio-1.9.1/simulariumio/data_objects/unit_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/exceptions.py` & `simulariumio-1.9.1/simulariumio/exceptions.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/file_converter.py` & `simulariumio-1.9.1/simulariumio/file_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/filters/__init__.py` & `simulariumio-1.9.1/simulariumio/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/filters/add_agents_filter.py` & `simulariumio-1.9.1/simulariumio/filters/add_agents_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/filters/every_nth_agent_filter.py` & `simulariumio-1.9.1/simulariumio/filters/every_nth_agent_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/filters/every_nth_subpoint_filter.py` & `simulariumio-1.9.1/simulariumio/filters/every_nth_subpoint_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/filters/every_nth_timestep_filter.py` & `simulariumio-1.9.1/simulariumio/filters/every_nth_timestep_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/filters/filter.py` & `simulariumio-1.9.1/simulariumio/filters/filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/filters/multiply_space_filter.py` & `simulariumio-1.9.1/simulariumio/filters/multiply_space_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/filters/multiply_time_filter.py` & `simulariumio-1.9.1/simulariumio/filters/multiply_time_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/filters/transform_spatial_axes_filter.py` & `simulariumio-1.9.1/simulariumio/filters/transform_spatial_axes_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/filters/translate_filter.py` & `simulariumio-1.9.1/simulariumio/filters/translate_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/mcell/mcell_converter.py` & `simulariumio-1.9.1/simulariumio/mcell/mcell_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/mcell/mcell_data.py` & `simulariumio-1.9.1/simulariumio/mcell/mcell_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/md/md_converter.py` & `simulariumio-1.9.1/simulariumio/md/md_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/md/md_data.py` & `simulariumio-1.9.1/simulariumio/md/md_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/medyan/medyan_converter.py` & `simulariumio-1.9.1/simulariumio/medyan/medyan_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/medyan/medyan_data.py` & `simulariumio-1.9.1/simulariumio/medyan/medyan_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/package_data/jmolcolors.csv` & `simulariumio-1.9.1/simulariumio/package_data/jmolcolors.csv`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/physicell/dep/pyMCDS.py` & `simulariumio-1.9.1/simulariumio/physicell/dep/pyMCDS.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/physicell/physicell_converter.py` & `simulariumio-1.9.1/simulariumio/physicell/physicell_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/physicell/physicell_data.py` & `simulariumio-1.9.1/simulariumio/physicell/physicell_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/plot_readers/histogram_plot_reader.py` & `simulariumio-1.9.1/simulariumio/plot_readers/histogram_plot_reader.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/plot_readers/scatter_plot_reader.py` & `simulariumio-1.9.1/simulariumio/plot_readers/scatter_plot_reader.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/readdy/readdy_converter.py` & `simulariumio-1.9.1/simulariumio/readdy/readdy_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/readdy/readdy_data.py` & `simulariumio-1.9.1/simulariumio/readdy/readdy_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/readers/binary_info.py` & `simulariumio-1.9.1/simulariumio/readers/binary_info.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/readers/simularium_binary_reader.py` & `simulariumio-1.9.1/simulariumio/readers/simularium_binary_reader.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/smoldyn/smoldyn_converter.py` & `simulariumio-1.9.1/simulariumio/smoldyn/smoldyn_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/smoldyn/smoldyn_data.py` & `simulariumio-1.9.1/simulariumio/smoldyn/smoldyn_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/springsalad/springsalad_converter.py` & `simulariumio-1.9.1/simulariumio/springsalad/springsalad_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/springsalad/springsalad_data.py` & `simulariumio-1.9.1/simulariumio/springsalad/springsalad_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/buffer/test_buffer_contents.py` & `simulariumio-1.9.1/simulariumio/tests/buffer/test_buffer_contents.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/buffer/test_buffer_size.py` & `simulariumio-1.9.1/simulariumio/tests/buffer/test_buffer_size.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/conftest.py` & `simulariumio-1.9.1/simulariumio/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/converters/test_cellpack_converter.py` & `simulariumio-1.9.1/simulariumio/tests/converters/test_cellpack_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/converters/test_cytosim_converter.py` & `simulariumio-1.9.1/simulariumio/tests/converters/test_cytosim_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/converters/test_mcell_converter.py` & `simulariumio-1.9.1/simulariumio/tests/converters/test_mcell_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/converters/test_md_converter.py` & `simulariumio-1.9.1/simulariumio/tests/converters/test_md_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/converters/test_medyan_converter.py` & `simulariumio-1.9.1/simulariumio/tests/converters/test_medyan_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/converters/test_physicell_converter.py` & `simulariumio-1.9.1/simulariumio/tests/converters/test_physicell_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/converters/test_readdy_converter.py` & `simulariumio-1.9.1/simulariumio/tests/converters/test_readdy_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/converters/test_smoldyn_converter.py` & `simulariumio-1.9.1/simulariumio/tests/converters/test_smoldyn_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/converters/test_springsalad_converter.py` & `simulariumio-1.9.1/simulariumio/tests/converters/test_springsalad_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/converters/test_trajectory_converter.py` & `simulariumio-1.9.1/simulariumio/tests/converters/test_trajectory_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/binary/50filaments_motor_linker_binary.binary` & `simulariumio-1.9.1/simulariumio/tests/data/binary/50filaments_motor_linker_binary.binary`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/binary/binary_test.binary` & `simulariumio-1.9.1/simulariumio/tests/data/binary/binary_test.binary`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cellpack/example_2D_recipe.json` & `simulariumio-1.9.1/simulariumio/tests/data/cellpack/example_2D_recipe.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cellpack/example_2D_results.json` & `simulariumio-1.9.1/simulariumio/tests/data/cellpack/example_2D_results.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cellpack/mock_recipe.json` & `simulariumio-1.9.1/simulariumio/tests/data/cellpack/mock_recipe.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cellpack/mock_results.json` & `simulariumio-1.9.1/simulariumio/tests/data/cellpack/mock_results.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cellpack/two_ingredients_recipe.json` & `simulariumio-1.9.1/simulariumio/tests/data/cellpack/two_ingredients_recipe.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cellpack/two_ingredients_results.json` & `simulariumio-1.9.1/simulariumio/tests/data/cellpack/two_ingredients_results.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/3_fibers_3_frames/fiber_points.txt` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/3_fibers_3_frames/fiber_points.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/3_fibers_3_frames/test.txt` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/3_fibers_3_frames/test.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/aster_pull3D_couple_actin_solid.cym` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/aster_pull3D_couple_actin_solid.cym`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/couples.txt` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/couples.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/fiber_points.txt` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/fiber_points.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/singles.txt` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/singles.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/solids.txt` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/solids.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couple_actin_solid.cym` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couple_actin_solid.cym`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames.json` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames_small.json` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames_small.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/couples.txt` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/couples.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/fiber_points.txt` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/fiber_points.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/singles.txt` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/singles.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/solids.txt` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/solids.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/cytosim/fiber_test/fiber_points.txt` & `simulariumio-1.9.1/simulariumio/tests/data/cytosim/fiber_test/fiber_points.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/malformed_data/malformed_cytosim.txt` & `simulariumio-1.9.1/simulariumio/tests/data/malformed_data/malformed_cytosim.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/malformed_data/malformed_medyan.traj` & `simulariumio-1.9.1/simulariumio/tests/data/malformed_data/malformed_medyan.traj`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/malformed_data/springsalad_broken_link.txt` & `simulariumio-1.9.1/simulariumio/tests/data/malformed_data/springsalad_broken_link.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example.blend` & `simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example.blend`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.geometry.mdl` & `simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.geometry.mdl`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.initialization.mdl` & `simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.initialization.mdl`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.instantiation.mdl` & `simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.instantiation.mdl`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.data_model.00.json` & `simulariumio-1.9.1/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.data_model.00.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/medyan/snapshot.traj` & `simulariumio-1.9.1/simulariumio/tests/data/medyan/snapshot.traj`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/medyan/test.traj` & `simulariumio-1.9.1/simulariumio/tests/data/medyan/test.traj`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/initial.xml` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/initial.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/initial_cells_physicell.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/initial_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/initial_mesh0.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/initial_mesh0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/initial_microenvironment0.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/initial_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000000.xml` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000000.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000000_cells_physicell.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000000_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000000_microenvironment0.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000000_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000001.xml` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000001.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000001_cells_physicell.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000001_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000001_microenvironment0.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000001_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000002.xml` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000002.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000002_cells_physicell.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000002_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/default_output/output00000002_microenvironment0.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/default_output/output00000002_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/initial.xml` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/initial.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/initial_cells.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/initial_cells.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/initial_cells_physicell.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/initial_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/initial_mesh0.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/initial_mesh0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/initial_microenvironment0.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/initial_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000000.xml` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000000.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000000_cells.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000000_cells.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000000_cells_physicell.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000000_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000000_microenvironment0.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000000_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000001.xml` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000001.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000001_cells.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000001_cells.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000001_cells_physicell.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000001_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000001_microenvironment0.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000001_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000002.xml` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000002.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000002_cells.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000002_cells.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000002_cells_physicell.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000002_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/physicell/subcell_output/output00000002_microenvironment0.mat` & `simulariumio-1.9.1/simulariumio/tests/data/physicell/subcell_output/output00000002_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/readdy/test.h5` & `simulariumio-1.9.1/simulariumio/tests/data/readdy/test.h5`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/springsalad/Simulation0_SIM_VIEW_Run0.txt` & `simulariumio-1.9.1/simulariumio/tests/data/springsalad/Simulation0_SIM_VIEW_Run0.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/data/springsalad/test.txt` & `simulariumio-1.9.1/simulariumio/tests/data/springsalad/test.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/filters/test_add_agents_filter.py` & `simulariumio-1.9.1/simulariumio/tests/filters/test_add_agents_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/filters/test_every_nth_agent_filter.py` & `simulariumio-1.9.1/simulariumio/tests/filters/test_every_nth_agent_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/filters/test_every_nth_subpoint_filter.py` & `simulariumio-1.9.1/simulariumio/tests/filters/test_every_nth_subpoint_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/filters/test_every_nth_timestep_filter.py` & `simulariumio-1.9.1/simulariumio/tests/filters/test_every_nth_timestep_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/filters/test_multiply_space_filter.py` & `simulariumio-1.9.1/simulariumio/tests/filters/test_multiply_space_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/filters/test_multiply_time_filter.py` & `simulariumio-1.9.1/simulariumio/tests/filters/test_multiply_time_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/filters/test_transform_spatial_axes_filter.py` & `simulariumio-1.9.1/simulariumio/tests/filters/test_transform_spatial_axes_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/filters/test_translate_filter.py` & `simulariumio-1.9.1/simulariumio/tests/filters/test_translate_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/filters/test_translate_filter_sphere_groups.py` & `simulariumio-1.9.1/simulariumio/tests/filters/test_translate_filter_sphere_groups.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/plot_readers/test_histogram_plot_reader.py` & `simulariumio-1.9.1/simulariumio/tests/plot_readers/test_histogram_plot_reader.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/plot_readers/test_scatter_plot_reader.py` & `simulariumio-1.9.1/simulariumio/tests/plot_readers/test_scatter_plot_reader.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/readers/test_binary_reader.py` & `simulariumio-1.9.1/simulariumio/tests/readers/test_binary_reader.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/test_agents_from_lists.py` & `simulariumio-1.9.1/simulariumio/tests/test_agents_from_lists.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/test_from_dict.py` & `simulariumio-1.9.1/simulariumio/tests/test_from_dict.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/test_input_file_data.py` & `simulariumio-1.9.1/simulariumio/tests/test_input_file_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/test_simularium_file_data.py` & `simulariumio-1.9.1/simulariumio/tests/test_simularium_file_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/tests/writers/test_binary_writer.py` & `simulariumio-1.9.1/simulariumio/tests/writers/test_binary_writer.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/trajectory_converter.py` & `simulariumio-1.9.1/simulariumio/trajectory_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/utils.py` & `simulariumio-1.9.1/simulariumio/utils.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/writers/binary_chunk.py` & `simulariumio-1.9.1/simulariumio/writers/binary_chunk.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/writers/binary_values.py` & `simulariumio-1.9.1/simulariumio/writers/binary_values.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/writers/binary_writer.py` & `simulariumio-1.9.1/simulariumio/writers/binary_writer.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/writers/json_writer.py` & `simulariumio-1.9.1/simulariumio/writers/json_writer.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio/writers/writer.py` & `simulariumio-1.9.1/simulariumio/writers/writer.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio.egg-info/PKG-INFO` & `simulariumio-1.9.1/simulariumio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulariumio
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python package that converts simulation outputs to the format consumed by the Simularium viewer website
 Author-email: Blair Lyons <blairl@alleninstitute.org>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://github.com/Simularium/simulariumio
 Project-URL: Bug Tracker, https://github.com/Simularium/simulariumio/issues
 Project-URL: Documentation, https://Simularium.github.io/simulariumio
 Project-URL: User Support, https://github.com/Simularium/simulariumio/issues
```

### Comparing `simulariumio-1.9.0/simulariumio.egg-info/SOURCES.txt` & `simulariumio-1.9.1/simulariumio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/simulariumio.egg-info/requires.txt` & `simulariumio-1.9.1/simulariumio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/README.md` & `simulariumio-1.9.1/ui-templates/README.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/base_types.json` & `simulariumio-1.9.1/ui-templates/base_types.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/cellpack_data.json` & `simulariumio-1.9.1/ui-templates/cellpack_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/custom-types/camera_data.json` & `simulariumio-1.9.1/ui-templates/custom-types/camera_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/custom-types/coordinates_xyz.json` & `simulariumio-1.9.1/ui-templates/custom-types/coordinates_xyz.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/custom-types/cytosim_object_info.json` & `simulariumio-1.9.1/ui-templates/custom-types/cytosim_object_info.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/custom-types/display_data.json` & `simulariumio-1.9.1/ui-templates/custom-types/display_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/custom-types/meta_data.json` & `simulariumio-1.9.1/ui-templates/custom-types/meta_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/custom-types/model_meta_data.json` & `simulariumio-1.9.1/ui-templates/custom-types/model_meta_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/custom-types/space_unit_data.json` & `simulariumio-1.9.1/ui-templates/custom-types/space_unit_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/custom-types/time_unit_data.json` & `simulariumio-1.9.1/ui-templates/custom-types/time_unit_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/cytosim_data.json` & `simulariumio-1.9.1/ui-templates/cytosim_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/medyan_data.json` & `simulariumio-1.9.1/ui-templates/medyan_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/smoldyn_data.json` & `simulariumio-1.9.1/ui-templates/smoldyn_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.9.0/ui-templates/springsalad_data.json` & `simulariumio-1.9.1/ui-templates/springsalad_data.json`

 * *Files identical despite different names*

