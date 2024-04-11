# Comparing `tmp/diracx-cli-0.0.1a8.tar.gz` & `tmp/diracx-cli-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diracx-cli-0.0.1a8.tar", last modified: Thu Nov 30 08:39:48 2023, max compression
+gzip compressed data, was "diracx-cli-0.0.1a9.tar", last modified: Sun Jan 28 09:11:36 2024, max compression
```

## Comparing `diracx-cli-0.0.1a8.tar` & `diracx-cli-0.0.1a9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:48.109117 diracx-cli-0.0.1a8/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-11-30 08:39:48.109117 diracx-cli-0.0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-30 08:39:48.109117 diracx-cli-0.0.1a8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:48.105117 diracx-cli-0.0.1a8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:48.105117 diracx-cli-0.0.1a8/src/diracx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:48.105117 diracx-cli-0.0.1a8/src/diracx/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/src/diracx/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/src/diracx/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:48.105117 diracx-cli-0.0.1a8/src/diracx/cli/internal/
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/src/diracx/cli/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9720 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/src/diracx/cli/internal/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/src/diracx/cli/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/src/diracx/cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/src/diracx/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:48.109117 diracx-cli-0.0.1a8/src/diracx_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-11-30 08:39:48.000000 diracx-cli-0.0.1a8/src/diracx_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-11-30 08:39:48.000000 diracx-cli-0.0.1a8/src/diracx_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 08:39:48.000000 diracx-cli-0.0.1a8/src/diracx_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-30 08:39:48.000000 diracx-cli-0.0.1a8/src/diracx_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-30 08:39:48.000000 diracx-cli-0.0.1a8/src/diracx_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-30 08:39:48.000000 diracx-cli-0.0.1a8/src/diracx_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:48.105117 diracx-cli-0.0.1a8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:48.105117 diracx-cli-0.0.1a8/tests/legacy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:48.109117 diracx-cli-0.0.1a8/tests/legacy/cs_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/tests/legacy/cs_sync/convert_integration_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    58102 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/tests/legacy/cs_sync/integration_test.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    27569 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/tests/legacy/cs_sync/integration_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/tests/legacy/cs_sync/integration_test_secret.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/tests/legacy/cs_sync/test_cssync.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/tests/legacy/test_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/tests/test_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2023-11-30 08:39:21.000000 diracx-cli-0.0.1a8/tests/test_login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:36.169114 diracx-cli-0.0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-28 09:11:36.169114 diracx-cli-0.0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 09:11:36.169114 diracx-cli-0.0.1a9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:36.165114 diracx-cli-0.0.1a9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:36.165114 diracx-cli-0.0.1a9/src/diracx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:36.165114 diracx-cli-0.0.1a9/src/diracx/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/src/diracx/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/src/diracx/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:36.165114 diracx-cli-0.0.1a9/src/diracx/cli/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/src/diracx/cli/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10847 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/src/diracx/cli/internal/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/src/diracx/cli/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/src/diracx/cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/src/diracx/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:36.169114 diracx-cli-0.0.1a9/src/diracx_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-28 09:11:36.000000 diracx-cli-0.0.1a9/src/diracx_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-28 09:11:36.000000 diracx-cli-0.0.1a9/src/diracx_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 09:11:36.000000 diracx-cli-0.0.1a9/src/diracx_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-28 09:11:36.000000 diracx-cli-0.0.1a9/src/diracx_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-28 09:11:36.000000 diracx-cli-0.0.1a9/src/diracx_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 09:11:36.000000 diracx-cli-0.0.1a9/src/diracx_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:36.169114 diracx-cli-0.0.1a9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:36.169114 diracx-cli-0.0.1a9/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:36.169114 diracx-cli-0.0.1a9/tests/legacy/cs_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)    59129 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/tests/legacy/cs_sync/integration_test.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    27944 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/tests/legacy/cs_sync/integration_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/tests/legacy/cs_sync/integration_test_buggy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/tests/legacy/cs_sync/integration_test_secret.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/tests/legacy/cs_sync/test_cssync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/tests/legacy/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/tests/test_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-01-28 09:11:11.000000 diracx-cli-0.0.1a9/tests/test_login.py
```

### Comparing `diracx-cli-0.0.1a8/PKG-INFO` & `diracx-cli-0.0.1a9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diracx-cli
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: TODO
 License: GPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
