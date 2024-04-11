# Comparing `tmp/diracx-routers-0.0.1a8.tar.gz` & `tmp/diracx-routers-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diracx-routers-0.0.1a8.tar", last modified: Thu Nov 30 08:40:38 2023, max compression
+gzip compressed data, was "diracx-routers-0.0.1a9.tar", last modified: Sun Jan 28 09:12:25 2024, max compression
```

## Comparing `diracx-routers-0.0.1a8.tar` & `diracx-routers-0.0.1a9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:38.757686 diracx-routers-0.0.1a8/
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2023-11-30 08:40:38.757686 diracx-routers-0.0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-30 08:40:38.757686 diracx-routers-0.0.1a8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:38.749685 diracx-routers-0.0.1a8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:38.749685 diracx-routers-0.0.1a8/src/diracx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:38.753685 diracx-routers-0.0.1a8/src/diracx/routers/
--rw-r--r--   0 runner    (1001) docker     (127)    10785 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/src/diracx/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35745 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/src/diracx/routers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/src/diracx/routers/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/src/diracx/routers/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/src/diracx/routers/fastapi_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:38.753685 diracx-routers-0.0.1a8/src/diracx/routers/job_manager/
--rw-r--r--   0 runner    (1001) docker     (127)    22835 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/src/diracx/routers/job_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/src/diracx/routers/job_manager/sandboxes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/src/diracx/routers/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/src/diracx/routers/well_known.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:38.753685 diracx-routers-0.0.1a8/src/diracx_routers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2023-11-30 08:40:38.000000 diracx-routers-0.0.1a8/src/diracx_routers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      828 2023-11-30 08:40:38.000000 diracx-routers-0.0.1a8/src/diracx_routers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 08:40:38.000000 diracx-routers-0.0.1a8/src/diracx_routers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-11-30 08:40:38.000000 diracx-routers-0.0.1a8/src/diracx_routers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-11-30 08:40:38.000000 diracx-routers-0.0.1a8/src/diracx_routers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-30 08:40:38.000000 diracx-routers-0.0.1a8/src/diracx_routers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:38.753685 diracx-routers-0.0.1a8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:38.753685 diracx-routers-0.0.1a8/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/tests/auth/test_legacy_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)    24269 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/tests/auth/test_standard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:38.749685 diracx-routers-0.0.1a8/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:38.749685 diracx-routers-0.0.1a8/tests/data/lhcb-auth.web.cern.ch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:38.753685 diracx-routers-0.0.1a8/tests/data/lhcb-auth.web.cern.ch/.well-known/
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/tests/data/lhcb-auth.web.cern.ch/.well-known/openid-configuration
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:38.753685 diracx-routers-0.0.1a8/tests/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/tests/jobs/test_sandboxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/tests/test_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    31638 2023-11-30 08:39:21.000000 diracx-routers-0.0.1a8/tests/test_job_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:25.824967 diracx-routers-0.0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-01-28 09:12:25.824967 diracx-routers-0.0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 09:12:25.824967 diracx-routers-0.0.1a9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:25.816967 diracx-routers-0.0.1a9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:25.816967 diracx-routers-0.0.1a9/src/diracx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:25.820967 diracx-routers-0.0.1a9/src/diracx/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/src/diracx/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35745 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/src/diracx/routers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/src/diracx/routers/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/src/diracx/routers/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/src/diracx/routers/fastapi_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:25.820967 diracx-routers-0.0.1a9/src/diracx/routers/job_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)    22839 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/src/diracx/routers/job_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/src/diracx/routers/job_manager/sandboxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/src/diracx/routers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/src/diracx/routers/well_known.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:25.824967 diracx-routers-0.0.1a9/src/diracx_routers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-01-28 09:12:25.000000 diracx-routers-0.0.1a9/src/diracx_routers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-01-28 09:12:25.000000 diracx-routers-0.0.1a9/src/diracx_routers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 09:12:25.000000 diracx-routers-0.0.1a9/src/diracx_routers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-01-28 09:12:25.000000 diracx-routers-0.0.1a9/src/diracx_routers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-28 09:12:25.000000 diracx-routers-0.0.1a9/src/diracx_routers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 09:12:25.000000 diracx-routers-0.0.1a9/src/diracx_routers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:25.820967 diracx-routers-0.0.1a9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:25.820967 diracx-routers-0.0.1a9/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/tests/auth/test_legacy_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24633 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/tests/auth/test_standard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:25.816967 diracx-routers-0.0.1a9/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:25.816967 diracx-routers-0.0.1a9/tests/data/lhcb-auth.web.cern.ch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:25.820967 diracx-routers-0.0.1a9/tests/data/lhcb-auth.web.cern.ch/.well-known/
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/tests/data/lhcb-auth.web.cern.ch/.well-known/openid-configuration
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:25.824967 diracx-routers-0.0.1a9/tests/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/tests/jobs/test_sandboxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/tests/test_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32111 2024-01-28 09:11:11.000000 diracx-routers-0.0.1a9/tests/test_job_manager.py
```

### Comparing `diracx-routers-0.0.1a8/PKG-INFO` & `diracx-routers-0.0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diracx-routers
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

