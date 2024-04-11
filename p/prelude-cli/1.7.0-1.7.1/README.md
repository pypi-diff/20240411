# Comparing `tmp/prelude-cli-1.7.0.tar.gz` & `tmp/prelude-cli-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.7.0.tar", last modified: Tue Mar 12 21:39:31 2024, max compression
+gzip compressed data, was "prelude-cli-1.7.1.tar", last modified: Thu Apr 11 20:57:01 2024, max compression
```

## Comparing `prelude-cli-1.7.0.tar` & `prelude-cli-1.7.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-03-12 21:39:31.588315 prelude-cli-1.7.0/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.7.0/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.7.0/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      909 2024-03-12 21:39:31.588250 prelude-cli-1.7.0/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.7.0/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-03-12 21:39:31.584323 prelude-cli-1.7.0/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.0/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      940 2023-12-14 20:44:38.000000 prelude-cli-1.7.0/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-12-08 16:31:30.000000 prelude-cli-1.7.0/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-03-12 21:39:31.585782 prelude-cli-1.7.0/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)     1120 2024-01-05 14:14:44.000000 prelude-cli-1.7.0/prelude_cli/templates/README.md
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.0/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      261 2024-01-05 14:14:44.000000 prelude-cli-1.7.0/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-03-12 21:39:31.587788 prelude-cli-1.7.0/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.0/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     6838 2024-03-12 19:51:09.000000 prelude-cli-1.7.0/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.7.0/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     9235 2024-03-12 19:51:09.000000 prelude-cli-1.7.0/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     8143 2024-01-05 14:14:44.000000 prelude-cli-1.7.0/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     4168 2023-12-08 16:31:30.000000 prelude-cli-1.7.0/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)      658 2023-12-08 16:31:30.000000 prelude-cli-1.7.0/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-03-12 21:39:31.588062 prelude-cli-1.7.0/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      909 2024-03-12 21:39:31.000000 prelude-cli-1.7.0/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      630 2024-03-12 21:39:31.000000 prelude-cli-1.7.0/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2024-03-12 21:39:31.000000 prelude-cli-1.7.0/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2024-03-12 21:39:31.000000 prelude-cli-1.7.0/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       32 2024-03-12 21:39:31.000000 prelude-cli-1.7.0/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2024-03-12 21:39:31.000000 prelude-cli-1.7.0/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.7.0/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      663 2024-03-12 21:39:31.588577 prelude-cli-1.7.0/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 20:57:01.202824 prelude-cli-1.7.1/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.7.1/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.7.1/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      909 2024-04-11 20:57:01.202717 prelude-cli-1.7.1/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.7.1/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 20:57:01.196599 prelude-cli-1.7.1/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.1/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1014 2024-04-03 22:19:39.000000 prelude-cli-1.7.1/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-12-08 16:31:30.000000 prelude-cli-1.7.1/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 20:57:01.198422 prelude-cli-1.7.1/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)     1120 2024-01-05 14:14:44.000000 prelude-cli-1.7.1/prelude_cli/templates/README.md
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.1/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      261 2024-01-05 14:14:44.000000 prelude-cli-1.7.1/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 20:57:01.201673 prelude-cli-1.7.1/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.1/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)    10043 2024-04-03 22:19:39.000000 prelude-cli-1.7.1/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.7.1/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)    10050 2024-04-11 16:14:14.000000 prelude-cli-1.7.1/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     2543 2024-04-11 19:46:08.000000 prelude-cli-1.7.1/prelude_cli/views/generate.py
+-rw-r--r--   0 pack       (501) staff       (20)     8143 2024-01-05 14:14:44.000000 prelude-cli-1.7.1/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     4674 2024-03-21 18:38:20.000000 prelude-cli-1.7.1/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)      662 2024-04-03 22:19:39.000000 prelude-cli-1.7.1/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 20:57:01.202368 prelude-cli-1.7.1/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      909 2024-04-11 20:57:01.000000 prelude-cli-1.7.1/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      660 2024-04-11 20:57:01.000000 prelude-cli-1.7.1/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2024-04-11 20:57:01.000000 prelude-cli-1.7.1/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2024-04-11 20:57:01.000000 prelude-cli-1.7.1/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       32 2024-04-11 20:57:01.000000 prelude-cli-1.7.1/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2024-04-11 20:57:01.000000 prelude-cli-1.7.1/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.7.1/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      663 2024-04-11 20:57:01.203155 prelude-cli-1.7.1/setup.cfg
```

### Comparing `prelude-cli-1.7.0/LICENSE` & `prelude-cli-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.0/PKG-INFO` & `prelude-cli-1.7.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.7.0
+Version: 1.7.1
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prelude-sdk==1.7.0
+Requires-Dist: prelude-sdk==1.7.1
 Requires-Dist: click>8
 Requires-Dist: rich
 
 # Prelude CLI
 
 Interact with the full range of features in Prelude Detect, organized by:
