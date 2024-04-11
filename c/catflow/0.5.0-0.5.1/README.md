# Comparing `tmp/catflow-0.5.0.tar.gz` & `tmp/catflow-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catflow-0.5.0.tar", max compression
+gzip compressed data, was "catflow-0.5.1.tar", max compression
```

## Comparing `catflow-0.5.0.tar` & `catflow-0.5.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    11357 2024-04-08 08:43:29.925534 catflow-0.5.0/LICENSE
--rw-r--r--   0        0        0     3433 2024-04-08 08:43:29.925534 catflow-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/atomic/__init__.py
--rw-r--r--   0        0        0      826 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/atomic/atomic_energy.py
--rw-r--r--   0        0        0     4532 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/atomic/utils.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/graph/__init__.py
--rw-r--r--   0        0        0     2472 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/graph/plotting.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/metad/__init__.py
--rw-r--r--   0        0        0    34345 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/metad/fes.py
--rw-r--r--   0        0        0     4392 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/metad/hills.py
--rw-r--r--   0        0        0     6469 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/metad/profile.py
--rw-r--r--   0        0        0    15587 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/metad/string.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/structure/__init__.py
--rw-r--r--   0        0        0     4936 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/structure/cluster.py
--rw-r--r--   0        0        0     2287 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/structure/coordination_number.py
--rw-r--r--   0        0        0    10306 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/structure/dynamic_selection.py
--rw-r--r--   0        0        0     1377 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/structure/lindemann_index.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/__init__.py
--rw-r--r--   0        0        0     1449 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/exploration.py
--rw-r--r--   0        0        0      573 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/labeling.py
--rw-r--r--   0        0        0     1750 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/task.py
--rw-r--r--   0        0        0     1471 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/training.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/base/__init__.py
--rw-r--r--   0        0        0    24722 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/base/exploration.py
--rw-r--r--   0        0        0     4475 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/base/labeling.py
--rw-r--r--   0        0        0      829 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/base/task.py
--rw-r--r--   0        0        0     2813 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/base/training.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/dpgen/__init__.py
--rw-r--r--   0        0        0    11349 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/dpgen/exploration.py
--rw-r--r--   0        0        0      749 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/dpgen/labeling.py
--rw-r--r--   0        0        0     3365 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/dpgen/task.py
--rw-r--r--   0        0        0     2079 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/dpgen/training.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/__init__.py
--rw-r--r--   0        0        0      553 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/base.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/calculation/__init__.py
--rw-r--r--   0        0        0     1520 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/calculation/dpgen.py
--rw-r--r--   0        0        0      468 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/calculation/vasp.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/workflow/__init__.py
--rw-r--r--   0        0        0      796 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/workflow/pmf.py
--rw-r--r--   0        0        0     1644 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/workflow/tesla.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/__init__.py
--rw-r--r--   0        0        0      111 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/__main__.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/calculation/__init__.py
--rw-r--r--   0        0        0       70 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/calculation/cp2k.py
--rw-r--r--   0        0        0    18491 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/calculation/dpgen.py
--rw-r--r--   0        0        0     9017 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/calculation/vasp.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/code/__init__.py
--rw-r--r--   0        0        0      915 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/code/base.py
--rw-r--r--   0        0        0      150 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/code/vasp.py
--rw-r--r--   0        0        0      882 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/configs/workflow/pmf_cp2k.yml
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/flows/__init__.py
--rw-r--r--   0        0        0    32933 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/flows/pmf_flow.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/resources/__init__.py
--rw-r--r--   0        0        0      376 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/resources/config.py
--rw-r--r--   0        0        0     1446 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/resources/submit.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/runner/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/tasks/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/tasks/defaults/__init__.py
--rw-r--r--   0        0        0     1795 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/tasks/defaults/pmf.py
--rw-r--r--   0        0        0    12976 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/tasks/pmf.py
--rw-r--r--   0        0        0    10450 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/tasks/screen.py
--rw-r--r--   0        0        0    24938 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/tasks/tesla.py
--rw-r--r--   0        0        0       54 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/__init__.py
--rw-r--r--   0        0        0     1089 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/config.py
--rw-r--r--   0        0        0     1957 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/constant.py
--rw-r--r--   0        0        0    13850 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/cp2k.py
--rw-r--r--   0        0        0      966 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/file.py
--rw-r--r--   0        0        0     3585 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/lammps.py
--rw-r--r--   0        0        0     1083 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/log_factory.py
--rw-r--r--   0        0        0     1283 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/messager.py
--rw-r--r--   0        0        0       45 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/output.py
--rw-r--r--   0        0        0     1629 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/statistics.py
--rw-r--r--   0        0        0     1229 2024-04-08 08:43:29.945534 catflow-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5344 1970-01-01 00:00:00.000000 catflow-0.5.0/setup.py
--rw-r--r--   0        0        0     4790 1970-01-01 00:00:00.000000 catflow-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-11 11:33:09.695316 catflow-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3410 2024-04-11 11:33:09.695316 catflow-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/atomic/__init__.py
+-rw-r--r--   0        0        0      826 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/atomic/atomic_energy.py
+-rw-r--r--   0        0        0     4532 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/atomic/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/graph/__init__.py
+-rw-r--r--   0        0        0     2472 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/graph/plotting.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/metad/__init__.py
+-rw-r--r--   0        0        0     1153 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/metad/colvar.py
+-rw-r--r--   0        0        0    39182 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/metad/fes.py
+-rw-r--r--   0        0        0     4392 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/metad/hills.py
+-rw-r--r--   0        0        0     6469 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/metad/profile.py
+-rw-r--r--   0        0        0    15587 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/metad/string.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/structure/__init__.py
+-rw-r--r--   0        0        0     4936 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/structure/cluster.py
+-rw-r--r--   0        0        0     2287 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/structure/coordination_number.py
+-rw-r--r--   0        0        0    10306 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/structure/dynamic_selection.py
+-rw-r--r--   0        0        0     1377 2024-04-11 11:33:09.695316 catflow-0.5.1/catflow/analyzer/structure/lindemann_index.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/ai2_kit/__init__.py
+-rw-r--r--   0        0        0     1449 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/ai2_kit/exploration.py
+-rw-r--r--   0        0        0      573 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/ai2_kit/labeling.py
+-rw-r--r--   0        0        0     1750 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/ai2_kit/task.py
+-rw-r--r--   0        0        0     1471 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/ai2_kit/training.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/base/__init__.py
+-rw-r--r--   0        0        0    24722 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/base/exploration.py
+-rw-r--r--   0        0        0     4475 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/base/labeling.py
+-rw-r--r--   0        0        0      829 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/base/task.py
+-rw-r--r--   0        0        0     2813 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/base/training.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/dpgen/__init__.py
+-rw-r--r--   0        0        0    11349 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/dpgen/exploration.py
+-rw-r--r--   0        0        0      749 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/dpgen/labeling.py
+-rw-r--r--   0        0        0     3365 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/dpgen/task.py
+-rw-r--r--   0        0        0     2079 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/analyzer/tesla/dpgen/training.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/cmdline/__init__.py
+-rw-r--r--   0        0        0      553 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/cmdline/base.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/cmdline/calculation/__init__.py
+-rw-r--r--   0        0        0     1520 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/cmdline/calculation/dpgen.py
+-rw-r--r--   0        0        0      468 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/cmdline/calculation/vasp.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/cmdline/workflow/__init__.py
+-rw-r--r--   0        0        0      796 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/cmdline/workflow/pmf.py
+-rw-r--r--   0        0        0     1644 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/cmdline/workflow/tesla.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/__init__.py
+-rw-r--r--   0        0        0      111 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/calculation/__init__.py
+-rw-r--r--   0        0        0       70 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/calculation/cp2k.py
+-rw-r--r--   0        0        0    18491 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/calculation/dpgen.py
+-rw-r--r--   0        0        0     9017 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/calculation/vasp.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/code/__init__.py
+-rw-r--r--   0        0        0      915 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/code/base.py
+-rw-r--r--   0        0        0      150 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/code/vasp.py
+-rw-r--r--   0        0        0      882 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/configs/workflow/pmf_cp2k.yml
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/flows/__init__.py
+-rw-r--r--   0        0        0    32933 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/flows/pmf_flow.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/resources/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/resources/config.py
+-rw-r--r--   0        0        0     1446 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/resources/submit.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/runner/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/tasks/defaults/__init__.py
+-rw-r--r--   0        0        0     1795 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/tasks/defaults/pmf.py
+-rw-r--r--   0        0        0    12976 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/tasks/pmf.py
+-rw-r--r--   0        0        0    10450 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/tasks/screen.py
+-rw-r--r--   0        0        0    24938 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/tasker/tasks/tesla.py
+-rw-r--r--   0        0        0       54 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/utils/__init__.py
+-rw-r--r--   0        0        0     1089 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/utils/config.py
+-rw-r--r--   0        0        0     1957 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/utils/constant.py
+-rw-r--r--   0        0        0    13850 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/utils/cp2k.py
+-rw-r--r--   0        0        0      966 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/utils/file.py
+-rw-r--r--   0        0        0     3585 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/utils/lammps.py
+-rw-r--r--   0        0        0     1083 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/utils/log_factory.py
+-rw-r--r--   0        0        0     1283 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/utils/messager.py
+-rw-r--r--   0        0        0       45 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/utils/output.py
+-rw-r--r--   0        0        0     1724 2024-04-11 11:33:09.699316 catflow-0.5.1/catflow/utils/statistics.py
+-rw-r--r--   0        0        0     1234 2024-04-11 11:33:09.715316 catflow-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4762 1970-01-01 00:00:00.000000 catflow-0.5.1/PKG-INFO
```

### Comparing `catflow-0.5.0/LICENSE` & `catflow-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/README.md` & `catflow-0.5.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # CatFlow
 
 > Parts of the code to be open source.
 
