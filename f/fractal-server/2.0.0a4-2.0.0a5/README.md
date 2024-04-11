# Comparing `tmp/fractal_server-2.0.0a4.tar.gz` & `tmp/fractal_server-2.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-2.0.0a4.tar", max compression
+gzip compressed data, was "fractal_server-2.0.0a5.tar", max compression
```

## Comparing `fractal_server-2.0.0a4.tar` & `fractal_server-2.0.0a5.tar`

### file list

```diff
@@ -1,163 +1,164 @@
--rw-r--r--   0        0        0     1576 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/LICENSE
--rw-r--r--   0        0        0     2466 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/README.md
--rw-r--r--   0        0        0       24 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/__init__.py
--rw-r--r--   0        0        0     4958 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/__init__.py
--rw-r--r--   0        0        0     4042 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      183 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0      567 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     3378 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1090 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/models/state.py
--rw-r--r--   0        0        0      413 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/models/v1/__init__.py
--rw-r--r--   0        0        0     2017 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/models/v1/dataset.py
--rw-r--r--   0        0        0     3304 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v1/job.py
--rw-r--r--   0        0        0      859 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v1/project.py
--rw-r--r--   0        0        0     2782 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v1/task.py
--rw-r--r--   0        0        0     3950 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v1/workflow.py
--rw-r--r--   0        0        0      400 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/__init__.py
--rw-r--r--   0        0        0     1483 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/dataset.py
--rw-r--r--   0        0        0     1535 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/job.py
--rw-r--r--   0        0        0      845 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/project.py
--rw-r--r--   0        0        0     3257 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/task.py
--rw-r--r--   0        0        0     1256 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/workflow.py
--rw-r--r--   0        0        0     2727 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/workflowtask.py
--rw-r--r--   0        0        0        0 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/admin/__init__.py
--rw-r--r--   0        0        0    13981 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/admin/v1.py
--rw-r--r--   0        0        0     9826 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/admin/v2.py
--rw-r--r--   0        0        0      315 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/__init__.py
--rw-r--r--   0        0        0      958 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/__init__.py
--rw-r--r--   0        0        0    11955 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/_aux_functions.py
--rw-r--r--   0        0        0    16911 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/dataset.py
--rw-r--r--   0        0        0     5436 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/job.py
--rw-r--r--   0        0        0    15765 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/project.py
--rw-r--r--   0        0        0     6123 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/task.py
--rw-r--r--   0        0        0     8457 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/task_collection.py
--rw-r--r--   0        0        0    10930 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/workflow.py
--rw-r--r--   0        0        0     5579 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/workflowtask.py
--rw-r--r--   0        0        0     1210 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/__init__.py
--rw-r--r--   0        0        0    14301 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/_aux_functions.py
--rw-r--r--   0        0        0     9680 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/dataset.py
--rw-r--r--   0        0        0     5956 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/images.py
--rw-r--r--   0        0        0     5334 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/job.py
--rw-r--r--   0        0        0     6024 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/project.py
--rw-r--r--   0        0        0     7171 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/submit.py
--rw-r--r--   0        0        0     7130 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/task.py
--rw-r--r--   0        0        0     8466 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/task_collection.py
--rw-r--r--   0        0        0    11845 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/workflow.py
--rw-r--r--   0        0        0     8414 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/workflowtask.py
--rw-r--r--   0        0        0     4885 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/auth.py
--rw-r--r--   0        0        0        0 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/aux/__init__.py
--rw-r--r--   0        0        0     1248 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/aux/_job.py
--rw-r--r--   0        0        0      675 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/aux/_runner.py
--rw-r--r--   0        0        0       16 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0        0 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0      829 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/async_wrap.py
--rw-r--r--   0        0        0      119 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/components.py
--rw-r--r--   0        0        0     4159 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/__init__.py
--rw-r--r--   0        0        0       65 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/__init__.py
--rw-r--r--   0        0        0     8841 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_batching.py
--rw-r--r--   0        0        0     1908 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
--rw-r--r--   0        0        0     4421 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    15552 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_slurm_config.py
--rw-r--r--   0        0        0     5123 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    44451 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/executor.py
--rw-r--r--   0        0        0     5852 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/remote.py
--rw-r--r--   0        0        0      206 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/filenames.py
--rw-r--r--   0        0        0     1254 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/set_start_and_last_task_index.py
--rw-r--r--   0        0        0     3219 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/task_files.py
--rw-r--r--   0        0        0    13608 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/__init__.py
--rw-r--r--   0        0        0    21238 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_common.py
--rw-r--r--   0        0        0     6926 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/__init__.py
--rw-r--r--   0        0        0     3147 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/_local_config.py
--rw-r--r--   0        0        0     1493 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/executor.py
--rw-r--r--   0        0        0    10853 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_slurm/__init__.py
--rw-r--r--   0        0        0     2738 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     5977 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0     3294 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/common.py
--rw-r--r--   0        0        0     4684 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/handle_failed_job.py
--rw-r--r--   0        0        0    12482 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/__init__.py
--rw-r--r--   0        0        0     5881 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/__init__.py
--rw-r--r--   0        0        0     3630 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/_local_config.py
--rw-r--r--   0        0        0     1614 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/executor.py
--rw-r--r--   0        0        0     4409 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_slurm/__init__.py
--rw-r--r--   0        0        0     2793 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     6621 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0      571 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/deduplicate_list.py
--rw-r--r--   0        0        0     5202 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/handle_failed_job.py
--rw-r--r--   0        0        0     1281 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/merge_outputs.py
--rw-r--r--   0        0        0    11119 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/runner.py
--rw-r--r--   0        0        0    10087 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/runner_functions.py
--rw-r--r--   0        0        0     3845 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/runner_functions_low_level.py
--rw-r--r--   0        0        0     1376 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/task_interface.py
--rw-r--r--   0        0        0      511 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/v1_compat.py
--rw-r--r--   0        0        0      157 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/__init__.py
--rw-r--r--   0        0        0     3264 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/_validators.py
--rw-r--r--   0        0        0      692 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/state.py
--rw-r--r--   0        0        0     3113 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/user.py
--rw-r--r--   0        0        0     2078 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/__init__.py
--rw-r--r--   0        0        0     4302 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/applyworkflow.py
--rw-r--r--   0        0        0     3444 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/dataset.py
--rw-r--r--   0        0        0     1274 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/dumps.py
--rw-r--r--   0        0        0     3829 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/manifest.py
--rw-r--r--   0        0        0     1218 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/project.py
--rw-r--r--   0        0        0     3731 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/task.py
--rw-r--r--   0        0        0     3057 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/task_collection.py
--rw-r--r--   0        0        0     4618 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/workflow.py
--rw-r--r--   0        0        0     1704 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/dataset.py
--rw-r--r--   0        0        0     2037 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/dumps.py
--rw-r--r--   0        0        0     3250 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/job.py
--rw-r--r--   0        0        0     6243 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/manifest.py
--rw-r--r--   0        0        0      814 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/project.py
--rw-r--r--   0        0        0     4574 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/task.py
--rw-r--r--   0        0        0     3171 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/task_collection.py
--rw-r--r--   0        0        0     1831 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/workflow.py
--rw-r--r--   0        0        0     5051 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/workflowtask.py
--rw-r--r--   0        0        0    11203 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0    15080 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/config.py
--rw-r--r--   0        0        0      398 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/data_migrations/README.md
--rw-r--r--   0        0        0       88 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/images/__init__.py
--rw-r--r--   0        0        0     1969 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/images/models.py
--rw-r--r--   0        0        0     2234 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/images/tools.py
--rw-r--r--   0        0        0     3924 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/logger.py
--rw-r--r--   0        0        0     3001 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/main.py
--rw-r--r--   0        0        0       59 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/README
--rw-r--r--   0        0        0     2630 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      526 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     1157 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
--rw-r--r--   0        0        0     8770 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0     1632 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
--rw-r--r--   0        0        0     1353 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
--rw-r--r--   0        0        0     2684 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
--rw-r--r--   0        0        0     1115 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
--rw-r--r--   0        0        0     1057 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
--rw-r--r--   0        0        0      883 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
--rw-r--r--   0        0        0     1849 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
--rw-r--r--   0        0        0      867 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
--rw-r--r--   0        0        0      949 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
--rw-r--r--   0        0        0     8240 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/d71e732236cd_v2.py
--rw-r--r--   0        0        0      963 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
--rw-r--r--   0        0        0     1221 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
--rw-r--r--   0        0        0      746 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/syringe.py
--rw-r--r--   0        0        0       23 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0     5379 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/endpoint_operations.py
--rw-r--r--   0        0        0     3278 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/utils.py
--rw-r--r--   0        0        0     3775 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/v1/_TaskCollectPip.py
--rw-r--r--   0        0        0        0 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/v1/__init__.py
--rw-r--r--   0        0        0    11725 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/v1/background_operations.py
--rw-r--r--   0        0        0      502 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/v1/get_collection_data.py
--rw-r--r--   0        0        0     3775 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/v2/_TaskCollectPip.py
--rw-r--r--   0        0        0        0 2024-04-10 10:17:25.457266 fractal_server-2.0.0a4/fractal_server/tasks/v2/__init__.py
--rw-r--r--   0        0        0    12803 2024-04-10 10:17:25.457266 fractal_server-2.0.0a4/fractal_server/tasks/v2/background_operations.py
--rw-r--r--   0        0        0      502 2024-04-10 10:17:25.457266 fractal_server-2.0.0a4/fractal_server/tasks/v2/get_collection_data.py
--rw-r--r--   0        0        0     2115 2024-04-10 10:17:25.457266 fractal_server-2.0.0a4/fractal_server/utils.py
--rw-r--r--   0        0        0     2999 2024-04-10 10:17:25.457266 fractal_server-2.0.0a4/pyproject.toml
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 fractal_server-2.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1576 2024-04-11 15:42:49.346867 fractal_server-2.0.0a5/LICENSE
+-rw-r--r--   0        0        0     2466 2024-04-11 15:42:49.346867 fractal_server-2.0.0a5/README.md
+-rw-r--r--   0        0        0       24 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/__init__.py
+-rw-r--r--   0        0        0     4958 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0     4042 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      183 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0      567 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     3378 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1090 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0      413 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/v1/__init__.py
+-rw-r--r--   0        0        0     2017 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/v1/dataset.py
+-rw-r--r--   0        0        0     3304 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/v1/job.py
+-rw-r--r--   0        0        0      859 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/v1/project.py
+-rw-r--r--   0        0        0     2782 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/v1/task.py
+-rw-r--r--   0        0        0     3950 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/v1/workflow.py
+-rw-r--r--   0        0        0      400 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/v2/__init__.py
+-rw-r--r--   0        0        0     1483 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/v2/dataset.py
+-rw-r--r--   0        0        0     1535 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/v2/job.py
+-rw-r--r--   0        0        0      845 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/v2/project.py
+-rw-r--r--   0        0        0     3257 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/v2/task.py
+-rw-r--r--   0        0        0     1256 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/v2/workflow.py
+-rw-r--r--   0        0        0     2727 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/models/v2/workflowtask.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/routes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/routes/admin/__init__.py
+-rw-r--r--   0        0        0    13981 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/routes/admin/v1.py
+-rw-r--r--   0        0        0     9826 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/routes/admin/v2.py
+-rw-r--r--   0        0        0      315 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/routes/api/__init__.py
+-rw-r--r--   0        0        0      958 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/__init__.py
+-rw-r--r--   0        0        0    11955 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0    16911 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/dataset.py
+-rw-r--r--   0        0        0     5436 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/job.py
+-rw-r--r--   0        0        0    15765 2024-04-11 15:42:49.350867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/project.py
+-rw-r--r--   0        0        0     6123 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/task.py
+-rw-r--r--   0        0        0     8873 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/task_collection.py
+-rw-r--r--   0        0        0    10930 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/workflow.py
+-rw-r--r--   0        0        0     5579 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/workflowtask.py
+-rw-r--r--   0        0        0     1373 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/__init__.py
+-rw-r--r--   0        0        0    14301 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/_aux_functions.py
+-rw-r--r--   0        0        0     9680 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/dataset.py
+-rw-r--r--   0        0        0     5956 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/images.py
+-rw-r--r--   0        0        0     5334 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/job.py
+-rw-r--r--   0        0        0     6024 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/project.py
+-rw-r--r--   0        0        0     7171 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/submit.py
+-rw-r--r--   0        0        0     7130 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/task.py
+-rw-r--r--   0        0        0     8904 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/task_collection.py
+-rw-r--r--   0        0        0     1628 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/task_legacy.py
+-rw-r--r--   0        0        0    11845 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/workflow.py
+-rw-r--r--   0        0        0     8414 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/workflowtask.py
+-rw-r--r--   0        0        0     4885 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/auth.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/aux/__init__.py
+-rw-r--r--   0        0        0     1248 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/aux/_job.py
+-rw-r--r--   0        0        0      675 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/routes/aux/_runner.py
+-rw-r--r--   0        0        0       16 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/async_wrap.py
+-rw-r--r--   0        0        0      119 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/components.py
+-rw-r--r--   0        0        0     4159 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/executors/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/__init__.py
+-rw-r--r--   0        0        0     8841 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/_batching.py
+-rw-r--r--   0        0        0     1908 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
+-rw-r--r--   0        0        0     4421 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    15552 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/_slurm_config.py
+-rw-r--r--   0        0        0     5123 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    44451 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/executor.py
+-rw-r--r--   0        0        0     5852 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/remote.py
+-rw-r--r--   0        0        0      206 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/filenames.py
+-rw-r--r--   0        0        0     1254 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/set_start_and_last_task_index.py
+-rw-r--r--   0        0        0     3219 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/task_files.py
+-rw-r--r--   0        0        0    13608 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v1/__init__.py
+-rw-r--r--   0        0        0    21240 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v1/_common.py
+-rw-r--r--   0        0        0     6926 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v1/_local/__init__.py
+-rw-r--r--   0        0        0     3147 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v1/_local/_local_config.py
+-rw-r--r--   0        0        0     1493 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v1/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v1/_local/executor.py
+-rw-r--r--   0        0        0    10853 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v1/_slurm/__init__.py
+-rw-r--r--   0        0        0     2738 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v1/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     5977 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0     3294 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v1/common.py
+-rw-r--r--   0        0        0     4684 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v1/handle_failed_job.py
+-rw-r--r--   0        0        0    12482 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/__init__.py
+-rw-r--r--   0        0        0     5881 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/_local/__init__.py
+-rw-r--r--   0        0        0     3630 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/_local/_local_config.py
+-rw-r--r--   0        0        0     1614 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/_local/executor.py
+-rw-r--r--   0        0        0     4409 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/_slurm/__init__.py
+-rw-r--r--   0        0        0     2793 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     6621 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0      639 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/deduplicate_list.py
+-rw-r--r--   0        0        0     5202 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/handle_failed_job.py
+-rw-r--r--   0        0        0     1281 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/merge_outputs.py
+-rw-r--r--   0        0        0    11784 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/runner.py
+-rw-r--r--   0        0        0    10087 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/runner_functions.py
+-rw-r--r--   0        0        0     3845 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/runner_functions_low_level.py
+-rw-r--r--   0        0        0     1410 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/task_interface.py
+-rw-r--r--   0        0        0      511 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/runner/v2/v1_compat.py
+-rw-r--r--   0        0        0      157 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/schemas/__init__.py
+-rw-r--r--   0        0        0     3264 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/schemas/_validators.py
+-rw-r--r--   0        0        0      692 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/schemas/state.py
+-rw-r--r--   0        0        0     3113 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/schemas/user.py
+-rw-r--r--   0        0        0     2078 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/schemas/v1/__init__.py
+-rw-r--r--   0        0        0     4302 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/schemas/v1/applyworkflow.py
+-rw-r--r--   0        0        0     3444 2024-04-11 15:42:49.354867 fractal_server-2.0.0a5/fractal_server/app/schemas/v1/dataset.py
+-rw-r--r--   0        0        0     1274 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v1/dumps.py
+-rw-r--r--   0        0        0     3829 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v1/manifest.py
+-rw-r--r--   0        0        0     1218 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v1/project.py
+-rw-r--r--   0        0        0     3704 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v1/task.py
+-rw-r--r--   0        0        0     3057 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v1/task_collection.py
+-rw-r--r--   0        0        0     4618 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v1/workflow.py
+-rw-r--r--   0        0        0     1752 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v2/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v2/dataset.py
+-rw-r--r--   0        0        0     2037 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v2/dumps.py
+-rw-r--r--   0        0        0     3250 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v2/job.py
+-rw-r--r--   0        0        0     6243 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v2/manifest.py
+-rw-r--r--   0        0        0      814 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v2/project.py
+-rw-r--r--   0        0        0     4672 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v2/task.py
+-rw-r--r--   0        0        0     3171 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v2/task_collection.py
+-rw-r--r--   0        0        0     1831 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v2/workflow.py
+-rw-r--r--   0        0        0     5051 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/schemas/v2/workflowtask.py
+-rw-r--r--   0        0        0    11203 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0    15080 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/config.py
+-rw-r--r--   0        0        0      398 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/data_migrations/README.md
+-rw-r--r--   0        0        0      144 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/images/__init__.py
+-rw-r--r--   0        0        0     2904 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/images/models.py
+-rw-r--r--   0        0        0     2234 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/images/tools.py
+-rw-r--r--   0        0        0     3924 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/logger.py
+-rw-r--r--   0        0        0     3001 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2630 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      526 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     1157 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
+-rw-r--r--   0        0        0     8770 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0     1632 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
+-rw-r--r--   0        0        0     1353 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
+-rw-r--r--   0        0        0     2684 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
+-rw-r--r--   0        0        0     1115 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
+-rw-r--r--   0        0        0     1057 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
+-rw-r--r--   0        0        0      883 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
+-rw-r--r--   0        0        0     1849 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
+-rw-r--r--   0        0        0      867 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
+-rw-r--r--   0        0        0      949 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
+-rw-r--r--   0        0        0     8240 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/d71e732236cd_v2.py
+-rw-r--r--   0        0        0      963 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
+-rw-r--r--   0        0        0     1221 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
+-rw-r--r--   0        0        0      746 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/syringe.py
+-rw-r--r--   0        0        0       23 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0     5379 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/tasks/endpoint_operations.py
+-rw-r--r--   0        0        0     3278 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/tasks/utils.py
+-rw-r--r--   0        0        0     3775 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/tasks/v1/_TaskCollectPip.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/tasks/v1/__init__.py
+-rw-r--r--   0        0        0    11725 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/tasks/v1/background_operations.py
+-rw-r--r--   0        0        0      502 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/tasks/v1/get_collection_data.py
+-rw-r--r--   0        0        0     3775 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/tasks/v2/_TaskCollectPip.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/tasks/v2/__init__.py
+-rw-r--r--   0        0        0    12803 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/tasks/v2/background_operations.py
+-rw-r--r--   0        0        0      502 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/tasks/v2/get_collection_data.py
+-rw-r--r--   0        0        0     2115 2024-04-11 15:42:49.358868 fractal_server-2.0.0a5/fractal_server/utils.py
+-rw-r--r--   0        0        0     2999 2024-04-11 15:42:49.362867 fractal_server-2.0.0a5/pyproject.toml
+-rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 fractal_server-2.0.0a5/PKG-INFO
```

### Comparing `fractal_server-2.0.0a4/LICENSE` & `fractal_server-2.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/README.md` & `fractal_server-2.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/__main__.py` & `fractal_server-2.0.0a5/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/alembic.ini` & `fractal_server-2.0.0a5/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/db/__init__.py` & `fractal_server-2.0.0a5/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/linkuserproject.py` & `fractal_server-2.0.0a5/fractal_server/app/models/linkuserproject.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/security.py` & `fractal_server-2.0.0a5/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/state.py` & `fractal_server-2.0.0a5/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/v1/dataset.py` & `fractal_server-2.0.0a5/fractal_server/app/models/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/v1/job.py` & `fractal_server-2.0.0a5/fractal_server/app/models/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/v1/project.py` & `fractal_server-2.0.0a5/fractal_server/app/models/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/v1/task.py` & `fractal_server-2.0.0a5/fractal_server/app/models/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/v1/workflow.py` & `fractal_server-2.0.0a5/fractal_server/app/models/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/v2/dataset.py` & `fractal_server-2.0.0a5/fractal_server/app/models/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/v2/job.py` & `fractal_server-2.0.0a5/fractal_server/app/models/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/v2/project.py` & `fractal_server-2.0.0a5/fractal_server/app/models/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/v2/task.py` & `fractal_server-2.0.0a5/fractal_server/app/models/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/v2/workflow.py` & `fractal_server-2.0.0a5/fractal_server/app/models/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/models/v2/workflowtask.py` & `fractal_server-2.0.0a5/fractal_server/app/models/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/admin/v1.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/admin/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/admin/v2.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/admin/v2.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/__init__.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/_aux_functions.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/dataset.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/job.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/project.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/task.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/task_collection.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/task_collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,14 +136,24 @@
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
                 detail=(
                     "Cannot collect package. Possible reason: another "
                     "collection of the same package is in progress. "
                     f"Original error: {e}"
                 ),
             )