### Comparing `diracx-routers-0.0.1a8/pyproject.toml` & `diracx-routers-0.0.1a9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -66,7 +66,10 @@
 addopts = [
     "-v",
     "--cov=diracx.routers", "--cov-report=term-missing",
     "-pdiracx.testing", "-pdiracx.testing.osdb",
     "--import-mode=importlib",
 ]
 asyncio_mode = "auto"
+markers = [
+    "enabled_dependencies: List of dependencies which should be available to the FastAPI test client",
+]
```

### Comparing `diracx-routers-0.0.1a8/src/diracx/routers/__init__.py` & `diracx-routers-0.0.1a9/src/diracx/routers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import inspect
 import logging
 import os
 from collections.abc import AsyncGenerator
 from functools import partial
-from typing import Any, Iterable, TypeVar
+from typing import Any, Awaitable, Callable, Iterable, TypeVar, cast
 
 import dotenv
 from cachetools import TTLCache
 from fastapi import APIRouter, Depends, Request, status
 from fastapi.dependencies.models import Dependant
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import JSONResponse, Response
@@ -160,17 +160,24 @@
             router,
             prefix=f"{path_root}/{system_name}",
             tags=[system_name],
             dependencies=dependencies,
         )
 
     # Add exception handlers
-    app.add_exception_handler(DiracError, dirac_error_handler)
-    app.add_exception_handler(DiracHttpResponse, http_response_handler)
-    app.add_exception_handler(DBUnavailable, route_unavailable_error_hander)
+    # We need to cast because callables are contravariant and we define our exception handlers
+    # with a subclass of Exception (https://mypy.readthedocs.io/en/latest/generics.html#variance-of-generic-types)
+    handler_signature = Callable[[Request, Exception], Response | Awaitable[Response]]
+    app.add_exception_handler(DiracError, cast(handler_signature, dirac_error_handler))
+    app.add_exception_handler(
+        DiracHttpResponse, cast(handler_signature, http_response_handler)
+    )
+    app.add_exception_handler(
+        DBUnavailable, cast(handler_signature, route_unavailable_error_hander)
+    )
 
     # TODO: remove the CORSMiddleware once we figure out how to launch
     # diracx and diracx-web under the same origin
     origins = [
         "http://localhost:8000",
     ]
```

### Comparing `diracx-routers-0.0.1a8/src/diracx/routers/auth.py` & `diracx-routers-0.0.1a9/src/diracx/routers/auth.py`

 * *Files identical despite different names*

### Comparing `diracx-routers-0.0.1a8/src/diracx/routers/configuration.py` & `diracx-routers-0.0.1a9/src/diracx/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `diracx-routers-0.0.1a8/src/diracx/routers/dependencies.py` & `diracx-routers-0.0.1a9/src/diracx/routers/dependencies.py`

 * *Files identical despite different names*