```

### Comparing `prelude-cli-1.7.0/prelude_cli/cli.py` & `prelude-cli-1.7.1/prelude_cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import click
 
-from prelude_cli.views.iam import iam
 from prelude_cli.views.build import build
+from prelude_cli.views.configure import configure
 from prelude_cli.views.detect import detect
+from prelude_cli.views.generate import generate
+from prelude_cli.views.iam import iam
 from prelude_cli.views.partner import partner
 from prelude_sdk.models.account import Account
-from prelude_cli.views.configure import configure
 
 
 def complete_profile(ctx, param, incomplete):
     return [x for x in Account().read_keychain_config() if x.startswith(incomplete)]
 
 @click.group(invoke_without_command=True)
 @click.version_option()
@@ -22,11 +23,12 @@
 
 
 cli.add_command(iam)
 cli.add_command(configure)
 cli.add_command(detect)
 cli.add_command(build)
 cli.add_command(partner)
+cli.add_command(generate)
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `prelude-cli-1.7.0/prelude_cli/templates/README.md` & `prelude-cli-1.7.1/prelude_cli/templates/README.md`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.0/prelude_cli/views/build.py` & `prelude-cli-1.7.1/prelude_cli/views/build.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import importlib.resources as pkg_resources
+import json
+import os
 import re
 import uuid
-import click
-import prelude_cli.templates as templates
-import importlib.resources as pkg_resources
+from datetime import datetime, timezone
+from pathlib import Path, PurePath
 
+import click
 from rich import print_json
-from pathlib import Path, PurePath
-from datetime import datetime, timezone
 
+import prelude_cli.templates as templates
 from prelude_cli.views.shared import handle_api_error, Spinner
 from prelude_sdk.controllers.build_controller import BuildController
+from prelude_sdk.models.codes import Control
 
 
 UUID = re.compile('[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}')
 
 
 @click.group()
 @click.pass_context
@@ -129,33 +132,51 @@
                 upload(p=Path(obj))
             except ValueError as e:
                 click.secho(e.args[0], fg='red')
 
 
 @build.command('create-threat')
 @click.argument('name')
+@click.option('-p', '--published', help='date the threat was published', required=True, type=str)
 @click.option('--id', help='identifier', type=str)
 @click.option('-s', '--source', help='source of threat (ex. www.cisa.gov)', default=None, type=str)
 @click.option('-i', '--source_id', help='ID of the threat, per the source (ex. aa23-075a)', default=None, type=str)
-@click.option('-p', '--published', help='date the threat was published', default=None, type=str)
 @click.option('-t', '--tests', help='comma-separated list of test IDs', default=None, type=str)
+@click.option('-d', '--directory', help='directory containing tests and IOAs generated from threat_intel', default=None, type=click.Path(exists=True, dir_okay=True, file_okay=False))
 @click.pass_obj
 @handle_api_error
-def create_threat(controller, name, id, source_id, source, published, tests):
+def create_threat(controller, name, published, id, source_id, source, tests, directory):
     """ Create a security threat """
     with Spinner(description='Creating new threat'):
