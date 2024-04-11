# Comparing `tmp/pyiron_continuum-0.0.8.tar.gz` & `tmp/pyiron_continuum-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_continuum-0.0.8.tar", last modified: Fri Dec  1 12:20:26 2023, max compression
+gzip compressed data, was "pyiron_continuum-0.0.9.tar", last modified: Thu Apr 11 07:09:04 2024, max compression
```

## Comparing `pyiron_continuum-0.0.8.tar` & `pyiron_continuum-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 12:20:26.350478 pyiron_continuum-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-12-01 12:20:26.350478 pyiron_continuum-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 12:20:26.346478 pyiron_continuum-0.0.8/pyiron_continuum/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-12-01 12:20:26.354478 pyiron_continuum-0.0.8/pyiron_continuum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 12:20:26.350478 pyiron_continuum-0.0.8/pyiron_continuum/damask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/damask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/damask/damaskjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     9579 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/damask/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 12:20:26.350478 pyiron_continuum-0.0.8/pyiron_continuum/elasticity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/elasticity/eschelby.py
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/elasticity/green.py
--rw-r--r--   0 runner    (1001) docker     (127)    21026 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/elasticity/linear_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/elasticity/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 12:20:26.350478 pyiron_continuum-0.0.8/pyiron_continuum/fenics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/fenics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/fenics/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/fenics/fix_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 12:20:26.350478 pyiron_continuum-0.0.8/pyiron_continuum/fenics/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/fenics/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/fenics/job/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)    15845 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/fenics/job/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/fenics/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    18389 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 12:20:26.350478 pyiron_continuum-0.0.8/pyiron_continuum/schroedinger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/schroedinger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/schroedinger/potentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/schroedinger/schroedinger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/pyiron_continuum/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 12:20:26.350478 pyiron_continuum-0.0.8/pyiron_continuum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-12-01 12:20:26.000000 pyiron_continuum-0.0.8/pyiron_continuum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-12-01 12:20:26.000000 pyiron_continuum-0.0.8/pyiron_continuum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-01 12:20:26.000000 pyiron_continuum-0.0.8/pyiron_continuum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-12-01 12:20:26.000000 pyiron_continuum-0.0.8/pyiron_continuum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-01 12:20:26.000000 pyiron_continuum-0.0.8/pyiron_continuum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-12-01 12:20:26.350478 pyiron_continuum-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-12-01 12:20:26.000000 pyiron_continuum-0.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2023-12-01 12:20:23.000000 pyiron_continuum-0.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:09:04.735947 pyiron_continuum-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-11 07:09:04.735947 pyiron_continuum-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:09:04.727947 pyiron_continuum-0.0.9/pyiron_continuum/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-11 07:09:04.735947 pyiron_continuum-0.0.9/pyiron_continuum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:09:04.731947 pyiron_continuum-0.0.9/pyiron_continuum/damask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/damask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/damask/damaskjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/damask/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/damask/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23550 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/damask/rolling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:09:04.731947 pyiron_continuum-0.0.9/pyiron_continuum/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/elasticity/eschelby.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/elasticity/green.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21026 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/elasticity/linear_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/elasticity/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:09:04.731947 pyiron_continuum-0.0.9/pyiron_continuum/fenics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/fenics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/fenics/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/fenics/fix_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:09:04.731947 pyiron_continuum-0.0.9/pyiron_continuum/fenics/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/fenics/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/fenics/job/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15845 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/fenics/job/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/fenics/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18389 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:09:04.731947 pyiron_continuum-0.0.9/pyiron_continuum/schroedinger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/schroedinger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/schroedinger/potentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/schroedinger/schroedinger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/pyiron_continuum/toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:09:04.731947 pyiron_continuum-0.0.9/pyiron_continuum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-11 07:09:04.000000 pyiron_continuum-0.0.9/pyiron_continuum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-11 07:09:04.000000 pyiron_continuum-0.0.9/pyiron_continuum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:09:04.000000 pyiron_continuum-0.0.9/pyiron_continuum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-11 07:09:04.000000 pyiron_continuum-0.0.9/pyiron_continuum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 07:09:04.000000 pyiron_continuum-0.0.9/pyiron_continuum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-11 07:09:04.735947 pyiron_continuum-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-11 07:09:04.000000 pyiron_continuum-0.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-11 07:09:02.000000 pyiron_continuum-0.0.9/versioneer.py
```

### Comparing `pyiron_continuum-0.0.8/LICENSE` & `pyiron_continuum-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/PKG-INFO` & `pyiron_continuum-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_continuum
-Version: 0.0.8
+Version: 0.0.9
 Summary: Repository for user-generated plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_continuum
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: huber@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
@@ -14,18 +14,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
-Requires-Dist: matplotlib>=3.8.2
-Requires-Dist: numpy>=1.26.2
-Requires-Dist: pyiron_base>=0.6.9
-Requires-Dist: scipy>=1.11.4
+Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: pyiron_base>=0.7.11
+Requires-Dist: scipy>=1.12.0
 Requires-Dist: sympy>=1.12
 Provides-Extra: fenics
 Requires-Dist: fenics>=2019.1.0; extra == "fenics"
 Requires-Dist: mshr>=2019.1.0; extra == "fenics"
 Provides-Extra: schroedinger
 Requires-Dist: k3d>=2.16.0; extra == "schroedinger"