### Comparing `diracx-routers-0.0.1a8/src/diracx/routers/fastapi_classes.py` & `diracx-routers-0.0.1a9/src/diracx/routers/fastapi_classes.py`

 * *Files identical despite different names*

### Comparing `diracx-routers-0.0.1a8/src/diracx/routers/job_manager/__init__.py` & `diracx-routers-0.0.1a9/src/diracx/routers/job_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,17 @@
 
 
 class JobID(BaseModel):
     job_id: int
 
 
 EXAMPLE_JDLS = {
-    "Simple JDL": [
-        """Arguments = "jobDescription.xml -o LogLevel=INFO";
+    "Simple JDL": {
+        "value": [
+            """Arguments = "jobDescription.xml -o LogLevel=INFO";
 Executable = "dirac-jobexec";
 JobGroup = jobGroup;
 JobName = jobName;
 JobType = User;
 LogLevel = INFO;
 OutputSandbox =
     {
@@ -97,23 +98,25 @@
         std.err,
         std.out
     };
 Priority = 1;
 Site = ANY;
 StdError = std.err;
 StdOutput = std.out;"""
-    ],
-    "Parametric JDL": ["""Arguments = "jobDescription.xml -o LogLevel=INFO"""],
+        ]
+    },
+    "Parametric JDL": {
+        "value": ["""Arguments = "jobDescription.xml -o LogLevel=INFO"""]
+    },
 }
 
 
 @router.post("/")
 async def submit_bulk_jobs(
-    # FIXME: Using mutliple doesn't work with swagger?
-    job_definitions: Annotated[list[str], Body(example=EXAMPLE_JDLS["Simple JDL"])],
+    job_definitions: Annotated[list[str], Body(openapi_examples=EXAMPLE_JDLS)],
     job_db: JobDB,
     job_logging_db: JobLoggingDB,
     user_info: Annotated[AuthorizedUserInfo, Depends(verify_dirac_access_token)],
 ) -> list[InsertedJob]:
     from DIRAC.Core.Utilities.ClassAd.ClassAdLight import ClassAd
     from DIRAC.Core.Utilities.ReturnValues import returnValueOrRaise
     from DIRAC.WorkloadManagementSystem.Service.JobPolicy import RIGHT_SUBMIT, JobPolicy
@@ -406,15 +409,15 @@
     #        jobList, RIGHT_RESCHEDULE
     #    )
     # For the moment all jobs are valid:
     valid_job_list = job_ids
     for job_id in valid_job_list:
         # TODO: delete job in TaskQueueDB
         # self.taskQueueDB.deleteJob(jobID)
-        result = job_db.rescheduleJob(job_id)
+        result = await job_db.rescheduleJob(job_id)
         try:
             res_status = await job_db.get_job_status(job_id)
         except NoResultFound as e:
             raise HTTPException(
                 status_code=HTTPStatus.NOT_FOUND, detail=f"Job {job_id} not found"
             ) from e
```

### Comparing `diracx-routers-0.0.1a8/src/diracx/routers/job_manager/sandboxes.py` & `diracx-routers-0.0.1a9/src/diracx/routers/job_manager/sandboxes.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
                         f"Failed to create bucket {self.bucket_name}"
                     ) from e
 
             yield
 
     @property
     def s3_client(self) -> S3Client:
+        if self._client is None:
+            raise RuntimeError("S3 client accessed before lifetime function")
         return self._client
 
 
 class SandboxUploadResponse(BaseModel):
     pfn: str
     url: str | None = None
     fields: dict[str, str] = {}
```

### Comparing `diracx-routers-0.0.1a8/src/diracx/routers/well_known.py` & `diracx-routers-0.0.1a9/src/diracx/routers/well_known.py`

 * *Files identical despite different names*

### Comparing `diracx-routers-0.0.1a8/src/diracx_routers.egg-info/PKG-INFO` & `diracx-routers-0.0.1a9/src/diracx_routers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diracx-routers
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