+        except ValidationError as e:
+            await db.close()
+            raise HTTPException(
+                status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+                detail=(
+                    "Cannot collect package. Possible reason: an old version "
+                    "of the same package has already been collected. "
+                    f"Original error: {e}"
+                ),
+            )
         task_collect_status.info = "Already installed"
         state = State(data=task_collect_status.sanitised_dict())
         response.status_code == status.HTTP_200_OK
         await db.close()
         return state
     settings = Inject(get_settings)
```

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/workflow.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/workflowtask.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v1/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/__init__.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,27 @@
 from .dataset import router as dataset_router_v2
 from .images import router as images_routes_v2
 from .job import router as job_router_v2
 from .project import router as project_router_v2
 from .submit import router as submit_job_router_v2
 from .task import router as task_router_v2
 from .task_collection import router as task_collection_router_v2
+from .task_legacy import router as task_legacy_router_v2
 from .workflow import router as workflow_router_v2
 from .workflowtask import router as workflowtask_router_v2
 
 router_api_v2 = APIRouter()
 
 router_api_v2.include_router(dataset_router_v2, tags=["V2 Dataset"])
 router_api_v2.include_router(job_router_v2, tags=["V2 Job"])
 router_api_v2.include_router(images_routes_v2, tags=["V2 Images"])
 router_api_v2.include_router(project_router_v2, tags=["V2 Project"])
 router_api_v2.include_router(submit_job_router_v2, tags=["V2 Job"])
-router_api_v2.include_router(task_router_v2, prefix="/task", tags=["V2 Task"])
 router_api_v2.include_router(
     task_collection_router_v2, prefix="/task", tags=["V2 Task Collection"]
 )
+router_api_v2.include_router(task_router_v2, prefix="/task", tags=["V2 Task"])
+router_api_v2.include_router(
+    task_legacy_router_v2, prefix="/task-legacy", tags=["V2 Task Legacy"]
+)
 router_api_v2.include_router(workflow_router_v2, tags=["V2 Workflow"])
 router_api_v2.include_router(workflowtask_router_v2, tags=["V2 WorkflowTask"])
```

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/_aux_functions.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/dataset.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/images.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/images.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/job.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/project.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/submit.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/submit.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/task.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/task_collection.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/task_collection.py`

 * *Files 9% similar despite different names*

```diff
@@ -133,15 +133,25 @@
         except FileNotFoundError as e:
             await db.close()
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
                 detail=(
                     "Cannot collect package. Possible reason: another "
                     "collection of the same package is in progress. "
-                    f"Original error: {e}"
+                    f"Original FileNotFoundError: {e}"
+                ),
+            )
+        except ValidationError as e:
+            await db.close()
+            raise HTTPException(
+                status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+                detail=(
+                    "Cannot collect package. Possible reason: an old version "
+                    "of the same package has already been collected. "
+                    f"Original ValidationError: {e}"
                 ),
             )
         task_collect_status.info = "Already installed"
         state = State(data=task_collect_status.sanitised_dict())
         response.status_code == status.HTTP_200_OK
         await db.close()
         return state