-        t = controller.create_threat(
-            name=name,
-            threat_id=id,
-            source_id=source_id,
-            source=source,
-            published=published,
-            tests=tests
-        )
-    print_json(data=t)
+        try:
+            created_tests = list()
+            uploads = list()
+            threat = None
+            if directory:
+                for technique_dir in os.listdir(directory):
+                    with open(f'{directory}/{technique_dir}/test.go', 'r') as f:
+                        go_code = f.read()
+                    with open(f'{directory}/{technique_dir}/config.json', 'r') as f:
+                        config = json.load(f)
+                    test = controller.create_test(name=config['name'], unit=config['unit'], technique=config['technique'])
+                    created_tests.append(test)
+                    uploads.append(controller.upload(test_id=test['id'], filename=f'{test["id"]}.go', data=go_code.encode()))
+                tests = ','.join([t['id'] for t in created_tests])
+            threat = controller.create_threat(
+                name=name,
+                threat_id=id,
+                source_id=source_id,
+                source=source,
+                published=published,
+                tests=tests,
+            )
+        except FileNotFoundError as e:
+            raise Exception(e)
+        finally:
+            print_json(data=dict(threat=threat, created_tests=created_tests, uploads=uploads))
 
 
 @build.command('update-threat')
 @click.argument('threat')
 @click.option('-n', '--name', help='test name', default=None, type=str)
 @click.option('-s', '--source', help='source of threat (ex. www.cisa.gov)', default=None, type=str)
 @click.option('-i', '--source_id', help='ID of the threat, per the source (ex. aa23-075a)', default=None, type=str)
@@ -184,7 +205,60 @@
 @click.pass_obj
 @handle_api_error
 def delete_threat(controller, threat, purge):
     """ Delete a threat """
     with Spinner(description='Removing threat'):
         data = controller.delete_threat(threat_id=threat, purge=purge)
     print_json(data=data)
+
+
+@build.command('create-detection')
+@click.argument('sigma_rule_file', type=click.Path(exists=True, dir_okay=False))
+@click.option('-t', '--test', help='ID of the test this detection is for', required=True, type=str)
+@click.option('--detection_id', help='detection ID', default=None, type=str)
+@click.option('--rule_id', help='rule ID', default=None, type=str)
+@click.pass_obj
+@handle_api_error
+def create_detection(controller, sigma_rule_file, test, detection_id, rule_id):
+    """ Create a detection rule """
+    with Spinner(description='Creating new detection'):
+        with open(sigma_rule_file, 'r') as f:
+            rule = f.read()
+        t = controller.create_detection(
+            rule=rule,
+            test_id=test,
+            detection_id=detection_id,
+            rule_id=rule_id
+        )
+    print_json(data=t)
+
+
+@build.command('update-detection')
+@click.argument('detection')
+@click.option('--sigma_rule_file', help='Sigma rule, from a yaml file',
+              default=None, type=click.Path(exists=True, dir_okay=False))
+@click.option('-t', '--test', help='ID of the test this detection is for', default=None, type=str)
+@click.pass_obj
+@handle_api_error
+def update_detection(controller, detection, sigma_rule_file, test):
+    """ Update a detection """
+    with Spinner(description='Updating detection'):
+        with open(sigma_rule_file, 'r') as f:
+            rule = f.read()
+        data = controller.update_detection(
+            rule=rule,
+            test_id=test,
+            detection_id=detection,
+        )
+    print_json(data=data)
+
+
+@build.command('delete-detection')
+@click.argument('detection')
+@click.confirmation_option(prompt='Are you sure?')
+@click.pass_obj
+@handle_api_error
+def delete_detection(controller, detection):
+    """ Delete a detection """
+    with Spinner(description='Removing detection'):
+        data = controller.delete_detection(detection_id=detection)
+    print_json(data=data)
```

### Comparing `prelude-cli-1.7.0/prelude_cli/views/configure.py` & `prelude-cli-1.7.1/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.0/prelude_cli/views/detect.py` & `prelude-cli-1.7.1/prelude_cli/views/detect.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import asyncio
 import click
-import asyncio 
 
-from rich import print_json
+from datetime import datetime, time, timedelta, timezone
+from dateutil.parser import parse
 from pathlib import Path, PurePath
-from datetime import datetime, timedelta, timezone, time
+from rich import print_json
 
-from prelude_sdk.models.codes import RunCode, Control
 from prelude_cli.views.shared import handle_api_error, Spinner