```

### Comparing `diracx-cli-0.0.1a8/pyproject.toml` & `diracx-cli-0.0.1a9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -51,7 +51,10 @@
 addopts = [
     "-v",
     "--cov=diracx.cli", "--cov-report=term-missing",
     "-pdiracx.testing",
     "--import-mode=importlib",
 ]
 asyncio_mode = "auto"
+markers = [
+    "enabled_dependencies: List of dependencies which should be available to the FastAPI test client",
+]
```

### Comparing `diracx-cli-0.0.1a8/src/diracx/cli/__init__.py` & `diracx-cli-0.0.1a9/src/diracx/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import json
 import os
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from typing import Annotated, Optional
 
 import typer
 
 from diracx.client.aio import DiracClient
 from diracx.client.models import DeviceFlowErrorResponse
 from diracx.core.preferences import get_diracx_preferences
@@ -54,16 +54,18 @@
     async with DiracClient() as api:
         data = await api.auth.initiate_device_flow(
             client_id=api.client_id,
             audience="Dirac server",
             scope=" ".join(scopes),
         )
         print("Now go to:", data.verification_uri_complete)
-        expires = datetime.now() + timedelta(seconds=data.expires_in - 30)
-        while expires > datetime.now():
+        expires = datetime.now(tz=timezone.utc) + timedelta(
+            seconds=data.expires_in - 30
+        )
+        while expires > datetime.now(tz=timezone.utc):
             print(".", end="", flush=True)
             response = await api.auth.token(device_code=data.device_code, client_id=api.client_id)  # type: ignore
             if isinstance(response, DeviceFlowErrorResponse):
                 if response.error == "authorization_pending":
                     # TODO: Setting more than 5 seconds results in an error
                     # Related to keep-alive disconnects from uvicon (--timeout-keep-alive)
                     await asyncio.sleep(2)
```

### Comparing `diracx-cli-0.0.1a8/src/diracx/cli/internal/__init__.py` & `diracx-cli-0.0.1a9/src/diracx/cli/internal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
     config = Config(
         Registry={},
         DIRAC=DIRACConfig(),
         Operations={"Defaults": OperationsConfig()},
     )
 
+    git.Repo.init(repo_path, initial_branch="master")
     update_config_and_commit(
         repo_path=repo_path, config=config, message="Initial commit"
     )
     typer.echo(f"Successfully created repo in {config_repo}", err=True)
 
 
 @app.command()
@@ -176,13 +177,13 @@
         message=f"Added user {sub} ({preferred_username}) to vo {vo} and groups {groups}",
     )
     typer.echo(f"Successfully added user to {config_repo}", err=True)
 
 
 def update_config_and_commit(repo_path: Path, config: Config, message: str):
     """Update the yaml file in the repo and commit it"""
-    repo = git.Repo.init(repo_path)
+    repo = git.Repo(repo_path)
     yaml_path = repo_path / "default.yml"
     typer.echo(f"Writing back configuration to {yaml_path}", err=True)
     yaml_path.write_text(yaml.safe_dump(config.dict(exclude_unset=True)))
     repo.index.add([yaml_path.relative_to(repo_path)])
     repo.index.commit(message)
```

### Comparing `diracx-cli-0.0.1a8/src/diracx/cli/internal/legacy.py` & `diracx-cli-0.0.1a9/src/diracx/cli/internal/legacy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import base64
 import hashlib
 import json
 import os
 from pathlib import Path
-from typing import cast
+from typing import TYPE_CHECKING, cast
 from urllib.parse import urljoin, urlparse
 
 import diraccfg
 import typer
 import yaml
+
+if TYPE_CHECKING:
+    from diraccfg.cfg import CFGAsDict
+
 from pydantic import BaseModel
 from typer import Option
 
 from diracx.core.config import Config
 from diracx.core.config.schema import Field, SupportInfo
 
 from ..utils import AsyncTyper
@@ -44,37 +48,49 @@
 #     args = parser.parse_args()
 
 
 #     main(args.old_file, args.conversion_config, args.repo / DEFAULT_CONFIG_FILE)
 
 
 @app.command()
