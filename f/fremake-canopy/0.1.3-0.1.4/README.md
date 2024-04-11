# Comparing `tmp/fremake_canopy-0.1.3.tar.gz` & `tmp/fremake_canopy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fremake_canopy-0.1.3.tar", last modified: Mon Apr  8 20:46:41 2024, max compression
+gzip compressed data, was "fremake_canopy-0.1.4.tar", last modified: Thu Apr 11 16:06:17 2024, max compression
```

## Comparing `fremake_canopy-0.1.3.tar` & `fremake_canopy-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-08 20:46:41.294296 fremake_canopy-0.1.3/
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7642 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/LICENSE.md
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       70 2024-04-08 20:46:19.000000 fremake_canopy-0.1.3/MANIFEST.in
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      208 2024-04-08 20:46:41.294286 fremake_canopy-0.1.3/PKG-INFO
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2382 2023-11-01 18:23:29.000000 fremake_canopy-0.1.3/README.md
-drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-08 20:46:41.259291 fremake_canopy-0.1.3/fremake_canopy.egg-info/
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      208 2024-04-08 20:46:41.000000 fremake_canopy-0.1.3/fremake_canopy.egg-info/PKG-INFO
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      640 2024-04-08 20:46:41.000000 fremake_canopy-0.1.3/fremake_canopy.egg-info/SOURCES.txt
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)        1 2024-04-08 20:46:41.000000 fremake_canopy-0.1.3/fremake_canopy.egg-info/dependency_links.txt
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       27 2024-04-08 20:46:41.000000 fremake_canopy-0.1.3/fremake_canopy.egg-info/requires.txt
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       13 2024-04-08 20:46:41.000000 fremake_canopy-0.1.3/fremake_canopy.egg-info/top_level.txt
-drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-08 20:46:41.282295 fremake_canopy-0.1.3/gfdl_fremake/
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-08 20:40:07.000000 fremake_canopy-0.1.3/gfdl_fremake/__init__.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     4475 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/buildBaremetal.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7968 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/buildDocker.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     5780 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/checkout.py
--rwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)    12023 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/fremake
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7576 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/makefilefre.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     4381 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/platformfre.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6593 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/schema.json
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2367 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/targetfre.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2493 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/varsfre.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6030 2024-04-08 18:46:00.000000 fremake_canopy-0.1.3/gfdl_fremake/yamlfre.py
-drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-08 20:46:41.291291 fremake_canopy-0.1.3/gfdl_fremake/yamls/
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      231 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/yamls/am5.yaml
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     3046 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/yamls/compile.yaml
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     1144 2024-04-08 18:19:48.000000 fremake_canopy-0.1.3/gfdl_fremake/yamls/platforms.yaml
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6593 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/yamls/schema.json
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       38 2024-04-08 20:46:41.295293 fremake_canopy-0.1.3/setup.cfg
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      400 2024-04-08 20:43:33.000000 fremake_canopy-0.1.3/setup.py
+drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-11 16:06:17.594604 fremake_canopy-0.1.4/
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7642 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/LICENSE.md
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       70 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/MANIFEST.in
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      272 2024-04-11 16:06:17.591590 fremake_canopy-0.1.4/PKG-INFO
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2382 2023-11-01 18:23:29.000000 fremake_canopy-0.1.4/README.md
+drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-11 16:06:17.550585 fremake_canopy-0.1.4/fremake_canopy.egg-info/
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      272 2024-04-11 16:06:17.000000 fremake_canopy-0.1.4/fremake_canopy.egg-info/PKG-INFO
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      640 2024-04-11 16:06:17.000000 fremake_canopy-0.1.4/fremake_canopy.egg-info/SOURCES.txt
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)        1 2024-04-11 16:06:17.000000 fremake_canopy-0.1.4/fremake_canopy.egg-info/dependency_links.txt
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       27 2024-04-11 16:06:17.000000 fremake_canopy-0.1.4/fremake_canopy.egg-info/requires.txt
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       13 2024-04-11 16:06:17.000000 fremake_canopy-0.1.4/fremake_canopy.egg-info/top_level.txt
+drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-11 16:06:17.577661 fremake_canopy-0.1.4/gfdl_fremake/
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/__init__.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     4488 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/buildBaremetal.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7981 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/buildDocker.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     5780 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/checkout.py
+-rwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)    12006 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/fremake
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7576 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/makefilefre.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     4381 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/platformfre.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6593 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/schema.json
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2367 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/targetfre.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2493 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/varsfre.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6043 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/yamlfre.py
+drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-11 16:06:17.588586 fremake_canopy-0.1.4/gfdl_fremake/yamls/
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      231 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/yamls/am5.yaml
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     3046 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/yamls/compile.yaml
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     1131 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/yamls/platforms.yaml
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6593 2024-04-10 13:57:11.000000 fremake_canopy-0.1.4/gfdl_fremake/yamls/schema.json
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       38 2024-04-11 16:06:17.594681 fremake_canopy-0.1.4/setup.cfg
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      392 2024-04-11 16:06:11.000000 fremake_canopy-0.1.4/setup.py
```

### Comparing `fremake_canopy-0.1.3/LICENSE.md` & `fremake_canopy-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.3/README.md` & `fremake_canopy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.3/fremake_canopy.egg-info/SOURCES.txt` & `fremake_canopy-0.1.4/fremake_canopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.3/gfdl_fremake/buildBaremetal.py` & `fremake_canopy-0.1.4/gfdl_fremake/buildBaremetal.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ## \date 2023
 ## \author Tom Robinson
 ## \email thomas.robinson@noaa.gov
 ## \description 
 
 import subprocess
 import os