-from prelude_sdk.controllers.iam_controller import IAMController
 from prelude_sdk.controllers.detect_controller import DetectController
+from prelude_sdk.controllers.iam_controller import IAMController
+from prelude_sdk.models.codes import RunCode, Control
 
 
 @click.group()
 @click.pass_context
 def detect(ctx):
     """ Continuous security testing """
     ctx.obj = DetectController(account=ctx.obj)
@@ -67,15 +68,15 @@
         data = controller.get_test(test_id=test_id)
     print_json(data=data)
 
 
 @detect.command('threats')
 @click.pass_obj
 @handle_api_error
-def threats(controller):
+def list_threats(controller):
     """ List all Prelude threats """
     with Spinner(description='Fetching threats'):
         data = controller.list_threats()
     print_json(data=data)
 
 
 @detect.command('threat')
@@ -85,14 +86,35 @@
 def get_threat(controller, threat_id):
     """ List properties for a threat """
     with Spinner(description='Fetching data for threat'):
         data = controller.get_threat(threat_id=threat_id)
     print_json(data=data)
 
 
+@detect.command('detections')
+@click.pass_obj
+@handle_api_error
+def list_detections(controller):
+    """ List all Prelude detections """
+    with Spinner(description='Fetching detections'):
+        data = controller.list_detections()
+    print_json(data=data)
+
+
+@detect.command('detection')
+@click.argument('detection_id')
+@click.pass_obj
+@handle_api_error
+def get_detection(controller, detection_id):
+    """ List properties for a detection """
+    with Spinner(description='Fetching data for detection'):
+        data = controller.get_detection(detection_id=detection_id)
+    print_json(data=data)
+
+
 @detect.command('download')
 @click.argument('test')
 @click.pass_obj
 @handle_api_error
 def download(controller, test):
     """ Download a test to your local environment """
     click.secho(f'Downloading {test}')
@@ -119,15 +141,15 @@
 @handle_api_error
 def schedule(controller, id, type, run_code, tags):
     """ Add test or threat to your queue """
     with Spinner(description=f'Scheduling {type.lower()}'):
         if type == 'TEST':
             data = controller.schedule([dict(test_id=id, run_code=run_code, tags=tags)])
         else:
-            data = controller.schedule([dict(test_id=id, run_code=run_code, tags=tags)])
+            data = controller.schedule([dict(threat_id=id, run_code=run_code, tags=tags)])
     print_json(data=data)
 
 
 @detect.command('unschedule')
 @click.argument('id')
 @click.option('-t', '--type', help='whether you are unscheduling a test or threat', required=True,
               type=click.Choice(['TEST', 'THREAT'], case_sensitive=False))
@@ -204,30 +226,33 @@
 
 @detect.command('activity')
 @click.option('--view',
               help='retrieve a specific result view',
               default='logs', show_default=True,
               type=click.Choice(['endpoints', 'findings', 'logs', 'metrics', 'protected', 'techniques', 'tests', 'threats']))
 @click.option('--control', type=click.Choice([c.name for c in Control], case_sensitive=False))
-@click.option('--days', help='days to look back (max: 29)', default=29, type=int)
 @click.option('--dos', help='comma-separated list of DOS', type=str)
 @click.option('--endpoints', help='comma-separated list of endpoint IDs', type=str)
+@click.option('--finish', help='end date of activity (end of day)', type=str)
 @click.option('--os', help='comma-separated list of OS', type=str)
 @click.option('--policy', help='comma-separated list of policies', type=str)
 @click.option('--social', help='whether to fetch account-specific or social stats. Applicable to the following views: protected', is_flag=True)
+@click.option('--start', help='start date of activity (beginning of day)', type=str)
 @click.option('--techniques', help='comma-separated list of techniques', type=str)
 @click.option('--tests', help='comma-separated list of test IDs', type=str)
 @click.option('--threats', help='comma-separated list of threat IDs', type=str)
 @click.pass_obj
 @handle_api_error
-def describe_activity(controller, control, days, dos, endpoints, os, policy, social, techniques, tests, threats, view):
+def describe_activity(controller, control, dos, endpoints, finish, os, policy, social, start, techniques, tests, threats, view):
     """ View my Detect results """
