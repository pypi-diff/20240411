# Comparing `tmp/CADET-RDM-0.0.6.tar.gz` & `tmp/CADET-RDM-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CADET-RDM-0.0.6.tar", last modified: Wed Nov 22 18:55:11 2023, max compression
+gzip compressed data, was "CADET-RDM-0.0.9.tar", last modified: Tue Dec  5 11:50:46 2023, max compression
```

## Comparing `CADET-RDM-0.0.6.tar` & `CADET-RDM-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-11-22 18:55:11.663071 CADET-RDM-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-11-22 18:55:11.662070 CADET-RDM-0.0.6/CADET_RDM.egg-info/
--rw-rw-rw-   0        0        0     4371 2023-11-22 18:55:11.000000 CADET-RDM-0.0.6/CADET_RDM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-11-22 18:55:11.000000 CADET-RDM-0.0.6/CADET_RDM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-22 18:55:11.000000 CADET-RDM-0.0.6/CADET_RDM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-11-22 18:55:11.000000 CADET-RDM-0.0.6/CADET_RDM.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      123 2023-11-22 18:55:11.000000 CADET-RDM-0.0.6/CADET_RDM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-11-22 18:55:11.000000 CADET-RDM-0.0.6/CADET_RDM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2023-08-14 14:33:48.000000 CADET-RDM-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     4371 2023-11-22 18:55:11.663071 CADET-RDM-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3274 2023-11-22 18:40:16.000000 CADET-RDM-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-11-22 18:55:11.659071 CADET-RDM-0.0.6/cadetrdm/
--rw-rw-rw-   0        0        0      182 2023-11-22 18:00:54.000000 CADET-RDM-0.0.6/cadetrdm/__init__.py
--rw-rw-rw-   0        0        0     3454 2023-11-22 18:00:54.000000 CADET-RDM-0.0.6/cadetrdm/cli_integration.py
--rw-rw-rw-   0        0        0      708 2023-09-01 14:10:57.000000 CADET-RDM-0.0.6/cadetrdm/conda_env_utils.py
--rw-rw-rw-   0        0        0     8331 2023-11-22 18:00:54.000000 CADET-RDM-0.0.6/cadetrdm/initialize_repo.py
--rw-rw-rw-   0        0        0     1613 2023-11-22 18:00:54.000000 CADET-RDM-0.0.6/cadetrdm/io_utils.py
--rw-rw-rw-   0        0        0    37156 2023-11-22 18:00:54.000000 CADET-RDM-0.0.6/cadetrdm/repositories.py
--rw-rw-rw-   0        0        0      330 2023-11-22 18:00:54.000000 CADET-RDM-0.0.6/cadetrdm/web_utils.py
--rw-rw-rw-   0        0        0       88 2023-08-28 11:00:36.000000 CADET-RDM-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0     1185 2023-11-22 18:55:11.665071 CADET-RDM-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0       96 2023-08-14 14:13:04.000000 CADET-RDM-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-22 18:55:11.661071 CADET-RDM-0.0.6/tests/
--rw-rw-rw-   0        0        0        0 2023-08-17 16:03:58.000000 CADET-RDM-0.0.6/tests/__init__.py
--rw-rw-rw-   0        0        0     8459 2023-11-22 18:00:54.000000 CADET-RDM-0.0.6/tests/test_git_adapter.py
+drwxrwxrwx   0        0        0        0 2023-12-05 11:50:46.452744 CADET-RDM-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-12-05 11:50:46.450743 CADET-RDM-0.0.9/CADET_RDM.egg-info/
+-rw-rw-rw-   0        0        0     5999 2023-12-05 11:50:46.000000 CADET-RDM-0.0.9/CADET_RDM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2023-12-05 11:50:46.000000 CADET-RDM-0.0.9/CADET_RDM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-05 11:50:46.000000 CADET-RDM-0.0.9/CADET_RDM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-12-05 11:50:46.000000 CADET-RDM-0.0.9/CADET_RDM.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      155 2023-12-05 11:50:46.000000 CADET-RDM-0.0.9/CADET_RDM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-12-05 11:50:46.000000 CADET-RDM-0.0.9/CADET_RDM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2023-08-14 14:33:48.000000 CADET-RDM-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5999 2023-12-05 11:50:46.452744 CADET-RDM-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4806 2023-12-04 15:29:00.000000 CADET-RDM-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-12-05 11:50:46.447743 CADET-RDM-0.0.9/cadetrdm/
+-rw-rw-rw-   0        0        0      195 2023-12-04 15:29:00.000000 CADET-RDM-0.0.9/cadetrdm/__init__.py
+-rw-rw-rw-   0        0        0     4206 2023-12-04 15:29:00.000000 CADET-RDM-0.0.9/cadetrdm/cli_integration.py
+-rw-rw-rw-   0        0        0      708 2023-09-01 14:10:57.000000 CADET-RDM-0.0.9/cadetrdm/conda_env_utils.py
+-rw-rw-rw-   0        0        0    10080 2023-12-04 16:09:05.000000 CADET-RDM-0.0.9/cadetrdm/initialize_repo.py
+-rw-rw-rw-   0        0        0     2386 2023-12-04 16:09:55.000000 CADET-RDM-0.0.9/cadetrdm/io_utils.py
+-rw-rw-rw-   0        0        0     5610 2023-12-04 16:36:13.000000 CADET-RDM-0.0.9/cadetrdm/jupyter_functionality.py
+-rw-rw-rw-   0        0        0    40631 2023-12-04 16:36:02.000000 CADET-RDM-0.0.9/cadetrdm/repositories.py
+-rw-rw-rw-   0        0        0       19 2023-12-05 11:49:11.000000 CADET-RDM-0.0.9/cadetrdm/version.py
+-rw-rw-rw-   0        0        0      330 2023-12-04 15:29:00.000000 CADET-RDM-0.0.9/cadetrdm/web_utils.py
+-rw-rw-rw-   0        0        0       88 2023-08-28 11:00:36.000000 CADET-RDM-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1225 2023-12-05 11:50:46.453743 CADET-RDM-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       96 2023-08-14 14:13:04.000000 CADET-RDM-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-05 11:50:46.449743 CADET-RDM-0.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2023-08-17 16:03:58.000000 CADET-RDM-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     9039 2023-12-04 15:29:00.000000 CADET-RDM-0.0.9/tests/test_git_adapter.py
```

### Comparing `CADET-RDM-0.0.6/CADET_RDM.egg-info/PKG-INFO` & `CADET-RDM-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,38 @@
-Metadata-Version: 2.1
-Name: CADET-RDM
-Version: 0.0.6
-Summary: A solution for research data management
-Home-page: https://jugit.fz-juelich.de/IBG-1/ModSim/cadet/CADET-RDM
-Author: Ronald Jäpel
-Author-email: r.jaepel@fz-juelich.de
-Project-URL: Bug Tracker, https://jugit.fz-juelich.de/IBG-1/ModSim/cadet/CADET-RDM/Issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: gitpython>=3.1
-Requires-Dist: git-lfs
-Requires-Dist: click
-Requires-Dist: tabulate
-Requires-Dist: pandas
-Provides-Extra: testing
-Requires-Dist: setuptools; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
-Requires-Dist: certifi; extra == "testing"
-Requires-Dist: pre-commit; extra == "testing"
-Requires-Dist: flake8; extra == "testing"
-Requires-Dist: matplotlib; extra == "testing"
-Requires-Dist: numpy; extra == "testing"
-Requires-Dist: build; extra == "testing"
-
 # The CADET-Research Data Management toolbox
 
 ## Getting started
+
 ### Installation
+
 CADET-RDM can be installed using
 
 ```pip install cadet-rdm```
 
 ### Initialize Project Repository
+
 Create a new project repository or convert an existing repository into a CADET-RDM repo:
 
 ```bash
 cadet-rdm initialize-repo <path-to-repo>
 ```
+
 or from python
 
 ```python
 from cadetrdm import initialize_repo
+
 initialize_repo(path_to_repo)
 ```
 
 The `output_folder_name` can be given optionally. It defaults to `output`.
 
-### Use CADET-RDM in Python
-#### Tracking Results
+## Use CADET-RDM in Python
+
+### Tracking Results
 
 ```python
 from cadetrdm import ProjectRepo
 
 """
 Your imports and function declarations
 e.g. generate_data(), write_data_to_file(), analyse_data() and plot_analysis_results()
@@ -72,61 +49,114 @@
     # The method repo.output_data() generates full paths to within your output_folder
     with repo.track_results(results_commit_message="Generate and analyse example data"):
         data = generate_data()
         output_filepath = repo.output_data(sub_path="raw_data/data.csv")
         write_data_to_file(data, output_filepath)
 
         analysis_results = analyse_data(data)
-        figure_path=repo.output_data("analysis/regression.png")
+        figure_path = repo.output_data("analysis/regression.png")
         plot_analysis_results(analysis_results, figure_path)
 
 ```
 
-#### Sharing Results
+### Sharing Results
 
