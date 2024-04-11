# Comparing `tmp/module_qc_database_tools-2.2.6.tar.gz` & `tmp/module_qc_database_tools-2.2.7.tar.gz`

## Comparing `module_qc_database_tools-2.2.6.tar` & `module_qc_database_tools-2.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/.env.template
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/.gitlab-ci.yml
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/tbump.toml
--rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/ci/pre-commit-update.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/docs/.gitkeep
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/src/module_qc_database_tools/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/src/module_qc_database_tools/_version.py
--rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/src/module_qc_database_tools/chip_config_api.py
--rw-r--r--   0        0        0    25008 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/src/module_qc_database_tools/core.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/src/module_qc_database_tools/utils.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/src/module_qc_database_tools/cli/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/src/module_qc_database_tools/cli/__main__.py
--rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/src/module_qc_database_tools/cli/generate_yarr_config.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/src/module_qc_database_tools/cli/main.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/src/module_qc_database_tools/cli/register_component.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/src/module_qc_database_tools/data/componentConfigs.json
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/src/module_qc_database_tools/data/YARR/chip_template.json
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/tests/test_cli.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/tests/test_config_api.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/tests/test_package.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/tests/test_utils.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/LICENSE
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/README.md
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/pyproject.toml
--rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.6/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/.env.template
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/tbump.toml
+-rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/ci/pre-commit-update.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/docs/.gitkeep
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/_version.py
+-rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/chip_config_api.py
+-rw-r--r--   0        0        0    25500 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/core.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/utils.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/__main__.py
+-rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/generate_yarr_config.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/main.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/register_component.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/data/componentConfigs.json
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/data/YARR/chip_template.json
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/tests/test_cli.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/tests/test_config_api.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/tests/test_package.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/tests/test_utils.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/LICENSE
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/README.md
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/pyproject.toml
+-rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/PKG-INFO
```

### Comparing `module_qc_database_tools-2.2.6/.gitlab-ci.yml` & `module_qc_database_tools-2.2.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.6/.pre-commit-config.yaml` & `module_qc_database_tools-2.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.6/tbump.toml` & `module_qc_database_tools-2.2.7/tbump.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2232 2e32 2e36 220a 0a23 2045  t = "2.2.6"..# E
+00000010: 7420 3d20 2232 2e32 2e37 220a 0a23 2045  t = "2.2.7"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -15,15 +15,15 @@
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
 00000140: 6d70 2076 6572 7369 6f6e 3a20 322e 322e  mp version: 2.2.
-00000150: 3620 e286 9220 7b6e 6577 5f76 6572 7369  6 ... {new_versi
+00000150: 3720 e286 9220 7b6e 6577 5f76 6572 7369  7 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
 000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
```

### Comparing `module_qc_database_tools-2.2.6/ci/pre-commit-update.sh` & `module_qc_database_tools-2.2.7/ci/pre-commit-update.sh`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.6/src/module_qc_database_tools/__init__.py` & `module_qc_database_tools-2.2.7/src/module_qc_database_tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,12 +11,12 @@
     import importlib_resources as resources
 data = resources.files("module_qc_database_tools") / "data"
 
 handler = RichHandler(markup=True)
 formatter = logging.Formatter(fmt="%(message)s", datefmt="[%X]")
 handler.setFormatter(formatter)
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+logger.setLevel(logging.INFO)
 logger.addHandler(handler)
 logger.propagate = False
 
 __all__ = ("__version__", "data")
```

### Comparing `module_qc_database_tools-2.2.6/src/module_qc_database_tools/chip_config_api.py` & `module_qc_database_tools-2.2.7/src/module_qc_database_tools/chip_config_api.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.6/src/module_qc_database_tools/core.py` & `module_qc_database_tools-2.2.7/src/module_qc_database_tools/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,18 +94,22 @@
         speed=1280,
         reverse=False,
     ):
         """
         Generate module config.
         """
         log.info(
-            "generating module config for module %s with %s",
+            "Generating module config for module %s with %s from %s version for %i MHz.",
             self.serial_number,
             layer_config,
+            version,
+            speed,
         )
+        if self.module_type == "triplet" and reverse:
+            log.info("Orientation is reverse!")
 
         configs = {"module": {"chipType": "RD53B", "chips": []}, "chips": []}
 
         for chip_index, chip in enumerate(self.chips):
             if self.module_type == "triplet":
                 rx = [2, 1, 0][chip_index] if reverse else [0, 1, 2][chip_index]
             else:
@@ -629,25 +633,39 @@
         )
 
         current_stage = qc_status.get("currentStage")
         log.info("current_stage: %s", current_stage)
 
         return current_stage
 