-[![Python package](https://github.com/Cloudac7/CatFlow/actions/workflows/ci.yml/badge.svg)](https://github.com/Cloudac7/CatFlow/actions/workflows/ci.yml)
-[![Coverage Status](https://coveralls.io/repos/github/Cloudac7/CatFlow/badge.svg?branch=master)](https://coveralls.io/github/Cloudac7/CatFlow?branch=master)
+[![Python package](https://github.com/chenggroup/catflow/actions/workflows/ci.yml/badge.svg)](https://github.com/chenggroup/catflow/actions/workflows/ci.yml)
+[![codecov](https://codecov.io/gh/chenggroup/catflow/graph/badge.svg?token=NGFDZX7WDO)](https://codecov.io/gh/chenggroup/catflow)
 
 
 Machine learning aided catalysis reaction free energy calculation and post-analysis workflow, thus, analyzer for catalysis.
 
 As is known to all, cat is fluid and thus cat flows. 🐱
 
 > Former Miko-Analyzer and Miko-Tasker
```

### Comparing `catflow-0.5.0/catflow/analyzer/atomic/atomic_energy.py` & `catflow-0.5.1/catflow/analyzer/atomic/atomic_energy.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/atomic/utils.py` & `catflow-0.5.1/catflow/analyzer/atomic/utils.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/graph/plotting.py` & `catflow-0.5.1/catflow/analyzer/graph/plotting.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/metad/fes.py` & `catflow-0.5.1/catflow/analyzer/metad/fes.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,111 +6,180 @@
 from joblib import Parallel, delayed
 from typing import Optional, List, Tuple, Union, Dict, Any
 from itertools import product
 from numpy.typing import ArrayLike
 from matplotlib.colors import Colormap
 
 from catflow.analyzer.metad.hills import Hills
+from catflow.analyzer.metad.colvar import Colvar
 from catflow.analyzer.graph.plotting import canvas_style
 from catflow.utils.config import parse_slice_string
 from catflow.utils.log_factory import logger
 
 dp2_cutoff_a = 1.0/(1.0 - np.exp(-6.25))
 dp2_cutoff_b = - np.exp(-6.25)/(1.0 - np.exp(-6.25))
 
+
 class FreeEnergySurface:
     """
     Computes the free energy surface corresponding to the provided Hills object.
 
     Usage:
     ```python
     from catflow.analyzer.metad.fes import FreeEnergySurface
     fes = FreeEnergySurface(hills)
     ```
 
     Args:
         hills (Hills): The Hills object used for computing the free energy surface.
         resolution (int, optional): \
-            The resolution of the free energy surface. Defaults to 256.
+            The resolution of the free energy surface. Defaults to 128.
         time_min (int): The starting time step of simulation. Defaults to 0.
         time_max (int, optional): The ending time step of simulation. Defaults to None.
     """
 
     fes: np.ndarray
     cvs: int
     cv_min: np.ndarray
     cv_max: np.ndarray
     periodic: np.ndarray
-    resolution: int = 256
+    resolution: int = 128
     hills: Optional[Hills] = None
+    colvar: Optional[Colvar] = None
     cv_fes_range: Optional[np.ndarray] = None
     cv_name: Optional[List[str]] = None
     minima: Optional[pd.DataFrame] = None
 
     def __init__(
         self,
-        resolution: int = 256
+        resolution: int = 128
     ):
         self.res = resolution
 
     @classmethod
     def from_hills(
         cls,
         hills: Hills,
-        resolution: int = 256
+        resolution: int = 128
     ):
         """Generate a FES object from a Hills object."""
         fes = cls(resolution=resolution)
-
         fes.cvs = hills.cvs
-
         fes.hills = hills
         fes.periodic = hills.periodic
         fes.cv_name = hills.cv_name
+        fes.generate_cv_map(typ="hills")
 
-        fes.generate_cv_map()
+        return fes
+
+    @classmethod
+    def from_colvar(
+        cls,
+        colvar: Colvar,
+        cv_name: Union[str, List[str]],
+        periodic: Union[bool, List[bool]] = False,
+        cv_per: Optional[List[List[float]]] = None,
+        resolution: int = 128
+    ):
+        fes = cls(resolution=resolution)
+        if isinstance(cv_name, str):
+            cv_name = [cv_name]
+        fes.cvs = len(cv_name)
+        fes.cv_name = cv_name
+        fes.colvar = colvar
+        fes.cv_min = np.min(colvar.colvars[cv_name].to_numpy(), axis=0)
+        fes.cv_max = np.max(colvar.colvars[cv_name].to_numpy(), axis=0)
+        if isinstance(periodic, bool):
+            fes.periodic = np.array([periodic] * fes.cvs, dtype=bool)
+        else:
+            fes.periodic = np.array(periodic[:fes.cvs], dtype=bool)
+
+        for i in range(fes.cvs):
+            if fes.periodic[i]:
+                if cv_per == None:
+                    raise ValueError(
+                        "cv_per has to be provided for each periodic CV"
+                    )
+                try:
+                    if cv_per[i][0] <= cv_per[i][1]:
+                        fes.cv_min[i] = cv_per[i][0]
+                        fes.cv_max[i] = cv_per[i][1]
+                except IndexError:
+                    raise ValueError(
+                        "cv_per has to be provided for each periodic CV"
+                    )
+
+        fes.generate_cv_map(typ="colvar")
 
         return fes
 
-    def generate_cv_map(self):
+    def generate_cv_map(self, typ="hills"):
         """generate CV map"""
-        if self.hills is not None:
-            cv_min = deepcopy(self.hills.cv_min)
-            cv_max = deepcopy(self.hills.cv_max)
-            cv_range = cv_max - cv_min
-            self.cv_range = cv_range
-
-            cv_min[~self.periodic] -= cv_range[~self.periodic] * 0.15
-            cv_max[~self.periodic] += cv_range[~self.periodic] * 0.15
-            cv_fes_range = np.abs(cv_max - cv_min)
-
-            # generate remapped cv_min and cv_max
-            self.cv_min = cv_min
-            self.cv_max = cv_max
-            self.cv_fes_range = cv_fes_range
+        if typ == "hills":
+            if self.hills is None:
+                raise ValueError("Hills not loaded yet.")
+            else:
+                cv_min = self.hills.cv_min
+                cv_max = self.hills.cv_max
+        elif typ == "colvar":
+            if self.colvar is None:
+                raise ValueError("Colvar not loaded yet.")
+            else:
+                cv_min = self.cv_min
+                cv_max = self.cv_max
+        else:
+            raise ValueError("Invalid type.")
+        cv_range = cv_max - cv_min
+        self.cv_range = cv_range
+
+        cv_min[~self.periodic] -= cv_range[~self.periodic] * 0.15
+        cv_max[~self.periodic] += cv_range[~self.periodic] * 0.15
+        cv_fes_range = np.abs(cv_max - cv_min)
+
+        # generate remapped cv_min and cv_max
+        self.cv_min = cv_min
+        self.cv_max = cv_max
+        self.cv_fes_range = cv_fes_range
 
     @classmethod
     def from_array(
         cls,
         fes_array: ArrayLike,
         cv_min: ArrayLike,
         cv_max: ArrayLike,
         periodic: ArrayLike,
         cv_name: List[str],
-        resolution: int = 256
+        cv_per: Optional[List[List[float]]] = None,
+        resolution: int = 128
     ):
         fes = cls(resolution=resolution)
         fes.fes = np.array(fes_array)
         fes.cv_min = np.array(cv_min)
         fes.cv_max = np.array(cv_max)
         fes.cv_fes_range = np.array(cv_max) - np.array(cv_min)
         fes.periodic = np.array(periodic, dtype=bool)
         fes.cv_name = cv_name
         fes.res = resolution
         fes.cvs = len(cv_name)
+
+        for i in range(fes.cvs):
+            if fes.periodic[i]:
+                if cv_per == None:
+                    raise ValueError(
+                        "cv_per has to be provided for each periodic CV"
+                    )
+                try:
+                    if cv_per[i][0] <= cv_per[i][1]:
+                        fes.cv_min[i] = cv_per[i][0]
+                        fes.cv_max[i] = cv_per[i][1]
+                except IndexError:
+                    raise ValueError(
+                        "cv_per has to be provided for each periodic CV"
+                    )
+
         return fes
 
     def name_cv(self):
         if self.cv_name is None:
             self.cv_name = []
             for i in range(self.cvs):
                 self.cv_name.append(f"CV{i+1}")
@@ -126,15 +195,15 @@
         return_fes: bool = False
     ):
         """Function used internally for summing hills in Hills object with the fast Bias Sum Algorithm. 
         From which could also be quick to get e_beta_c for reweighting.
 
         Args:
             resolution (int, optional): \
-                The resolution of the free energy surface. Defaults to 256.
+                The resolution of the free energy surface. Defaults to 128.
             time_min (int): The starting time step of simulation. Defaults to 0.
             time_max (int, optional): The ending time step of simulation. Defaults to None.
             reweighting (bool, optional): \
                 If True, the function of c(t) will be calculated and stored in `self.e_beta_c`.
                 Defaults to False.
             kb (float, optional): The Boltzmann Constant in the energy unit. Defaults to 8.314e-3.
             temp (float, optional): The temperature of the simulation in Kelvins. Defaults to 300.0.
@@ -261,44 +330,44 @@
         gauss_center = np.array(gauss.shape) // 2
 
         fes = np.zeros([resolution] * cvs)
         d_cv = np.prod(cv_fes_range / resolution)
 
         with h5py.File(filename, "w") as f:
             fes_data = f.create_dataset(
-                "fes_data", 
-                shape=(len(cv_bins[0]), *fes.shape), 
-                dtype=np.float64, 
+                "fes_data",
+                shape=(len(cv_bins[0]), *fes.shape),
+                dtype=np.float64,
                 chunks=(1, *fes.shape)
             )
             for line in trange(len(cv_bins[0])):
                 fes_index_to_edit, delta_fes = \
                     self._sum_bias(
                         gauss_center, gauss, cv_bins, line, cvs, resolution
                     )
                 fes[fes_index_to_edit] += delta_fes
                 correction = np.sum(np.exp(- fes / kb / temp)) * d_cv
                 fes_corrected = fes + kb * temp * np.log(correction)
                 fes_data[line] = fes_corrected
         del fes, d_cv, fes_corrected
 
     def load_fes_with_correction(
-        self, 
+        self,
         filename: str,
         slice_string: Optional[str] = None
     ):
         import h5py
 
         with h5py.File(filename, 'r') as f:
             dataset = f["fes_data"]
             if slice_string:
                 data_slice = parse_slice_string(slice_string)
-                return dataset[data_slice] # type: ignore
+                return dataset[data_slice]  # type: ignore
             else:
-                return dataset[:] # type: ignore
+                return dataset[:]  # type: ignore
 
     def _gauss_kernel(self, gauss_res, sigma_res):
 
         gauss_center = gauss_res // 2
         grids = np.indices(gauss_res)
 
         grids_flatten = grids.reshape(gauss_res.shape[0], -1).T
@@ -388,18 +457,21 @@
 
     def _calculate_dp2(self, index, cv, sigma, cv_min, cv_fes_range):
 
         dp2 = np.zeros(cv.shape[0])
         for cv_idx in range(cv.shape[1]):
             dist_cv = \
                 cv[:, cv_idx] - \
-                (cv_min[cv_idx] + index[cv_idx] * cv_fes_range[cv_idx] / self.res)
+                (cv_min[cv_idx] + index[cv_idx] *
+                 cv_fes_range[cv_idx] / self.res)
             if self.periodic[cv_idx]:
-                dist_cv[dist_cv < -0.5*cv_fes_range[cv_idx]] += cv_fes_range[cv_idx]
-                dist_cv[dist_cv > +0.5*cv_fes_range[cv_idx]] -= cv_fes_range[cv_idx]
+                dist_cv[dist_cv < -0.5*cv_fes_range[cv_idx]
+                        ] += cv_fes_range[cv_idx]
+                dist_cv[dist_cv > +0.5*cv_fes_range[cv_idx]
+                        ] -= cv_fes_range[cv_idx]
             dp2_local = dist_cv ** 2 / \
                 (2 * sigma[:, cv_idx] ** 2)
             dp2 += dp2_local
 
         return dp2
 
     def make_fes_original(
@@ -410,15 +482,15 @@
         n_workers: int = -1
     ):
         """
         Function internally used to sum Hills in the same way as Plumed `sum_hills`. 
 
         Args:
             resolution (int, optional): \
-                The resolution of the free energy surface. Defaults to 256.
+                The resolution of the free energy surface. Defaults to 128.
             time_min (int): The starting time step of simulation. Defaults to 0.
             time_max (int, optional): The ending time step of simulation. Defaults to None.
             n_workers (int, optional): Number of workers for parallelization. Defaults to 2.
         """
         if self.hills is None:
             raise ValueError("Hills not loaded yet.")
 
@@ -462,14 +534,64 @@
         if results is not None:
             for index, value in results:
                 fes[index] = value
             fes -= np.min(fes)
         self.fes = fes
         return fes
 
+    def make_fes_reweighting(
+        self,
+        resolution: int = 128,
+        kb: float = 8.314e-3,
+        temp: float = 300.0,
+        weight_factor: float = 1.0,
+        time_min: Optional[int] = None,
+        time_max: Optional[int] = None,
+        cv_used_names: Optional[List[str]] = None
+    ):
+        from scipy.stats import gaussian_kde
+
+        kbt = kb * temp
+        beta = 1 / kbt
+        if not self.colvar:
+            raise ValueError("Colvar not loaded yet."
+                             "Please use fes.colvar = Colvar(file, bias_name) to load colvar.")
+        bias = self.colvar.colvars[self.colvar.bias_key].to_numpy(dtype=np.float64)[
+            time_min:time_max]
+        if cv_used_names:
+            if len(cv_used_names) > 2:
+                raise ValueError("Only 2 CVs are supported for reweighting.")
+            elif len(cv_used_names) == 1:
+                idx0 = self.cv_name.index(cv_used_names[0]) # type: ignore
+                grid_points = np.linspace(
+                    self.cv_min[idx0], self.cv_max[idx0], resolution) # type: ignore
+            elif len(cv_used_names) == 2:
+                idx0, idx1 = self.cv_name.index( # type: ignore
+                    cv_used_names[0]), self.cv_name.index(cv_used_names[1]) # type: ignore
+                grid_points = np.meshgrid(
+                    np.linspace(self.cv_min[idx0], # type: ignore
+                                self.cv_max[idx0], resolution), # type: ignore
+                    np.linspace(self.cv_min[idx1], # type: ignore
+                                self.cv_max[idx1], resolution) # type: ignore
+                )
+            else:
+                cv_used_names = self.cv_name[:1]  # type: ignore
+        else:
+            cv_used_names = self.cv_name[:1]  # type: ignore
+        cv = self.colvar.colvars[cv_used_names].to_numpy(dtype=np.float64)[time_min:time_max]
+        if len(cv_used_names) == 1:
+            kde = gaussian_kde(cv.flatten(), weights=weight_factor*np.exp(beta*bias))
+        elif len(cv_used_names) == 2:
+            kde = gaussian_kde(cv.T, weights=weight_factor*np.exp(beta*bias))
+        dens = kde.evaluate(grid_points)
+        fes = -kbt * np.log(dens)
+        fes -= np.min(fes)
+        self.fes = fes
+        return fes
+
     def remove_cv(
         self,
         CV: int,
         kb: Optional[float] = None,
         energy_unit: str = "kJ/mol",
         temp: float = 300.0
     ):
@@ -751,15 +873,15 @@
                     xlabel=xlabel, ylabel=ylabel,
                     energy_unit=energy_unit,
                     **surface_params, **kwargs
                 )
             fig, ax = PlottingFES._plot2d(
                 self,
                 levels=levels, cmap=cmap, image_size=image_size, dpi=dpi,
-                xlabel=xlabel, ylabel=ylabel, 
+                xlabel=xlabel, ylabel=ylabel,
                 energy_unit=energy_unit, **kwargs
             )
 
         else:
             raise ValueError("Only 1D and 2D FES are supported.")
 
         if png_name != None:
```

### Comparing `catflow-0.5.0/catflow/analyzer/metad/hills.py` & `catflow-0.5.1/catflow/analyzer/metad/hills.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/metad/profile.py` & `catflow-0.5.1/catflow/analyzer/metad/profile.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/metad/string.py` & `catflow-0.5.1/catflow/analyzer/metad/string.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/structure/cluster.py` & `catflow-0.5.1/catflow/analyzer/structure/cluster.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/structure/coordination_number.py` & `catflow-0.5.1/catflow/analyzer/structure/coordination_number.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/structure/dynamic_selection.py` & `catflow-0.5.1/catflow/analyzer/structure/dynamic_selection.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/structure/lindemann_index.py` & `catflow-0.5.1/catflow/analyzer/structure/lindemann_index.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/exploration.py` & `catflow-0.5.1/catflow/analyzer/tesla/ai2_kit/exploration.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/labeling.py` & `catflow-0.5.1/catflow/analyzer/tesla/ai2_kit/labeling.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/task.py` & `catflow-0.5.1/catflow/analyzer/tesla/ai2_kit/task.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/training.py` & `catflow-0.5.1/catflow/analyzer/tesla/ai2_kit/training.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/tesla/base/exploration.py` & `catflow-0.5.1/catflow/analyzer/tesla/base/exploration.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/tesla/base/labeling.py` & `catflow-0.5.1/catflow/analyzer/tesla/base/labeling.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/tesla/base/task.py` & `catflow-0.5.1/catflow/analyzer/tesla/base/task.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/tesla/base/training.py` & `catflow-0.5.1/catflow/analyzer/tesla/base/training.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/tesla/dpgen/exploration.py` & `catflow-0.5.1/catflow/analyzer/tesla/dpgen/exploration.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/tesla/dpgen/labeling.py` & `catflow-0.5.1/catflow/analyzer/tesla/dpgen/labeling.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/tesla/dpgen/task.py` & `catflow-0.5.1/catflow/analyzer/tesla/dpgen/task.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/analyzer/tesla/dpgen/training.py` & `catflow-0.5.1/catflow/analyzer/tesla/dpgen/training.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/cmdline/base.py` & `catflow-0.5.1/catflow/cmdline/base.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/cmdline/calculation/dpgen.py` & `catflow-0.5.1/catflow/cmdline/calculation/dpgen.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/cmdline/workflow/pmf.py` & `catflow-0.5.1/catflow/cmdline/workflow/pmf.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/cmdline/workflow/tesla.py` & `catflow-0.5.1/catflow/cmdline/workflow/tesla.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/tasker/calculation/dpgen.py` & `catflow-0.5.1/catflow/tasker/calculation/dpgen.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/tasker/calculation/vasp.py` & `catflow-0.5.1/catflow/tasker/calculation/vasp.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/tasker/code/base.py` & `catflow-0.5.1/catflow/tasker/code/base.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/tasker/configs/workflow/pmf_cp2k.yml` & `catflow-0.5.1/catflow/tasker/configs/workflow/pmf_cp2k.yml`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/tasker/flows/pmf_flow.py` & `catflow-0.5.1/catflow/tasker/flows/pmf_flow.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/tasker/resources/submit.py` & `catflow-0.5.1/catflow/tasker/resources/submit.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/tasker/tasks/defaults/pmf.py` & `catflow-0.5.1/catflow/tasker/tasks/defaults/pmf.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/tasker/tasks/pmf.py` & `catflow-0.5.1/catflow/tasker/tasks/pmf.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/tasker/tasks/screen.py` & `catflow-0.5.1/catflow/tasker/tasks/screen.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/tasker/tasks/tesla.py` & `catflow-0.5.1/catflow/tasker/tasks/tesla.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/utils/config.py` & `catflow-0.5.1/catflow/utils/config.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/utils/constant.py` & `catflow-0.5.1/catflow/utils/constant.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/utils/cp2k.py` & `catflow-0.5.1/catflow/utils/cp2k.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/utils/file.py` & `catflow-0.5.1/catflow/utils/file.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/utils/lammps.py` & `catflow-0.5.1/catflow/utils/lammps.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/utils/log_factory.py` & `catflow-0.5.1/catflow/utils/log_factory.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/utils/messager.py` & `catflow-0.5.1/catflow/utils/messager.py`

 * *Files identical despite different names*

### Comparing `catflow-0.5.0/catflow/utils/statistics.py` & `catflow-0.5.1/catflow/utils/statistics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from typing import Tuple
 
 import numpy as np
 from numpy.typing import ArrayLike
 
 
-def block_average(data: ArrayLike, block_size: int, axis: int = 0) -> Tuple[float, float]:
+def block_average(data: ArrayLike, block_size: int, axis: int = 0):
+    reshape_flag = False
     data = np.array(data)
     if data.ndim == 1:
+        reshape_flag = True
         data = np.reshape(data, (-1, 1))  # Reshape data into a 2D array
     N_b = data.shape[axis] // block_size
     if N_b == 0:
         raise ValueError(f"Cannot block average data: block size {block_size} is larger than "
                          f"the size of the array along axis {axis} ({data.shape[axis]})")
     # drop the last block if it is not full
     slices = [slice(None)] * data.ndim
     slices[axis] = slice(0, block_size * N_b)
 
     # reshape data into blocks
     reshaped_data = reshape_array(data[tuple(slices)], N_b, axis)
     blocked_data = np.mean(reshaped_data, axis=axis+1)
     mean = np.mean(blocked_data, axis=axis)
     var = np.std(blocked_data, ddof=1, axis=axis) / np.sqrt(N_b)
+    if reshape_flag:
+        mean = mean[0]
+        var = var[0]
     return mean, var
 
 
 def auto_correlation(data, tau_max):
     mean = np.mean(data)
     var = np.var(data)
     tau_array = np.arange(1, tau_max + 1)
```

### Comparing `catflow-0.5.0/pyproject.toml` & `catflow-0.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 [tool.poetry]
 name = "catflow"
-version = "0.5.0"
+version = "0.5.1"
 description = "Analyzing tool for deep learning based chemical research."
 authors = ["Cloudac7 <scottryuu@outlook.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/chenggroup/CatFlow"
 packages = [{include = "catflow"}]
 
 [tool.poetry.dependencies]
-python = "<3.12,>=3.8"
+python = "^3.9"
 ase = "^3.21.1"
 click = "*"
 dpdata = "*"
 dpdispatcher = "^0.5.6"
 dpgen = "^0.11.1"
 dynaconf = "*"
 matplotlib = "^3.7.1"
-numpy = "<1.24,>=1.18"
+numpy = "^1.24"
 pandas = "^1.3.3"
 dscribe = "^1.2.2"
 mdanalysis = "^2.2"
-scipy = "^1.10.1"
+scipy = "^1.10"
 seaborn = "^0.12.2"
 pymatgen = "^2023.5.10"
 ai2-kit = ">=0.9.0"
 fire = "^0.5.0"
 ruamel-yaml = ">=0.17.21,<0.18.0"
 h5py = "^3.10.0"
 
 [tool.poetry.group.test.dependencies]
 flake8 = "*"
 pytest = "*"
 pytest-mock = "*"
 pytest-datadir = "*"
+pytest-asyncio = "*"
 coverage = "*"
 coveralls = "*"
 
 [tool.poetry.group.docs.dependencies]
 mkdocstrings = { version = ">=0.18", extras = ["python"] }
 mkdocs-material = "*"
 mike = "*"
```

### Comparing `catflow-0.5.0/PKG-INFO` & `catflow-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
 Name: catflow
-Version: 0.5.0
+Version: 0.5.1
 Summary: Analyzing tool for deep learning based chemical research.
 Home-page: https://github.com/chenggroup/CatFlow
 License: Apache-2.0
 Author: Cloudac7
 Author-email: scottryuu@outlook.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ai2-kit (>=0.9.0)
 Requires-Dist: ase (>=3.21.1,<4.0.0)
 Requires-Dist: click
 Requires-Dist: dpdata
 Requires-Dist: dpdispatcher (>=0.5.6,<0.6.0)
 Requires-Dist: dpgen (>=0.11.1,<0.12.0)
 Requires-Dist: dscribe (>=1.2.2,<2.0.0)
 Requires-Dist: dynaconf
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: h5py (>=3.10.0,<4.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: mdanalysis (>=2.2,<3.0)
-Requires-Dist: numpy (>=1.18,<1.24)
+Requires-Dist: numpy (>=1.24,<2.0)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
 Requires-Dist: pymatgen (>=2023.5.10,<2024.0.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
-Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Requires-Dist: scipy (>=1.10,<2.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Project-URL: Repository, https://github.com/chenggroup/CatFlow
 Description-Content-Type: text/markdown
 
 # CatFlow
 
 > Parts of the code to be open source.
 
-[![Python package](https://github.com/Cloudac7/CatFlow/actions/workflows/ci.yml/badge.svg)](https://github.com/Cloudac7/CatFlow/actions/workflows/ci.yml)
-[![Coverage Status](https://coveralls.io/repos/github/Cloudac7/CatFlow/badge.svg?branch=master)](https://coveralls.io/github/Cloudac7/CatFlow?branch=master)
+[![Python package](https://github.com/chenggroup/catflow/actions/workflows/ci.yml/badge.svg)](https://github.com/chenggroup/catflow/actions/workflows/ci.yml)
+[![codecov](https://codecov.io/gh/chenggroup/catflow/graph/badge.svg?token=NGFDZX7WDO)](https://codecov.io/gh/chenggroup/catflow)
 
 
 Machine learning aided catalysis reaction free energy calculation and post-analysis workflow, thus, analyzer for catalysis.
 
 As is known to all, cat is fluid and thus cat flows. 🐱
 
 > Former Miko-Analyzer and Miko-Tasker
```