```

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/workflow.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/workflowtask.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/api/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/auth.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/auth.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/aux/_job.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/aux/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/routes/aux/_runner.py` & `fractal_server-2.0.0a5/fractal_server/app/routes/aux/_runner.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/async_wrap.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/async_wrap.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/exceptions.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/exceptions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_batching.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_check_jobs_status.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/_check_jobs_status.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_slurm_config.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/executor.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/remote.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/executors/slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/set_start_and_last_task_index.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/set_start_and_last_task_index.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/task_files.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/task_files.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v1/__init__.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_common.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v1/_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 
     # This try/except block covers the case of a task that ran successfully but
     # did not write the expected metadiff file (ref fractal-server issue #854).
     try:
         with task_files.metadiff.open("r") as f_metadiff:
             diff_metadata = json.load(f_metadiff)
     except FileNotFoundError as e:
-        logger.error(
+        logger.warning(
             f"Skip collection of updated metadata. Original error: {str(e)}"
         )
         diff_metadata = {}
 
     # Cover the case where the task wrote `null`, rather than a valid
     # dictionary (ref fractal-server issue #878).
     if diff_metadata is None:
```

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/__init__.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v1/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/_local_config.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v1/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/_submit_setup.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v1/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/executor.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v1/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_slurm/__init__.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v1/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_slurm/_submit_setup.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v1/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_slurm/get_slurm_config.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v1/_slurm/get_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v1/common.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v1/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v1/handle_failed_job.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v1/handle_failed_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/__init__.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/__init__.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/_local_config.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/_submit_setup.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/executor.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_slurm/__init__.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_slurm/_submit_setup.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_slurm/get_slurm_config.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/_slurm/get_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/deduplicate_list.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/deduplicate_list.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import TypeVar
 
 from ....images import SingleImage