### Comparing `diracx-routers-0.0.1a8/src/diracx_routers.egg-info/SOURCES.txt` & `diracx-routers-0.0.1a9/src/diracx_routers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diracx-routers-0.0.1a8/tests/auth/test_legacy_exchange.py` & `diracx-routers-0.0.1a9/tests/auth/test_legacy_exchange.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,26 +4,35 @@
 import secrets
 import time
 from typing import Any
 
 import pytest
 
 DIRAC_CLIENT_ID = "myDIRACClientID"
+pytestmark = pytest.mark.enabled_dependencies(
+    ["AuthDB", "AuthSettings", "ConfigSource"]
+)
 
 
 @pytest.fixture
 def legacy_credentials(monkeypatch):
     secret = secrets.token_bytes()
     valid_token = f"diracx:legacy:{base64.urlsafe_b64encode(secret).decode()}"
     monkeypatch.setenv(
         "DIRACX_LEGACY_EXCHANGE_HASHED_API_KEY", hashlib.sha256(secret).hexdigest()
     )
     yield {"Authorization": f"Bearer {valid_token}"}
 
 
+@pytest.fixture
+def test_client(client_factory):
+    with client_factory.unauthenticated() as client:
+        yield client
+
+
 def _jwt_payload(jwt: str) -> dict[str, Any]:
     header, payload, signature = jwt.split(".")
 
     # Add padding to the payload, if necessary
     padding = len(payload) % 4
     if padding:
         payload += "=" * (4 - padding)
```

### Comparing `diracx-routers-0.0.1a8/tests/auth/test_standard.py` & `diracx-routers-0.0.1a9/tests/auth/test_standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import base64
 import hashlib
 import secrets
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from pathlib import Path
 from urllib.parse import parse_qs, urlparse
 
 import httpx
 import jwt
 import pytest
 from cryptography.hazmat.primitives import serialization
@@ -19,14 +19,23 @@
     _server_metadata_cache,
     create_token,
     get_server_metadata,
     parse_and_validate_scope,
 )
 
 DIRAC_CLIENT_ID = "myDIRACClientID"
+pytestmark = pytest.mark.enabled_dependencies(
+    ["AuthDB", "AuthSettings", "ConfigSource"]
+)
+
+
+@pytest.fixture
+def test_client(client_factory):
+    with client_factory.unauthenticated() as client:
+        yield client
 
 
 @pytest.fixture
 def non_mocked_hosts(test_client) -> list[str]:
     return [test_client.base_url.host]
 
 
@@ -309,15 +318,17 @@
 
     # Decode it
     refresh_payload = jwt.decode(
         initial_refresh_token, options={"verify_signature": False}
     )
 
     # Modify the expiration time (utc now - 5 hours)