```

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/__init__.py` & `pyiron_continuum-0.0.9/pyiron_continuum/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,13 +11,14 @@
 from pyiron_continuum.toolkit import ContinuumTools
 ProjectBase.register_tools('continuum', ContinuumTools)
 
 # Make classes available for new pyiron version
 JOB_CLASS_DICT['Fenics'] = 'pyiron_continuum.fenics.job.generic'
 JOB_CLASS_DICT['FenicsLinearElastic'] = 'pyiron_continuum.fenics.job.elastic'
 JOB_CLASS_DICT['DAMASK'] = 'pyiron_continuum.damask.damaskjob'
+JOB_CLASS_DICT['ROLLING'] = 'pyiron_continuum.damask.rolling'
 JOB_CLASS_DICT['TISE'] = 'pyiron_continuum.schroedinger.schroedinger'
 
 from ._version import get_versions
 
 __version__ = get_versions()["version"]
 del get_versions
```

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/damask/damaskjob.py` & `pyiron_continuum-0.0.9/pyiron_continuum/damask/damaskjob.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 DAMASK job, which runs a damask simulation, and create the necessary inputs
 """
 
 from pyiron_base import TemplateJob, ImportAlarm
+
 with ImportAlarm(
         'DAMASK functionality requires the `damask` module (and its dependencies) specified as extra'
         'requirements. Please install it and try again.'
 ) as damask_alarm:
-    from damask import Result
+    from damask import Result as ResultDamask
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 
-
 __author__ = "Muhammad Hassani"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Muhammad Hassani"
 __email__ = "hassani@mpie.de"
 __status__ = "development"
 __date__ = "Oct 04, 2021"
 
 
+class Result(ResultDamask):
+    def average_spatio_temporal_tensors(self, name):
+        return np.average(list(self.get(name).values()), axis=1)
+
+
 class DAMASK(TemplateJob):
     def __init__(self, project, job_name):
         """
         The damask job
         Args:
             project(pyiron.project): a pyiron project
             job_name(str): the name of the job
         """
         super(DAMASK, self).__init__(project, job_name)
-        self._damask_hdf = os.path.join(self.working_directory, "damask_loading_material.hdf5")
         self._material = None
         self._loading = None
         self._grid = None
         self._results = None
         self._executable_activate()
 
     @property
@@ -93,54 +97,33 @@
 
     def _load_results(self, file_name="damask_loading_material.hdf5"):
         """
             loads the results from damask hdf file
             Args:
                 file_name(str): path to the hdf file
         """
-        if self._results is None:
-            if file_name != "damask_loading_material.hdf5":
-                self._damask_hdf = os.path.join(self.working_directory, file_name)
+        damask_hdf = os.path.join(self.working_directory, file_name)
 
-        self._results = Result(self._damask_hdf)
+        self._results = Result(damask_hdf)
         self._results.add_stress_Cauchy()
         self._results.add_strain()
         self._results.add_equivalent_Mises('sigma')
         self._results.add_equivalent_Mises('epsilon_V^0.0(F)')
-        self.output.stress = self.average_spatio_temporal_tensors('sigma')
-        self.output.strain = self.average_spatio_temporal_tensors('epsilon_V^0.0(F)')
-        self.output.stress_von_Mises = self.average_spatio_temporal_tensors('sigma_vM')
-        self.output.strain_von_Mises = self.average_spatio_temporal_tensors('epsilon_V^0.0(F)_vM')
-    
+        self.output.stress = self._results.average_spatio_temporal_tensors('sigma')
+        self.output.strain = self._results.average_spatio_temporal_tensors('epsilon_V^0.0(F)')
+        self.output.stress_von_Mises = self._results.average_spatio_temporal_tensors('sigma_vM')
+        self.output.strain_von_Mises = self._results.average_spatio_temporal_tensors('epsilon_V^0.0(F)_vM')
+
     def writeresults2vtk(self):
         """
             save results to vtk files
         """
-        cwd = os.getcwd() # get the current dir
-        os.chdir(self.working_directory) # cd into the working dir
-        result=self._results
-        result.export_VTK()
-        os.chdir(cwd) # cd back to the notebook dir
-
-    def temporal_spatial_shape(self, name):
-        property_dict = self._results.get(name)
-        shape_list = [len(property_dict)]
-        for shape in property_dict[list(property_dict.keys())[0]].shape:
-            shape_list.append(shape)
-        return tuple(shape_list)
-
-    def average_spatio_temporal_tensors(self, name):
-        _shape = self.temporal_spatial_shape(name)
-        temporal_spatial_array = np.empty(_shape)
-        property_dict = self._results.get(name)
-        i = 0
-        for key in property_dict.keys():
-            temporal_spatial_array[i] = property_dict[key]
-            i = i + 1
-        return  np.average(temporal_spatial_array, axis=1)
+        if self._results is None:
+            raise ValueError("Results not loaded; call collect_output")
+        self._results.export_VTK(target_dir=self.working_directory)
 
     @staticmethod
     def list_solvers():
         """
         lists the solvers for a damask job
         """
         return [{'mechanical': 'spectral_basic'},
@@ -160,15 +143,15 @@
                 raise ValueError("It is not allowed that component is specified and von_mises is also True ")
             if len(component) != 2:
                 ValueError("The length of direction must be 2, like 'xx', 'xy', ... ")
             if component[0] != 'x' or component[0] != 'y' or component[0] != 'z':
                 ValueError("The direction should be from x, y, and z")
             if component[1] != 'x' or component[1] != 'y' or component[1] != 'z':
                 ValueError("The direction should be from x, y, and z")
-            _component_dict={'x': 0, 'y': 1, 'z': 2}
+            _component_dict = {'x': 0, 'y': 1, 'z': 2}
             _zero_axis = int(_component_dict[component[0]])
             _first_axis = int(_component_dict[component[1]])
             ax.plot(self.output.strain[:, _zero_axis, _first_axis],
                     self.output.stress[:, _zero_axis, _first_axis],
                     linestyle='-', linewidth='2.5')
             ax.grid(True)
             ax.set_xlabel(rf'$\varepsilon_{component[0]}$' + rf'$_{component[1]}$', fontsize=18)
@@ -179,8 +162,7 @@
             ax.grid(True)
             ax.set_xlabel(r'$\varepsilon_{vM}$', fontsize=18)
             ax.set_ylabel(r'$\sigma_{vM}$ (Pa)', fontsize=18)
         else:
             raise ValueError("either direction should be passed in "
                              "or vonMises should be set to True")
         return fig, ax
-
```

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/damask/factory.py` & `pyiron_continuum-0.0.9/pyiron_continuum/damask/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """Factory of the damask classes and methods to a pyironized manner"""
 
 from pyiron_base import ImportAlarm
+
 with ImportAlarm(
         'DAMASK functionality requires the `damask` module (and its dependencies) specified as extra'
         'requirements. Please install it and try again.'
 ) as damask_alarm:
-    from damask import Grid, Config, ConfigMaterial, seeds
+    from damask import GeomGrid, YAML, ConfigMaterial, seeds
 import numpy as np
 
 __author__ = "Muhammad Hassani"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Muhammad Hassani"
 __email__ = "hassani@mpie.de"
 __status__ = "development"
 __date__ = "Oct 04, 2021"
 
-#TODO: reimplement export_vtk() here. Currently, damask dumps vtk files in the cwd
+
+# TODO: reimplement export_vtk() here. Currently, damask dumps vtk files in the cwd
 
 
 class MaterialFactory:
     def __init__(self):
         """A factory for damask ConfigMaterial class."""
         pass
 
@@ -43,50 +45,50 @@
     @staticmethod
     def write(file_path):
         ConfigMaterial.save(fname=file_path)
 
 
 class GridFactory:
     def __init__(self):
-        """A factory for damask._grid.Grid class."""
+        """A factory for damask._grid.GeomGrid class."""
         self._origin = None
 
     @staticmethod
     def read(file_path):
-        return Grid.load(fname=file_path)
+        return GeomGrid.load(fname=file_path)
 
     @property
     def origin(self):
         """