-import targetfre
+import gfdl_fremake.targetfre
 ## \brief Called for parallel execution purposes.  Runs the builds.
 ## \param fremakeBuildList the fremakeBuild object list passes by pool.map
 def fremake_parallel(fremakeBuildList):
 	fremakeBuildList.run()
 
 class buildBaremetal():
 ## \brief Creates the build script to compile the model
```

### Comparing `fremake_canopy-0.1.3/gfdl_fremake/buildDocker.py` & `fremake_canopy-0.1.4/gfdl_fremake/buildDocker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 ## \date 2023
 ## \author Tom Robinson
 ## \email thomas.robinson@noaa.gov
 ## \description 
 
 import os
-import targetfre
+import gfdl_fremake.targetfre
 
 class container():
 ## \brief Opens the Dockerfile for writing
 ## \param self The dockerfile object
 ## \param base The docker base image to start from
 ## \param libs Additional libraries defined by user 
 ## \param exp The experiment name
```

### Comparing `fremake_canopy-0.1.3/gfdl_fremake/checkout.py` & `fremake_canopy-0.1.4/gfdl_fremake/checkout.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.3/gfdl_fremake/fremake` & `fremake_canopy-0.1.4/gfdl_fremake/fremake`

 * *Files 0% similar despite different names*

```diff
@@ -246,10 +246,10 @@
           ## Run the dockerfile; build the container
           dockerBuild.build(containerBuild,containerRun)
 
           #freCheckout.cleanup()
           #buildDockerfile(fremakeYaml,image)
 
 if baremetalRun:
-          if __name__ == '__main__':
-                pool = Pool(processes=nparallel)                         # Create a multiprocessing Pool
-                pool.map(buildBaremetal.fremake_parallel,fremakeBuildList)  # process data_inputs iterable with pool 
+     if __name__ == '__main__':
+          pool = Pool(processes=nparallel)                         # Create a multiprocessing Pool
+          pool.map(buildBaremetal.fremake_parallel,fremakeBuildList)  # process data_inputs iterable with pool
```

### Comparing `fremake_canopy-0.1.3/gfdl_fremake/makefilefre.py` & `fremake_canopy-0.1.4/gfdl_fremake/makefilefre.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.3/gfdl_fremake/platformfre.py` & `fremake_canopy-0.1.4/gfdl_fremake/platformfre.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.3/gfdl_fremake/schema.json` & `fremake_canopy-0.1.4/gfdl_fremake/schema.json`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.3/gfdl_fremake/targetfre.py` & `fremake_canopy-0.1.4/gfdl_fremake/targetfre.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.3/gfdl_fremake/varsfre.py` & `fremake_canopy-0.1.4/gfdl_fremake/varsfre.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.3/gfdl_fremake/yamlfre.py` & `fremake_canopy-0.1.4/gfdl_fremake/yamlfre.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import yaml
 import json
 from jsonschema import validate, ValidationError, SchemaError
-import platformfre
+import gfdl_fremake.platformfre
 
 ## Open the yaml file and parse as fremakeYaml
 ## \param fname the name of the yaml file to parse
 ## \param v the FRE yaml varaibles (FRE properties)
 def parseCompile(fname,v):
 ## Open the yaml file and parse as fremakeYaml
      with open(fname, 'r') as file:
```

### Comparing `fremake_canopy-0.1.3/gfdl_fremake/yamls/compile.yaml` & `fremake_canopy-0.1.4/gfdl_fremake/yamls/compile.yaml`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.3/gfdl_fremake/yamls/platforms.yaml` & `fremake_canopy-0.1.4/gfdl_fremake/yamls/platforms.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
    - name: ncrc5.intel
      compiler: intel
      modulesInit: [" module use -a /ncrc/home2/fms/local/modulefiles \n","source $MODULESHOME/init/sh \n"]
      modules: ["$(INTEL)/2022.2.1","fre/bronx-20",cray-hdf5/1.12.2.3, cray-netcdf/4.9.0.3]
      fc: ftn
      cc: cc
      mkTemplate: "/ncrc/home2/fms/local/opt/fre-commands/bronx-20/site/ncrc5/$(INTEL).mk"
-     modelRoot: ${HOME}/fremake_canopy/gfdl_fremake/test
+     modelRoot: ${HOME}/fremake_canopy/test
    - name: ncrc5.intel23
      compiler: intel
      modulesInit: [" module use -a /ncrc/home2/fms/local/modulefiles \n","source $MODULESHOME/init/sh \n"]
      modules: ["$(INTEL)/2023.1.0","fre/bronx-20",cray-hdf5/1.12.2.3, cray-netcdf/4.9.0.3]
      fc: ftn
      cc: cc
      mkTemplate: "/ncrc/home2/fms/local/opt/fre-commands/bronx-20/site/ncrc5/$(INTEL).mk"
```

### Comparing `fremake_canopy-0.1.3/gfdl_fremake/yamls/schema.json` & `fremake_canopy-0.1.4/gfdl_fremake/yamls/schema.json`

 * *Files identical despite different names*

