# Comparing `tmp/viur_cli-2.0.0rc5.tar.gz` & `tmp/viur_cli-2.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur_cli-2.0.0rc5.tar", last modified: Tue Mar  5 15:16:51 2024, max compression
+gzip compressed data, was "viur_cli-2.0.0rc6.tar", last modified: Fri Mar 22 14:06:43 2024, max compression
```

## Comparing `viur_cli-2.0.0rc5.tar` & `viur_cli-2.0.0rc6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:16:51.105780 viur_cli-2.0.0rc5/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8993 2024-03-05 15:16:51.105780 viur_cli-2.0.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-05 15:16:51.105780 viur_cli-2.0.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:16:51.097780 viur_cli-2.0.0rc5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:16:51.101780 viur_cli-2.0.0rc5/src/viur_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    26522 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:16:51.101780 viur_cli-2.0.0rc5/src/viur_cli/scriptor/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scriptor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:16:51.101780 viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/csvwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/viur.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:16:51.105780 viur_cli-2.0.0rc5/src/viur_cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scripts/get_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/scripts/viur_2to3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-05 15:16:43.000000 viur_cli-2.0.0rc5/src/viur_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:16:51.105780 viur_cli-2.0.0rc5/src/viur_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8993 2024-03-05 15:16:51.000000 viur_cli-2.0.0rc5/src/viur_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-05 15:16:51.000000 viur_cli-2.0.0rc5/src/viur_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 15:16:51.000000 viur_cli-2.0.0rc5/src/viur_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-05 15:16:51.000000 viur_cli-2.0.0rc5/src/viur_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-05 15:16:51.000000 viur_cli-2.0.0rc5/src/viur_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-05 15:16:51.000000 viur_cli-2.0.0rc5/src/viur_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.633774 viur_cli-2.0.0rc6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-03-22 14:06:43.633774 viur_cli-2.0.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-22 14:06:43.633774 viur_cli-2.0.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.621774 viur_cli-2.0.0rc6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.625774 viur_cli-2.0.0rc6/src/viur_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26913 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.629774 viur_cli-2.0.0rc6/src/viur_cli/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.629774 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/csvwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/viur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.629774 viur_cli-2.0.0rc6/src/viur_cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scripts/get_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scripts/viur_2to3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.629774 viur_cli-2.0.0rc6/src/viur_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-03-22 14:06:43.000000 viur_cli-2.0.0rc6/src/viur_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-22 14:06:43.000000 viur_cli-2.0.0rc6/src/viur_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 14:06:43.000000 viur_cli-2.0.0rc6/src/viur_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-22 14:06:43.000000 viur_cli-2.0.0rc6/src/viur_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-22 14:06:43.000000 viur_cli-2.0.0rc6/src/viur_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-22 14:06:43.000000 viur_cli-2.0.0rc6/src/viur_cli.egg-info/top_level.txt
```

### Comparing `viur_cli-2.0.0rc5/LICENSE` & `viur_cli-2.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/PKG-INFO` & `viur_cli-2.0.0rc6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur_cli
-Version: 2.0.0rc5
+Version: 2.0.0rc6
 Summary: Command-line interface for ViUR application maintenance.
 Home-page: https://github.com/viur-framework/viur-cli
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -103,14 +103,20 @@
 Scripts:
 - `app`           Deploy application to the Google Appengine
   - `index`         Deploy index.yaml to Google Appenginge
   - `cloudfunction` Deploy Cloudfunction to Google Appengine
   Commands:
   - `profile`       The project.json profile you want to Work from
 
+```sh
+$ viur cloud init {service} {profile} 
+```
+This Function makes the init deployment for a ViUR project.
+This Function needs to be called so that the development server works locally.
+
 
 ```sh
 $ viur cloud {enable|disable} backup
 ```
 Enable/ Disable the Backup buckets you need to Backup a cloud project in the Google Cloud Console
 
 ```sh
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur_cli Version: 2.0.0rc5 Summary: Command-line
+Metadata-Version: 2.1 Name: viur_cli Version: 2.0.0rc6 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.11 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: app_server==0.9.9 Requires-Dist: click==8.1.7 Requires-Dist:
@@ -33,58 +33,60 @@
 specific application - `clean` Clean up Build Artifacts - `release` Build all
 relevant applications to deploy the project ```sh $ viur cloud deploy
 {app|index|cloudfunction} {profile} {--ext|--yes|--name} ``` This Function
 deploys the Google Cloud application and / or different .yaml files Scripts: -
 `app` Deploy application to the Google Appengine - `index` Deploy index.yaml to
 Google Appenginge - `cloudfunction` Deploy Cloudfunction to Google Appengine
 Commands: - `profile` The project.json profile you want to Work from ```sh $