-        Returns damask._grid.Grid, it can be used to call damask original methods.
+        Returns damask._grid.GeomGrid, it can be used to call damask original methods.
         For example:
         origin.from_Voronoi_tessellation(...)
         """
         if self._origin is None:
-            return Grid(material=np.ones((1, 1, 1)), size=[1., 1., 1.])
+            return GeomGrid(material=np.ones((1, 1, 1)), size=[1., 1., 1.])
         else:
             return self._origin
 
     @origin.setter
     def origin(self, value):
         self._origin = value
 
     @staticmethod
-    def via_voronoi_tessellation(grid_dim, num_grains, box_size):
-        if isinstance(grid_dim, int) or isinstance(grid_dim, float):
-            grid_dim = np.array([grid_dim, grid_dim, grid_dim])
+    def via_voronoi_tessellation(spatial_discretization, num_grains, box_size):
+        if isinstance(spatial_discretization, int) or isinstance(spatial_discretization, float):
+            spatial_discretization = np.array([spatial_discretization, spatial_discretization, spatial_discretization])
         if isinstance(box_size, int) or isinstance(box_size, float):
             box_size = np.array([box_size, box_size, box_size])
         seed = seeds.from_random(box_size, num_grains)
-        return Grid.from_Voronoi_tessellation(grid_dim, box_size, seed)
+        return GeomGrid.from_Voronoi_tessellation(spatial_discretization, box_size, seed)
 
 
 class DamaskLoading(dict):
     def __init__(self, solver, load_steps):
-        """A factory for damask Loading class, which is a damask._config.Config object."""
+        """A factory for damask Loading class, which is a damask._config.YAML object."""
         super(DamaskLoading, self).__init__(self)
 
     def __new__(cls, solver, load_steps):
         loading_dict = dict()
         loading_dict["solver"] = solver
         if isinstance(load_steps, list):
             loading_dict["loadstep"] = [
@@ -96,15 +98,16 @@
                 for load_step in load_steps]
         else:
             loading_dict["loadstep"] = [
                 LoadStep(mech_bc_dict=load_steps['mech_bc_dict'],
                          discretization=load_steps['discretization'],
                          additional_parameters_dict=load_steps["additional"])
             ]
-        return Config(solver=loading_dict["solver"], loadstep=loading_dict["loadstep"])
+        return YAML(solver=loading_dict["solver"], loadstep=loading_dict["loadstep"])
+
 
 class LoadStep(dict):
     def __init__(self, mech_bc_dict, discretization, additional_parameters_dict=None):
         """An auxilary class, which helps to parse loadsteps to a dictionary."""
         super(LoadStep, self).__init__(self)
         self.update({'boundary_conditions': {'mechanical': {}},
                      'discretization': discretization})
@@ -194,21 +197,21 @@
                                     h_sl_sl=[1, 1, 1.4, 1.4, 1.4, 1.4],
                                     n_sl=20, output=['xi_sl'],
                                     type='phenopowerlaw', xi_0_sl=[31e6],
                                     xi_inf_sl=[63e6])
         """
         if plasticity == None:
             return {composition: {'lattice': lattice,
-                              'mechanical': {'output': output_list,
-                                             'elastic': elasticity}}}
+                                  'mechanical': {'output': output_list,
+                                                 'elastic': elasticity}}}
         else:
             return {composition: {'lattice': lattice,
-                              'mechanical': {'output': output_list,
-                                             'elastic': elasticity,
-                                             'plasticity': plasticity}}}
+                                  'mechanical': {'output': output_list,
+                                                 'elastic': elasticity,
+                                                 'plastic': plasticity}}}
 
     @staticmethod
     def elasticity(**kwargs):
         """
         Returns a dictionary of elasticity parameters for damask input file.
         Examples:
              elasticity= elasticity(type= 'Hooke', C_11= 106.75e9,
@@ -225,14 +228,30 @@
                                     atol_xi=1.0, dot_gamma_0_sl=0.001,
                                     h_0_sl_sl=75e6,
                                     h_sl_sl=[1, 1, 1.4, 1.4, 1.4, 1.4],
                                     n_sl=20, output=['xi_sl'],
                                     type='phenopowerlaw', xi_0_sl=[31e6],
                                     xi_inf_sl=[63e6])
         """