-    refresh_payload["exp"] = int((datetime.utcnow() - timedelta(hours=5)).timestamp())
+    refresh_payload["exp"] = int(
+        (datetime.now(tz=timezone.utc) - timedelta(hours=5)).timestamp()
+    )
 
     # Encode it differently
     new_refresh_token = create_token(refresh_payload, test_auth_settings)
 
     request_data = {
         "grant_type": "refresh_token",
         "refresh_token": new_refresh_token,
@@ -342,15 +353,19 @@
 
     # Decode it
     refresh_payload = jwt.decode(
         initial_refresh_token, options={"verify_signature": False}
     )
 
     # Encode it differently (using another algorithm)
-    private_key = rsa.generate_private_key(public_exponent=65537, key_size=4096)
+    private_key = rsa.generate_private_key(
+        public_exponent=65537,
+        # DANGER: 512-bits is a bad idea for prod but makes the test notably faster!
+        key_size=512,
+    )
     pem = private_key.private_bytes(
         encoding=serialization.Encoding.PEM,
         format=serialization.PrivateFormat.PKCS8,
         encryption_algorithm=serialization.NoEncryption(),
     ).decode()
 
     new_auth_settings = AuthSettings(
```

### Comparing `diracx-routers-0.0.1a8/tests/data/lhcb-auth.web.cern.ch/.well-known/openid-configuration` & `diracx-routers-0.0.1a9/tests/data/lhcb-auth.web.cern.ch/.well-known/openid-configuration`

 * *Files identical despite different names*

### Comparing `diracx-routers-0.0.1a8/tests/jobs/test_sandboxes.py` & `diracx-routers-0.0.1a9/tests/jobs/test_sandboxes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 from __future__ import annotations
 
 import hashlib
 import secrets
 from copy import deepcopy
 from io import BytesIO
 
+import pytest
 import requests
 from fastapi.testclient import TestClient
 
 from diracx.routers.auth import AuthSettings, create_token
 
+pytestmark = pytest.mark.enabled_dependencies(
+    ["AuthSettings", "SandboxMetadataDB", "SandboxStoreSettings"]
+)
+
+
+@pytest.fixture
+def normal_user_client(client_factory):
+    with client_factory.normal_user() as client:
+        yield client
+
 
 def test_upload_then_download(
     normal_user_client: TestClient, test_auth_settings: AuthSettings
 ):
     data = secrets.token_bytes(512)
     checksum = hashlib.sha256(data).hexdigest()
```

### Comparing `diracx-routers-0.0.1a8/tests/test_config_manager.py` & `diracx-routers-0.0.1a9/tests/test_config_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,21 @@
+import pytest
 from fastapi import status
-from fastapi.testclient import TestClient
 
+pytestmark = pytest.mark.enabled_dependencies(["AuthSettings", "ConfigSource"])
 
-def test_unauthenticated(with_app):
-    with TestClient(with_app) as client:
+
+@pytest.fixture
+def normal_user_client(client_factory):
+    with client_factory.normal_user() as client:
+        yield client
+
+
+def test_unauthenticated(client_factory):
+    with client_factory.unauthenticated() as client:
         response = client.get("/api/config/lhcb/")
         assert response.status_code == status.HTTP_403_FORBIDDEN
 
 
 def test_get_config(normal_user_client):
     r = normal_user_client.get("/api/config/lhcb")
     assert r.status_code == status.HTTP_200_OK, r.json()
```

### Comparing `diracx-routers-0.0.1a8/tests/test_job_manager.py` & `diracx-routers-0.0.1a9/tests/test_job_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,37 @@
     Executable = "echo";
     Arguments = "%s";
     JobName = "Test_%n";
     Parameters = 100;
     ParameterStart = 1;
 """
 
+pytestmark = pytest.mark.enabled_dependencies(
+    [
+        "AuthSettings",
+        "JobDB",
+        "JobLoggingDB",
+        "ConfigSource",
+        "TaskQueueDB",
+        "SandboxMetadataDB",
+    ]
+)
+
+
+@pytest.fixture
+def normal_user_client(client_factory):
+    with client_factory.normal_user() as client:
+        yield client
+
+
+@pytest.fixture
+def admin_user_client(client_factory):
+    with client_factory.admin_user() as client:
+        yield client
+
 
 def test_insert_and_list_parametric_jobs(normal_user_client):
     job_definitions = [TEST_PARAMETRIC_JDL]
     r = normal_user_client.post("/api/jobs/", json=job_definitions)
     assert r.status_code == 200, r.json()
     assert len(r.json()) == 3  # Parameters.JOB_ID is 3
 
@@ -446,15 +469,15 @@
 
 
 def test_set_job_status_offset_naive_datetime_return_bad_request(
     normal_user_client: TestClient,
     valid_job_id: int,
 ):
     # Act
-    date = datetime.utcnow().isoformat(sep=" ")
+    date = datetime.utcnow().isoformat(sep=" ")  # noqa: DTZ003
     r = normal_user_client.patch(
         f"/api/jobs/{valid_job_id}/status",
         json={
             date: {
                 "Status": JobStatus.CHECKING.value,
                 "MinorStatus": "JobPath",
             }
```