-viur cloud {enable|disable} backup ``` Enable/ Disable the Backup buckets you
-need to Backup a cloud project in the Google Cloud Console ```sh $ viur cloud
-setup {gcloud|gcroles} ``` Scripts: - `gcloud` This Function setups your
-project to work on the gcloud plattform - `gcroles` This function lets you set
-up Roles for your google appengine Workspace ```sh $ viur cloud get {gcroles}
-``` Scripts: - `gcroles` This function lets you get Roles for your google
-appengine Workspace in a readable .json Format ```sh $ viur package
-{update|install} {vi|admin|scriptor|all} [profile] [version] ``` Performs
-operations on packages Scripts: - `update` Updates an installed package -
-`install` Installs a declared package Options: - `vi` - `admin` - `scriptor` -
-`all` ```sh $ viur env ``` Show information about your current environment.
-```sh $ viur project list ``` Pretty prints your `project.json` file on the
-console. ```sh $ viur update {requirements} ``` with this you can update your
-project specific requirements.txt file automatically ## The project.json The
-`project.json` is your core project configuration file for every viur related
-operation. It contains the default viur project profile and it can be expanded
-with several individual project profiles. ### Example project.json ```json
-lines { /* The format Key, Value pair defines the project json format, the
-viur-cli uses */ "format": "2.0.0", /* The first level contains of your
-profiles "default" is a profile, which is inherited by "develop" and "live" and
-can be customized for particular versions and/or GAE projects. Therefore, every
-profile can contain all keys from the "default" profile.*/ "default": { /* The
-builds level declares steps for the `viur build` command. It can contain viur
-components and other components that need to be build before project deployment
-*/ "builds": { "admin": { "command": "viur install admin", "kind": "exec",
-"version": "4.0.8" }, "npm": { "command": "build", "kind": "npm", "source": ""
-} }, "gcloud": { "functions": { //Declarations for a cloud function
-"testfunction1": { "entry-point": "main", "env-vars-file": "env.yaml",
-"memory": "512MB", "runtime": "python311", "source": "deploy/cloudfunction/
-function1", "trigger": "http" } }, "max-instances": "1", "region": "europe-
-west3" }, "core": "3.5.1", // viur-core version of your project
-"distribution_folder": "./deploy", // Deploy folder uploaded to GAE
-"sources_folder": "./sources", "version": "live-$(year)-$(month)-$(day)", /
-/ Version string; Variables can be used here. "application_name": "my-live-app-
-viur3" // Name of the GAE project *4 }, "develop": { "application_name": "my-
-dev-app-viur3", "version": "dev-$(user)" } } ``` ## Viur scripting interface
-There is a new core component that enables us to pull and push python scripts
-from/to a deployed application and run these in a sandbox or even locally. The
-GUI version is called scriptor and can be accessed via a webinterface, but
-viur-cli also has a cli for this: ```sh $ viur script
-{configure|pull|push|run|setup} ``` Manage your ViUR Scriptor Scripts via the
-CLI Commands: - `configure` Manage configuration settings. - `pull` Pull
-contents from server to working_dir. - `push` Push contents of working_dir to
-server. - `run` Locally run a script located in the working_dir. - `setup`
+viur cloud init {service} {profile} ``` This Function makes the init deployment
+for a ViUR project. This Function needs to be called so that the development
+server works locally. ```sh $ viur cloud {enable|disable} backup ``` Enable/
+Disable the Backup buckets you need to Backup a cloud project in the Google
+Cloud Console ```sh $ viur cloud setup {gcloud|gcroles} ``` Scripts: - `gcloud`
+This Function setups your project to work on the gcloud plattform - `gcroles`
+This function lets you set up Roles for your google appengine Workspace ```sh $
+viur cloud get {gcroles} ``` Scripts: - `gcroles` This function lets you get
+Roles for your google appengine Workspace in a readable .json Format ```sh $
+viur package {update|install} {vi|admin|scriptor|all} [profile] [version] ```
+Performs operations on packages Scripts: - `update` Updates an installed
+package - `install` Installs a declared package Options: - `vi` - `admin` -
+`scriptor` - `all` ```sh $ viur env ``` Show information about your current
+environment. ```sh $ viur project list ``` Pretty prints your `project.json`
+file on the console. ```sh $ viur update {requirements} ``` with this you can
+update your project specific requirements.txt file automatically ## The
+project.json The `project.json` is your core project configuration file for
+every viur related operation. It contains the default viur project profile and
+it can be expanded with several individual project profiles. ### Example
+project.json ```json lines { /* The format Key, Value pair defines the project
+json format, the viur-cli uses */ "format": "2.0.0", /* The first level
+contains of your profiles "default" is a profile, which is inherited by
+"develop" and "live" and can be customized for particular versions and/or GAE
+projects. Therefore, every profile can contain all keys from the "default"
+profile.*/ "default": { /* The builds level declares steps for the `viur build`
+command. It can contain viur components and other components that need to be
+build before project deployment */ "builds": { "admin": { "command": "viur
+install admin", "kind": "exec", "version": "4.0.8" }, "npm": { "command":
+"build", "kind": "npm", "source": "" } }, "gcloud": { "functions": { //
+Declarations for a cloud function "testfunction1": { "entry-point": "main",
+"env-vars-file": "env.yaml", "memory": "512MB", "runtime": "python311",
+"source": "deploy/cloudfunction/function1", "trigger": "http" } }, "max-
+instances": "1", "region": "europe-west3" }, "core": "3.5.1", // viur-core
+version of your project "distribution_folder": "./deploy", // Deploy folder
+uploaded to GAE "sources_folder": "./sources", "version": "live-$(year)-$
+(month)-$(day)", // Version string; Variables can be used here.
+"application_name": "my-live-app-viur3" // Name of the GAE project *4 },
+"develop": { "application_name": "my-dev-app-viur3", "version": "dev-$(user)" }
+} ``` ## Viur scripting interface There is a new core component that enables us
+to pull and push python scripts from/to a deployed application and run these in
+a sandbox or even locally. The GUI version is called scriptor and can be
+accessed via a webinterface, but viur-cli also has a cli for this: ```sh $ viur
+script {configure|pull|push|run|setup} ``` Manage your ViUR Scriptor Scripts
+via the CLI Commands: - `configure` Manage configuration settings. - `pull`
+Pull contents from server to working_dir. - `push` Push contents of working_dir
+to server. - `run` Locally run a script located in the working_dir. - `setup`
 Setup user session with a given username and... ## Packaged tools In order to
 use the packaged tools, you can run: ```sh $ viur tool {2to3|pyodide|ssl-fix}
 ``` Scripts: - `2to3` viur porting script - `pyodide` run the get_pyodide
 command - `ssl-fix` ssl fix for MacOS for example the 2to3 script helps porting
 viur2 project to viur3, it can be used to automatically rename some things that
 are deprecated in viur3 as well, so you can use it whenever a new core version
 is released for viur3 projects as well: ```sh $ viur tool 2to3 -d . ``` will
```

### Comparing `viur_cli-2.0.0rc5/README.md` & `viur_cli-2.0.0rc6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,20 @@
 Scripts:
 - `app`           Deploy application to the Google Appengine
   - `index`         Deploy index.yaml to Google Appenginge
   - `cloudfunction` Deploy Cloudfunction to Google Appengine
   Commands:
   - `profile`       The project.json profile you want to Work from
 
+```sh
+$ viur cloud init {service} {profile} 
+```
+This Function makes the init deployment for a ViUR project.
+This Function needs to be called so that the development server works locally.
+
 
 ```sh
 $ viur cloud {enable|disable} backup
 ```
 Enable/ Disable the Backup buckets you need to Backup a cloud project in the Google Cloud Console
 
 ```sh
```

#### html2text {}

```diff
@@ -23,58 +23,60 @@
 specific application - `clean` Clean up Build Artifacts - `release` Build all
 relevant applications to deploy the project ```sh $ viur cloud deploy
 {app|index|cloudfunction} {profile} {--ext|--yes|--name} ``` This Function
 deploys the Google Cloud application and / or different .yaml files Scripts: -
 `app` Deploy application to the Google Appengine - `index` Deploy index.yaml to
 Google Appenginge - `cloudfunction` Deploy Cloudfunction to Google Appengine
 Commands: - `profile` The project.json profile you want to Work from ```sh $
-viur cloud {enable|disable} backup ``` Enable/ Disable the Backup buckets you
-need to Backup a cloud project in the Google Cloud Console ```sh $ viur cloud
-setup {gcloud|gcroles} ``` Scripts: - `gcloud` This Function setups your
-project to work on the gcloud plattform - `gcroles` This function lets you set
-up Roles for your google appengine Workspace ```sh $ viur cloud get {gcroles}
-``` Scripts: - `gcroles` This function lets you get Roles for your google
-appengine Workspace in a readable .json Format ```sh $ viur package
-{update|install} {vi|admin|scriptor|all} [profile] [version] ``` Performs
-operations on packages Scripts: - `update` Updates an installed package -
-`install` Installs a declared package Options: - `vi` - `admin` - `scriptor` -
-`all` ```sh $ viur env ``` Show information about your current environment.
-```sh $ viur project list ``` Pretty prints your `project.json` file on the
-console. ```sh $ viur update {requirements} ``` with this you can update your
-project specific requirements.txt file automatically ## The project.json The
-`project.json` is your core project configuration file for every viur related
-operation. It contains the default viur project profile and it can be expanded
-with several individual project profiles. ### Example project.json ```json
-lines { /* The format Key, Value pair defines the project json format, the
-viur-cli uses */ "format": "2.0.0", /* The first level contains of your
-profiles "default" is a profile, which is inherited by "develop" and "live" and
-can be customized for particular versions and/or GAE projects. Therefore, every
-profile can contain all keys from the "default" profile.*/ "default": { /* The
-builds level declares steps for the `viur build` command. It can contain viur
-components and other components that need to be build before project deployment
-*/ "builds": { "admin": { "command": "viur install admin", "kind": "exec",
-"version": "4.0.8" }, "npm": { "command": "build", "kind": "npm", "source": ""
-} }, "gcloud": { "functions": { //Declarations for a cloud function
-"testfunction1": { "entry-point": "main", "env-vars-file": "env.yaml",
-"memory": "512MB", "runtime": "python311", "source": "deploy/cloudfunction/
-function1", "trigger": "http" } }, "max-instances": "1", "region": "europe-
-west3" }, "core": "3.5.1", // viur-core version of your project
-"distribution_folder": "./deploy", // Deploy folder uploaded to GAE
-"sources_folder": "./sources", "version": "live-$(year)-$(month)-$(day)", /
-/ Version string; Variables can be used here. "application_name": "my-live-app-
-viur3" // Name of the GAE project *4 }, "develop": { "application_name": "my-
-dev-app-viur3", "version": "dev-$(user)" } } ``` ## Viur scripting interface
-There is a new core component that enables us to pull and push python scripts
-from/to a deployed application and run these in a sandbox or even locally. The
-GUI version is called scriptor and can be accessed via a webinterface, but
-viur-cli also has a cli for this: ```sh $ viur script
-{configure|pull|push|run|setup} ``` Manage your ViUR Scriptor Scripts via the
-CLI Commands: - `configure` Manage configuration settings. - `pull` Pull
-contents from server to working_dir. - `push` Push contents of working_dir to
-server. - `run` Locally run a script located in the working_dir. - `setup`
+viur cloud init {service} {profile} ``` This Function makes the init deployment
+for a ViUR project. This Function needs to be called so that the development
+server works locally. ```sh $ viur cloud {enable|disable} backup ``` Enable/
+Disable the Backup buckets you need to Backup a cloud project in the Google
+Cloud Console ```sh $ viur cloud setup {gcloud|gcroles} ``` Scripts: - `gcloud`
+This Function setups your project to work on the gcloud plattform - `gcroles`
+This function lets you set up Roles for your google appengine Workspace ```sh $
+viur cloud get {gcroles} ``` Scripts: - `gcroles` This function lets you get
+Roles for your google appengine Workspace in a readable .json Format ```sh $
+viur package {update|install} {vi|admin|scriptor|all} [profile] [version] ```
+Performs operations on packages Scripts: - `update` Updates an installed
+package - `install` Installs a declared package Options: - `vi` - `admin` -
+`scriptor` - `all` ```sh $ viur env ``` Show information about your current
+environment. ```sh $ viur project list ``` Pretty prints your `project.json`
+file on the console. ```sh $ viur update {requirements} ``` with this you can
+update your project specific requirements.txt file automatically ## The
+project.json The `project.json` is your core project configuration file for
+every viur related operation. It contains the default viur project profile and
+it can be expanded with several individual project profiles. ### Example
+project.json ```json lines { /* The format Key, Value pair defines the project
+json format, the viur-cli uses */ "format": "2.0.0", /* The first level
+contains of your profiles "default" is a profile, which is inherited by
+"develop" and "live" and can be customized for particular versions and/or GAE
+projects. Therefore, every profile can contain all keys from the "default"
+profile.*/ "default": { /* The builds level declares steps for the `viur build`
+command. It can contain viur components and other components that need to be
+build before project deployment */ "builds": { "admin": { "command": "viur
+install admin", "kind": "exec", "version": "4.0.8" }, "npm": { "command":
+"build", "kind": "npm", "source": "" } }, "gcloud": { "functions": { //
+Declarations for a cloud function "testfunction1": { "entry-point": "main",
+"env-vars-file": "env.yaml", "memory": "512MB", "runtime": "python311",
+"source": "deploy/cloudfunction/function1", "trigger": "http" } }, "max-
+instances": "1", "region": "europe-west3" }, "core": "3.5.1", // viur-core
+version of your project "distribution_folder": "./deploy", // Deploy folder
+uploaded to GAE "sources_folder": "./sources", "version": "live-$(year)-$
+(month)-$(day)", // Version string; Variables can be used here.
+"application_name": "my-live-app-viur3" // Name of the GAE project *4 },
+"develop": { "application_name": "my-dev-app-viur3", "version": "dev-$(user)" }
+} ``` ## Viur scripting interface There is a new core component that enables us
+to pull and push python scripts from/to a deployed application and run these in
+a sandbox or even locally. The GUI version is called scriptor and can be
+accessed via a webinterface, but viur-cli also has a cli for this: ```sh $ viur
+script {configure|pull|push|run|setup} ``` Manage your ViUR Scriptor Scripts
+via the CLI Commands: - `configure` Manage configuration settings. - `pull`
+Pull contents from server to working_dir. - `push` Push contents of working_dir
+to server. - `run` Locally run a script located in the working_dir. - `setup`
 Setup user session with a given username and... ## Packaged tools In order to
 use the packaged tools, you can run: ```sh $ viur tool {2to3|pyodide|ssl-fix}
 ``` Scripts: - `2to3` viur porting script - `pyodide` run the get_pyodide
 command - `ssl-fix` ssl fix for MacOS for example the 2to3 script helps porting
 viur2 project to viur3, it can be used to automatically rename some things that
 are deprecated in viur3 as well, so you can use it whenever a new core version
 is released for viur3 projects as well: ```sh $ viur tool 2to3 -d . ``` will
```

### Comparing `viur_cli-2.0.0rc5/setup.cfg` & `viur_cli-2.0.0rc6/setup.cfg`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/build.py` & `viur_cli-2.0.0rc6/src/viur_cli/build.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/cli.py` & `viur_cli-2.0.0rc6/src/viur_cli/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/cloud.py` & `viur_cli-2.0.0rc6/src/viur_cli/cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,22 @@
             print(f'An Error Occured during Roles {e}\n '
                   f'Please make sure you have the correct Google Cloud Access rights'
                   )
             return
 
     print('Success! It may take a while until you can use Gcloud Backups')
 
+@cloud.command(context_settings={"ignore_unknown_options": True})
+@click.argument("service", type=click.Choice(["gcloud"]), default="gcloud")
+@click.argument("profile", default="default")
+def init(service, profile):
+    deployments = ["cron", "queue", "cron"]
+    if service == "gcloud":
+        for element in deployments:
+            os.system(f"viur cloud deploy {element} {profile} -y")
 
 @cloud.command(context_settings={"ignore_unknown_options": True})
 @click.argument("service", type=click.Choice(["gcloud"]), default="gcloud")
 @click.argument("option", type=click.Choice(["datastore"]), default="datastore")
 @click.argument("profile", default="default")
 def cleanup(service, option, profile):
     conf = config.get_profile(profile)
```

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/conf.py` & `viur_cli-2.0.0rc6/src/viur_cli/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import json
 import click
+import requests
+import difflib
 from .utils import *
+from .version import __version__ as cli_version
 
 PROJECT_CONFIG_FILE = "project.json"
 PROJECT_CONFIG_VERSION = "2.0.0"
+LAST_VERSION = ""
 
 
 class ProjectConfig(dict):
 
     def __init__(self):
         super().__init__()
         self["default"] = {}
@@ -81,23 +85,31 @@
             self.save()
         except:
             raise click.ClickException(click.style(f"{configname} not found", fg="red"))
 
     def migrate(self):
         if old_format := self["default"].get("format"):
             self["format"] = old_format
-                del self["default"]["format"]
+            del self["default"]["format"]
 
         assert self["format"] in ["1.0.0", "1.0.1", "1.1.0", "1.1.1", "1.2.0", PROJECT_CONFIG_VERSION], \
             "Invalid formatversion, you have to fix it manually"
 
         # Version 1.0.1
         if (pyodide_version := self["default"].get("pyodide")) and pyodide_version.startswith("v"):
             self["default"]["pyodide"] = pyodide_version[1:]  # remove v prefix
 
+        if not self.get("cli-version"):
+            print_changelog_from_github('viur-framework', 'viur-cli', None)
+            self["cli-version"] = cli_version
+
+        elif self.get("cli-version") != cli_version:
+            print_changelog_from_github('viur-framework', 'viur-cli', self.get("cli-version"))
+            self["cli-version"] = cli_version
+
         if self["format"] == "1.0.0":
             self["format"] = "1.0.1"
 
         # Version 1.1.1
         if self["format"] == "1.1.0":
             self["format"] = "1.1.1"
             builds = self["default"].get("builds", {}).copy()
@@ -167,8 +179,39 @@
         except:
             self["default"]["core"] = "submodule"
 
         # conf updates must increase format version
         self.save()
 
 
+def print_changelog_from_github(user, repo, last_version):
+    version_url = f"https://raw.githubusercontent.com/{user}/{repo}/main/CHANGELOG.md"
+    response = requests.get(version_url)
+
+    if last_version is not None:
+        version_url1 = f"https://raw.githubusercontent.com/{user}/{repo}/{last_version}/CHANGELOG.md"
+        echo_warning(version_url1)
+        response1 = requests.get(version_url1)
+
+    if last_version is None and response.ok:
+        changelog_lines = response.text.split("\n")[:20]
+        echo_info("It seems you have updated your viur-cli!\n "
+                  "Please consider reading the changelog: https://github.com/viur-framework/viur-cli/blob/main/CHANGELOG.md")
+        click.echo("\n".join(changelog_lines))
+        click.confirm("Done?", default=True)
+
+    elif response.ok and response1.ok:
+        get_changelog_difference(response.text.split('\n'), response1.text.split('\n'))
+
+    else:
+        echo_error("Unable to fetch the changelog.")
+
+
+def get_changelog_difference(response, response1):
+    diff = difflib.unified_diff(response, response1)
+    for line in diff:  # Skip the first 2 lines
+        if line.startswith('@@') or line.startswith('---') or line.startswith('+++'):
+            continue
+        echo_info(line[1:])
+
+
 config = ProjectConfig()
```

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/local.py` & `viur_cli-2.0.0rc6/src/viur_cli/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 @click.argument("profile", default='default')
 @click.argument("additional_args", nargs=-1)
 def run(profile, additional_args):
     """
         Start your application locally.
         The 'run' command launches your ViUR application locally specified configuration and optional arguments.
     """
-    echo_warning(f"You are using the development Server with your default account: {get_user_info()["email"]}")
+    echo_warning(f"You are using the development Server with your default account: {get_user_info()['email']}")
     conf = config.get_profile(profile)
 
     utils.system(f'app_server -A={conf["application_name"]} {conf["distribution_folder"]} {" ".join(additional_args)}')
 
 @cli.command()
 @click.argument("profile", default="default")
 def env(profile):
```

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/package.py` & `viur_cli-2.0.0rc6/src/viur_cli/package.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/scriptor/cli.py` & `viur_cli-2.0.0rc6/src/viur_cli/scriptor/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/__init__.py` & `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/__init__.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/csvwriter.py` & `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/csvwriter.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/dialog.py` & `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/dialog.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/logger.py` & `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/logger.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/module.py` & `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/module.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/network.py` & `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/network.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/readers.py` & `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/readers.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/viur.py` & `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/viur.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/scriptor/scriptor/writer.py` & `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/writer.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/scripts/get_pyodide.py` & `viur_cli-2.0.0rc6/src/viur_cli/scripts/get_pyodide.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/scripts/viur_2to3.py` & `viur_cli-2.0.0rc6/src/viur_cli/scripts/viur_2to3.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/setup.py` & `viur_cli-2.0.0rc6/src/viur_cli/setup.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/tool.py` & `viur_cli-2.0.0rc6/src/viur_cli/tool.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/update.py` & `viur_cli-2.0.0rc6/src/viur_cli/update.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli/utils.py` & `viur_cli-2.0.0rc6/src/viur_cli/utils.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc5/src/viur_cli.egg-info/PKG-INFO` & `viur_cli-2.0.0rc6/src/viur_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur_cli
-Version: 2.0.0rc5
+Version: 2.0.0rc6
 Summary: Command-line interface for ViUR application maintenance.
 Home-page: https://github.com/viur-framework/viur-cli
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -103,14 +103,20 @@
 Scripts:
 - `app`           Deploy application to the Google Appengine
   - `index`         Deploy index.yaml to Google Appenginge
   - `cloudfunction` Deploy Cloudfunction to Google Appengine
   Commands:
   - `profile`       The project.json profile you want to Work from
 
+```sh
+$ viur cloud init {service} {profile} 
+```
+This Function makes the init deployment for a ViUR project.
+This Function needs to be called so that the development server works locally.
+
 
 ```sh
 $ viur cloud {enable|disable} backup
 ```
 Enable/ Disable the Backup buckets you need to Backup a cloud project in the Google Cloud Console
 
 ```sh
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur_cli Version: 2.0.0rc5 Summary: Command-line
+Metadata-Version: 2.1 Name: viur_cli Version: 2.0.0rc6 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.11 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: app_server==0.9.9 Requires-Dist: click==8.1.7 Requires-Dist:
@@ -33,58 +33,60 @@
 specific application - `clean` Clean up Build Artifacts - `release` Build all
 relevant applications to deploy the project ```sh $ viur cloud deploy
 {app|index|cloudfunction} {profile} {--ext|--yes|--name} ``` This Function
 deploys the Google Cloud application and / or different .yaml files Scripts: -
 `app` Deploy application to the Google Appengine - `index` Deploy index.yaml to
 Google Appenginge - `cloudfunction` Deploy Cloudfunction to Google Appengine
 Commands: - `profile` The project.json profile you want to Work from ```sh $
-viur cloud {enable|disable} backup ``` Enable/ Disable the Backup buckets you
-need to Backup a cloud project in the Google Cloud Console ```sh $ viur cloud
-setup {gcloud|gcroles} ``` Scripts: - `gcloud` This Function setups your
-project to work on the gcloud plattform - `gcroles` This function lets you set
-up Roles for your google appengine Workspace ```sh $ viur cloud get {gcroles}
-``` Scripts: - `gcroles` This function lets you get Roles for your google
-appengine Workspace in a readable .json Format ```sh $ viur package
-{update|install} {vi|admin|scriptor|all} [profile] [version] ``` Performs
-operations on packages Scripts: - `update` Updates an installed package -
-`install` Installs a declared package Options: - `vi` - `admin` - `scriptor` -
-`all` ```sh $ viur env ``` Show information about your current environment.
-```sh $ viur project list ``` Pretty prints your `project.json` file on the
-console. ```sh $ viur update {requirements} ``` with this you can update your
-project specific requirements.txt file automatically ## The project.json The
-`project.json` is your core project configuration file for every viur related
-operation. It contains the default viur project profile and it can be expanded
-with several individual project profiles. ### Example project.json ```json
-lines { /* The format Key, Value pair defines the project json format, the
-viur-cli uses */ "format": "2.0.0", /* The first level contains of your
-profiles "default" is a profile, which is inherited by "develop" and "live" and
-can be customized for particular versions and/or GAE projects. Therefore, every
-profile can contain all keys from the "default" profile.*/ "default": { /* The
-builds level declares steps for the `viur build` command. It can contain viur
-components and other components that need to be build before project deployment
-*/ "builds": { "admin": { "command": "viur install admin", "kind": "exec",
-"version": "4.0.8" }, "npm": { "command": "build", "kind": "npm", "source": ""
-} }, "gcloud": { "functions": { //Declarations for a cloud function
-"testfunction1": { "entry-point": "main", "env-vars-file": "env.yaml",
-"memory": "512MB", "runtime": "python311", "source": "deploy/cloudfunction/
-function1", "trigger": "http" } }, "max-instances": "1", "region": "europe-
-west3" }, "core": "3.5.1", // viur-core version of your project
-"distribution_folder": "./deploy", // Deploy folder uploaded to GAE
-"sources_folder": "./sources", "version": "live-$(year)-$(month)-$(day)", /
-/ Version string; Variables can be used here. "application_name": "my-live-app-
-viur3" // Name of the GAE project *4 }, "develop": { "application_name": "my-
-dev-app-viur3", "version": "dev-$(user)" } } ``` ## Viur scripting interface
-There is a new core component that enables us to pull and push python scripts
-from/to a deployed application and run these in a sandbox or even locally. The
-GUI version is called scriptor and can be accessed via a webinterface, but
-viur-cli also has a cli for this: ```sh $ viur script
-{configure|pull|push|run|setup} ``` Manage your ViUR Scriptor Scripts via the
-CLI Commands: - `configure` Manage configuration settings. - `pull` Pull
-contents from server to working_dir. - `push` Push contents of working_dir to
-server. - `run` Locally run a script located in the working_dir. - `setup`
+viur cloud init {service} {profile} ``` This Function makes the init deployment
+for a ViUR project. This Function needs to be called so that the development
+server works locally. ```sh $ viur cloud {enable|disable} backup ``` Enable/
+Disable the Backup buckets you need to Backup a cloud project in the Google
+Cloud Console ```sh $ viur cloud setup {gcloud|gcroles} ``` Scripts: - `gcloud`
+This Function setups your project to work on the gcloud plattform - `gcroles`
+This function lets you set up Roles for your google appengine Workspace ```sh $
+viur cloud get {gcroles} ``` Scripts: - `gcroles` This function lets you get
+Roles for your google appengine Workspace in a readable .json Format ```sh $
+viur package {update|install} {vi|admin|scriptor|all} [profile] [version] ```
+Performs operations on packages Scripts: - `update` Updates an installed
+package - `install` Installs a declared package Options: - `vi` - `admin` -
+`scriptor` - `all` ```sh $ viur env ``` Show information about your current
+environment. ```sh $ viur project list ``` Pretty prints your `project.json`
+file on the console. ```sh $ viur update {requirements} ``` with this you can
+update your project specific requirements.txt file automatically ## The
+project.json The `project.json` is your core project configuration file for
+every viur related operation. It contains the default viur project profile and
+it can be expanded with several individual project profiles. ### Example
+project.json ```json lines { /* The format Key, Value pair defines the project
+json format, the viur-cli uses */ "format": "2.0.0", /* The first level
+contains of your profiles "default" is a profile, which is inherited by
+"develop" and "live" and can be customized for particular versions and/or GAE
+projects. Therefore, every profile can contain all keys from the "default"
+profile.*/ "default": { /* The builds level declares steps for the `viur build`
+command. It can contain viur components and other components that need to be
+build before project deployment */ "builds": { "admin": { "command": "viur
+install admin", "kind": "exec", "version": "4.0.8" }, "npm": { "command":
+"build", "kind": "npm", "source": "" } }, "gcloud": { "functions": { //
+Declarations for a cloud function "testfunction1": { "entry-point": "main",
+"env-vars-file": "env.yaml", "memory": "512MB", "runtime": "python311",
+"source": "deploy/cloudfunction/function1", "trigger": "http" } }, "max-
+instances": "1", "region": "europe-west3" }, "core": "3.5.1", // viur-core
+version of your project "distribution_folder": "./deploy", // Deploy folder
+uploaded to GAE "sources_folder": "./sources", "version": "live-$(year)-$
+(month)-$(day)", // Version string; Variables can be used here.
+"application_name": "my-live-app-viur3" // Name of the GAE project *4 },
+"develop": { "application_name": "my-dev-app-viur3", "version": "dev-$(user)" }
+} ``` ## Viur scripting interface There is a new core component that enables us
+to pull and push python scripts from/to a deployed application and run these in
+a sandbox or even locally. The GUI version is called scriptor and can be
+accessed via a webinterface, but viur-cli also has a cli for this: ```sh $ viur
+script {configure|pull|push|run|setup} ``` Manage your ViUR Scriptor Scripts
+via the CLI Commands: - `configure` Manage configuration settings. - `pull`
+Pull contents from server to working_dir. - `push` Push contents of working_dir
+to server. - `run` Locally run a script located in the working_dir. - `setup`
 Setup user session with a given username and... ## Packaged tools In order to
 use the packaged tools, you can run: ```sh $ viur tool {2to3|pyodide|ssl-fix}
 ``` Scripts: - `2to3` viur porting script - `pyodide` run the get_pyodide
 command - `ssl-fix` ssl fix for MacOS for example the 2to3 script helps porting
 viur2 project to viur3, it can be used to automatically rename some things that
 are deprecated in viur3 as well, so you can use it whenever a new core version
 is released for viur3 projects as well: ```sh $ viur tool 2to3 -d . ``` will
```

### Comparing `viur_cli-2.0.0rc5/src/viur_cli.egg-info/SOURCES.txt` & `viur_cli-2.0.0rc6/src/viur_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

