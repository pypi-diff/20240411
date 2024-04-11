# Comparing `tmp/slurmpie-0.8.2.tar.gz` & `tmp/slurmpie-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slurmpie-0.8.2.tar", last modified: Mon Apr  8 13:58:25 2024, max compression
+gzip compressed data, was "dist/slurmpie-0.8.3.tar", last modified: Thu Apr 11 06:58:06 2024, max compression
```

## Comparing `slurmpie-0.8.2.tar` & `slurmpie-0.8.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:25.000000 slurmpie-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 13:58:03.000000 slurmpie-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-08 13:58:25.000000 slurmpie-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-08 13:58:03.000000 slurmpie-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 13:58:25.000000 slurmpie-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-08 13:58:03.000000 slurmpie-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:25.000000 slurmpie-0.8.2/slurmpie/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:03.000000 slurmpie-0.8.2/slurmpie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22661 2024-04-08 13:58:03.000000 slurmpie-0.8.2/slurmpie/slurmpie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:25.000000 slurmpie-0.8.2/slurmpie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-08 13:58:25.000000 slurmpie-0.8.2/slurmpie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 13:58:25.000000 slurmpie-0.8.2/slurmpie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:58:25.000000 slurmpie-0.8.2/slurmpie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 13:58:25.000000 slurmpie-0.8.2/slurmpie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:25.000000 slurmpie-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:03.000000 slurmpie-0.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-04-08 13:58:03.000000 slurmpie-0.8.2/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-08 13:58:03.000000 slurmpie-0.8.2/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:58:06.000000 slurmpie-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 06:57:47.000000 slurmpie-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-11 06:58:06.000000 slurmpie-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-11 06:57:47.000000 slurmpie-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-11 06:58:06.000000 slurmpie-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-11 06:57:47.000000 slurmpie-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:58:06.000000 slurmpie-0.8.3/slurmpie/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:47.000000 slurmpie-0.8.3/slurmpie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22813 2024-04-11 06:57:47.000000 slurmpie-0.8.3/slurmpie/slurmpie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:58:06.000000 slurmpie-0.8.3/slurmpie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-11 06:58:06.000000 slurmpie-0.8.3/slurmpie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-11 06:58:06.000000 slurmpie-0.8.3/slurmpie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 06:58:06.000000 slurmpie-0.8.3/slurmpie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 06:58:06.000000 slurmpie-0.8.3/slurmpie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:58:06.000000 slurmpie-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:47.000000 slurmpie-0.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-04-11 06:57:47.000000 slurmpie-0.8.3/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-11 06:57:47.000000 slurmpie-0.8.3/tests/test_pipeline.py
```

### Comparing `slurmpie-0.8.2/LICENSE` & `slurmpie-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slurmpie-0.8.2/PKG-INFO` & `slurmpie-0.8.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmpie
-Version: 0.8.2
+Version: 0.8.3
 Summary: Package to interact with SLURM
 Home-page: https://github.com/svdvoort/slurmpie
 Author: Sebastian van der Voort
 Author-email: Svdvoort@users.noreply.github.com
 License: UNKNOWN
 Description: # slurmpie
```

### Comparing `slurmpie-0.8.2/README.md` & `slurmpie-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `slurmpie-0.8.2/setup.py` & `slurmpie-0.8.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="slurmpie",
-    version="0.8.2",
+    version="0.8.3",
     author="Sebastian van der Voort",
     author_email="Svdvoort@users.noreply.github.com",
     description="Package to interact with SLURM",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/svdvoort/slurmpie",
     packages=setuptools.find_packages(),
```

### Comparing `slurmpie-0.8.2/slurmpie/slurmpie.py` & `slurmpie-0.8.3/slurmpie/slurmpie.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,20 +353,20 @@
         elif isinstance(attribute_value, dict) and attribute_value == {}:
             return True
         elif isinstance(attribute_value, list) and attribute_value == []:
             return True
         else:
             return False
 