+from ....images import SingleImageTaskOutput
 from .task_interface import InitArgsModel
 
-T = TypeVar("T", SingleImage, InitArgsModel)
+T = TypeVar("T", SingleImage, SingleImageTaskOutput, InitArgsModel)
 
 
 def deduplicate_list(
     this_list: list[T],
 ) -> list[T]:
     """
     Custom replacement for `set(this_list)`, when items are non-hashable.
```

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/handle_failed_job.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/handle_failed_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/merge_outputs.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/merge_outputs.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/runner.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,14 +153,28 @@
                 updated_types = copy(original_img["types"])
 
                 # Update image attributes/types with task output and manifest
                 updated_attributes.update(image["attributes"])
                 updated_types.update(image["types"])
                 updated_types.update(task.output_types)
 
+                # Unset attributes with None value
+                updated_attributes = {
+                    key: value
+                    for key, value in updated_attributes.items()
+                    if value is not None
+                }
+
+                # Validate new image
+                SingleImage(
+                    zarr_url=image["zarr_url"],
+                    types=updated_types,
+                    attributes=updated_attributes,
+                )
+
                 # Update image in the dataset image list
                 tmp_images[original_index]["attributes"] = updated_attributes
                 tmp_images[original_index]["types"] = updated_types
             # Add new image
             else:
                 # Check that image['zarr_url'] is relative to zarr_dir
                 if not image["zarr_url"].startswith(zarr_dir):
@@ -178,14 +192,19 @@
                     )
                     if img_search is not None:
                         original_img = img_search["image"]
                         updated_attributes = copy(original_img["attributes"])
                         updated_types = copy(original_img["types"])
                 # Update image attributes/types with task output and manifest
                 updated_attributes.update(image["attributes"])
+                updated_attributes = {
+                    key: value
+                    for key, value in updated_attributes.items()
+                    if value is not None
+                }
                 updated_types.update(image["types"])
                 updated_types.update(task.output_types)
                 new_image = dict(
                     zarr_url=image["zarr_url"],
                     origin=image["origin"],
                     attributes=updated_attributes,
                     types=updated_types,
```

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/runner_functions.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/runner_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/runner_functions_low_level.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/runner_functions_low_level.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/runner/v2/task_interface.py` & `fractal_server-2.0.0a5/fractal_server/app/runner/v2/task_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import Any
 
 from pydantic import BaseModel
 from pydantic import Field
 
-from ....images import SingleImage
+from ....images import SingleImageTaskOutput
 from fractal_server.images import Filters
 
 
 class TaskOutput(BaseModel):
     class Config:
         extra = "forbid"
 
-    image_list_updates: list[SingleImage] = Field(default_factory=list)
+    image_list_updates: list[SingleImageTaskOutput] = Field(
+        default_factory=list
+    )
     image_list_removals: list[str] = Field(default_factory=list)
     filters: Filters = Field(default_factory=Filters)
 
     def check_zarr_urls_are_unique(self) -> None:
         zarr_urls = [img.zarr_url for img in self.image_list_updates]
         zarr_urls.extend(self.image_list_removals)
         if len(zarr_urls) != len(set(zarr_urls)):
```

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/_validators.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/state.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/user.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/__init__.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/applyworkflow.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v1/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/dataset.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/dumps.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v1/dumps.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/manifest.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v1/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/project.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/task.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v1/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,14 @@
     meta: Optional[dict[str, Any]] = Field(default={})
     owner: Optional[str]
     version: Optional[str]
     args_schema: Optional[dict[str, Any]]
     args_schema_version: Optional[str]
     docs_info: Optional[str]
     docs_link: Optional[HttpUrl]
-    is_v2_compatible: bool
 
 
 class TaskCreateV1(_TaskBaseV1):
     """
     Class for `Task` creation.
 
     Attributes:
```

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/task_collection.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/workflow.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/__init__.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .manifest import ManifestV2  # noqa F401
 from .project import ProjectCreateV2  # noqa F401
 from .project import ProjectReadV2  # noqa F401
 from .project import ProjectUpdateV2  # noqa F401
 from .task import TaskCreateV2  # noqa F401
 from .task import TaskExportV2  # noqa F401
 from .task import TaskImportV2  # noqa F401
+from .task import TaskLegacyReadV2  # noqa F401
 from .task import TaskReadV2  # noqa F401
 from .task import TaskUpdateV2  # noqa F401
 from .task_collection import TaskCollectPipV2  # noqa F401
 from .task_collection import TaskCollectStatusV2  # noqa F401
 from .workflow import WorkflowCreateV2  # noqa F401
 from .workflow import WorkflowExportV2  # noqa F401
 from .workflow import WorkflowImportV2  # noqa F401
```

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/dataset.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/dumps.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v2/dumps.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/job.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/manifest.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v2/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/project.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/task.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v2/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pydantic import Field
 from pydantic import HttpUrl
 from pydantic import root_validator
 from pydantic import validator
 
 from .._validators import valdictkeys
 from .._validators import valstr
+from ..v1.task import TaskReadV1
 
 
 class TaskCreateV2(BaseModel, extra=Extra.forbid):
 
     name: str
 
     command_non_parallel: Optional[str]