+        has_h0 = False
+        has_h = False
+        vals = {}
+        for key, value in kwargs.items():
+            if 'h_0_sl_sl' in key:
+                has_h0 = True
+                vals['h_0_sl-sl'] = value
+            if 'h_sl_sl' in key:
+                has_h = True
+                vals['h_sl-sl'] = value
+        if has_h0:
+            kwargs['h_0_sl-sl'] = vals['h_0_sl-sl']
+            del kwargs['h_0_sl_sl']
+        if has_h:
+            kwargs['h_sl-sl'] = vals['h_sl-sl']
+            del kwargs['h_sl_sl']
         return kwargs
 
     @staticmethod
     def rotation(method, *args):
         """
         Returns a damask.Rotation object by a given method.
         Args:
```

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/elasticity/eschelby.py` & `pyiron_continuum-0.0.9/pyiron_continuum/elasticity/eschelby.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/elasticity/green.py` & `pyiron_continuum-0.0.9/pyiron_continuum/elasticity/green.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/elasticity/linear_elasticity.py` & `pyiron_continuum-0.0.9/pyiron_continuum/elasticity/linear_elasticity.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/elasticity/tools.py` & `pyiron_continuum-0.0.9/pyiron_continuum/elasticity/tools.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/fenics/factory.py` & `pyiron_continuum-0.0.9/pyiron_continuum/fenics/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/fenics/fix_plotting.py` & `pyiron_continuum-0.0.9/pyiron_continuum/fenics/fix_plotting.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/fenics/job/elastic.py` & `pyiron_continuum-0.0.9/pyiron_continuum/fenics/job/elastic.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/fenics/job/generic.py` & `pyiron_continuum-0.0.9/pyiron_continuum/fenics/job/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/fenics/plot.py` & `pyiron_continuum-0.0.9/pyiron_continuum/fenics/plot.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/mesh.py` & `pyiron_continuum-0.0.9/pyiron_continuum/mesh.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/project.py` & `pyiron_continuum-0.0.9/pyiron_continuum/project.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/schroedinger/potentials.py` & `pyiron_continuum-0.0.9/pyiron_continuum/schroedinger/potentials.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/schroedinger/schroedinger.py` & `pyiron_continuum-0.0.9/pyiron_continuum/schroedinger/schroedinger.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum/toolkit.py` & `pyiron_continuum-0.0.9/pyiron_continuum/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum.egg-info/PKG-INFO` & `pyiron_continuum-0.0.9/pyiron_continuum.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyiron-continuum
-Version: 0.0.8
+Name: pyiron_continuum
+Version: 0.0.9
 Summary: Repository for user-generated plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_continuum
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: huber@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
@@ -14,18 +14,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
-Requires-Dist: matplotlib>=3.8.2
-Requires-Dist: numpy>=1.26.2
-Requires-Dist: pyiron_base>=0.6.9
-Requires-Dist: scipy>=1.11.4
+Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: pyiron_base>=0.7.11
+Requires-Dist: scipy>=1.12.0
 Requires-Dist: sympy>=1.12
 Provides-Extra: fenics
 Requires-Dist: fenics>=2019.1.0; extra == "fenics"
 Requires-Dist: mshr>=2019.1.0; extra == "fenics"
 Provides-Extra: schroedinger
 Requires-Dist: k3d>=2.16.0; extra == "schroedinger"
```

### Comparing `pyiron_continuum-0.0.8/pyiron_continuum.egg-info/SOURCES.txt` & `pyiron_continuum-0.0.9/pyiron_continuum.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 pyiron_continuum.egg-info/SOURCES.txt
 pyiron_continuum.egg-info/dependency_links.txt
 pyiron_continuum.egg-info/requires.txt
 pyiron_continuum.egg-info/top_level.txt
 pyiron_continuum/damask/__init__.py
 pyiron_continuum/damask/damaskjob.py
 pyiron_continuum/damask/factory.py
+pyiron_continuum/damask/regrid.py
+pyiron_continuum/damask/rolling.py
 pyiron_continuum/elasticity/__init__.py
 pyiron_continuum/elasticity/eschelby.py
 pyiron_continuum/elasticity/green.py
 pyiron_continuum/elasticity/linear_elasticity.py
 pyiron_continuum/elasticity/tools.py
 pyiron_continuum/fenics/__init__.py
 pyiron_continuum/fenics/factory.py
```

### Comparing `pyiron_continuum-0.0.8/setup.py` & `pyiron_continuum-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11'
     ],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[
-        'matplotlib>=3.8.2',
-        'numpy>=1.26.2',
-        'pyiron_base>=0.6.9',
-        'scipy>=1.11.4',
+        'matplotlib>=3.8.3',
+        'numpy>=1.26.4',
+        'pyiron_base>=0.7.11',
+        'scipy>=1.12.0',
         'sympy>=1.12'
     ],
     extras_require={
         'fenics': [
             'fenics>=2019.1.0',
             'mshr>=2019.1.0',
         ],
```

### Comparing `pyiron_continuum-0.0.8/versioneer.py` & `pyiron_continuum-0.0.9/versioneer.py`

 * *Files identical despite different names*