-    def _format_sbatch_command(self) -> list:
+    def _format_sbatch_command(self) -> str:
         """
         Formats the command for sbatch from the job settings.
 
         Returns:
-            list: Formatted command with one argument per item.
+            str: Formatted command.
         """
 
         command_mapping = {
             "array": "array",
             "cpus_per_task": "cpus-per-task",
             "dependencies": "dependency",
             "error_file": "error",
@@ -396,15 +396,18 @@
                 command.append("--{}={}".format(bash_argument, attribute_value))
 
         if self.script_is_file:
             command.append(self.script)
         else:
             command.append("--wrap='{}'".format(self.script))
 
-        return command
+        # It's better to have it as a list for Popen
+        # but then it doesn't work with the quotes for the --wrap
+        # so we provide it as a string.
+        return " ".join(command)
 
     def submit(self) -> str:
         """
         Submit the job using `sbatch`
 
         Raises:
             RuntimeError: If `sbatch` returns an error
@@ -413,15 +416,15 @@
             str: The job number of the submitted job if successful
         """
 
         # The submission is not currently tested, since it requires a slurm install
         # Perhaps a docker with slurm pre-installed is a good idea in this case
         sbatch_command = self._format_sbatch_command()
         sbatch_process = subprocess.Popen(
-            sbatch_command, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+            sbatch_command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
         )
 
         stdout, stderr = sbatch_process.communicate()
 
         if sbatch_process.returncode != 0 or "error" in stdout.decode("utf-8").lower():
             submitted_command = " ".join(sbatch_command)
             err_msg = "Sbatch job submission failed with follow error:\n{msg}\nSubmitted using the following command:\n{submitted_command}"
```

### Comparing `slurmpie-0.8.2/slurmpie.egg-info/PKG-INFO` & `slurmpie-0.8.3/slurmpie.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmpie
-Version: 0.8.2
+Version: 0.8.3
 Summary: Package to interact with SLURM
 Home-page: https://github.com/svdvoort/slurmpie
 Author: Sebastian van der Voort
 Author-email: Svdvoort@users.noreply.github.com
 License: UNKNOWN
 Description: # slurmpie
```

### Comparing `slurmpie-0.8.2/tests/test_jobs.py` & `slurmpie-0.8.3/tests/test_jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import pytest
 from slurmpie import slurmpie
 import os
 
-FIXTURE_DIR = os.path.join(os.path.dirname(os.path.realpath(__file__)), "test_data",)
+FIXTURE_DIR = os.path.join(
+    os.path.dirname(os.path.realpath(__file__)),
+    "test_data",
+)
 
 
-@pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "slurm_script.sh"),)
+@pytest.mark.datafiles(
+    os.path.join(FIXTURE_DIR, "slurm_script.sh"),
+)
 def test_init(datafiles):
     script_file = str(datafiles)
     job = slurmpie.Job(script_file)
     job_2 = slurmpie.Job(script_file)
     assert job._id != job_2._id
 
     job = slurmpie.Job(script_file, mail_address="user@example.com")
@@ -18,28 +23,32 @@
     job = slurmpie.Job(script_file, mail_address="user@example.com", mail_type="FAIL")
     assert job.mail_type == "FAIL"
 
     job = slurmpie.Job(script_file, memory_size="50GB")
     assert job.memory_size == "50G"
 
 
-@pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "slurm_script.sh"),)
+@pytest.mark.datafiles(
+    os.path.join(FIXTURE_DIR, "slurm_script.sh"),
+)
 def test_argument_list_formatting(datafiles):
     script_file = str(datafiles)
     job = slurmpie.Job(script_file)
 
     assert job._format_argument_list("", "") == ""
     assert job._format_argument_list("", "new_value") == "new_value"
     assert job._format_argument_list("old_value", "") == "old_value"
     assert job._format_argument_list("old_value", "new_value") == "old_value,new_value"
     assert job._format_argument_list("gpu:1", "cpu:3") == "gpu:1,cpu:3"
     assert job._format_argument_list("gpu:1,cpu:3", "ssd:4") == "gpu:1,cpu:3,ssd:4"
 
 
-@pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "slurm_script.sh"),)
+@pytest.mark.datafiles(
+    os.path.join(FIXTURE_DIR, "slurm_script.sh"),
+)
 def test_gres_formatting(datafiles):
     script_file = str(datafiles)
     job = slurmpie.Job(script_file)
 
     assert job._format_gres({}) == ""
     assert job._format_gres({"gpu": 1}) == "gpu:1"
     assert job._format_gres({"gpu": 1, "ssd": 3}) == "gpu:1,ssd:3"
@@ -51,15 +60,18 @@
     assert (
         job._format_gres(
             {"gpu": {"Titan": 3, "k40": 2}, "ssd": {"fast": 2, "slow": 1}, "cpu": 15}
         )
         == "cpu:15,gpu:k40:2,gpu:Titan:3,ssd:fast:2,ssd:slow:1"
     )
 