@@ -96,14 +97,18 @@
     args_schema_version: Optional[str]
     docs_info: Optional[str]
     docs_link: Optional[HttpUrl]
     input_types: dict[str, bool]
     output_types: dict[str, bool]
 
 
+class TaskLegacyReadV2(TaskReadV1):
+    is_v2_compatible: bool
+
+
 class TaskUpdateV2(BaseModel):
 
     name: Optional[str]
     version: Optional[str]
     command_parallel: Optional[str]
     command_non_parallel: Optional[str]
     input_types: Optional[dict[str, bool]]
```

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/task_collection.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v2/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/workflow.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/workflowtask.py` & `fractal_server-2.0.0a5/fractal_server/app/schemas/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/app/security/__init__.py` & `fractal_server-2.0.0a5/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/config.py` & `fractal_server-2.0.0a5/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/images/models.py` & `fractal_server-2.0.0a5/fractal_server/images/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,28 +5,62 @@
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from fractal_server.app.schemas._validators import valdictkeys
 
 
-class SingleImage(BaseModel):
+class SingleImageBase(BaseModel):
+    """
+    Base for SingleImage and SingleImageTaskOutput.
+
+    Attributes:
+        zarr_url:
+        origin:
+        attributes:
+        types:
+    """
 
     zarr_url: str
     origin: Optional[str] = None
 
     attributes: dict[str, Any] = Field(default_factory=dict)
     types: dict[str, bool] = Field(default_factory=dict)
 
     # Validators
     _attributes = validator("attributes", allow_reuse=True)(
         valdictkeys("attributes")
     )
     _types = validator("types", allow_reuse=True)(valdictkeys("types"))
 
+
+class SingleImageTaskOutput(SingleImageBase):
+    """
+    `SingleImageBase`, with scalar `attributes` values (`None` included).
+    """
+
+    @validator("attributes")
+    def validate_attributes(
+        cls, v: dict[str, Any]
+    ) -> dict[str, Union[int, float, str, bool, None]]:
+        for key, value in v.items():
+            if not isinstance(value, (int, float, str, bool, type(None))):
+                raise ValueError(
+                    f"SingleImageTaskOutput.attributes[{key}] must be a "
+                    "scalar (int, float, str or bool). "
+                    f"Given {value} ({type(value)})"
+                )
+        return v
+
+
+class SingleImage(SingleImageBase):
+    """
+    `SingleImageBase`, with scalar `attributes` values (`None` excluded).
+    """
+
     @validator("attributes")
     def validate_attributes(
         cls, v: dict[str, Any]
     ) -> dict[str, Union[int, float, str, bool]]:
         for key, value in v.items():
             if not isinstance(value, (int, float, str, bool)):
                 raise ValueError(
```

