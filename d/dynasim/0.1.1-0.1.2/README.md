# Comparing `tmp/dynasim-0.1.1.tar.gz` & `tmp/dynasim-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynasim-0.1.1.tar", last modified: Wed Feb 14 15:12:12 2024, max compression
+gzip compressed data, was "dynasim-0.1.2.tar", last modified: Thu Apr 11 08:33:48 2024, max compression
```

## Comparing `dynasim-0.1.1.tar` & `dynasim-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-02-14 15:12:12.841234 dynasim-0.1.1/
--rw-------   0 marcus     (501) staff       (20)     1067 2024-02-14 13:34:54.000000 dynasim-0.1.1/LICENSE
--rw-r--r--   0 marcus     (501) staff       (20)     4427 2024-02-14 15:12:12.840588 dynasim-0.1.1/PKG-INFO
--rw-------   0 marcus     (501) staff       (20)     3946 2024-02-14 15:10:12.000000 dynasim-0.1.1/README.md
--rw-------   0 marcus     (501) staff       (20)      553 2024-02-14 15:11:58.000000 dynasim-0.1.1/pyproject.toml
--rw-r--r--   0 marcus     (501) staff       (20)       38 2024-02-14 15:12:12.841345 dynasim-0.1.1/setup.cfg
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-02-14 15:12:12.814510 dynasim-0.1.1/src/
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-02-14 15:12:12.835351 dynasim-0.1.1/src/dynasim/
--rw-------   0 marcus     (501) staff       (20)      197 2024-02-12 08:50:38.000000 dynasim-0.1.1/src/dynasim/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)     2477 2024-02-12 08:50:38.000000 dynasim-0.1.1/src/dynasim/actuators.py
--rw-r--r--   0 marcus     (501) staff       (20)     3831 2024-02-14 14:28:03.000000 dynasim-0.1.1/src/dynasim/base.py
--rw-------   0 marcus     (501) staff       (20)     2962 2024-02-14 15:09:07.000000 dynasim-0.1.1/src/dynasim/nonlinearities.py
--rw-r--r--   0 marcus     (501) staff       (20)     2456 2024-02-12 08:50:38.000000 dynasim-0.1.1/src/dynasim/simulators.py
--rw-------   0 marcus     (501) staff       (20)     8365 2024-02-14 14:48:48.000000 dynasim-0.1.1/src/dynasim/systems.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-02-14 15:12:12.839924 dynasim-0.1.1/src/dynasim.egg-info/
--rw-r--r--   0 marcus     (501) staff       (20)     4427 2024-02-14 15:12:12.000000 dynasim-0.1.1/src/dynasim.egg-info/PKG-INFO
--rw-r--r--   0 marcus     (501) staff       (20)      354 2024-02-14 15:12:12.000000 dynasim-0.1.1/src/dynasim.egg-info/SOURCES.txt
--rw-r--r--   0 marcus     (501) staff       (20)        1 2024-02-14 15:12:12.000000 dynasim-0.1.1/src/dynasim.egg-info/dependency_links.txt
--rw-r--r--   0 marcus     (501) staff       (20)       12 2024-02-14 15:12:12.000000 dynasim-0.1.1/src/dynasim.egg-info/requires.txt
--rw-r--r--   0 marcus     (501) staff       (20)        8 2024-02-14 15:12:12.000000 dynasim-0.1.1/src/dynasim.egg-info/top_level.txt
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-04-11 08:33:48.406197 dynasim-0.1.2/
+-rw-------   0 marcus     (501) staff       (20)     1067 2024-02-14 13:34:54.000000 dynasim-0.1.2/LICENSE
+-rw-r--r--   0 marcus     (501) staff       (20)     4475 2024-04-11 08:33:48.405913 dynasim-0.1.2/PKG-INFO
+-rw-r--r--   0 marcus     (501) staff       (20)     3995 2024-04-11 07:57:51.000000 dynasim-0.1.2/README.md
+-rw-------   0 marcus     (501) staff       (20)      553 2024-04-11 08:01:29.000000 dynasim-0.1.2/pyproject.toml
+-rw-r--r--   0 marcus     (501) staff       (20)       38 2024-04-11 08:33:48.406251 dynasim-0.1.2/setup.cfg
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-04-11 08:33:48.401083 dynasim-0.1.2/src/
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-04-11 08:33:48.404512 dynasim-0.1.2/src/dynasim/
+-rw-------   0 marcus     (501) staff       (20)      197 2024-02-12 08:50:38.000000 dynasim-0.1.2/src/dynasim/__init__.py
+-rw-r--r--   0 marcus     (501) staff       (20)     3462 2024-04-11 07:55:38.000000 dynasim-0.1.2/src/dynasim/actuators.py
+-rw-r--r--   0 marcus     (501) staff       (20)     3831 2024-02-14 14:28:03.000000 dynasim-0.1.2/src/dynasim/base.py
+-rw-------   0 marcus     (501) staff       (20)     2962 2024-02-14 15:09:07.000000 dynasim-0.1.2/src/dynasim/nonlinearities.py
+-rw-r--r--   0 marcus     (501) staff       (20)     2456 2024-02-12 08:50:38.000000 dynasim-0.1.2/src/dynasim/simulators.py
+-rw-------   0 marcus     (501) staff       (20)     8365 2024-02-14 14:48:48.000000 dynasim-0.1.2/src/dynasim/systems.py
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-04-11 08:33:48.405660 dynasim-0.1.2/src/dynasim.egg-info/
+-rw-r--r--   0 marcus     (501) staff       (20)     4475 2024-04-11 08:33:48.000000 dynasim-0.1.2/src/dynasim.egg-info/PKG-INFO
+-rw-r--r--   0 marcus     (501) staff       (20)      354 2024-04-11 08:33:48.000000 dynasim-0.1.2/src/dynasim.egg-info/SOURCES.txt
+-rw-r--r--   0 marcus     (501) staff       (20)        1 2024-04-11 08:33:48.000000 dynasim-0.1.2/src/dynasim.egg-info/dependency_links.txt
+-rw-r--r--   0 marcus     (501) staff       (20)       12 2024-04-11 08:33:48.000000 dynasim-0.1.2/src/dynasim.egg-info/requires.txt
+-rw-r--r--   0 marcus     (501) staff       (20)        8 2024-04-11 08:33:48.000000 dynasim-0.1.2/src/dynasim.egg-info/top_level.txt
```

### Comparing `dynasim-0.1.1/LICENSE` & `dynasim-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynasim-0.1.1/PKG-INFO` & `dynasim-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynasim
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dynamic System Simulators
 Author-email: Marcus Haywood-Alexander <mhaywood@ethz.ch>
 Project-URL: Homepage, https://github.com/MarcusHA94/dynasim
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -18,30 +18,30 @@
 <!--- These are examples. See https://shields.io for others or to customize this set of shields. You might want to include dependencies, project status and licence info here --->
 ![GitHub repo size](https://img.shields.io/github/repo-size/MarcusHA94/dynasim)
 ![GitHub contributors](https://img.shields.io/github/contributors/MarcusHA94/dynasim)
 
 <!-- Project name is a `<utility/tool/feature>` that allows `<insert_target_audience>` to do `<action/task_it_does>`. -->
 
 The dynasim package simulates dynamic systems in the form:
-$$
+```math
 \mathbf{M}\ddot{\mathbf{x}} + \mathbf{C}\dot{\mathbf{x}} + \mathbf{K}\mathbf{x} + \mathbf{C}_n g_c(\mathbf{x}, \dot{\mathbf{x}}) + \mathbf{K}_n g_k(\mathbf{x}, \dot{\mathbf{x}}) = \mathbf{f}
-$$
+```
 where $\mathbf{\Xi}_n g_{\bullet}(\mathbf{x},\dot{\mathbf{x}})$ represents the nonlinear system forces. For example, a 3DOF Duffing oscillator, connected at one end, would have representative nonlinear forces,
-$$
+```math
 \mathbf{K}_n g_n(\mathbf{x}) = \begin{bmatrix}
     k_{n,1} & - k_{n,2} & 0 \\
     0 & k_{n,2} & -k_{n,3} \\
     0 & 0 & k_{n,3}
 \end{bmatrix}
 \begin{bmatrix}
     x_1^3 \\
     (x_2-x_1)^3 \\
     (x_3 - x_2)^3
 \end{bmatrix}
-$$
+```
 
 ## Installing DynaSim
 
 To install SynaSim, follow these steps:
 
 Linux and macOS:
 ```
@@ -112,14 +112,15 @@
 
 The forcing for the system should be a list of actuations, equal in length to the number of DOFs of the system, there many actuation types,
 ```
 dynasim.actuators.sinusoid(...)
 dynasim.actuators.white_gaussian(...)
 dynasim.actuators.sine_sweep(...)
 dynasim.actuators.rand_phase_ms(...)
+dynasim.actuators.banded_noise(...)
 ```
 
 ### Totally custom system
 
 One can generate a custom system by instantiating an MDOF system with corresponding modal matrices, but the nonlinearity must also be instantiated and 
 ```
 dynasim.base.mdof_system(M, C, K, Cn, Kn)
```

### Comparing `dynasim-0.1.1/README.md` & `dynasim-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 <!--- These are examples. See https://shields.io for others or to customize this set of shields. You might want to include dependencies, project status and licence info here --->
 ![GitHub repo size](https://img.shields.io/github/repo-size/MarcusHA94/dynasim)
 ![GitHub contributors](https://img.shields.io/github/contributors/MarcusHA94/dynasim)
 
 <!-- Project name is a `<utility/tool/feature>` that allows `<insert_target_audience>` to do `<action/task_it_does>`. -->
 
 The dynasim package simulates dynamic systems in the form:
-$$
+```math
 \mathbf{M}\ddot{\mathbf{x}} + \mathbf{C}\dot{\mathbf{x}} + \mathbf{K}\mathbf{x} + \mathbf{C}_n g_c(\mathbf{x}, \dot{\mathbf{x}}) + \mathbf{K}_n g_k(\mathbf{x}, \dot{\mathbf{x}}) = \mathbf{f}
-$$
+```
 where $\mathbf{\Xi}_n g_{\bullet}(\mathbf{x},\dot{\mathbf{x}})$ represents the nonlinear system forces. For example, a 3DOF Duffing oscillator, connected at one end, would have representative nonlinear forces,
-$$
+```math
 \mathbf{K}_n g_n(\mathbf{x}) = \begin{bmatrix}
     k_{n,1} & - k_{n,2} & 0 \\
     0 & k_{n,2} & -k_{n,3} \\
     0 & 0 & k_{n,3}
 \end{bmatrix}
 \begin{bmatrix}
     x_1^3 \\
     (x_2-x_1)^3 \\
     (x_3 - x_2)^3
 \end{bmatrix}
-$$
+```
 
 ## Installing DynaSim
 
 To install SynaSim, follow these steps:
 
 Linux and macOS:
 ```
@@ -97,14 +97,15 @@
 
 The forcing for the system should be a list of actuations, equal in length to the number of DOFs of the system, there many actuation types,
 ```
 dynasim.actuators.sinusoid(...)
 dynasim.actuators.white_gaussian(...)
 dynasim.actuators.sine_sweep(...)
 dynasim.actuators.rand_phase_ms(...)
+dynasim.actuators.banded_noise(...)
 ```
 
 ### Totally custom system
 
 One can generate a custom system by instantiating an MDOF system with corresponding modal matrices, but the nonlinearity must also be instantiated and 
 ```
 dynasim.base.mdof_system(M, C, K, Cn, Kn)
@@ -113,8 +114,8 @@
 ## Contact
 
 If you want to contact me you can reach me at <mhaywood@ethz.ch>.
 
 ## License
 <!--- If you're not sure which open license to use see https://choosealicense.com/--->
 
-This project uses the following license: [MIT](<https://opensource.org/license/mit/>).
+This project uses the following license: [MIT](<https://opensource.org/license/mit/>).
```

### Comparing `dynasim-0.1.1/pyproject.toml` & `dynasim-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynasim"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Marcus Haywood-Alexander", email="mhaywood@ethz.ch" },
 ]
 description = "Dynamic System Simulators"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dynasim-0.1.1/src/dynasim/base.py` & `dynasim-0.1.2/src/dynasim/base.py`

 * *Files identical despite different names*

### Comparing `dynasim-0.1.1/src/dynasim/nonlinearities.py` & `dynasim-0.1.2/src/dynasim/nonlinearities.py`

 * *Files identical despite different names*

### Comparing `dynasim-0.1.1/src/dynasim/simulators.py` & `dynasim-0.1.2/src/dynasim/simulators.py`

 * *Files identical despite different names*

### Comparing `dynasim-0.1.1/src/dynasim/systems.py` & `dynasim-0.1.2/src/dynasim/systems.py`

 * *Files identical despite different names*

### Comparing `dynasim-0.1.1/src/dynasim.egg-info/PKG-INFO` & `dynasim-0.1.2/src/dynasim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynasim
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dynamic System Simulators
 Author-email: Marcus Haywood-Alexander <mhaywood@ethz.ch>
 Project-URL: Homepage, https://github.com/MarcusHA94/dynasim
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -18,30 +18,30 @@
 <!--- These are examples. See https://shields.io for others or to customize this set of shields. You might want to include dependencies, project status and licence info here --->
 ![GitHub repo size](https://img.shields.io/github/repo-size/MarcusHA94/dynasim)
 ![GitHub contributors](https://img.shields.io/github/contributors/MarcusHA94/dynasim)
 
 <!-- Project name is a `<utility/tool/feature>` that allows `<insert_target_audience>` to do `<action/task_it_does>`. -->
 
 The dynasim package simulates dynamic systems in the form:
-$$
+```math
 \mathbf{M}\ddot{\mathbf{x}} + \mathbf{C}\dot{\mathbf{x}} + \mathbf{K}\mathbf{x} + \mathbf{C}_n g_c(\mathbf{x}, \dot{\mathbf{x}}) + \mathbf{K}_n g_k(\mathbf{x}, \dot{\mathbf{x}}) = \mathbf{f}
-$$
+```
 where $\mathbf{\Xi}_n g_{\bullet}(\mathbf{x},\dot{\mathbf{x}})$ represents the nonlinear system forces. For example, a 3DOF Duffing oscillator, connected at one end, would have representative nonlinear forces,
-$$
+```math
 \mathbf{K}_n g_n(\mathbf{x}) = \begin{bmatrix}
     k_{n,1} & - k_{n,2} & 0 \\
     0 & k_{n,2} & -k_{n,3} \\
     0 & 0 & k_{n,3}
 \end{bmatrix}
 \begin{bmatrix}
     x_1^3 \\
     (x_2-x_1)^3 \\
     (x_3 - x_2)^3
 \end{bmatrix}
-$$
+```
 
 ## Installing DynaSim
 
 To install SynaSim, follow these steps:
 
 Linux and macOS:
 ```
@@ -112,14 +112,15 @@
 
 The forcing for the system should be a list of actuations, equal in length to the number of DOFs of the system, there many actuation types,
 ```
 dynasim.actuators.sinusoid(...)
 dynasim.actuators.white_gaussian(...)
 dynasim.actuators.sine_sweep(...)
 dynasim.actuators.rand_phase_ms(...)
+dynasim.actuators.banded_noise(...)
 ```
 
 ### Totally custom system
 
 One can generate a custom system by instantiating an MDOF system with corresponding modal matrices, but the nonlinearity must also be instantiated and 
 ```
 dynasim.base.mdof_system(M, C, K, Cn, Kn)
```