+    start = parse(start) if start else datetime.now(timezone.utc) - timedelta(days=29)
+    finish = parse(finish) if finish else datetime.now(timezone.utc)
     filters = dict(
-        start=datetime.combine(datetime.now(timezone.utc) - timedelta(days=min(days, 29)), time.min),
-        finish=datetime.combine(datetime.now(timezone.utc), time.max)
+        start=datetime.combine(start, time.min),
+        finish=datetime.combine(finish, time.max)
     )
     if control:
         filters['control'] = Control[control.upper()].value
     if dos:
         filters['dos'] = dos
     if endpoints:
         filters['endpoints'] = endpoints
```

### Comparing `prelude-cli-1.7.0/prelude_cli/views/iam.py` & `prelude-cli-1.7.1/prelude_cli/views/iam.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.0/prelude_cli/views/partner.py` & `prelude-cli-1.7.1/prelude_cli/views/partner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import click
-
 from rich import print_json
 
-from prelude_sdk.models.codes import Control
 from prelude_cli.views.shared import handle_api_error, Spinner
 from prelude_sdk.controllers.partner_controller import PartnerController
+from prelude_sdk.models.codes import Control
 
 
 @click.group()
 @click.pass_context
 def partner(ctx):
     """ Partner system commands """
     ctx.obj = PartnerController(account=ctx.obj)
@@ -89,7 +88,19 @@
 @handle_api_error
 def generate_webhook(controller, partner):
     """ Generate webhook credentials for an EDR system to enable the forwarding of alerts to the Prelude API, facilitating automatic alert suppression """
     with Spinner(description='Generating webhook credentials'):
         data = controller.generate_webhook(partner=Control[partner])
     print_json(data=data)
     print("\nVisit https://docs.preludesecurity.com/docs/alert-management for details on configuring your EDR to forward alerts.\n")
+
+
+@partner.command('reports')
+@click.argument('partner', type=click.Choice([Control.CROWDSTRIKE.name], case_sensitive=False))
+@click.option('-t', '--test_id', required=True, help='test to get reports for')
+@click.pass_obj
+@handle_api_error
+def partner_reports(controller, partner, test_id):
+    """ Get reports to a partner for a test """
+    with Spinner(description='Getting reports to partner'):
+        data = controller.list_reports(partner=Control[partner], test_id=test_id)
+    print_json(data=data)
```

### Comparing `prelude-cli-1.7.0/prelude_cli/views/shared.py` & `prelude-cli-1.7.1/prelude_cli/views/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,12 @@
     return handler
 
 
 class Spinner(Progress): 
     def __init__(self, description='Loading'): 
         super().__init__(
             SpinnerColumn(style='green', spinner_name='line'),
-            TextColumn(f'[green]{description}...'),
+            TextColumn('[green]{task.description}...'),
             transient=True, 
             refresh_per_second=10
         )
         self.add_task(description)
```

### Comparing `prelude-cli-1.7.0/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.7.1/prelude_cli.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.7.0
+Version: 1.7.1
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prelude-sdk==1.7.0
+Requires-Dist: prelude-sdk==1.7.1
 Requires-Dist: click>8
 Requires-Dist: rich
 
 # Prelude CLI
 
 Interact with the full range of features in Prelude Detect, organized by:
```

### Comparing `prelude-cli-1.7.0/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.7.1/prelude_cli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,10 +15,11 @@
 prelude_cli/templates/README.md
 prelude_cli/templates/__init__.py
 prelude_cli/templates/template.go
 prelude_cli/views/__init__.py
 prelude_cli/views/build.py
 prelude_cli/views/configure.py
 prelude_cli/views/detect.py
+prelude_cli/views/generate.py
 prelude_cli/views/iam.py
 prelude_cli/views/partner.py
 prelude_cli/views/shared.py
```

### Comparing `prelude-cli-1.7.0/setup.cfg` & `prelude-cli-1.7.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.7.0
+version = 1.7.1
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.7.0
+	prelude-sdk == 1.7.1
 	click > 8
 	rich
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