### Comparing `fractal_server-2.0.0a4/fractal_server/images/tools.py` & `fractal_server-2.0.0a5/fractal_server/images/tools.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/logger.py` & `fractal_server-2.0.0a5/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/main.py` & `fractal_server-2.0.0a5/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/env.py` & `fractal_server-2.0.0a5/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/script.py.mako` & `fractal_server-2.0.0a5/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/d71e732236cd_v2.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/d71e732236cd_v2.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-2.0.0a5/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/syringe.py` & `fractal_server-2.0.0a5/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/tasks/endpoint_operations.py` & `fractal_server-2.0.0a5/fractal_server/tasks/endpoint_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/tasks/utils.py` & `fractal_server-2.0.0a5/fractal_server/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/tasks/v1/_TaskCollectPip.py` & `fractal_server-2.0.0a5/fractal_server/tasks/v1/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/tasks/v1/background_operations.py` & `fractal_server-2.0.0a5/fractal_server/tasks/v1/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/tasks/v2/_TaskCollectPip.py` & `fractal_server-2.0.0a5/fractal_server/tasks/v2/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/tasks/v2/background_operations.py` & `fractal_server-2.0.0a5/fractal_server/tasks/v2/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/fractal_server/utils.py` & `fractal_server-2.0.0a5/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a4/pyproject.toml` & `fractal_server-2.0.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "2.0.0a4"
+version = "2.0.0a5"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -82,15 +82,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "2.0.0a4"
+current_version = "2.0.0a5"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-2.0.0a4/PKG-INFO` & `fractal_server-2.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 2.0.0a4
+Version: 2.0.0a5
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

