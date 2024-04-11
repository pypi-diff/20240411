# Comparing `tmp/bbrl_gymnasium-0.3.3.tar.gz` & `tmp/bbrl_gymnasium-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbrl_gymnasium-0.3.3.tar", last modified: Thu Feb 29 09:53:30 2024, max compression
+gzip compressed data, was "bbrl_gymnasium-0.3.4.tar", last modified: Thu Apr 11 06:57:24 2024, max compression
```

## Comparing `bbrl_gymnasium-0.3.3.tar` & `bbrl_gymnasium-0.3.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:53:30.020520 bbrl_gymnasium-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:53:30.012520 bbrl_gymnasium-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:53:30.012520 bbrl_gymnasium-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)       25 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (127)     1388 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-29 09:53:30.016520 bbrl_gymnasium-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:53:30.016520 bbrl_gymnasium-0.3.3/bbrl_gymnasium/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-29 09:53:29.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:53:30.016520 bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/
--rwxr-xr-x   0 runner    (1001) docker     (127)      684 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/cartpole_pixels.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2706 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/continuous_2D_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/continuous_cartpole.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2606 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/continuous_line_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1799 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/debug_env.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2404 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/line_mdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/maze_mdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/pendulum_frottements.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21855 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/rocket_lander.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/single_state_mdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/swimmer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:53:30.016520 bbrl_gymnasium-0.3.3/bbrl_gymnasium/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      966 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:53:30.016520 bbrl_gymnasium-0.3.3/bbrl_gymnasium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-29 09:53:29.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-29 09:53:30.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 09:53:29.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-29 09:53:29.000000 bbrl_gymnasium-0.3.3/bbrl_gymnasium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 09:53:30.020520 bbrl_gymnasium-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:53:30.016520 bbrl_gymnasium-0.3.3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/tests/test_bbrl_gym.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2811 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/tests/test_maze.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      144 2024-02-29 09:53:19.000000 bbrl_gymnasium-0.3.3/tests/test_rocket_lander.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.068448 bbrl_gymnasium-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.072448 bbrl_gymnasium-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)       25 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1388 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.072448 bbrl_gymnasium-0.3.4/bbrl_gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 06:57:23.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      684 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/cartpole_pixels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2706 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/continuous_2D_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/continuous_cartpole.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2606 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/continuous_line_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1799 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/debug_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2404 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/line_mdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/maze_mdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/pendulum_frottements.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21855 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/rocket_lander.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/single_state_mdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/swimmer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/bbrl_gymnasium/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      966 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/bbrl_gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-11 06:57:24.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-11 06:57:24.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 06:57:24.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 06:57:24.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/tests/test_bbrl_gym.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2811 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/tests/test_maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      144 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/tests/test_rocket_lander.py
```

### Comparing `bbrl_gymnasium-0.3.3/.flake8` & `bbrl_gymnasium-0.3.4/.flake8`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/.github/workflows/python-publish.yml` & `bbrl_gymnasium-0.3.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/.pre-commit-config.yaml` & `bbrl_gymnasium-0.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/LICENSE` & `bbrl_gymnasium-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/Makefile` & `bbrl_gymnasium-0.3.4/Makefile`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/PKG-INFO` & `bbrl_gymnasium-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbrl_gymnasium
-Version: 0.3.3
+Version: 0.3.4
 Summary: A set of additional gym environments
 Home-page: https://github.com/osigaud/bbrl_gym
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bbrl_gymnasium-0.3.3/README.md` & `bbrl_gymnasium-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/__init__.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,9 +57,9 @@
     id="CartPolePixelsEnv-v1",
     entry_point="bbrl_gymnasium.envs:CartPolePixelsEnv",
     max_episode_steps=500,
 )
 register(
     id="SwimmerBBRLEnv-v0",
     entry_point="bbrl_gymnasium.envs:SwimmerBBRLEnv",
-    max_episode_steps=400,
+    max_episode_steps=1000,
 )
```

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/__init__.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/cartpole_pixels.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/cartpole_pixels.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/continuous_2D_mdp.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/continuous_2D_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/continuous_cartpole.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/continuous_cartpole.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/continuous_line_mdp.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/continuous_line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/debug_env.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/debug_env.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/line_mdp.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/maze_mdp.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/maze_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/pendulum_frottements.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/pendulum_frottements.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/rocket_lander.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/rocket_lander.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/envs/single_state_mdp.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/single_state_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium.egg-info/PKG-INFO` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbrl_gymnasium
-Version: 0.3.3
+Version: 0.3.4
 Summary: A set of additional gym environments
 Home-page: https://github.com/osigaud/bbrl_gym
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bbrl_gymnasium-0.3.3/bbrl_gymnasium.egg-info/SOURCES.txt` & `bbrl_gymnasium-0.3.4/bbrl_gymnasium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/tests/test_bbrl_gym.py` & `bbrl_gymnasium-0.3.4/tests/test_bbrl_gym.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.3/tests/test_maze.py` & `bbrl_gymnasium-0.3.4/tests/test_maze.py`

 * *Files identical despite different names*

