# Comparing `tmp/snakemake_executor_plugin_slurm_jobstep-0.1.9.tar.gz` & `tmp/snakemake_executor_plugin_slurm_jobstep-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_executor_plugin_slurm_jobstep-0.1.9.tar", max compression
+gzip compressed data, was "snakemake_executor_plugin_slurm_jobstep-0.2.0.tar", max compression
```

## Comparing `snakemake_executor_plugin_slurm_jobstep-0.1.9.tar` & `snakemake_executor_plugin_slurm_jobstep-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2024-01-13 13:09:49.983954 snakemake_executor_plugin_slurm_jobstep-0.1.9/LICENSE
--rw-r--r--   0        0        0      166 2024-01-13 13:09:49.983954 snakemake_executor_plugin_slurm_jobstep-0.1.9/README.md
--rw-r--r--   0        0        0     1170 2024-01-13 13:09:49.983954 snakemake_executor_plugin_slurm_jobstep-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     5961 2024-01-13 13:09:49.987954 snakemake_executor_plugin_slurm_jobstep-0.1.9/snakemake_executor_plugin_slurm_jobstep/__init__.py
--rw-r--r--   0        0        0     1207 1970-01-01 00:00:00.000000 snakemake_executor_plugin_slurm_jobstep-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-11 14:21:04.405587 snakemake_executor_plugin_slurm_jobstep-0.2.0/LICENSE
+-rw-r--r--   0        0        0      166 2024-04-11 14:21:04.405587 snakemake_executor_plugin_slurm_jobstep-0.2.0/README.md
+-rw-r--r--   0        0        0     1183 2024-04-11 14:21:04.405587 snakemake_executor_plugin_slurm_jobstep-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6114 2024-04-11 14:21:04.405587 snakemake_executor_plugin_slurm_jobstep-0.2.0/snakemake_executor_plugin_slurm_jobstep/__init__.py
+-rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 snakemake_executor_plugin_slurm_jobstep-0.2.0/PKG-INFO
```

### Comparing `snakemake_executor_plugin_slurm_jobstep-0.1.9/LICENSE` & `snakemake_executor_plugin_slurm_jobstep-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_slurm_jobstep-0.1.9/pyproject.toml` & `snakemake_executor_plugin_slurm_jobstep-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-executor-plugin-slurm-jobstep"
-version = "0.1.9"
+version = "0.2.0"
 description = "A Snakemake executor plugin for running srun jobs inside of SLURM jobs (meant for internal use by snakemake-executor-plugin-slurm)"
 authors = [
     "Christian Meesters <meesters@uni-mainz.de>",
     "David Lähnemann <david.laehnemann@dkfz-heidelberg.de>",
     "Johannes Koester <johannes.koester@uni-due.de>",
 ]
 readme = "README.md"