-To share your project code and results with others, you need to create remote repositories on e.g. 
+To share your project code and results with others, you need to create remote repositories on e.g.
 [GitHub](https://github.com/) or GitLab. You need to create a remote for both the _project_ repo and the
 _results_ repo.
 
 Once created, the remotes need to be added to the local repositories.
 
 ```bash
-cadet-rdm add-remote-to-repo <path_to_repo> git@<my_git_server.foo>:<project>.git
-cadet-rdm add-remote-to-repo <path_to_repo/output_folder> git@<my_git_server.foo>:<project>_output.git
+cadet-rdm add-remote-to-repo git@<my_git_server.foo>:<project>.git
+cadet-rdm --path_to_repo output add-remote-to-repo git@<my_git_server.foo>:<project>_output.git
 ```
+
 or in Python:
 
 ```python
 repo = ProjectRepo()
 repo.add_remote("git@<my_git_server.foo>:<project>.git")
 repo.output_repo.add_remote("git@<my_git_server.foo>:<project>_output.git")
 ```
 
-Once remotes are configured, you can push all changes to the project repo and the results repos with the 
+Once remotes are configured, you can push all changes to the project repo and the results repos with the
 command
 
 ```python
 # push all changes to the Project and Output repositories with one command:
 repo.push()
 ```
 
-
-#### Re-using results from previous iterations
+### Re-using results from previous iterations
 
 Each result stored with CADET-RDM is given a unique branch name, formatted as:
 `<timestamp>_<output_folder>_"from"_<active_project_branch>_<project_repo_hash[:7]>`
 
-With this branch name, previously generated data can be loaded in as input data for 
+With this branch name, previously generated data can be loaded in as input data for
 further calculations.
 
 ```python
 cached_array_path = repo.input_data(branch_name=branch_name, source_file_path="raw_data/data.csv")
 ```
 
 Alternatively, using the auto-generated cache of previous results, CADET-RDM can infer
 the correct branch name from the path to the file within the cache
 
 ```python
 cached_array_path = repo.input_data(source_file_path="output_cached/<branch_name>/raw_data/data.csv")
 ```
 
+## Use CADET RDM from the CLI
+
+### Executing scripts
+
+You can execute python files or arbitray commands using the CLI:
+
+```bash
+cd path/to/your/project
+cadet-rdm run-python-file <path/to/file> "commit message for the results"
+cadet-rdm run-command "command as it would be run" "commit message for the results"
+```
+
+For the run-command option, the command must be given in quotes, so:
+
+```bash
+cadet-rdm run-command "python example_file.py" "commit message for the results"
+```
 
+
+### Using results from another repository
+
+You can load in results from another repository to use in your project using the CLI:
+
+```bash
+cd path/to/your/project
+cadet-rdm import-remote-repo <URL> <branch_name>
+cadet-rdm import-remote-repo <URL> <branch_name> --target_repo_location <path/to/where/you/want/it>
+```
+
+This will store the URL, branch_name and location in the .cadet-rdm-cache.json file, like this:
+
+```json
+{
+  "__example/path/to/repo__": {
+    "source_repo_location": "git@jugit.fz-juelich.de:IBG-1/ModSim/cadet/agile_cadet_rdm_presentation_output.git",
+    "branch_name": "output_from_master_3910c84_2023-10-25_00-17-23",
+    "commit_hash": "6e3c26527999036e9490d2d86251258fe81d46dc"
+  }
+}
+```
+
+You can use this file to load the remote repositories based on the cache.json with
+
+```bash
+cadet-rdm fill-data-from-cadet-rdm-json
+```
+
+### Cloning from remote
+
+You should use `cadet-rdm clone` instead of `git clone` to clone the repo to a new location.
+
+```bash
+cadet-rdm clone <URL> <path/to/repo>
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `CADET-RDM-0.0.6/LICENSE` & `CADET-RDM-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CADET-RDM-0.0.6/PKG-INFO` & `CADET-RDM-0.0.9/CADET_RDM.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CADET-RDM
-Version: 0.0.6
+Version: 0.0.9
 Summary: A solution for research data management
 Home-page: https://jugit.fz-juelich.de/IBG-1/ModSim/cadet/CADET-RDM
 Author: Ronald Jäpel
 Author-email: r.jaepel@fz-juelich.de
 Project-URL: Bug Tracker, https://jugit.fz-juelich.de/IBG-1/ModSim/cadet/CADET-RDM/Issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,49 +13,59 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gitpython>=3.1
 Requires-Dist: git-lfs
 Requires-Dist: click
 Requires-Dist: tabulate
 Requires-Dist: pandas
+Requires-Dist: nbformat
+Requires-Dist: nbconvert
+Requires-Dist: ipylab
+Requires-Dist: junix
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: certifi; extra == "testing"
 Requires-Dist: pre-commit; extra == "testing"
 Requires-Dist: flake8; extra == "testing"
 Requires-Dist: matplotlib; extra == "testing"
 Requires-Dist: numpy; extra == "testing"
 Requires-Dist: build; extra == "testing"
 
 # The CADET-Research Data Management toolbox
 
 ## Getting started
+
 ### Installation
+
 CADET-RDM can be installed using
 
 ```pip install cadet-rdm```
 
 ### Initialize Project Repository
+
 Create a new project repository or convert an existing repository into a CADET-RDM repo:
 
 ```bash
 cadet-rdm initialize-repo <path-to-repo>
 ```
+
 or from python
 
 ```python
 from cadetrdm import initialize_repo
+
 initialize_repo(path_to_repo)
 ```
 
 The `output_folder_name` can be given optionally. It defaults to `output`.
 
-### Use CADET-RDM in Python
-#### Tracking Results
+## Use CADET-RDM in Python
+
+### Tracking Results
 
 ```python
 from cadetrdm import ProjectRepo
 
 """
 Your imports and function declarations
 e.g. generate_data(), write_data_to_file(), analyse_data() and plot_analysis_results()
@@ -72,61 +82,114 @@
     # The method repo.output_data() generates full paths to within your output_folder
     with repo.track_results(results_commit_message="Generate and analyse example data"):
         data = generate_data()
         output_filepath = repo.output_data(sub_path="raw_data/data.csv")
         write_data_to_file(data, output_filepath)
 
         analysis_results = analyse_data(data)
-        figure_path=repo.output_data("analysis/regression.png")
+        figure_path = repo.output_data("analysis/regression.png")
         plot_analysis_results(analysis_results, figure_path)
 
 ```
 
-#### Sharing Results
+### Sharing Results
 
-To share your project code and results with others, you need to create remote repositories on e.g. 
+To share your project code and results with others, you need to create remote repositories on e.g.
 [GitHub](https://github.com/) or GitLab. You need to create a remote for both the _project_ repo and the
 _results_ repo.
 
 Once created, the remotes need to be added to the local repositories.
 
 ```bash
-cadet-rdm add-remote-to-repo <path_to_repo> git@<my_git_server.foo>:<project>.git
-cadet-rdm add-remote-to-repo <path_to_repo/output_folder> git@<my_git_server.foo>:<project>_output.git
+cadet-rdm add-remote-to-repo git@<my_git_server.foo>:<project>.git
+cadet-rdm --path_to_repo output add-remote-to-repo git@<my_git_server.foo>:<project>_output.git
 ```
+
 or in Python:
 
 ```python
 repo = ProjectRepo()
 repo.add_remote("git@<my_git_server.foo>:<project>.git")
 repo.output_repo.add_remote("git@<my_git_server.foo>:<project>_output.git")
 ```
 
-Once remotes are configured, you can push all changes to the project repo and the results repos with the 
+Once remotes are configured, you can push all changes to the project repo and the results repos with the
 command
 
 ```python
 # push all changes to the Project and Output repositories with one command:
 repo.push()
 ```
 
-
-#### Re-using results from previous iterations
+### Re-using results from previous iterations
 
 Each result stored with CADET-RDM is given a unique branch name, formatted as:
 `<timestamp>_<output_folder>_"from"_<active_project_branch>_<project_repo_hash[:7]>`
 
-With this branch name, previously generated data can be loaded in as input data for 
+With this branch name, previously generated data can be loaded in as input data for
 further calculations.
 
 ```python
 cached_array_path = repo.input_data(branch_name=branch_name, source_file_path="raw_data/data.csv")
 ```
 
 Alternatively, using the auto-generated cache of previous results, CADET-RDM can infer
 the correct branch name from the path to the file within the cache
 
 ```python
 cached_array_path = repo.input_data(source_file_path="output_cached/<branch_name>/raw_data/data.csv")
 ```
 
+## Use CADET RDM from the CLI
+
+### Executing scripts
+
+You can execute python files or arbitray commands using the CLI:
+
+```bash
+cd path/to/your/project
+cadet-rdm run-python-file <path/to/file> "commit message for the results"
+cadet-rdm run-command "command as it would be run" "commit message for the results"
+```
+
+For the run-command option, the command must be given in quotes, so:
+
+```bash
+cadet-rdm run-command "python example_file.py" "commit message for the results"
+```
+
+
+### Using results from another repository
+
+You can load in results from another repository to use in your project using the CLI:
+
+```bash
+cd path/to/your/project
+cadet-rdm import-remote-repo <URL> <branch_name>
+cadet-rdm import-remote-repo <URL> <branch_name> --target_repo_location <path/to/where/you/want/it>
+```
+
+This will store the URL, branch_name and location in the .cadet-rdm-cache.json file, like this:
+
+```json
+{
+  "__example/path/to/repo__": {
+    "source_repo_location": "git@jugit.fz-juelich.de:IBG-1/ModSim/cadet/agile_cadet_rdm_presentation_output.git",
+    "branch_name": "output_from_master_3910c84_2023-10-25_00-17-23",
+    "commit_hash": "6e3c26527999036e9490d2d86251258fe81d46dc"
+  }
+}
+```
 
+You can use this file to load the remote repositories based on the cache.json with
+
+```bash
+cadet-rdm fill-data-from-cadet-rdm-json
+```
+
+### Cloning from remote
+
+You should use `cadet-rdm clone` instead of `git clone` to clone the repo to a new location.
+
+```bash
+cadet-rdm clone <URL> <path/to/repo>
+```
```

### Comparing `CADET-RDM-0.0.6/cadetrdm/cli_integration.py` & `CADET-RDM-0.0.9/cadetrdm/cli_integration.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,80 @@
+import shlex
+import subprocess
+
 import click
 
-from .repositories import ProjectRepo
+from .repositories import ProjectRepo, BaseRepo
 from .initialize_repo import initialize_repo as initialize_git_repo_implementation, init_lfs
-from .initialize_repo import initialize_from_remote as initialize_from_remote_implementation
+from .initialize_repo import clone as clone_implementation
 from .conda_env_utils import prepare_conda_env as prepare_conda_env_implementation
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 def cli():
     pass
 
 
 @cli.command()
 @click.option('--path_to_repo', default=None,
               help='Path to folder for the repository. Optional.')
 @click.argument('project_url')
-def initialize_from_remote(project_url, path_to_repo: str = None):
-    initialize_from_remote_implementation(project_url, path_to_repo)
+def clone(project_url, path_to_repo: str = None):
+    clone_implementation(project_url, path_to_repo)
 
 
 @cli.command()
 @click.option('--target_repo_location', default=None,
               help='Path to folder for the repository. Optional.')
 @click.argument('source_repo_location')
 @click.argument('source_repo_branch')
 def import_remote_repo(source_repo_location, source_repo_branch, target_repo_location=None):
-    repo = ProjectRepo(".")
+    repo = BaseRepo(".")
     repo.import_remote_repo(source_repo_location=source_repo_location,
                             source_repo_branch=source_repo_branch,
                             target_repo_location=target_repo_location)
 
 
 @cli.command()
 def verify_unchanged_cache():
-    repo = ProjectRepo(".")
+    repo = BaseRepo(".")
     repo.verify_unchanged_cache()
 
 
 @cli.command()
 @click.option('--re_load', default=False,
               help='Re-load all data.')
 def fill_data_from_cadet_rdm_json(re_load=False):
-    repo = ProjectRepo(".")
+    repo = BaseRepo(".")
     repo.fill_data_from_cadet_rdm_json(re_load=re_load)
 
 
 @cli.command()
+@click.argument('file_name')
+@click.argument('results_commit_message')
+def run_python_file(file_name, results_commit_message):
+    repo = ProjectRepo(".")
+    repo.enter_context()
+    subprocess.run(["python", file_name])
+    repo.exit_context(results_commit_message)
+
+
+@cli.command()
+@click.argument('command')
+@click.argument('results_commit_message')
+def run_command(command, results_commit_message):
+    repo = ProjectRepo(".")
+    repo.enter_context()
+    subprocess.run(shlex.split(command))
+    repo.exit_context(results_commit_message)
+
+
+@cli.command()
 @click.option('--output_repo_name', default="output",
               help='Name of the folder where the tracked output should be stored. Optional. Default: "output".')
 @click.option('--gitignore', default=None,
               help='List of files to be added to the gitignore file. Optional.')
 @click.option('--gitattributes', default=None,
               help='List of files to be added to the gitattributes file. Optional.')
 @click.option('--lfs_filetypes', default=None,
@@ -62,34 +85,37 @@
                     output_repo_kwargs: dict = None):
     initialize_git_repo_implementation(path_to_repo, output_repo_name, gitignore,
                                        gitattributes, lfs_filetypes,
                                        output_repo_kwargs)
 
 
 @cli.command()
+@click.option("-p", '--path_to_repo', default=".",
+              help='Path to repository to which the remote is added. Default is cwd.')
 @click.argument('remote_url')
-def add_remote_to_repo(remote_url: str, ):
-    repo = ProjectRepo(".")
+def add_remote_to_repo(remote_url: str, path_to_repo="."):
+    repo = BaseRepo(path_to_repo)
     repo.add_remote(remote_url)
     print("Done.")
 
 
 @cli.command()
 @click.argument('file_type')
 def add_file_type_to_lfs(file_type: str, ):
     init_lfs(lfs_filetypes=[file_type], path=".")
-    repo = ProjectRepo(".")
+    repo = BaseRepo(".")
     repo.add_all_files()
     repo.commit(f"Add {file_type} to lfs")
 
 
 @cli.command()
 @click.option('--url', default=None,
               help='Url to the environment.yml file.')
 def prepare_conda_env(url):
     prepare_conda_env_implementation(url)
 
 
 @cli.command()
 def print_output_log():
+    # ToDo: test if Project or Output repo
     repo = ProjectRepo(".")
     repo.print_output_log()
```

### Comparing `CADET-RDM-0.0.6/cadetrdm/conda_env_utils.py` & `CADET-RDM-0.0.9/cadetrdm/conda_env_utils.py`

 * *Files identical despite different names*

### Comparing `CADET-RDM-0.0.6/cadetrdm/initialize_repo.py` & `CADET-RDM-0.0.9/cadetrdm/initialize_repo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 import json
 import uuid
+from pathlib import Path
 
 try:
     import git
 except ImportError:
     # Adding this hint to save users the confusion of trying $pip install git
     raise ImportError("No module named git, please install the gitpython package")
 
 import cadetrdm
 from cadetrdm.repositories import ProjectRepo, OutputRepo
 from cadetrdm.web_utils import ssh_url_to_http_url
-from cadetrdm.io_utils import write_lines_to_file, is_tool
+from cadetrdm.io_utils import write_lines_to_file, is_tool, wait_for_user
 
 
 def init_lfs(lfs_filetypes: list, path: str = None):
     """
     Initialize lfs in the git repository at the path.
     If path is None, the current working directory is used.
     :param lfs_filetypes:
@@ -33,126 +34,183 @@
     os.system(f"git lfs track {lfs_filetypes_string}")
 
     if path is not None:
         os.chdir(previous_path)
 
 
 def initialize_repo(path_to_repo: str, output_folder_name: (str | bool) = "output", gitignore: list = None,
-                    gitattributes: list = None, lfs_filetypes: list = None,
-                    output_repo_kwargs: dict = None):
+                    gitattributes: list = None, output_repo_kwargs: dict = None):
     """
     Initialize a git repository at the given path with an optional included output results repository.
 
     :param path_to_repo:
         Path to main repository.
     :param output_folder_name:
         Name for the output repository.
     :param gitignore:
         List of files to be added to the gitignore file.
     :param gitattributes:
-        List of lines to be added to the gittatributes file
-    :param lfs_filetypes:
-        List of filetypes to be handled by git lfs.
+        List of lines to be added to the gitattributes file
     :param output_repo_kwargs:
         kwargs to be given to the creation of the output repo initalization function.
         Include gitignore, gitattributes, and lfs_filetypes kwargs.
     :return:
     """
     if not is_tool("git-lfs"):
         raise RuntimeError("Git LFS is not installed. Please install it via e.g. apt-get install git-lfs or the "
                            "instructions found below \n"
                            "https://docs.github.com/en/repositories/working-with-files"
                            "/managing-large-files/installing-git-large-file-storage")
 
     if gitignore is None:
-        gitignore = [".idea", "*diskcache*", "*tmp*", ".ipynb_checkpoints", "__pycache__"]
+        gitignore = get_default_gitignore() + ["*.ipynb"]
 
-    if output_folder_name:
-        gitignore.append(output_folder_name)
-        gitignore.append(output_folder_name + "_cached")
+    gitignore.append(output_folder_name)
+    gitignore.append(output_folder_name + "_cached")
 
     if gitattributes is None:
         gitattributes = []
 
-    if lfs_filetypes is None:
-        lfs_filetypes = ["*.jpg", "*.png", "*.xlsx", "*.h5", "*.ipynb", "*.pdf", "*.docx"]
+    if output_repo_kwargs is None:
+        output_repo_kwargs = {}
 
     starting_directory = os.getcwd()
     project_repo_uuid = str(uuid.uuid4())
     output_repo_uuid = str(uuid.uuid4())
 
     if path_to_repo != ".":
         os.makedirs(path_to_repo, exist_ok=True)
         os.chdir(path_to_repo)
 
+    initialize_git()
+
+    write_lines_to_file(path=".gitattributes", lines=gitattributes, open_type="a")
+    write_lines_to_file(path=".gitignore", lines=gitignore, open_type="a")
+
+    create_readme()
+    create_environment_yml()
+
+    ProjectRepo.add_jupytext_file()
+
+    rdm_data = {
+        "is_project_repo": True, "is_output_repo": False,
+        "project_uuid": project_repo_uuid, "output_uuid": output_repo_uuid,
+        "cadet_rdm_version": cadetrdm.__version__
+    }
+    with open(".cadet-rdm-data.json", "w") as f:
+        json.dump(rdm_data, f, indent=2)
+
+    with open(".cadet-rdm-cache.json", "w") as f:
+        json.dump({"__example/path/to/repo__": {
+            "source_repo_location": "git@jugit.fz-juelich.de:IBG-1/ModSim/cadet"
+                                    "/agile_cadet_rdm_presentation_output.git",
+            "branch_name": "output_from_master_3910c84_2023-10-25_00-17-23",
+            "commit_hash": "6e3c26527999036e9490d2d86251258fe81d46dc"
+        }}, f, indent=2)
+
+    with open("output_remotes.json", "w") as file_handle:
+        remotes_dict = {}
+        json_dict = {"output_folder_name": output_folder_name, "output_remotes": remotes_dict}
+        json.dump(json_dict, file_handle, indent=2)
+
+    initialize_output_repo(output_folder_name, project_repo_uuid=project_repo_uuid,
+                           output_repo_uuid=output_repo_uuid, **output_repo_kwargs)
+
+    repo = ProjectRepo(".", output_folder=output_folder_name)
+    repo.update_output_remotes_json()
+
+    repo.commit("initial commit")
+
+    os.chdir(starting_directory)
+
+
+def initialize_git(folder="."):
+    if folder != ":":
+        starting_directory = os.getcwd()
+        os.chdir(folder)
+
     try:
         repo = git.Repo(".")
-        proceed = input(f'The target directory already contains a git repo.\n'
-                        f'Please back up or push all changes to the repo before continuing.'
-                        f'Proceed? Y/n \n')
-        if not (proceed.lower() == "y" or proceed == ""):
+        proceed = wait_for_user('The target directory already contains a git repo.\n'
+                                'Please back up or push all changes to the repo before continuing.\n'
+                                'Proceed?')
+        if not proceed:
             raise KeyboardInterrupt
     except git.exc.InvalidGitRepositoryError:
         os.system(f"git init")
 
+    if folder != ":":
+        os.chdir(starting_directory)
+
+
+def get_default_gitignore():
+    return [".idea", "*diskcache*", "*tmp*", ".ipynb_checkpoints", "__pycache__"]
+
+
+def get_default_lfs_filetypes():
+    return ["*.jpg", "*.png", "*.xlsx", "*.h5", "*.ipynb", "*.pdf", "*.docx", "*.zip", "*.html"]
+
+
+def initialize_output_repo(output_folder_name, gitignore: list = None,
+                           gitattributes: list = None, lfs_filetypes: list = None,
+                           project_repo_uuid: str = None, output_repo_uuid: str = None):
+    """
+    Initialize a git repository at the given path with an optional included output results repository.
+
+    :param output_folder_name:
+        Name for the output repository.
+    :param gitignore:
+        List of files to be added to the gitignore file.
+    :param gitattributes:
+        List of lines to be added to the gitattributes file
+    :param lfs_filetypes:
+        List of filetypes to be handled by git lfs.
+    :return:
+    """
+    starting_directory = os.getcwd()
+    os.makedirs(output_folder_name, exist_ok=True)
+    os.chdir(output_folder_name)
+
+    if gitignore is None:
+        gitignore = get_default_gitignore()
+
+    if gitattributes is None:
+        gitattributes = ["rdm-log.tsv merge=union"]
+
+    if lfs_filetypes is None:
+        lfs_filetypes = get_default_lfs_filetypes()
+
+    initialize_git()
+
     write_lines_to_file(path=".gitattributes", lines=gitattributes, open_type="a")
     write_lines_to_file(path=".gitignore", lines=gitignore, open_type="a")
 
-    if output_repo_kwargs is None:
-        output_repo_kwargs = {"gitattributes": ["logs/log.csv merge=union"]}
-
-    if output_folder_name:
-        # This means we are in the project repo and should now initialize the output_repo
-        create_readme()
-        create_environment_yml()
-
-        rdm_data = {
-            "is_project_repo": True, "is_output_repo": False,
-            "project_uuid": project_repo_uuid, "output_uuid": output_repo_uuid,
-            "cadet_rdm_version": cadetrdm.__version__
-        }
-        with open(".cadet-rdm-data.json", "w") as f:
-            json.dump(rdm_data, f, indent=2)
-
-        with open(".cadet-rdm-cache.json", "w") as f:
-            json.dump({"__example/path/to/repo__": {
-                "source_repo_location": "git@jugit.fz-juelich.de:IBG-1/ModSim/cadet"
-                                        "/agile_cadet_rdm_presentation_output.git",
-                "branch_name": "output_from_master_3910c84_2023-10-25_00-17-23",
-                "commit_hash": "6e3c26527999036e9490d2d86251258fe81d46dc"
-            }}, f, indent=2)
-
-        initialize_repo(output_folder_name, output_folder_name=False, **output_repo_kwargs)
-        # This instance of ProjectRepo is therefore the project repo
-        repo = ProjectRepo(".", output_folder=output_folder_name)
-    else:
-        # If output_repo_name is False we are in the output_repo and should finish by committing the changes
-        rdm_data = {
-            "is_project_repo": False, "is_output_repo": True,
-            "project_uuid": project_repo_uuid, "output_uuid": output_repo_uuid,
-            "cadet_rdm_version": cadetrdm.__version__
-        }
-        with open(".cadet-rdm-data.json", "w") as f:
-            json.dump(rdm_data, f, indent=2)
-        init_lfs(lfs_filetypes)
+    rdm_data = {
+        "is_project_repo": False, "is_output_repo": True,
+        "project_uuid": project_repo_uuid, "output_uuid": output_repo_uuid,
+        "cadet_rdm_version": cadetrdm.__version__
+    }
+    with open(".cadet-rdm-data.json", "w") as f:
+        json.dump(rdm_data, f, indent=2)
 
-        create_output_readme()
+    init_lfs(lfs_filetypes)
 
-        repo = OutputRepo(".")
+    create_output_readme()
 
+    repo = OutputRepo(".")
     repo.commit("initial commit")
 
     os.chdir(starting_directory)
 
 
 def create_environment_yml():
     file_lines = ["name: rdm_example", "channels:", "  - conda-forge", "dependencies:", "  - python=3.10", "  - conda",
                   "  - cadet", "  - pip", "  - pip:", "      - cadet-process", "      - cadet-rdm"]
-
-    write_lines_to_file("environment.yml", file_lines, open_type="w")
+    if not os.path.exists("environment.yml"):
+        write_lines_to_file("environment.yml", file_lines, open_type="w")
 
 
 def create_readme():
     readme_lines = ["# Project repo", "Your code goes in this repo.", "Please add a description here including: ",
                     "- authors", "- project", "- things we will find interesting later", "", "",
                     "Please update the environment.yml with your python environment requirements.", "", "",
                     "The output repository can be found at:",
@@ -164,33 +222,41 @@
     readme_lines = ["# Output repo", "Your results will be stored here.", "Please add a description here including: ",
                     "- authors", "- project", "- things we will find interesting later", "", "",
                     "The project repository can be found at:",
                     "[project_repo]() (not actually set yet because no remote has been configured at this moment"]
     write_lines_to_file("README.md", readme_lines, open_type="a")
 
 
-def initialize_from_remote(project_url, path_to_repo: str = None):
+def clone(project_url, path_to_repo: str = None):
     if path_to_repo is None:
         path_to_repo = project_url.split("/")[-1]
+        path_to_repo = path_to_repo.replace(".git", "")
     print(f"Cloning {project_url} into {path_to_repo}")
     git.Repo.clone_from(project_url, path_to_repo)
 
+    path_to_repo = Path(path_to_repo)
+
     # Clone output repo from remotes
-    json_path = os.path.join(path_to_repo, "output_remotes.json")
+    json_path = path_to_repo / "output_remotes.json"
     with open(json_path, "r") as file_handle:
         meta_dict = json.load(file_handle)
 
-    output_folder_name = os.path.join(path_to_repo, meta_dict["output_folder_name"])
+    output_folder_name = path_to_repo / meta_dict["output_folder_name"]
     ssh_remotes = list(meta_dict["output_remotes"].values())
     http_remotes = [ssh_url_to_http_url(url) for url in ssh_remotes]
+    if len(ssh_remotes + http_remotes) == 0:
+        raise RuntimeError("No output remotes configured in output_remotes.json")
     for output_remote in ssh_remotes + http_remotes:
         try:
             print(f"Attempting to clone {output_remote} into {output_folder_name}")
             git.Repo.clone_from(output_remote, output_folder_name)
         except Exception as e:
             print(e)
         else:
             break
-    environment_path = os.path.join(os.getcwd(), path_to_repo, "environment.yml")
+    environment_path = Path(os.getcwd()) / path_to_repo / "environment.yml"
+
+    repo = ProjectRepo(path_to_repo)
+    repo.fill_data_from_cadet_rdm_json()
 
     print("To set up the project conda environment please run this command:\n"
           f"conda deactivate && conda env create -f '{environment_path}'")
```

### Comparing `CADET-RDM-0.0.6/cadetrdm/io_utils.py` & `CADET-RDM-0.0.9/cadetrdm/io_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,49 @@
 import os
 import shutil
 from _stat import S_IWRITE
 
 
-def add_linebreaks(input_list):
+def add_linebreaks(input_list, initial_linebreak=True):
     """
     Add linebreaks between each entry in the input_list
+
+    :param input_list:
+    List of strings to add linebreaks to.
+
+    :param initial_linebreak:
+    Bool, if true: add a newline before the first line.
     """
-    return ["\n" + line for line in input_list]
+    lines = [line + "\n" for line in input_list]
+    if initial_linebreak:
+        lines = ["\n"] + lines
+    return lines
 
 
 def write_lines_to_file(path, lines, open_type="a"):
     """
     Convenience function. Write lines to a file at path with added newlines between each line.
     :param path:
         Path to file.
     :param lines:
         List of lines to be written to file.
     :param open_type:
         The way the file should be opened. I.e. "a" for append and "w" for fresh write.
     """
+
+    add_initial_linebreak = False
+
+    if os.path.exists(path) and open_type == "a":
+        with open(path, "r") as f:
+            existing_lines = f.readlines()
+        if len(existing_lines) > 0 and not existing_lines[-1].endswith("\n"):
+            add_initial_linebreak = True
+
     with open(path, open_type) as f:
-        f.writelines(add_linebreaks(lines))
+        f.writelines(add_linebreaks(lines, initial_linebreak=add_initial_linebreak))
 
 
 def is_tool(name):
     """Check whether `name` is on PATH and marked as executable."""
 
     from shutil import which
     return which(name) is not None
@@ -48,7 +66,15 @@
         func(path)
 
     absolute_path = os.path.abspath(filename)
     if os.path.isdir(absolute_path):
         shutil.rmtree(absolute_path, onerror=remove_readonly)
     else:
         os.remove(absolute_path)
+
+
+def wait_for_user(message):
+    proceed = input(message + " Y/n \n")
+    if proceed.lower() == "y" or proceed == "":
+        return True
+    else:
+        return False
```

### Comparing `CADET-RDM-0.0.6/cadetrdm/repositories.py` & `CADET-RDM-0.0.9/cadetrdm/repositories.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import os
+from pathlib import Path
 import json
 import sys
 import traceback
 from datetime import datetime
 import shutil
+import zipfile
 import contextlib
 import glob
 from stat import S_IREAD, S_IWRITE
 from urllib.request import urlretrieve
 
 from tabulate import tabulate
 import pandas as pd
 
-from cadetrdm.io_utils import recursive_chmod
+from cadetrdm.io_utils import recursive_chmod, write_lines_to_file, wait_for_user
+from cadetrdm.jupyter_functionality import Notebook
+from cadetrdm.version import version as cadetrdm_version
 
 try:
     import git
 except ImportError:
     # Adding this hint to save users the confusion of trying $pip install git
     raise ImportError("No module named git, please install the gitpython package")
 
 from cadetrdm.web_utils import ssh_url_to_http_url
 from cadetrdm.io_utils import delete_path
 
 
 def validate_is_output_repo(path_to_repo):
-    with open(os.path.join(path_to_repo, ".cadet-rdm-data.json", "r")) as file_handle:
+    with open(os.path.join(path_to_repo, ".cadet-rdm-data.json"), "r") as file_handle:
         rdm_data = json.load(file_handle)
         if rdm_data["is_project_repo"]:
             raise ValueError("Please use the URL to the output repository.")
 
 
 class BaseRepo:
     def __init__(self, repository_path=None, search_parent_directories=False, *args, **kwargs):
@@ -46,14 +50,18 @@
         :param args:
             Args handed to git.Repo()
         :param kwargs:
             Kwargs handed to git.Repo()
         """
         if repository_path is None or repository_path == ".":
             repository_path = os.getcwd()
+
+        if type(repository_path) is str:
+            repository_path = Path(repository_path)
+
         self._git_repo = git.Repo(repository_path, search_parent_directories=search_parent_directories, *args, **kwargs)
         self._git = self._git_repo.git
 
         self._most_recent_branch = self.active_branch.name
         self._earliest_commit = None
 
         self.add = self._git.add
@@ -68,15 +76,15 @@
 
     @property
     def current_commit_hash(self):
         return str(self.head.commit)
 
     @property
     def working_dir(self):
-        return self._git_repo.working_dir
+        return Path(self._git_repo.working_dir)
 
     @property
     def head(self):
         return self._git_repo.head
 
     @property
     def remotes(self):
@@ -93,24 +101,215 @@
         if self._earliest_commit is None:
             *_, earliest_commit = self._git_repo.iter_commits()
             self._earliest_commit = earliest_commit
         return self._earliest_commit
 
     @property
     def tags(self):
-        return None
+        return list()
+
+    @property
+    def data_json_path(self):
+        return self.working_dir / ".cadet-rdm-data.json"
+
+    @property
+    def cache_json_path(self):
+        return self.working_dir / ".cadet-rdm-cache.json"
 
     def add_remote(self, remote_url, remote_name="origin"):
         """
         ToDO add documentation
         :param remote_url:
         :param remote_name:
         :return:
         """
         self._git_repo.create_remote(remote_name, url=remote_url)
+        with open(self.data_json_path, "r") as handle:
+            rdm_data = json.load(handle)
+        if rdm_data["is_project_repo"]:
+            pass
+        if rdm_data["is_output_repo"]:
+            project_repo = ProjectRepo(self.working_dir.parent)
+            project_repo.update_output_remotes_json()
+
+    def import_remote_repo(self, source_repo_location, source_repo_branch, target_repo_location=None):
+        """
+        Import a remote repo and update the cadet-rdm-cache
+
+        :param source_repo_location:
+        Path or URL to the source repo.
+        Example https://jugit.fz-juelich.de/IBG-1/ModSim/cadet/agile_cadet_rdm_presentation_output.git
+        or git@jugit.fz-juelich.de:IBG-1/ModSim/cadet/agile_cadet_rdm_presentation_output.git
+
+        :param source_repo_branch:
+        Branch of the source repo to check out.
+
+        :param target_repo_location:
+        Place to store the repo. If None, the external_cache folder is used.
+
+        :return:
+        Path to the cloned repository
+        """
+        if target_repo_location is None:
+            target_repo_location = self.working_dir / "external_cache" / source_repo_location.split("/")[-1]
+        else:
+            target_repo_location = self.working_dir / target_repo_location
+
+        self.add_path_to_gitignore(target_repo_location)
+
+        print(f"Cloning from {source_repo_location} into {target_repo_location}")
+        multi_options = ["--filter=blob:none", "--branch", source_repo_branch, "--single-branch"]
+        repo = git.Repo.clone_from(source_repo_location, target_repo_location, multi_options=multi_options)
+        repo.git.clear_cache()
+        repo.close()
+
+        self.update_cadet_rdm_cache_json(source_repo_branch=source_repo_branch,
+                                         target_repo_location=target_repo_location,
+                                         source_repo_location=source_repo_location)
+        return target_repo_location
+
+    def add_path_to_gitignore(self, path_to_be_ignored):
+        """
+        Add the path to the .gitignore file
+
+        :param path_to_be_ignored:
+        :return:
+        """
+        path_to_be_ignored = self.ensure_relative_path(path_to_be_ignored)
+        with open(self.working_dir / ".gitignore", "r") as file_handle:
+            gitignore = file_handle.readlines()
+            gitignore[-1] += "\n"  # Sometimes there is no trailing newline
+        if str(path_to_be_ignored) + "\n" not in gitignore:
+            gitignore.append(str(path_to_be_ignored) + "\n")
+        with open(self.working_dir / ".gitignore", "w") as file_handle:
+            file_handle.writelines(gitignore)
+
+    def update_cadet_rdm_cache_json(self, source_repo_location, source_repo_branch, target_repo_location):
+        """
+        Update the information in the .cadet_rdm_cache.json file
+
+        :param source_repo_location:
+        Path or URL to the source repo.
+        :param source_repo_branch:
+        Name of the branch to check out.
+        :param target_repo_location:
+        Path where to put the repo or data
+        """
+        if not self.cache_json_path.exists():
+            with open(self.cache_json_path, "w") as file_handle:
+                file_handle.writelines("{}")
+
+        with open(self.cache_json_path, "r") as file_handle:
+            rdm_cache = json.load(file_handle)
+
+        repo = BaseRepo(target_repo_location)
+        commit_hash = repo.current_commit_hash
+        if "__example/path/to/repo__" in rdm_cache.keys():
+            rdm_cache.pop("__example/path/to/repo__")
+
+        target_repo_location = str(self.ensure_relative_path(target_repo_location))
+
+        rdm_cache[target_repo_location] = {
+            "source_repo_location": source_repo_location,
+            "branch_name": source_repo_branch,
+            "commit_hash": commit_hash,
+        }
+
+        with open(self.cache_json_path, "w") as file_handle:
+            json.dump(rdm_cache, file_handle, indent=2)
+
+    def ensure_relative_path(self, input_path):
+        """
+        Turn the input path into a relative path, relative to the repo working directory.
+
+        :param input_path:
+        :return:
+        """
+        if type(input_path) is str:
+            input_path = Path(input_path)
+
+        if input_path.is_absolute:
+            relative_path = input_path.relative_to(self.working_dir)
+        else:
+            relative_path = input_path
+        return relative_path
+
+    def verify_unchanged_cache(self):
+        """
+        Verify that all repos referenced in .cadet-rdm-data.json are
+        in an unmodified state. Raises a RuntimeError if the commit hash has changed or if
+        uncommited changes are found.
+
+        :return:
+        """
+
+        with open(self.cache_json_path, "r") as file_handle:
+            rdm_cache = json.load(file_handle)
+
+        if "__example/path/to/repo__" in rdm_cache.keys():
+            rdm_cache.pop("__example/path/to/repo__")
+
+        for repo_location, repo_info in rdm_cache.items():
+            try:
+                repo = BaseRepo(repo_location)
+                repo._git.clear_cache()
+            except git.exc.NoSuchPathError:
+                raise git.exc.NoSuchPathError(f"The imported repository at {repo_location} was not found.")
+
+            self.verify_cache_folder_is_unchanged(repo_location, repo_info["commit_hash"])
+
+    def verify_cache_folder_is_unchanged(self, repo_location, commit_hash):
+        """
+        Verify that the repo located at repo_location has no uncommited changes and that the current commit_hash
+        is equal to the given commit_hash
+
+        :param repo_location:
+        :param commit_hash:
+        :return:
+        """
+        repo = BaseRepo(repo_location)
+        commit_changed = repo.current_commit_hash != commit_hash
+        uncommited_changes = repo.exist_uncomitted_changes
+        if commit_changed or uncommited_changes:
+            raise RuntimeError(f"The contents of {repo_location} have been modified. Don't do that.")
+        repo._git.clear_cache()
+
+    def fill_data_from_cadet_rdm_json(self, re_load=False):
+        """
+        Iterate through all references within the .cadet-rdm-data.json and
+        load or re-load the data.
+
+        :param re_load:
+        If true: delete and re-load all data. If false, existing data will be left as-is.
+
+        ToDo: add to cadetrdm post-clone function
+        ToDo: can we integrate into git post-clone hooks?
+
+        :return:
+        """
+
+        with open(self.cache_json_path, "r") as file_handle:
+            rdm_cache = json.load(file_handle)
+
+        if "__example/path/to/repo__" in rdm_cache.keys():
+            rdm_cache.pop("__example/path/to/repo__")
+
+        for repo_location, repo_info in rdm_cache.items():
+            if os.path.exists(repo_location) and re_load is False:
+                continue
+            elif os.path.exists(repo_location) and re_load is True:
+                delete_path(repo_location)
+
+            if repo_info["source_repo_location"] == ".":
+                self.copy_data_to_cache(branch_name=repo_info["branch_name"])
+            else:
+                self.import_remote_repo(
+                    target_repo_location=repo_location,
+                    source_repo_location=repo_info["source_repo_location"],
+                    source_repo_branch=repo_info["branch_name"])
 
     def checkout(self, *args, **kwargs):
         self._most_recent_branch = self.active_branch
         self._git.checkout(*args, **kwargs)
 
     def push(self, remote=None, local_branch=None, remote_branch=None, push_all=True):
         """
@@ -169,19 +368,19 @@
             If this is set to false a user input will be prompted if untracked files are about to be added.
         :return:
             List of all staged changes.
         """
         self.add(".")
 
     def reset_hard_to_head(self):
-        proceed = input(f'The output directory contains the following uncommitted changes:\n'
-                        f'{self.untracked_files + self.changed_files}\n'
-                        f' These will be lost if you continue\n'
-                        f'Proceed? Y/n \n')
-        if not (proceed.lower() == "y" or proceed == ""):
+        proceed = wait_for_user(f'The output directory contains the following uncommitted changes:\n'
+                                f'{self.untracked_files + self.changed_files}\n'
+                                f' These will be lost if you continue\n'
+                                f'Proceed?')
+        if not proceed:
             raise KeyboardInterrupt
         # reset all tracked files to previous commit, -q silences output
         self._git.reset("-q", "--hard", "HEAD")
         # remove all untracked files and directories, -q silences output
         try:
             self._git.clean("-q", "-f", "-d")
         except git.exc.GitCommandError:
@@ -279,32 +478,35 @@
 
     def prepare_new_branch(self, branch_name):
         """
         Prepares a new branch to recieve data. This includes:
          - checking out the master branch,
          - creating a new branch from there
         This thereby produces a clear, empty directory for data, while still maintaining
-        .gitignore and .gitatributes
+        .gitignore and .gitattributes
         :param branch_name:
             Name of the new branch.
         """
         self._git.checkout("master")
         self._git.checkout('-b', branch_name)  # equivalent to $ git checkout -b %branch_name
-        try:
-            # Remove previous code backup
-            code_backup_path = os.path.join(self.working_dir, "logs", "code_backup")
-            delete_path(code_backup_path)
-        except Exception as e:
-            print(e)
-        try:
-            # Remove previous logs
-            logs_path = os.path.join(self.working_dir, "logs")
-            delete_path(logs_path)
-        except Exception as e:
-            print(e)
+        code_backup_path = self.working_dir / "run_history"
+        logs_path = self.working_dir / "log.tsv"
+        if code_backup_path.exists():
+            try:
+                # Remove previous code backup
+
+                delete_path(code_backup_path)
+            except Exception as e:
+                print(e)
+        if logs_path.exists():
+            try:
+                # Remove previous logs
+                delete_path(logs_path)
+            except Exception as e:
+                print(e)
 
     def apply_stashed_changes(self):
         """
         Apply the last stashed changes.
         If a "CONFLICT (modify/delete)" error is encountered, this is ignored.
         All other errors are raised.
         """
@@ -328,15 +530,15 @@
     def add_list_of_remotes_in_readme_file(self, repo_identifier: str, remotes_url_list: list):
         if len(remotes_url_list) > 0:
             remotes_url_list_http = [ssh_url_to_http_url(remote)
                                      for remote in remotes_url_list]
             output_link_line = " and ".join(f"[{repo_identifier}]({output_repo_remote})"
                                             for output_repo_remote in remotes_url_list_http) + "\n"
 
-            readme_filepath = os.path.join(self.working_dir, "README.md")
+            readme_filepath = self.working_dir / "README.md"
             with open(readme_filepath, "r") as file_handle:
                 filelines = file_handle.readlines()
                 filelines_giving_output_repo = [i for i in range(len(filelines))
                                                 if filelines[i].startswith(f"[{repo_identifier}](")]
                 if len(filelines_giving_output_repo) == 1:
                     line_to_be_modified = filelines_giving_output_repo[0]
                     filelines[line_to_be_modified] = output_link_line
@@ -349,62 +551,75 @@
                                        "Can't automatically update the link.")
 
             with open(readme_filepath, "w") as file_handle:
                 file_handle.writelines(filelines)
 
 
 class ProjectRepo(BaseRepo):
-    def __init__(self, repository_path=None, output_folder=None,
+    def __init__(self, repository_path=".", output_folder=None,
                  search_parent_directories=True, *args, **kwargs):
         """
         Class for Project-Repositories. Handles interaction between the project repo and
         the output (i.e. results) repo.
 
         :param repository_path:
             Path to the root of the git repository.
         :param output_folder:
-            Path to the root of the output repository.
+            Deprecated: Path to the root of the output repository.
         :param search_parent_directories:
             if True, all parent directories will be searched for a valid repo as well.
 
             Please note that this was the default behaviour in older versions of GitPython,
             which is considered a bug though.
         :param args:
             Additional args to be handed to BaseRepo.
         :param kwargs:
             Additional kwargs to be handed to BaseRepo.
         """
+        repository_path = Path(repository_path)
 
         super().__init__(repository_path, search_parent_directories=search_parent_directories, *args, **kwargs)
 
+        with open(repository_path / "output_remotes.json", "r") as handle:
+            output_remotes = json.load(handle)
+
         if output_folder is not None:
-            output_folder = os.path.split(output_folder)[-1]
-            self.output_folder = output_folder
-        else:
-            with open(os.path.join(repository_path, "output_remotes.json"), "r") as handle:
-                data = json.load(handle)
-            self.output_folder = data["output_folder_name"]
+            print("Deprecation Warning. Setting the outputfolder manually during repo instantiation is deprecated"
+                  " and will be removed in a future update.")
+
+        self.output_folder = output_remotes["output_folder_name"]
 
-        self._output_repo = OutputRepo(os.path.join(self.working_dir, self.output_folder))
+        with open(repository_path / ".cadet-rdm-data.json", "r") as handle:
+            metadata = json.load(handle)
+            repo_version = metadata["cadet_rdm_version"]
+            if cadetrdm_version != repo_version:
+                print(f"Repo version {repo_version} is outdated. Current CADET-RDM version is {cadetrdm_version}\n"
+                      "Updating the repository now.")
+
+        self._output_repo = OutputRepo(self.working_dir / self.output_folder)
         self._on_context_enter_commit_hash = None
         self._is_in_context_manager = False
 
     @property
     def output_repo(self):
         if self._output_repo is None:
             raise ValueError("The output repo has not been set yet.")
         return self._output_repo
 
-    @property
-    def data_json_path(self):
-        return os.path.join(self.working_dir, ".cadet-rdm-data.json")
-
-    @property
-    def cache_json_path(self):
-        return os.path.join(self.working_dir, ".cadet-rdm-cache.json")
+    def update_version(self, current_version):
+        version_parts = [int(x) for x in current_version.split(".")]
+        version_sum = version_parts[0] * 1000 * 1000 + version_parts[1] * 1000 + version_parts[2]
+        if current_version < 9:
+            self.convert_csv_to_tsv_if_necessary()
+            self.add_jupytext_file(self.working_dir)
+
+    @staticmethod
+    def add_jupytext_file(path_root: str | Path = "."):
+        jupytext_lines = ['# Pair ipynb notebooks to py:percent text notebooks', 'formats: "ipynb,py:percent"']
+        write_lines_to_file(Path(path_root) / "jupytext.yml", lines=jupytext_lines, open_type="w")
 
     def get_new_output_branch_name(self):
         """
         Construct a name for the new branch in the output repository.
         :return: the new branch name
         """
         project_repo_hash = str(self.head.commit)
@@ -430,17 +645,17 @@
             lines = []
             for i in range(0, len(string), every):
                 lines.append(string[i:i + every])
             return '\n'.join(lines)
 
         self.output_repo.checkout("master")
 
-        csv_filepath = os.path.join(self.working_dir, self.output_folder, "logs", "log.csv")
+        tsv_filepath = self.working_dir / self.output_folder / "log.tsv"
 
-        df = pd.read_csv(csv_filepath, sep=",", header=0)
+        df = pd.read_csv(tsv_filepath, sep="\t", header=0)
         # Clean up the headers
         df = df.rename(columns={"Output repo commit message": 'Output commit message',
                                 "Output repo branch": "Output branch",
                                 "Output repo commit hash": "Output hash", "Project repo commit hash": "Project hash"})
         # Shorten the commit hashes
         df.loc[:, "Output hash"] = df.loc[:, "Output hash"].apply(lambda x: x[:8])
         # Shorten commit messages
@@ -451,120 +666,147 @@
         df = df.loc[:, ["Output commit message", "Output hash", "Output branch"]]
 
         # Print
         print(tabulate(df, headers=df.columns, showindex=False))
 
         self.output_repo.checkout(self.output_repo._most_recent_branch)
 
+    def convert_csv_to_tsv_if_necessary(self):
+        """
+        If not tsv log is found AND a csv log is found, convert the csv to tsv.
+
+        :return:
+        """
+        tsv_filepath = self.working_dir / self.output_folder / "log.tsv"
+        if tsv_filepath.exists():
+            return
+
+        csv_filepath = self.working_dir / self.output_folder / "log.csv"
+        if not csv_filepath.exists():
+            # We have just initialized the repo and neither tsv nor csv exist.
+            return
+
+        with open(csv_filepath) as csv_handle:
+            csv_lines = csv_handle.readlines()
+
+        tsv_lines = [line.replace(",", "\t") for line in csv_lines]
+
+        with open(tsv_filepath, "w") as f:
+            f.writelines(tsv_lines)
+
+        write_lines_to_file(path=self.working_dir / ".gitattributes",
+                            lines=["rdm-log.tsv merge=union"],
+                            open_type="a")
+
     def update_output_master_logs(self, ):
         """
         Dumps all the metadata information about the project repositories state and
         the commit hash and branch name of the ouput repository into the master branch of
         the output repository.
         """
         output_branch_name = str(self._output_repo.active_branch)
 
         output_repo_hash = str(self._output_repo.head.commit)
         output_commit_message = self._output_repo.active_branch.commit.message
         output_commit_message = output_commit_message.replace("\n", "; ")
 
         self._output_repo._git.checkout("master")
 
-        logs_folderpath = os.path.join(self.working_dir, self.output_folder, "logs")
-        if not os.path.exists(logs_folderpath):
+        logs_folderpath = self.working_dir / self.output_folder / "run_history" / output_branch_name
+        if not logs_folderpath.exists():
             os.makedirs(logs_folderpath)
 
-        json_filepath = os.path.join(logs_folderpath, f"{output_branch_name}.json")
-        # note: if filename of "log.csv" is changed,
+        json_filepath = logs_folderpath / "metadata.json"
+        # note: if filename of "log.tsv" is changed,
         #  this also has to be changed in the gitattributes of the init repo func
-        csv_filepath = os.path.join(logs_folderpath, "log.csv")
+        tsv_filepath = self.output_repo.working_dir / "log.tsv"
 
         meta_info_dict = {
             "Output repo commit message": output_commit_message,
             "Output repo branch": output_branch_name,
             "Output repo commit hash": output_repo_hash,
             "Project repo commit hash": str(self.head.commit),
-            "Project repo folder name": os.path.split(self.working_dir)[-1],
+            "Project repo folder name": self.working_dir.name,
             "Project repo remotes": self.remote_urls,
             "Python sys args": str(sys.argv),
-            "Tags": self.tags,
+            "Tags": ", ".join(self.tags),
         }
-        csv_header = ",".join(meta_info_dict.keys())
-        csv_data = ",".join([str(x) for x in meta_info_dict.values()])
+        csv_header = "\t".join(meta_info_dict.keys())
+        csv_data = "\t".join([str(x) for x in meta_info_dict.values()])
 
         with open(json_filepath, "w") as f:
             json.dump(meta_info_dict, f, indent=2)
 
-        if not os.path.exists(csv_filepath):
-            with open(csv_filepath, "w") as f:
+        if not tsv_filepath.exists():
+            with open(tsv_filepath, "w") as f:
                 f.write(csv_header + "\n")
                 # csv.writer(csv_header + "\n")
 
-        with open(csv_filepath, "r") as f:
+        with open(tsv_filepath, "r") as f:
             existing_header = f.readline().replace("\n", "")
             if existing_header != csv_header:
-                raise ValueError("The used structure of the meta_dict doesn't match the header found in log.csv")
+                raise ValueError("The used structure of the meta_dict doesn't match the header found in log.tsv")
 
-        with open(csv_filepath, "a") as f:
+        with open(tsv_filepath, "a") as f:
             f.write(csv_data + "\n")
 
         self.dump_package_list(logs_folderpath)
 
-        # Copy all code files from the project git repo to the output repo
-        code_copy_folderpath = os.path.join(logs_folderpath, "code_backup")
-        if not os.path.exists(code_copy_folderpath):
-            os.makedirs(code_copy_folderpath)
-        self.copy_code(code_copy_folderpath)
+        self.copy_code(logs_folderpath)
 
         self._output_repo.add(".")
         self._output_repo._git.commit("-m", f"log for '{output_commit_message}' \n"
                                             f"of branch '{output_branch_name}'")
 
         self._output_repo._git.checkout(output_branch_name)
         self._most_recent_branch = output_branch_name
 
     def copy_code(self, target_path):
-        for file in self._git.ls_files().split("\n"):
-            if "\\" in file:
-                file = bytes(file, "utf-8").decode("unicode_escape").encode("cp1252").decode("utf-8")
-            if "'" in file or '"' in file:
-                file = file.replace("'", "").replace('"', '')
-            try:
-                target_file_path = os.path.join(self.working_dir, target_path, file)
-                target_folder = os.path.split(target_file_path)[0]
-                if not os.path.exists(target_folder):
-                    os.makedirs(target_folder)
-                shutil.copyfile(
-                    os.path.join(self.working_dir, file),
-                    target_file_path
-                )
-            except:
-                traceback.print_exc()
+        """
+        Clone only the current branch of the project repo to the target_path
+        and then compress it into a zip file.
+
+        :param target_path:
+        :return:
+        """
+        if type(target_path) is str:
+            target_path = Path(target_path)
+
+        code_tmp_folder = target_path / "git_repo"
+
+        multi_options = ["--filter=blob:none", "--single-branch"]
+        git.Repo.clone_from(self.working_dir, code_tmp_folder, multi_options=multi_options)
+
+        shutil.make_archive(target_path / "code", "zip", code_tmp_folder)
+
+        delete_path(code_tmp_folder)
 
     def commit(self, message: str, add_all=True):
         """
         Commit current state of the repository.
 
         :param message:
             Commit message
         :param add_all:
             Option to add all changed and new files to git automatically.
         """
 
+        self.update_output_remotes_json()
+
+        super().commit(message=message, add_all=add_all)
+
+    def update_output_remotes_json(self):
         output_repo_remotes = self.output_repo.remote_urls
         self.add_list_of_remotes_in_readme_file("output_repo", output_repo_remotes)
-
-        output_json_filepath = os.path.join(self.working_dir, "output_remotes.json")
+        output_json_filepath = self.working_dir / "output_remotes.json"
         with open(output_json_filepath, "w") as file_handle:
             remotes_dict = {remote.name: str(remote.url) for remote in self.output_repo.remotes}
             json_dict = {"output_folder_name": self.output_folder, "output_remotes": remotes_dict}
             json.dump(json_dict, file_handle, indent=2)
 
-        super().commit(message=message, add_all=add_all)
-
     def download_file(self, url, file_path):
         """
         Download the file from the url and put it in the output+file_path location.
 
         :param file_path:
         :param url:
         :return:
@@ -603,216 +845,54 @@
             has_stashed_changes = True
         else:
             has_stashed_changes = False
 
         previous_branch = self.output_repo.active_branch.name
         self.output_repo._git.checkout(branch_name)
 
-        source_filepath = os.path.join(self.output_repo.working_dir, file_path)
+        source_filepath = self.output_repo.working_dir / file_path
 
-        target_folder = os.path.join(self.output_repo.working_dir + "_cached", branch_name)
+        target_folder = self.working_dir / (self.output_folder + "_cached") / branch_name
         os.makedirs(target_folder, exist_ok=True)
 
-        target_filepath = os.path.join(target_folder, file_path)
-        if os.path.exists(target_filepath):
+        target_filepath = target_folder / file_path
+        if target_filepath.exists():
             os.chmod(target_filepath, S_IWRITE)
             os.remove(target_filepath)
         shutil.copyfile(source_filepath, target_filepath)
         os.chmod(target_filepath, S_IREAD)
 
         self.output_repo._git.checkout(previous_branch)
         if has_stashed_changes:
             self.output_repo.apply_stashed_changes()
 
         return target_filepath
 
-    def import_remote_repo(self, source_repo_location, source_repo_branch, target_repo_location=None):
-        """
-
-        :param source_repo_location:
-        Path or URL to the source repo.
-        Example https://jugit.fz-juelich.de/IBG-1/ModSim/cadet/agile_cadet_rdm_presentation_output.git
-        or git@jugit.fz-juelich.de:IBG-1/ModSim/cadet/agile_cadet_rdm_presentation_output.git
-
-        :param source_repo_branch:
-        Branch of the source repo to check out.
-
-        :param target_repo_location:
-        Place to store the repo. If None, the external_cache folder is used.
-
-        :return:
-        Path to the cloned repository
-        """
-        if target_repo_location is None:
-            target_repo_location = os.path.join(self.working_dir, "external_cache", source_repo_location.split("/")[-1])
-        else:
-            target_repo_location = os.path.join(self.working_dir, target_repo_location)
-
-        multi_options = ["--filter=blob:none", "--branch", source_repo_branch, "--single-branch"]
-
-        self.add_path_to_gitignore(target_repo_location)
-
-        print(f"Cloning from {source_repo_location} into {target_repo_location}")
-        repo = git.Repo.clone_from(source_repo_location, target_repo_location, multi_options=multi_options)
-        repo.git.clear_cache()
-
-        self.update_cadet_rdm_cache_json(source_repo_branch=source_repo_branch,
-                                         target_repo_location=target_repo_location,
-                                         source_repo_location=source_repo_location)
-        return target_repo_location
-
-    def add_path_to_gitignore(self, path_to_be_ignored):
-        """
-        Add the path to the .gitignore file
-
-        :param path_to_be_ignored:
-        :return:
-        """
-        path_to_be_ignored = self.ensure_relative_path(path_to_be_ignored)
-        with open(os.path.join(self.working_dir, ".gitignore"), "r") as file_handle:
-            gitignore = file_handle.readlines()
-            gitignore[-1] += "\n"  # Sometimes there is no trailing newline
-        if path_to_be_ignored + "\n" not in gitignore:
-            gitignore.append(path_to_be_ignored + "\n")
-        with open(os.path.join(self.working_dir, ".gitignore"), "w") as file_handle:
-            file_handle.writelines(gitignore)
-
-    def update_cadet_rdm_cache_json(self, source_repo_location, source_repo_branch, target_repo_location):
-        """
-        Update the information in the .cadet_rdm_cache.json file
-
-        :param source_repo_location:
-        Path or URL to the source repo.
-        :param source_repo_branch:
-        Name of the branch to check out.
-        :param target_repo_location:
-        Path where to put the repo or data
-        """
-
-        with open(self.cache_json_path, "r") as file_handle:
-            rdm_cache = json.load(file_handle)
-
-        repo = BaseRepo(target_repo_location)
-        commit_hash = repo.current_commit_hash
-        if "__example/path/to/repo__" in rdm_cache.keys():
-            rdm_cache.pop("__example/path/to/repo__")
-
-        target_repo_location = self.ensure_relative_path(target_repo_location)
-
-        rdm_cache[target_repo_location] = {
-            "source_repo_location": source_repo_location,
-            "branch_name": source_repo_branch,
-            "commit_hash": commit_hash,
-        }
-
-        with open(self.cache_json_path, "w") as file_handle:
-            json.dump(rdm_cache, file_handle, indent=2)
-
-    def ensure_relative_path(self, input_path):
-        """
-        Turn the input path into a relative path, relative to the repo working directory.
-
-        :param input_path:
-        :return:
-        """
-        if os.path.isabs(input_path):
-            relative_path = os.path.relpath(input_path, self.working_dir)
-        else:
-            relative_path = input_path
-        return relative_path
-
-    def verify_unchanged_cache(self):
-        """
-        Verify that all repos referenced in .cadet-rdm-data.json are
-        in an unmodified state. Raises a RuntimeError if the commit hash has changed or if
-        uncommited changes are found.
-
-        :return:
-        """
-
-        with open(self.cache_json_path, "r") as file_handle:
-            rdm_cache = json.load(file_handle)
-
-        if "__example/path/to/repo__" in rdm_cache.keys():
-            rdm_cache.pop("__example/path/to/repo__")
-
-        for repo_location, repo_info in rdm_cache.items():
-            try:
-                repo = BaseRepo(repo_location)
-                repo._git.clear_cache()
-            except git.exc.NoSuchPathError:
-                raise git.exc.NoSuchPathError(f"The imported repository at {repo_location} was not found.")
-
-            self.verify_cache_folder_is_unchanged(repo_location, repo_info["commit_hash"])
-
-    def verify_cache_folder_is_unchanged(self, repo_location, commit_hash):
-        """
-        Verify that the repo located at repo_location has no uncommited changes and that the current commit_hash
-        is equal to the given commit_hash
-
-        :param repo_location:
-        :param commit_hash:
-        :return:
-        """
-        repo = BaseRepo(repo_location)
-        commit_changed = repo.current_commit_hash != commit_hash
-        uncommited_changes = repo.exist_uncomitted_changes
-        if commit_changed or uncommited_changes:
-            raise RuntimeError(f"The contents of {repo_location} have been modified. Don't do that.")
-        repo._git.clear_cache()
-
-    def fill_data_from_cadet_rdm_json(self, re_load=False):
-        """
-        Iterate through all references within the .cadet-rdm-data.json and
-        load or re-load the data.
-
-        :param re_load:
-        If true: delete and re-load all data. If false, existing data will be left as-is.
-
-        ToDo: add to cadetrdm post-clone function
-        ToDo: can we integrate into git post-clone hooks?
-
-        :return:
-        """
-
-        with open(self.cache_json_path, "r") as file_handle:
-            rdm_cache = json.load(file_handle)
-
-        if "__example/path/to/repo__" in rdm_cache.keys():
-            rdm_cache.pop("__example/path/to/repo__")
-
-        for repo_location, repo_info in rdm_cache.items():
-            if os.path.exists(repo_location) and re_load is False:
-                continue
-            elif os.path.exists(repo_location) and re_load is True:
-                delete_path(repo_location)
-
-            if repo_info["source_repo_location"] == ".":
-                self.copy_data_to_cache(branch_name=repo_info["branch_name"])
-            else:
-                self.import_remote_repo(
-                    target_repo_location=repo_location,
-                    source_repo_location=repo_info["source_repo_location"],
-                    source_repo_branch=repo_info["branch_name"])
+    @property
+    def output_path(self):
+        return self.output_data()
 
-    def output_data(self, sub_path):
+    def output_data(self, sub_path=None):
         """
         Return an absolute path with the repo_dir/output_dir/sub_path
 
         :param sub_path:
         :return:
         """
-        return os.path.join(self.working_dir, self.output_repo.working_dir, sub_path)
+        if sub_path is None:
+            return self.working_dir / self.output_repo.working_dir
+        else:
+            return self.working_dir / self.output_repo.working_dir, sub_path
 
     def remove_cached_files(self):
         """
         Delete all previously cached results.
         """
-        if os.path.exists(self.output_repo.working_dir + "_cached"):
-            delete_path(self.output_repo.working_dir + "_cached")
+        if (self.working_dir / (self.output_folder + "_cached")).exists():
+            delete_path(self.working_dir / (self.output_folder + "_cached"))
 
     def test_for_correct_repo_setup(self):
         """
         ToDo: implement
         :return:
         """
 
@@ -864,15 +944,15 @@
             if branch_name is None:
                 branch_name = self.output_repo.active_branch.name
                 previous_branch = None
             else:
                 previous_branch = self.output_repo.active_branch.name
                 self.output_repo.checkout(branch_name)
 
-            target_folder = os.path.join(self.output_repo.working_dir + "_cached", branch_name)
+            target_folder = self.working_dir / (self.output_folder + "_cached") / branch_name
 
             shutil.copytree(source_filepath, target_folder)
 
             # Set all files to read only
             for filename in glob.iglob(f"{target_folder}/**/*", recursive=True):
                 absolute_path = os.path.abspath(filename)
                 if os.path.isdir(absolute_path):
@@ -931,10 +1011,25 @@
             yield new_branch_name
         except Exception as e:
             self.output_repo.delete_active_branch_if_branch_is_empty()
             raise e
         else:
             self.exit_context(message=results_commit_message)
 
+    def commit_notebook(self, notebook_path: str, results_commit_message: str,
+                        force_rerun=False, timeout=600, conversion_formats: list = None):
+        if not Path(notebook_path).is_absolute():
+            notebook_path = self.working_dir / notebook_path
+
+        self.enter_context()
+
+        notebook = Notebook(notebook_path)
+        notebook.check_and_rerun_notebook(force_rerun=force_rerun,
+                                          timeout=timeout)
+        notebook.convert_ipynb(self.output_path, formats=conversion_formats)
+        notebook.export_all_figures(self.output_path)
+
+        self.exit_context(results_commit_message)
+
 
 class OutputRepo(BaseRepo):
     pass
```

### Comparing `CADET-RDM-0.0.6/setup.cfg` & `CADET-RDM-0.0.9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 4144 4554 2d52 444d 0d0a 7665   = CADET-RDM..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 360d 0a61  rsion = 0.0.6..a
+00000020: 7273 696f 6e20 3d20 302e 302e 390d 0a61  rsion = 0.0.9..a
 00000030: 7574 686f 7220 3d20 526f 6e61 6c64 204a  uthor = Ronald J
 00000040: c3a4 7065 6c0d 0a61 7574 686f 725f 656d  ..pel..author_em
 00000050: 6169 6c20 3d20 722e 6a61 6570 656c 4066  ail = r.jaepel@f
 00000060: 7a2d 6a75 656c 6963 682e 6465 0d0a 6465  z-juelich.de..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4120 736f  scription = A so
 00000080: 6c75 7469 6f6e 2066 6f72 2072 6573 6561  lution for resea
 00000090: 7263 6820 6461 7461 206d 616e 6167 656d  rch data managem
@@ -37,39 +37,41 @@
 00000240: 735d 0d0a 7061 636b 6167 6573 203d 2066  s]..packages = f
 00000250: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
 00000260: 7569 7265 7320 3d20 3e3d 332e 380d 0a69  uires = >=3.8..i
 00000270: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
 00000280: 3d20 0d0a 0967 6974 7079 7468 6f6e 3e3d  = ...gitpython>=
 00000290: 332e 310d 0a09 6769 742d 6c66 730d 0a09  3.1...git-lfs...
 000002a0: 636c 6963 6b0d 0a09 7461 6275 6c61 7465  click...tabulate
-000002b0: 0d0a 0970 616e 6461 730d 0a69 6e63 6c75  ...pandas..inclu
-000002c0: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
-000002d0: 3d20 5472 7565 0d0a 0d0a 5b6f 7074 696f  = True....[optio
-000002e0: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-000002f0: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
-00000300: 7320 3d20 0d0a 0963 6164 6574 2d72 646d  s = ...cadet-rdm
-00000310: 203d 2063 6164 6574 7264 6d2e 636c 695f   = cadetrdm.cli_
-00000320: 696e 7465 6772 6174 696f 6e3a 636c 690d  integration:cli.
-00000330: 0a0d 0a5b 6f70 7469 6f6e 732e 6578 7472  ...[options.extr
-00000340: 6173 5f72 6571 7569 7265 5d0d 0a74 6573  as_require]..tes
-00000350: 7469 6e67 203d 200d 0a09 7365 7475 7074  ting = ...setupt
-00000360: 6f6f 6c73 0d0a 0970 7974 6573 740d 0a09  ools...pytest...
-00000370: 6365 7274 6966 6920 2020 2020 2320 7472  certifi     # tr
-00000380: 6965 7320 746f 2070 7265 7665 6e74 2063  ies to prevent c
-00000390: 6572 7469 6669 6361 7465 2070 726f 626c  ertificate probl
-000003a0: 656d 7320 6f6e 2077 696e 646f 7773 0d0a  ems on windows..
-000003b0: 0970 7265 2d63 6f6d 6d69 7420 2023 2073  .pre-commit  # s
-000003c0: 7973 7465 6d20 7465 7374 7320 7275 6e20  ystem tests run 
-000003d0: 7072 652d 636f 6d6d 6974 0d0a 0966 6c61  pre-commit...fla
-000003e0: 6b65 3820 2020 2020 2023 2073 7973 7465  ke8      # syste
-000003f0: 6d20 7465 7374 7320 7275 6e20 666c 616b  m tests run flak
-00000400: 6538 0d0a 096d 6174 706c 6f74 6c69 620d  e8...matplotlib.
-00000410: 0a09 6e75 6d70 790d 0a09 6275 696c 640d  ..numpy...build.
-00000420: 0a0d 0a5b 666c 616b 6538 5d0d 0a6d 6178  ...[flake8]..max
-00000430: 5f6c 696e 655f 6c65 6e67 7468 203d 2038  _line_length = 8
-00000440: 380d 0a65 7863 6c75 6465 203d 200d 0a09  8..exclude = ...
-00000450: 6275 696c 640d 0a09 6469 7374 0d0a 092e  build...dist....
-00000460: 6567 6773 0d0a 0964 6f63 732f 636f 6e66  eggs...docs/conf
-00000470: 2e70 790d 0a0d 0a5b 6567 675f 696e 666f  .py....[egg_info
-00000480: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000490: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-000004a0: 0a                                       .
+000002b0: 0d0a 0970 616e 6461 730d 0a09 6e62 666f  ...pandas...nbfo
+000002c0: 726d 6174 0d0a 096e 6263 6f6e 7665 7274  rmat...nbconvert
+000002d0: 0d0a 0969 7079 6c61 620d 0a09 6a75 6e69  ...ipylab...juni
+000002e0: 780d 0a69 6e63 6c75 6465 5f70 6163 6b61  x..include_packa
+000002f0: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
+00000300: 0d0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
+00000310: 5f70 6f69 6e74 735d 0d0a 636f 6e73 6f6c  _points]..consol
+00000320: 655f 7363 7269 7074 7320 3d20 0d0a 0963  e_scripts = ...c
+00000330: 6164 6574 2d72 646d 203d 2063 6164 6574  adet-rdm = cadet
+00000340: 7264 6d2e 636c 695f 696e 7465 6772 6174  rdm.cli_integrat
+00000350: 696f 6e3a 636c 690d 0a0d 0a5b 6f70 7469  ion:cli....[opti
+00000360: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
+00000370: 7265 5d0d 0a74 6573 7469 6e67 203d 200d  re]..testing = .
+00000380: 0a09 7365 7475 7074 6f6f 6c73 0d0a 0970  ..setuptools...p
+00000390: 7974 6573 740d 0a09 6365 7274 6966 6920  ytest...certifi 
+000003a0: 2020 2020 2320 7472 6965 7320 746f 2070      # tries to p
+000003b0: 7265 7665 6e74 2063 6572 7469 6669 6361  revent certifica
+000003c0: 7465 2070 726f 626c 656d 7320 6f6e 2077  te problems on w
+000003d0: 696e 646f 7773 0d0a 0970 7265 2d63 6f6d  indows...pre-com
+000003e0: 6d69 7420 2023 2073 7973 7465 6d20 7465  mit  # system te
+000003f0: 7374 7320 7275 6e20 7072 652d 636f 6d6d  sts run pre-comm
+00000400: 6974 0d0a 0966 6c61 6b65 3820 2020 2020  it...flake8     
+00000410: 2023 2073 7973 7465 6d20 7465 7374 7320   # system tests 
+00000420: 7275 6e20 666c 616b 6538 0d0a 096d 6174  run flake8...mat
+00000430: 706c 6f74 6c69 620d 0a09 6e75 6d70 790d  plotlib...numpy.
+00000440: 0a09 6275 696c 640d 0a0d 0a5b 666c 616b  ..build....[flak
+00000450: 6538 5d0d 0a6d 6178 5f6c 696e 655f 6c65  e8]..max_line_le
+00000460: 6e67 7468 203d 2038 380d 0a65 7863 6c75  ngth = 88..exclu
+00000470: 6465 203d 200d 0a09 6275 696c 640d 0a09  de = ...build...
+00000480: 6469 7374 0d0a 092e 6567 6773 0d0a 0964  dist....eggs...d
+00000490: 6f63 732f 636f 6e66 2e70 790d 0a0d 0a5b  ocs/conf.py....[
+000004a0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000004b0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+000004c0: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `CADET-RDM-0.0.6/tests/test_git_adapter.py` & `CADET-RDM-0.0.9/tests/test_git_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,61 @@
-import os.path
-import shutil
-import stat
+from pathlib import Path
+import os
 import random
 
 import pytest
 import git
 import numpy as np
 
-from cadetrdm import initialize_repo, ProjectRepo, initialize_from_remote
+from cadetrdm import initialize_repo, ProjectRepo, clone
 from cadetrdm.initialize_repo import init_lfs
-from cadetrdm.repositories import OutputRepo
+from cadetrdm.repositories import OutputRepo, BaseRepo
 from cadetrdm.io_utils import delete_path
 
 
 @pytest.fixture(scope="module")
 def path_to_repo():
     # a "fixture" serves up shared, ready variables to test functions that should use the fixture as a kwarg
-    return "test_repo"
-
-
-# @pytest.fixture(scope="module", autouse=True)
-# def my_fixture(path_to_repo):
-#     print('INITIALIZATION')
-#     if os.path.exists(path_to_repo):
-#         remove_dir(path_to_repo)
-#     yield "this is just here because something must yield"
-#     print("TEAR DOWN")
-#     remove_dir(path_to_repo)
+    return Path("test_repo")
 
 
 def modify_code(path_to_repo):
     # Add changes to the project code
     random_number = random.randint(0, 265)
-    filepath = os.path.join(path_to_repo, f"print_random_number.py")
+    filepath = path_to_repo / f"print_random_number.py"
     with open(filepath, "w") as file:
         file.write(f"print({random_number})\n")
 
 
 def count_commit_number(repo):
     commit_log = repo._git.log("--oneline").split("\n")
     current_commit_number = len(commit_log)
     return current_commit_number
 
 
 def example_generate_results_array(path_to_repo, output_folder):
     results_array = np.random.random((500, 3))
-    np.savetxt(os.path.join(path_to_repo, output_folder, "result.csv"),
-               results_array,
-               delimiter=",")
+    np.savetxt(path_to_repo / output_folder / "result.csv", results_array, delimiter=",")
     return results_array
 
 
 def try_init_gitpython_repo(repo_path):
-    os.path.exists(repo_path)
+    repo_path.exists()
     git.Repo(repo_path)
     return True
 
 
 def try_initialize_git_repo(path_to_repo):
-    if os.path.exists(path_to_repo):
+    if path_to_repo.exists():
         delete_path(path_to_repo)
 
     initialize_repo(path_to_repo, "results")
 
     assert try_init_gitpython_repo(path_to_repo)
-    assert try_init_gitpython_repo(os.path.join(path_to_repo, "results"))
+    assert try_init_gitpython_repo(path_to_repo / "results")
 
 
 def try_commit_code(path_to_repo):
     repo = ProjectRepo(path_to_repo)
     current_commit_number = count_commit_number(repo)
 
     modify_code(path_to_repo)
@@ -113,39 +100,39 @@
 def try_load_previous_output(path_to_repo, branch_name):
     repo = ProjectRepo(path_to_repo)
     with repo.track_results(results_commit_message="Load array and extend"):
         cached_array_path = repo.input_data(branch_name=branch_name,
                                             file_path="result.csv")
         previous_array = np.loadtxt(cached_array_path, delimiter=",")
         extended_array = np.concatenate([previous_array, previous_array])
-        extended_array_file_path = os.path.join(path_to_repo, repo.output_folder, "extended_result.csv")
+        extended_array_file_path = path_to_repo / repo.output_folder / "extended_result.csv"
         np.savetxt(extended_array_file_path,
                    extended_array,
                    delimiter=",")
-        assert os.path.exists(cached_array_path)
-        assert os.path.exists(extended_array_file_path)
+        assert cached_array_path.exists()
+        assert extended_array_file_path.exists()
 
 
 def try_add_remote(path_to_repo):
     repo = ProjectRepo(path_to_repo)
     repo.add_remote("git@jugit.fz-juelich.de:IBG-1/ModSim/cadet/CADET-RDM.git")
     assert "origin" in repo._git_repo.remotes
 
 
 def try_initialize_from_remote():
-    if os.path.exists("test_repo_from_remote"):
+    if Path("test_repo_from_remote").exists():
         delete_path("test_repo_from_remote")
-    initialize_from_remote("https://jugit.fz-juelich.de/IBG-1/ModSim/cadet/rdm-examples-fraunhofer-ime-aachen",
-                           "test_repo_from_remote")
+    clone("https://jugit.fz-juelich.de/IBG-1/ModSim/cadet/rdm-examples-fraunhofer-ime-aachen",
+          "test_repo_from_remote")
     assert try_init_gitpython_repo("test_repo_from_remote")
 
 
 def test_init_over_existing_repo(monkeypatch):
-    path_to_repo = "test_repo_2"
-    if os.path.exists(path_to_repo):
+    path_to_repo = Path("test_repo_2")
+    if path_to_repo.exists():
         delete_path(path_to_repo)
     os.makedirs(path_to_repo)
     os.chdir(path_to_repo)
     os.system(f"git init")
     with open("README.md", "w") as handle:
         handle.write("Readme-line 1\n")
     with open(".gitignore", "w") as handle:
@@ -158,17 +145,44 @@
     # using monkeypath to simulate user input
     monkeypatch.setattr('builtins.input', lambda x: "Y")
 
     initialize_repo(path_to_repo)
     delete_path(path_to_repo)
 
 
+def test_cache_with_non_rdm_repo(monkeypatch):
+    path_to_repo = Path("test_repo_5")
+    if path_to_repo.exists():
+        delete_path(path_to_repo)
+    os.makedirs(path_to_repo)
+    os.chdir(path_to_repo)
+    os.system(f"git init")
+    with open("README.md", "w") as handle:
+        handle.write("Readme-line 1\n")
+    with open(".gitignore", "w") as handle:
+        handle.write("foo.bar.*")
+    repo = git.Repo(".")
+    repo.git.add(".")
+    repo.git.commit("-m", "Initial commit")
+
+    imported_repo = OutputRepo("../test_repo/results")
+    branch_name = imported_repo.active_branch.name
+
+    repo = BaseRepo(".")
+
+    # import two repos and confirm verify works.
+    repo.import_remote_repo(source_repo_location="../test_repo/results", source_repo_branch=branch_name)
+    repo.import_remote_repo(source_repo_location="../test_repo/results", source_repo_branch=branch_name,
+                            target_repo_location="foo/bar/repo")
+    repo.verify_unchanged_cache()
+
+
 def test_add_lfs_filetype():
-    path_to_repo = "test_repo_3"
-    if os.path.exists(path_to_repo):
+    path_to_repo = Path("test_repo_3")
+    if path_to_repo.exists():
         delete_path(path_to_repo)
     os.makedirs(path_to_repo)
     initialize_repo(path_to_repo)
     file_type = "*.bak"
     init_lfs(lfs_filetypes=[file_type], path=path_to_repo)
     repo = ProjectRepo(path_to_repo)
     repo.add_all_files()
@@ -194,16 +208,16 @@
 
     try_commit_code(path_to_repo)
 
     try_load_previous_output(path_to_repo, results_branch_name)
 
 
 def test_with_external_repos():
-    path_to_repo = "test_repo_external_data"
-    if os.path.exists(path_to_repo):
+    path_to_repo = Path("test_repo_external_data")
+    if path_to_repo.exists():
         delete_path(path_to_repo)
     os.makedirs(path_to_repo)
     initialize_repo(path_to_repo)
 
     os.chdir(path_to_repo)
 
     # to be able to hand over a valid branch, I first need to determine that branch
@@ -212,18 +226,20 @@
 
     repo = ProjectRepo(".")
 
     # import two repos and confirm verify works.
     repo.import_remote_repo(source_repo_location="../test_repo/results", source_repo_branch=branch_name)
     repo.import_remote_repo(source_repo_location="../test_repo/results", source_repo_branch=branch_name,
                             target_repo_location="foo/bar/repo")
-    repo.verify_unchanged_cache()
-
     # delete folder and reload
     delete_path("foo/bar/repo")
+
+    with pytest.raises(Exception):
+        repo.verify_unchanged_cache()
+
     repo.fill_data_from_cadet_rdm_json()
     repo.verify_unchanged_cache()
 
     # Test if re_load correctly re_loads by modifying and then reloading
     with open("external_cache/results/README.md", "w") as file_handle:
         file_handle.writelines(["a", "b", "c"])
     repo.fill_data_from_cadet_rdm_json(re_load=True)
```