-@pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "slurm_script.sh"),)
+
+@pytest.mark.datafiles(
+    os.path.join(FIXTURE_DIR, "slurm_script.sh"),
+)
 def test_gres_settting(datafiles):
     script_file = str(datafiles)
     job = slurmpie.Job(script_file)
 
     job.gres = {}
     assert job.gres == ""
 
@@ -79,15 +91,18 @@
     job.gres = {"gpu": {"Titan": 3, "k40": 2}, "ssd": 3}
     assert job.gres == "gpu:k40:2,gpu:Titan:3,ssd:3"
 
     job = slurmpie.Job(script_file)
     job.gres = {"gpu": {"Titan": 3, "k40": 2}, "ssd": {"fast": 2, "slow": 1}, "cpu": 15}
     assert job.gres == "cpu:15,gpu:k40:2,gpu:Titan:3,ssd:fast:2,ssd:slow:1"
 
-@pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "slurm_script.sh"),)
+
+@pytest.mark.datafiles(
+    os.path.join(FIXTURE_DIR, "slurm_script.sh"),
+)
 def test_memory_formatting(datafiles):
     script_file = str(datafiles)
     job = slurmpie.Job(script_file)
 
     memory_size, memory_units = job._format_memory_size("50M")
     assert memory_size == "50"
     assert memory_units == "M"
@@ -101,15 +116,17 @@
     assert memory_units is None
 
     memory_size, memory_units = job._format_memory_size("25000")
     assert memory_size == "25000"
     assert memory_units is None
 
 
-@pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "slurm_script.sh"),)
+@pytest.mark.datafiles(
+    os.path.join(FIXTURE_DIR, "slurm_script.sh"),
+)
 def test_memory_setting(datafiles):
     script_file = str(datafiles)
     job = slurmpie.Job(script_file)
 
     assert job.memory_size == ""
     assert job.memory_units is None
 
@@ -120,15 +137,17 @@
 
     job.memory_size = 213.5
 
     assert job.memory_size == "214"
     assert job.memory_units is None
 
 
-@pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "slurm_script.sh"),)
+@pytest.mark.datafiles(
+    os.path.join(FIXTURE_DIR, "slurm_script.sh"),
+)
 def test_job_dependencies(datafiles):
     script_file = str(datafiles)
     job = slurmpie.Job(script_file)
 
     assert job.dependencies == ""
 
     job = slurmpie.Job(script_file)
@@ -153,15 +172,17 @@
     job.depends_on(["1001", "9040294"], "afterok")
     job.depends_on("123", "afternotok")
     job.depends_on("987", "afterok")
 
     assert job.dependencies == "afterok:1001:9040294,afternotok:123,afterok:987"
 
 
-@pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "slurm_script.sh"),)
+@pytest.mark.datafiles(
+    os.path.join(FIXTURE_DIR, "slurm_script.sh"),
+)
 def test_array_setting(datafiles):
     script_file = str(datafiles)
     job = slurmpie.Job(script_file)
     assert job.array == ""
 
     job = slurmpie.Job(script_file)
     job.array = [5, 9, 10]
@@ -172,30 +193,34 @@
     assert job.array == "1,5,101"
 
     job = slurmpie.Job(script_file)
     job.array = "0-15%4"
     assert job.array == "0-15%4"
 
 
-@pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "slurm_script.sh"),)
+@pytest.mark.datafiles(
+    os.path.join(FIXTURE_DIR, "slurm_script.sh"),
+)
 def test_gpu_setting(datafiles):
     script_file = str(datafiles)
     job = slurmpie.Job(script_file)
     assert job.gpus == ""
 
     job = slurmpie.Job(script_file)
-    job.gpus = {'Titan': 5}
+    job.gpus = {"Titan": 5}
     assert job.gpus == "Titan:5"
 
     job = slurmpie.Job(script_file)
-    job.gpus = {'Titan': 5, "k40": "3"}
+    job.gpus = {"Titan": 5, "k40": "3"}
     assert job.gpus == "k40:3,Titan:5"
 
 
-@pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "slurm_script.sh"),)
+@pytest.mark.datafiles(
+    os.path.join(FIXTURE_DIR, "slurm_script.sh"),
+)
 def test_empty_attributes(datafiles):
     script_file = str(datafiles)
     job = slurmpie.Job(script_file)
 
     assert job.attribute_is_empty("")
     assert job.attribute_is_empty(-1)
     assert job.attribute_is_empty(-1.0)
@@ -203,50 +228,85 @@
     assert job.attribute_is_empty([])
     assert not job.attribute_is_empty("-1")
     assert not job.attribute_is_empty([""])
     assert not job.attribute_is_empty({"a": "b"})
     assert not job.attribute_is_empty([-1])
 
 