@@ -12,21 +12,21 @@
 repository = "https://github.com/snakemake/snakemake-executor-plugin-slurm-jobstep"
 documentation = "https://snakemake.github.io/snakemake-plugin-catalog/plugins/executor/slurm-jobstep.html"
 keywords = ["snakemake", "plugin", "executor", "cluster", "slurm"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 snakemake-interface-common = "^1.13.0"
-snakemake-interface-executor-plugins = "^8.0.2"
+snakemake-interface-executor-plugins = "^9.0.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.7.0"
+black = ">=23.7,<25.0"
 flake8 = ">=6.1,<8.0"
 coverage = "^7.3.1"
-pytest = "^7.4.2"
+pytest = ">=7.4.2,<9.0.0"
 snakemake = {git = "https://github.com/snakemake/snakemake.git"}
 
 [tool.coverage.run]
 omit = [".*", "*/site-packages/*", "Snakefile"]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `snakemake_executor_plugin_slurm_jobstep-0.1.9/snakemake_executor_plugin_slurm_jobstep/__init__.py` & `snakemake_executor_plugin_slurm_jobstep-0.2.0/snakemake_executor_plugin_slurm_jobstep/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 __author__ = "David Lähnemann, Johannes Köster, Christian Meesters"
 __copyright__ = "Copyright 2023, David Lähnemann, Johannes Köster, Christian Meesters"
 __email__ = "johannes.koester@uni-due.de"
 __license__ = "MIT"
 
 import os
+import socket
 import subprocess
 import sys
-from typing import Generator, List
 from snakemake_interface_executor_plugins.executors.base import SubmittedJobInfo
-from snakemake_interface_executor_plugins.executors.remote import RemoteExecutor
+from snakemake_interface_executor_plugins.executors.real import RealExecutor
 from snakemake_interface_executor_plugins.jobs import (
     JobExecutorInterface,
 )
 from snakemake_interface_executor_plugins.settings import ExecMode, CommonSettings
 
 
 # Required:
 # Specify common settings shared by various executors.
 common_settings = CommonSettings(
     # define whether your executor plugin executes locally
     # or remotely. In virtually all cases, it will be remote execution
     # (cluster, cloud, etc.). Only Snakemake's standard execution
     # plugins (snakemake-executor-plugin-dryrun, snakemake-executor-plugin-local)
     # are expected to specify False here.
-    non_local_exec=False,
+    non_local_exec=True,
     # Define whether your executor plugin implies that there is no shared
     # filesystem (True) or not (False).
     # This is e.g. the case for cloud execution.
     implies_no_shared_fs=False,
     job_deploy_sources=False,
     pass_default_storage_provider_args=True,
     pass_default_resources_args=True,
     pass_envvar_declarations_to_cmd=False,
     auto_deploy_default_storage_provider=False,
+    spawned_jobs_assume_shared_fs=True,
 )
 
 
 # Required:
 # Implementation of your executor
-class Executor(RemoteExecutor):
+class Executor(RealExecutor):
     def __post_init__(self):
         # These environment variables are set by SLURM.
         # only needed for commented out jobstep handling below
         self.jobid = os.getenv("SLURM_JOB_ID")
-        self.jobs = dict()
 
     def run_job(self, job: JobExecutorInterface):
+        # Implement here how to run a job.
+        # You can access the job's resources, etc.
+        # via the job object.
+        # After submitting the job, you have to call
+        # self.report_job_submission(job_info).
+        # with job_info being of type
+        # snakemake_interface_executor_plugins.executors.base.SubmittedJobInfo.
+
+        jobsteps = dict()
         # TODO revisit special handling for group job levels via srun at a later stage
         # if job.is_group():
 
         #     def get_call(level_job, aux=""):
         #         # we need this calculation, because of srun's greediness and
         #         # SLURM's limits: it is not able to limit the memory if we divide the
         #         # job per CPU by itself.
@@ -100,37 +109,29 @@
             # SMP job, execute snakemake with srun, to ensure proper placing of threaded
             # executables within the c-group
             # The -n1 is important to avoid that srun executes the given command
             # multiple times, depending on the relation between
             # cpus per task and the number of CPU cores.
             call = f"srun -n1 --cpu-bind=q {self.format_job_exec(job)}"
 
+        self.logger.debug(f"This job is a group job: {job.is_group()}")
+        self.logger.debug(f"The call for this job is: {call}")
+        self.logger.debug(f"Job is running on host: {socket.gethostname()}")
         # this dict is to support the to be implemented feature of oversubscription in
         # "ordinary" group jobs.
-        proc = subprocess.Popen(call, shell=True)
-        job_info = SubmittedJobInfo(job, aux={"proc": proc})
+        jobsteps[job] = subprocess.Popen(call, shell=True)
 
+        job_info = SubmittedJobInfo(job)
         self.report_job_submission(job_info)
 
-    async def check_active_jobs(
-        self, active_jobs: List[SubmittedJobInfo]
-    ) -> Generator[SubmittedJobInfo, None, None]:
-        for active_job in active_jobs:
-            ret = active_job.aux["proc"].poll()
-            if ret is not None:
-                if ret != 0:
-                    self.report_job_error(active_job)
-                else:
-                    self.report_job_success(active_job)
-            else:
-                yield active_job
-
-    def cancel_jobs(self, active_jobs: List[SubmittedJobInfo]):
-        for active_job in active_jobs:
-            active_job.aux["proc"].terminate()
+        # wait until all steps are finished
+        if any(proc.wait() != 0 for proc in jobsteps.values()):
+            self.report_job_error(job_info)
+        else:
+            self.report_job_success(job_info)
 
     def cancel(self):
         pass
 
     def shutdown(self):
         pass
```

### Comparing `snakemake_executor_plugin_slurm_jobstep-0.1.9/PKG-INFO` & `snakemake_executor_plugin_slurm_jobstep-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: snakemake-executor-plugin-slurm-jobstep
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Snakemake executor plugin for running srun jobs inside of SLURM jobs (meant for internal use by snakemake-executor-plugin-slurm)
 Home-page: https://github.com/snakemake/snakemake-executor-plugin-slurm-jobstep
 License: MIT
 Keywords: snakemake,plugin,executor,cluster,slurm
 Author: Christian Meesters
 Author-email: meesters@uni-mainz.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: snakemake-interface-common (>=1.13.0,<2.0.0)
-Requires-Dist: snakemake-interface-executor-plugins (>=8.0.2,<9.0.0)
+Requires-Dist: snakemake-interface-executor-plugins (>=9.0.0,<10.0.0)
 Project-URL: Documentation, https://snakemake.github.io/snakemake-plugin-catalog/plugins/executor/slurm-jobstep.html
 Project-URL: Repository, https://github.com/snakemake/snakemake-executor-plugin-slurm-jobstep
 Description-Content-Type: text/markdown
 
 # snakemake-executor-plugin-slurm
 
 A Snakemake executor plugin for running srun jobs inside of SLURM jobs (meant for
```