-def cs_sync(old_file: Path, conversion_config: Path, new_file: Path):
+def cs_sync(old_file: Path, new_file: Path):
     """Load the old CS and convert it to the new YAML format"""
     if not os.environ.get("DIRAC_COMPAT_ENABLE_CS_CONVERSION"):
         raise RuntimeError(
             "DIRAC_COMPAT_ENABLE_CS_CONVERSION must be set for the conversion to be possible"
         )
 
     old_data = old_file.read_text()
     cfg = diraccfg.CFG().loadFromBuffer(old_data)
     raw = cfg.getAsDict()
 
-    _apply_fixes(raw, conversion_config)
+    diracx_section = cast("CFGAsDict", raw["DiracX"])
+    # DisabledVOs cannot be set if any Legacy clients are enabled
+    disabled_vos = diracx_section.get("DisabledVOs")
+    enabled_clients = []
+    for _, client_status in cast(
+        "CFGAsDict", diracx_section.get("LegacyClientEnabled", {})
+    ).items():
+        for _, str_status in cast("CFGAsDict", client_status).items():
+            enabled_clients.append(str_status == "True")
+    if disabled_vos and any(enabled_clients):
+        raise RuntimeError(
+            "DisabledVOs cannot be set if any Legacy clients are enabled"
+        )
+
+    _apply_fixes(raw)
 
     config = Config.parse_obj(raw)
     new_file.write_text(yaml.safe_dump(config.dict(exclude_unset=True)))
 
 
-def _apply_fixes(raw, conversion_config: Path):
+def _apply_fixes(raw):
     """Modify raw in place to make any layout changes between the old and new structure"""
 
-    conv_config = ConversionConfig.parse_obj(
-        yaml.safe_load(conversion_config.read_text())
-    )
+    conv_config = ConversionConfig.parse_obj(raw["DiracX"]["CsSync"])
 
     raw.pop("DiracX", None)
     # Remove dips specific parts from the CS
     raw["DIRAC"].pop("Extensions", None)
     raw["DIRAC"].pop("Framework", None)
     raw["DIRAC"].pop("Security", None)
 
@@ -113,14 +129,18 @@
             raw["Registry"][vo]["DefaultStorageQuota"] = original_registry[
                 "DefaultStorageQuota"
             ]
         if "DefaultProxyLifeTime" in original_registry:
             raw["Registry"][vo]["DefaultProxyLifeTime"] = original_registry[
                 "DefaultProxyLifeTime"
             ]
+        # Copy over the necessary parts of the VO section
+        for key in {"VOMSName"}:
+            if key in original_registry.get("VO", {}).get(vo, {}):
+                raw["Registry"][vo][key] = original_registry["VO"][vo][key]
         # Find the groups that belong to this VO
         vo_users = set()
         for name, info in original_registry["Groups"].items():
             if "VO" not in info:
                 print(
                     f"Can't convert group {name} because it is not associated to any VO"
                 )
@@ -139,16 +159,22 @@
         # Find the users that belong to this VO
         for name, info in original_registry["Users"].items():
             if name in vo_users:
                 if subject := vo_meta.UserSubjects.get(name):
                     raw["Registry"][vo]["Users"][subject] = info | {
                         "PreferedUsername": name
                     }