-    def generate_config(self, chip_template, layer_config, suffix, version):
+    # speed and reverse needed to match the non-localDB module generate_config function
+    def generate_config(
+        self,
+        chip_template,
+        layer_config,
+        suffix,
+        version,
+        speed=1280,
+        reverse=False,
+    ):
         """
         Generate module config.
         """
         log.info(
-            "generating module config for module %s with %s | chip_template '%s' version '%s'",
+            "Generating module config for module %s with %s from %s version.",
             self.serial_number,
             layer_config,
-            chip_template,
             version,
         )
+        log.debug(
+            "Unused variables: chip template: %s, speed: %i MHz, reverse orientation: %s.",
+            chip_template,
+            speed,
+            reverse,
+        )
 
         config_api = ChipConfigAPI(self.client)
 
         current_stage = self.get_current_stage()
 
         configs = {"module": {"chipType": "RD53B", "chips": []}, "chips": []}
```

### Comparing `module_qc_database_tools-2.2.6/src/module_qc_database_tools/utils.py` & `module_qc_database_tools-2.2.7/src/module_qc_database_tools/utils.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.6/src/module_qc_database_tools/cli/generate_yarr_config.py` & `module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/generate_yarr_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,18 @@
     modes: List[str] = typer.Option(
         ["warm", "cold", "LP"],
         "-m",
         "--mode",
         help="Modes to generate configs for.",
     ),
     version: str = typer.Option(
-        "latest",  ## "TESTONWAFER", "MODULE/INITIAL_WARM", "etc"], ## use stage/test names?
+        "latest",  ## TODO: ["latest", "TESTONWAFER", "MODULE/INITIAL_WARM", ...], ## use stage/test names?
         "-v",
         "--version",
-        help="Generate chip configs, default is 'latest'. Possible choices: 'TESTONWAFER'...",
+        help="Generate chip configs, default is 'latest'. Possible choices: 'TESTONWAFER', 'latest'",
     ),
     speed: int = typer.Option(
         1280,
         "-s",
         "--speed",
         help="Readout speed in MHz. Possible choices: [1280, 640, 320, 160] MHz.",
     ),
```

### Comparing `module_qc_database_tools-2.2.6/src/module_qc_database_tools/cli/main.py` & `module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.6/src/module_qc_database_tools/cli/register_component.py` & `module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/register_component.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.6/src/module_qc_database_tools/data/componentConfigs.json` & `module_qc_database_tools-2.2.7/src/module_qc_database_tools/data/componentConfigs.json`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.6/tests/test_cli.py` & `module_qc_database_tools-2.2.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.6/tests/test_config_api.py` & `module_qc_database_tools-2.2.7/tests/test_config_api.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.6/.gitignore` & `module_qc_database_tools-2.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.6/LICENSE` & `module_qc_database_tools-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.6/README.md` & `module_qc_database_tools-2.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Module QC Database Tools v2.2.6
+# Module QC Database Tools v2.2.7
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```

### Comparing `module_qc_database_tools-2.2.6/pyproject.toml` & `module_qc_database_tools-2.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 description = "Python wrapper to interface with LocalDB and Production DB for common tasks for pixel modules."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 dependencies = [
-    "itkdb>=0.4.13",  # for interface with production database
+    "itkdb>=0.5.1",  # for interface with production database
     "pandas",
     "pyarrow",
     "typer",
     "pymongo",
     "jsondiff",
     "importlib_resources>=1.4.0; python_version < '3.9'",  # for resources
     "jsbeautifier", # for chip config linebreaks vs size
```

### Comparing `module_qc_database_tools-2.2.6/PKG-INFO` & `module_qc_database_tools-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: module-qc-database-tools
-Version: 2.2.6
+Version: 2.2.7
 Summary: Python wrapper to interface with LocalDB and Production DB for common tasks for pixel modules.
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <kratsg@gmail.com>, Elisabetta Pianori <elisabetta.pianori@cern.ch>, Lingxin Meng <lingxin.meng@cern.ch>
 License: Copyright (c) 2022 ATLAS ITk Pixel Modules
@@ -39,26 +39,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
-Requires-Dist: itkdb>=0.4.13
+Requires-Dist: itkdb>=0.5.1
 Requires-Dist: jsbeautifier
 Requires-Dist: jsondiff
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pymongo
 Requires-Dist: rich
 Requires-Dist: typer
 Requires-Dist: urllib3<2,>=1.26.11; 'el7.x86_64' in platform_release
 Description-Content-Type: text/markdown
 
-# Module QC Database Tools v2.2.6
+# Module QC Database Tools v2.2.7
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```