-
-@pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "slurm_script.sh"),)
+@pytest.mark.datafiles(
+    os.path.join(FIXTURE_DIR, "slurm_script.sh"),
+)
 def test_sbatch_formatting(datafiles):
     script_file = str(datafiles)
     job = slurmpie.Job(script_file)
 
     sbatch_command = job._format_sbatch_command()
-    assert sbatch_command == ["sbatch", "--parsable", script_file]
+    assert sbatch_command == " ".join(["sbatch", "--parsable", script_file])
 
     job.memory_size = 50
 
     sbatch_command = job._format_sbatch_command()
-    assert sbatch_command == ["sbatch", "--parsable", "--mem=50", script_file]
+    assert sbatch_command == " ".join(["sbatch", "--parsable", "--mem=50", script_file])
 
     job.gres = {"gpu": {"Titan": 1, "k40": 2}}
 
-    assert job._format_sbatch_command() == ["sbatch", "--parsable", "--gres=gpu:k40:2,gpu:Titan:1", "--mem=50", script_file]
+    assert job._format_sbatch_command() == " ".join(
+        [
+            "sbatch",
+            "--parsable",
+            "--gres=gpu:k40:2,gpu:Titan:1",
+            "--mem=50",
+            script_file,
+        ]
+    )
 
     job = slurmpie.Job(script_file, memory_size="100GB", name="test_job")
-    assert job._format_sbatch_command() == ["sbatch", "--parsable", "--mem=100G", "--job-name=test_job", script_file]
+    assert job._format_sbatch_command() == " ".join(
+        [
+            "sbatch",
+            "--parsable",
+            "--mem=100G",
+            "--job-name=test_job",
+            script_file,
+        ]
+    )
 
-    job = slurmpie.Job(script_file, array=[1, 2, 3], cpus_per_task=5, error_file="/tmp/error.log", gpus={'Titan':8},
-    gres={'cpus': {'haskell':2, 'lake': "3"}}, mail_address="user@example.com", mail_type="FAIL", memory_size="10KB",
-    name="test_job", nodes=4, output_file="/tmp/output.log", partition="test_partition", tasks=7, time="01:33",
-    workdir="/tmp/workdir")
-    assert job._format_sbatch_command() == ["sbatch",
-                                            "--parsable",
-                                            "--array=1,2,3",
-                                            "--cpus-per-task=5",
-                                            "--error=/tmp/error.log",
-                                            "--gpus=Titan:8",
-                                            "--gres=cpus:haskell:2,cpus:lake:3",
-                                            "--mail-user=user@example.com",
-                                            "--mail-type=FAIL",
-                                            "--mem=10K",
-                                            "--job-name=test_job",
-                                            "--nodes=4",
-                                            "--output=/tmp/output.log",
-                                            "--partition=test_partition",
-                                            "--ntasks=7",
-                                            "--time=01:33",
-                                            "--chdir=/tmp/workdir",
-                                            script_file]
+    job = slurmpie.Job(
+        script_file,
+        array=[1, 2, 3],
+        cpus_per_task=5,
+        error_file="/tmp/error.log",
+        gpus={"Titan": 8},
+        gres={"cpus": {"haskell": 2, "lake": "3"}},
+        mail_address="user@example.com",
+        mail_type="FAIL",
+        memory_size="10KB",
+        name="test_job",
+        nodes=4,
+        output_file="/tmp/output.log",
+        partition="test_partition",
+        tasks=7,
+        time="01:33",
+        workdir="/tmp/workdir",
+    )
+    assert job._format_sbatch_command() == " ".join(
+        [
+            "sbatch",
+            "--parsable",
+            "--array=1,2,3",
+            "--cpus-per-task=5",
+            "--error=/tmp/error.log",
+            "--gpus=Titan:8",
+            "--gres=cpus:haskell:2,cpus:lake:3",
+            "--mail-user=user@example.com",
+            "--mail-type=FAIL",
+            "--mem=10K",
+            "--job-name=test_job",
+            "--nodes=4",
+            "--output=/tmp/output.log",
+            "--partition=test_partition",
+            "--ntasks=7",
+            "--time=01:33",
+            "--chdir=/tmp/workdir",
+            script_file,
+        ]
+    )
```

### Comparing `slurmpie-0.8.2/tests/test_pipeline.py` & `slurmpie-0.8.3/tests/test_pipeline.py`

 * *Files identical despite different names*