-                    # We ignore the DN and CA
-                    raw["Registry"][vo]["Users"][subject].pop("DN", None)
+                    # Strip any DNs which are from the failed OAuth2 attempt
+                    raw_dn = raw["Registry"][vo]["Users"][subject].pop("DN", None)
+                    raw["Registry"][vo]["Users"][subject]["DNs"] = [
+                        dn.strip()
+                        for dn in raw_dn.split(",")
+                        if not dn.strip().startswith("/O=DIRAC/")
+                    ]
+                    # We ignore the CA
                     raw["Registry"][vo]["Users"][subject].pop("CA", None)
 
 
 @app.command()
 def generate_helm_values(
     public_cfg: Path = Option(help="Path to the cfg file served by the CS"),
     secret_cfg: Path = Option(
```

### Comparing `diracx-cli-0.0.1a8/src/diracx/cli/jobs.py` & `diracx-cli-0.0.1a9/src/diracx/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `diracx-cli-0.0.1a8/src/diracx_cli.egg-info/PKG-INFO` & `diracx-cli-0.0.1a9/src/diracx_cli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diracx-cli
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: TODO
 License: GPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
```

### Comparing `diracx-cli-0.0.1a8/src/diracx_cli.egg-info/SOURCES.txt` & `diracx-cli-0.0.1a9/src/diracx_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 src/diracx_cli.egg-info/entry_points.txt
 src/diracx_cli.egg-info/requires.txt
 src/diracx_cli.egg-info/top_level.txt
 tests/test_internal.py
 tests/test_jobs.py
 tests/test_login.py
 tests/legacy/test_legacy.py
-tests/legacy/cs_sync/convert_integration_test.yaml
 tests/legacy/cs_sync/integration_test.cfg
 tests/legacy/cs_sync/integration_test.yaml
+tests/legacy/cs_sync/integration_test_buggy.cfg
 tests/legacy/cs_sync/integration_test_secret.cfg
 tests/legacy/cs_sync/test_cssync.py
```

### Comparing `diracx-cli-0.0.1a8/tests/legacy/cs_sync/integration_test.cfg` & `diracx-cli-0.0.1a9/tests/legacy/cs_sync/integration_test.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,57 @@
     }
   }
 }
 DiracX
 {
   URL = https://dirac-integration-tests.invalid:1234
   LegacyExchangeApiKey = diracx:legacy:ChangeME
+
+  CsSync
+  {
+    VOs
+    {
+      Jenkins
+      {
+        DefaultGroup = jenkins_user
+        IdP
+        {
+          ClientID = 995ed3b9-d5bd-49d3-a7f4-7fc7dbd5a0cd
+          URL = https://jenkins.invalid/
+        }
+        UserSubjects
+        {
+          adminusername = e2cb28ec-1a1e-40ee-a56d-d899b79879ce
+          ciuser = 26dbe36e-cf5c-4c52-a834-29a1c904ef74
+          trialUser = a95ab678-3fa4-41b9-b863-fe62ce8064ce
+        }
+        Support
+        {
+          Message = Contact the help desk
+          Email = helpdesk@example.invalid
+          Webpage = https://helpdesk.vo.invalid
+        }
+      }
+      vo
+      {
+        DefaultGroup = dirac_user
+        IdP
+        {
+          ClientID = 072afab5-ed92-46e0-a61d-4ecbc96e0770
+          URL = https://vo.invalid/
+        }
+        UserSubjects
+        {
+          adminusername = 26b14fc9-6d40-4ca5-b014-6234eaf0fb6e
+          ciuser = d3adc733-6588-4d6f-8581-5986b02d0c87
+          trialUser = ff2152ff-34f4-4739-b106-3def37e291e3
+        }
+      }
+    }
+  }
 }
 Systems
 {
   Configuration
   {
     Production
     {
```

### Comparing `diracx-cli-0.0.1a8/tests/legacy/cs_sync/integration_test.yaml` & `diracx-cli-0.0.1a9/tests/legacy/cs_sync/integration_test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -66,27 +66,34 @@
           26dbe36e-cf5c-4c52-a834-29a1c904ef74: null
           a95ab678-3fa4-41b9-b863-fe62ce8064ce: null
           e2cb28ec-1a1e-40ee-a56d-d899b79879ce: null
     IdP:
       ClientID: 995ed3b9-d5bd-49d3-a7f4-7fc7dbd5a0cd
       URL: https://jenkins.invalid/
     Support:
-      Email: "helpdesk@example.invalid"
-      Message: "Contact the help desk"
-      Webpage: "https://helpdesk.vo.invalid"
+      Email: helpdesk@example.invalid
+      Message: Contact the help desk
+      Webpage: https://helpdesk.vo.invalid
     Users:
       26dbe36e-cf5c-4c52-a834-29a1c904ef74:
+        DNs:
+        - /C=ch/O=DIRAC/OU=DIRAC CI/CN=ciuser
         Email: lhcb-dirac-ci@cern.ch
         PreferedUsername: ciuser
       a95ab678-3fa4-41b9-b863-fe62ce8064ce:
+        DNs:
+        - /C=ch/O=DIRAC/OU=DIRAC CI/CN=trialUser
         Email: lhcb-dirac-ci@cern.ch
         PreferedUsername: trialUser
       e2cb28ec-1a1e-40ee-a56d-d899b79879ce:
+        DNs:
+        - /C=ch/O=DIRAC/OU=DIRAC CI/CN=ciuser
         Email: lhcb-dirac-ci@cern.ch
         PreferedUsername: adminusername
+    VOMSName: myVOMS
   vo:
     DefaultGroup: dirac_user
     Groups:
       dirac_admin:
         Properties: !!set
           AlarmsManagement: null
           CSAdministrator: null
@@ -106,20 +113,26 @@
           ff2152ff-34f4-4739-b106-3def37e291e3: null
     IdP:
       ClientID: 072afab5-ed92-46e0-a61d-4ecbc96e0770
       URL: https://vo.invalid/
     Support: {}
     Users:
       26b14fc9-6d40-4ca5-b014-6234eaf0fb6e:
+        DNs:
+        - /C=ch/O=DIRAC/OU=DIRAC CI/CN=ciuser
         Email: lhcb-dirac-ci@cern.ch
         PreferedUsername: adminusername
       d3adc733-6588-4d6f-8581-5986b02d0c87:
+        DNs:
+        - /C=ch/O=DIRAC/OU=DIRAC CI/CN=ciuser
         Email: lhcb-dirac-ci@cern.ch
         PreferedUsername: ciuser
       ff2152ff-34f4-4739-b106-3def37e291e3:
+        DNs:
+        - /C=ch/O=DIRAC/OU=DIRAC CI/CN=trialUser
         Email: lhcb-dirac-ci@cern.ch
         PreferedUsername: trialUser
 Resources:
   FTSEndpoints:
     FTS3:
       JENKINS-FTS3: https://jenkins-fts3.cern.ch:8446
   FileCatalogs:
```

### Comparing `diracx-cli-0.0.1a8/tests/legacy/cs_sync/integration_test_secret.cfg` & `diracx-cli-0.0.1a9/tests/legacy/cs_sync/integration_test_secret.cfg`

 * *Files identical despite different names*

### Comparing `diracx-cli-0.0.1a8/tests/legacy/test_legacy.py` & `diracx-cli-0.0.1a9/tests/legacy/test_legacy.py`

 * *Files identical despite different names*

### Comparing `diracx-cli-0.0.1a8/tests/test_internal.py` & `diracx-cli-0.0.1a9/tests/test_internal.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,87 @@
 from __future__ import annotations
 
+import shutil
+
 import pytest
 from typer.testing import CliRunner
 
 from diracx.cli import app
 from diracx.core.config import ConfigSource
 
 runner = CliRunner()
 
-
-@pytest.mark.parametrize("protocol", [None, "git+file://"])
-def test_generate_cs(tmp_path, protocol):
-    cs_repo = f"{tmp_path}"
-    if protocol is None:
-        cs_repo = f"git+file://{cs_repo}"
-
-    result = runner.invoke(app, ["internal", "generate-cs", cs_repo])
-    assert result.exit_code == 0
-    assert (tmp_path / ".git").is_dir()
-    assert (tmp_path / "default.yml").is_file()
-
-    # Running a second time should fail
-    result = runner.invoke(app, ["internal", "generate-cs", cs_repo])
-    assert result.exit_code != 0
+TEST_VO = "testvo"
+TEST_USER_GROUP = "user"
+TEST_ADMIN_GROUP = "admin"
 
 
-def test_add_vo(tmp_path):
+@pytest.fixture(scope="session")
+def reference_cs_repo(tmp_path_factory):
+    tmp_path = tmp_path_factory.mktemp("reference_cs_repo")
     cs_repo = f"git+file://{tmp_path}"
 
-    # Create the CS
-    runner.invoke(app, ["internal", "generate-cs", cs_repo])
-
-    # Add a VO to it
-    vo1 = "testvo"
+    result = runner.invoke(app, ["internal", "generate-cs", cs_repo])
+    assert result.exit_code == 0, result.output
     result = runner.invoke(
         app,
         [
             "internal",
             "add-vo",
             cs_repo,
-            f"--vo={vo1}",
+            f"--vo={TEST_VO}",
             "--idp-url=https://idp.invalid",
             "--idp-client-id=idp-client-id",
         ],
     )
     assert result.exit_code == 0, result.output
+    result = runner.invoke(
+        app,
+        [
+            "internal",
+            "add-group",
+            cs_repo,
+            f"--vo={TEST_VO}",
+            f"--group={TEST_ADMIN_GROUP}",
+        ],
+    )
+    assert result.exit_code == 0, result.output
+
+    yield tmp_path
+
+
+@pytest.fixture
+def cs_repo(reference_cs_repo, tmp_path):
+    shutil.copytree(reference_cs_repo, tmp_path / "cs")
+    yield f"git+file://{tmp_path}/cs"
+
+
+@pytest.mark.parametrize("protocol", [None, "git+file://"])
+def test_generate_cs(tmp_path, protocol):
+    cs_repo = f"{tmp_path}"
+    if protocol is None:
+        cs_repo = f"git+file://{cs_repo}"
+
+    result = runner.invoke(app, ["internal", "generate-cs", cs_repo])
+    assert result.exit_code == 0, result.output
+    assert (tmp_path / ".git").is_dir()
+    assert (tmp_path / "default.yml").is_file()
+
+    # Running a second time should fail
+    result = runner.invoke(app, ["internal", "generate-cs", cs_repo])
+    assert result.exit_code != 0
+
 
+def test_add_vo(cs_repo):
     config = ConfigSource.create_from_url(backend_url=cs_repo).read_config()
 
-    assert vo1 in config.Registry
-    assert config.Registry[vo1].DefaultGroup == "user"
-    assert config.Registry[vo1].IdP.URL == "https://idp.invalid"
-    assert config.Registry[vo1].IdP.ClientID == "idp-client-id"
+    assert TEST_VO in config.Registry
+    assert config.Registry[TEST_VO].DefaultGroup == "user"
+    assert config.Registry[TEST_VO].IdP.URL == "https://idp.invalid"
+    assert config.Registry[TEST_VO].IdP.ClientID == "idp-client-id"
 
     # Add a second VO to it
     vo2 = "lhcb"
     result = runner.invoke(
         app,
         [
             "internal",
@@ -80,122 +106,94 @@
     # Try to insert a VO that already exists
     result = runner.invoke(
         app,
         [
             "internal",
             "add-vo",
             cs_repo,
-            f"--vo={vo1}",
+            f"--vo={TEST_VO}",
             "--idp-url=https://idp.invalid",
             "--idp-client-id=idp-client-id",
         ],
     )
     assert result.exit_code != 0, result.output
 
 
-def test_add_group(tmp_path):
-    cs_repo = f"git+file://{tmp_path}"
-    vo = "testvo"
-    group1 = "testgroup1"
-    group2 = "testgroup2"
-
-    # Create the CS
-    runner.invoke(app, ["internal", "generate-cs", cs_repo])
-    runner.invoke(
-        app,
-        [
-            "internal",
-            "add-vo",
-            cs_repo,
-            f"--vo={vo}",
-            "--idp-url=https://idp.invalid",
-            "--idp-client-id=idp-client-id",
-        ],
-    )
-
-    # Add a group to it
-    result = runner.invoke(
-        app, ["internal", "add-group", cs_repo, f"--vo={vo}", f"--group={group1}"]
-    )
-    assert result.exit_code == 0, result.output
+def test_add_group(cs_repo):
+    new_group = "testgroup2"
 
     config = ConfigSource.create_from_url(backend_url=cs_repo).read_config()
 
-    assert group1 in config.Registry[vo].Groups
-    assert config.Registry[vo].Groups[group1].JobShare == 1000
-    assert config.Registry[vo].Groups[group1].Properties == {"NormalUser"}
-    assert config.Registry[vo].Groups[group1].Users == set()
+    assert TEST_USER_GROUP in config.Registry[TEST_VO].Groups
+    assert config.Registry[TEST_VO].Groups[TEST_USER_GROUP].JobShare == 1000
+    assert config.Registry[TEST_VO].Groups[TEST_USER_GROUP].Properties == {"NormalUser"}
+    assert config.Registry[TEST_VO].Groups[TEST_USER_GROUP].Users == set()
 
     # Add a second group to it
     result = runner.invoke(
         app,
         [
             "internal",
             "add-group",
             cs_repo,
-            f"--vo={vo}",
-            f"--group={group2}",
+            f"--vo={TEST_VO}",
+            f"--group={new_group}",
             "--properties",
             "NormalUser",
             "--properties",
             "AdminUser",
         ],
     )
     config = ConfigSource.create_from_url(backend_url=cs_repo).read_config()
     assert result.exit_code == 0, result.output
 
-    assert group2 in config.Registry[vo].Groups
-    assert config.Registry[vo].Groups[group2].JobShare == 1000
-    assert config.Registry[vo].Groups[group2].Properties == {"AdminUser", "NormalUser"}
-    assert config.Registry[vo].Groups[group2].Users == set()
+    assert new_group in config.Registry[TEST_VO].Groups
+    assert config.Registry[TEST_VO].Groups[new_group].JobShare == 1000
+    assert config.Registry[TEST_VO].Groups[new_group].Properties == {
+        "AdminUser",
+        "NormalUser",
+    }
+    assert config.Registry[TEST_VO].Groups[new_group].Users == set()
 
     # Try to insert a group that already exists
     result = runner.invoke(
-        app, ["internal", "add-group", cs_repo, f"--vo={vo}", f"--group={group1}"]
+        app,
+        [
+            "internal",
+            "add-group",
+            cs_repo,
+            f"--vo={TEST_VO}",
+            f"--group={TEST_USER_GROUP}",
+        ],
     )
     assert result.exit_code != 0, result.output
 
     # Try to insert a group with a non-existing VO
     result = runner.invoke(
         app,
-        ["internal", "add-group", cs_repo, "--vo=nonexistingvo", f"--group={group1}"],
+        [
+            "internal",
+            "add-group",
+            cs_repo,
+            "--vo=nonexistingvo",
+            f"--group={TEST_USER_GROUP}",
+        ],
     )
     assert result.exit_code != 0, result.output
 
 
-@pytest.mark.parametrize("vo", ["nonexistingvo", "testvo"])
+@pytest.mark.parametrize("vo", ["nonexistingvo", TEST_VO])
 @pytest.mark.parametrize(
-    "user_group", [["nonexisting_group"], ["user"], ["user", "admin"], []]
+    "user_group",
+    [["nonexisting_group"], [TEST_USER_GROUP], [TEST_USER_GROUP, TEST_ADMIN_GROUP], []],
 )
-def test_add_user(tmp_path, vo, user_group):
-    cs_repo = f"git+file://{tmp_path}"
-
+def test_add_user(cs_repo, vo, user_group):
     sub = "lhcb:chaen"
     preferred_username = "dontCallMeShirley"
 
-    # Create the CS
-    runner.invoke(app, ["internal", "generate-cs", cs_repo])
-    runner.invoke(
-        app,
-        [
-            "internal",
-            "add-vo",
-            cs_repo,
-            "--vo=testvo",
-            "--idp-url=https://idp.invalid",
-            "--idp-client-id=idp-client-id",
-        ],
-    )
-    runner.invoke(
-        app, ["internal", "add-group", cs_repo, "--vo=testvo", "--group=user"]
-    )
-    runner.invoke(
-        app, ["internal", "add-group", cs_repo, "--vo=testvo", "--group=admin"]
-    )
-
     config = ConfigSource.create_from_url(backend_url=cs_repo).read_config()
 
     # Check the user isn't in it
     if vo in config.Registry:
         assert sub not in config.Registry[vo].Users
 
     # Add a user to it
@@ -218,9 +216,9 @@
 
     assert result.exit_code == 0, result.output
 
     config = ConfigSource.create_from_url(backend_url=cs_repo).read_config()
     # check the user is defined
     assert vo in config.Registry
     assert sub in config.Registry[vo].Users
-    for group in user_group or ["user"]:
+    for group in user_group or [TEST_USER_GROUP]:
         assert config.Registry[vo].Groups[group].Users == {sub}
```

### Comparing `diracx-cli-0.0.1a8/tests/test_login.py` & `diracx-cli-0.0.1a9/tests/test_login.py`

 * *Files identical despite different names*

