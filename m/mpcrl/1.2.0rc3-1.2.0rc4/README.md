# Comparing `tmp/mpcrl-1.2.0rc3.tar.gz` & `tmp/mpcrl-1.2.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcrl-1.2.0rc3.tar", last modified: Wed Feb 14 09:15:19 2024, max compression
+gzip compressed data, was "mpcrl-1.2.0rc4.tar", last modified: Fri Apr  5 20:49:47 2024, max compression
```

## Comparing `mpcrl-1.2.0rc3.tar` & `mpcrl-1.2.0rc4.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxrwxr-x   0 fairaldi  (1001) fairaldi  (1001)        0 2024-02-14 09:15:19.777928 mpcrl-1.2.0rc3/
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     1072 2023-01-31 17:10:35.000000 mpcrl-1.2.0rc3/LICENSE
--rw-r--r--   0 fairaldi  (1001) fairaldi  (1001)     6059 2024-02-14 09:15:19.777928 mpcrl-1.2.0rc3/PKG-INFO
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     4845 2023-11-30 11:01:44.000000 mpcrl-1.2.0rc3/README.md
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     2102 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/pyproject.toml
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)       38 2024-02-14 09:15:19.777928 mpcrl-1.2.0rc3/setup.cfg
-drwxrwxr-x   0 fairaldi  (1001) fairaldi  (1001)        0 2024-02-14 09:15:19.769928 mpcrl-1.2.0rc3/src/
-drwxrwxr-x   0 fairaldi  (1001) fairaldi  (1001)        0 2024-02-14 09:15:19.769928 mpcrl-1.2.0rc3/src/mpcrl/
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     1178 2024-02-14 09:10:50.000000 mpcrl-1.2.0rc3/src/mpcrl/__init__.py
-drwxrwxr-x   0 fairaldi  (1001) fairaldi  (1001)        0 2024-02-14 09:15:19.773928 mpcrl-1.2.0rc3/src/mpcrl/agents/
-drwxrwxr-x   0 fairaldi  (1001) fairaldi  (1001)        0 2024-02-14 09:15:19.773928 mpcrl-1.2.0rc3/src/mpcrl/agents/common/
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)    22245 2024-02-13 17:52:13.000000 mpcrl-1.2.0rc3/src/mpcrl/agents/common/agent.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     3614 2024-02-04 11:50:44.000000 mpcrl-1.2.0rc3/src/mpcrl/agents/common/globopt_learning_agent.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)    16822 2024-02-13 16:53:13.000000 mpcrl-1.2.0rc3/src/mpcrl/agents/common/learning_agent.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     1702 2024-02-04 11:50:44.000000 mpcrl-1.2.0rc3/src/mpcrl/agents/common/rl_learning_agent.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)    19439 2024-02-13 18:29:46.000000 mpcrl-1.2.0rc3/src/mpcrl/agents/lstd_dpg.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)    14241 2024-02-13 18:30:49.000000 mpcrl-1.2.0rc3/src/mpcrl/agents/lstd_q_learning.py
-drwxrwxr-x   0 fairaldi  (1001) fairaldi  (1001)        0 2024-02-14 09:15:19.773928 mpcrl-1.2.0rc3/src/mpcrl/core/
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)        0 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/core/__init__.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     9543 2023-11-30 11:01:44.000000 mpcrl-1.2.0rc3/src/mpcrl/core/callbacks.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     1548 2023-01-31 17:10:35.000000 mpcrl-1.2.0rc3/src/mpcrl/core/errors.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     3211 2023-11-30 11:01:44.000000 mpcrl-1.2.0rc3/src/mpcrl/core/experience.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)    12323 2023-11-30 11:01:44.000000 mpcrl-1.2.0rc3/src/mpcrl/core/exploration.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)    11776 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/core/parameters.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     6942 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/core/schedulers.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     2467 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/core/update.py
-drwxrwxr-x   0 fairaldi  (1001) fairaldi  (1001)        0 2024-02-14 09:15:19.773928 mpcrl-1.2.0rc3/src/mpcrl/optim/
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)      462 2024-02-04 11:50:44.000000 mpcrl-1.2.0rc3/src/mpcrl/optim/__init__.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     7029 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/optim/adam.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     2535 2023-12-30 19:55:26.000000 mpcrl-1.2.0rc3/src/mpcrl/optim/base_optimizer.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     6514 2023-12-30 19:55:26.000000 mpcrl-1.2.0rc3/src/mpcrl/optim/gradient_based_optimizer.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     5491 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/optim/gradient_descent.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     2370 2023-12-30 19:55:26.000000 mpcrl-1.2.0rc3/src/mpcrl/optim/gradient_free_optimizer.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     6560 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/optim/newton_method.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     6378 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/optim/rmsprop.py
-drwxrwxr-x   0 fairaldi  (1001) fairaldi  (1001)        0 2024-02-14 09:15:19.777928 mpcrl-1.2.0rc3/src/mpcrl/util/
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     2691 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/util/control.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)      776 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/util/iters.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     4694 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/util/math.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)      901 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/util/named.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)      605 2023-11-30 11:01:44.000000 mpcrl-1.2.0rc3/src/mpcrl/util/seeding.py
-drwxrwxr-x   0 fairaldi  (1001) fairaldi  (1001)        0 2024-02-14 09:15:19.769928 mpcrl-1.2.0rc3/src/mpcrl/wrappers/
-drwxrwxr-x   0 fairaldi  (1001) fairaldi  (1001)        0 2024-02-14 09:15:19.777928 mpcrl-1.2.0rc3/src/mpcrl/wrappers/agents/
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)      175 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/wrappers/agents/__init__.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     8183 2024-02-04 11:50:44.000000 mpcrl-1.2.0rc3/src/mpcrl/wrappers/agents/log.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     1229 2024-02-04 11:50:44.000000 mpcrl-1.2.0rc3/src/mpcrl/wrappers/agents/record_updates.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     4871 2024-02-04 11:50:44.000000 mpcrl-1.2.0rc3/src/mpcrl/wrappers/agents/wrapper.py
-drwxrwxr-x   0 fairaldi  (1001) fairaldi  (1001)        0 2024-02-14 09:15:19.777928 mpcrl-1.2.0rc3/src/mpcrl/wrappers/envs/
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)      133 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/wrappers/envs/__init__.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     3710 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/wrappers/envs/monitor_episodes.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     4807 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/src/mpcrl/wrappers/envs/monitor_infos.py
-drwxrwxr-x   0 fairaldi  (1001) fairaldi  (1001)        0 2024-02-14 09:15:19.777928 mpcrl-1.2.0rc3/src/mpcrl.egg-info/
--rw-r--r--   0 fairaldi  (1001) fairaldi  (1001)     6059 2024-02-14 09:15:19.000000 mpcrl-1.2.0rc3/src/mpcrl.egg-info/PKG-INFO
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     1464 2024-02-14 09:15:19.000000 mpcrl-1.2.0rc3/src/mpcrl.egg-info/SOURCES.txt
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)        1 2024-02-14 09:15:19.000000 mpcrl-1.2.0rc3/src/mpcrl.egg-info/dependency_links.txt
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)       84 2024-02-14 09:15:19.000000 mpcrl-1.2.0rc3/src/mpcrl.egg-info/requires.txt
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)        6 2024-02-14 09:15:19.000000 mpcrl-1.2.0rc3/src/mpcrl.egg-info/top_level.txt
-drwxrwxr-x   0 fairaldi  (1001) fairaldi  (1001)        0 2024-02-14 09:15:19.777928 mpcrl-1.2.0rc3/tests/
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)    15463 2023-11-30 11:01:44.000000 mpcrl-1.2.0rc3/tests/test_agent.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)    22339 2023-11-30 11:01:32.000000 mpcrl-1.2.0rc3/tests/test_core.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)    10868 2024-02-13 16:53:13.000000 mpcrl-1.2.0rc3/tests/test_examples.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)    18225 2023-12-30 19:55:26.000000 mpcrl-1.2.0rc3/tests/test_optim.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)     4888 2023-11-30 11:01:44.000000 mpcrl-1.2.0rc3/tests/test_util.py
--rw-rw-r--   0 fairaldi  (1001) fairaldi  (1001)    14299 2023-11-30 11:01:44.000000 mpcrl-1.2.0rc3/tests/test_wrappers.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.474789 mpcrl-1.2.0rc4/
+-rw-rw-rw-   0        0        0     1093 2022-11-28 16:28:05.000000 mpcrl-1.2.0rc4/LICENSE
+-rw-rw-rw-   0        0        0     6181 2024-04-05 20:49:47.473775 mpcrl-1.2.0rc4/PKG-INFO
+-rw-rw-rw-   0        0        0     4935 2023-12-29 16:34:56.000000 mpcrl-1.2.0rc4/README.md
+-rw-rw-rw-   0        0        0     2198 2024-03-20 18:16:17.000000 mpcrl-1.2.0rc4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 20:49:47.474789 mpcrl-1.2.0rc4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.413842 mpcrl-1.2.0rc4/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.423898 mpcrl-1.2.0rc4/src/mpcrl/
+-rw-rw-rw-   0        0        0     1289 2024-03-22 14:09:50.000000 mpcrl-1.2.0rc4/src/mpcrl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.433929 mpcrl-1.2.0rc4/src/mpcrl/agents/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.438937 mpcrl-1.2.0rc4/src/mpcrl/agents/common/
+-rw-rw-rw-   0        0        0    24076 2024-03-23 23:52:56.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/common/agent.py
+-rw-rw-rw-   0        0        0     3389 2024-03-23 23:36:33.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/common/globopt_learning_agent.py
+-rw-rw-rw-   0        0        0    13551 2024-03-23 23:58:18.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/common/learning_agent.py
+-rw-rw-rw-   0        0        0     1749 2024-02-02 22:17:54.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/common/offpolicy_rl_agent copy.py
+-rw-rw-rw-   0        0        0     1749 2024-02-02 22:17:54.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/common/rl_learning_agent.py
+-rw-rw-rw-   0        0        0    20477 2024-03-20 15:43:51.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/lstd_dpg.py
+-rw-rw-rw-   0        0        0    15173 2024-03-20 15:44:06.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/lstd_q_learning.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.443957 mpcrl-1.2.0rc4/src/mpcrl/core/
+-rw-rw-rw-   0        0        0        0 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/core/__init__.py
+-rw-rw-rw-   0        0        0     9816 2024-02-03 22:29:54.000000 mpcrl-1.2.0rc4/src/mpcrl/core/callbacks.py
+-rw-rw-rw-   0        0        0     1609 2023-01-07 11:39:22.000000 mpcrl-1.2.0rc4/src/mpcrl/core/errors.py
+-rw-rw-rw-   0        0        0     3294 2023-12-29 16:11:51.000000 mpcrl-1.2.0rc4/src/mpcrl/core/experience.py
+-rw-rw-rw-   0        0        0    12631 2023-12-29 16:11:51.000000 mpcrl-1.2.0rc4/src/mpcrl/core/exploration.py
+-rw-rw-rw-   0        0        0    12085 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/core/parameters.py
+-rw-rw-rw-   0        0        0     7143 2023-10-26 16:39:17.000000 mpcrl-1.2.0rc4/src/mpcrl/core/schedulers.py
+-rw-rw-rw-   0        0        0     2537 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/core/update.py
+-rw-rw-rw-   0        0        0     5167 2024-03-22 13:40:45.000000 mpcrl-1.2.0rc4/src/mpcrl/core/warmstart.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.443957 mpcrl-1.2.0rc4/src/mpcrl/optim/
+-rw-rw-rw-   0        0        0      482 2024-02-02 21:55:26.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/__init__.py
+-rw-rw-rw-   0        0        0     7193 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/adam.py
+-rw-rw-rw-   0        0        0     2600 2023-12-29 18:05:40.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/base_optimizer.py
+-rw-rw-rw-   0        0        0     6668 2023-12-29 18:04:08.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/gradient_based_optimizer.py
+-rw-rw-rw-   0        0        0     5624 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/gradient_descent.py
+-rw-rw-rw-   0        0        0     2429 2023-12-30 18:29:00.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/gradient_free_optimizer.py
+-rw-rw-rw-   0        0        0     6712 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/newton_method.py
+-rw-rw-rw-   0        0        0     6532 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/rmsprop.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.459354 mpcrl-1.2.0rc4/src/mpcrl/util/
+-rw-rw-rw-   0        0        0     2785 2023-08-28 20:00:11.000000 mpcrl-1.2.0rc4/src/mpcrl/util/control.py
+-rw-rw-rw-   0        0        0      800 2023-09-21 13:43:47.000000 mpcrl-1.2.0rc4/src/mpcrl/util/iters.py
+-rw-rw-rw-   0        0        0     4855 2023-10-26 16:35:58.000000 mpcrl-1.2.0rc4/src/mpcrl/util/math.py
+-rw-rw-rw-   0        0        0      933 2023-09-21 13:43:47.000000 mpcrl-1.2.0rc4/src/mpcrl/util/named.py
+-rw-rw-rw-   0        0        0      638 2023-12-29 16:11:53.000000 mpcrl-1.2.0rc4/src/mpcrl/util/seeding.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.418847 mpcrl-1.2.0rc4/src/mpcrl/wrappers/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.462350 mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/
+-rw-rw-rw-   0        0        0      180 2023-10-26 16:37:23.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/__init__.py
+-rw-rw-rw-   0        0        0     8402 2024-02-02 21:42:27.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/log.py
+-rw-rw-rw-   0        0        0     1261 2024-02-02 21:42:27.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/record_updates.py
+-rw-rw-rw-   0        0        0     4998 2024-02-02 21:42:27.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.464350 mpcrl-1.2.0rc4/src/mpcrl/wrappers/envs/
+-rw-rw-rw-   0        0        0      137 2023-10-26 16:37:23.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/envs/__init__.py
+-rw-rw-rw-   0        0        0     4446 2024-03-20 13:12:09.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/envs/monitor_episodes.py
+-rw-rw-rw-   0        0        0     4939 2023-09-21 13:43:47.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/envs/monitor_infos.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.472754 mpcrl-1.2.0rc4/src/mpcrl.egg-info/
+-rw-rw-rw-   0        0        0     6181 2024-04-05 20:49:47.000000 mpcrl-1.2.0rc4/src/mpcrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1543 2024-04-05 20:49:47.000000 mpcrl-1.2.0rc4/src/mpcrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 20:49:47.000000 mpcrl-1.2.0rc4/src/mpcrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-05 20:49:47.000000 mpcrl-1.2.0rc4/src/mpcrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-05 20:49:47.000000 mpcrl-1.2.0rc4/src/mpcrl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.470224 mpcrl-1.2.0rc4/tests/
+-rw-rw-rw-   0        0        0    15889 2023-12-29 16:11:53.000000 mpcrl-1.2.0rc4/tests/test_agent.py
+-rw-rw-rw-   0        0        0    22905 2023-10-26 16:39:25.000000 mpcrl-1.2.0rc4/tests/test_core.py
+-rw-rw-rw-   0        0        0    11156 2024-02-09 18:59:51.000000 mpcrl-1.2.0rc4/tests/test_examples.py
+-rw-rw-rw-   0        0        0    18686 2023-12-29 18:06:31.000000 mpcrl-1.2.0rc4/tests/test_optim.py
+-rw-rw-rw-   0        0        0     5040 2023-12-29 16:11:53.000000 mpcrl-1.2.0rc4/tests/test_util.py
+-rw-rw-rw-   0        0        0    14705 2023-12-29 16:11:49.000000 mpcrl-1.2.0rc4/tests/test_wrappers.py
```

### Comparing `mpcrl-1.2.0rc3/LICENSE` & `mpcrl-1.2.0rc4/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Filippo Airaldi
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Filippo Airaldi
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `mpcrl-1.2.0rc3/PKG-INFO` & `mpcrl-1.2.0rc4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-Metadata-Version: 2.1
-Name: mpcrl
-Version: 1.2.0rc3
-Summary: Reinforcement Learning with Model Predictive Control
-Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/FilippoAiraldi/mpc-reinforcement-learning
-Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues
-Keywords: reinforcement-learning,model-predictive-control,optimization,casadi
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: typing_extensions>=4.5.0
-Requires-Dist: numba>=0.57.1
-Requires-Dist: csnlp>=1.5.8
-Requires-Dist: scipy>=1.11.0
-Requires-Dist: gymnasium>=0.28.1
-
-# Reinforcement Learning with Model Predictive Control
-
-**mpcrl** is a library for training model-based Reinforcement Learning (RL) agents with Model Predictive Control (MPC) as function approximation. This framework, also known as MPC-based RL, was first proposed in [[1]](#1) and has so far been shown effective in various applications and with different learning algorithms, e.g., [[2](#2),[3](#3)].
-
-[![PyPI version](https://badge.fury.io/py/mpcrl.svg)](https://badge.fury.io/py/mpcrl)
-[![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
-![Python 3.9](https://img.shields.io/badge/python->=3.9-green.svg)
-
-[![Tests](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml/badge.svg)](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml)
-[![Downloads](https://static.pepy.tech/badge/mpcrl)](https://www.pepy.tech/projects/mpcrl)
-[![Maintainability](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/maintainability)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/maintainability)
-[![Test Coverage](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/test_coverage)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/test_coverage)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
----
-
-## Introduction
-
-This framework merges two powerful control techinques into a single data-driven one
-
-- MPC, a well-known control methodology that exploits a prediction model to predict the future behaviour of the environment and compute the optimal action
-
-- and RL, a Machine Learning paradigm that showed many successes in recent years (with  games such as chess, Go, etc.) and is highly adaptable to unknown and complex-to-model environments.
-
-<div align="center">
-  <img src="https://raw.githubusercontent.com/FilippoAiraldi/mpc-reinforcement-learning/main/resources/mpcrl-diagram.png" alt="mpcrl-diagram" height="300">
-</div>
-
-The figure shows the main idea behind this learning-based control approach. The MPC controller, parametrized in $\vartheta$, acts both as policy provider (providing an action to the environment, given the current state) and as function approximation for the state and action value functions. Concurrently, an RL agent is employed to tune the parameters of the MPC in such a way to increase the controller's performance and achieve an (sub)optimal policy.
-
----
-
-## Installation
-
-To install the package, run
-
-```bash
-pip install mpcrl
-```
-
-**mpcrl** has the following dependencies
-
-- [csnlp](https://pypi.org/project/csnlp/)
-- [SciPy](https://scipy.org/)
-- [Gymnasium](https://gymnasium.farama.org/)
-- [Numba](https://numba.pydata.org/)
-- [typing_extensions](https://pypi.org/project/typing-extensions/)
-
-For playing around with the source code instead, run
-
-```bash
-git clone https://github.com/FilippoAiraldi/mpc-reinforcement-learning.git
-```
-
----
-
-## Examples
-
-Our [examples](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/tree/main/examples) subdirectory contains an example application on a small linear time-invariant (LTI) system, tackled both with Q-learning and Deterministic Policy Gradient (DPG).
-
----
-
-## License
-
-The repository is provided under the MIT License. See the LICENSE file included with this repository.
-
----
-
-## Author
-
-[Filippo Airaldi](https://www.tudelft.nl/staff/f.airaldi/), PhD Candidate [f.airaldi@tudelft.nl | filippoairaldi@gmail.com]
-
-> [Delft Center for Systems and Control](https://www.tudelft.nl/en/3me/about/departments/delft-center-for-systems-and-control/) in [Delft University of Technology](https://www.tudelft.nl/en/)
-
-Copyright (c) 2023 Filippo Airaldi.
-
-Copyright notice: Technische Universiteit Delft hereby disclaims all copyright interest in the program “mpcrl” (Reinforcement Learning with Model Predictive Control) written by the Author(s). Prof. Dr. Ir. Fred van Keulen, Dean of 3mE.
-
----
-
-## References
-
-<a id="1">[1]</a>
-S. Gros and M. Zanon, "Data-Driven Economic NMPC Using Reinforcement Learning," in _IEEE Transactions on Automatic Control_, vol. 65, no. 2, pp. 636-648, Feb. 2020, doi: 10.1109/TAC.2019.2913768.
-
-<a id="2">[2]</a>
-H. N. Esfahani, A. B. Kordabad and S. Gros, "Approximate Robust NMPC using Reinforcement Learning," _2021 European Control Conference (ECC)_, 2021, pp. 132-137, doi: 10.23919/ECC54610.2021.9655129.
-
-<a id="3">[3]</a>
-W. Cai, A. B. Kordabad, H. N. Esfahani, A. M. Lekkas and S. Gros, "MPC-based Reinforcement Learning for a Simplified Freight Mission of Autonomous Surface Vehicles," _2021 60th IEEE Conference on Decision and Control (CDC)_, 2021, pp. 2990-2995, doi: 10.1109/CDC45484.2021.9683750.
+Metadata-Version: 2.1
+Name: mpcrl
+Version: 1.2.0rc4
+Summary: Reinforcement Learning with Model Predictive Control
+Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/FilippoAiraldi/mpc-reinforcement-learning
+Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues
+Keywords: reinforcement-learning,model-predictive-control,optimization,casadi
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: typing_extensions>=4.5.0
+Requires-Dist: numba>=0.57.1
+Requires-Dist: csnlp>=1.5.10rc3
+Requires-Dist: scipy>=1.11.0
+Requires-Dist: gymnasium>=0.28.1
+
+# Reinforcement Learning with Model Predictive Control
+
+**mpcrl** is a library for training model-based Reinforcement Learning (RL) agents with Model Predictive Control (MPC) as function approximation. This framework, also known as MPC-based RL, was first proposed in [[1]](#1) and has so far been shown effective in various applications and with different learning algorithms, e.g., [[2](#2),[3](#3)].
+
+[![PyPI version](https://badge.fury.io/py/mpcrl.svg)](https://badge.fury.io/py/mpcrl)
+[![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
+![Python 3.9](https://img.shields.io/badge/python->=3.9-green.svg)
+
+[![Tests](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml/badge.svg)](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml)
+[![Downloads](https://static.pepy.tech/badge/mpcrl)](https://www.pepy.tech/projects/mpcrl)
+[![Maintainability](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/maintainability)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/test_coverage)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/test_coverage)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+---
+
+## Introduction
+
+This framework merges two powerful control techinques into a single data-driven one
+
+- MPC, a well-known control methodology that exploits a prediction model to predict the future behaviour of the environment and compute the optimal action
+
+- and RL, a Machine Learning paradigm that showed many successes in recent years (with  games such as chess, Go, etc.) and is highly adaptable to unknown and complex-to-model environments.
+
+<div align="center">
+  <img src="https://raw.githubusercontent.com/FilippoAiraldi/mpc-reinforcement-learning/main/resources/mpcrl-diagram.png" alt="mpcrl-diagram" height="300">
+</div>
+
+The figure shows the main idea behind this learning-based control approach. The MPC controller, parametrized in $\vartheta$, acts both as policy provider (providing an action to the environment, given the current state) and as function approximation for the state and action value functions. Concurrently, an RL agent is employed to tune the parameters of the MPC in such a way to increase the controller's performance and achieve an (sub)optimal policy.
+
+---
+
+## Installation
+
+To install the package, run
+
+```bash
+pip install mpcrl
+```
+
+**mpcrl** has the following dependencies
+
+- [csnlp](https://pypi.org/project/csnlp/)
+- [SciPy](https://scipy.org/)
+- [Gymnasium](https://gymnasium.farama.org/)
+- [Numba](https://numba.pydata.org/)
+- [typing_extensions](https://pypi.org/project/typing-extensions/)
+
+For playing around with the source code instead, run
+
+```bash
+git clone https://github.com/FilippoAiraldi/mpc-reinforcement-learning.git
+```
+
+---
+
+## Examples
+
+Our [examples](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/tree/main/examples) subdirectory contains an example application on a small linear time-invariant (LTI) system, tackled both with Q-learning and Deterministic Policy Gradient (DPG).
+
+---
+
+## License
+
+The repository is provided under the MIT License. See the LICENSE file included with this repository.
+
+---
+
+## Author
+
+[Filippo Airaldi](https://www.tudelft.nl/staff/f.airaldi/), PhD Candidate [f.airaldi@tudelft.nl | filippoairaldi@gmail.com]
+
+> [Delft Center for Systems and Control](https://www.tudelft.nl/en/3me/about/departments/delft-center-for-systems-and-control/) in [Delft University of Technology](https://www.tudelft.nl/en/)
+
+Copyright (c) 2023 Filippo Airaldi.
+
+Copyright notice: Technische Universiteit Delft hereby disclaims all copyright interest in the program “mpcrl” (Reinforcement Learning with Model Predictive Control) written by the Author(s). Prof. Dr. Ir. Fred van Keulen, Dean of 3mE.
+
+---
+
+## References
+
+<a id="1">[1]</a>
+S. Gros and M. Zanon, "Data-Driven Economic NMPC Using Reinforcement Learning," in _IEEE Transactions on Automatic Control_, vol. 65, no. 2, pp. 636-648, Feb. 2020, doi: 10.1109/TAC.2019.2913768.
+
+<a id="2">[2]</a>
+H. N. Esfahani, A. B. Kordabad and S. Gros, "Approximate Robust NMPC using Reinforcement Learning," _2021 European Control Conference (ECC)_, 2021, pp. 132-137, doi: 10.23919/ECC54610.2021.9655129.
+
+<a id="3">[3]</a>
+W. Cai, A. B. Kordabad, H. N. Esfahani, A. M. Lekkas and S. Gros, "MPC-based Reinforcement Learning for a Simplified Freight Mission of Autonomous Surface Vehicles," _2021 60th IEEE Conference on Decision and Control (CDC)_, 2021, pp. 2990-2995, doi: 10.1109/CDC45484.2021.9683750.
```

### Comparing `mpcrl-1.2.0rc3/README.md` & `mpcrl-1.2.0rc4/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-# Reinforcement Learning with Model Predictive Control
-
-**mpcrl** is a library for training model-based Reinforcement Learning (RL) agents with Model Predictive Control (MPC) as function approximation. This framework, also known as MPC-based RL, was first proposed in [[1]](#1) and has so far been shown effective in various applications and with different learning algorithms, e.g., [[2](#2),[3](#3)].
-
-[![PyPI version](https://badge.fury.io/py/mpcrl.svg)](https://badge.fury.io/py/mpcrl)
-[![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
-![Python 3.9](https://img.shields.io/badge/python->=3.9-green.svg)
-
-[![Tests](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml/badge.svg)](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml)
-[![Downloads](https://static.pepy.tech/badge/mpcrl)](https://www.pepy.tech/projects/mpcrl)
-[![Maintainability](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/maintainability)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/maintainability)
-[![Test Coverage](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/test_coverage)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/test_coverage)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
----
-
-## Introduction
-
-This framework merges two powerful control techinques into a single data-driven one
-
-- MPC, a well-known control methodology that exploits a prediction model to predict the future behaviour of the environment and compute the optimal action
-
-- and RL, a Machine Learning paradigm that showed many successes in recent years (with  games such as chess, Go, etc.) and is highly adaptable to unknown and complex-to-model environments.
-
-<div align="center">
-  <img src="https://raw.githubusercontent.com/FilippoAiraldi/mpc-reinforcement-learning/main/resources/mpcrl-diagram.png" alt="mpcrl-diagram" height="300">
-</div>
-
-The figure shows the main idea behind this learning-based control approach. The MPC controller, parametrized in $\vartheta$, acts both as policy provider (providing an action to the environment, given the current state) and as function approximation for the state and action value functions. Concurrently, an RL agent is employed to tune the parameters of the MPC in such a way to increase the controller's performance and achieve an (sub)optimal policy.
-
----
-
-## Installation
-
-To install the package, run
-
-```bash
-pip install mpcrl
-```
-
-**mpcrl** has the following dependencies
-
-- [csnlp](https://pypi.org/project/csnlp/)
-- [SciPy](https://scipy.org/)
-- [Gymnasium](https://gymnasium.farama.org/)
-- [Numba](https://numba.pydata.org/)
-- [typing_extensions](https://pypi.org/project/typing-extensions/)
-
-For playing around with the source code instead, run
-
-```bash
-git clone https://github.com/FilippoAiraldi/mpc-reinforcement-learning.git
-```
-
----
-
-## Examples
-
-Our [examples](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/tree/main/examples) subdirectory contains an example application on a small linear time-invariant (LTI) system, tackled both with Q-learning and Deterministic Policy Gradient (DPG).
-
----
-
-## License
-
-The repository is provided under the MIT License. See the LICENSE file included with this repository.
-
----
-
-## Author
-
-[Filippo Airaldi](https://www.tudelft.nl/staff/f.airaldi/), PhD Candidate [f.airaldi@tudelft.nl | filippoairaldi@gmail.com]
-
-> [Delft Center for Systems and Control](https://www.tudelft.nl/en/3me/about/departments/delft-center-for-systems-and-control/) in [Delft University of Technology](https://www.tudelft.nl/en/)
-
-Copyright (c) 2023 Filippo Airaldi.
-
-Copyright notice: Technische Universiteit Delft hereby disclaims all copyright interest in the program “mpcrl” (Reinforcement Learning with Model Predictive Control) written by the Author(s). Prof. Dr. Ir. Fred van Keulen, Dean of 3mE.
-
----
-
-## References
-
-<a id="1">[1]</a>
-S. Gros and M. Zanon, "Data-Driven Economic NMPC Using Reinforcement Learning," in _IEEE Transactions on Automatic Control_, vol. 65, no. 2, pp. 636-648, Feb. 2020, doi: 10.1109/TAC.2019.2913768.
-
-<a id="2">[2]</a>
-H. N. Esfahani, A. B. Kordabad and S. Gros, "Approximate Robust NMPC using Reinforcement Learning," _2021 European Control Conference (ECC)_, 2021, pp. 132-137, doi: 10.23919/ECC54610.2021.9655129.
-
-<a id="3">[3]</a>
-W. Cai, A. B. Kordabad, H. N. Esfahani, A. M. Lekkas and S. Gros, "MPC-based Reinforcement Learning for a Simplified Freight Mission of Autonomous Surface Vehicles," _2021 60th IEEE Conference on Decision and Control (CDC)_, 2021, pp. 2990-2995, doi: 10.1109/CDC45484.2021.9683750.
+# Reinforcement Learning with Model Predictive Control
+
+**mpcrl** is a library for training model-based Reinforcement Learning (RL) agents with Model Predictive Control (MPC) as function approximation. This framework, also known as MPC-based RL, was first proposed in [[1]](#1) and has so far been shown effective in various applications and with different learning algorithms, e.g., [[2](#2),[3](#3)].
+
+[![PyPI version](https://badge.fury.io/py/mpcrl.svg)](https://badge.fury.io/py/mpcrl)
+[![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
+![Python 3.9](https://img.shields.io/badge/python->=3.9-green.svg)
+
+[![Tests](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml/badge.svg)](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml)
+[![Downloads](https://static.pepy.tech/badge/mpcrl)](https://www.pepy.tech/projects/mpcrl)
+[![Maintainability](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/maintainability)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/test_coverage)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/test_coverage)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+---
+
+## Introduction
+
+This framework merges two powerful control techinques into a single data-driven one
+
+- MPC, a well-known control methodology that exploits a prediction model to predict the future behaviour of the environment and compute the optimal action
+
+- and RL, a Machine Learning paradigm that showed many successes in recent years (with  games such as chess, Go, etc.) and is highly adaptable to unknown and complex-to-model environments.
+
+<div align="center">
+  <img src="https://raw.githubusercontent.com/FilippoAiraldi/mpc-reinforcement-learning/main/resources/mpcrl-diagram.png" alt="mpcrl-diagram" height="300">
+</div>
+
+The figure shows the main idea behind this learning-based control approach. The MPC controller, parametrized in $\vartheta$, acts both as policy provider (providing an action to the environment, given the current state) and as function approximation for the state and action value functions. Concurrently, an RL agent is employed to tune the parameters of the MPC in such a way to increase the controller's performance and achieve an (sub)optimal policy.
+
+---
+
+## Installation
+
+To install the package, run
+
+```bash
+pip install mpcrl
+```
+
+**mpcrl** has the following dependencies
+
+- [csnlp](https://pypi.org/project/csnlp/)
+- [SciPy](https://scipy.org/)
+- [Gymnasium](https://gymnasium.farama.org/)
+- [Numba](https://numba.pydata.org/)
+- [typing_extensions](https://pypi.org/project/typing-extensions/)
+
+For playing around with the source code instead, run
+
+```bash
+git clone https://github.com/FilippoAiraldi/mpc-reinforcement-learning.git
+```
+
+---
+
+## Examples
+
+Our [examples](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/tree/main/examples) subdirectory contains an example application on a small linear time-invariant (LTI) system, tackled both with Q-learning and Deterministic Policy Gradient (DPG).
+
+---
+
+## License
+
+The repository is provided under the MIT License. See the LICENSE file included with this repository.
+
+---
+
+## Author
+
+[Filippo Airaldi](https://www.tudelft.nl/staff/f.airaldi/), PhD Candidate [f.airaldi@tudelft.nl | filippoairaldi@gmail.com]
+
+> [Delft Center for Systems and Control](https://www.tudelft.nl/en/3me/about/departments/delft-center-for-systems-and-control/) in [Delft University of Technology](https://www.tudelft.nl/en/)
+
+Copyright (c) 2023 Filippo Airaldi.
+
+Copyright notice: Technische Universiteit Delft hereby disclaims all copyright interest in the program “mpcrl” (Reinforcement Learning with Model Predictive Control) written by the Author(s). Prof. Dr. Ir. Fred van Keulen, Dean of 3mE.
+
+---
+
+## References
+
+<a id="1">[1]</a>
+S. Gros and M. Zanon, "Data-Driven Economic NMPC Using Reinforcement Learning," in _IEEE Transactions on Automatic Control_, vol. 65, no. 2, pp. 636-648, Feb. 2020, doi: 10.1109/TAC.2019.2913768.
+
+<a id="2">[2]</a>
+H. N. Esfahani, A. B. Kordabad and S. Gros, "Approximate Robust NMPC using Reinforcement Learning," _2021 European Control Conference (ECC)_, 2021, pp. 132-137, doi: 10.23919/ECC54610.2021.9655129.
+
+<a id="3">[3]</a>
+W. Cai, A. B. Kordabad, H. N. Esfahani, A. M. Lekkas and S. Gros, "MPC-based Reinforcement Learning for a Simplified Freight Mission of Autonomous Surface Vehicles," _2021 60th IEEE Conference on Decision and Control (CDC)_, 2021, pp. 2990-2995, doi: 10.1109/CDC45484.2021.9683750.
```

### Comparing `mpcrl-1.2.0rc3/pyproject.toml` & `mpcrl-1.2.0rc4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-[build-system]
-requires = ["setuptools>=67.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "mpcrl"
-authors = [
-  { name="Filippo Airaldi", email="filippoairaldi@gmail.com" },
-]
-description = "Reinforcement Learning with Model Predictive Control"
-readme = "README.md"
-requires-python = ">=3.9"
-license = { text = "MIT" }
-classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3 :: Only",
-	"Programming Language :: Python :: 3.9",
-	"Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Intended Audience :: Science/Research",
-    "Topic :: Scientific/Engineering :: Mathematics",
-    "Topic :: Scientific/Engineering :: Artificial Intelligence",
-]
-dependencies = [
-    "typing_extensions >= 4.5.0",
-    "numba >= 0.57.1",
-    "csnlp >= 1.5.8",
-    "scipy >= 1.11.0",
-    "gymnasium >= 0.28.1",
-]
-keywords = [
-    "reinforcement-learning",
-    "model-predictive-control",
-    "optimization",
-    "casadi",
-]
-dynamic = ["version"]
-
-[project.urls]
-"Homepage" = "https://github.com/FilippoAiraldi/mpc-reinforcement-learning"
-"Bug Tracker" = "https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues"
-
-[tool.setuptools]
-license-files = ["LICENSE"]
-
-[tool.setuptools.dynamic]
-version = {attr = "mpcrl.__version__"}
-
-[tool.black]
-target-version = ["py39", "py310", "py311"]
-color = true
-
-[tool.isort]
-profile = "black"
-py_version = 39
-
-[tool.mypy]
-python_version = "3.9"
-plugins = ["numpy.typing.mypy_plugin"]
-exclude = ["tests"]
-
-[[tool.mypy.overrides]]
-module = [
-    "casadi.*",
-    "csnlp.*",
-    "matplotlib.*",
-    "parameterized.*",
-    "scipy.*",
-    "mpcrl.*",
-]
-ignore_missing_imports = true
-
-[tool.coverage.run]
-branch = true
-omit = [
-    "tests/*",
-    "examples/*",
-    "*/csnlp/*",
-]
-
-[tool.coverage.report]
-exclude_also = [
-    "def __repr__",
-    "def __str__",
-    "raise AssertionError",
-    "raise NotImplementedError",
-    "if __name__ == .__main__.:",
-    "@(abc\\.)?abstractmethod",
-]
-sort = "miss"
+[build-system]
+requires = ["setuptools>=67.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "mpcrl"
+authors = [
+  { name="Filippo Airaldi", email="filippoairaldi@gmail.com" },
+]
+description = "Reinforcement Learning with Model Predictive Control"
+readme = "README.md"
+requires-python = ">=3.9"
+license = { text = "MIT" }
+classifiers = [
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3 :: Only",
+	"Programming Language :: Python :: 3.9",
+	"Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Intended Audience :: Science/Research",
+    "Topic :: Scientific/Engineering :: Mathematics",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+]
+dependencies = [
+    "typing_extensions >= 4.5.0",
+    "numba >= 0.57.1",
+    "csnlp >= 1.5.10rc3",
+    "scipy >= 1.11.0",
+    "gymnasium >= 0.28.1",
+]
+keywords = [
+    "reinforcement-learning",
+    "model-predictive-control",
+    "optimization",
+    "casadi",
+]
+dynamic = ["version"]
+
+[project.urls]
+"Homepage" = "https://github.com/FilippoAiraldi/mpc-reinforcement-learning"
+"Bug Tracker" = "https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues"
+
+[tool.setuptools]
+license-files = ["LICENSE"]
+
+[tool.setuptools.dynamic]
+version = {attr = "mpcrl.__version__"}
+
+[tool.black]
+target-version = ["py39", "py310", "py311"]
+color = true
+
+[tool.isort]
+profile = "black"
+py_version = 39
+
+[tool.mypy]
+python_version = "3.9"
+plugins = ["numpy.typing.mypy_plugin"]
+exclude = ["tests"]
+
+[[tool.mypy.overrides]]
+module = [
+    "casadi.*",
+    "csnlp.*",
+    "matplotlib.*",
+    "parameterized.*",
+    "scipy.*",
+    "mpcrl.*",
+]
+ignore_missing_imports = true
+
+[tool.coverage.run]
+branch = true
+omit = [
+    "tests/*",
+    "examples/*",
+    "*/csnlp/*",
+]
+
+[tool.coverage.report]
+exclude_also = [
+    "def __repr__",
+    "def __str__",
+    "raise AssertionError",
+    "raise NotImplementedError",
+    "if __name__ == .__main__.:",
+    "@(abc\\.)?abstractmethod",
+]
+sort = "miss"
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/agents/common/agent.py` & `mpcrl-1.2.0rc4/src/mpcrl/agents/common/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,499 +1,528 @@
-from collections.abc import Collection, Iterable, Iterator
-from typing import Any, Generic, Literal, Optional, TypeVar, Union
-
-import casadi as cs
-import numpy as np
-import numpy.typing as npt
-from csnlp import Solution, wrappers
-from csnlp.core.cache import invalidate_caches_of
-from csnlp.util.io import SupportsDeepcopyAndPickle
-from csnlp.wrappers import Mpc
-from gymnasium import Env
-from typing_extensions import TypeAlias
-
-from ...core.callbacks import AgentCallbackMixin
-from ...core.exploration import ExplorationStrategy, NoExploration
-from ...util.named import Named
-from ...util.seeding import RngType, mk_seed
-
-SymType = TypeVar("SymType", cs.SX, cs.MX)
-ActType: TypeAlias = Union[npt.ArrayLike, dict[str, npt.ArrayLike]]
-ObsType: TypeAlias = Union[npt.ArrayLike, dict[str, npt.ArrayLike]]
-
-
-def _update_dicts(sinks: Iterable[dict], source: dict) -> Iterator[dict]:
-    """Internal utility for updating dicts `sinks` with one `source`."""
-    for sink in sinks:
-        sink.update(source)
-        yield sink
-
-
-class Agent(Named, SupportsDeepcopyAndPickle, AgentCallbackMixin, Generic[SymType]):
-    """Simple MPC-based agent with a fixed (i.e., non-learnable) MPC controller.
-
-    In this agent, the MPC controller is used as policy provider, as well as to provide
-    the value function `V(s)` and quality function `Q(s,a)`, where `s` and `a` are the
-    state and action of the environment, respectively. However, this class does not use
-    any RL method to improve its MPC policy."""
-
-    cost_perturbation_method = "normal"
-    cost_perturbation_parameter = "cost_perturbation"
-    init_action_parameter = init_action_constraint = "a_init"
-
-    def __init__(
-        self,
-        mpc: Mpc[SymType],
-        fixed_parameters: Union[
-            None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]
-        ] = None,
-        warmstart: Literal["last", "last-successful"] = "last-successful",
-        use_last_action_on_fail: bool = False,
-        remove_bounds_on_initial_action: bool = False,
-        name: Optional[str] = None,
-    ) -> None:
-        """Instantiates an agent with an MPC controller.
-
-        Parameters
-        ----------
-        mpc : Mpc[casadi.SX or MX]
-            The MPC controller used as policy provider by this agent. The instance is
-            modified in place to create the approximations of the state function `V(s)`
-            and action value function `Q(s,a)`, so it is recommended not to modify it
-            further after initialization of the agent. Moreover, some parameter and
-            constraint names will need to be created, so an error is thrown if these
-            names are already in use in the mpc. These names are under the attributes
-            `perturbation_parameter`, `action_parameter` and `action_constraint`.
-        fixed_parameters : dict[str, array_like] or collection of, optional
-            A dict (or collection of dict, in case of `csnlp.MultistartNlp`) whose keys
-            are the names of the MPC parameters and the values are their corresponding
-            values. Use this to specify fixed parameters, that is, non-learnable. If
-            `None`, then no fixed parameter is assumed.
-        warmstart: 'last' or 'last-successful', optional
-            The warmstart strategy for the MPC's NLP. If 'last-successful', the last
-            successful solution is used to warm start the solver for the next iteration.
-            If 'last', the last solution is used, regardless of success or failure.
-        use_last_action_on_fail : bool, optional
-            When `True`, if the MPC solver fails in solving the state value function
-            `V(s)`, the last successful action is returned. When `False`, the action
-            from the last MPC iteration is returned instead. By default, `False`.
-        remove_bounds_on_initial_action : bool, optional
-            When `True`, the upper and lower bounds on the initial action are removed in
-            the action-value function approximator Q(s,a) since the first action is
-            constrained to be equal to the initial action. This is useful to avoid
-            issues in the LICQ of the NLP. However, it can lead to numerical problems.
-            By default, `False`.
-        name : str, optional
-            Name of the agent. If `None`, one is automatically created from a counter of
-            the class' instancies.
-
-        Raises
-        ------
-        ValueError
-            Raises if the given mpc has no control action as optimization variable; or
-            if the required parameter and constraint names are already specified in the
-            mpc.
-        """
-        Named.__init__(self, name)
-        SupportsDeepcopyAndPickle.__init__(self)
-        AgentCallbackMixin.__init__(self)
-        self._fixed_pars = fixed_parameters
-        self._exploration: ExplorationStrategy = NoExploration()
-        self._store_last_successful = warmstart == "last-successful"
-        self._last_action_on_fail = use_last_action_on_fail
-        self._last_solution: Optional[Solution[SymType]] = None
-        self._last_action: Optional[cs.DM] = None
-        self._V, self._Q = self._setup_V_and_Q(mpc, remove_bounds_on_initial_action)
-        self._post_setup_V_and_Q()
-
-    @property
-    def unwrapped(self) -> "Agent":
-        """Gets the underlying wrapped instance of an agent."""
-        return self
-
-    def is_wrapped(self, *args: Any, **kwargs: Any) -> bool:
-        """Gets whether the agent instance is wrapped or not by the wrapper type."""
-        return False
-
-    @property
-    def V(self) -> Mpc[SymType]:
-        """Gets the MPC function approximation of the state value function `V(s)`."""
-        return self._V
-
-    @property
-    def Q(self) -> Mpc[SymType]:
-        """Gets the MPC function approximation of the action value function `Q(s,a)`."""
-        return self._Q
-
-    @property
-    def fixed_parameters(
-        self,
-    ) -> Union[None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]]:
-        """Gets the fixed parameters of the MPC controller (i.e., non-learnable). Can be
-        an iterable in the case of `csnlp.MultistartNpl`, where multiple parameters can
-        be specified, one for each scenario in the MPC scheme."""
-        return self._fixed_pars
-
-    @property
-    def exploration(self) -> ExplorationStrategy:
-        """Gets the exploration strategy used within this agent."""
-        return self._exploration
-
-    def reset(self, seed: RngType = None) -> None:
-        """Resets the agent's internal variables and exploration's RNG."""
-        self._last_solution = None
-        self._last_action = None
-        if hasattr(self.exploration, "reset"):
-            self.exploration.reset(seed)
-
-    def solve_mpc(
-        self,
-        mpc: Mpc[SymType],
-        state: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
-        action: Union[None, npt.ArrayLike, dict[str, npt.ArrayLike]] = None,
-        perturbation: Optional[npt.ArrayLike] = None,
-        vals0: Union[
-            None, dict[str, npt.ArrayLike], Iterable[dict[str, npt.ArrayLike]]
-        ] = None,
-        store_solution: bool = True,
-    ) -> Solution[SymType]:
-        """Solves the agent's specific MPC optimal control problem.
-
-        Parameters
-        ----------
-        mpc : Mpc
-            The MPC problem to solve, either `Agent.V` or `Agent.Q`.
-        state : array_like or dict[str, array_like]
-            A 1D array representing the value of all states of the MPC, concatenated.
-            Otherwise, a dict whose keys are the names of each state, and values are
-            their numerical values.
-        action : array_like or dict[str, array_like], optional
-            Same for `state`, for the action. Only valid if evaluating the action value
-            function `Q(s,a)`. For this reason, it can be `None` for `V(s)`.
-        perturbation : array_like, optional
-            The cost perturbation used to induce exploration in `V(s)`. Can be `None`
-            for `Q(s,a)`.
-        vals0 : dict[str, array_like] or iterable of, optional
-            A dict (or an iterable of dict, in case of `csnlp.MultistartNlp`), whose
-            keys are the names of the MPC variables, and values are the numerical
-            initial values of each variable. Use this to warm-start the MPC. If `None`,
-            and a previous solution (possibly, successful) is available, the MPC solver
-            is automatically warm-started.
-        store_solution : bool, optional
-            By default, the mpc solution is stored accordingly to the `warmstart`
-            strategy. If set to `False`, this flag allows to disable the behaviour for
-            this particular solution.
-
-        Returns
-        -------
-        Solution
-            The solution of the MPC.
-        """
-        # convert state keys into initial state keys (i.e., with "_0")
-        if isinstance(state, dict):
-            x0_dict = {f"{k}_0": v for k, v in state.items()}
-        else:
-            mpcstates = mpc.initial_states
-            if len(mpcstates) == 1:
-                states = (state,)
-            else:
-                cumsizes = np.cumsum([s.shape[0] for s in mpcstates.values()][:-1])
-                states = np.split(state, cumsizes)
-            x0_dict = dict(zip(mpcstates.keys(), states))
-
-        # convert action dict to vector if not None
-        if action is None:
-            u0_vec = None
-        elif isinstance(action, dict):
-            u0_vec = cs.vertcat(*(action[k] for k in mpc.actions.keys()))
-        else:
-            u0_vec = action
-
-        # merge (initial) state, action and perturbation in unique dict
-        additional_pars = x0_dict
-        if u0_vec is not None:
-            additional_pars[self.init_action_parameter] = u0_vec
-        if self.cost_perturbation_parameter in mpc.parameters:
-            additional_pars[self.cost_perturbation_parameter] = (
-                0 if perturbation is None else perturbation
-            )
-
-        # create pars and vals0
-        pars = self._get_parameters()
-        if pars is None:
-            pars = additional_pars
-        elif isinstance(pars, dict):
-            pars.update(additional_pars)
-        else:  # iterable of dict
-            pars = _update_dicts(pars, additional_pars)
-        if vals0 is None and self._last_solution is not None:
-            vals0 = self._last_solution.vals
-
-        # solve and store solution
-        sol = mpc(pars, vals0)
-        if store_solution and (not self._store_last_successful or sol.success):
-            self._last_solution = sol
-        return sol
-
-    def state_value(
-        self,
-        state: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
-        deterministic: bool = False,
-        vals0: Union[
-            None, dict[str, npt.ArrayLike], Iterable[dict[str, npt.ArrayLike]]
-        ] = None,
-        **kwargs,
-    ) -> tuple[cs.DM, Solution[SymType]]:
-        """Computes the state value function `V(s)` approximated by the MPC.
-
-        Parameters
-        ----------
-        state : array_like or dict[str, array_like]
-            The state `s` at which to evaluate the value function `V(s)`. Can either be
-            a dict of state names and values, or a single concatenated column vector of
-            all the states.
-        deterministic : bool, optional
-            If `True`, the cost of the MPC is perturbed according to the exploration
-            strategy to induce some exploratory behaviour. Otherwise, no perturbation is
-            performed. By default, `deterministic=False`.
-        vals0 : dict[str, array_like] or iterable of, optional
-            A dict (or an iterable of dict, in case of `csnlp.MultistartNlp`), whose
-            keys are the names of the MPC variables, and values are the numerical
-            initial values of each variable. Use this to warm-start the MPC. If `None`,
-            and a previous solution (possibly, successful) is available, the MPC solver
-            is automatically warm-started.
-
-        Returns
-        -------
-        casadi.DM
-            The first optimal action according to the solution of `V(s)`.
-        Solution
-            The solution of the MPC approximating `V(s)` at the given state.
-        """
-        if deterministic or not self._exploration.can_explore():
-            pert = None
-        else:
-            pert = self._exploration.perturbation(
-                self.cost_perturbation_method,
-                size=self.V.parameters[self.cost_perturbation_parameter].shape,
-            )
-        sol = self.solve_mpc(self._V, state, perturbation=pert, vals0=vals0, **kwargs)
-        first_action = cs.vertcat(*(sol.vals[u][:, 0] for u in self._V.actions.keys()))
-
-        if sol.success:
-            self._last_action = first_action
-        elif self._last_action_on_fail and self._last_action is not None:
-            first_action = self._last_action
-
-        return first_action, sol
-
-    def action_value(
-        self,
-        state: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
-        action: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
-        vals0: Union[
-            None, dict[str, npt.ArrayLike], Iterable[dict[str, npt.ArrayLike]]
-        ] = None,
-        **kwargs,
-    ) -> Solution[SymType]:
-        """Computes the action value function `Q(s,a)` approximated by the MPC.
-
-        Parameters
-        ----------
-        state : array_like or dict[str, array_like]
-            The state `s` at which to evaluate the value function `Q(s,a)`. Can either
-            be a dict of state names and values, or a single concatenated column vector
-            of all the states.
-        action : array_like or dict[str, array_like]
-            The action `a` at which to evaluate the value function `Q(s,a)`. Can either
-            be a dict of action names and values, or a single concatenated column vector
-            of all the actions.
-        vals0 : dict[str, array_like] or iterable of, optional
-            A dict (or an iterable of dict, in case of `csnlp.MultistartNlp`), whose
-            keys are the names of the MPC variables, and values are the numerical
-            initial values of each variable. Use this to warm-start the MPC. If `None`,
-            and a previous solution (possibly, successful) is available, the MPC solver
-            is automatically warm-started.
-
-        Returns
-        -------
-        Solution
-            The solution of the MPC approximating `Q(s,a)` at given state and action.
-        """
-        return self.solve_mpc(self._Q, state, action, vals0=vals0, **kwargs)
-
-    def evaluate(
-        self,
-        env: Env[ObsType, ActType],
-        episodes: int,
-        deterministic: bool = True,
-        seed: RngType = None,
-        raises: bool = True,
-        env_reset_options: Optional[dict[str, Any]] = None,
-    ) -> npt.NDArray[np.floating]:
-        """Evaluates the agent in a given environment.
-
-        Note: after solving `V(s)` for the current state `s`, the action is computed and
-        passed to the environment as the concatenation of the first optimal action
-        variables of the MPC (see `csnlp.Mpc.actions`).
-
-        Parameters
-        ----------
-        env : Env[ObsType, ActType]
-            A gym environment where to test the agent in.
-        episodes : int
-            Number of evaluation episodes.
-        deterministic : bool, optional
-            Whether the agent should act deterministically; by default, `True`.
-        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
-            Agent's and each env's RNG seed.
-        raises : bool, optional
-            If `True`, when any of the MPC solver runs fails, or when an update fails,
-            the corresponding error is raised; otherwise, only a warning is raised.
-        env_reset_options : dict, optional
-            Additional information to specify how the environment is reset at each
-            evalution episode (optional, depending on the specific environment).
-
-        Returns
-        -------
-        array of doubles
-            The cumulative returns (one return per evaluation episode).
-
-        Raises
-        ------
-            Raises if the MPC optimization solver fails and `warns_on_exception=False`.
-        """
-        rng = np.random.default_rng(seed)
-        self.reset(rng)
-        returns = np.zeros(episodes)
-        self.on_validation_start(env)
-
-        for episode in range(episodes):
-            state, _ = env.reset(seed=mk_seed(rng), options=env_reset_options)
-            truncated, terminated, timestep = False, False, 0
-            self.on_episode_start(env, episode, state)
-
-            while not (truncated or terminated):
-                action, sol = self.state_value(state, deterministic)
-                if not sol.success:
-                    self.on_mpc_failure(episode, timestep, sol.status, raises)
-
-                state, r, truncated, terminated, _ = env.step(action)
-                self.on_env_step(env, episode, timestep)
-
-                returns[episode] += r
-                timestep += 1
-                self.on_timestep_end(env, episode, timestep)
-
-            self.on_episode_end(env, episode, returns[episode])
-
-        self.on_validation_end(env, returns)
-        return returns
-
-    def _setup_V_and_Q(
-        self, mpc: Mpc[SymType], remove_bounds_on_initial_action: bool
-    ) -> tuple[Mpc[SymType], Mpc[SymType]]:
-        """Internal utility to setup the function approximators for the value function
-        V(s) and the quality function Q(s,a)."""
-        na = mpc.na
-        if na <= 0:
-            raise ValueError(f"Expected Mpc with na>0; got na={na} instead.")
-
-        # create V and Q function approximations
-        V, Q = mpc, mpc.copy()
-        V.unwrapped.name += "_V"
-        Q.unwrapped.name += "_Q"
-        a0 = Q.nlp.parameter(self.init_action_parameter, (na, 1))
-        perturbation = V.nlp.parameter(self.cost_perturbation_parameter, (na, 1))
-
-        u0 = cs.vcat(mpc.first_actions.values())
-        f = V.nlp.f
-        if mpc.is_wrapped(wrappers.NlpScaling):
-            f = mpc.scale(f)
-
-        V.nlp.minimize(f + cs.dot(perturbation, u0))
-        Q.nlp.constraint(self.init_action_constraint, u0, "==", a0)
-
-        # remove upper/lower bound on initial action in Q, since it is constrained as a0
-        if remove_bounds_on_initial_action:
-            for name, a in mpc.first_actions.items():
-                na_ = a.size1()
-                Q.nlp.remove_variable_bounds(name, "both", ((r, 0) for r in range(na_)))
-
-        # invalidate caches for V and Q since some modifications have been done
-        for nlp in (V, Q):
-            nlp_ = nlp
-            while nlp_ is not nlp_.unwrapped:
-                invalidate_caches_of(nlp_)
-                nlp_ = nlp_.nlp
-            invalidate_caches_of(nlp_.unwrapped)
-        return V, Q
-
-    def _post_setup_V_and_Q(self) -> None:
-        """Internal utility that is run after the creation of V and Q, allowing for
-        further customization in inheriting classes."""
-        # warn user of any constraints that linearly includes x0 and u0 (aside from
-        # x(0)==s0 and u(0)==a0), which may thus lead to LICQ-failure
-        # - u0 in Q should only appear in the 1st dynamics constraint and a0 con
-        # - u0 in V should only appear in the 1st dynamics constraint and lbx/ubx
-        # - x0 in V, Q should only appear in the 1st dynamics constraint and s0 con
-        # for mpc in (self._V, self._Q):
-        #     name = mpc.unwrapped.name[-1]
-        #     u0 = cs.vcat(self._V.first_actions.values())
-        #     x0 = cs.vvcat(self._V.first_states.values())
-        #     con = cs.vertcat(mpc.g, mpc.h, mpc.h_lbx, mpc.h_ubx)
-
-        #     if mpc.unwrapped.sym_type.__name__ == "SX":
-        #         nnz_con_u0 = len(set(cs.jacobian_sparsity(con, u0).get_triplet()[0]))
-        #         nnz_con_x0 = len(set(cs.jacobian_sparsity(con, x0).get_triplet()[0]))
-        #     else:
-        #         nnz_con_u0 = len(  # computes the same as above, but for MX
-        #             set(
-        #                 chain.from_iterable(
-        #                     cs.jacobian(con, a)[:, : a.size1()]
-        #                     .sparsity()
-        #                     .get_triplet()[0]
-        #                     for a in mpc.actions.values()
-        #                 )
-        #             )
-        #         )
-        #         nnz_con_x0 = len(
-        #             set(
-        #                 chain.from_iterable(
-        #                     cs.jacobian(con, s)[:, : s.size1()]
-        #                     .sparsity()
-        #                     .get_triplet()[0]
-        #                     for s in mpc.states.values()
-        #                 )
-        #             )
-        #         )
-
-        #     nnz_exp_u0 = mpc.ns + (mpc.na * 2 if name == "V" else mpc.na)
-        #     if nnz_con_u0 > nnz_exp_u0:
-        #         warnings.warn(
-        #             f"detected {nnz_con_u0} (expected {nnz_exp_u0}) constraints on "
-        #             f"initial actions in {name}; make sure that the initial action is"
-        #             "not overconstrained (LICQ may be compromised).",
-        #             RuntimeWarning,
-        #         )
-        #     nnz_exp_x0 = mpc.ns * 2
-        #     if nnz_con_x0 > nnz_exp_x0:
-        #         warnings.warn(
-        #             f"detected {nnz_con_x0} (expected {nnz_exp_x0}) constraints on "
-        #             f"initial states in {name}; make sure that the initial state is "
-        #             "not overconstrained (LICQ may be compromised).",
-        #             RuntimeWarning,
-        #         )
-
-    def _get_parameters(
-        self,
-    ) -> Union[None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]]:
-        """Internal utility to retrieve parameters of the MPC in order to solve it.
-        `Agent` has no learnable parameter, so only fixed parameters are returned."""
-        return self._fixed_pars
-
-    def __deepcopy__(self, memo: Optional[dict[int, list[Any]]] = None) -> "Agent":
-        """Ensures that the copy has a new name."""
-        y = super().__deepcopy__(memo)
-        if hasattr(y, "name"):
-            y.name += "_copy"
-        return y
+from collections.abc import Collection, Iterable, Iterator
+from itertools import chain
+from typing import Any, Generic, Literal, Optional, TypeVar, Union
+
+import casadi as cs
+import numpy as np
+import numpy.typing as npt
+from csnlp import Solution, wrappers
+from csnlp.core.cache import invalidate_caches_of
+from csnlp.util.io import SupportsDeepcopyAndPickle
+from csnlp.wrappers import Mpc
+from gymnasium import Env
+from typing_extensions import TypeAlias
+
+from ...core.callbacks import AgentCallbackMixin
+from ...core.exploration import ExplorationStrategy, NoExploration
+from ...core.warmstart import WarmStartStrategy
+from ...util.named import Named
+from ...util.seeding import RngType, mk_seed
+
+SymType = TypeVar("SymType", cs.SX, cs.MX)
+ActType: TypeAlias = Union[npt.ArrayLike, dict[str, npt.ArrayLike]]
+ObsType: TypeAlias = Union[npt.ArrayLike, dict[str, npt.ArrayLike]]
+
+
+def _update_dicts(sinks: Iterable[dict], source: dict) -> Iterator[dict]:
+    """Internal utility for updating dicts `sinks` with one `source`."""
+    for sink in sinks:
+        sink.update(source)
+        yield sink
+
+
+class Agent(Named, SupportsDeepcopyAndPickle, AgentCallbackMixin, Generic[SymType]):
+    """Simple MPC-based agent with a fixed (i.e., non-learnable) MPC controller.
+
+    In this agent, the MPC controller is used as policy provider, as well as to provide
+    the value function `V(s)` and quality function `Q(s,a)`, where `s` and `a` are the
+    state and action of the environment, respectively. However, this class does not use
+    any RL method to improve its MPC policy."""
+
+    cost_perturbation_method = "normal"
+    cost_perturbation_parameter = "cost_perturbation"
+    init_action_parameter = init_action_constraint = "a_init"
+
+    def __init__(
+        self,
+        mpc: Mpc[SymType],
+        fixed_parameters: Union[
+            None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]
+        ] = None,
+        warmstart: Union[
+            Literal["last", "last-successful"], WarmStartStrategy
+        ] = "last-successful",
+        use_last_action_on_fail: bool = False,
+        remove_bounds_on_initial_action: bool = False,
+        name: Optional[str] = None,
+    ) -> None:
+        """Instantiates an agent with an MPC controller.
+
+        Parameters
+        ----------
+        mpc : Mpc[casadi.SX or MX]
+            The MPC controller used as policy provider by this agent. The instance is
+            modified in place to create the approximations of the state function `V(s)`
+            and action value function `Q(s,a)`, so it is recommended not to modify it
+            further after initialization of the agent. Moreover, some parameter and
+            constraint names will need to be created, so an error is thrown if these
+            names are already in use in the mpc. These names are under the attributes
+            `perturbation_parameter`, `action_parameter` and `action_constraint`.
+        fixed_parameters : dict[str, array_like] or collection of, optional
+            A dict (or collection of dict, in case of `csnlp.MultistartNlp`) whose keys
+            are the names of the MPC parameters and the values are their corresponding
+            values. Use this to specify fixed parameters, that is, non-learnable. If
+            `None`, then no fixed parameter is assumed.
+        warmstart: "last" or "last-successful" or WarmStartStrategy, optional
+            The warmstart strategy for the MPC's NLP. If `last-successful`, the last
+            successful solution is used to warm start the solver for the next iteration.
+            If `last`, the last solution is used, regardless of success or failure.
+            Furthermoer, a `WarmStartStrategy` object can be passed to specify a
+            strategy for generating multiple warmstart points for the NLP. This is
+            useful to generate multiple initial conditions for very non-convex problems.
+            Can only be used with an MPC that has an underlying multistart NLP problem
+            (see `csnlp.MultistartNlp`).
+        use_last_action_on_fail : bool, optional
+            In case the MPC solver fails
+             * if `False`, the action from the last solver's iteration is returned
+               anyway (though suboptimal)
+             * if `True`, the action from the last successful call to the MPC is
+               returned instead (if the MPC has been solved at least once successfully).
+
+            By default, `False`.
+        remove_bounds_on_initial_action : bool, optional
+            When `True`, the upper and lower bounds on the initial action are removed in
+            the action-value function approximator Q(s,a) since the first action is
+            constrained to be equal to the initial action. This is useful to avoid
+            issues in the LICQ of the NLP. However, it can lead to numerical problems.
+            By default, `False`.
+        name : str, optional
+            Name of the agent. If `None`, one is automatically created from a counter of
+            the class' instancies.
+
+        Raises
+        ------
+        ValueError
+            Raises if the given mpc has no control action as optimization variable; or
+            if the required parameter and constraint names are already specified in the
+            mpc.
+        """
+        Named.__init__(self, name)
+        SupportsDeepcopyAndPickle.__init__(self)
+        AgentCallbackMixin.__init__(self)
+        self._fixed_pars = fixed_parameters
+        self._exploration: ExplorationStrategy = NoExploration()
+        if isinstance(warmstart, str):
+            warmstart = WarmStartStrategy(warmstart)
+        self._warmstart = warmstart
+        self._last_action_on_fail = use_last_action_on_fail
+        self._last_solution: Optional[Solution[SymType]] = None
+        self._last_action: Optional[cs.DM] = None
+        self._V, self._Q = self._setup_V_and_Q(mpc, remove_bounds_on_initial_action)
+        self._post_setup_V_and_Q()
+
+    @property
+    def unwrapped(self) -> "Agent":
+        """Gets the underlying wrapped instance of an agent."""
+        return self
+
+    def is_wrapped(self, *args: Any, **kwargs: Any) -> bool:
+        """Gets whether the agent instance is wrapped or not by the wrapper type."""
+        return False
+
+    @property
+    def V(self) -> Mpc[SymType]:
+        """Gets the MPC function approximation of the state value function `V(s)`."""
+        return self._V
+
+    @property
+    def Q(self) -> Mpc[SymType]:
+        """Gets the MPC function approximation of the action value function `Q(s,a)`."""
+        return self._Q
+
+    @property
+    def fixed_parameters(
+        self,
+    ) -> Union[None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]]:
+        """Gets the fixed parameters of the MPC controller (i.e., non-learnable). Can be
+        an iterable in the case of `csnlp.MultistartNpl`, where multiple parameters can
+        be specified, one for each scenario in the MPC scheme."""
+        return self._fixed_pars
+
+    @property
+    def exploration(self) -> ExplorationStrategy:
+        """Gets the exploration strategy used within this agent."""
+        return self._exploration
+
+    @property
+    def warmstart(self) -> WarmStartStrategy:
+        """Gets the warm start strategy used within this agent."""
+        return self._warmstart
+
+    def reset(self, seed: RngType = None) -> None:
+        """Resets the agent's internal variables and exploration's RNG."""
+        self._last_solution = None
+        self._last_action = None
+        self.warmstart.reset(seed)
+        if hasattr(self.exploration, "reset"):
+            self.exploration.reset(seed)
+
+    def solve_mpc(
+        self,
+        mpc: Mpc[SymType],
+        state: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
+        action: Union[None, npt.ArrayLike, dict[str, npt.ArrayLike]] = None,
+        perturbation: Optional[npt.ArrayLike] = None,
+        vals0: Union[
+            None, dict[str, npt.ArrayLike], Iterable[dict[str, npt.ArrayLike]]
+        ] = None,
+        store_solution: bool = True,
+    ) -> Solution[SymType]:
+        """Solves the agent's specific MPC optimal control problem.
+
+        Parameters
+        ----------
+        mpc : Mpc
+            The MPC problem to solve, either `Agent.V` or `Agent.Q`.
+        state : array_like or dict[str, array_like]
+            A 1D array representing the value of all states of the MPC, concatenated.
+            Otherwise, a dict whose keys are the names of each state, and values are
+            their numerical values.
+        action : array_like or dict[str, array_like], optional
+            Same for `state`, for the action. Only valid if evaluating the action value
+            function `Q(s,a)`. For this reason, it can be `None` for `V(s)`.
+        perturbation : array_like, optional
+            The cost perturbation used to induce exploration in `V(s)`. Can be `None`
+            for `Q(s,a)`.
+        vals0 : dict[str, array_like] or iterable of, optional
+            A dict (or an iterable of dict, in case of `csnlp.MultistartNlp`), whose
+            keys are the names of the MPC variables, and values are the numerical
+            initial values of each variable. Use this to warm-start the MPC. If `None`,
+            and a previous solution (possibly, successful) is available, the MPC solver
+            is automatically warm-started.
+        store_solution : bool, optional
+            By default, the mpc solution is stored accordingly to the `warmstart`
+            strategy. If set to `False`, this flag allows to disable the behaviour for
+            this particular solution.
+
+        Returns
+        -------
+        Solution
+            The solution of the MPC.
+        """
+        # convert state keys into initial state keys (i.e., with "_0")
+        if isinstance(state, dict):
+            x0_dict = {f"{k}_0": v for k, v in state.items()}
+        else:
+            mpcstates = mpc.initial_states
+            if len(mpcstates) == 1:
+                states = (state,)
+            else:
+                cumsizes = np.cumsum([s.shape[0] for s in mpcstates.values()][:-1])
+                states = np.split(state, cumsizes)
+            x0_dict = dict(zip(mpcstates.keys(), states))
+
+        # convert action dict to vector if not None
+        if action is None:
+            u0_vec = None
+        elif isinstance(action, dict):
+            u0_vec = cs.vertcat(*(action[k] for k in mpc.actions.keys()))
+        else:
+            u0_vec = action
+
+        # merge (initial) state, action and perturbation in unique dict
+        additional_pars = x0_dict
+        if u0_vec is not None:
+            additional_pars[self.init_action_parameter] = u0_vec
+        if self.cost_perturbation_parameter in mpc.parameters:
+            additional_pars[self.cost_perturbation_parameter] = (
+                0 if perturbation is None else perturbation
+            )
+
+        # create pars and vals0
+        pars = self._get_parameters()
+        if pars is None:
+            pars = additional_pars
+        elif isinstance(pars, dict):
+            pars.update(additional_pars)
+        else:  # iterable of dict
+            pars = _update_dicts(pars, additional_pars)
+        if vals0 is None and self._last_solution is not None:
+            vals0 = self._last_solution.vals
+
+        # if available, use the warmstart strategy to generate multiple initial
+        # warm-start points for the NLP - remember to include `vals0` among these
+        if mpc.is_multi and self._warmstart.can_generate:
+            starts = mpc.nlp.starts - 1
+            n = starts // 2
+            vals0_iter = self._warmstart.generate(n, starts - n, vals0)
+            vals0 = chain((vals0,), vals0_iter)
+
+        # solve and store solution
+        sol = mpc(pars, vals0)
+        if store_solution and (self._warmstart.store_always or sol.success):
+            self._last_solution = sol
+        return sol
+
+    def state_value(
+        self,
+        state: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
+        deterministic: bool = False,
+        vals0: Union[
+            None, dict[str, npt.ArrayLike], Iterable[dict[str, npt.ArrayLike]]
+        ] = None,
+        **kwargs,
+    ) -> tuple[cs.DM, Solution[SymType]]:
+        """Computes the state value function `V(s)` approximated by the MPC.
+
+        Parameters
+        ----------
+        state : array_like or dict[str, array_like]
+            The state `s` at which to evaluate the value function `V(s)`. Can either be
+            a dict of state names and values, or a single concatenated column vector of
+            all the states.
+        deterministic : bool, optional
+            If `True`, the cost of the MPC is perturbed according to the exploration
+            strategy to induce some exploratory behaviour. Otherwise, no perturbation is
+            performed. By default, `deterministic=False`.
+        vals0 : dict[str, array_like] or iterable of, optional
+            A dict (or an iterable of dict, in case of `csnlp.MultistartNlp`), whose
+            keys are the names of the MPC variables, and values are the numerical
+            initial values of each variable. Use this to warm-start the MPC. If `None`,
+            and a previous solution (possibly, successful) is available, the MPC solver
+            is automatically warm-started.
+
+        Returns
+        -------
+        casadi.DM
+            The first optimal action according to the solution of `V(s)`.
+        Solution
+            The solution of the MPC approximating `V(s)` at the given state.
+        """
+        if deterministic or not self._exploration.can_explore():
+            pert = None
+        else:
+            pert = self._exploration.perturbation(
+                self.cost_perturbation_method,
+                size=self.V.parameters[self.cost_perturbation_parameter].shape,
+            )
+        sol = self.solve_mpc(self._V, state, perturbation=pert, vals0=vals0, **kwargs)
+        first_action = cs.vertcat(*(sol.vals[u][:, 0] for u in self._V.actions.keys()))
+
+        if sol.success:
+            self._last_action = first_action
+        elif self._last_action_on_fail and self._last_action is not None:
+            first_action = self._last_action
+
+        return first_action, sol
+
+    def action_value(
+        self,
+        state: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
+        action: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
+        vals0: Union[
+            None, dict[str, npt.ArrayLike], Iterable[dict[str, npt.ArrayLike]]
+        ] = None,
+        **kwargs,
+    ) -> Solution[SymType]:
+        """Computes the action value function `Q(s,a)` approximated by the MPC.
+
+        Parameters
+        ----------
+        state : array_like or dict[str, array_like]
+            The state `s` at which to evaluate the value function `Q(s,a)`. Can either
+            be a dict of state names and values, or a single concatenated column vector
+            of all the states.
+        action : array_like or dict[str, array_like]
+            The action `a` at which to evaluate the value function `Q(s,a)`. Can either
+            be a dict of action names and values, or a single concatenated column vector
+            of all the actions.
+        vals0 : dict[str, array_like] or iterable of, optional
+            A dict (or an iterable of dict, in case of `csnlp.MultistartNlp`), whose
+            keys are the names of the MPC variables, and values are the numerical
+            initial values of each variable. Use this to warm-start the MPC. If `None`,
+            and a previous solution (possibly, successful) is available, the MPC solver
+            is automatically warm-started.
+
+        Returns
+        -------
+        Solution
+            The solution of the MPC approximating `Q(s,a)` at given state and action.
+        """
+        return self.solve_mpc(self._Q, state, action, vals0=vals0, **kwargs)
+
+    def evaluate(
+        self,
+        env: Env[ObsType, ActType],
+        episodes: int,
+        deterministic: bool = True,
+        seed: RngType = None,
+        raises: bool = True,
+        env_reset_options: Optional[dict[str, Any]] = None,
+    ) -> npt.NDArray[np.floating]:
+        """Evaluates the agent in a given environment.
+
+        Note: after solving `V(s)` for the current state `s`, the action is computed and
+        passed to the environment as the concatenation of the first optimal action
+        variables of the MPC (see `csnlp.Mpc.actions`).
+
+        Parameters
+        ----------
+        env : Env[ObsType, ActType]
+            A gym environment where to test the agent in.
+        episodes : int
+            Number of evaluation episodes.
+        deterministic : bool, optional
+            Whether the agent should act deterministically; by default, `True`.
+        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
+            Agent's and each env's RNG seed.
+        raises : bool, optional
+            If `True`, when any of the MPC solver runs fails, or when an update fails,
+            the corresponding error is raised; otherwise, only a warning is raised.
+        env_reset_options : dict, optional
+            Additional information to specify how the environment is reset at each
+            evalution episode (optional, depending on the specific environment).
+
+        Returns
+        -------
+        array of doubles
+            The cumulative returns (one return per evaluation episode).
+
+        Raises
+        ------
+            Raises if the MPC optimization solver fails and `warns_on_exception=False`.
+        """
+        rng = np.random.default_rng(seed)
+        self.reset(rng)
+        returns = np.zeros(episodes)
+        self.on_validation_start(env)
+
+        for episode in range(episodes):
+            state, _ = env.reset(seed=mk_seed(rng), options=env_reset_options)
+            truncated, terminated, timestep = False, False, 0
+            self.on_episode_start(env, episode, state)
+
+            while not (truncated or terminated):
+                action, sol = self.state_value(state, deterministic)
+                if not sol.success:
+                    self.on_mpc_failure(episode, timestep, sol.status, raises)
+
+                state, r, truncated, terminated, _ = env.step(action)
+                self.on_env_step(env, episode, timestep)
+
+                returns[episode] += r
+                timestep += 1
+                self.on_timestep_end(env, episode, timestep)
+
+            self.on_episode_end(env, episode, returns[episode])
+
+        self.on_validation_end(env, returns)
+        return returns
+
+    def _setup_V_and_Q(
+        self, mpc: Mpc[SymType], remove_bounds_on_initial_action: bool
+    ) -> tuple[Mpc[SymType], Mpc[SymType]]:
+        """Internal utility to setup the function approximators for the value function
+        V(s) and the quality function Q(s,a)."""
+        na = mpc.na
+        if na <= 0:
+            raise ValueError(f"Expected Mpc with na>0; got na={na} instead.")
+
+        # create V and Q function approximations
+        V, Q = mpc, mpc.copy()
+        V.unwrapped.name += "_V"
+        Q.unwrapped.name += "_Q"
+        a0 = Q.nlp.parameter(self.init_action_parameter, (na, 1))
+        perturbation = V.nlp.parameter(self.cost_perturbation_parameter, (na, 1))
+
+        u0 = cs.vcat(mpc.first_actions.values())
+        f = V.nlp.f
+        if mpc.is_wrapped(wrappers.NlpScaling):
+            f = mpc.scale(f)
+
+        V.nlp.minimize(f + cs.dot(perturbation, u0))
+        Q.nlp.constraint(self.init_action_constraint, u0, "==", a0)
+
+        # remove upper/lower bound on initial action in Q, since it is constrained as a0
+        if remove_bounds_on_initial_action:
+            for name, a in mpc.first_actions.items():
+                na_ = a.size1()
+                Q.nlp.remove_variable_bounds(name, "both", ((r, 0) for r in range(na_)))
+
+        # invalidate caches for V and Q since some modifications have been done
+        for nlp in (V, Q):
+            nlp_ = nlp
+            while nlp_ is not nlp_.unwrapped:
+                invalidate_caches_of(nlp_)
+                nlp_ = nlp_.nlp
+            invalidate_caches_of(nlp_.unwrapped)
+        return V, Q
+
+    def _post_setup_V_and_Q(self) -> None:
+        """Internal utility that is run after the creation of V and Q, allowing for
+        further customization in inheriting classes."""
+        # warn user of any constraints that linearly includes x0 and u0 (aside from
+        # x(0)==s0 and u(0)==a0), which may thus lead to LICQ-failure
+        # - u0 in Q should only appear in the 1st dynamics constraint and a0 con
+        # - u0 in V should only appear in the 1st dynamics constraint and lbx/ubx
+        # - x0 in V, Q should only appear in the 1st dynamics constraint and s0 con
+        # for mpc in (self._V, self._Q):
+        #     name = mpc.unwrapped.name[-1]
+        #     u0 = cs.vcat(self._V.first_actions.values())
+        #     x0 = cs.vvcat(self._V.first_states.values())
+        #     con = cs.vertcat(mpc.g, mpc.h, mpc.h_lbx, mpc.h_ubx)
+
+        #     if mpc.unwrapped.sym_type.__name__ == "SX":
+        #         nnz_con_u0 = len(set(cs.jacobian_sparsity(con, u0).get_triplet()[0]))
+        #         nnz_con_x0 = len(set(cs.jacobian_sparsity(con, x0).get_triplet()[0]))
+        #     else:
+        #         nnz_con_u0 = len(  # computes the same as above, but for MX
+        #             set(
+        #                 chain.from_iterable(
+        #                     cs.jacobian(con, a)[:, : a.size1()]
+        #                     .sparsity()
+        #                     .get_triplet()[0]
+        #                     for a in mpc.actions.values()
+        #                 )
+        #             )
+        #         )
+        #         nnz_con_x0 = len(
+        #             set(
+        #                 chain.from_iterable(
+        #                     cs.jacobian(con, s)[:, : s.size1()]
+        #                     .sparsity()
+        #                     .get_triplet()[0]
+        #                     for s in mpc.states.values()
+        #                 )
+        #             )
+        #         )
+
+        #     nnz_exp_u0 = mpc.ns + (mpc.na * 2 if name == "V" else mpc.na)
+        #     if nnz_con_u0 > nnz_exp_u0:
+        #         warnings.warn(
+        #             f"detected {nnz_con_u0} (expected {nnz_exp_u0}) constraints on "
+        #             f"initial actions in {name}; make sure that the initial action is"
+        #             "not overconstrained (LICQ may be compromised).",
+        #             RuntimeWarning,
+        #         )
+        #     nnz_exp_x0 = mpc.ns * 2
+        #     if nnz_con_x0 > nnz_exp_x0:
+        #         warnings.warn(
+        #             f"detected {nnz_con_x0} (expected {nnz_exp_x0}) constraints on "
+        #             f"initial states in {name}; make sure that the initial state is "
+        #             "not overconstrained (LICQ may be compromised).",
+        #             RuntimeWarning,
+        #         )
+
+    def _get_parameters(
+        self,
+    ) -> Union[None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]]:
+        """Internal utility to retrieve parameters of the MPC in order to solve it.
+        `Agent` has no learnable parameter, so only fixed parameters are returned."""
+        return self._fixed_pars
+
+    def __deepcopy__(self, memo: Optional[dict[int, list[Any]]] = None) -> "Agent":
+        """Ensures that the copy has a new name."""
+        y = super().__deepcopy__(memo)
+        if hasattr(y, "name"):
+            y.name += "_copy"
+        return y
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/agents/common/globopt_learning_agent.py` & `mpcrl-1.2.0rc4/src/mpcrl/agents/common/globopt_learning_agent.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,93 +1,86 @@
-from abc import ABC
-from typing import Any, Generic, Optional
-
-from gymnasium import Env
-
-from mpcrl.agents.common.agent import ActType, ObsType
-
-from ...core.update import UpdateStrategy
-from ...optim.gradient_free_optimizer import GradientFreeOptimizer
-from .agent import SymType
-from .learning_agent import LearningAgent
-
-
-class GlobOptLearningAgent(LearningAgent[SymType, None], ABC, Generic[SymType]):
-    """Class for learning agents that employe gradient-free Global Optimization
-    strategies (e.g., Bayesian Optimization) to learn/improve the MPC policy.
-
-    An instance of this class requires a gradient-free optimizer that adheres to the
-    ask-tell interface, i..e., it must implement the `ask` and `tell` methods.
-    """
-
-    def __init__(
-        self, optimizer: GradientFreeOptimizer[SymType], **kwargs: Any
-    ) -> None:
-        """Instantiates the RL learning agent.
-
-        Parameters
-        ----------
-        optimizer : GradientFreeOptimizer
-            A gradient-free optimizer to ask for parameters and tell the values of the
-            objective function.
-        kwargs
-            Additional arguments to be passed to `LearningAgent`.
-
-            Note: the following kwargs are not yet supported
-             - "experience": usually, GO strategies do not require experience replay
-             - "update_strategy": updates are fixed at the end of each episode
-        """
-        for key in ("experience", "update_strategy"):
-            if key in kwargs:
-                raise ValueError(
-                    f"{self.__class__.__name__} does not yet support `{key}` kwargs."
-                )
-        self.optimizer = optimizer
-        super().__init__(update_strategy=UpdateStrategy(1, "on_episode_end"), **kwargs)
-        self.optimizer.set_learnable_parameters(self._learnable_pars)
-
-    def train(self, *args: Any, **kwargs: Any) -> Any:
-        # prime the initial value of the learnable parameters by asking it to the
-        # optimizer. This is the usual way to start Global Optimization strategies,
-        # whereas in RL we usually start the user's given initial values.
-        self.update()
-        return super().train(*args, **kwargs)
-
-    def train_one_episode(
-        self,
-        env: Env[ObsType, ActType],
-        episode: int,
-        init_state: ObsType,
-        raises: bool = True,
-    ) -> float:
-        # simply evaluate the MPC on the env with the current set of parameters for one
-        # episode, and then tell the optimizer the value of the objective function
-        rewards = 0.0
-        state = init_state
-        truncated, terminated, timestep = False, False, 0
-
-        while not (truncated or terminated):
-            action, sol = self.state_value(state, False)
-            if not sol.success:
-                self.on_mpc_failure(episode, timestep, sol.status, raises)
-
-            state, r, truncated, terminated, _ = env.step(action)
-            self.on_env_step(env, episode, timestep)
-
-            rewards += float(r)
-            timestep += 1
-            self.on_timestep_end(env, episode, timestep)
-
-        values = (
-            self._learnable_pars.value_as_dict
-            if self.optimizer.prefers_dict
-            else self._learnable_pars.value
-        )
-        self.optimizer.tell(values, rewards)
-        return rewards
-
-    def update(self) -> Optional[str]:
-        # simply ask the optimizer for a new set of parameters, and then update the
-        # current parameters with this new set
-        theta_new, status = self.optimizer.ask()
-        self._learnable_pars.update_values(theta_new)
-        return status
+from abc import ABC
+from typing import Any, Generic, Optional
+
+from gymnasium import Env
+
+from mpcrl.agents.common.agent import ActType, ObsType
+
+from ...core.update import UpdateStrategy
+from ...optim.gradient_free_optimizer import GradientFreeOptimizer
+from .agent import SymType
+from .learning_agent import LearningAgent
+
+
+class GlobOptLearningAgent(LearningAgent[SymType, None], ABC, Generic[SymType]):
+    """Class for learning agents that employe gradient-free Global Optimization
+    strategies (e.g., Bayesian Optimization) to learn/improve the MPC policy.
+
+    An instance of this class requires a gradient-free optimizer that adheres to the
+    ask-tell interface, i..e., it must implement the `ask` and `tell` methods.
+    """
+
+    def __init__(
+        self, optimizer: GradientFreeOptimizer[SymType], **kwargs: Any
+    ) -> None:
+        """Instantiates the RL learning agent.
+
+        Parameters
+        ----------
+        optimizer : GradientFreeOptimizer
+            A gradient-free optimizer to ask for parameters and tell the values of the
+            objective function.
+        kwargs
+            Additional arguments to be passed to `LearningAgent` (with the exclusion of
+            the `update_strategy` argument, which is always set to update at the end of
+            each episode).
+        """
+        self.optimizer = optimizer
+        super().__init__(update_strategy=UpdateStrategy(1, "on_episode_end"), **kwargs)
+        self.optimizer.set_learnable_parameters(self._learnable_pars)
+
+    def train(self, *args: Any, **kwargs: Any) -> Any:
+        # prime the initial value of the learnable parameters by asking it to the
+        # optimizer. This is the usual way to start Global Optimization strategies,
+        # whereas in RL we usually start the user's given initial values.
+        self.update()
+        return super().train(*args, **kwargs)
+
+    def train_one_episode(
+        self,
+        env: Env[ObsType, ActType],
+        episode: int,
+        init_state: ObsType,
+        raises: bool = True,
+    ) -> float:
+        # simply evaluate the MPC on the env with the current set of parameters for one
+        # episode, and then tell the optimizer the value of the objective function
+        rewards = 0.0
+        state = init_state
+        truncated, terminated, timestep = False, False, 0
+
+        while not (truncated or terminated):
+            action, sol = self.state_value(state, False)
+            if not sol.success:
+                self.on_mpc_failure(episode, timestep, sol.status, raises)
+
+            state, r, truncated, terminated, _ = env.step(action)
+            self.on_env_step(env, episode, timestep)
+
+            rewards += float(r)
+            timestep += 1
+            self.on_timestep_end(env, episode, timestep)
+
+        values = (
+            self._learnable_pars.value_as_dict
+            if self.optimizer.prefers_dict
+            else self._learnable_pars.value
+        )
+        self.optimizer.tell(values, rewards)
+        return rewards
+
+    def update(self) -> Optional[str]:
+        # simply ask the optimizer for a new set of parameters, and then update the
+        # current parameters with this new set
+        theta_new, status = self.optimizer.ask()
+        self._learnable_pars.update_values(theta_new)
+        return status
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/agents/common/learning_agent.py` & `mpcrl-1.2.0rc4/src/mpcrl/agents/common/learning_agent.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,395 +1,319 @@
-from abc import ABC, abstractmethod
-from collections.abc import Collection, Iterable
-from typing import Any, Callable, Generic, Optional, TypeVar, Union
-
-import numpy as np
-import numpy.typing as npt
-from gymnasium import Env
-
-from ...core.callbacks import LearningAgentCallbackMixin
-from ...core.experience import ExperienceReplay
-from ...core.exploration import ExplorationStrategy
-from ...core.parameters import LearnableParametersDict
-from ...core.update import UpdateStrategy
-from ...util.seeding import RngType, mk_seed
-from .agent import ActType, Agent, ObsType, SymType, _update_dicts
-
-ExpType = TypeVar("ExpType")
-
-
-class LearningAgent(
-    Agent[SymType], LearningAgentCallbackMixin, ABC, Generic[SymType, ExpType]
-):
-    """Base class for a learning agent with MPC as policy provider where the main method
-    `update`, which is called to update the learnable parameters of the MPC according to
-    the underlying learning methodology (e.g., Bayesian Optimization, RL, etc.) is
-    abstract and must be implemented by inheriting classes.
-
-    Aside of `update`, this class implements also the basic structure for both on-policy
-    and off-policy learning, which require further ad-hoc implementations. For on-policy
-    learning, the `train` method should be run, which requires the implementation of
-    `train_one_episode`. For off-policy learning, run `train_offpolicy` and implement
-    `train_one_rollout` instead. At least one of the two implementations is required in
-    the inheriting class, depending on the learning algorithm. Some algorithms might
-    support both.
-
-    Note: this class makes no assumptions on the learning methodology used to update the
-    MPC's learnable parameters."""
-
-    def __init__(
-        self,
-        update_strategy: Union[int, UpdateStrategy],
-        learnable_parameters: LearnableParametersDict[SymType],
-        exploration: Optional[ExplorationStrategy] = None,
-        experience: Union[None, int, ExperienceReplay[ExpType]] = None,
-        **kwargs: Any,
-    ) -> None:
-        """Instantiates the learning agent.
-
-        Parameters
-        ----------
-        update_strategy : UpdateStrategy or int
-            The strategy used to decide which frequency to update the mpc parameters
-            with. If an `int` is passed, then the default strategy that updates every
-            `n` env's steps is used (where `n` is the argument passed); otherwise, an
-            instance of `UpdateStrategy` can be passed to specify these in more details.
-        learnable_parameters : LearnableParametersDict
-            A special dict containing the learnable parameters of the MPC, together with
-            their bounds and values. This dict is complementary with `fixed_parameters`,
-            which contains the MPC parameters that are not learnt by the agent.
-        exploration : ExplorationStrategy, optional
-            Exploration strategy for inducing exploration in the MPC policy. By default
-            `None`, in which case `NoExploration` is used in the fixed-MPC agent.
-        experience : int or ExperienceReplay, optional
-            The container for experience replay memory. If `None` is passed, then a
-            memory with length 1 is created, i.e., it keeps only the latest memory
-            transition. If an integer `n` is passed, then a memory with the length `n`
-            is created and with sample size `n`.
-        kwargs
-            Additional arguments to be passed to `Agent`.
-        """
-        Agent.__init__(self, **kwargs)
-        LearningAgentCallbackMixin.__init__(self)
-        self._raises: bool = True
-        self._learnable_pars = learnable_parameters
-        if experience is None:
-            experience = ExperienceReplay(maxlen=1)
-        elif isinstance(experience, int):
-            experience = ExperienceReplay(maxlen=experience, sample_size=experience)
-        self._experience = experience
-        if exploration is not None:
-            self._exploration = exploration
-        if not isinstance(update_strategy, UpdateStrategy):
-            update_strategy = UpdateStrategy(update_strategy, "on_timestep_end")
-        self._update_strategy = update_strategy
-        self._updates_enabled = True
-        self.establish_callback_hooks()
-
-    @property
-    def experience(self) -> ExperienceReplay[ExpType]:
-        """Gets the experience replay memory of the agent."""
-        return self._experience
-
-    @property
-    def update_strategy(self) -> UpdateStrategy:
-        """Gets the update strategy of the agent."""
-        return self._update_strategy
-
-    @property
-    def learnable_parameters(self) -> LearnableParametersDict[SymType]:
-        """Gets the parameters of the MPC that can be learnt by the agent."""
-        return self._learnable_pars
-
-    def reset(self, seed: RngType = None) -> None:
-        """Resets agent's internal variables, exploration and experience's RNG"""
-        super().reset(seed)
-        self.experience.reset(seed)
-
-    def store_experience(self, item: ExpType) -> None:
-        """Stores the given item in the agent's memory for later experience replay.
-
-        Parameters
-        ----------
-        item : experience-type
-            Item to be stored in memory.
-        """
-        self._experience.append(item)
-
-    def evaluate(self, *args: Any, **kwargs: Any) -> npt.NDArray[np.floating]:
-        self._updates_enabled = False
-        return super().evaluate(*args, **kwargs)
-
-    def train(
-        self,
-        env: Env[ObsType, ActType],
-        episodes: int,
-        seed: RngType = None,
-        raises: bool = True,
-        env_reset_options: Optional[dict[str, Any]] = None,
-    ) -> npt.NDArray[np.floating]:
-        """On-policy training of the agent on an environment.
-
-        Parameters
-        ----------
-        env : Env[ObsType, ActType]
-            A gym environment where to train the agent in.
-        episodes : int
-            Number of training episodes.
-        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
-            Agent's and each env's RNG seed.
-        raises : bool, optional
-            If `True`, when any of the MPC solver runs fails, or when an update fails,
-            the corresponding error is raised; otherwise, only a warning is raised.
-        env_reset_options : dict, optional
-            Additional information to specify how the environment is reset at each
-            training episode (optional, depending on the specific environment).
-
-        Returns
-        -------
-        array of doubles
-            The cumulative returns for each training episode.
-
-        Raises
-        ------
-        MpcSolverError or MpcSolverWarning
-            Raises the error or the warning (depending on `raises`) if any of the MPC
-            solvers fail.
-        UpdateError or UpdateWarning
-            Raises the error or the warning (depending on `raises`) if the update fails.
-        """
-        rng = np.random.default_rng(seed)
-        self.reset(rng)
-        self._updates_enabled = True
-        self._raises = raises
-        returns = np.zeros(episodes, float)
-
-        self.on_training_start(env)
-        for episode in range(episodes):
-            state, _ = env.reset(seed=mk_seed(rng), options=env_reset_options)
-            self.on_episode_start(env, episode, state)
-            r = self.train_one_episode(env, episode, state, raises)
-            self.on_episode_end(env, episode, r)
-            returns[episode] = r
-
-        self.on_training_end(env, returns)
-        return returns
-
-    def train_one_episode(
-        self,
-        env: Env[ObsType, ActType],
-        episode: int,
-        init_state: ObsType,
-        raises: bool = True,
-    ) -> float:
-        """On-policy training of the agent on an environment for one episode.
-
-        Parameters
-        ----------
-        env : Env[ObsType, ActType]
-            A gym environment where to train the agent in.
-        episode : int
-            Number of the current training episode.
-        init_state : observation type
-            Initial state/observation of the environment.
-        raises : bool, optional
-            If `True`, when any of the MPC solver runs fails, or when an update fails,
-            the corresponding error is raised; otherwise, only a warning is raised.
-
-        Returns
-        -------
-        float
-            The cumulative rewards for this training episode.
-
-        Raises
-        ------
-        MpcSolverError or MpcSolverWarning
-            Raises the error or the warning (depending on `raises`) if any of the MPC
-            solvers fail.
-        UpdateError or UpdateWarning
-            Raises the error or the warning (depending on `raises`) if the update fails.
-        """
-        raise NotImplementedError(
-            f"{self.__class__.__name__} does not implement `train_one_episode` for "
-            "on-policy learning."
-        )
-
-    def train_offpolicy(
-        self,
-        episode_rollouts: Iterable[Iterable[Any]],
-        seed: RngType = None,
-        raises: bool = True,
-        eval_frequency: Optional[int] = None,
-        eval_env_factory: Callable[[], Optional[Env[ObsType, ActType]]] = None,
-        eval_kwargs: Optional[dict[str, Any]] = None,
-        eval_at_start: bool = True,
-    ) -> Optional[npt.NDArray[np.floating]]:
-        """Off-policy training of the agent on an environment.
-
-        Parameters
-        ----------
-        episode_rollouts : iterable of iterables of any
-            An iterable, i.e., sequence, of episodical rollouts generated off-policy.
-            Each rollout is itself a sequence of transitions, e.g., SARSA tuples. In
-            general, these can be of different types, depending on the specific learning
-            algorithm.
-        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
-            Agent's (and each evaluation env's, if applicable) RNG seed.
-        raises : bool, optional
-            If `True`, when any of the MPC solver runs fails, or when an update fails,
-            the corresponding error is raised; otherwise, only a warning is raised.
-        eval_frequency : int, optional
-            Frequency of evaluation of the agent's performance during off-policy
-            training. If `None`, no evaluation is performed. If an integer is passed,
-            then also `eval_env_factory` must be given as argument.
-        eval_env_factory : callable, optional
-            A callable that returns a new environment instance to be used for
-            evaluation, if `eval_frequency` is given. Otherwise, it is unused.
-        eval_kwargs : dict, optional
-            Additional keyword arguments to be passed to the agent's `evaluate` method.
-            Must contain the `episode` key (which is a required argument to `evaluate`),
-            and must not contain the `env`, `seed` or `raises` key, as these are already
-            handled by this method automatically.
-        eval_at_start : bool, optional
-            If `True`, an evaluation round is also performed before the training starts.
-
-        Returns
-        -------
-        2d-array of doubles or None
-            The cumulative returns for each evaluation episode, if evaluation is
-            enabled; otherwise, `None`.
-
-        Raises
-        ------
-        ValueError
-            Raises if `eval_frequency` is given but `eval_env_factory` is not callable.
-        MpcSolverError or MpcSolverWarning
-            Raises the error or the warning (depending on `raises`) if any of the MPC
-            solvers fail.
-        UpdateError or UpdateWarning
-            Raises the error or the warning (depending on `raises`) if the update fails.
-        """
-        if eval_frequency is not None:
-            if not callable(eval_env_factory):
-                raise ValueError(
-                    "If `eval_frequency` is given, `eval_env_factory` must be callable."
-                )
-            returns = []
-            if eval_kwargs is None:
-                eval_kwargs = {}
-            do_eval = lambda: self.evaluate(
-                eval_env_factory(), seed=rng, raises=raises, **eval_kwargs
-            )
-        else:
-            returns = np.empty(())
-
-        rng = np.random.default_rng(seed)
-        self.reset(rng)
-        self._raises = raises
-        env_proxy = "off-policy"
-
-        if eval_frequency is not None and eval_at_start:
-            returns.append(do_eval())
-
-        self._updates_enabled = True
-        self.on_training_start(env_proxy)
-        for episode, rollout in enumerate(episode_rollouts):
-            self.on_episode_start(env_proxy, episode, float("nan"))
-            self.train_one_rollout(rollout, episode, raises)
-            self.on_episode_end(env_proxy, episode, float("nan"))
-            if eval_frequency is not None and (episode + 1) % eval_frequency == 0:
-                returns.append(do_eval())
-                self._updates_enabled = True  # updates must be re-enabled after eval
-
-        returns = np.asarray(returns, float)
-        self.on_training_end(env_proxy, returns)
-        if eval_frequency is not None:
-            return returns
-
-    def train_one_rollout(
-        self, rollout: Iterable[Any], episode: int, raises: bool = True
-    ) -> None:
-        """Train the agent in an off-policy manner on the given rollout.
-
-        Parameters
-        ----------
-        rollout : iterable of any
-            Rollout, i.e., a sequence of transitions generated off-policy, e.g., SARSA
-            tuples. In general, these can be of different types, depending on the
-            specific learning algorithm.
-        raises : bool, optional
-            If `True`, when any of the MPC solver runs fails, or when an update fails,
-            the corresponding error is raised; otherwise, only a warning is raised.
-
-        Raises
-        ------
-        MpcSolverError or MpcSolverWarning
-            Raises the error or the warning (depending on `raises`) if any of the MPC
-            solvers fail.
-        UpdateError or UpdateWarning
-            Raises the error or the warning (depending on `raises`) if the update fails.
-        """
-        raise NotImplementedError(
-            f"{self.__class__.__name__} does not implement `train_offpolicy` for "
-            "off-policy learning."
-        )
-
-    @abstractmethod
-    def update(self) -> Optional[str]:
-        """Updates the learnable parameters of the MPC according to the agent's learning
-        algorithm.
-
-        Returns
-        -------
-        errormsg : str or None
-            In case the update fails, an error message is returned to be raised as error
-            or warning; otherwise, `None` is returned.
-        """
-
-    def establish_callback_hooks(self) -> None:
-        super().establish_callback_hooks()
-        # hook exploration (only if necessary)
-        exploration_hook: Optional[str] = getattr(self._exploration, "hook", None)
-        if exploration_hook is not None:
-            self.hook_callback(
-                repr(self._exploration), exploration_hook, self._exploration.step
-            )
-        # hook updates (always necessary)
-        assert self._update_strategy.hook in {
-            "on_episode_end",
-            "on_timestep_end",
-        }, "Updates can be hooked only to `episode_end` or `on_timestep_end`."
-        func: Callable[..., None] = (
-            (lambda _, e, __: self._check_and_perform_update(e, None))
-            if self._update_strategy.hook == "on_episode_end"
-            else (lambda _, e, t: self._check_and_perform_update(e, t))
-        )
-        self.hook_callback(
-            repr(self._update_strategy),
-            self._update_strategy.hook,
-            func,
-        )
-
-    def _check_and_perform_update(self, episode: int, timestep: Optional[int]) -> None:
-        """Internal utility to check if an update is due and perform it."""
-        if not self._updates_enabled or not self._update_strategy.can_update():
-            return
-        update_msg = self.update()
-        if update_msg is not None:
-            self.on_update_failure(episode, timestep, update_msg, self._raises)
-        self.on_update()
-
-    def _get_parameters(
-        self,
-    ) -> Union[None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]]:
-        """Internal utility to retrieve parameters of the MPC in order to solve it.
-        `LearningAgent` returns both fixed and learnable parameters."""
-        learnable_pars = self._learnable_pars.value_as_dict
-        fixed_pars = self._fixed_pars
-        if fixed_pars is None:
-            return learnable_pars  # type: ignore[return-value]
-        if isinstance(fixed_pars, dict):
-            fixed_pars.update(learnable_pars)
-            return fixed_pars
-        return tuple(
-            _update_dicts(self._fixed_pars, learnable_pars)  # type: ignore[arg-type]
-        )
+from abc import ABC, abstractmethod
+from collections.abc import Collection, Iterable
+from typing import Any, Callable, Generic, Optional, TypeVar, Union
+
+import numpy as np
+import numpy.typing as npt
+from gymnasium import Env
+
+from ...core.callbacks import LearningAgentCallbackMixin
+from ...core.exploration import ExplorationStrategy
+from ...core.parameters import LearnableParametersDict
+from ...core.update import UpdateStrategy
+from ...util.seeding import RngType, mk_seed
+from .agent import ActType, Agent, ObsType, SymType, _update_dicts
+
+ExpType = TypeVar("ExpType")
+
+
+class LearningAgent(
+    Agent[SymType], LearningAgentCallbackMixin, ABC, Generic[SymType, ExpType]
+):
+    """Base class for a learning agent with MPC as policy provider where the main method
+    `update`, which is called to update the learnable parameters of the MPC according to
+    the underlying learning methodology (e.g., Bayesian Optimization, RL, etc.) is
+    abstract and must be implemented by inheriting classes.
+
+    Aside of `update`, this class implements also the basic structure for both on-policy
+    and off-policy learning, which require further ad-hoc implementations. For on-policy
+    learning, the `train` method should be run, which requires the implementation of
+    `train_one_episode`. For off-policy learning, run `train_offpolicy` and implement
+    `train_one_rollout` instead. At least one of the two implementations is required in
+    the inheriting class, depending on the learning algorithm. Some algorithms might
+    support both.
+
+    Note: this class makes no assumptions on the learning methodology used to update the
+    MPC's learnable parameters."""
+
+    def __init__(
+        self,
+        update_strategy: Union[int, UpdateStrategy],
+        learnable_parameters: LearnableParametersDict[SymType],
+        exploration: Optional[ExplorationStrategy] = None,
+        **kwargs: Any,
+    ) -> None:
+        """Instantiates the learning agent.
+
+        Parameters
+        ----------
+        update_strategy : UpdateStrategy or int
+            The strategy used to decide which frequency to update the mpc parameters
+            with. If an `int` is passed, then the default strategy that updates every
+            `n` env's steps is used (where `n` is the argument passed); otherwise, an
+            instance of `UpdateStrategy` can be passed to specify these in more details.
+        learnable_parameters : LearnableParametersDict
+            A special dict containing the learnable parameters of the MPC, together with
+            their bounds and values. This dict is complementary with `fixed_parameters`,
+            which contains the MPC parameters that are not learnt by the agent.
+        exploration : ExplorationStrategy, optional
+            Exploration strategy for inducing exploration in the MPC policy. By default
+            `None`, in which case `NoExploration` is used in the fixed-MPC agent.
+        kwargs
+            Additional arguments to be passed to `Agent`.
+        """
+        Agent.__init__(self, **kwargs)
+        LearningAgentCallbackMixin.__init__(self)
+        self._raises: bool = True
+        self._learnable_pars = learnable_parameters
+        if exploration is not None:
+            self._exploration = exploration
+        if not isinstance(update_strategy, UpdateStrategy):
+            update_strategy = UpdateStrategy(update_strategy, "on_timestep_end")
+        self._update_strategy = update_strategy
+        self._updates_enabled = True
+        self.establish_callback_hooks()
+
+    @property
+    def update_strategy(self) -> UpdateStrategy:
+        """Gets the update strategy of the agent."""
+        return self._update_strategy
+
+    @property
+    def learnable_parameters(self) -> LearnableParametersDict[SymType]:
+        """Gets the parameters of the MPC that can be learnt by the agent."""
+        return self._learnable_pars
+
+    def evaluate(self, *args: Any, **kwargs: Any) -> npt.NDArray[np.floating]:
+        self._updates_enabled = False
+        return super().evaluate(*args, **kwargs)
+
+    def train(
+        self,
+        env: Env[ObsType, ActType],
+        episodes: int,
+        seed: RngType = None,
+        raises: bool = True,
+        env_reset_options: Optional[dict[str, Any]] = None,
+    ) -> npt.NDArray[np.floating]:
+        """On-policy training of the agent on an environment.
+
+        Parameters
+        ----------
+        env : Env[ObsType, ActType]
+            A gym environment where to train the agent in.
+        episodes : int
+            Number of training episodes.
+        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
+            Agent's and each env's RNG seed.
+        raises : bool, optional
+            If `True`, when any of the MPC solver runs fails, or when an update fails,
+            the corresponding error is raised; otherwise, only a warning is raised.
+        env_reset_options : dict, optional
+            Additional information to specify how the environment is reset at each
+            training episode (optional, depending on the specific environment).
+
+        Returns
+        -------
+        array of doubles
+            The cumulative returns for each training episode.
+
+        Raises
+        ------
+        MpcSolverError or MpcSolverWarning
+            Raises the error or the warning (depending on `raises`) if any of the MPC
+            solvers fail.
+        UpdateError or UpdateWarning
+            Raises the error or the warning (depending on `raises`) if the update fails.
+        """
+        rng = np.random.default_rng(seed)
+        self.reset(rng)
+        self._updates_enabled = True
+        self._raises = raises
+        returns = np.zeros(episodes, float)
+
+        self.on_training_start(env)
+        for episode in range(episodes):
+            state, _ = env.reset(seed=mk_seed(rng), options=env_reset_options)
+            self.on_episode_start(env, episode, state)
+            r = self.train_one_episode(env, episode, state, raises)
+            self.on_episode_end(env, episode, r)
+            returns[episode] = r
+
+        self.on_training_end(env, returns)
+        return returns
+
+    def train_one_episode(
+        self,
+        env: Env[ObsType, ActType],
+        episode: int,
+        init_state: ObsType,
+        raises: bool = True,
+    ) -> float:
+        """On-policy training of the agent on an environment for one episode.
+
+        Parameters
+        ----------
+        env : Env[ObsType, ActType]
+            A gym environment where to train the agent in.
+        episode : int
+            Number of the current training episode.
+        init_state : observation type
+            Initial state/observation of the environment.
+        raises : bool, optional
+            If `True`, when any of the MPC solver runs fails, or when an update fails,
+            the corresponding error is raised; otherwise, only a warning is raised.
+
+        Returns
+        -------
+        float
+            The cumulative rewards for this training episode.
+
+        Raises
+        ------
+        MpcSolverError or MpcSolverWarning
+            Raises the error or the warning (depending on `raises`) if any of the MPC
+            solvers fail.
+        UpdateError or UpdateWarning
+            Raises the error or the warning (depending on `raises`) if the update fails.
+        """
+        raise NotImplementedError(
+            f"{self.__class__.__name__} does not implement `train_one_episode` for "
+            "on-policy learning."
+        )
+
+    def train_offpolicy(
+        self,
+        episode_rollouts: Iterable[Iterable[Any]],
+        seed: RngType = None,
+        raises: bool = True,
+    ) -> None:
+        """Off-policy training of the agent on an environment.
+
+        Parameters
+        ----------
+        episode_rollouts : iterable of iterables of any
+            An iterable (i.e., a sequence) of episodical rollouts generated off-policy.
+            Each rollout is itself a sequence of transitions, e.g., SARSA tuples. In
+            general, these can be of different types, depending on the specific learning
+            algorithm.
+        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
+            Agent's (and each evaluation env's, if applicable) RNG seed.
+        raises : bool, optional
+            If `True`, when any of the MPC solver runs fails, or when an update fails,
+            the corresponding error is raised; otherwise, only a warning is raised.
+
+        Raises
+        ------
+        MpcSolverError or MpcSolverWarning
+            Raises the error or the warning (depending on `raises`) if any of the MPC
+            solvers fail.
+        UpdateError or UpdateWarning
+            Raises the error or the warning (depending on `raises`) if the update fails.
+        """
+        # TODO: implement the agent's `EvalWrapper` and use that to evaluate the
+        # agent's performance during off-policy training.
+
+        # TODO: `train` will need a rehaul, right? it will need to collect offpolicy
+
+        rng = np.random.default_rng(seed)
+        self.reset(rng)
+        self._raises = raises
+        env_proxy = "off-policy"
+
+        self._updates_enabled = True
+        self.on_training_start(env_proxy)
+        for episode, rollout in enumerate(episode_rollouts):
+            self.on_episode_start(env_proxy, episode, float("nan"))
+            self.train_one_rollout(rollout, episode, raises)
+            self.on_episode_end(env_proxy, episode, float("nan"))
+
+        self.on_training_end(env_proxy, [])
+
+    def train_one_rollout(
+        self, rollout: Iterable[Any], episode: int, raises: bool = True
+    ) -> None:
+        """Train the agent in an off-policy manner on the given rollout.
+
+        Parameters
+        ----------
+        rollout : iterable of any
+            Rollout, i.e., a sequence of transitions generated off-policy, e.g., SARSA
+            tuples. In general, these can be of different types, depending on the
+            specific learning algorithm.
+        raises : bool, optional
+            If `True`, when any of the MPC solver runs fails, or when an update fails,
+            the corresponding error is raised; otherwise, only a warning is raised.
+
+        Raises
+        ------
+        MpcSolverError or MpcSolverWarning
+            Raises the error or the warning (depending on `raises`) if any of the MPC
+            solvers fail.
+        UpdateError or UpdateWarning
+            Raises the error or the warning (depending on `raises`) if the update fails.
+        """
+        raise NotImplementedError(
+            f"{self.__class__.__name__} does not implement `train_offpolicy` for "
+            "off-policy learning."
+        )
+
+    @abstractmethod
+    def update(self) -> Optional[str]:
+        """Updates the learnable parameters of the MPC according to the agent's learning
+        algorithm.
+
+        Returns
+        -------
+        errormsg : str or None
+            In case the update fails, an error message is returned to be raised as error
+            or warning; otherwise, `None` is returned.
+        """
+
+    def establish_callback_hooks(self) -> None:
+        super().establish_callback_hooks()
+        # hook exploration (only if necessary)
+        exploration_hook: Optional[str] = getattr(self._exploration, "hook", None)
+        if exploration_hook is not None:
+            self.hook_callback(
+                repr(self._exploration), exploration_hook, self._exploration.step
+            )
+        # hook updates (always necessary)
+        assert self._update_strategy.hook in {
+            "on_episode_end",
+            "on_timestep_end",
+        }, "Updates can be hooked only to `episode_end` or `on_timestep_end`."
+        func: Callable[..., None] = (
+            (lambda _, e, __: self._check_and_perform_update(e, None))
+            if self._update_strategy.hook == "on_episode_end"
+            else (lambda _, e, t: self._check_and_perform_update(e, t))
+        )
+        self.hook_callback(
+            repr(self._update_strategy),
+            self._update_strategy.hook,
+            func,
+        )
+
+    def _check_and_perform_update(self, episode: int, timestep: Optional[int]) -> None:
+        """Internal utility to check if an update is due and perform it."""
+        if not self._updates_enabled or not self._update_strategy.can_update():
+            return
+        update_msg = self.update()
+        if update_msg is not None:
+            self.on_update_failure(episode, timestep, update_msg, self._raises)
+        self.on_update()
+
+    def _get_parameters(
+        self,
+    ) -> Union[None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]]:
+        """Internal utility to retrieve parameters of the MPC in order to solve it.
+        `LearningAgent` returns both fixed and learnable parameters."""
+        learnable_pars = self._learnable_pars.value_as_dict
+        fixed_pars = self._fixed_pars
+        if fixed_pars is None:
+            return learnable_pars  # type: ignore[return-value]
+        if isinstance(fixed_pars, dict):
+            fixed_pars.update(learnable_pars)
+            return fixed_pars
+        return tuple(
+            _update_dicts(self._fixed_pars, learnable_pars)  # type: ignore[arg-type]
+        )
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/agents/common/rl_learning_agent.py` & `mpcrl-1.2.0rc4/src/mpcrl/agents/common/offpolicy_rl_agent copy.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from abc import ABC
-from typing import Any, Generic, TypeVar
-
-from ...optim.gradient_based_optimizer import GradientBasedOptimizer, LrType
-from .agent import SymType
-from .learning_agent import LearningAgent
-
-ExpType = TypeVar("ExpType")
-
-
-class RlLearningAgent(
-    LearningAgent[SymType, ExpType], ABC, Generic[SymType, ExpType, LrType]
-):
-    """Base class for learning agents that employe gradient-based RL strategies to
-    learn/improve the MPC policy."""
-
-    def __init__(
-        self,
-        discount_factor: float,
-        optimizer: GradientBasedOptimizer[SymType, LrType],
-        **kwargs: Any,
-    ) -> None:
-        """Instantiates the RL learning agent.
-
-        Parameters
-        ----------
-        discount_factor : float
-            In RL, the factor that discounts future rewards in favor of immediate
-            rewards. Usually denoted as `\\gamma`. Should be a number in (0, 1).
-        optimizer : GradientBasedOptimizer
-            A gradient-based optimizer (e.g., `mpcrl.optim.GradientDescent`) to compute
-            the updates of the learnable parameters, based on the current gradient-based
-            RL algorithm.
-        kwargs
-            Additional arguments to be passed to `LearningAgent`.
-        """
-        self.discount_factor = discount_factor
-        self.optimizer = optimizer
-        super().__init__(**kwargs)
-        self.optimizer.set_learnable_parameters(self._learnable_pars)
-
-    def establish_callback_hooks(self) -> None:
-        super().establish_callback_hooks()
-        optim = self.optimizer
-        optimizer_hook = optim.hook
-        if optimizer_hook is not None:
-            self.hook_callback(repr(optim), optimizer_hook, optim.step)
+from abc import ABC
+from typing import Any, Generic, TypeVar
+
+from ...optim.gradient_based_optimizer import GradientBasedOptimizer, LrType
+from .agent import SymType
+from .learning_agent import LearningAgent
+
+ExpType = TypeVar("ExpType")
+
+
+class RlLearningAgent(
+    LearningAgent[SymType, ExpType], ABC, Generic[SymType, ExpType, LrType]
+):
+    """Base class for learning agents that employe gradient-based RL strategies to
+    learn/improve the MPC policy."""
+
+    def __init__(
+        self,
+        discount_factor: float,
+        optimizer: GradientBasedOptimizer[SymType, LrType],
+        **kwargs: Any,
+    ) -> None:
+        """Instantiates the RL learning agent.
+
+        Parameters
+        ----------
+        discount_factor : float
+            In RL, the factor that discounts future rewards in favor of immediate
+            rewards. Usually denoted as `\\gamma`. Should be a number in (0, 1).
+        optimizer : GradientBasedOptimizer
+            A gradient-based optimizer (e.g., `mpcrl.optim.GradientDescent`) to compute
+            the updates of the learnable parameters, based on the current gradient-based
+            RL algorithm.
+        kwargs
+            Additional arguments to be passed to `LearningAgent`.
+        """
+        self.discount_factor = discount_factor
+        self.optimizer = optimizer
+        super().__init__(**kwargs)
+        self.optimizer.set_learnable_parameters(self._learnable_pars)
+
+    def establish_callback_hooks(self) -> None:
+        super().establish_callback_hooks()
+        optim = self.optimizer
+        optimizer_hook = optim.hook
+        if optimizer_hook is not None:
+            self.hook_callback(repr(optim), optimizer_hook, optim.step)
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/agents/lstd_dpg.py` & `mpcrl-1.2.0rc4/src/mpcrl/agents/lstd_dpg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,411 +1,423 @@
-from collections.abc import Collection, Iterator
-from typing import Callable, Generic, Literal, Optional, SupportsFloat, Union
-
-import casadi as cs
-import numba as nb
-import numpy as np
-import numpy.typing as npt
-from csnlp.wrappers import Mpc, NlpSensitivity
-from gymnasium import Env
-from typing_extensions import TypeAlias
-
-from ..core.experience import ExperienceReplay
-from ..core.exploration import ExplorationStrategy
-from ..core.parameters import LearnableParametersDict
-from ..core.update import UpdateStrategy
-from ..optim.gradient_based_optimizer import GradientBasedOptimizer
-from ..util.math import monomials_basis_function
-from .common.agent import ActType, ObsType, SymType
-from .common.rl_learning_agent import LrType, RlLearningAgent
-
-ExpType: TypeAlias = tuple[
-    npt.NDArray[np.floating],  # rollout's costs
-    npt.NDArray[np.floating],  # rollout's state feature vectors Phi(s)
-    npt.NDArray[np.floating],  # rollout's Psi(s,a)
-    npt.NDArray[np.floating],  # rollout's gradient of policy w.r.t. theta
-    npt.NDArray[np.floating],  # rollout's CAFA weight v
-]
-
-
-class LstdDpgAgent(RlLearningAgent[SymType, ExpType, LrType], Generic[SymType, LrType]):
-    """Least-Squares Temporal Difference (LSTD) Deterministic Policy Gradient (DPG)
-    agent, as first introduced in [1] as its stochastic counterpart, and then refined in
-    [2]. An application can be found in [3].
-
-    The DPG agent uses an MPC controller as policy provider and function approximation,
-    and adjusts its parametrization according to the temporal-difference error, with the
-    goal of improving the policy, in a direct fashion by estimating the gradient of the
-    policy and descending in its direction.
-
-    References
-    ----------
-    [1] Gros, S. and Zanon, M., 2021, May. Reinforcement Learning based on MPC
-        and the Stochastic Policy Gradient Method. In 2021 American Control
-        Conference (ACC) (pp. 1947-1952). IEEE.
-    [2] Gros, S. and Zanon, M., 2019. Towards Safe Reinforcement Learning Using NMPC and
-        Policy Gradients: Part II - Deterministic Case. arXiv preprint arXiv:1906.04034.
-    [3] Cai, W., Kordabad, A.B., Esfahani, H.N., Lekkas, A.M. and Gros, S., 2021,
-        December. MPC-based reinforcement learning for a simplified freight mission of
-        autonomous surface vehicles. In 2021 60th IEEE Conference on Decision and
-        Control (CDC) (pp. 2990-2995). IEEE.
-    """
-
-    def __init__(
-        self,
-        mpc: Mpc[SymType],
-        update_strategy: Union[int, UpdateStrategy],
-        discount_factor: float,
-        optimizer: GradientBasedOptimizer,
-        learnable_parameters: LearnableParametersDict[SymType],
-        fixed_parameters: Union[
-            None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]
-        ] = None,
-        exploration: Optional[ExplorationStrategy] = None,
-        experience: Union[None, int, ExperienceReplay[ExpType]] = None,
-        warmstart: Literal["last", "last-successful"] = "last-successful",
-        rollout_length: Optional[int] = None,
-        record_policy_performance: bool = False,
-        record_policy_gradient: bool = False,
-        state_features: Optional[cs.Function] = None,
-        linsolver: Literal["csparse", "mldivide"] = "csparse",
-        ridge_regression_regularization: float = 1e-6,
-        use_last_action_on_fail: bool = False,
-        name: Optional[str] = None,
-    ) -> None:
-        """Instantiates the LSTD DPG agent.
-
-        Parameters
-        ----------
-        mpc : Mpc[casadi.SX or MX]
-            The MPC controller used as policy provider by this agent. The instance is
-            modified in place to create the approximations of the state function `V(s)`
-            and action value function `Q(s,a)`, so it is recommended not to modify it
-            further after initialization of the agent. Moreover, some parameter and
-            constraint names will need to be created, so an error is thrown if these
-            names are already in use in the mpc. These names are under the attributes
-            `perturbation_parameter`, `action_parameter` and `action_constraint`.
-        update_strategy : UpdateStrategy or int
-            The strategy used to decide which frequency to update the mpc parameters
-            with. If an `int` is passed, then the default strategy that updates every
-            `n` episodes is used (where `n` is the argument passed); otherwise, an
-            instance of `UpdateStrategy` can be passed to specify these in more details.
-        discount_factor : float
-            In RL, the factor that discounts future rewards in favor of immediate
-            rewards. Usually denoted as `\\gamma`. Should be a number in (0, 1).
-        optimizer : GradientBasedOptimizer
-            A gradient-based optimizer (e.g., `mpcrl.optim.GradientDescent`) to compute
-            the updates of the learnable parameters, based on the current gradient-based
-            RL algorithm.
-        learnable_parameters : LearnableParametersDict
-            A special dict containing the learnable parameters of the MPC, together with
-            their bounds and values. This dict is complementary with `fixed_parameters`,
-            which contains the MPC parameters that are not learnt by the agent.
-        fixed_parameters : dict[str, array_like] or collection of, optional
-            A dict (or collection of dict, in case of `csnlp.MultistartNlp`) whose keys
-            are the names of the MPC parameters and the values are their corresponding
-            values. Use this to specify fixed parameters, that is, non-learnable. If
-            `None`, then no fixed parameter is assumed.
-        exploration : ExplorationStrategy, optional
-            Exploration strategy for inducing exploration in the MPC policy. By default
-            `None`, in which case `NoExploration` is used in the fixed-MPC agent.
-        experience : int or ExperienceReplay, optional
-            The container for experience replay memory. If `None` is passed, then a
-            memory with length 1 is created, i.e., it keeps only the latest memory
-            transition. If an integer `n` is passed, then a memory with the length `n`
-            is created and with sample size `n`.
-            In case of LSTD DPG, each memory item is obtain from a single rollout, and
-            is a 4-tuple that contains: costs, state vector features (Phi), Psi (a
-            temporary value), and the gradient of the policy.
-        max_percentage_update : float, optional
-            A positive float that specifies the maximum percentage the parameters can be
-            changed during each update. For example, `max_percentage_update=0.5` means
-            that the parameters can be updated by up to 50% of their current value. By
-            default, it is set to `+inf`.
-        weight_decay : float, optional
-            A positive float that specifies the decay of the learnable parameters in the
-            form of an L2 regularization term. By default, it is set to `0.0`, so no
-            decay/regularization takes place.
-        warmstart: 'last' or 'last-successful', optional
-            The warmstart strategy for the MPC's NLP. If 'last-successful', the last
-            successful solution is used to warm start the solver for the next iteration.
-            If 'last', the last solution is used, regardless of success or failure.
-        rollout_length : int, optional
-            Time-step length of a closed-loop simulation, which defines a complete
-            trajectory of the states, and is saved in the experience as a single item
-            (since LSTD DPG needs to draw samples of trajectories). In case the env is
-            episodic, it can be `None`, in which case the rollout length coincides with
-            the episode's. In case the env is not episodic, i.e., it never terminates, a
-            rollout length must be given in order to save the current trajectory as an
-            atomic item in memory.
-        record_policy_performance: bool, optional
-            If `True`, the performance of each rollout is stored in the field
-            `policy_performances`, which otherwise is `None`. By default, does not
-            record them.
-        record_policy_gradient: bool, optional
-            If `True`, the (estimated) policy gradient of each update is stored in the
-            field `policy_gradients`, which otherwise is `None`. By default, does not
-            record them.
-        state_features : casadi.Function, optional
-            The state feature vector to be used in the linear approximation of the
-            value function, which takes the form of
-            ```
-            V_v(s) = Phi(s)^T * v
-            ```
-            where `s` is the state, `v` are the weights, and `Phi(s)` is the state
-            feature vector. This function is assumed to have one input and one output.
-            By default, if not provided, it is designed as all monomials of the state
-            with degrees <= 2 (see `mpcrl.util.math.monomials_basis_function`).
-        linsolver : "csparse" or "mldivide", optional
-            The type of linear solver to be used for solving the linear system derived
-            from the KKT conditions and used to estimate the gradient of the policy. By
-            default, `"csparse"` is chosen as the KKT matrix is most often sparse.
-        ridge_regression_regularization : float, optional
-            Ridge regression regularization used during the computations of the LSTD
-            weights via least-squares. By default, `1e-6`.
-        use_last_action_on_fail : bool, optional
-            When `True`, if the MPC solver fails in solving the state value function
-            `V(s)`, the last successful action is returned. When `False`, the action
-            from the last MPC iteration is returned instead. By default, `False`.
-        name : str, optional
-            Name of the agent. If `None`, one is automatically created from a counter of
-            the class' instancies.
-        """
-        # change default update hook to 'on_episode_end'
-        if not isinstance(update_strategy, UpdateStrategy):
-            update_strategy = UpdateStrategy(update_strategy, "on_episode_end")
-        super().__init__(
-            mpc=mpc,
-            update_strategy=update_strategy,
-            discount_factor=discount_factor,
-            optimizer=optimizer,
-            learnable_parameters=learnable_parameters,
-            fixed_parameters=fixed_parameters,
-            exploration=exploration,
-            experience=experience,
-            warmstart=warmstart,
-            use_last_action_on_fail=use_last_action_on_fail,
-            name=name,
-        )
-        self._sensitivity = self._init_sensitivity(linsolver)
-        self._Phi = (
-            monomials_basis_function(mpc.ns, 0, 2)
-            if state_features is None
-            else state_features
-        )
-        self.ridge_regression_regularization = ridge_regression_regularization
-        self.rollout_length = rollout_length or float("+inf")
-        self._rollout: list[
-            tuple[
-                ObsType,
-                ActType,
-                SupportsFloat,
-                ObsType,
-                npt.NDArray[np.floating],
-            ]
-        ] = nb.typed.List()
-        self.policy_performances: Optional[list[float]] = (
-            [] if record_policy_performance else None
-        )
-        self.policy_gradients: Optional[list[npt.NDArray[np.floating]]] = (
-            [] if record_policy_gradient else None
-        )
-
-    def update(self) -> Optional[str]:
-        sample = self.experience.sample()
-        dJdtheta = _estimate_gradient_update(
-            sample, self.discount_factor, self.ridge_regression_regularization
-        )
-        if self.policy_gradients is not None:
-            self.policy_gradients.append(dJdtheta)
-        return self.optimizer.update(dJdtheta)
-
-    def train_one_episode(
-        self,
-        env: Env[ObsType, ActType],
-        episode: int,
-        init_state: ObsType,
-        raises: bool = True,
-    ) -> float:
-        truncated = terminated = False
-        timestep = 0
-        rewards = 0.0
-        state = init_state
-
-        while not (truncated or terminated):
-            # compute V(s) (perturbed and not perturbed)
-            action, sol = self.state_value(state, False)
-            action_opt, sol_opt = self.state_value(state, True)
-
-            # step the system with the action just computed
-            state_new, cost, truncated, terminated, _ = env.step(action)
-            self.on_env_step(env, episode, timestep)
-
-            # store transition in experience
-            if sol.success and sol_opt.success:
-                # NOTE: according to Cai et al. [3], the sensitivities should naively be
-                # computed with the solution of unpertubed MPC (i.e., sol_opt).
-                # According to Gros and Zanon [2], it is hinted that the perturbed
-                # solution should be used instead (sol).
-                exploration = np.asarray((action - action_opt).elements())
-                sol_vals = np.asarray(sol_opt.all_vals.elements())
-                self._rollout.append((state, exploration, cost, state_new, sol_vals))
-            else:
-                status = f"{sol.status}/{sol_opt.status}"
-                self.on_mpc_failure(episode, timestep, status, raises)
-
-            # increase counters
-            state = state_new
-            rewards += float(cost)
-            timestep += 1
-
-            # first, check if current rollout has reached its length, and only then
-            # invoke on_timestep_end (as it might trigger an update)
-            if len(self._rollout) >= self.rollout_length:
-                self._consolidate_rollout_into_memory()
-            self.on_timestep_end(env, episode, timestep)
-
-        # consolidate rollout at the end of episode, if no length was specified
-        if self.rollout_length == float("+inf"):
-            self._consolidate_rollout_into_memory()
-        return rewards
-
-    def _init_sensitivity(self, linsolver: str) -> Callable[[cs.DM, int], np.ndarray]:
-        """Internal utility to compute the derivatives w.r.t. the learnable parameters
-        and other functions in order to estimate the policy gradient."""
-        assert self.optimizer._order == 1, "Expected 1st-order optimizer."
-        nlp = self._V.nlp
-        y = nlp.primal_dual
-        theta = cs.vvcat(self._learnable_pars.sym.values())
-        u0 = cs.vcat(self._V.first_actions.values())
-        x_lam_p = cs.vertcat(nlp.primal_dual, nlp.p)
-
-        # compute first bunch of derivatives
-        nlp_ = NlpSensitivity(nlp, theta)
-        Kt = nlp_.jacobians["K-p"]
-        Ky = nlp_.jacobians["K-y"]
-        dydu0 = cs.jacobian_sparsity(u0, y).T
-
-        # instantiate linear solver (must be MX, so SX has to be converted)
-        if nlp.sym_type is cs.SX:
-            x_lam_p, x_lam_p_sx = cs.MX.sym("in", *x_lam_p.shape), x_lam_p
-            Kt, Ky = cs.Function("sx2mx", (x_lam_p_sx,), (Kt, Ky))(x_lam_p)
-        solver = (
-            cs.solve  # cs.mldivide
-            if linsolver == "mldivide"
-            else cs.Linsol("linsolver", linsolver, Ky.sparsity()).solve
-        )
-
-        # compute sensitivity and convert to function (faster runtime)
-        dpidtheta = -solver(Ky, Kt).T @ dydu0
-        sensitivity = cs.Function(
-            "dpidtheta",
-            (x_lam_p,),
-            (dpidtheta,),
-            ("x_lam_p",),
-            ("dpidtheta",),
-            {"cse": True},
-        )
-        ntheta, na = dpidtheta.shape
-
-        # wrap to conveniently return arrays. Casadi does not support tensors with
-        # >2 dims, so dpidtheta gets squished in the 3rd dim and needs reshaping
-        def func(sol_values: cs.DM, N: int) -> np.ndarray:
-            return (
-                np.ascontiguousarray(sensitivity(sol_values.T).elements())
-                .reshape(ntheta, na, N, order="F")
-                .transpose((2, 0, 1))
-            )
-
-        return func
-
-    def _consolidate_rollout_into_memory(self) -> None:
-        """Internal utility to compact current rollout into a single item in memory."""
-        # convert rollout to arrays and clear it
-        N, S, E, L, vals = _consolidate_rollout(self._rollout, self._V.ns, self._V.na)
-        self._rollout.clear()
-
-        # compute Phi, dpidtheta, Psi, and CAFA weight v
-        Phi = np.ascontiguousarray(self._Phi(S.T).elements()).reshape(N + 1, -1)
-        dpidtheta = self._sensitivity(vals, N)
-        Psi = (dpidtheta @ E).reshape(N, dpidtheta.shape[1])
-        R = self.ridge_regression_regularization
-        v = _compute_cafa_weight_v(Phi, L, self.discount_factor, R)
-
-        # save to experience
-        self.store_experience((L, Phi, Psi, dpidtheta, v))
-        if self.policy_performances is not None:
-            self.policy_performances.append(L.sum())
-
-
-@nb.njit(cache=True, nogil=True, parallel=True)
-def _consolidate_rollout(
-    rollout: list[tuple[ObsType, ActType, float, ObsType, np.ndarray]],
-    ns: int,
-    na: int,
-) -> tuple[int, np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
-    """Internal utility to convert a rollout list to arrays."""
-    N = len(rollout)
-    S = np.empty((N + 1, ns))
-    E = np.empty((N, na, 1))  # additional dim required for Psi
-    L = np.empty(N)
-    sol_vals = np.empty((N, rollout[0][-1].size))
-    for i in nb.prange(N):
-        s, e, cost, _, sol_val = rollout[i]
-        S[i] = s.reshape(-1)
-        E[i] = e
-        L[i] = cost
-        sol_vals[i] = sol_val
-    S[-1] = rollout[-1][3].reshape(-1)
-    return N, S, E, L, sol_vals
-
-
-@nb.njit(cache=True, nogil=True)
-def _compute_cafa_weight_v(
-    Phi_all: np.ndarray, L: np.ndarray, discount_factor: float, regularization: float
-) -> np.ndarray:
-    """Compute the CAFA weight v via ridge regression."""
-    # solve for v via ridge regression: -phi'(gamma phi+ - phi) v = phi'L
-    Phi = Phi_all[:-1]
-    Phi_next = Phi_all[1:]
-    Phi_diff = discount_factor * Phi_next - Phi
-    M = Phi_diff.T @ Phi @ Phi.T
-    R = regularization * np.eye(M.shape[0])
-    return np.linalg.solve(M @ Phi_diff + R, -M @ L)
-
-
-@nb.njit(cache=True, nogil=True)
-def _compute_cafa_weight_w(
-    Phi_all: np.ndarray,
-    Psi: np.ndarray,
-    L: np.ndarray,
-    v: np.ndarray,
-    discount_factor: float,
-    regularization: float,
-) -> np.ndarray:
-    """Compute the CAFA weight w via ridge regression."""
-    # solve for w via ridge regression: psi' psi w = psi' (L + (gamma phi+ - phi) v)
-    Phi = Phi_all[:-1]
-    Phi_next = Phi_all[1:]
-    Phi_diff = discount_factor * Phi_next - Phi
-    A = Psi.T @ Psi
-    b = Psi.T @ (L + Phi_diff @ v)
-    R = regularization * np.eye(A.shape[0])
-    return np.linalg.solve(A.T @ A + R, A.T @ b)
-
-
-def _estimate_gradient_update(
-    sample: Iterator[ExpType], discount_factor: float, regularization: float
-) -> np.ndarray:
-    """Internal utility to estimate the gradient of the policy."""
-    # compute average v and w
-    sample_ = list(sample)  # load whole iterator into a list
-    v = np.mean([o[4] for o in sample_], 0)
-    w_list = [
-        _compute_cafa_weight_w(Phi, Psi, L, v, discount_factor, regularization)
-        for L, Phi, Psi, _, _ in sample_
-    ]
-    w = np.mean(w_list, 0)
-
-    # compute policy gradient estimate
-    dJdtheta_list = [(o[3] @ o[3].transpose((0, 2, 1))).sum(0) @ w for o in sample_]
-    return np.mean(dJdtheta_list, 0)
+from collections.abc import Collection, Iterator
+from typing import Callable, Generic, Literal, Optional, SupportsFloat, Union
+
+import casadi as cs
+import numba as nb
+import numpy as np
+import numpy.typing as npt
+from csnlp.wrappers import Mpc, NlpSensitivity
+from gymnasium import Env
+from typing_extensions import TypeAlias
+
+from ..core.experience import ExperienceReplay
+from ..core.exploration import ExplorationStrategy
+from ..core.parameters import LearnableParametersDict
+from ..core.update import UpdateStrategy
+from ..core.warmstart import WarmStartStrategy
+from ..optim.gradient_based_optimizer import GradientBasedOptimizer
+from ..util.math import monomials_basis_function
+from .common.agent import ActType, ObsType, SymType
+from .common.rl_learning_agent import LrType, RlLearningAgent
+
+ExpType: TypeAlias = tuple[
+    npt.NDArray[np.floating],  # rollout's costs
+    npt.NDArray[np.floating],  # rollout's state feature vectors Phi(s)
+    npt.NDArray[np.floating],  # rollout's Psi(s,a)
+    npt.NDArray[np.floating],  # rollout's gradient of policy w.r.t. theta
+    npt.NDArray[np.floating],  # rollout's CAFA weight v
+]
+
+
+class LstdDpgAgent(RlLearningAgent[SymType, ExpType, LrType], Generic[SymType, LrType]):
+    """Least-Squares Temporal Difference (LSTD) Deterministic Policy Gradient (DPG)
+    agent, as first introduced in [1] as its stochastic counterpart, and then refined in
+    [2]. An application can be found in [3].
+
+    The DPG agent uses an MPC controller as policy provider and function approximation,
+    and adjusts its parametrization according to the temporal-difference error, with the
+    goal of improving the policy, in a direct fashion by estimating the gradient of the
+    policy and descending in its direction.
+
+    References
+    ----------
+    [1] Gros, S. and Zanon, M., 2021, May. Reinforcement Learning based on MPC
+        and the Stochastic Policy Gradient Method. In 2021 American Control
+        Conference (ACC) (pp. 1947-1952). IEEE.
+    [2] Gros, S. and Zanon, M., 2019. Towards Safe Reinforcement Learning Using NMPC and
+        Policy Gradients: Part II - Deterministic Case. arXiv preprint arXiv:1906.04034.
+    [3] Cai, W., Kordabad, A.B., Esfahani, H.N., Lekkas, A.M. and Gros, S., 2021,
+        December. MPC-based reinforcement learning for a simplified freight mission of
+        autonomous surface vehicles. In 2021 60th IEEE Conference on Decision and
+        Control (CDC) (pp. 2990-2995). IEEE.
+    """
+
+    def __init__(
+        self,
+        mpc: Mpc[SymType],
+        update_strategy: Union[int, UpdateStrategy],
+        discount_factor: float,
+        optimizer: GradientBasedOptimizer,
+        learnable_parameters: LearnableParametersDict[SymType],
+        fixed_parameters: Union[
+            None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]
+        ] = None,
+        exploration: Optional[ExplorationStrategy] = None,
+        experience: Union[None, int, ExperienceReplay[ExpType]] = None,
+        warmstart: Union[
+            Literal["last", "last-successful"], WarmStartStrategy
+        ] = "last-successful",
+        rollout_length: Optional[int] = None,
+        record_policy_performance: bool = False,
+        record_policy_gradient: bool = False,
+        state_features: Optional[cs.Function] = None,
+        linsolver: Literal["csparse", "mldivide"] = "csparse",
+        ridge_regression_regularization: float = 1e-6,
+        use_last_action_on_fail: bool = False,
+        name: Optional[str] = None,
+    ) -> None:
+        """Instantiates the LSTD DPG agent.
+
+        Parameters
+        ----------
+        mpc : Mpc[casadi.SX or MX]
+            The MPC controller used as policy provider by this agent. The instance is
+            modified in place to create the approximations of the state function `V(s)`
+            and action value function `Q(s,a)`, so it is recommended not to modify it
+            further after initialization of the agent. Moreover, some parameter and
+            constraint names will need to be created, so an error is thrown if these
+            names are already in use in the mpc. These names are under the attributes
+            `perturbation_parameter`, `action_parameter` and `action_constraint`.
+        update_strategy : UpdateStrategy or int
+            The strategy used to decide which frequency to update the mpc parameters
+            with. If an `int` is passed, then the default strategy that updates every
+            `n` episodes is used (where `n` is the argument passed); otherwise, an
+            instance of `UpdateStrategy` can be passed to specify these in more details.
+        discount_factor : float
+            In RL, the factor that discounts future rewards in favor of immediate
+            rewards. Usually denoted as `\\gamma`. Should be a number in (0, 1).
+        optimizer : GradientBasedOptimizer
+            A gradient-based optimizer (e.g., `mpcrl.optim.GradientDescent`) to compute
+            the updates of the learnable parameters, based on the current gradient-based
+            RL algorithm.
+        learnable_parameters : LearnableParametersDict
+            A special dict containing the learnable parameters of the MPC, together with
+            their bounds and values. This dict is complementary with `fixed_parameters`,
+            which contains the MPC parameters that are not learnt by the agent.
+        fixed_parameters : dict[str, array_like] or collection of, optional
+            A dict (or collection of dict, in case of `csnlp.MultistartNlp`) whose keys
+            are the names of the MPC parameters and the values are their corresponding
+            values. Use this to specify fixed parameters, that is, non-learnable. If
+            `None`, then no fixed parameter is assumed.
+        exploration : ExplorationStrategy, optional
+            Exploration strategy for inducing exploration in the MPC policy. By default
+            `None`, in which case `NoExploration` is used in the fixed-MPC agent.
+        experience : int or ExperienceReplay, optional
+            The container for experience replay memory. If `None` is passed, then a
+            memory with length 1 is created, i.e., it keeps only the latest memory
+            transition. If an integer `n` is passed, then a memory with the length `n`
+            is created and with sample size `n`.
+            In case of LSTD DPG, each memory item is obtain from a single rollout, and
+            is a 4-tuple that contains: costs, state vector features (Phi), Psi (a
+            temporary value), and the gradient of the policy.
+        max_percentage_update : float, optional
+            A positive float that specifies the maximum percentage the parameters can be
+            changed during each update. For example, `max_percentage_update=0.5` means
+            that the parameters can be updated by up to 50% of their current value. By
+            default, it is set to `+inf`.
+        weight_decay : float, optional
+            A positive float that specifies the decay of the learnable parameters in the
+            form of an L2 regularization term. By default, it is set to `0.0`, so no
+            decay/regularization takes place.
+        warmstart: "last" or "last-successful" or WarmStartStrategy, optional
+            The warmstart strategy for the MPC's NLP. If `last-successful`, the last
+            successful solution is used to warm start the solver for the next iteration.
+            If `last`, the last solution is used, regardless of success or failure.
+            Furthermoer, a `WarmStartStrategy` object can be passed to specify a
+            strategy for generating multiple warmstart points for the NLP. This is
+            useful to generate multiple initial conditions for very non-convex problems.
+            Can only be used with an MPC that has an underlying multistart NLP problem
+            (see `csnlp.MultistartNlp`).
+        rollout_length : int, optional
+            Time-step length of a closed-loop simulation, which defines a complete
+            trajectory of the states, and is saved in the experience as a single item
+            (since LSTD DPG needs to draw samples of trajectories). In case the env is
+            episodic, it can be `None`, in which case the rollout length coincides with
+            the episode's. In case the env is not episodic, i.e., it never terminates, a
+            rollout length must be given in order to save the current trajectory as an
+            atomic item in memory.
+        record_policy_performance: bool, optional
+            If `True`, the performance of each rollout is stored in the field
+            `policy_performances`, which otherwise is `None`. By default, does not
+            record them.
+        record_policy_gradient: bool, optional
+            If `True`, the (estimated) policy gradient of each update is stored in the
+            field `policy_gradients`, which otherwise is `None`. By default, does not
+            record them.
+        state_features : casadi.Function, optional
+            The state feature vector to be used in the linear approximation of the
+            value function, which takes the form of
+            ```
+            V_v(s) = Phi(s)^T * v
+            ```
+            where `s` is the state, `v` are the weights, and `Phi(s)` is the state
+            feature vector. This function is assumed to have one input and one output.
+            By default, if not provided, it is designed as all monomials of the state
+            with degrees <= 2 (see `mpcrl.util.math.monomials_basis_function`).
+        linsolver : "csparse" or "mldivide", optional
+            The type of linear solver to be used for solving the linear system derived
+            from the KKT conditions and used to estimate the gradient of the policy. By
+            default, `"csparse"` is chosen as the KKT matrix is most often sparse.
+        ridge_regression_regularization : float, optional
+            Ridge regression regularization used during the computations of the LSTD
+            weights via least-squares. By default, `1e-6`.
+        use_last_action_on_fail : bool, optional
+            In case the MPC solver fails
+             * if `False`, the action from the last solver's iteration is returned
+               anyway (though suboptimal)
+             * if `True`, the action from the last successful call to the MPC is
+               returned instead (if the MPC has been solved at least once successfully).
+
+            By default, `False`.
+        name : str, optional
+            Name of the agent. If `None`, one is automatically created from a counter of
+            the class' instancies.
+        """
+        # change default update hook to 'on_episode_end'
+        if not isinstance(update_strategy, UpdateStrategy):
+            update_strategy = UpdateStrategy(update_strategy, "on_episode_end")
+        super().__init__(
+            mpc=mpc,
+            update_strategy=update_strategy,
+            discount_factor=discount_factor,
+            optimizer=optimizer,
+            learnable_parameters=learnable_parameters,
+            fixed_parameters=fixed_parameters,
+            exploration=exploration,
+            experience=experience,
+            warmstart=warmstart,
+            use_last_action_on_fail=use_last_action_on_fail,
+            name=name,
+        )
+        self._sensitivity = self._init_sensitivity(linsolver)
+        self._Phi = (
+            monomials_basis_function(mpc.ns, 0, 2)
+            if state_features is None
+            else state_features
+        )
+        self.ridge_regression_regularization = ridge_regression_regularization
+        self.rollout_length = rollout_length or float("+inf")
+        self._rollout: list[
+            tuple[
+                ObsType,
+                ActType,
+                SupportsFloat,
+                ObsType,
+                npt.NDArray[np.floating],
+            ]
+        ] = nb.typed.List()
+        self.policy_performances: Optional[list[float]] = (
+            [] if record_policy_performance else None
+        )
+        self.policy_gradients: Optional[list[npt.NDArray[np.floating]]] = (
+            [] if record_policy_gradient else None
+        )
+
+    def update(self) -> Optional[str]:
+        sample = self.experience.sample()
+        dJdtheta = _estimate_gradient_update(
+            sample, self.discount_factor, self.ridge_regression_regularization
+        )
+        if self.policy_gradients is not None:
+            self.policy_gradients.append(dJdtheta)
+        return self.optimizer.update(dJdtheta)
+
+    def train_one_episode(
+        self,
+        env: Env[ObsType, ActType],
+        episode: int,
+        init_state: ObsType,
+        raises: bool = True,
+    ) -> float:
+        truncated = terminated = False
+        timestep = 0
+        rewards = 0.0
+        state = init_state
+
+        while not (truncated or terminated):
+            # compute V(s) (perturbed and not perturbed)
+            action, sol = self.state_value(state, False)
+            action_opt, sol_opt = self.state_value(state, True)
+
+            # step the system with the action just computed
+            state_new, cost, truncated, terminated, _ = env.step(action)
+            self.on_env_step(env, episode, timestep)
+
+            # store transition in experience
+            if sol.success and sol_opt.success:
+                # NOTE: according to Cai et al. [3], the sensitivities should naively be
+                # computed with the solution of unpertubed MPC (i.e., sol_opt).
+                # According to Gros and Zanon [2], it is hinted that the perturbed
+                # solution should be used instead (sol).
+                exploration = np.asarray((action - action_opt).elements())
+                sol_vals = np.asarray(sol_opt.all_vals.elements())
+                self._rollout.append((state, exploration, cost, state_new, sol_vals))
+            else:
+                status = f"{sol.status}/{sol_opt.status}"
+                self.on_mpc_failure(episode, timestep, status, raises)
+
+            # increase counters
+            state = state_new
+            rewards += float(cost)
+            timestep += 1
+
+            # first, check if current rollout has reached its length, and only then
+            # invoke on_timestep_end (as it might trigger an update)
+            if len(self._rollout) >= self.rollout_length:
+                self._consolidate_rollout_into_memory()
+            self.on_timestep_end(env, episode, timestep)
+
+        # consolidate rollout at the end of episode, if no length was specified
+        if self.rollout_length == float("+inf"):
+            self._consolidate_rollout_into_memory()
+        return rewards
+
+    def _init_sensitivity(self, linsolver: str) -> Callable[[cs.DM, int], np.ndarray]:
+        """Internal utility to compute the derivatives w.r.t. the learnable parameters
+        and other functions in order to estimate the policy gradient."""
+        assert self.optimizer._order == 1, "Expected 1st-order optimizer."
+        nlp = self._V.nlp
+        y = nlp.primal_dual
+        theta = cs.vvcat(self._learnable_pars.sym.values())
+        u0 = cs.vcat(self._V.first_actions.values())
+        x_lam_p = cs.vertcat(nlp.primal_dual, nlp.p)
+
+        # compute first bunch of derivatives
+        nlp_ = NlpSensitivity(nlp, theta)
+        Kt = nlp_.jacobians["K-p"]
+        Ky = nlp_.jacobians["K-y"]
+        dydu0 = cs.jacobian_sparsity(u0, y).T
+
+        # instantiate linear solver (must be MX, so SX has to be converted)
+        if nlp.sym_type is cs.SX:
+            x_lam_p, x_lam_p_sx = cs.MX.sym("in", *x_lam_p.shape), x_lam_p
+            Kt, Ky = cs.Function("sx2mx", (x_lam_p_sx,), (Kt, Ky))(x_lam_p)
+        solver = (
+            cs.solve  # cs.mldivide
+            if linsolver == "mldivide"
+            else cs.Linsol("linsolver", linsolver, Ky.sparsity()).solve
+        )
+
+        # compute sensitivity and convert to function (faster runtime)
+        dpidtheta = -solver(Ky, Kt).T @ dydu0
+        sensitivity = cs.Function(
+            "dpidtheta",
+            (x_lam_p,),
+            (dpidtheta,),
+            ("x_lam_p",),
+            ("dpidtheta",),
+            {"cse": True},
+        )
+        ntheta, na = dpidtheta.shape
+
+        # wrap to conveniently return arrays. Casadi does not support tensors with
+        # >2 dims, so dpidtheta gets squished in the 3rd dim and needs reshaping
+        def func(sol_values: cs.DM, N: int) -> np.ndarray:
+            return (
+                np.ascontiguousarray(sensitivity(sol_values.T).elements())
+                .reshape(ntheta, na, N, order="F")
+                .transpose((2, 0, 1))
+            )
+
+        return func
+
+    def _consolidate_rollout_into_memory(self) -> None:
+        """Internal utility to compact current rollout into a single item in memory."""
+        # convert rollout to arrays and clear it
+        N, S, E, L, vals = _consolidate_rollout(self._rollout, self._V.ns, self._V.na)
+        self._rollout.clear()
+
+        # compute Phi, dpidtheta, Psi, and CAFA weight v
+        Phi = np.ascontiguousarray(self._Phi(S.T).elements()).reshape(N + 1, -1)
+        dpidtheta = self._sensitivity(vals, N)
+        Psi = (dpidtheta @ E).reshape(N, dpidtheta.shape[1])
+        R = self.ridge_regression_regularization
+        v = _compute_cafa_weight_v(Phi, L, self.discount_factor, R)
+
+        # save to experience
+        self.store_experience((L, Phi, Psi, dpidtheta, v))
+        if self.policy_performances is not None:
+            self.policy_performances.append(L.sum())
+
+
+@nb.njit(cache=True, nogil=True, parallel=True)
+def _consolidate_rollout(
+    rollout: list[tuple[ObsType, ActType, float, ObsType, np.ndarray]],
+    ns: int,
+    na: int,
+) -> tuple[int, np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
+    """Internal utility to convert a rollout list to arrays."""
+    N = len(rollout)
+    S = np.empty((N + 1, ns))
+    E = np.empty((N, na, 1))  # additional dim required for Psi
+    L = np.empty(N)
+    sol_vals = np.empty((N, rollout[0][-1].size))
+    for i in nb.prange(N):
+        s, e, cost, _, sol_val = rollout[i]
+        S[i] = s.reshape(-1)
+        E[i] = e
+        L[i] = cost
+        sol_vals[i] = sol_val
+    S[-1] = rollout[-1][3].reshape(-1)
+    return N, S, E, L, sol_vals
+
+
+@nb.njit(cache=True, nogil=True)
+def _compute_cafa_weight_v(
+    Phi_all: np.ndarray, L: np.ndarray, discount_factor: float, regularization: float
+) -> np.ndarray:
+    """Compute the CAFA weight v via ridge regression."""
+    # solve for v via ridge regression: -phi'(gamma phi+ - phi) v = phi'L
+    Phi = Phi_all[:-1]
+    Phi_next = Phi_all[1:]
+    Phi_diff = discount_factor * Phi_next - Phi
+    M = Phi_diff.T @ Phi @ Phi.T
+    R = regularization * np.eye(M.shape[0])
+    return np.linalg.solve(M @ Phi_diff + R, -M @ L)
+
+
+@nb.njit(cache=True, nogil=True)
+def _compute_cafa_weight_w(
+    Phi_all: np.ndarray,
+    Psi: np.ndarray,
+    L: np.ndarray,
+    v: np.ndarray,
+    discount_factor: float,
+    regularization: float,
+) -> np.ndarray:
+    """Compute the CAFA weight w via ridge regression."""
+    # solve for w via ridge regression: psi' psi w = psi' (L + (gamma phi+ - phi) v)
+    Phi = Phi_all[:-1]
+    Phi_next = Phi_all[1:]
+    Phi_diff = discount_factor * Phi_next - Phi
+    A = Psi.T @ Psi
+    b = Psi.T @ (L + Phi_diff @ v)
+    R = regularization * np.eye(A.shape[0])
+    return np.linalg.solve(A.T @ A + R, A.T @ b)
+
+
+def _estimate_gradient_update(
+    sample: Iterator[ExpType], discount_factor: float, regularization: float
+) -> np.ndarray:
+    """Internal utility to estimate the gradient of the policy."""
+    # compute average v and w
+    sample_ = list(sample)  # load whole iterator into a list
+    v = np.mean([o[4] for o in sample_], 0)
+    w_list = [
+        _compute_cafa_weight_w(Phi, Psi, L, v, discount_factor, regularization)
+        for L, Phi, Psi, _, _ in sample_
+    ]
+    w = np.mean(w_list, 0)
+
+    # compute policy gradient estimate
+    dJdtheta_list = [(o[3] @ o[3].transpose((0, 2, 1))).sum(0) @ w for o in sample_]
+    return np.mean(dJdtheta_list, 0)
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/agents/lstd_q_learning.py` & `mpcrl-1.2.0rc4/src/mpcrl/agents/lstd_q_learning.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,305 +1,317 @@
-from collections.abc import Collection, Iterable
-from typing import Callable, Generic, Literal, Optional, SupportsFloat, Union
-
-import casadi as cs
-import numpy as np
-import numpy.typing as npt
-from csnlp import Solution
-from csnlp.wrappers import Mpc, NlpSensitivity
-from gymnasium import Env
-from typing_extensions import TypeAlias
-
-from ..core.experience import ExperienceReplay
-from ..core.exploration import ExplorationStrategy
-from ..core.parameters import LearnableParametersDict
-from ..core.update import UpdateStrategy
-from ..optim.gradient_based_optimizer import GradientBasedOptimizer
-from .common.agent import ActType, ObsType, SymType
-from .common.rl_learning_agent import LrType, RlLearningAgent
-
-ExpType: TypeAlias = tuple[
-    npt.NDArray[np.floating],  # gradient of Bellman residuals w.r.t. theta
-    npt.NDArray[np.floating],  # (approximate) hessian of Bellman residuals w.r.t. theta
-]
-
-
-class LstdQLearningAgent(
-    RlLearningAgent[SymType, ExpType, LrType], Generic[SymType, LrType]
-):
-    """Second-order Least-Squares Temporal Difference (LSTD) Q-learning agent, as first
-    proposed in a simpler format in [1], and then in [2].
-
-    The Q-learning agent uses an MPC controller as policy provider and function
-    approximation, and adjusts its parametrization according to the temporal-difference
-    error, with the goal of improving the policy, in an indirect fashion by learning the
-    action value function.
-
-    References
-    ----------
-    [1] Gros, S. and Zanon, M., 2019. Data-driven economic NMPC using reinforcement
-        learning. IEEE Transactions on Automatic Control, 65(2), pp. 636-648.
-    [2] Esfahani, H.N., Kordabad, A.B. and Gros, S., 2021, June. Approximate Robust NMPC
-        using Reinforcement Learning. In 2021 European Control Conference (ECC), pp.
-        132-137. IEEE.
-    """
-
-    def __init__(
-        self,
-        mpc: Mpc[SymType],
-        update_strategy: Union[int, UpdateStrategy],
-        discount_factor: float,
-        optimizer: GradientBasedOptimizer,
-        learnable_parameters: LearnableParametersDict[SymType],
-        fixed_parameters: Union[
-            None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]
-        ] = None,
-        exploration: Optional[ExplorationStrategy] = None,
-        experience: Union[None, int, ExperienceReplay[ExpType]] = None,
-        warmstart: Literal["last", "last-successful"] = "last-successful",
-        hessian_type: Literal["none", "approx", "full"] = "approx",
-        record_td_errors: bool = False,
-        use_last_action_on_fail: bool = False,
-        remove_bounds_on_initial_action: bool = False,
-        name: Optional[str] = None,
-    ) -> None:
-        """Instantiates the LSTD Q-learning agent.
-
-        Parameters
-        ----------
-        mpc : Mpc[casadi.SX or MX]
-            The MPC controller used as policy provider by this agent. The instance is
-            modified in place to create the approximations of the state function `V(s)`
-            and action value function `Q(s,a)`, so it is recommended not to modify it
-            further after initialization of the agent. Moreover, some parameter and
-            constraint names will need to be created, so an error is thrown if these
-            names are already in use in the mpc. These names are under the attributes
-            `perturbation_parameter`, `action_parameter` and `action_constraint`.
-        update_strategy : UpdateStrategy or int
-            The strategy used to decide which frequency to update the mpc parameters
-            with. If an `int` is passed, then the default strategy that updates every
-            `n` env's steps is used (where `n` is the argument passed); otherwise, an
-            instance of `UpdateStrategy` can be passed to specify these in more details.
-        discount_factor : float
-            In RL, the factor that discounts future rewards in favor of immediate
-            rewards. Usually denoted as `\\gamma`. Should be a number in (0, 1].
-        optimizer : GradientBasedOptimizer
-            A gradient-based optimizer (e.g., `mpcrl.optim.GradientDescent`) to compute
-            the updates of the learnable parameters, based on the current gradient-based
-            RL algorithm.
-        learnable_parameters : LearnableParametersDict
-            A special dict containing the learnable parameters of the MPC, together with
-            their bounds and values. This dict is complementary with `fixed_parameters`,
-            which contains the MPC parameters that are not learnt by the agent.
-        fixed_parameters : dict[str, array_like] or collection of, optional
-            A dict (or collection of dict, in case of `csnlp.MultistartNlp`) whose keys
-            are the names of the MPC parameters and the values are their corresponding
-            values. Use this to specify fixed parameters, that is, non-learnable. If
-            `None`, then no fixed parameter is assumed.
-        exploration : ExplorationStrategy, optional
-            Exploration strategy for inducing exploration in the MPC policy. By default
-            `None`, in which case `NoExploration` is used in the fixed-MPC agent.
-        experience : int or ExperienceReplay, optional
-            The container for experience replay memory. If `None` is passed, then a
-            memory with length 1 is created, i.e., it keeps only the latest memory
-            transition.  If an integer `n` is passed, then a memory with the length `n`
-            is created and with sample size `n`.
-            In the case of LSTD Q-learning, each memory item consists of the action
-            value function's gradient and hessian computed at each (succesful) env's
-            step.
-        warmstart: 'last' or 'last-successful', optional
-            The warmstart strategy for the MPC's NLP. If 'last-successful', the last
-            successful solution is used to warm start the solver for the next iteration.
-            If 'last', the last solution is used, regardless of success or failure.
-        hessian_type : 'none', 'approx' or 'full', optional
-            The type of hessian to use in this (potentially) second-order algorithm.
-            If 'none', no second order information is used. If `approx`, an easier
-            approximation of it is used; otherwise, the full hessian is computed but
-            this is much more expensive. This option must be in accordance with the
-            choice of `optimizer`, that is, if the optimizer does not use second order
-            information, then this option must be set to `none`.
-        record_td_errors: bool, optional
-            If `True`, the TD errors are recorded in the field `td_errors`, which
-            otherwise is `None`. By default, does not record them.
-        use_last_action_on_fail : bool, optional
-            When `True`, if the MPC solver fails in solving the state value function
-            `V(s)`, the last successful action is returned. When `False`, the action
-            from the last MPC iteration is returned instead. By default, `False`.
-        remove_bounds_on_initial_action : bool, optional
-            When `True`, the upper and lower bounds on the initial action are removed in
-            the action-value function approximator Q(s,a) since the first action is
-            constrained to be equal to the initial action. This is useful to avoid
-            issues in the LICQ of the NLP. However, it can lead to numerical problems.
-            By default, `False`.
-        name : str, optional
-            Name of the agent. If `None`, one is automatically created from a counter of
-            the class' instancies.
-        """
-        super().__init__(
-            mpc=mpc,
-            update_strategy=update_strategy,
-            discount_factor=discount_factor,
-            learnable_parameters=learnable_parameters,
-            optimizer=optimizer,
-            fixed_parameters=fixed_parameters,
-            exploration=exploration,
-            experience=experience,
-            warmstart=warmstart,
-            use_last_action_on_fail=use_last_action_on_fail,
-            remove_bounds_on_initial_action=remove_bounds_on_initial_action,
-            name=name,
-        )
-        self.hessian_type = hessian_type
-        self._sensitivity = self._init_sensitivity(hessian_type)
-        self.td_errors: Optional[list[float]] = [] if record_td_errors else None
-
-    def update(self) -> Optional[str]:
-        sample = self.experience.sample()
-        gradients = []
-        hessians = []
-        for g, H in sample:
-            gradients.append(g)
-            hessians.append(H)
-        gradient = np.mean(gradients, 0)
-        hessian = np.mean(hessians, 0) if self.hessian_type != "none" else None
-        return self.optimizer.update(gradient, hessian)
-
-    def train_one_episode(
-        self,
-        env: Env[ObsType, ActType],
-        episode: int,
-        init_state: ObsType,
-        raises: bool = True,
-    ) -> float:
-        truncated = terminated = False
-        timestep = 0
-        rewards = 0.0
-        state = init_state
-
-        # solve for the first action
-        action, solV = self.state_value(state, False)
-        if not solV.success:
-            self.on_mpc_failure(episode, None, solV.status, raises)
-
-        while not (truncated or terminated):
-            # compute Q(s,a)
-            solQ = self.action_value(state, action)
-
-            # step the system with action computed at the previous iteration
-            new_state, cost, truncated, terminated, _ = env.step(action)
-            self.on_env_step(env, episode, timestep)
-
-            # compute V(s+) and store transition
-            new_action, solV = self.state_value(new_state, False)
-            if not self._try_store_experience(cost, solQ, solV):
-                self.on_mpc_failure(
-                    episode, timestep, f"{solQ.status} (Q); {solV.status} (V)", raises
-                )
-
-            # increase counters
-            state = new_state
-            action = new_action
-            rewards += float(cost)
-            timestep += 1
-            self.on_timestep_end(env, episode, timestep)
-        return rewards
-
-    def train_one_rollout(
-        self,
-        rollout: Iterable[tuple[ObsType, ActType, float, ObsType]],
-        episode: int,
-        raises: bool = True,
-    ) -> None:
-        # in the case of off-policy q-learning, rollouts are made of
-        # State-Action-Reward-next State (SARS) tuples
-        for timestep, (state, action, cost, new_state) in enumerate(rollout, start=1):
-            # compute Q(s,a)
-            solQ = self.action_value(state, action)
-
-            # compute V(s+) and store transition
-            _, solV = self.state_value(new_state, False)
-            if not self._try_store_experience(cost, solQ, solV):
-                self.on_mpc_failure(
-                    episode, timestep, f"{solQ.status} (Q); {solV.status} (V)", raises
-                )
-            self.on_timestep_end("off-policy", episode, timestep)
-
-    def _init_sensitivity(
-        self, hessian_type: Literal["none", "approx", "full"]
-    ) -> Union[
-        Callable[[cs.DM], np.ndarray], Callable[[cs.DM], tuple[np.ndarray, np.ndarray]]
-    ]:
-        """Internal utility to compute the derivative of Q(s,a) w.r.t. the learnable
-        parameters, a.k.a., theta."""
-        assert hessian_type in ("none", "approx", "full"), "Invalid hessian type."
-        order = self.optimizer._order
-        theta = cs.vvcat(self._learnable_pars.sym.values())
-        nlp = self._Q.nlp
-        x_lam_p = cs.vertcat(nlp.primal_dual, nlp.p)
-
-        # compute first order sensitivity
-        snlp = NlpSensitivity(self._Q.nlp, theta)
-        gradient = snlp.jacobians["L-p"]  # exact gradient, i.e., dQ/dtheta
-
-        if hessian_type == "none":
-            assert order == 1, "Expected 1st-order optimizer with `hessian_type=none`."
-
-            sensitivity = cs.Function(
-                "S", (x_lam_p,), (gradient,), ("x_lam_p",), ("dQ",), {"cse": True}
-            )
-
-            def func(sol_values: cs.DM) -> np.ndarray:
-                return np.asarray(sensitivity(sol_values).elements())
-
-        else:
-            assert (
-                order == 2
-            ), "Expected 2nd-order optimizer with `hessian_type=approx` or `full`."
-
-            # compute second order sensitivity
-            hessian = snlp.hessians["L-pp"]  # approximate hessian
-            if hessian_type == "full":
-                Kp = snlp.jacobians["K-p"]
-                Ky = snlp.jacobians["K-y"]
-                dydtheta = -cs.solve(Ky, Kp)
-                Lpy = cs.jacobian(gradient, nlp.primal_dual)
-                hessian += Lpy @ dydtheta  # not sure if Lpy or Kp.T
-
-            sensitivity = cs.Function(
-                "S",
-                (x_lam_p,),
-                (gradient, hessian),
-                ("x_lam_p",),
-                ("dQ", "ddQ"),
-                {"cse": True},
-            )
-
-            def func(sol_values: cs.DM) -> tuple[np.ndarray, np.ndarray]:
-                dQ, ddQ = sensitivity(sol_values)
-                return np.asarray(dQ.elements()), ddQ.toarray()
-
-        return func
-
-    def _try_store_experience(
-        self, cost: SupportsFloat, solQ: Solution[SymType], solV: Solution[SymType]
-    ) -> bool:
-        """Internal utility that tries to store the gradient and hessian for the current
-        transition in memory, if both V and Q were successful; otherwise, does not store
-        it. Returns whether it was successful or not."""
-        if solQ.success and solV.success:
-            sol_values = solQ.all_vals
-            td_error = cost + self.discount_factor * solV.f - solQ.f
-            if self.hessian_type == "none":
-                dQ = self._sensitivity(sol_values)
-                hessian = np.nan
-            else:
-                dQ, ddQ = self._sensitivity(sol_values)
-                hessian = np.multiply.outer(dQ, dQ) - td_error * ddQ
-            gradient = -td_error * dQ
-            self.store_experience((gradient, hessian))
-            success = True
-        else:
-            td_error = np.nan
-            success = False
-        if self.td_errors is not None:
-            self.td_errors.append(td_error)
-        return success
+from collections.abc import Collection, Iterable
+from typing import Callable, Generic, Literal, Optional, SupportsFloat, Union
+
+import casadi as cs
+import numpy as np
+import numpy.typing as npt
+from csnlp import Solution
+from csnlp.wrappers import Mpc, NlpSensitivity
+from gymnasium import Env
+from typing_extensions import TypeAlias
+
+from ..core.experience import ExperienceReplay
+from ..core.exploration import ExplorationStrategy
+from ..core.parameters import LearnableParametersDict
+from ..core.update import UpdateStrategy
+from ..core.warmstart import WarmStartStrategy
+from ..optim.gradient_based_optimizer import GradientBasedOptimizer
+from .common.agent import ActType, ObsType, SymType
+from .common.rl_learning_agent import LrType, RlLearningAgent
+
+ExpType: TypeAlias = tuple[
+    npt.NDArray[np.floating],  # gradient of Bellman residuals w.r.t. theta
+    npt.NDArray[np.floating],  # (approximate) hessian of Bellman residuals w.r.t. theta
+]
+
+
+class LstdQLearningAgent(
+    RlLearningAgent[SymType, ExpType, LrType], Generic[SymType, LrType]
+):
+    """Second-order Least-Squares Temporal Difference (LSTD) Q-learning agent, as first
+    proposed in a simpler format in [1], and then in [2].
+
+    The Q-learning agent uses an MPC controller as policy provider and function
+    approximation, and adjusts its parametrization according to the temporal-difference
+    error, with the goal of improving the policy, in an indirect fashion by learning the
+    action value function.
+
+    References
+    ----------
+    [1] Gros, S. and Zanon, M., 2019. Data-driven economic NMPC using reinforcement
+        learning. IEEE Transactions on Automatic Control, 65(2), pp. 636-648.
+    [2] Esfahani, H.N., Kordabad, A.B. and Gros, S., 2021, June. Approximate Robust NMPC
+        using Reinforcement Learning. In 2021 European Control Conference (ECC), pp.
+        132-137. IEEE.
+    """
+
+    def __init__(
+        self,
+        mpc: Mpc[SymType],
+        update_strategy: Union[int, UpdateStrategy],
+        discount_factor: float,
+        optimizer: GradientBasedOptimizer,
+        learnable_parameters: LearnableParametersDict[SymType],
+        fixed_parameters: Union[
+            None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]
+        ] = None,
+        exploration: Optional[ExplorationStrategy] = None,
+        experience: Union[None, int, ExperienceReplay[ExpType]] = None,
+        warmstart: Union[
+            Literal["last", "last-successful"], WarmStartStrategy
+        ] = "last-successful",
+        hessian_type: Literal["none", "approx", "full"] = "approx",
+        record_td_errors: bool = False,
+        use_last_action_on_fail: bool = False,
+        remove_bounds_on_initial_action: bool = False,
+        name: Optional[str] = None,
+    ) -> None:
+        """Instantiates the LSTD Q-learning agent.
+
+        Parameters
+        ----------
+        mpc : Mpc[casadi.SX or MX]
+            The MPC controller used as policy provider by this agent. The instance is
+            modified in place to create the approximations of the state function `V(s)`
+            and action value function `Q(s,a)`, so it is recommended not to modify it
+            further after initialization of the agent. Moreover, some parameter and
+            constraint names will need to be created, so an error is thrown if these
+            names are already in use in the mpc. These names are under the attributes
+            `perturbation_parameter`, `action_parameter` and `action_constraint`.
+        update_strategy : UpdateStrategy or int
+            The strategy used to decide which frequency to update the mpc parameters
+            with. If an `int` is passed, then the default strategy that updates every
+            `n` env's steps is used (where `n` is the argument passed); otherwise, an
+            instance of `UpdateStrategy` can be passed to specify these in more details.
+        discount_factor : float
+            In RL, the factor that discounts future rewards in favor of immediate
+            rewards. Usually denoted as `\\gamma`. Should be a number in (0, 1].
+        optimizer : GradientBasedOptimizer
+            A gradient-based optimizer (e.g., `mpcrl.optim.GradientDescent`) to compute
+            the updates of the learnable parameters, based on the current gradient-based
+            RL algorithm.
+        learnable_parameters : LearnableParametersDict
+            A special dict containing the learnable parameters of the MPC, together with
+            their bounds and values. This dict is complementary with `fixed_parameters`,
+            which contains the MPC parameters that are not learnt by the agent.
+        fixed_parameters : dict[str, array_like] or collection of, optional
+            A dict (or collection of dict, in case of `csnlp.MultistartNlp`) whose keys
+            are the names of the MPC parameters and the values are their corresponding
+            values. Use this to specify fixed parameters, that is, non-learnable. If
+            `None`, then no fixed parameter is assumed.
+        exploration : ExplorationStrategy, optional
+            Exploration strategy for inducing exploration in the MPC policy. By default
+            `None`, in which case `NoExploration` is used in the fixed-MPC agent.
+        experience : int or ExperienceReplay, optional
+            The container for experience replay memory. If `None` is passed, then a
+            memory with length 1 is created, i.e., it keeps only the latest memory
+            transition.  If an integer `n` is passed, then a memory with the length `n`
+            is created and with sample size `n`.
+            In the case of LSTD Q-learning, each memory item consists of the action
+            value function's gradient and hessian computed at each (succesful) env's
+            step.
+        warmstart: "last" or "last-successful" or WarmStartStrategy, optional
+            The warmstart strategy for the MPC's NLP. If `last-successful`, the last
+            successful solution is used to warm start the solver for the next iteration.
+            If `last`, the last solution is used, regardless of success or failure.
+            Furthermoer, a `WarmStartStrategy` object can be passed to specify a
+            strategy for generating multiple warmstart points for the NLP. This is
+            useful to generate multiple initial conditions for very non-convex problems.
+            Can only be used with an MPC that has an underlying multistart NLP problem
+            (see `csnlp.MultistartNlp`).
+        hessian_type : 'none', 'approx' or 'full', optional
+            The type of hessian to use in this (potentially) second-order algorithm.
+            If 'none', no second order information is used. If `approx`, an easier
+            approximation of it is used; otherwise, the full hessian is computed but
+            this is much more expensive. This option must be in accordance with the
+            choice of `optimizer`, that is, if the optimizer does not use second order
+            information, then this option must be set to `none`.
+        record_td_errors: bool, optional
+            If `True`, the TD errors are recorded in the field `td_errors`, which
+            otherwise is `None`. By default, does not record them.
+        use_last_action_on_fail : bool, optional
+            In case the MPC solver fails
+             * if `False`, the action from the last solver's iteration is returned
+               anyway (though suboptimal)
+             * if `True`, the action from the last successful call to the MPC is
+               returned instead (if the MPC has been solved at least once successfully).
+
+            By default, `False`.
+        remove_bounds_on_initial_action : bool, optional
+            When `True`, the upper and lower bounds on the initial action are removed in
+            the action-value function approximator Q(s,a) since the first action is
+            constrained to be equal to the initial action. This is useful to avoid
+            issues in the LICQ of the NLP. However, it can lead to numerical problems.
+            By default, `False`.
+        name : str, optional
+            Name of the agent. If `None`, one is automatically created from a counter of
+            the class' instancies.
+        """
+        super().__init__(
+            mpc=mpc,
+            update_strategy=update_strategy,
+            discount_factor=discount_factor,
+            learnable_parameters=learnable_parameters,
+            optimizer=optimizer,
+            fixed_parameters=fixed_parameters,
+            exploration=exploration,
+            experience=experience,
+            warmstart=warmstart,
+            use_last_action_on_fail=use_last_action_on_fail,
+            remove_bounds_on_initial_action=remove_bounds_on_initial_action,
+            name=name,
+        )
+        self.hessian_type = hessian_type
+        self._sensitivity = self._init_sensitivity(hessian_type)
+        self.td_errors: Optional[list[float]] = [] if record_td_errors else None
+
+    def update(self) -> Optional[str]:
+        sample = self.experience.sample()
+        gradients = []
+        hessians = []
+        for g, H in sample:
+            gradients.append(g)
+            hessians.append(H)
+        gradient = np.mean(gradients, 0)
+        hessian = np.mean(hessians, 0) if self.hessian_type != "none" else None
+        return self.optimizer.update(gradient, hessian)
+
+    def train_one_episode(
+        self,
+        env: Env[ObsType, ActType],
+        episode: int,
+        init_state: ObsType,
+        raises: bool = True,
+    ) -> float:
+        truncated = terminated = False
+        timestep = 0
+        rewards = 0.0
+        state = init_state
+
+        # solve for the first action
+        action, solV = self.state_value(state, False)
+        if not solV.success:
+            self.on_mpc_failure(episode, None, solV.status, raises)
+
+        while not (truncated or terminated):
+            # compute Q(s,a)
+            solQ = self.action_value(state, action)
+
+            # step the system with action computed at the previous iteration
+            new_state, cost, truncated, terminated, _ = env.step(action)
+            self.on_env_step(env, episode, timestep)
+
+            # compute V(s+) and store transition
+            new_action, solV = self.state_value(new_state, False)
+            if not self._try_store_experience(cost, solQ, solV):
+                self.on_mpc_failure(
+                    episode, timestep, f"{solQ.status} (Q); {solV.status} (V)", raises
+                )
+
+            # increase counters
+            state = new_state
+            action = new_action
+            rewards += float(cost)
+            timestep += 1
+            self.on_timestep_end(env, episode, timestep)
+        return rewards
+
+    def train_one_rollout(
+        self,
+        rollout: Iterable[tuple[ObsType, ActType, float, ObsType]],
+        episode: int,
+        raises: bool = True,
+    ) -> None:
+        # in the case of off-policy q-learning, rollouts are made of
+        # State-Action-Reward-next State (SARS) tuples
+        for timestep, (state, action, cost, new_state) in enumerate(rollout, start=1):
+            # compute Q(s,a)
+            solQ = self.action_value(state, action)
+
+            # compute V(s+) and store transition
+            _, solV = self.state_value(new_state, False)
+            if not self._try_store_experience(cost, solQ, solV):
+                self.on_mpc_failure(
+                    episode, timestep, f"{solQ.status} (Q); {solV.status} (V)", raises
+                )
+            self.on_timestep_end("off-policy", episode, timestep)
+
+    def _init_sensitivity(
+        self, hessian_type: Literal["none", "approx", "full"]
+    ) -> Union[
+        Callable[[cs.DM], np.ndarray], Callable[[cs.DM], tuple[np.ndarray, np.ndarray]]
+    ]:
+        """Internal utility to compute the derivative of Q(s,a) w.r.t. the learnable
+        parameters, a.k.a., theta."""
+        assert hessian_type in ("none", "approx", "full"), "Invalid hessian type."
+        order = self.optimizer._order
+        theta = cs.vvcat(self._learnable_pars.sym.values())
+        nlp = self._Q.nlp
+        x_lam_p = cs.vertcat(nlp.primal_dual, nlp.p)
+
+        # compute first order sensitivity
+        snlp = NlpSensitivity(self._Q.nlp, theta)
+        gradient = snlp.jacobians["L-p"]  # exact gradient, i.e., dQ/dtheta
+
+        if hessian_type == "none":
+            assert order == 1, "Expected 1st-order optimizer with `hessian_type=none`."
+
+            sensitivity = cs.Function(
+                "S", (x_lam_p,), (gradient,), ("x_lam_p",), ("dQ",), {"cse": True}
+            )
+
+            def func(sol_values: cs.DM) -> np.ndarray:
+                return np.asarray(sensitivity(sol_values).elements())
+
+        else:
+            assert (
+                order == 2
+            ), "Expected 2nd-order optimizer with `hessian_type=approx` or `full`."
+
+            # compute second order sensitivity
+            hessian = snlp.hessians["L-pp"]  # approximate hessian
+            if hessian_type == "full":
+                Kp = snlp.jacobians["K-p"]
+                Ky = snlp.jacobians["K-y"]
+                dydtheta = -cs.solve(Ky, Kp)
+                Lpy = cs.jacobian(gradient, nlp.primal_dual)
+                hessian += Lpy @ dydtheta  # not sure if Lpy or Kp.T
+
+            sensitivity = cs.Function(
+                "S",
+                (x_lam_p,),
+                (gradient, hessian),
+                ("x_lam_p",),
+                ("dQ", "ddQ"),
+                {"cse": True},
+            )
+
+            def func(sol_values: cs.DM) -> tuple[np.ndarray, np.ndarray]:
+                dQ, ddQ = sensitivity(sol_values)
+                return np.asarray(dQ.elements()), ddQ.toarray()
+
+        return func
+
+    def _try_store_experience(
+        self, cost: SupportsFloat, solQ: Solution[SymType], solV: Solution[SymType]
+    ) -> bool:
+        """Internal utility that tries to store the gradient and hessian for the current
+        transition in memory, if both V and Q were successful; otherwise, does not store
+        it. Returns whether it was successful or not."""
+        if solQ.success and solV.success:
+            sol_values = solQ.all_vals
+            td_error = cost + self.discount_factor * solV.f - solQ.f
+            if self.hessian_type == "none":
+                dQ = self._sensitivity(sol_values)
+                hessian = np.nan
+            else:
+                dQ, ddQ = self._sensitivity(sol_values)
+                hessian = np.multiply.outer(dQ, dQ) - td_error * ddQ
+            gradient = -td_error * dQ
+            self.store_experience((gradient, hessian))
+            success = True
+        else:
+            td_error = np.nan
+            success = False
+        if self.td_errors is not None:
+            self.td_errors.append(td_error)
+        return success
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/core/callbacks.py` & `mpcrl-1.2.0rc4/src/mpcrl/core/callbacks.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,273 +1,273 @@
-from typing import Any, Callable, Literal, Optional, TypeVar, Union
-
-import numpy as np
-import numpy.typing as npt
-from gymnasium import Env
-
-from .errors import raise_or_warn_on_mpc_failure, raise_or_warn_on_update_failure
-
-ObsType = TypeVar("ObsType")
-ActType = TypeVar("ActType")
-
-
-def _failure_msg(
-    category: Literal["mpc", "update"],
-    name: str,
-    episode: int,
-    timestep: Optional[int],
-    status: str,
-) -> str:
-    """Internal utility for composing message for mpc/update failure."""
-    C = category.title()
-    if timestep is None:
-        return f"{C} failure of {name} at episode {episode}, status: {status}."
-    else:
-        return (
-            f"{C} failure of {name} at episode {episode}, time {timestep}, "
-            f"status: {status}."
-        )
-
-
-class CallbackMixin:
-    """A class with the particular purpose of creating, storing and deleting hooks.
-    Particularly touchy is when the state is set, and the hooks need to be reestablished
-    automatically. In fact, if the old hooks are used, the new object (created from the
-    state) would reference callbacks belonging to the old agent. In this way, the
-    callbacks are linked to the new instance.
-    """
-
-    def __init__(self) -> None:
-        self._hooks: dict[str, list[tuple[str, Callable[..., None]]]] = {}
-
-    def __setstate__(
-        self,
-        state: Union[
-            None, dict[str, Any], tuple[Optional[dict[str, Any]], dict[str, Any]]
-        ],
-    ) -> None:
-        if isinstance(state, tuple) and len(state) == 2:
-            state, slotstate = state
-        else:
-            slotstate = None
-        if state is not None:
-            # remove hooks (otherwise, new copies will still be calling the old object)
-            state["_hooks"] = {}
-            self.__dict__.update(state)
-        if slotstate is not None:
-            for key, value in slotstate.items():
-                setattr(self, key, value)
-        # re-establish hooks
-        self.establish_callback_hooks()
-
-    def _run_hooks(self, method_name: str, *args: Any) -> None:
-        """Runs the internal hooks attached to the given method."""
-        if hooks := self._hooks.get(method_name):
-            for hook in hooks.values():
-                hook(*args)
-
-    def establish_callback_hooks(self) -> None:
-        """This method must be used to perform the connections between callbacks and any
-        invokable method (hook). If the object has no hooks, then this method does
-        nothing."""
-
-    def hook_callback(
-        self, attachername: str, callbackname: str, func: Callable[..., None]
-    ) -> None:
-        """Hooks a function to be called each time a callback is invoked.
-
-        Parameters
-        ----------
-        attachername : str
-            The name of the object requesting the hook. Has only info purposes.
-        callbackname : str
-            Name of the callback to hook to, i.e., the target of the hooking.
-        func : Callable
-            function to be called when the callback is invoked. Must accept the same
-            input arguments as the callback it is hooked to. Moreover, the return value
-            is discarded.
-
-        Raises
-        ------
-        ValueError
-            If an hook with name `attachername` is already attached to this callback.
-        """
-        hook_dict = self._hooks.setdefault(callbackname, {})
-        if attachername in hook_dict:
-            raise ValueError(
-                f"Hook '{attachername}' already attached to callback '{callbackname}'."
-            )
-        hook_dict[attachername] = func
-
-
-class AgentCallbackMixin(CallbackMixin):
-    """Callbacks for agents."""
-
-    def on_mpc_failure(
-        self, episode: int, timestep: Optional[int], status: str, raises: bool
-    ) -> None:
-        """Callback in case of MPC failure.
-
-        Parameters
-        ----------
-        episode : int
-            Number of the episode when the failure happened.
-        timestep : int or None
-            Timestep of the current episode when the failure happened. Can be `None` in
-            case the error occurs inter-episodically.
-        status : str
-            Status of the solver that failed.
-        raises : bool
-            Whether the failure should be raised as exception.
-        """
-        name: str = getattr(self, "name", "agent")
-        raise_or_warn_on_mpc_failure(
-            _failure_msg("mpc", name, episode, timestep, status),
-            raises,
-        )
-        self._run_hooks("on_mpc_failure", episode, timestep, status, raises)
-
-    def on_validation_start(self, env: Env[ObsType, ActType]) -> None:
-        """Callback called at the beginning of the validation process.
-
-        Parameters
-        ----------
-        env : gym env
-            A gym environment where the agent is being validated on.
-        """
-        self._run_hooks("on_validation_start", env)
-
-    def on_validation_end(
-        self, env: Env[ObsType, ActType], returns: npt.NDArray[np.floating]
-    ) -> None:
-        """Callback called at the end of the validation process.
-
-        Parameters
-        ----------
-        env : gym env
-            A gym environment where the agent has been validated on.
-        returns : array of double
-            Each episode's cumulative rewards.
-        """
-        self._run_hooks("on_validation_end", env, returns)
-
-    def on_episode_start(
-        self, env: Env[ObsType, ActType], episode: int, state: ObsType
-    ) -> None:
-        """Callback called at the beginning of each episode in the training process.
-
-        Parameters
-        ----------
-        env : gym env
-            A gym environment where the agent is being trained on.
-        episode : int
-            Number of the training episode.
-        state : ObsType
-            Starting state for this episode.
-        """
-        self._run_hooks("on_episode_start", env, episode, state)
-
-    def on_episode_end(
-        self, env: Env[ObsType, ActType], episode: int, rewards: float
-    ) -> None:
-        """Callback called at the end of each episode in the training process.
-
-        Parameters
-        ----------
-        env : gym env
-            A gym environment where the agent is being trained on.
-        episode : int
-            Number of the training episode.
-        rewards : float
-            Cumulative rewards for this episode.
-        """
-        self._run_hooks("on_episode_end", env, episode, rewards)
-
-    def on_env_step(
-        self, env: Env[ObsType, ActType], episode: int, timestep: int
-    ) -> None:
-        """Callback called after each `env.step`.
-
-        Parameters
-        ----------
-        env : gym env
-            A gym environment where the agent is being trained on.
-        episode : int
-            Number of the training episode.
-        timestep : int
-            Time instant of the current training episode.
-        """
-        self._run_hooks("on_env_step", env, episode, timestep)
-
-    def on_timestep_end(
-        self, env: Env[ObsType, ActType], episode: int, timestep: int
-    ) -> None:
-        """Callback called at the end of each time iteration. It is called with the same
-        frequency as `env.step`, but with different timing.
-
-        Parameters
-        ----------
-        env : gym env
-            A gym environment where the agent is being trained on.
-        episode : int
-            Number of the training episode.
-        timestep : int
-            Time instant of the current training episode.
-        """
-        self._run_hooks("on_timestep_end", env, episode, timestep)
-
-
-class LearningAgentCallbackMixin(AgentCallbackMixin):
-    """Callbacks for learning agents."""
-
-    def on_update_failure(
-        self, episode: int, timestep: Optional[int], errormsg: str, raises: bool
-    ) -> None:
-        """Callback in case of update failure.
-
-        Parameters
-        ----------
-        episode : int
-            Number of the episode when the failure happened.
-        timestep : int or None
-            Timestep of the current episode when the failure happened. Can be `None` in
-            case the update occurs inter-episodically.
-        errormsg : str
-            Error message of the update failure.
-        raises : bool
-            Whether the failure should be raised as exception.
-        """
-        name: str = getattr(self, "name", "agent")
-        raise_or_warn_on_update_failure(
-            _failure_msg("update", name, episode, timestep, errormsg),
-            raises,
-        )
-        self._run_hooks("on_update_failure", episode, timestep, errormsg, raises)
-
-    def on_training_start(self, env: Env[ObsType, ActType]) -> None:
-        """Callback called at the beginning of the training process.
-
-        Parameters
-        ----------
-        env : gym env
-            A gym environment where the agent is being trained on.
-        """
-        self._run_hooks("on_training_start", env)
-
-    def on_training_end(
-        self, env: Env[ObsType, ActType], returns: npt.NDArray[np.floating]
-    ) -> None:
-        """Callback called at the end of the training process.
-
-        Parameters
-        ----------
-        env : gym env
-            A gym environment where the agent has been trained on.
-        returns : array of double
-            Each episode's cumulative rewards.
-        """
-        self._run_hooks("on_training_end", env, returns)
-
-    def on_update(self) -> None:
-        """Callback called after each `agent.update`. Use this callback for, e.g.,
-        decaying exploration probabilities or learning rates."""
-        self._run_hooks("on_update")
+from typing import Any, Callable, Literal, Optional, TypeVar, Union
+
+import numpy as np
+import numpy.typing as npt
+from gymnasium import Env
+
+from .errors import raise_or_warn_on_mpc_failure, raise_or_warn_on_update_failure
+
+ObsType = TypeVar("ObsType")
+ActType = TypeVar("ActType")
+
+
+def _failure_msg(
+    category: Literal["mpc", "update"],
+    name: str,
+    episode: int,
+    timestep: Optional[int],
+    status: str,
+) -> str:
+    """Internal utility for composing message for mpc/update failure."""
+    C = category.title()
+    if timestep is None:
+        return f"{C} failure of {name} at episode {episode}, status: {status}."
+    else:
+        return (
+            f"{C} failure of {name} at episode {episode}, time {timestep}, "
+            f"status: {status}."
+        )
+
+
+class CallbackMixin:
+    """A class with the particular purpose of creating, storing and deleting hooks.
+    Particularly touchy is when the state is set, and the hooks need to be reestablished
+    automatically. In fact, if the old hooks are used, the new object (created from the
+    state) would reference callbacks belonging to the old agent. In this way, the
+    callbacks are linked to the new instance.
+    """
+
+    def __init__(self) -> None:
+        self._hooks: dict[str, list[tuple[str, Callable[..., None]]]] = {}
+
+    def __setstate__(
+        self,
+        state: Union[
+            None, dict[str, Any], tuple[Optional[dict[str, Any]], dict[str, Any]]
+        ],
+    ) -> None:
+        if isinstance(state, tuple) and len(state) == 2:
+            state, slotstate = state
+        else:
+            slotstate = None
+        if state is not None:
+            # remove hooks (otherwise, new copies will still be calling the old object)
+            state["_hooks"] = {}
+            self.__dict__.update(state)
+        if slotstate is not None:
+            for key, value in slotstate.items():
+                setattr(self, key, value)
+        # re-establish hooks
+        self.establish_callback_hooks()
+
+    def _run_hooks(self, method_name: str, *args: Any) -> None:
+        """Runs the internal hooks attached to the given method."""
+        if hooks := self._hooks.get(method_name):
+            for hook in hooks.values():
+                hook(*args)
+
+    def establish_callback_hooks(self) -> None:
+        """This method must be used to perform the connections between callbacks and any
+        invokable method (hook). If the object has no hooks, then this method does
+        nothing."""
+
+    def hook_callback(
+        self, attachername: str, callbackname: str, func: Callable[..., None]
+    ) -> None:
+        """Hooks a function to be called each time a callback is invoked.
+
+        Parameters
+        ----------
+        attachername : str
+            The name of the object requesting the hook. Has only info purposes.
+        callbackname : str
+            Name of the callback to hook to, i.e., the target of the hooking.
+        func : Callable
+            function to be called when the callback is invoked. Must accept the same
+            input arguments as the callback it is hooked to. Moreover, the return value
+            is discarded.
+
+        Raises
+        ------
+        ValueError
+            If an hook with name `attachername` is already attached to this callback.
+        """
+        hook_dict = self._hooks.setdefault(callbackname, {})
+        if attachername in hook_dict:
+            raise ValueError(
+                f"Hook '{attachername}' already attached to callback '{callbackname}'."
+            )
+        hook_dict[attachername] = func
+
+
+class AgentCallbackMixin(CallbackMixin):
+    """Callbacks for agents."""
+
+    def on_mpc_failure(
+        self, episode: int, timestep: Optional[int], status: str, raises: bool
+    ) -> None:
+        """Callback in case of MPC failure.
+
+        Parameters
+        ----------
+        episode : int
+            Number of the episode when the failure happened.
+        timestep : int or None
+            Timestep of the current episode when the failure happened. Can be `None` in
+            case the error occurs inter-episodically.
+        status : str
+            Status of the solver that failed.
+        raises : bool
+            Whether the failure should be raised as exception.
+        """
+        name: str = getattr(self, "name", "agent")
+        raise_or_warn_on_mpc_failure(
+            _failure_msg("mpc", name, episode, timestep, status),
+            raises,
+        )
+        self._run_hooks("on_mpc_failure", episode, timestep, status, raises)
+
+    def on_validation_start(self, env: Env[ObsType, ActType]) -> None:
+        """Callback called at the beginning of the validation process.
+
+        Parameters
+        ----------
+        env : gym env
+            A gym environment where the agent is being validated on.
+        """
+        self._run_hooks("on_validation_start", env)
+
+    def on_validation_end(
+        self, env: Env[ObsType, ActType], returns: npt.NDArray[np.floating]
+    ) -> None:
+        """Callback called at the end of the validation process.
+
+        Parameters
+        ----------
+        env : gym env
+            A gym environment where the agent has been validated on.
+        returns : array of double
+            Each episode's cumulative rewards.
+        """
+        self._run_hooks("on_validation_end", env, returns)
+
+    def on_episode_start(
+        self, env: Env[ObsType, ActType], episode: int, state: ObsType
+    ) -> None:
+        """Callback called at the beginning of each episode in the training process.
+
+        Parameters
+        ----------
+        env : gym env
+            A gym environment where the agent is being trained on.
+        episode : int
+            Number of the training episode.
+        state : ObsType
+            Starting state for this episode.
+        """
+        self._run_hooks("on_episode_start", env, episode, state)
+
+    def on_episode_end(
+        self, env: Env[ObsType, ActType], episode: int, rewards: float
+    ) -> None:
+        """Callback called at the end of each episode in the training process.
+
+        Parameters
+        ----------
+        env : gym env
+            A gym environment where the agent is being trained on.
+        episode : int
+            Number of the training episode.
+        rewards : float
+            Cumulative rewards for this episode.
+        """
+        self._run_hooks("on_episode_end", env, episode, rewards)
+
+    def on_env_step(
+        self, env: Env[ObsType, ActType], episode: int, timestep: int
+    ) -> None:
+        """Callback called after each `env.step`.
+
+        Parameters
+        ----------
+        env : gym env
+            A gym environment where the agent is being trained on.
+        episode : int
+            Number of the training episode.
+        timestep : int
+            Time instant of the current training episode.
+        """
+        self._run_hooks("on_env_step", env, episode, timestep)
+
+    def on_timestep_end(
+        self, env: Env[ObsType, ActType], episode: int, timestep: int
+    ) -> None:
+        """Callback called at the end of each time iteration. It is called with the same
+        frequency as `env.step`, but with different timing.
+
+        Parameters
+        ----------
+        env : gym env
+            A gym environment where the agent is being trained on.
+        episode : int
+            Number of the training episode.
+        timestep : int
+            Time instant of the current training episode.
+        """
+        self._run_hooks("on_timestep_end", env, episode, timestep)
+
+
+class LearningAgentCallbackMixin(AgentCallbackMixin):
+    """Callbacks for learning agents."""
+
+    def on_update_failure(
+        self, episode: int, timestep: Optional[int], errormsg: str, raises: bool
+    ) -> None:
+        """Callback in case of update failure.
+
+        Parameters
+        ----------
+        episode : int
+            Number of the episode when the failure happened.
+        timestep : int or None
+            Timestep of the current episode when the failure happened. Can be `None` in
+            case the update occurs inter-episodically.
+        errormsg : str
+            Error message of the update failure.
+        raises : bool
+            Whether the failure should be raised as exception.
+        """
+        name: str = getattr(self, "name", "agent")
+        raise_or_warn_on_update_failure(
+            _failure_msg("update", name, episode, timestep, errormsg),
+            raises,
+        )
+        self._run_hooks("on_update_failure", episode, timestep, errormsg, raises)
+
+    def on_training_start(self, env: Env[ObsType, ActType]) -> None:
+        """Callback called at the beginning of the training process.
+
+        Parameters
+        ----------
+        env : gym env
+            A gym environment where the agent is being trained on.
+        """
+        self._run_hooks("on_training_start", env)
+
+    def on_training_end(
+        self, env: Env[ObsType, ActType], returns: npt.NDArray[np.floating]
+    ) -> None:
+        """Callback called at the end of the training process.
+
+        Parameters
+        ----------
+        env : gym env
+            A gym environment where the agent has been trained on.
+        returns : array of double
+            Each episode's cumulative rewards.
+        """
+        self._run_hooks("on_training_end", env, returns)
+
+    def on_update(self) -> None:
+        """Callback called after each `agent.update`. Use this callback for, e.g.,
+        decaying exploration probabilities or learning rates."""
+        self._run_hooks("on_update")
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/core/experience.py` & `mpcrl-1.2.0rc4/src/mpcrl/core/experience.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-from collections.abc import Iterable, Iterator
-from itertools import chain
-from typing import Deque, Optional, TypeVar, Union
-
-import numpy as np
-
-from ..util.seeding import RngType
-
-ExpType = TypeVar("ExpType")
-
-
-class ExperienceReplay(Deque[ExpType]):
-    """Deque-based class for RL traning to save and sample experience transitions. The
-    class inherits from `collections.deque`, adding a couple of simple functionalities
-    to it for sampling transitions at random from past observed data."""
-
-    def __init__(
-        self,
-        iterable: Iterable[ExpType] = (),
-        maxlen: Optional[int] = None,
-        sample_size: Union[int, float] = 1,
-        include_latest: Union[int, float] = 0,
-        seed: RngType = None,
-    ) -> None:
-        """Instantiate the container for experience replay memory.
-
-        Parameters
-        ----------
-        iterable : Iterable of T, optional
-            Initial items to be inserted in the container. By default, empty.
-        maxlen : int, optional
-            Maximum length/capacity of the memory. If `None`, the deque has no maximum
-            size, which is the default behaviour.
-        sample_size : int or float, optional
-            Size (or percentage of replay `maxlen`) of the experience replay items to
-            draw when performing an update. By default, one item per sampling is drawn.
-        include_latest : int or float, optional
-            Size (or percentage of `sample_size`) dedicated to including the latest
-            experience transitions. By default, 0, i.e., no last item is included.
-        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
-            Seed for the random number generator. By default, `None`.
-        """
-        super().__init__(iterable, maxlen=maxlen)
-        self.sample_size = sample_size
-        self.include_latest = include_latest
-        self.reset(seed)
-
-    def reset(self, seed: RngType = None) -> None:
-        """Resets the sampling RNG."""
-        self.np_random = np.random.default_rng(seed)
-
-    def sample(self) -> Iterator[ExpType]:
-        """Samples the experience memory and yields the sampled items.
-
-        Returns
-        -------
-        sample : iterator of T
-            An iterable sample is yielded.
-
-        Raises
-        ------
-        TypeError
-            Raises if `sample_size` is a float (a percentage of the maximum length), but
-            `maxlen` is `None`, since it is impossible to compute the percentage of an
-            unknown quantity.
-        """
-        L = len(self)
-        n = self.sample_size
-        last_n = self.include_latest
-        if isinstance(n, float):
-            assert (
-                self.maxlen is not None
-            ), "Maxlen is `None`; cannot use sample percentages."
-            n = int(self.maxlen * n)
-        n = min(max(n, 0), L)
-        if isinstance(last_n, float):
-            last_n = int(n * last_n)
-        last_n = min(max(last_n, 0), n)
-
-        # get last n indices and the sampled indices from the remaining
-        last = range(L - last_n, L)
-        sampled = self.np_random.choice(range(L - last_n), n - last_n, False)
-        yield from (self[i] for i in chain(sampled, last))
+from collections.abc import Iterable, Iterator
+from itertools import chain
+from typing import Deque, Optional, TypeVar, Union
+
+import numpy as np
+
+from ..util.seeding import RngType
+
+ExpType = TypeVar("ExpType")
+
+
+class ExperienceReplay(Deque[ExpType]):
+    """Deque-based class for RL traning to save and sample experience transitions. The
+    class inherits from `collections.deque`, adding a couple of simple functionalities
+    to it for sampling transitions at random from past observed data."""
+
+    def __init__(
+        self,
+        iterable: Iterable[ExpType] = (),
+        maxlen: Optional[int] = None,
+        sample_size: Union[int, float] = 1,
+        include_latest: Union[int, float] = 0,
+        seed: RngType = None,
+    ) -> None:
+        """Instantiate the container for experience replay memory.
+
+        Parameters
+        ----------
+        iterable : Iterable of T, optional
+            Initial items to be inserted in the container. By default, empty.
+        maxlen : int, optional
+            Maximum length/capacity of the memory. If `None`, the deque has no maximum
+            size, which is the default behaviour.
+        sample_size : int or float, optional
+            Size (or percentage of replay `maxlen`) of the experience replay items to
+            draw when performing an update. By default, one item per sampling is drawn.
+        include_latest : int or float, optional
+            Size (or percentage of `sample_size`) dedicated to including the latest
+            experience transitions. By default, 0, i.e., no last item is included.
+        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
+            Seed for the random number generator. By default, `None`.
+        """
+        super().__init__(iterable, maxlen=maxlen)
+        self.sample_size = sample_size
+        self.include_latest = include_latest
+        self.reset(seed)
+
+    def reset(self, seed: RngType = None) -> None:
+        """Resets the sampling RNG."""
+        self.np_random = np.random.default_rng(seed)
+
+    def sample(self) -> Iterator[ExpType]:
+        """Samples the experience memory and yields the sampled items.
+
+        Returns
+        -------
+        sample : iterator of T
+            An iterable sample is yielded.
+
+        Raises
+        ------
+        TypeError
+            Raises if `sample_size` is a float (a percentage of the maximum length), but
+            `maxlen` is `None`, since it is impossible to compute the percentage of an
+            unknown quantity.
+        """
+        L = len(self)
+        n = self.sample_size
+        last_n = self.include_latest
+        if isinstance(n, float):
+            assert (
+                self.maxlen is not None
+            ), "Maxlen is `None`; cannot use sample percentages."
+            n = int(self.maxlen * n)
+        n = min(max(n, 0), L)
+        if isinstance(last_n, float):
+            last_n = int(n * last_n)
+        last_n = min(max(last_n, 0), n)
+
+        # get last n indices and the sampled indices from the remaining
+        last = range(L - last_n, L)
+        sampled = self.np_random.choice(range(L - last_n), n - last_n, False)
+        yield from (self[i] for i in chain(sampled, last))
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/core/exploration.py` & `mpcrl-1.2.0rc4/src/mpcrl/core/exploration.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,308 +1,308 @@
-from abc import ABC, abstractmethod
-from typing import Any, Literal, Optional, Union
-
-import numpy as np
-import numpy.typing as npt
-
-from ..util.seeding import RngType
-from .schedulers import NoScheduling, Scheduler
-
-
-class ExplorationStrategy(ABC):
-    """Base class for exploration strategies such as greedy, epsilon-greeyd, etc."""
-
-    @abstractmethod
-    def can_explore(self) -> bool:
-        """Computes whether, according to the exploration strategy, the agent should
-        explore or not at the current instant.
-
-        Returns
-        -------
-        bool
-            `True` if the agent should explore according to this strategy; otherwise,
-            `False`.
-        """
-
-    @abstractmethod
-    def step(self, *args: Any, **kwargs: Any) -> None:
-        """Updates the exploration strength and/or probability, in case the strategy
-        supports them (usually, by decaying them over time)."""
-
-    @abstractmethod
-    def perturbation(self, *args: Any, **kwargs: Any) -> npt.NDArray[np.floating]:
-        """Returns a random perturbation."""
-
-    def __str__(self) -> str:
-        return self.__class__.__name__
-
-    def __repr__(self) -> str:
-        hook: Optional[str] = getattr(self, "hook", None)
-        if hook is None:
-            return self.__class__.__name__
-        return f"{self.__class__.__name__}(hook='{hook}')"
-
-
-class NoExploration(ExplorationStrategy):
-    """Strategy where no exploration is allowed at any time or, in other words, the
-    policy is always deterministic (only based on the current state, and not perturbed).
-    """
-
-    def can_explore(self) -> bool:
-        return False
-
-    def step(self, *_, **__) -> None:
-        return
-
-    def perturbation(self, *args: Any, **kwargs: Any) -> npt.NDArray[np.floating]:
-        raise NotImplementedError(
-            f"Perturbation not implemented in {self.__class__.__name__}"
-        )
-
-
-class GreedyExploration(ExplorationStrategy):
-    """Fully greedy strategy for perturbing the policy, thus inducing exploration. This
-    strategy always perturbs randomly the policy."""
-
-    def __init__(
-        self,
-        strength: Union[Scheduler[npt.NDArray[np.floating]], npt.NDArray[np.floating]],
-        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
-        seed: RngType = None,
-    ) -> None:
-        """Initializes the greedy exploration strategy.
-
-        Parameters
-        ----------
-        strength : scheduler or array/supports-algebraic-operations
-            The strength of the exploration. If passed in the form of an
-            `mpcrl.schedulers.Scheduler`, then the strength can be scheduled to
-            decay/increase every time `exploration.step` is called. If an array or
-            something other than a scheduler is passed, then this quantity will get
-            wrapped in a base scheduler which will kept it constant.
-        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
-            Specifies to which callback to hook, i.e., when to step the exploration's
-            schedulers (if any) to, e.g., decay the chances of exploring or the
-            perturbation strength (see `step` method also). The options are:
-             - `on_update` steps the exploration after each agent's update
-             - `on_episode_end` steps the exploration after each episode's end
-             - `on_timestep_end` steps the exploration after each env's timestep.
-
-            By default, 'on_update' is selected.
-        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
-            Number to seed the RNG engine used for randomizing the exploration. By
-            default, `None`.
-        """
-        super().__init__()
-        self._hook = hook
-        if not isinstance(strength, Scheduler):
-            strength = NoScheduling[npt.NDArray[np.floating]](strength)
-        self.strength_scheduler = strength
-        self.reset(seed)
-
-    @property
-    def hook(self) -> Optional[str]:
-        """Specifies to which callback to hook, i.e., when to step the exploration's
-        schedulers (if any) to, e.g., decay the chances of exploring or the perturbation
-        strength (see `step` method also). Can be `None` in case no hook is needed."""
-        # return hook only if the strength scheduler requires to be stepped
-        return None if isinstance(self.strength_scheduler, NoScheduling) else self._hook
-
-    @property
-    def strength(self) -> npt.NDArray[np.floating]:
-        """Gets the current strength of the exploration strategy."""
-        return self.strength_scheduler.value
-
-    def reset(self, seed: RngType = None) -> None:
-        """Resets the exploration RNG."""
-        self.np_random = np.random.default_rng(seed)
-
-    def can_explore(self) -> bool:
-        return True
-
-    def step(self, *_, **__) -> None:
-        """Updates the exploration strength according to its scheduler."""
-        self.strength_scheduler.step()
-
-    def perturbation(
-        self, method: str, *args: Any, **kwargs: Any
-    ) -> npt.NDArray[np.floating]:
-        """Returns a random perturbation.
-
-        Parameters
-        ----------
-        method : str
-            The name of a method from the ones available to `numpy.random.Generator`,
-            e.g., 'random', 'normal', etc.
-        args, kwargs
-            Args and kwargs with which to call such method.
-
-        Returns
-        -------
-        array
-            An array representing the perturbation.
-        """
-        return (
-            getattr(self.np_random, method)(*args, **kwargs)
-            * self.strength_scheduler.value
-        )
-
-    def __repr__(self) -> str:
-        hook = self.hook
-        hookstr = "None" if hook is None else f"'{hook}'"
-        return (
-            f"{self.__class__.__name__}(stn={self.strength_scheduler.value},"
-            f"hook={hookstr})"
-        )
-
-
-class EpsilonGreedyExploration(GreedyExploration):
-    """Epsilon-greedy strategy for perturbing the policy, thus inducing exploration.
-    This strategy only occasionally perturbs randomly the policy."""
-
-    def __init__(
-        self,
-        epsilon: Union[Scheduler[float], float],
-        strength: Union[Scheduler[npt.NDArray[np.floating]], npt.NDArray[np.floating]],
-        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
-        seed: RngType = None,
-    ) -> None:
-        """Initializes the epsilon-greedy exploration strategy.
-
-        Parameters
-        ----------
-        epsilon : scheduler or float
-            The probability to explore. Should be in range [0, 1]. If passed in the form
-            of an `mpcrl.schedulers.Scheduler`, then the probability can be scheduled to
-            decay/increase every time `exploration.step` is called. If an array or
-            something other than a scheduler is passed, then this quantity will get
-            wrapped in a base scheduler which will kept it constant.
-        strength : scheduler or array/supports-algebraic-operations
-            The strength of the exploration. Can be scheduled, see `epsilon`.
-        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
-            Specifies to which callback to hook, i.e., when to step the exploration's
-            schedulers (if any) to, e.g., decay the chances of exploring or the
-            perturbation strength (see `step` method also). The options are:
-             - `on_update` steps the exploration after each agent's update
-             - `on_episode_end` steps the exploration after each episode's end
-             - `on_timestep_end` steps the exploration after each env's timestep.
-
-            By default, 'on_update' is selected.
-        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
-            Number to seed the RNG engine used for randomizing the exploration. By
-            default, `None`.
-        """
-        super().__init__(strength, hook, seed)
-        if not isinstance(epsilon, Scheduler):
-            epsilon = NoScheduling[float](epsilon)
-        self.epsilon_scheduler = epsilon
-
-    @property
-    def hook(self) -> Optional[str]:
-        # return hook only if the strength or epislon scheduler requires to be stepped
-        return (
-            None
-            if isinstance(self.strength_scheduler, NoScheduling)
-            and isinstance(self.epsilon_scheduler, NoScheduling)
-            else self._hook
-        )
-
-    @property
-    def epsilon(self) -> float:
-        """Gets the current probability of the exploration strategy."""
-        return self.epsilon_scheduler.value
-
-    def can_explore(self) -> bool:
-        return self.np_random.random() <= self.epsilon_scheduler.value
-
-    def step(self, *_, **__) -> None:
-        """Updates the exploration probability and strength according to their
-        schedulers."""
-        self.strength_scheduler.step()
-        self.epsilon_scheduler.step()
-
-    def __repr__(self) -> str:
-        hook = self.hook
-        hookstr = "None" if hook is None else f"'{hook}'"
-        return (
-            f"{self.__class__.__name__}(eps={self.epsilon_scheduler.value},"
-            f"stn={self.strength_scheduler.value},hook={hookstr})"
-        )
-
-
-class StepWiseExploration(ExplorationStrategy):
-    """Wrapper exploration class that enables a base exploration strategy to change only
-    every N steps, thus yielding a step-wise strategy with steps of the given length.
-    This is useful when, e.g., the exploration strategy must be kept constant across
-    time for a number of steps.
-
-    Note
-    ----
-    This exploration wrapper modifies the exploration chance and magnitude of the
-    wrapped base strategy as well as the step behaviour, i.e., the decay of the base
-    exploration's schedulers (if any) is enlarged by the step size factor. This is
-    because the number of calls to the base exploration's `step` method is reduced by
-    a factor of the step size.
-    """
-
-    def __init__(
-        self,
-        base_exploration: ExplorationStrategy,
-        step_size: int,
-        stepwise_decay: bool = True,
-    ) -> None:
-        """Creates a step-wise exploration strategy wrapepr.
-
-        Parameters
-        ----------
-        base_exploration : ExplorationStrategy
-            The base exploration strategy to be made step-wise.
-        step_size : int
-            Size of each step.
-        stepwise_decay : bool, optional
-            Enables the decay `step` to also be step-wise, i.e., applied only every N
-            steps.
-        """
-        super().__init__()
-        self.base_exploration = base_exploration
-        self.step_size = step_size
-        self._explore_counter = 0
-        self._step_counter = 0
-        self._stepwise_decay = stepwise_decay
-
-    @property
-    def hook(self) -> Optional[str]:
-        """Returns the hook of the base exploration strategy, if any."""
-        return getattr(self.base_exploration, "hook", None)
-
-    def can_explore(self) -> bool:
-        # since this method is called at every timestep (when deterministic=False), we
-        # decide here if the base exploration is frozen or not, i.e., if we are at the
-        # new step or not
-        self._explore_counter %= self.step_size
-        if self._explore_counter == 0:
-            self._cached_can_explore = self._cached_perturbation = None
-        self._explore_counter += 1
-
-        if self._cached_can_explore is not None:
-            return self._cached_can_explore
-        self._cached_can_explore = self.base_exploration.can_explore()
-        return self._cached_can_explore
-
-    def step(self, *_, **__) -> None:
-        if not self._stepwise_decay:
-            return self.base_exploration.step()
-        self._step_counter %= self.step_size
-        if self._step_counter == 0:
-            self.base_exploration.step()
-        self._step_counter += 1
-
-    def perturbation(self, *args: Any, **kwargs: Any) -> npt.NDArray[np.floating]:
-        if self._cached_perturbation is not None:
-            return self._cached_perturbation
-        self._cached_perturbation = self.base_exploration.perturbation(*args, **kwargs)
-        return self._cached_perturbation
-
-    def __repr__(self) -> str:
-        clsn = self.__class__.__name__
-        bclsn = self.base_exploration.__class__.__name__
-        return f"{clsn}(base={bclsn},step_size={self.step_size})"
+from abc import ABC, abstractmethod
+from typing import Any, Literal, Optional, Union
+
+import numpy as np
+import numpy.typing as npt
+
+from ..util.seeding import RngType
+from .schedulers import NoScheduling, Scheduler
+
+
+class ExplorationStrategy(ABC):
+    """Base class for exploration strategies such as greedy, epsilon-greeyd, etc."""
+
+    @abstractmethod
+    def can_explore(self) -> bool:
+        """Computes whether, according to the exploration strategy, the agent should
+        explore or not at the current instant.
+
+        Returns
+        -------
+        bool
+            `True` if the agent should explore according to this strategy; otherwise,
+            `False`.
+        """
+
+    @abstractmethod
+    def step(self, *args: Any, **kwargs: Any) -> None:
+        """Updates the exploration strength and/or probability, in case the strategy
+        supports them (usually, by decaying them over time)."""
+
+    @abstractmethod
+    def perturbation(self, *args: Any, **kwargs: Any) -> npt.NDArray[np.floating]:
+        """Returns a random perturbation."""
+
+    def __str__(self) -> str:
+        return self.__class__.__name__
+
+    def __repr__(self) -> str:
+        hook: Optional[str] = getattr(self, "hook", None)
+        if hook is None:
+            return self.__class__.__name__
+        return f"{self.__class__.__name__}(hook='{hook}')"
+
+
+class NoExploration(ExplorationStrategy):
+    """Strategy where no exploration is allowed at any time or, in other words, the
+    policy is always deterministic (only based on the current state, and not perturbed).
+    """
+
+    def can_explore(self) -> bool:
+        return False
+
+    def step(self, *_, **__) -> None:
+        return
+
+    def perturbation(self, *args: Any, **kwargs: Any) -> npt.NDArray[np.floating]:
+        raise NotImplementedError(
+            f"Perturbation not implemented in {self.__class__.__name__}"
+        )
+
+
+class GreedyExploration(ExplorationStrategy):
+    """Fully greedy strategy for perturbing the policy, thus inducing exploration. This
+    strategy always perturbs randomly the policy."""
+
+    def __init__(
+        self,
+        strength: Union[Scheduler[npt.NDArray[np.floating]], npt.NDArray[np.floating]],
+        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
+        seed: RngType = None,
+    ) -> None:
+        """Initializes the greedy exploration strategy.
+
+        Parameters
+        ----------
+        strength : scheduler or array/supports-algebraic-operations
+            The strength of the exploration. If passed in the form of an
+            `mpcrl.schedulers.Scheduler`, then the strength can be scheduled to
+            decay/increase every time `exploration.step` is called. If an array or
+            something other than a scheduler is passed, then this quantity will get
+            wrapped in a base scheduler which will kept it constant.
+        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
+            Specifies to which callback to hook, i.e., when to step the exploration's
+            schedulers (if any) to, e.g., decay the chances of exploring or the
+            perturbation strength (see `step` method also). The options are:
+             - `on_update` steps the exploration after each agent's update
+             - `on_episode_end` steps the exploration after each episode's end
+             - `on_timestep_end` steps the exploration after each env's timestep.
+
+            By default, 'on_update' is selected.
+        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
+            Number to seed the RNG engine used for randomizing the exploration. By
+            default, `None`.
+        """
+        super().__init__()
+        self._hook = hook
+        if not isinstance(strength, Scheduler):
+            strength = NoScheduling[npt.NDArray[np.floating]](strength)
+        self.strength_scheduler = strength
+        self.reset(seed)
+
+    @property
+    def hook(self) -> Optional[str]:
+        """Specifies to which callback to hook, i.e., when to step the exploration's
+        schedulers (if any) to, e.g., decay the chances of exploring or the perturbation
+        strength (see `step` method also). Can be `None` in case no hook is needed."""
+        # return hook only if the strength scheduler requires to be stepped
+        return None if isinstance(self.strength_scheduler, NoScheduling) else self._hook
+
+    @property
+    def strength(self) -> npt.NDArray[np.floating]:
+        """Gets the current strength of the exploration strategy."""
+        return self.strength_scheduler.value
+
+    def reset(self, seed: RngType = None) -> None:
+        """Resets the exploration RNG."""
+        self.np_random = np.random.default_rng(seed)
+
+    def can_explore(self) -> bool:
+        return True
+
+    def step(self, *_, **__) -> None:
+        """Updates the exploration strength according to its scheduler."""
+        self.strength_scheduler.step()
+
+    def perturbation(
+        self, method: str, *args: Any, **kwargs: Any
+    ) -> npt.NDArray[np.floating]:
+        """Returns a random perturbation.
+
+        Parameters
+        ----------
+        method : str
+            The name of a method from the ones available to `numpy.random.Generator`,
+            e.g., 'random', 'normal', etc.
+        args, kwargs
+            Args and kwargs with which to call such method.
+
+        Returns
+        -------
+        array
+            An array representing the perturbation.
+        """
+        return (
+            getattr(self.np_random, method)(*args, **kwargs)
+            * self.strength_scheduler.value
+        )
+
+    def __repr__(self) -> str:
+        hook = self.hook
+        hookstr = "None" if hook is None else f"'{hook}'"
+        return (
+            f"{self.__class__.__name__}(stn={self.strength_scheduler.value},"
+            f"hook={hookstr})"
+        )
+
+
+class EpsilonGreedyExploration(GreedyExploration):
+    """Epsilon-greedy strategy for perturbing the policy, thus inducing exploration.
+    This strategy only occasionally perturbs randomly the policy."""
+
+    def __init__(
+        self,
+        epsilon: Union[Scheduler[float], float],
+        strength: Union[Scheduler[npt.NDArray[np.floating]], npt.NDArray[np.floating]],
+        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
+        seed: RngType = None,
+    ) -> None:
+        """Initializes the epsilon-greedy exploration strategy.
+
+        Parameters
+        ----------
+        epsilon : scheduler or float
+            The probability to explore. Should be in range [0, 1]. If passed in the form
+            of an `mpcrl.schedulers.Scheduler`, then the probability can be scheduled to
+            decay/increase every time `exploration.step` is called. If an array or
+            something other than a scheduler is passed, then this quantity will get
+            wrapped in a base scheduler which will kept it constant.
+        strength : scheduler or array/supports-algebraic-operations
+            The strength of the exploration. Can be scheduled, see `epsilon`.
+        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
+            Specifies to which callback to hook, i.e., when to step the exploration's
+            schedulers (if any) to, e.g., decay the chances of exploring or the
+            perturbation strength (see `step` method also). The options are:
+             - `on_update` steps the exploration after each agent's update
+             - `on_episode_end` steps the exploration after each episode's end
+             - `on_timestep_end` steps the exploration after each env's timestep.
+
+            By default, 'on_update' is selected.
+        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
+            Number to seed the RNG engine used for randomizing the exploration. By
+            default, `None`.
+        """
+        super().__init__(strength, hook, seed)
+        if not isinstance(epsilon, Scheduler):
+            epsilon = NoScheduling[float](epsilon)
+        self.epsilon_scheduler = epsilon
+
+    @property
+    def hook(self) -> Optional[str]:
+        # return hook only if the strength or epislon scheduler requires to be stepped
+        return (
+            None
+            if isinstance(self.strength_scheduler, NoScheduling)
+            and isinstance(self.epsilon_scheduler, NoScheduling)
+            else self._hook
+        )
+
+    @property
+    def epsilon(self) -> float:
+        """Gets the current probability of the exploration strategy."""
+        return self.epsilon_scheduler.value
+
+    def can_explore(self) -> bool:
+        return self.np_random.random() <= self.epsilon_scheduler.value
+
+    def step(self, *_, **__) -> None:
+        """Updates the exploration probability and strength according to their
+        schedulers."""
+        self.strength_scheduler.step()
+        self.epsilon_scheduler.step()
+
+    def __repr__(self) -> str:
+        hook = self.hook
+        hookstr = "None" if hook is None else f"'{hook}'"
+        return (
+            f"{self.__class__.__name__}(eps={self.epsilon_scheduler.value},"
+            f"stn={self.strength_scheduler.value},hook={hookstr})"
+        )
+
+
+class StepWiseExploration(ExplorationStrategy):
+    """Wrapper exploration class that enables a base exploration strategy to change only
+    every N steps, thus yielding a step-wise strategy with steps of the given length.
+    This is useful when, e.g., the exploration strategy must be kept constant across
+    time for a number of steps.
+
+    Note
+    ----
+    This exploration wrapper modifies the exploration chance and magnitude of the
+    wrapped base strategy as well as the step behaviour, i.e., the decay of the base
+    exploration's schedulers (if any) is enlarged by the step size factor. This is
+    because the number of calls to the base exploration's `step` method is reduced by
+    a factor of the step size.
+    """
+
+    def __init__(
+        self,
+        base_exploration: ExplorationStrategy,
+        step_size: int,
+        stepwise_decay: bool = True,
+    ) -> None:
+        """Creates a step-wise exploration strategy wrapepr.
+
+        Parameters
+        ----------
+        base_exploration : ExplorationStrategy
+            The base exploration strategy to be made step-wise.
+        step_size : int
+            Size of each step.
+        stepwise_decay : bool, optional
+            Enables the decay `step` to also be step-wise, i.e., applied only every N
+            steps.
+        """
+        super().__init__()
+        self.base_exploration = base_exploration
+        self.step_size = step_size
+        self._explore_counter = 0
+        self._step_counter = 0
+        self._stepwise_decay = stepwise_decay
+
+    @property
+    def hook(self) -> Optional[str]:
+        """Returns the hook of the base exploration strategy, if any."""
+        return getattr(self.base_exploration, "hook", None)
+
+    def can_explore(self) -> bool:
+        # since this method is called at every timestep (when deterministic=False), we
+        # decide here if the base exploration is frozen or not, i.e., if we are at the
+        # new step or not
+        self._explore_counter %= self.step_size
+        if self._explore_counter == 0:
+            self._cached_can_explore = self._cached_perturbation = None
+        self._explore_counter += 1
+
+        if self._cached_can_explore is not None:
+            return self._cached_can_explore
+        self._cached_can_explore = self.base_exploration.can_explore()
+        return self._cached_can_explore
+
+    def step(self, *_, **__) -> None:
+        if not self._stepwise_decay:
+            return self.base_exploration.step()
+        self._step_counter %= self.step_size
+        if self._step_counter == 0:
+            self.base_exploration.step()
+        self._step_counter += 1
+
+    def perturbation(self, *args: Any, **kwargs: Any) -> npt.NDArray[np.floating]:
+        if self._cached_perturbation is not None:
+            return self._cached_perturbation
+        self._cached_perturbation = self.base_exploration.perturbation(*args, **kwargs)
+        return self._cached_perturbation
+
+    def __repr__(self) -> str:
+        clsn = self.__class__.__name__
+        bclsn = self.base_exploration.__class__.__name__
+        return f"{clsn}(base={bclsn},step_size={self.step_size})"
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/core/parameters.py` & `mpcrl-1.2.0rc4/src/mpcrl/core/parameters.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,309 +1,309 @@
-from collections.abc import Iterable
-from functools import cached_property
-from itertools import chain
-from numbers import Integral
-from typing import Any, Generic, Optional, TypeVar, Union
-
-import numpy as np
-import numpy.typing as npt
-from csnlp.core.cache import invalidate_cache
-from csnlp.util.io import SupportsDeepcopyAndPickle
-
-from ..util.math import summarize_array
-
-SymType = TypeVar("SymType")  # most likely, T is cs.SX or MX
-
-
-class LearnableParameter(SupportsDeepcopyAndPickle, Generic[SymType]):
-    """A parameter that is learnable, that is, it can be adjusted via RL. This class
-    is useful for managing symbols, bounds and value of learnable parameters."""
-
-    def __init__(
-        self,
-        name: str,
-        shape: Union[int, tuple[int, ...]],
-        value: npt.ArrayLike,
-        lb: npt.ArrayLike = -np.inf,
-        ub: npt.ArrayLike = +np.inf,
-        sym: Optional[SymType] = None,
-    ) -> None:
-        """Instantiates a learnable parameter.
-
-        Parameters
-        ----------
-        name : str
-            Name of the learnable parameter.
-        shape : int or tuple of ints
-            Shape of the parameter.
-        value : array_like
-            Starting value of the parameter. This can then be updated via `update`.
-        lb : array_like, optional
-            Lower bound of the parameter values. If not specified, it is unbounded.
-        ub : array_like, optional
-            Upper bound of the parameter values. If not specified, it is unbounded.
-        sym : T, optional
-            An optional reference to a symbolic variable representing this parameter.
-
-        Raises
-        ------
-        ValueError
-            Raises if `value`, `lb` or `ub` cannot be broadcasted to a 1D vector with
-            shape equal to `shape`; or if the shape of the symbolic variable `sym` does
-            not match the shape of the parameter.
-        """
-        super().__init__()
-        self.name = name
-        self.shape: tuple[int, ...] = (
-            (shape,) if isinstance(shape, Integral) else shape  # type: ignore
-        )
-        self.sym = sym
-        self.lb: npt.NDArray[np.floating] = np.broadcast_to(lb, shape)
-        self.ub: npt.NDArray[np.floating] = np.broadcast_to(ub, shape)
-        self._check_sym_shape()
-        self._update_value(value)
-
-    @property
-    def size(self) -> int:
-        """Gets the number of elements in the parameter."""
-        return np.prod(self.shape, dtype=int).item()
-
-    def _update_value(self, v: npt.ArrayLike, **is_close_kwargs: Any) -> None:
-        """Internal utility for updating the parameter value with a new value.
-
-        Parameters
-        ----------
-        new_value : array_like
-            New value of the parameter.
-        is_close_kwargs
-            Additional kwargs for `np.isclose`, e.g., `rtol` and `atol`, for checking
-            numerical values close to a bound.
-
-        Raises
-        ------
-        ValueError
-            Raises if `new_value` cannot be broadcasted to a 1D vector with shape equal
-            to `shape`; or if it does not lie inside the upper and lower bounds within
-            the specified tolerances.
-        """
-        v = np.broadcast_to(v, self.shape)
-        lb = self.lb
-        ub = self.ub
-        if ((v < lb) & ~np.isclose(v, lb, **is_close_kwargs)).any() or (
-            (v > ub) & ~np.isclose(v, ub, **is_close_kwargs)
-        ).any():
-            raise ValueError(f"Updated parameter `{self.name}` is outside bounds.")
-        self.value: npt.NDArray[np.floating] = np.clip(v, lb, ub)
-
-    def _check_sym_shape(self) -> None:
-        """Internal utility for checking that the shape of the symbolic variable matches
-        the shape of the parameter."""
-        if self.sym is None or not hasattr(self.sym, "shape"):
-            return
-        sym_shape = tuple(self.sym.shape)
-        shape = self.shape + tuple(1 for _ in range(len(sym_shape) - len(self.shape)))
-        if sym_shape != shape:
-            raise ValueError("Shape of `sym` does not match `shape`.")
-
-    def __str__(self) -> str:
-        return f"<{self.name}(shape={self.shape})>"
-
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}(name={self.name},shape={self.shape})>"
-
-
-class LearnableParametersDict(
-    dict[str, LearnableParameter[SymType]], SupportsDeepcopyAndPickle
-):
-    """dict-based collection of `LearnableParameter` instances that simplifies the
-    process of managing and updating these. The dict contains pairs of parameter's name
-    vs parameter's instance.
-
-    Note: to speed up computations, properties of this class are often cached for faster
-    calls to the same methods. However, these are cleared when the underlying dict is
-    modified."""
-
-    def __init__(self, pars: Optional[Iterable[LearnableParameter[SymType]]] = None):
-        """Initializes the collection of learnable parameters.
-
-        Parameters
-        ----------
-        pars : iterable of LearnableParameter, optional
-            An optional iterable of parameters to insert into the dict by their names.
-        """
-        if pars is None:
-            dict.__init__(self)
-        else:
-            dict.__init__(self, map(lambda p: (p.name, p), chain(pars)))
-        SupportsDeepcopyAndPickle.__init__(self)
-
-    @cached_property
-    def size(self) -> int:
-        """Gets the overall size of all the learnable parameters."""
-        return sum(p.size for p in self.values())
-
-    @cached_property
-    def lb(self) -> npt.NDArray[np.floating]:
-        """Gets the lower bound of all the learnable parameters, concatenated."""
-        return (
-            np.concatenate([p.lb.reshape(-1, order="F") for p in self.values()])
-            if self
-            else np.empty(0)
-        )
-
-    @cached_property
-    def ub(self) -> npt.NDArray[np.floating]:
-        """Gets the upper bound of all the learnable parameters, concatenated."""
-        return (
-            np.concatenate([p.ub.reshape(-1, order="F") for p in self.values()])
-            if self
-            else np.empty(0)
-        )
-
-    @cached_property
-    def value(self) -> npt.NDArray[np.floating]:
-        """Gets the values of all the learnable parameters, concatenated."""
-        return (
-            np.concatenate([p.value.reshape(-1, order="F") for p in self.values()])
-            if self
-            else np.empty(0)
-        )
-
-    @cached_property
-    def value_as_dict(self) -> dict[str, npt.NDArray[np.floating]]:
-        """Gets the values of all the learnable parameters, in a dict."""
-        return {p.name: p.value for p in self.values()}
-
-    @cached_property
-    def sym(self) -> dict[str, Optional[SymType]]:
-        """Gets symbols of all the learnable parameters, in a dict. If one parameter
-        does not possess the symbol, `None` is put."""
-        return {
-            parname: None if par.sym is None else par.sym
-            for parname, par in self.items()
-        }
-
-    @invalidate_cache(value, value_as_dict)
-    def update_values(
-        self,
-        new_values: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
-        **is_close_kwargs: Any,
-    ) -> None:
-        """Updates the value of each parameter
-
-        Parameters
-        ----------
-        new_values : array_like or dict[str, array_like]
-            The parameters' new values, either as a single concatenated array (which
-            will be splitted according to the sizes and each piece sequentially assigned
-            to each parameter), or as a dict of parameter's name vs parameter's new
-            value.
-        is_close_kwargs
-            Additional kwargs for `np.isclose`, e.g., `rtol` and `atol`, for checking
-            numerical values of parameters close to a bound.
-
-        Raises
-        ------
-        ValueError
-            In case of array-like, raises if `new_values` cannot be split according to
-            the sizes of parameters; or if the new values cannot be broadcasted to 1D
-            vectors according to each parameter's size; or if the new values lie outside
-            either the lower or upper bounds of each parameter.
-        """
-        if isinstance(new_values, dict):
-            for parname, new_value in new_values.items():
-                self[parname]._update_value(new_value, **is_close_kwargs)
-        else:
-            cumsizes = np.cumsum([p.size for p in self.values()])[:-1]
-            values_ = np.split(new_values, cumsizes)
-            for par, val in zip(self.values(), values_):
-                par._update_value(val.reshape(par.shape, order="F"), **is_close_kwargs)
-
-    __cache_decorator = invalidate_cache(size, lb, ub, value, value_as_dict, sym)
-
-    @__cache_decorator
-    def __setitem__(self, name: str, par: LearnableParameter[SymType]) -> None:
-        assert name == par.name, f"Key '{name}' must match parameter name '{par.name}'."
-        return super().__setitem__(name, par)
-
-    @__cache_decorator
-    def update(
-        self,
-        pars: Iterable[LearnableParameter[SymType]],
-        *args: LearnableParameter[SymType],
-    ) -> None:
-        return super().update(map(lambda p: (p.name, p), chain(pars, args)))
-
-    @__cache_decorator
-    def setdefault(
-        self,
-        par: LearnableParameter[SymType],
-    ) -> LearnableParameter[SymType]:
-        return super().setdefault(par.name, par)
-
-    __delitem__ = __cache_decorator(dict.__delitem__)
-    pop = __cache_decorator(dict.pop)
-    popitem = __cache_decorator(dict.popitem)
-    clear = __cache_decorator(dict.clear)
-
-    def copy(
-        self, deep: bool = False, invalidate_caches: bool = True
-    ) -> "LearnableParametersDict[SymType]":
-        """Creates a shallow or deep copy of the dict of learnable parameters.
-
-        Parameters
-        ----------
-        deep : bool, optional
-            If `True`, a deepcopy of the dict and its parameters is returned; otherwise,
-            the copy is only shallow.
-        invalidate_caches : bool, optional
-            If `True`, methods decorated with `csnlp.util.funcs.invalidate_cache` are
-            called to clear cached properties/lru caches in the copied instance.
-            Otherwise, caches in the copy are not invalidated. By default, `True`.
-            Only relevant when `deep=True`.
-
-        Returns
-        -------
-        LearnableParametersDict[T]
-            A copy of the dict of learnable parameters.
-        """
-        return (
-            SupportsDeepcopyAndPickle.copy(self, invalidate_caches)
-            if deep
-            else LearnableParametersDict[SymType](self.values())
-        )
-
-    def stringify(
-        self, summarize: bool = True, precision: int = 3, ddof: int = 0
-    ) -> str:
-        """Returns a string representing the dict of learnable parameters.
-
-        Parameters
-        ----------
-        summarize : bool, optional
-            If `True` (default), array parameters are summarized; otherwise, the entire
-            array is printed.
-        precision : int, optional
-            The printing precision of floating point numbers.
-        ddof : int, optional
-            Degrees of freedom for computing standard deviations (see `numpy.std`).
-
-        Returns
-        -------
-        str
-            A string representing the dict and its parameters.
-        """
-
-        def p2s(p: LearnableParameter) -> str:
-            if p.size == 1:
-                return f"{p.name}={p.value.item():.{precision}f}"
-            if summarize:
-                return f"{p.name}: {summarize_array(p.value, precision, ddof)}"
-            return np.array2string(p.value, precision=precision)
-
-        return "; ".join(p2s(p) for p in self.values())
-
-    def __str__(self) -> str:
-        return self.stringify()
-
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}: {super().__repr__()}>"
+from collections.abc import Iterable
+from functools import cached_property
+from itertools import chain
+from numbers import Integral
+from typing import Any, Generic, Optional, TypeVar, Union
+
+import numpy as np
+import numpy.typing as npt
+from csnlp.core.cache import invalidate_cache
+from csnlp.util.io import SupportsDeepcopyAndPickle
+
+from ..util.math import summarize_array
+
+SymType = TypeVar("SymType")  # most likely, T is cs.SX or MX
+
+
+class LearnableParameter(SupportsDeepcopyAndPickle, Generic[SymType]):
+    """A parameter that is learnable, that is, it can be adjusted via RL. This class
+    is useful for managing symbols, bounds and value of learnable parameters."""
+
+    def __init__(
+        self,
+        name: str,
+        shape: Union[int, tuple[int, ...]],
+        value: npt.ArrayLike,
+        lb: npt.ArrayLike = -np.inf,
+        ub: npt.ArrayLike = +np.inf,
+        sym: Optional[SymType] = None,
+    ) -> None:
+        """Instantiates a learnable parameter.
+
+        Parameters
+        ----------
+        name : str
+            Name of the learnable parameter.
+        shape : int or tuple of ints
+            Shape of the parameter.
+        value : array_like
+            Starting value of the parameter. This can then be updated via `update`.
+        lb : array_like, optional
+            Lower bound of the parameter values. If not specified, it is unbounded.
+        ub : array_like, optional
+            Upper bound of the parameter values. If not specified, it is unbounded.
+        sym : T, optional
+            An optional reference to a symbolic variable representing this parameter.
+
+        Raises
+        ------
+        ValueError
+            Raises if `value`, `lb` or `ub` cannot be broadcasted to a 1D vector with
+            shape equal to `shape`; or if the shape of the symbolic variable `sym` does
+            not match the shape of the parameter.
+        """
+        super().__init__()
+        self.name = name
+        self.shape: tuple[int, ...] = (
+            (shape,) if isinstance(shape, Integral) else shape  # type: ignore
+        )
+        self.sym = sym
+        self.lb: npt.NDArray[np.floating] = np.broadcast_to(lb, shape)
+        self.ub: npt.NDArray[np.floating] = np.broadcast_to(ub, shape)
+        self._check_sym_shape()
+        self._update_value(value)
+
+    @property
+    def size(self) -> int:
+        """Gets the number of elements in the parameter."""
+        return np.prod(self.shape, dtype=int).item()
+
+    def _update_value(self, v: npt.ArrayLike, **is_close_kwargs: Any) -> None:
+        """Internal utility for updating the parameter value with a new value.
+
+        Parameters
+        ----------
+        new_value : array_like
+            New value of the parameter.
+        is_close_kwargs
+            Additional kwargs for `np.isclose`, e.g., `rtol` and `atol`, for checking
+            numerical values close to a bound.
+
+        Raises
+        ------
+        ValueError
+            Raises if `new_value` cannot be broadcasted to a 1D vector with shape equal
+            to `shape`; or if it does not lie inside the upper and lower bounds within
+            the specified tolerances.
+        """
+        v = np.broadcast_to(v, self.shape)
+        lb = self.lb
+        ub = self.ub
+        if ((v < lb) & ~np.isclose(v, lb, **is_close_kwargs)).any() or (
+            (v > ub) & ~np.isclose(v, ub, **is_close_kwargs)
+        ).any():
+            raise ValueError(f"Updated parameter `{self.name}` is outside bounds.")
+        self.value: npt.NDArray[np.floating] = np.clip(v, lb, ub)
+
+    def _check_sym_shape(self) -> None:
+        """Internal utility for checking that the shape of the symbolic variable matches
+        the shape of the parameter."""
+        if self.sym is None or not hasattr(self.sym, "shape"):
+            return
+        sym_shape = tuple(self.sym.shape)
+        shape = self.shape + tuple(1 for _ in range(len(sym_shape) - len(self.shape)))
+        if sym_shape != shape:
+            raise ValueError("Shape of `sym` does not match `shape`.")
+
+    def __str__(self) -> str:
+        return f"<{self.name}(shape={self.shape})>"
+
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__}(name={self.name},shape={self.shape})>"
+
+
+class LearnableParametersDict(
+    dict[str, LearnableParameter[SymType]], SupportsDeepcopyAndPickle
+):
+    """dict-based collection of `LearnableParameter` instances that simplifies the
+    process of managing and updating these. The dict contains pairs of parameter's name
+    vs parameter's instance.
+
+    Note: to speed up computations, properties of this class are often cached for faster
+    calls to the same methods. However, these are cleared when the underlying dict is
+    modified."""
+
+    def __init__(self, pars: Optional[Iterable[LearnableParameter[SymType]]] = None):
+        """Initializes the collection of learnable parameters.
+
+        Parameters
+        ----------
+        pars : iterable of LearnableParameter, optional
+            An optional iterable of parameters to insert into the dict by their names.
+        """
+        if pars is None:
+            dict.__init__(self)
+        else:
+            dict.__init__(self, map(lambda p: (p.name, p), chain(pars)))
+        SupportsDeepcopyAndPickle.__init__(self)
+
+    @cached_property
+    def size(self) -> int:
+        """Gets the overall size of all the learnable parameters."""
+        return sum(p.size for p in self.values())
+
+    @cached_property
+    def lb(self) -> npt.NDArray[np.floating]:
+        """Gets the lower bound of all the learnable parameters, concatenated."""
+        return (
+            np.concatenate([p.lb.reshape(-1, order="F") for p in self.values()])
+            if self
+            else np.empty(0)
+        )
+
+    @cached_property
+    def ub(self) -> npt.NDArray[np.floating]:
+        """Gets the upper bound of all the learnable parameters, concatenated."""
+        return (
+            np.concatenate([p.ub.reshape(-1, order="F") for p in self.values()])
+            if self
+            else np.empty(0)
+        )
+
+    @cached_property
+    def value(self) -> npt.NDArray[np.floating]:
+        """Gets the values of all the learnable parameters, concatenated."""
+        return (
+            np.concatenate([p.value.reshape(-1, order="F") for p in self.values()])
+            if self
+            else np.empty(0)
+        )
+
+    @cached_property
+    def value_as_dict(self) -> dict[str, npt.NDArray[np.floating]]:
+        """Gets the values of all the learnable parameters, in a dict."""
+        return {p.name: p.value for p in self.values()}
+
+    @cached_property
+    def sym(self) -> dict[str, Optional[SymType]]:
+        """Gets symbols of all the learnable parameters, in a dict. If one parameter
+        does not possess the symbol, `None` is put."""
+        return {
+            parname: None if par.sym is None else par.sym
+            for parname, par in self.items()
+        }
+
+    @invalidate_cache(value, value_as_dict)
+    def update_values(
+        self,
+        new_values: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
+        **is_close_kwargs: Any,
+    ) -> None:
+        """Updates the value of each parameter
+
+        Parameters
+        ----------
+        new_values : array_like or dict[str, array_like]
+            The parameters' new values, either as a single concatenated array (which
+            will be splitted according to the sizes and each piece sequentially assigned
+            to each parameter), or as a dict of parameter's name vs parameter's new
+            value.
+        is_close_kwargs
+            Additional kwargs for `np.isclose`, e.g., `rtol` and `atol`, for checking
+            numerical values of parameters close to a bound.
+
+        Raises
+        ------
+        ValueError
+            In case of array-like, raises if `new_values` cannot be split according to
+            the sizes of parameters; or if the new values cannot be broadcasted to 1D
+            vectors according to each parameter's size; or if the new values lie outside
+            either the lower or upper bounds of each parameter.
+        """
+        if isinstance(new_values, dict):
+            for parname, new_value in new_values.items():
+                self[parname]._update_value(new_value, **is_close_kwargs)
+        else:
+            cumsizes = np.cumsum([p.size for p in self.values()])[:-1]
+            values_ = np.split(new_values, cumsizes)
+            for par, val in zip(self.values(), values_):
+                par._update_value(val.reshape(par.shape, order="F"), **is_close_kwargs)
+
+    __cache_decorator = invalidate_cache(size, lb, ub, value, value_as_dict, sym)
+
+    @__cache_decorator
+    def __setitem__(self, name: str, par: LearnableParameter[SymType]) -> None:
+        assert name == par.name, f"Key '{name}' must match parameter name '{par.name}'."
+        return super().__setitem__(name, par)
+
+    @__cache_decorator
+    def update(
+        self,
+        pars: Iterable[LearnableParameter[SymType]],
+        *args: LearnableParameter[SymType],
+    ) -> None:
+        return super().update(map(lambda p: (p.name, p), chain(pars, args)))
+
+    @__cache_decorator
+    def setdefault(
+        self,
+        par: LearnableParameter[SymType],
+    ) -> LearnableParameter[SymType]:
+        return super().setdefault(par.name, par)
+
+    __delitem__ = __cache_decorator(dict.__delitem__)
+    pop = __cache_decorator(dict.pop)
+    popitem = __cache_decorator(dict.popitem)
+    clear = __cache_decorator(dict.clear)
+
+    def copy(
+        self, deep: bool = False, invalidate_caches: bool = True
+    ) -> "LearnableParametersDict[SymType]":
+        """Creates a shallow or deep copy of the dict of learnable parameters.
+
+        Parameters
+        ----------
+        deep : bool, optional
+            If `True`, a deepcopy of the dict and its parameters is returned; otherwise,
+            the copy is only shallow.
+        invalidate_caches : bool, optional
+            If `True`, methods decorated with `csnlp.util.funcs.invalidate_cache` are
+            called to clear cached properties/lru caches in the copied instance.
+            Otherwise, caches in the copy are not invalidated. By default, `True`.
+            Only relevant when `deep=True`.
+
+        Returns
+        -------
+        LearnableParametersDict[T]
+            A copy of the dict of learnable parameters.
+        """
+        return (
+            SupportsDeepcopyAndPickle.copy(self, invalidate_caches)
+            if deep
+            else LearnableParametersDict[SymType](self.values())
+        )
+
+    def stringify(
+        self, summarize: bool = True, precision: int = 3, ddof: int = 0
+    ) -> str:
+        """Returns a string representing the dict of learnable parameters.
+
+        Parameters
+        ----------
+        summarize : bool, optional
+            If `True` (default), array parameters are summarized; otherwise, the entire
+            array is printed.
+        precision : int, optional
+            The printing precision of floating point numbers.
+        ddof : int, optional
+            Degrees of freedom for computing standard deviations (see `numpy.std`).
+
+        Returns
+        -------
+        str
+            A string representing the dict and its parameters.
+        """
+
+        def p2s(p: LearnableParameter) -> str:
+            if p.size == 1:
+                return f"{p.name}={p.value.item():.{precision}f}"
+            if summarize:
+                return f"{p.name}: {summarize_array(p.value, precision, ddof)}"
+            return np.array2string(p.value, precision=precision)
+
+        return "; ".join(p2s(p) for p in self.values())
+
+    def __str__(self) -> str:
+        return self.stringify()
+
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__}: {super().__repr__()}>"
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/core/schedulers.py` & `mpcrl-1.2.0rc4/src/mpcrl/core/schedulers.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-from abc import ABC, abstractmethod
-from collections.abc import Iterable
-from itertools import accumulate, repeat
-from operator import mul
-from typing import Generic, TypeVar, Union
-
-import numpy as np
-
-ScType = TypeVar("ScType")
-ScType.__doc__ = "A type that supports basic algebraic operations."
-
-
-class Scheduler(ABC, Generic[ScType]):
-    """Schedulers are helpful classes to update or decay different quantities, such as
-    learning rates and/or exploration probability.
-
-    Note
-    ----
-    If the scheduler has a final iteration, it is expected to raise a `StopIteration`
-    exception when the last iteration is reached.
-    """
-
-    def __init__(self, init_value: ScType) -> None:
-        """Builds the scheduler.
-
-        Parameters
-        ----------
-        init_value : supports-algebraic-operations
-            Initial value that will be updated by this scheduler.
-        """
-        super().__init__()
-        self.value = init_value
-
-    @abstractmethod
-    def step(self) -> None:
-        """Updates the value of the scheduler by one step.
-
-        Raises
-        ------
-        StopIteration
-            Raises if the final iteration of the scheduler (if any) has been reached and
-            `step` was called again.
-        """
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(x={self.value})"
-
-    def __str__(self) -> str:
-        return self.__repr__()
-
-
-class NoScheduling(Scheduler[ScType]):
-    """Scheduler that actually performs no scheduling and holds the initial value
-    constant."""
-
-    def step(self) -> None:
-        return
-
-
-class ExponentialScheduler(Scheduler[ScType]):
-    """Exponentiallly decays the value of the scheduler by `factor` every step, i.e.,
-    after k steps the value `value_k = init_value * factor**k`."""
-
-    def __init__(self, init_value: ScType, factor: ScType) -> None:
-        """Builds the exponential scheduler.
-
-        Parameters
-        ----------
-        init_value : supports-algebraic-operations
-            Initial value that will be updated by this scheduler.
-        factor : Tsc
-            The exponential factor to decay the initial value with.
-        """
-        super().__init__(init_value)
-        self.factor = factor
-
-    def step(self) -> None:
-        self.value *= self.factor  # type: ignore[operator]
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(x={self.value},factor={self.factor})"
-
-
-class LinearScheduler(Scheduler[ScType]):
-    """Linearly updates the initial value of the scheduler towards a final one to be
-    reached in N total steps, i.e., after k steps, the value is
-    `value_k = init_value + (final_value - init_value) * k / total_steps`.
-    """
-
-    def __init__(
-        self, init_value: ScType, final_value: ScType, total_steps: int
-    ) -> None:
-        """Builds the exponential scheduler.
-
-        Parameters
-        ----------
-        init_value : supports-algebraic-operations
-            Initial value that will be updated by this scheduler.
-        final_value : supports-algebraic-operations
-            Final value that will be reached by the scheduler after `total_steps`.
-        total_steps : int
-            Total number of steps to linearly interpolate between `init_value` and
-            `final_value`.
-        """
-        super().__init__(init_value)
-        increment = (final_value - init_value) / total_steps  # type: ignore[operator]
-        self.init_value = init_value
-        self.final_value = final_value
-        self.total_steps = total_steps
-        self.generator = accumulate(repeat(increment, total_steps), initial=init_value)
-        next(self.generator)
-
-    def step(self) -> None:
-        self.value = next(self.generator)
-
-    def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__name__}(x={self.value},x0={self.init_value},"
-            f"xf={self.final_value},N={self.total_steps})"
-        )
-
-
-class LogLinearScheduler(ExponentialScheduler[ScType]):
-    """Updates the initial value of the scheduler towards a final one to be
-    reached in N total steps in a linear fashion between the exponents of the two, i.e.,
-    after k steps, the value is
-    `value_k = init_value * exp(ln(final_value / init_value) / total_steps)**k`.
-    """
-
-    def __init__(
-        self, init_value: ScType, final_value: ScType, total_steps: int
-    ) -> None:
-        factor = np.exp(
-            np.log(final_value / init_value) / total_steps  # type: ignore[operator]
-        )
-        super().__init__(init_value, factor)
-        self.init_value = init_value
-        self.final_value = final_value
-        self.total_steps = total_steps
-        self.generator = accumulate(
-            repeat(factor, total_steps), mul, initial=init_value
-        )
-        next(self.generator)
-
-    def step(self) -> None:
-        self.value = next(self.generator)
-
-    def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__name__}(x={self.value},x0={self.init_value},"
-            f"xf={self.final_value},N={self.total_steps})"
-        )
-
-
-class Chain(Scheduler[ScType]):
-    """Chains multiple schedulers together."""
-
-    def __init__(
-        self,
-        schedulers: Iterable[Union[Scheduler[ScType], tuple[Scheduler[ScType], int]]],
-    ) -> None:
-        """Builds the chain of schedulers.
-
-        Parameters
-        ----------
-        schedulers : iterable of schedulers or (scheduler, int)
-            An iterable of schedulers to chain together. If a tuple is passed, the first
-            element is expected to be a scheduler, and the second one an integer
-            indicating the number of steps to run that scheduler for. This is useful in
-            case the scheduler has no fixed number of steps, such as `LinearScheduler`.
-        """
-        self.schedulers = iter(schedulers)
-        self._next_scheduler()
-        super().__init__(self._current_scheduler.value)
-
-    def step(self) -> None:
-        if self._current_steps is not None:
-            self._current_scheduler.step()
-            self._current_steps -= 1
-            if self._current_steps == 0:
-                self._next_scheduler()
-        else:
-            try:
-                self._current_scheduler.step()
-            except StopIteration:
-                self._next_scheduler()
-        self.value = self._current_scheduler.value
-
-    def _next_scheduler(self) -> None:
-        """Fetches the next scheduler in the chain. If the chain is over, raises
-        `StopIteration`, which is in line with the behaviour of other schedulers."""
-        scheduler = next(self.schedulers)
-        if isinstance(scheduler, tuple):
-            self._current_scheduler, self._current_steps = scheduler
-        else:
-            self._current_scheduler = scheduler
-            self._current_steps = None
-
-    def __repr__(self) -> str:
-        s = self._current_scheduler
-        return f"{self.__class__.__name__}(x={self.value},current={s})"
+from abc import ABC, abstractmethod
+from collections.abc import Iterable
+from itertools import accumulate, repeat
+from operator import mul
+from typing import Generic, TypeVar, Union
+
+import numpy as np
+
+ScType = TypeVar("ScType")
+ScType.__doc__ = "A type that supports basic algebraic operations."
+
+
+class Scheduler(ABC, Generic[ScType]):
+    """Schedulers are helpful classes to update or decay different quantities, such as
+    learning rates and/or exploration probability.
+
+    Note
+    ----
+    If the scheduler has a final iteration, it is expected to raise a `StopIteration`
+    exception when the last iteration is reached.
+    """
+
+    def __init__(self, init_value: ScType) -> None:
+        """Builds the scheduler.
+
+        Parameters
+        ----------
+        init_value : supports-algebraic-operations
+            Initial value that will be updated by this scheduler.
+        """
+        super().__init__()
+        self.value = init_value
+
+    @abstractmethod
+    def step(self) -> None:
+        """Updates the value of the scheduler by one step.
+
+        Raises
+        ------
+        StopIteration
+            Raises if the final iteration of the scheduler (if any) has been reached and
+            `step` was called again.
+        """
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(x={self.value})"
+
+    def __str__(self) -> str:
+        return self.__repr__()
+
+
+class NoScheduling(Scheduler[ScType]):
+    """Scheduler that actually performs no scheduling and holds the initial value
+    constant."""
+
+    def step(self) -> None:
+        return
+
+
+class ExponentialScheduler(Scheduler[ScType]):
+    """Exponentiallly decays the value of the scheduler by `factor` every step, i.e.,
+    after k steps the value `value_k = init_value * factor**k`."""
+
+    def __init__(self, init_value: ScType, factor: ScType) -> None:
+        """Builds the exponential scheduler.
+
+        Parameters
+        ----------
+        init_value : supports-algebraic-operations
+            Initial value that will be updated by this scheduler.
+        factor : Tsc
+            The exponential factor to decay the initial value with.
+        """
+        super().__init__(init_value)
+        self.factor = factor
+
+    def step(self) -> None:
+        self.value *= self.factor  # type: ignore[operator]
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(x={self.value},factor={self.factor})"
+
+
+class LinearScheduler(Scheduler[ScType]):
+    """Linearly updates the initial value of the scheduler towards a final one to be
+    reached in N total steps, i.e., after k steps, the value is
+    `value_k = init_value + (final_value - init_value) * k / total_steps`.
+    """
+
+    def __init__(
+        self, init_value: ScType, final_value: ScType, total_steps: int
+    ) -> None:
+        """Builds the exponential scheduler.
+
+        Parameters
+        ----------
+        init_value : supports-algebraic-operations
+            Initial value that will be updated by this scheduler.
+        final_value : supports-algebraic-operations
+            Final value that will be reached by the scheduler after `total_steps`.
+        total_steps : int
+            Total number of steps to linearly interpolate between `init_value` and
+            `final_value`.
+        """
+        super().__init__(init_value)
+        increment = (final_value - init_value) / total_steps  # type: ignore[operator]
+        self.init_value = init_value
+        self.final_value = final_value
+        self.total_steps = total_steps
+        self.generator = accumulate(repeat(increment, total_steps), initial=init_value)
+        next(self.generator)
+
+    def step(self) -> None:
+        self.value = next(self.generator)
+
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}(x={self.value},x0={self.init_value},"
+            f"xf={self.final_value},N={self.total_steps})"
+        )
+
+
+class LogLinearScheduler(ExponentialScheduler[ScType]):
+    """Updates the initial value of the scheduler towards a final one to be
+    reached in N total steps in a linear fashion between the exponents of the two, i.e.,
+    after k steps, the value is
+    `value_k = init_value * exp(ln(final_value / init_value) / total_steps)**k`.
+    """
+
+    def __init__(
+        self, init_value: ScType, final_value: ScType, total_steps: int
+    ) -> None:
+        factor = np.exp(
+            np.log(final_value / init_value) / total_steps  # type: ignore[operator]
+        )
+        super().__init__(init_value, factor)
+        self.init_value = init_value
+        self.final_value = final_value
+        self.total_steps = total_steps
+        self.generator = accumulate(
+            repeat(factor, total_steps), mul, initial=init_value
+        )
+        next(self.generator)
+
+    def step(self) -> None:
+        self.value = next(self.generator)
+
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}(x={self.value},x0={self.init_value},"
+            f"xf={self.final_value},N={self.total_steps})"
+        )
+
+
+class Chain(Scheduler[ScType]):
+    """Chains multiple schedulers together."""
+
+    def __init__(
+        self,
+        schedulers: Iterable[Union[Scheduler[ScType], tuple[Scheduler[ScType], int]]],
+    ) -> None:
+        """Builds the chain of schedulers.
+
+        Parameters
+        ----------
+        schedulers : iterable of schedulers or (scheduler, int)
+            An iterable of schedulers to chain together. If a tuple is passed, the first
+            element is expected to be a scheduler, and the second one an integer
+            indicating the number of steps to run that scheduler for. This is useful in
+            case the scheduler has no fixed number of steps, such as `LinearScheduler`.
+        """
+        self.schedulers = iter(schedulers)
+        self._next_scheduler()
+        super().__init__(self._current_scheduler.value)
+
+    def step(self) -> None:
+        if self._current_steps is not None:
+            self._current_scheduler.step()
+            self._current_steps -= 1
+            if self._current_steps == 0:
+                self._next_scheduler()
+        else:
+            try:
+                self._current_scheduler.step()
+            except StopIteration:
+                self._next_scheduler()
+        self.value = self._current_scheduler.value
+
+    def _next_scheduler(self) -> None:
+        """Fetches the next scheduler in the chain. If the chain is over, raises
+        `StopIteration`, which is in line with the behaviour of other schedulers."""
+        scheduler = next(self.schedulers)
+        if isinstance(scheduler, tuple):
+            self._current_scheduler, self._current_steps = scheduler
+        else:
+            self._current_scheduler = scheduler
+            self._current_steps = None
+
+    def __repr__(self) -> str:
+        s = self._current_scheduler
+        return f"{self.__class__.__name__}(x={self.value},current={s})"
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/core/update.py` & `mpcrl-1.2.0rc4/src/mpcrl/core/update.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from collections.abc import Iterator
-from typing import Literal
-
-from ..util.iters import bool_cycle, chain, repeat
-
-
-class UpdateStrategy:
-    """A class for the update strategy."""
-
-    def __init__(
-        self,
-        frequency: int,
-        hook: Literal["on_episode_end", "on_timestep_end"] = "on_timestep_end",
-        skip_first: int = 0,
-    ) -> None:
-        """Initializes the update strategy.
-
-        Parameters
-        ----------
-        frequency : int
-            Frequency at which, each time the hook is called, an update should be
-            carried out.
-        skip_first : int, optional
-            Skips the first `skip_first` updates. By default 0, so no update is skipped.
-            This is useful when, e.g., the agent has to wait for the experience buffer
-            to be filled before starting to update.
-        hook : {'on_episode_end', 'on_timestep_end'}, optional
-            Specifies to which callback to hook, i.e., when to check if an update is due
-            according to the given frequency. The options are:
-             - `on_episode_end` checks for an update after each episode's end
-             - `on_timestep_end` checks for an update after each env's timestep.
-
-            By default, 'on_timestep_end' is selected.
-        """
-        self.frequency = frequency
-        self.hook = hook
-        self._update_cycle = chain(
-            repeat(False, skip_first * frequency), bool_cycle(frequency)
-        )
-
-    def can_update(self) -> bool:
-        """Returns whether an update must be carried out at the current instant
-        according to the strategy.
-
-        Notes
-        -----
-        This methods steps internal iterators to check whether an update is due, so
-        calling this method again will return a different value.
-
-        Returns
-        -------
-        bool
-            `True` if the agent should update according to this strategy; otherwise,
-            `False`.
-        """
-        return next(self._update_cycle)
-
-    def __iter__(self) -> Iterator[bool]:
-        """With `__next__`, makes this class act like an iterator."""
-        return self._update_cycle
-
-    def __next__(self) -> bool:
-        """With `__iter__`, makes this class act like an iterator."""
-        return next(self._update_cycle)
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(frequency={self.frequency},hook={self.hook})"
-
-    def __str__(self) -> str:
-        return self.__repr__()
+from collections.abc import Iterator
+from typing import Literal
+
+from ..util.iters import bool_cycle, chain, repeat
+
+
+class UpdateStrategy:
+    """A class for the update strategy."""
+
+    def __init__(
+        self,
+        frequency: int,
+        hook: Literal["on_episode_end", "on_timestep_end"] = "on_timestep_end",
+        skip_first: int = 0,
+    ) -> None:
+        """Initializes the update strategy.
+
+        Parameters
+        ----------
+        frequency : int
+            Frequency at which, each time the hook is called, an update should be
+            carried out.
+        skip_first : int, optional
+            Skips the first `skip_first` updates. By default 0, so no update is skipped.
+            This is useful when, e.g., the agent has to wait for the experience buffer
+            to be filled before starting to update.
+        hook : {'on_episode_end', 'on_timestep_end'}, optional
+            Specifies to which callback to hook, i.e., when to check if an update is due
+            according to the given frequency. The options are:
+             - `on_episode_end` checks for an update after each episode's end
+             - `on_timestep_end` checks for an update after each env's timestep.
+
+            By default, 'on_timestep_end' is selected.
+        """
+        self.frequency = frequency
+        self.hook = hook
+        self._update_cycle = chain(
+            repeat(False, skip_first * frequency), bool_cycle(frequency)
+        )
+
+    def can_update(self) -> bool:
+        """Returns whether an update must be carried out at the current instant
+        according to the strategy.
+
+        Notes
+        -----
+        This methods steps internal iterators to check whether an update is due, so
+        calling this method again will return a different value.
+
+        Returns
+        -------
+        bool
+            `True` if the agent should update according to this strategy; otherwise,
+            `False`.
+        """
+        return next(self._update_cycle)
+
+    def __iter__(self) -> Iterator[bool]:
+        """With `__next__`, makes this class act like an iterator."""
+        return self._update_cycle
+
+    def __next__(self) -> bool:
+        """With `__iter__`, makes this class act like an iterator."""
+        return next(self._update_cycle)
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(frequency={self.frequency},hook={self.hook})"
+
+    def __str__(self) -> str:
+        return self.__repr__()
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/optim/adam.py` & `mpcrl-1.2.0rc4/src/mpcrl/optim/adam.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-from typing import Literal, Optional, Union
-
-import casadi as cs
-import numpy as np
-import numpy.typing as npt
-
-from ..core.parameters import LearnableParametersDict, SymType
-from ..core.schedulers import Scheduler
-from .gradient_based_optimizer import GradientBasedOptimizer, LrType
-
-
-class Adam(GradientBasedOptimizer[SymType, LrType]):
-    """Adam and AdamW optimizers, based on [1,2] and [3,4], respectively. AMSGrad is
-    also supported [5].
-
-    References
-    ----------
-    [1] Kingma, D.P. and Ba, J., 2014. Adam: A method for stochastic optimization.
-        arXiv preprint arXiv:1412.6980.
-    [2] Loshchilov, I. and Hutter, F., 2017. Decoupled weight decay regularization.
-        arXiv preprint arXiv:1711.05101.
-    [3] Adam - PyTorch 2.1 documentation.
-        https://pytorch.org/docs/stable/generated/torch.optim.Adam.html
-    [4] AdamW - PyTorch 2.1 documentation.
-        https://pytorch.org/docs/stable/generated/torch.optim.AdamW.html
-    [5] Reddi, S.J., Kale, S. and Kumar, S., 2019. On the convergence of adam and
-        beyond. arXiv preprint arXiv:1904.09237.
-    """
-
-    _order = 1
-    _hessian_sparsity = "diag"
-    """In Adam, hessian is at most diagonal, i.e., in case we have constraints."""
-
-    def __init__(
-        self,
-        learning_rate: Union[LrType, Scheduler[LrType]],
-        betas: tuple[float, float] = (0.9, 0.999),
-        eps: float = 1e-8,
-        weight_decay: float = 0.0,
-        decoupled_weight_decay: bool = False,
-        amsgrad: bool = False,
-        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
-        max_percentage_update: float = float("+inf"),
-    ) -> None:
-        """Instantiates the optimizer.
-
-        Parameters
-        ----------
-        learning_rate : float/array, scheduler
-            The learning rate of the optimizer. A float/array can be passed in case the
-            learning rate must stay constant; otherwise, a scheduler can be passed which
-            will be stepped `on_update` by default (see `hook` argument).
-        betas : tuple of 2 floats, optional
-            Coefficients used for computing running averages of gradient and its square.
-            By default, they are set to `(0.9, 0.999)`.
-        eps : float, optional
-            Term added to the denominator to improve numerical stability. By default, it
-            is set to `1e-8`.
-        weight_decay : float, optional
-            A positive float that specifies the decay of the learnable parameters in the
-            form of an L2 regularization term. By default, it is set to `0.0`, so no
-            decay/regularization takes place.
-        decoupled_weight_decay : bool, optional
-            If `False`, the optimizer is Adam. Otherwise, it is `AdamW`. By default, it
-            is `False`.
-        amsgrad : bool, optional
-            If `True`, uses the AMSGrad variant. By default, it is `False`.
-        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
-            Specifies when to step the optimizer's learning rate's scheduler to decay
-            its value (see `step` method also). This allows to vary the rate over the
-            learning iterations. The options are:
-             - `on_update` steps the learning rate after each agent's update
-             - `on_episode_end` steps the learning rate after each episode's end
-             - `on_timestep_end` steps the learning rate after each env's timestep.
-
-            By default, 'on_update' is selected.
-        max_percentage_update : float, optional
-            A positive float that specifies the maximum percentage change the learnable
-            parameters can experience in each update. For example,
-            `max_percentage_update=0.5` means that the parameters can be updated by up
-            to 50% of their current value. By default, it is set to `+inf`. If
-            specified, the update becomes constrained and has to be solved as a QP,
-            which is inevitably slower than its unconstrained counterpart.
-        """
-        super().__init__(learning_rate, hook, max_percentage_update)
-        self.weight_decay = weight_decay
-        self.beta1, self.beta2 = betas
-        self.eps = eps
-        self.decoupled_weight_decay = decoupled_weight_decay
-        self.amsgrad = amsgrad
-
-    def set_learnable_parameters(self, pars: LearnableParametersDict[SymType]) -> None:
-        super().set_learnable_parameters(pars)
-        # initialize also running averages
-        n = pars.size
-        self._exp_avg = np.zeros(n, dtype=float)
-        self._exp_avg_sq = np.zeros(n, dtype=float)
-        self._max_exp_avg_sq = np.zeros(n, dtype=float) if self.amsgrad else None
-        self._step = 0
-
-    def _first_order_update(
-        self, gradient: npt.NDArray[np.floating]
-    ) -> tuple[npt.NDArray[np.floating], Optional[str]]:
-        theta = self.learnable_parameters.value
-
-        # compute candidate update
-        weight_decay = self.weight_decay
-        lr = self.lr_scheduler.value
-        if weight_decay > 0.0:
-            if self.decoupled_weight_decay:  # i.e., AdamW
-                theta = theta * (1 - weight_decay * lr)
-            else:
-                gradient = gradient + weight_decay * theta
-        self._step += 1
-        dtheta, self._exp_avg, self._exp_avg_sq, self._max_exp_avg_sq = _adam(
-            self._step,
-            gradient,
-            self._exp_avg,
-            self._exp_avg_sq,
-            lr,
-            self.beta1,
-            self.beta2,
-            self.eps,
-            self._max_exp_avg_sq,
-        )
-
-        # if unconstrained, apply the update directly; otherwise, solve the QP
-        solver = self._update_solver
-        if solver is None:
-            return theta + dtheta, None
-        lbx, ubx = self._get_update_bounds(theta)
-        sol = solver(h=cs.DM.eye(theta.shape[0]), g=-dtheta, lbx=lbx, ubx=ubx)
-        dtheta = np.asarray(sol["x"].elements())
-        stats = solver.stats()
-        return theta + dtheta, None if stats["success"] else stats["return_status"]
-
-
-def _adam(
-    step: int,
-    g: np.ndarray,
-    exp_avg: np.ndarray,
-    exp_avg_sq: np.ndarray,
-    lr: LrType,
-    beta1: float,
-    beta2: float,
-    eps: float,
-    max_exp_avg_sq: Optional[np.ndarray],
-) -> tuple[np.ndarray, np.ndarray, np.ndarray, Optional[np.ndarray]]:
-    """Computes the update's change according to Adam algorithm."""
-    exp_avg = beta1 * exp_avg + (1 - beta1) * g
-    exp_avg_sq = beta2 * exp_avg_sq + (1 - beta2) * np.square(g)
-
-    bias_correction1 = 1 - beta1**step
-    bias_correction2 = 1 - beta2**step
-    step_size = lr / bias_correction1
-    bias_correction2_sqrt = np.sqrt(bias_correction2)
-
-    if max_exp_avg_sq is None:
-        denom = np.sqrt(exp_avg_sq) / bias_correction2_sqrt + eps
-    else:  # i.e., AMSGrad
-        max_exp_avg_sq = np.maximum(max_exp_avg_sq, exp_avg_sq)
-        denom = np.sqrt(max_exp_avg_sq) / bias_correction2_sqrt + eps
-    dtheta = -step_size * (exp_avg / denom)
-    return dtheta, exp_avg, exp_avg_sq, max_exp_avg_sq
+from typing import Literal, Optional, Union
+
+import casadi as cs
+import numpy as np
+import numpy.typing as npt
+
+from ..core.parameters import LearnableParametersDict, SymType
+from ..core.schedulers import Scheduler
+from .gradient_based_optimizer import GradientBasedOptimizer, LrType
+
+
+class Adam(GradientBasedOptimizer[SymType, LrType]):
+    """Adam and AdamW optimizers, based on [1,2] and [3,4], respectively. AMSGrad is
+    also supported [5].
+
+    References
+    ----------
+    [1] Kingma, D.P. and Ba, J., 2014. Adam: A method for stochastic optimization.
+        arXiv preprint arXiv:1412.6980.
+    [2] Loshchilov, I. and Hutter, F., 2017. Decoupled weight decay regularization.
+        arXiv preprint arXiv:1711.05101.
+    [3] Adam - PyTorch 2.1 documentation.
+        https://pytorch.org/docs/stable/generated/torch.optim.Adam.html
+    [4] AdamW - PyTorch 2.1 documentation.
+        https://pytorch.org/docs/stable/generated/torch.optim.AdamW.html
+    [5] Reddi, S.J., Kale, S. and Kumar, S., 2019. On the convergence of adam and
+        beyond. arXiv preprint arXiv:1904.09237.
+    """
+
+    _order = 1
+    _hessian_sparsity = "diag"
+    """In Adam, hessian is at most diagonal, i.e., in case we have constraints."""
+
+    def __init__(
+        self,
+        learning_rate: Union[LrType, Scheduler[LrType]],
+        betas: tuple[float, float] = (0.9, 0.999),
+        eps: float = 1e-8,
+        weight_decay: float = 0.0,
+        decoupled_weight_decay: bool = False,
+        amsgrad: bool = False,
+        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
+        max_percentage_update: float = float("+inf"),
+    ) -> None:
+        """Instantiates the optimizer.
+
+        Parameters
+        ----------
+        learning_rate : float/array, scheduler
+            The learning rate of the optimizer. A float/array can be passed in case the
+            learning rate must stay constant; otherwise, a scheduler can be passed which
+            will be stepped `on_update` by default (see `hook` argument).
+        betas : tuple of 2 floats, optional
+            Coefficients used for computing running averages of gradient and its square.
+            By default, they are set to `(0.9, 0.999)`.
+        eps : float, optional
+            Term added to the denominator to improve numerical stability. By default, it
+            is set to `1e-8`.
+        weight_decay : float, optional
+            A positive float that specifies the decay of the learnable parameters in the
+            form of an L2 regularization term. By default, it is set to `0.0`, so no
+            decay/regularization takes place.
+        decoupled_weight_decay : bool, optional
+            If `False`, the optimizer is Adam. Otherwise, it is `AdamW`. By default, it
+            is `False`.
+        amsgrad : bool, optional
+            If `True`, uses the AMSGrad variant. By default, it is `False`.
+        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
+            Specifies when to step the optimizer's learning rate's scheduler to decay
+            its value (see `step` method also). This allows to vary the rate over the
+            learning iterations. The options are:
+             - `on_update` steps the learning rate after each agent's update
+             - `on_episode_end` steps the learning rate after each episode's end
+             - `on_timestep_end` steps the learning rate after each env's timestep.
+
+            By default, 'on_update' is selected.
+        max_percentage_update : float, optional
+            A positive float that specifies the maximum percentage change the learnable
+            parameters can experience in each update. For example,
+            `max_percentage_update=0.5` means that the parameters can be updated by up
+            to 50% of their current value. By default, it is set to `+inf`. If
+            specified, the update becomes constrained and has to be solved as a QP,
+            which is inevitably slower than its unconstrained counterpart.
+        """
+        super().__init__(learning_rate, hook, max_percentage_update)
+        self.weight_decay = weight_decay
+        self.beta1, self.beta2 = betas
+        self.eps = eps
+        self.decoupled_weight_decay = decoupled_weight_decay
+        self.amsgrad = amsgrad
+
+    def set_learnable_parameters(self, pars: LearnableParametersDict[SymType]) -> None:
+        super().set_learnable_parameters(pars)
+        # initialize also running averages
+        n = pars.size
+        self._exp_avg = np.zeros(n, dtype=float)
+        self._exp_avg_sq = np.zeros(n, dtype=float)
+        self._max_exp_avg_sq = np.zeros(n, dtype=float) if self.amsgrad else None
+        self._step = 0
+
+    def _first_order_update(
+        self, gradient: npt.NDArray[np.floating]
+    ) -> tuple[npt.NDArray[np.floating], Optional[str]]:
+        theta = self.learnable_parameters.value
+
+        # compute candidate update
+        weight_decay = self.weight_decay
+        lr = self.lr_scheduler.value
+        if weight_decay > 0.0:
+            if self.decoupled_weight_decay:  # i.e., AdamW
+                theta = theta * (1 - weight_decay * lr)
+            else:
+                gradient = gradient + weight_decay * theta
+        self._step += 1
+        dtheta, self._exp_avg, self._exp_avg_sq, self._max_exp_avg_sq = _adam(
+            self._step,
+            gradient,
+            self._exp_avg,
+            self._exp_avg_sq,
+            lr,
+            self.beta1,
+            self.beta2,
+            self.eps,
+            self._max_exp_avg_sq,
+        )
+
+        # if unconstrained, apply the update directly; otherwise, solve the QP
+        solver = self._update_solver
+        if solver is None:
+            return theta + dtheta, None
+        lbx, ubx = self._get_update_bounds(theta)
+        sol = solver(h=cs.DM.eye(theta.shape[0]), g=-dtheta, lbx=lbx, ubx=ubx)
+        dtheta = np.asarray(sol["x"].elements())
+        stats = solver.stats()
+        return theta + dtheta, None if stats["success"] else stats["return_status"]
+
+
+def _adam(
+    step: int,
+    g: np.ndarray,
+    exp_avg: np.ndarray,
+    exp_avg_sq: np.ndarray,
+    lr: LrType,
+    beta1: float,
+    beta2: float,
+    eps: float,
+    max_exp_avg_sq: Optional[np.ndarray],
+) -> tuple[np.ndarray, np.ndarray, np.ndarray, Optional[np.ndarray]]:
+    """Computes the update's change according to Adam algorithm."""
+    exp_avg = beta1 * exp_avg + (1 - beta1) * g
+    exp_avg_sq = beta2 * exp_avg_sq + (1 - beta2) * np.square(g)
+
+    bias_correction1 = 1 - beta1**step
+    bias_correction2 = 1 - beta2**step
+    step_size = lr / bias_correction1
+    bias_correction2_sqrt = np.sqrt(bias_correction2)
+
+    if max_exp_avg_sq is None:
+        denom = np.sqrt(exp_avg_sq) / bias_correction2_sqrt + eps
+    else:  # i.e., AMSGrad
+        max_exp_avg_sq = np.maximum(max_exp_avg_sq, exp_avg_sq)
+        denom = np.sqrt(max_exp_avg_sq) / bias_correction2_sqrt + eps
+    dtheta = -step_size * (exp_avg / denom)
+    return dtheta, exp_avg, exp_avg_sq, max_exp_avg_sq
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/optim/base_optimizer.py` & `mpcrl-1.2.0rc4/src/mpcrl/optim/base_optimizer.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from typing import Any, Generic
-
-import numpy as np
-
-from ..core.parameters import LearnableParametersDict, SymType
-
-
-class BaseOptimizer(Generic[SymType]):
-    """Base class for optimization algorithms
-
-    This class contains useful methods for, e.g., initializing the optimizer, retrieving
-    bounds on the learnable parameters, etc."""
-
-    def __init__(self, max_percentage_update: float = float("+inf")) -> None:
-        """Instantiates the optimizer.
-
-        Parameters
-        ----------
-        max_percentage_update : float, optional
-            A positive float that specifies the maximum percentage change the learnable
-            parameters can experience in each update. For example,
-            `max_percentage_update=0.5` means that the parameters can be updated by up
-            to 50% of their current value. By default, it is set to `+inf`.
-        """
-        self.max_percentage_update = max_percentage_update
-        self.learnable_parameters: LearnableParametersDict[SymType] = None
-
-    def set_learnable_parameters(self, pars: LearnableParametersDict[SymType]) -> None:
-        """Makes the optimization class aware of the dictionary of the learnable
-        parameters.
-
-        Parmeters
-        ---------
-        pars : LearnableParametersDict
-            The dictionary of the learnable parameters.
-        """
-        self.learnable_parameters = pars
-        self._update_solver = self._init_update_solver()
-
-    def _get_update_bounds(
-        self, theta: np.ndarray, eps: float = 0.1
-    ) -> tuple[np.ndarray, np.ndarray]:
-        """Internal utility to retrieve the current bounds on the learnable parameters.
-        Only useful if the update problem is not unconstrained, i.e., there are either
-        some lb or ub, or a maximum percentage update."""
-        lb = self.learnable_parameters.lb - theta
-        ub = self.learnable_parameters.ub - theta
-        perc = self.max_percentage_update
-        if perc != float("+inf"):
-            max_update_delta = np.maximum(np.abs(perc * theta), eps)
-            lb = np.maximum(lb, -max_update_delta)
-            ub = np.minimum(ub, +max_update_delta)
-        return lb, ub
-
-    def _init_update_solver(self) -> Any:
-        """Internal utility to initialize whatever solver is necessary to compute the
-        learning strategy."""
-
-    def __str__(self) -> str:
-        return self.__class__.__name__
-
-    def __repr__(self) -> str:
-        cn = self.__class__.__name__
-        mp = self.max_percentage_update
-        return f"{cn}(max%={mp})"
+from typing import Any, Generic
+
+import numpy as np
+
+from ..core.parameters import LearnableParametersDict, SymType
+
+
+class BaseOptimizer(Generic[SymType]):
+    """Base class for optimization algorithms
+
+    This class contains useful methods for, e.g., initializing the optimizer, retrieving
+    bounds on the learnable parameters, etc."""
+
+    def __init__(self, max_percentage_update: float = float("+inf")) -> None:
+        """Instantiates the optimizer.
+
+        Parameters
+        ----------
+        max_percentage_update : float, optional
+            A positive float that specifies the maximum percentage change the learnable
+            parameters can experience in each update. For example,
+            `max_percentage_update=0.5` means that the parameters can be updated by up
+            to 50% of their current value. By default, it is set to `+inf`.
+        """
+        self.max_percentage_update = max_percentage_update
+        self.learnable_parameters: LearnableParametersDict[SymType] = None
+
+    def set_learnable_parameters(self, pars: LearnableParametersDict[SymType]) -> None:
+        """Makes the optimization class aware of the dictionary of the learnable
+        parameters.
+
+        Parmeters
+        ---------
+        pars : LearnableParametersDict
+            The dictionary of the learnable parameters.
+        """
+        self.learnable_parameters = pars
+        self._update_solver = self._init_update_solver()
+
+    def _get_update_bounds(
+        self, theta: np.ndarray, eps: float = 0.1
+    ) -> tuple[np.ndarray, np.ndarray]:
+        """Internal utility to retrieve the current bounds on the learnable parameters.
+        Only useful if the update problem is not unconstrained, i.e., there are either
+        some lb or ub, or a maximum percentage update."""
+        lb = self.learnable_parameters.lb - theta
+        ub = self.learnable_parameters.ub - theta
+        perc = self.max_percentage_update
+        if perc != float("+inf"):
+            max_update_delta = np.maximum(np.abs(perc * theta), eps)
+            lb = np.maximum(lb, -max_update_delta)
+            ub = np.minimum(ub, +max_update_delta)
+        return lb, ub
+
+    def _init_update_solver(self) -> Any:
+        """Internal utility to initialize whatever solver is necessary to compute the
+        learning strategy."""
+
+    def __str__(self) -> str:
+        return self.__class__.__name__
+
+    def __repr__(self) -> str:
+        cn = self.__class__.__name__
+        mp = self.max_percentage_update
+        return f"{cn}(max%={mp})"
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/optim/gradient_based_optimizer.py` & `mpcrl-1.2.0rc4/src/mpcrl/optim/gradient_based_optimizer.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-from typing import Generic, Literal, Optional, TypeVar, Union
-
-import casadi as cs
-import numpy as np
-import numpy.typing as npt
-
-from ..core.schedulers import NoScheduling, Scheduler
-from .base_optimizer import BaseOptimizer, SymType
-
-LrType = TypeVar("LrType", npt.NDArray[np.floating], float)
-
-
-class GradientBasedOptimizer(BaseOptimizer[SymType], Generic[SymType, LrType]):
-    """Base class for first- and second-order gradient-based optimization algorithms."""
-
-    _order: Literal[1, 2]
-    """Order of the optimizer: 1 for first-order, 2 for second-order."""
-
-    _hessian_sparsity: Literal["dense", "diag"]
-    """Sparsity of the hessian. It can be overridden by each subclass, in case a
-    particular structure is known, e.g., diagonal."""
-
-    def __init__(
-        self,
-        learning_rate: Union[LrType, Scheduler[LrType]],
-        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
-        max_percentage_update: float = float("+inf"),
-    ) -> None:
-        """Instantiates the optimizer.
-
-        Parameters
-        ----------
-        learning_rate : float/array, scheduler
-            The learning rate of the optimizer. A float/array can be passed in case the
-            learning rate must stay constant; otherwise, a scheduler can be passed which
-            will be stepped `on_update` by default (see `hook` argument).
-        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
-            Specifies when to step the optimizer's learning rate's scheduler to decay
-            its value (see `step` method also). This allows to vary the rate over the
-            learning iterations. The options are:
-             - `on_update` steps the learning rate after each agent's update
-             - `on_episode_end` steps the learning rate after each episode's end
-             - `on_timestep_end` steps the learning rate after each env's timestep.
-
-            By default, 'on_update' is selected.
-        max_percentage_update : float, optional
-            A positive float that specifies the maximum percentage change the learnable
-            parameters can experience in each update. For example,
-            `max_percentage_update=0.5` means that the parameters can be updated by up
-            to 50% of their current value. By default, it is set to `+inf`.
-        """
-        super().__init__(max_percentage_update)
-        if not isinstance(learning_rate, Scheduler):
-            learning_rate = NoScheduling[LrType](learning_rate)
-        self.lr_scheduler: Scheduler[LrType] = learning_rate
-        self._hook = hook
-        self._update_solver: cs.Function
-
-    @property
-    def hook(self) -> Optional[str]:
-        """Specifies to which callback to hook, i.e., when to step the learning rate's
-        scheduler to decay its value (see `step` method also). Can be `None` in case no
-        hook is needed."""
-        # return hook only if the learning rate scheduler requires to be stepped
-        return None if isinstance(self.lr_scheduler, NoScheduling) else self._hook
-
-    def step(self, *_, **__) -> None:
-        """Steps/decays the learning rate according to its scheduler."""
-        self.lr_scheduler.step()
-
-    def _init_update_solver(self) -> Optional[cs.Function]:
-        """Internal utility to initialize, if the learnable parameters are constrained,
-        a constrained update solver which, by default, is a QP. Otherwise, no solver is
-        required to perform the update.
-        """
-        if (
-            self.max_percentage_update == float("+inf")
-            and np.isneginf(self.learnable_parameters.lb).all()
-            and np.isposinf(self.learnable_parameters.ub).all()
-        ):
-            return None
-        n_params = self.learnable_parameters.size
-        qp = {"h": getattr(cs.Sparsity, self._hessian_sparsity)(n_params, n_params)}
-        opts = {
-            "error_on_fail": False,
-            "osqp": {
-                "verbose": False,
-                "polish": True,
-                "scaling": 20,
-                "eps_abs": 1e-9,
-                "eps_rel": 1e-9,
-                "eps_prim_inf": 1e-10,
-                "eps_dual_inf": 1e-10,
-                "max_iter": 6000,
-            },
-        }
-        return cs.conic(f"qpsol_{id(self)}", "osqp", qp, opts)
-
-    def update(
-        self,
-        gradient: npt.NDArray[np.floating],
-        hessian: Optional[npt.NDArray[np.floating]] = None,
-    ) -> Optional[str]:
-        """Computes the gradient update of the learnable parameters dictated by the
-        current RL algorithm.
-
-        Parameters
-        ----------
-        gradient : 1D array
-            The gradient of the learnable parameters.
-        hessian : None, or 2D array
-            The hessian of the learnable parameters. When the optimizer is firt-order,
-            it is expected to be `None` (as it is unused). When the optimizer is
-            second-order, it is expected to be a 2D array.
-
-        Returns
-        -------
-        status : str, optional
-            An optional string containing the status of the update, e.g., the status of
-            the QP solver, if used.
-        """
-        if self._order == 1:
-            theta_new, status = self._first_order_update(gradient)
-        else:
-            theta_new, status = self._second_order_update(gradient, hessian)
-        # theta_new = np.clip(
-        #     theta_new, self.learnable_parameters.lb, self.learnable_parameters.ub
-        # )
-        self.learnable_parameters.update_values(theta_new)
-        return status
-
-    def _first_order_update(
-        self, gradient: npt.NDArray[np.floating]
-    ) -> tuple[npt.NDArray[np.floating], Optional[str]]:
-        """Internally runs a first order update."""
-        raise NotImplementedError(
-            f"`{self.__class__.__name__}` optimizer does not implement "
-            "`_first_order_update`"
-        )
-
-    def _second_order_update(
-        self, gradient: npt.NDArray[np.floating], hessian: npt.NDArray[np.floating]
-    ) -> tuple[npt.NDArray[np.floating], Optional[str]]:
-        """Internally runs a second order update."""
-        raise NotImplementedError(
-            f"`{self.__class__.__name__}` optimizer does not implement "
-            "`_second_order_update`"
-        )
-
-    def __repr__(self) -> str:
-        cn = self.__class__.__name__
-        hookstr = "None" if self.hook is None else f"'{self.hook}'"
-        mp = self.max_percentage_update
-        return f"{cn}(lr={self.lr_scheduler},hook={hookstr},max%={mp})"
+from typing import Generic, Literal, Optional, TypeVar, Union
+
+import casadi as cs
+import numpy as np
+import numpy.typing as npt
+
+from ..core.schedulers import NoScheduling, Scheduler
+from .base_optimizer import BaseOptimizer, SymType
+
+LrType = TypeVar("LrType", npt.NDArray[np.floating], float)
+
+
+class GradientBasedOptimizer(BaseOptimizer[SymType], Generic[SymType, LrType]):
+    """Base class for first- and second-order gradient-based optimization algorithms."""
+
+    _order: Literal[1, 2]
+    """Order of the optimizer: 1 for first-order, 2 for second-order."""
+
+    _hessian_sparsity: Literal["dense", "diag"]
+    """Sparsity of the hessian. It can be overridden by each subclass, in case a
+    particular structure is known, e.g., diagonal."""
+
+    def __init__(
+        self,
+        learning_rate: Union[LrType, Scheduler[LrType]],
+        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
+        max_percentage_update: float = float("+inf"),
+    ) -> None:
+        """Instantiates the optimizer.
+
+        Parameters
+        ----------
+        learning_rate : float/array, scheduler
+            The learning rate of the optimizer. A float/array can be passed in case the
+            learning rate must stay constant; otherwise, a scheduler can be passed which
+            will be stepped `on_update` by default (see `hook` argument).
+        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
+            Specifies when to step the optimizer's learning rate's scheduler to decay
+            its value (see `step` method also). This allows to vary the rate over the
+            learning iterations. The options are:
+             - `on_update` steps the learning rate after each agent's update
+             - `on_episode_end` steps the learning rate after each episode's end
+             - `on_timestep_end` steps the learning rate after each env's timestep.
+
+            By default, 'on_update' is selected.
+        max_percentage_update : float, optional
+            A positive float that specifies the maximum percentage change the learnable
+            parameters can experience in each update. For example,
+            `max_percentage_update=0.5` means that the parameters can be updated by up
+            to 50% of their current value. By default, it is set to `+inf`.
+        """
+        super().__init__(max_percentage_update)
+        if not isinstance(learning_rate, Scheduler):
+            learning_rate = NoScheduling[LrType](learning_rate)
+        self.lr_scheduler: Scheduler[LrType] = learning_rate
+        self._hook = hook
+        self._update_solver: cs.Function
+
+    @property
+    def hook(self) -> Optional[str]:
+        """Specifies to which callback to hook, i.e., when to step the learning rate's
+        scheduler to decay its value (see `step` method also). Can be `None` in case no
+        hook is needed."""
+        # return hook only if the learning rate scheduler requires to be stepped
+        return None if isinstance(self.lr_scheduler, NoScheduling) else self._hook
+
+    def step(self, *_, **__) -> None:
+        """Steps/decays the learning rate according to its scheduler."""
+        self.lr_scheduler.step()
+
+    def _init_update_solver(self) -> Optional[cs.Function]:
+        """Internal utility to initialize, if the learnable parameters are constrained,
+        a constrained update solver which, by default, is a QP. Otherwise, no solver is
+        required to perform the update.
+        """
+        if (
+            self.max_percentage_update == float("+inf")
+            and np.isneginf(self.learnable_parameters.lb).all()
+            and np.isposinf(self.learnable_parameters.ub).all()
+        ):
+            return None
+        n_params = self.learnable_parameters.size
+        qp = {"h": getattr(cs.Sparsity, self._hessian_sparsity)(n_params, n_params)}
+        opts = {
+            "error_on_fail": False,
+            "osqp": {
+                "verbose": False,
+                "polish": True,
+                "scaling": 20,
+                "eps_abs": 1e-9,
+                "eps_rel": 1e-9,
+                "eps_prim_inf": 1e-10,
+                "eps_dual_inf": 1e-10,
+                "max_iter": 6000,
+            },
+        }
+        return cs.conic(f"qpsol_{id(self)}", "osqp", qp, opts)
+
+    def update(
+        self,
+        gradient: npt.NDArray[np.floating],
+        hessian: Optional[npt.NDArray[np.floating]] = None,
+    ) -> Optional[str]:
+        """Computes the gradient update of the learnable parameters dictated by the
+        current RL algorithm.
+
+        Parameters
+        ----------
+        gradient : 1D array
+            The gradient of the learnable parameters.
+        hessian : None, or 2D array
+            The hessian of the learnable parameters. When the optimizer is firt-order,
+            it is expected to be `None` (as it is unused). When the optimizer is
+            second-order, it is expected to be a 2D array.
+
+        Returns
+        -------
+        status : str, optional
+            An optional string containing the status of the update, e.g., the status of
+            the QP solver, if used.
+        """
+        if self._order == 1:
+            theta_new, status = self._first_order_update(gradient)
+        else:
+            theta_new, status = self._second_order_update(gradient, hessian)
+        # theta_new = np.clip(
+        #     theta_new, self.learnable_parameters.lb, self.learnable_parameters.ub
+        # )
+        self.learnable_parameters.update_values(theta_new)
+        return status
+
+    def _first_order_update(
+        self, gradient: npt.NDArray[np.floating]
+    ) -> tuple[npt.NDArray[np.floating], Optional[str]]:
+        """Internally runs a first order update."""
+        raise NotImplementedError(
+            f"`{self.__class__.__name__}` optimizer does not implement "
+            "`_first_order_update`"
+        )
+
+    def _second_order_update(
+        self, gradient: npt.NDArray[np.floating], hessian: npt.NDArray[np.floating]
+    ) -> tuple[npt.NDArray[np.floating], Optional[str]]:
+        """Internally runs a second order update."""
+        raise NotImplementedError(
+            f"`{self.__class__.__name__}` optimizer does not implement "
+            "`_second_order_update`"
+        )
+
+    def __repr__(self) -> str:
+        cn = self.__class__.__name__
+        hookstr = "None" if self.hook is None else f"'{self.hook}'"
+        mp = self.max_percentage_update
+        return f"{cn}(lr={self.lr_scheduler},hook={hookstr},max%={mp})"
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/optim/gradient_descent.py` & `mpcrl-1.2.0rc4/src/mpcrl/optim/gradient_descent.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-from typing import Literal, Optional, Union
-
-import casadi as cs
-import numpy as np
-import numpy.typing as npt
-
-from ..core.schedulers import Scheduler
-from .gradient_based_optimizer import GradientBasedOptimizer, LrType, SymType
-
-
-class GradientDescent(GradientBasedOptimizer[SymType, LrType]):
-    """First-order Gradient descent optimizer, based on [1,2].
-
-    References
-    ----------
-    [1] Sutskever, I., Martens, J., Dahl, G. and Hinton, G., 2013, May. On the
-        importance of initialization and momentum in deep learning. In International
-        conference on machine learning (pp. 1139-1147). PMLR.
-    [2] SGD - PyTorch 2.1 documentation.
-        https://pytorch.org/docs/stable/generated/torch.optim.SGD.html
-    """
-
-    _order = 1
-    _hessian_sparsity = "diag"
-    """In GD, the hessian is at most diagonal, i.e., in case we have constraints."""
-
-    def __init__(
-        self,
-        learning_rate: Union[LrType, Scheduler[LrType]],
-        weight_decay: float = 0.0,
-        momentum: float = 0.0,
-        dampening: float = 0.0,
-        nesterov: bool = False,
-        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
-        max_percentage_update: float = float("+inf"),
-    ) -> None:
-        """Instantiates the optimizer.
-
-        Parameters
-        ----------
-        learning_rate : float/array, scheduler
-            The learning rate of the optimizer. A float/array can be passed in case the
-            learning rate must stay constant; otherwise, a scheduler can be passed which
-            will be stepped `on_update` by default (see `hook` argument).
-        weight_decay : float, optional
-            A positive float that specifies the decay of the learnable parameters in the
-            form of an L2 regularization term. By default, it is set to `0.0`, so no
-            decay/regularization takes place.
-        momentum : float, optional
-            A positive float that specifies the momentum factor. By default, it is set
-            to `0.0`, so no momentum is used.
-        dampening : float, optional
-            A positive float that specifies the dampening factor for the momentum. By
-            default, it is set to `0.0`, so no dampening is used.
-        nesterov : bool, optional
-            A boolean that specifies whether to use Nesterov momentum. By default, it is
-            set to `False`.
-        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
-            Specifies when to step the optimizer's learning rate's scheduler to decay
-            its value (see `step` method also). This allows to vary the rate over the
-            learning iterations. The options are:
-             - `on_update` steps the learning rate after each agent's update
-             - `on_episode_end` steps the learning rate after each episode's end
-             - `on_timestep_end` steps the learning rate after each env's timestep.
-
-            By default, 'on_update' is selected.
-        max_percentage_update : float, optional
-            A positive float that specifies the maximum percentage change the learnable
-            parameters can experience in each update. For example,
-            `max_percentage_update=0.5` means that the parameters can be updated by up
-            to 50% of their current value. By default, it is set to `+inf`. If
-            specified, the update becomes constrained and has to be solved as a QP,
-            which is inevitably slower than its unconstrained counterpart.
-        """
-        super().__init__(learning_rate, hook, max_percentage_update)
-        self.weight_decay = weight_decay
-        self.momentum = momentum
-        self.dampening = dampening
-        self.nesterov = nesterov
-        self._momentum_buffer = None
-
-    def _first_order_update(
-        self, gradient: npt.NDArray[np.floating]
-    ) -> tuple[npt.NDArray[np.floating], Optional[str]]:
-        theta = self.learnable_parameters.value
-
-        # compute candidate update
-        dtheta, self._momentum_buffer = _gd(
-            theta,
-            gradient,
-            self._momentum_buffer,
-            self.weight_decay,
-            self.momentum,
-            self.lr_scheduler.value,
-            self.dampening,
-            self.nesterov,
-        )
-
-        # if unconstrained, apply the update directly; otherwise, solve the QP
-        solver = self._update_solver
-        if solver is None:
-            return theta + dtheta, None
-        lbx, ubx = self._get_update_bounds(theta)
-        sol = solver(h=cs.DM.eye(theta.shape[0]), g=-dtheta, lbx=lbx, ubx=ubx)
-        dtheta = np.asarray(sol["x"].elements())
-        stats = solver.stats()
-        return theta + dtheta, None if stats["success"] else stats["return_status"]
-
-
-def _gd(
-    theta: np.ndarray,
-    g: np.ndarray,
-    momentum_buffer: Optional[np.ndarray],
-    weight_decay: float,
-    momentum: float,
-    lr: LrType,
-    dampening: float,
-    nesterov: bool,
-) -> tuple[np.ndarray, Optional[np.ndarray]]:
-    """Computes the update's change according to the gradient descent algorithm."""
-    if weight_decay > 0.0:
-        g += weight_decay * theta
-    if momentum > 0.0:
-        if momentum_buffer is None:
-            momentum_buffer = g.copy()
-        else:
-            momentum_buffer = momentum * momentum_buffer + (1 - dampening) * g
-        if nesterov:
-            g += momentum * momentum_buffer
-        else:
-            g = momentum_buffer
-    dtheta = -lr * g
-    return dtheta, momentum_buffer
+from typing import Literal, Optional, Union
+
+import casadi as cs
+import numpy as np
+import numpy.typing as npt
+
+from ..core.schedulers import Scheduler
+from .gradient_based_optimizer import GradientBasedOptimizer, LrType, SymType
+
+
+class GradientDescent(GradientBasedOptimizer[SymType, LrType]):
+    """First-order Gradient descent optimizer, based on [1,2].
+
+    References
+    ----------
+    [1] Sutskever, I., Martens, J., Dahl, G. and Hinton, G., 2013, May. On the
+        importance of initialization and momentum in deep learning. In International
+        conference on machine learning (pp. 1139-1147). PMLR.
+    [2] SGD - PyTorch 2.1 documentation.
+        https://pytorch.org/docs/stable/generated/torch.optim.SGD.html
+    """
+
+    _order = 1
+    _hessian_sparsity = "diag"
+    """In GD, the hessian is at most diagonal, i.e., in case we have constraints."""
+
+    def __init__(
+        self,
+        learning_rate: Union[LrType, Scheduler[LrType]],
+        weight_decay: float = 0.0,
+        momentum: float = 0.0,
+        dampening: float = 0.0,
+        nesterov: bool = False,
+        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
+        max_percentage_update: float = float("+inf"),
+    ) -> None:
+        """Instantiates the optimizer.
+
+        Parameters
+        ----------
+        learning_rate : float/array, scheduler
+            The learning rate of the optimizer. A float/array can be passed in case the
+            learning rate must stay constant; otherwise, a scheduler can be passed which
+            will be stepped `on_update` by default (see `hook` argument).
+        weight_decay : float, optional
+            A positive float that specifies the decay of the learnable parameters in the
+            form of an L2 regularization term. By default, it is set to `0.0`, so no
+            decay/regularization takes place.
+        momentum : float, optional
+            A positive float that specifies the momentum factor. By default, it is set
+            to `0.0`, so no momentum is used.
+        dampening : float, optional
+            A positive float that specifies the dampening factor for the momentum. By
+            default, it is set to `0.0`, so no dampening is used.
+        nesterov : bool, optional
+            A boolean that specifies whether to use Nesterov momentum. By default, it is
+            set to `False`.
+        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
+            Specifies when to step the optimizer's learning rate's scheduler to decay
+            its value (see `step` method also). This allows to vary the rate over the
+            learning iterations. The options are:
+             - `on_update` steps the learning rate after each agent's update
+             - `on_episode_end` steps the learning rate after each episode's end
+             - `on_timestep_end` steps the learning rate after each env's timestep.
+
+            By default, 'on_update' is selected.
+        max_percentage_update : float, optional
+            A positive float that specifies the maximum percentage change the learnable
+            parameters can experience in each update. For example,
+            `max_percentage_update=0.5` means that the parameters can be updated by up
+            to 50% of their current value. By default, it is set to `+inf`. If
+            specified, the update becomes constrained and has to be solved as a QP,
+            which is inevitably slower than its unconstrained counterpart.
+        """
+        super().__init__(learning_rate, hook, max_percentage_update)
+        self.weight_decay = weight_decay
+        self.momentum = momentum
+        self.dampening = dampening
+        self.nesterov = nesterov
+        self._momentum_buffer = None
+
+    def _first_order_update(
+        self, gradient: npt.NDArray[np.floating]
+    ) -> tuple[npt.NDArray[np.floating], Optional[str]]:
+        theta = self.learnable_parameters.value
+
+        # compute candidate update
+        dtheta, self._momentum_buffer = _gd(
+            theta,
+            gradient,
+            self._momentum_buffer,
+            self.weight_decay,
+            self.momentum,
+            self.lr_scheduler.value,
+            self.dampening,
+            self.nesterov,
+        )
+
+        # if unconstrained, apply the update directly; otherwise, solve the QP
+        solver = self._update_solver
+        if solver is None:
+            return theta + dtheta, None
+        lbx, ubx = self._get_update_bounds(theta)
+        sol = solver(h=cs.DM.eye(theta.shape[0]), g=-dtheta, lbx=lbx, ubx=ubx)
+        dtheta = np.asarray(sol["x"].elements())
+        stats = solver.stats()
+        return theta + dtheta, None if stats["success"] else stats["return_status"]
+
+
+def _gd(
+    theta: np.ndarray,
+    g: np.ndarray,
+    momentum_buffer: Optional[np.ndarray],
+    weight_decay: float,
+    momentum: float,
+    lr: LrType,
+    dampening: float,
+    nesterov: bool,
+) -> tuple[np.ndarray, Optional[np.ndarray]]:
+    """Computes the update's change according to the gradient descent algorithm."""
+    if weight_decay > 0.0:
+        g += weight_decay * theta
+    if momentum > 0.0:
+        if momentum_buffer is None:
+            momentum_buffer = g.copy()
+        else:
+            momentum_buffer = momentum * momentum_buffer + (1 - dampening) * g
+        if nesterov:
+            g += momentum * momentum_buffer
+        else:
+            g = momentum_buffer
+    dtheta = -lr * g
+    return dtheta, momentum_buffer
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/optim/gradient_free_optimizer.py` & `mpcrl-1.2.0rc4/src/mpcrl/optim/gradient_free_optimizer.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from abc import ABC, abstractmethod
-from typing import Optional, Union
-
-import numpy as np
-import numpy.typing as npt
-
-from .base_optimizer import BaseOptimizer, SymType
-
-
-class GradientFreeOptimizer(BaseOptimizer[SymType], ABC):
-    """Base class for gradient-free optimization algorithms, e.g., Bayesian
-    Optimization.
-
-    This optimizer adopts the ask-tell interface, i.e., it must implement the `ask` and
-    `tell` methods. The former allows the agent to ask for a new set of parameters to
-    evaluate, while the latter allows the agent to tell the optimizer the values of the
-    objective function(s) for the set of parameters it asked for.
-    """
-
-    prefers_dict: bool
-
-    @abstractmethod
-    def ask(
-        self,
-    ) -> tuple[Union[dict[str, npt.ArrayLike], npt.ArrayLike], Optional[str],]:
-        """Asks the learning agent for a new set of parameters to evaluate.
-
-        Returns
-        -------
-        dict of (str, 1d arrays) or a single 1d array
-            A dictionary of learnable parameter names and their corresponding values.
-            Or a single array that results from the concatenation of the parameter
-            values.
-        str, optional (default=None)
-            A string that specifies the status of the optimizer. This is useful to
-            communicate to the learning agent whether the optimization algorithm has
-            encountered, e.g., some error or failure.
-        """
-
-    @abstractmethod
-    def tell(
-        self,
-        values: Union[dict[str, npt.NDArray[np.floating]], npt.NDArray[np.floating]],
-        objective: Union[float, npt.NDArray[np.floating]],
-    ) -> None:
-        """Tells the learning agent the values of the objective function for the set of
-        parameters it asked for.
-
-        Parameters
-        ----------
-        values : dict of (str, 1d arrays) or a single 1d array
-            A dictionary of learnable parameter names and their corresponding values for
-            which the objective function(s) was (were) evaluated. Or a single array that
-            results from the concatenation of the parameter values. This depends on the
-            optimizer's `prefers_dict` class attribute.
-        objective : float or array
-            Value(s) of the objective function(s) for the set of parameters. Can be
-            single-objective or multi-objective.
-        """
+from abc import ABC, abstractmethod
+from typing import Optional, Union
+
+import numpy as np
+import numpy.typing as npt
+
+from .base_optimizer import BaseOptimizer, SymType
+
+
+class GradientFreeOptimizer(BaseOptimizer[SymType], ABC):
+    """Base class for gradient-free optimization algorithms, e.g., Bayesian
+    Optimization.
+
+    This optimizer adopts the ask-tell interface, i.e., it must implement the `ask` and
+    `tell` methods. The former allows the agent to ask for a new set of parameters to
+    evaluate, while the latter allows the agent to tell the optimizer the values of the
+    objective function(s) for the set of parameters it asked for.
+    """
+
+    prefers_dict: bool
+
+    @abstractmethod
+    def ask(
+        self,
+    ) -> tuple[Union[dict[str, npt.ArrayLike], npt.ArrayLike], Optional[str],]:
+        """Asks the learning agent for a new set of parameters to evaluate.
+
+        Returns
+        -------
+        dict of (str, 1d arrays) or a single 1d array
+            A dictionary of learnable parameter names and their corresponding values.
+            Or a single array that results from the concatenation of the parameter
+            values.
+        str, optional (default=None)
+            A string that specifies the status of the optimizer. This is useful to
+            communicate to the learning agent whether the optimization algorithm has
+            encountered, e.g., some error or failure.
+        """
+
+    @abstractmethod
+    def tell(
+        self,
+        values: Union[dict[str, npt.NDArray[np.floating]], npt.NDArray[np.floating]],
+        objective: Union[float, npt.NDArray[np.floating]],
+    ) -> None:
+        """Tells the learning agent the values of the objective function for the set of
+        parameters it asked for.
+
+        Parameters
+        ----------
+        values : dict of (str, 1d arrays) or a single 1d array
+            A dictionary of learnable parameter names and their corresponding values for
+            which the objective function(s) was (were) evaluated. Or a single array that
+            results from the concatenation of the parameter values. This depends on the
+            optimizer's `prefers_dict` class attribute.
+        objective : float or array
+            Value(s) of the objective function(s) for the set of parameters. Can be
+            single-objective or multi-objective.
+        """
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/optim/newton_method.py` & `mpcrl-1.2.0rc4/src/mpcrl/optim/newton_method.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-from typing import Any, Literal, Optional, Union
-
-import numpy as np
-import numpy.typing as npt
-from scipy.linalg import cho_solve
-
-from ..core.schedulers import Scheduler
-from ..util.math import cholesky_added_multiple_identities
-from .gradient_based_optimizer import GradientBasedOptimizer, LrType, SymType
-
-
-class NetwonMethod(GradientBasedOptimizer[SymType, LrType]):
-    """Netwon Method."""
-
-    _order = 2
-    _hessian_sparsity = "dense"
-
-    def __init__(
-        self,
-        learning_rate: Union[LrType, Scheduler[LrType]],
-        weight_decay: float = 0.0,
-        cho_before_update: bool = False,
-        cho_maxiter: int = 1000,
-        cho_solve_kwargs: Optional[dict[str, Any]] = None,
-        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
-        max_percentage_update: float = float("+inf"),
-    ) -> None:
-        """Instantiates the optimizer.
-
-        Parameters
-        ----------
-        learning_rate : float/array, scheduler
-            The learning rate of the optimizer. A float/array can be passed in case the
-            learning rate must stay constant; otherwise, a scheduler can be passed which
-            will be stepped `on_update` by default (see `hook` argument).
-        weight_decay : float, optional
-            A positive float that specifies the decay of the learnable parameters in the
-            form of an L2 regularization term. By default, it is set to `0.0`, so no
-            decay/regularization takes place.
-        cho_before_update : bool, optional
-            Whether to perform a Cholesky's factorization of the hessian in preparation
-            of each update. If `False`, the QP update's objective is
-            ```math
-                min 1/2 * dtheta' * H * dtheta + (lr * g)' * dtheta
-            ```
-            else, if `True`, the objective is
-            ```math
-                min 1/2 * ||dtheta||^2' + (lr * H^-1 * g)' * dtheta
-            ```
-            where the hessian linear system is performed via Cholesky's factorization.
-            Only relevant if the update is  constrained. By default, `False`.
-        cho_maxiter : int, optional
-            Maximum number of iterations in the Cholesky's factorization with additive
-            multiples of the identity to ensure positive definiteness of the hessian. By
-            default, `1000`.
-        cho_solve_kwargs : kwargs for `scipy.linalg.cho_solve`, optional
-            The optional kwargs to be passed to `scipy.linalg.cho_solve` to solve linear
-            systems with the hessian's Cholesky decomposition. If `None`, it is
-            equivalent to `cho_solve_kwargs = {'check_finite': False }`.
-        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
-            Specifies when to step the optimizer's learning rate's scheduler to decay
-            its value (see `step` method also). This allows to vary the rate over the
-            learning iterations. The options are:
-             - `on_update` steps the learning rate after each agent's update
-             - `on_episode_end` steps the learning rate after each episode's end
-             - `on_timestep_end` steps the learning rate after each env's timestep.
-
-            By default, 'on_update' is selected.
-        max_percentage_update : float, optional
-            A positive float that specifies the maximum percentage change the learnable
-            parameters can experience in each update. For example,
-            `max_percentage_update=0.5` means that the parameters can be updated by up
-            to 50% of their current value. By default, it is set to `+inf`. If
-            specified, the update becomes constrained and has to be solved as a QP,
-            which is inevitably slower than its unconstrained counterpart.
-        """
-        if cho_before_update:
-            self._hessian_sparsity = "diag"
-        super().__init__(learning_rate, hook, max_percentage_update)
-        self.weight_decay = weight_decay
-        self.cho_before_update = cho_before_update
-        self.cho_maxiter = cho_maxiter
-        if cho_solve_kwargs is None:
-            cho_solve_kwargs = {"check_finite": False}
-        self.cho_solve_kwargs = cho_solve_kwargs
-
-    def _second_order_update(
-        self, gradient: npt.NDArray[np.floating], hessian: npt.NDArray[np.floating]
-    ) -> tuple[npt.NDArray[np.floating], Optional[str]]:
-        theta = self.learnable_parameters.value
-        lr = self.lr_scheduler.value
-        w = self.weight_decay
-        cho_kw = self.cho_solve_kwargs
-        L = cholesky_added_multiple_identities(hessian, maxiter=self.cho_maxiter)
-
-        # if unconstrained, apply the update directly; otherwise, solve the QP
-        solver = self._update_solver
-        if solver is None:
-            dtheta = _nm_unconstrained(theta, gradient, L, lr, w, cho_kw)
-            return theta + dtheta, None
-        H, G = _nm_constrained(
-            theta, gradient, hessian, L, lr, w, self.cho_before_update, cho_kw
-        )
-        lbx, ubx = self._get_update_bounds(theta)
-        sol = solver(h=H, g=G, lbx=lbx, ubx=ubx)
-        dtheta = np.asarray(sol["x"].elements())
-        stats = solver.stats()
-        return theta + dtheta, None if stats["success"] else stats["return_status"]
-
-
-def _nm_unconstrained(
-    theta: np.ndarray,
-    g: np.ndarray,
-    L: np.ndarray,
-    lr: LrType,
-    weight_decay: float,
-    cho_solve_kwargs: dict,
-) -> np.ndarray:
-    """Computes the update's change according to the Netwon's Method."""
-    if weight_decay <= 0.0:
-        return -lr * cho_solve((L, True), g, **cho_solve_kwargs)
-    return -np.linalg.solve(
-        L @ L.T + weight_decay * np.eye(theta.shape[0]), lr * g + weight_decay * theta
-    )
-
-
-def _nm_constrained(
-    theta: np.ndarray,
-    g: np.ndarray,
-    H: np.ndarray,
-    L: np.ndarray,
-    lr: LrType,
-    weight_decay: float,
-    cho_before_update: bool,
-    cho_solve_kwargs: dict,
-) -> tuple[np.ndarray, np.ndarray]:
-    """Computes the update's change according to the Netwon's Method, which is solved
-    numerically due to the presence of constraints."""
-    if weight_decay <= 0.0:
-        if cho_before_update:
-            G = cho_solve((L, True), lr * g, **cho_solve_kwargs)
-            H = np.eye(theta.shape[0])
-        else:
-            G = lr * g
-            H = L @ L.T
-    else:
-        G = lr * g + weight_decay * theta
-        H = L @ L.T + weight_decay * np.eye(theta.shape[0])
-        if cho_before_update:
-            G = np.linalg.solve(H, G)
-            H = np.eye(theta.shape[0])
-    return H, G
+from typing import Any, Literal, Optional, Union
+
+import numpy as np
+import numpy.typing as npt
+from scipy.linalg import cho_solve
+
+from ..core.schedulers import Scheduler
+from ..util.math import cholesky_added_multiple_identities
+from .gradient_based_optimizer import GradientBasedOptimizer, LrType, SymType
+
+
+class NetwonMethod(GradientBasedOptimizer[SymType, LrType]):
+    """Netwon Method."""
+
+    _order = 2
+    _hessian_sparsity = "dense"
+
+    def __init__(
+        self,
+        learning_rate: Union[LrType, Scheduler[LrType]],
+        weight_decay: float = 0.0,
+        cho_before_update: bool = False,
+        cho_maxiter: int = 1000,
+        cho_solve_kwargs: Optional[dict[str, Any]] = None,
+        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
+        max_percentage_update: float = float("+inf"),
+    ) -> None:
+        """Instantiates the optimizer.
+
+        Parameters
+        ----------
+        learning_rate : float/array, scheduler
+            The learning rate of the optimizer. A float/array can be passed in case the
+            learning rate must stay constant; otherwise, a scheduler can be passed which
+            will be stepped `on_update` by default (see `hook` argument).
+        weight_decay : float, optional
+            A positive float that specifies the decay of the learnable parameters in the
+            form of an L2 regularization term. By default, it is set to `0.0`, so no
+            decay/regularization takes place.
+        cho_before_update : bool, optional
+            Whether to perform a Cholesky's factorization of the hessian in preparation
+            of each update. If `False`, the QP update's objective is
+            ```math
+                min 1/2 * dtheta' * H * dtheta + (lr * g)' * dtheta
+            ```
+            else, if `True`, the objective is
+            ```math
+                min 1/2 * ||dtheta||^2' + (lr * H^-1 * g)' * dtheta
+            ```
+            where the hessian linear system is performed via Cholesky's factorization.
+            Only relevant if the update is  constrained. By default, `False`.
+        cho_maxiter : int, optional
+            Maximum number of iterations in the Cholesky's factorization with additive
+            multiples of the identity to ensure positive definiteness of the hessian. By
+            default, `1000`.
+        cho_solve_kwargs : kwargs for `scipy.linalg.cho_solve`, optional
+            The optional kwargs to be passed to `scipy.linalg.cho_solve` to solve linear
+            systems with the hessian's Cholesky decomposition. If `None`, it is
+            equivalent to `cho_solve_kwargs = {'check_finite': False }`.
+        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
+            Specifies when to step the optimizer's learning rate's scheduler to decay
+            its value (see `step` method also). This allows to vary the rate over the
+            learning iterations. The options are:
+             - `on_update` steps the learning rate after each agent's update
+             - `on_episode_end` steps the learning rate after each episode's end
+             - `on_timestep_end` steps the learning rate after each env's timestep.
+
+            By default, 'on_update' is selected.
+        max_percentage_update : float, optional
+            A positive float that specifies the maximum percentage change the learnable
+            parameters can experience in each update. For example,
+            `max_percentage_update=0.5` means that the parameters can be updated by up
+            to 50% of their current value. By default, it is set to `+inf`. If
+            specified, the update becomes constrained and has to be solved as a QP,
+            which is inevitably slower than its unconstrained counterpart.
+        """
+        if cho_before_update:
+            self._hessian_sparsity = "diag"
+        super().__init__(learning_rate, hook, max_percentage_update)
+        self.weight_decay = weight_decay
+        self.cho_before_update = cho_before_update
+        self.cho_maxiter = cho_maxiter
+        if cho_solve_kwargs is None:
+            cho_solve_kwargs = {"check_finite": False}
+        self.cho_solve_kwargs = cho_solve_kwargs
+
+    def _second_order_update(
+        self, gradient: npt.NDArray[np.floating], hessian: npt.NDArray[np.floating]
+    ) -> tuple[npt.NDArray[np.floating], Optional[str]]:
+        theta = self.learnable_parameters.value
+        lr = self.lr_scheduler.value
+        w = self.weight_decay
+        cho_kw = self.cho_solve_kwargs
+        L = cholesky_added_multiple_identities(hessian, maxiter=self.cho_maxiter)
+
+        # if unconstrained, apply the update directly; otherwise, solve the QP
+        solver = self._update_solver
+        if solver is None:
+            dtheta = _nm_unconstrained(theta, gradient, L, lr, w, cho_kw)
+            return theta + dtheta, None
+        H, G = _nm_constrained(
+            theta, gradient, hessian, L, lr, w, self.cho_before_update, cho_kw
+        )
+        lbx, ubx = self._get_update_bounds(theta)
+        sol = solver(h=H, g=G, lbx=lbx, ubx=ubx)
+        dtheta = np.asarray(sol["x"].elements())
+        stats = solver.stats()
+        return theta + dtheta, None if stats["success"] else stats["return_status"]
+
+
+def _nm_unconstrained(
+    theta: np.ndarray,
+    g: np.ndarray,
+    L: np.ndarray,
+    lr: LrType,
+    weight_decay: float,
+    cho_solve_kwargs: dict,
+) -> np.ndarray:
+    """Computes the update's change according to the Netwon's Method."""
+    if weight_decay <= 0.0:
+        return -lr * cho_solve((L, True), g, **cho_solve_kwargs)
+    return -np.linalg.solve(
+        L @ L.T + weight_decay * np.eye(theta.shape[0]), lr * g + weight_decay * theta
+    )
+
+
+def _nm_constrained(
+    theta: np.ndarray,
+    g: np.ndarray,
+    H: np.ndarray,
+    L: np.ndarray,
+    lr: LrType,
+    weight_decay: float,
+    cho_before_update: bool,
+    cho_solve_kwargs: dict,
+) -> tuple[np.ndarray, np.ndarray]:
+    """Computes the update's change according to the Netwon's Method, which is solved
+    numerically due to the presence of constraints."""
+    if weight_decay <= 0.0:
+        if cho_before_update:
+            G = cho_solve((L, True), lr * g, **cho_solve_kwargs)
+            H = np.eye(theta.shape[0])
+        else:
+            G = lr * g
+            H = L @ L.T
+    else:
+        G = lr * g + weight_decay * theta
+        H = L @ L.T + weight_decay * np.eye(theta.shape[0])
+        if cho_before_update:
+            G = np.linalg.solve(H, G)
+            H = np.eye(theta.shape[0])
+    return H, G
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/optim/rmsprop.py` & `mpcrl-1.2.0rc4/src/mpcrl/optim/rmsprop.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-from typing import Literal, Optional, Union
-
-import casadi as cs
-import numpy as np
-import numpy.typing as npt
-
-from ..core.parameters import LearnableParametersDict, SymType
-from ..core.schedulers import Scheduler
-from .gradient_based_optimizer import GradientBasedOptimizer, LrType
-
-
-class RMSprop(GradientBasedOptimizer[SymType, LrType]):
-    """RMSprop optimizer, based on [1,2].
-
-    References
-    ----------
-    [1] Geoffrey Hinton, Nitish Srivastava, and Kevin Swersky. Neural networks for
-        machine learning lecture 6a overview of mini-batch gradient descent. page 14,
-        2012.
-    [2] RMSprop - PyTorch 2.1 documentation.
-        https://pytorch.org/docs/stable/generated/torch.optim.RMSprop.html
-    """
-
-    _order = 1
-    _hessian_sparsity = "diag"
-    """In RMSprop, hessian is at most diagonal, i.e., in case we have constraints."""
-
-    def __init__(
-        self,
-        learning_rate: Union[LrType, Scheduler[LrType]],
-        alpha: float = 0.99,
-        eps: float = 1e-8,
-        weight_decay: float = 0.0,
-        momentum: float = 0.0,
-        centered: bool = False,
-        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
-        max_percentage_update: float = float("+inf"),
-    ) -> None:
-        """Instantiates the optimizer.
-
-        Parameters
-        ----------
-        learning_rate : float/array, scheduler
-            The learning rate of the optimizer. A float/array can be passed in case the
-            learning rate must stay constant; otherwise, a scheduler can be passed which
-            will be stepped `on_update` by default (see `hook` argument).
-        alpha : float, optional
-            A positive float that specifies the decay rate of the running average of the
-            gradient. By default, it is set to `0.99`.
-        eps : float, optional
-            Term added to the denominator to improve numerical stability. By default, it
-            is set to `1e-8`.
-        weight_decay : float, optional
-            A positive float that specifies the decay of the learnable parameters in the
-            form of an L2 regularization term. By default, it is set to `0.0`, so no
-            decay/regularization takes place.
-        momentum : float, optional
-            A positive float that specifies the momentum factor. By default, it is set
-            to `0.0`, so no momentum is used.
-        centered : bool, optional
-            If `True`, compute the centered RMSProp, i.e., the gradient is normalized by
-            an estimation of its variance.
-        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
-            Specifies when to step the optimizer's learning rate's scheduler to decay
-            its value (see `step` method also). This allows to vary the rate over the
-            learning iterations. The options are:
-             - `on_update` steps the learning rate after each agent's update
-             - `on_episode_end` steps the learning rate after each episode's end
-             - `on_timestep_end` steps the learning rate after each env's timestep.
-
-            By default, 'on_update' is selected.
-        max_percentage_update : float, optional
-            A positive float that specifies the maximum percentage change the learnable
-            parameters can experience in each update. For example,
-            `max_percentage_update=0.5` means that the parameters can be updated by up
-            to 50% of their current value. By default, it is set to `+inf`. If
-            specified, the update becomes constrained and has to be solved as a QP,
-            which is inevitably slower than its unconstrained counterpart.
-        """
-        super().__init__(learning_rate, hook, max_percentage_update)
-        self.weight_decay = weight_decay
-        self.alpha = alpha
-        self.eps = eps
-        self.momentum = momentum
-        self.centered = centered
-
-    def set_learnable_parameters(self, pars: LearnableParametersDict[SymType]) -> None:
-        super().set_learnable_parameters(pars)
-        # initialize also running averages
-        n = pars.size
-        self._square_avg = np.zeros(n, dtype=float)
-        self._grad_avg = np.zeros(n, dtype=float) if self.centered else None
-        self._momentum_buf = np.zeros(n, dtype=float) if self.momentum > 0.0 else None
-
-    def _first_order_update(
-        self, gradient: npt.NDArray[np.floating]
-    ) -> tuple[npt.NDArray[np.floating], Optional[str]]:
-        theta = self.learnable_parameters.value
-
-        # compute candidate update
-        weight_decay = self.weight_decay
-        lr = self.lr_scheduler.value
-        if weight_decay > 0.0:
-            gradient = gradient + weight_decay * theta
-        dtheta, self._square_avg, self._grad_avg, self._momentum_buf = _rmsprop(
-            gradient,
-            self._square_avg,
-            lr,
-            self.alpha,
-            self.eps,
-            self.centered,
-            self._grad_avg,
-            self.momentum,
-            self._momentum_buf,
-        )
-
-        # if unconstrained, apply the update directly; otherwise, solve the QP
-        solver = self._update_solver
-        if solver is None:
-            return theta + dtheta, None
-        lbx, ubx = self._get_update_bounds(theta)
-        sol = solver(h=cs.DM.eye(theta.shape[0]), g=-dtheta, lbx=lbx, ubx=ubx)
-        dtheta = np.asarray(sol["x"].elements())
-        stats = solver.stats()
-        return theta + dtheta, None if stats["success"] else stats["return_status"]
-
-
-def _rmsprop(
-    grad: np.ndarray,
-    square_avg: np.ndarray,
-    lr: LrType,
-    alpha: float,
-    eps: float,
-    centered: bool,
-    grad_avg: Optional[np.ndarray],
-    momentum: float,
-    momentum_buffer: Optional[np.ndarray],
-) -> tuple[np.ndarray, np.ndarray, Optional[np.ndarray], Optional[np.ndarray]]:
-    """Computes the update's change according to Adam algorithm."""
-    square_avg = alpha * square_avg + (1 - alpha) * np.square(grad)
-
-    if centered:
-        grad_avg = alpha * grad_avg + (1 - alpha) * grad
-        avg = np.sqrt(square_avg - np.square(grad_avg))
-    else:
-        avg = np.sqrt(square_avg)
-    avg += eps
-
-    if momentum > 0.0:
-        momentum_buffer = momentum * momentum_buffer + grad / avg
-        dtheta = -lr * momentum_buffer
-    else:
-        dtheta = -lr * grad / avg
-    return dtheta, square_avg, grad_avg, momentum_buffer
+from typing import Literal, Optional, Union
+
+import casadi as cs
+import numpy as np
+import numpy.typing as npt
+
+from ..core.parameters import LearnableParametersDict, SymType
+from ..core.schedulers import Scheduler
+from .gradient_based_optimizer import GradientBasedOptimizer, LrType
+
+
+class RMSprop(GradientBasedOptimizer[SymType, LrType]):
+    """RMSprop optimizer, based on [1,2].
+
+    References
+    ----------
+    [1] Geoffrey Hinton, Nitish Srivastava, and Kevin Swersky. Neural networks for
+        machine learning lecture 6a overview of mini-batch gradient descent. page 14,
+        2012.
+    [2] RMSprop - PyTorch 2.1 documentation.
+        https://pytorch.org/docs/stable/generated/torch.optim.RMSprop.html
+    """
+
+    _order = 1
+    _hessian_sparsity = "diag"
+    """In RMSprop, hessian is at most diagonal, i.e., in case we have constraints."""
+
+    def __init__(
+        self,
+        learning_rate: Union[LrType, Scheduler[LrType]],
+        alpha: float = 0.99,
+        eps: float = 1e-8,
+        weight_decay: float = 0.0,
+        momentum: float = 0.0,
+        centered: bool = False,
+        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
+        max_percentage_update: float = float("+inf"),
+    ) -> None:
+        """Instantiates the optimizer.
+
+        Parameters
+        ----------
+        learning_rate : float/array, scheduler
+            The learning rate of the optimizer. A float/array can be passed in case the
+            learning rate must stay constant; otherwise, a scheduler can be passed which
+            will be stepped `on_update` by default (see `hook` argument).
+        alpha : float, optional
+            A positive float that specifies the decay rate of the running average of the
+            gradient. By default, it is set to `0.99`.
+        eps : float, optional
+            Term added to the denominator to improve numerical stability. By default, it
+            is set to `1e-8`.
+        weight_decay : float, optional
+            A positive float that specifies the decay of the learnable parameters in the
+            form of an L2 regularization term. By default, it is set to `0.0`, so no
+            decay/regularization takes place.
+        momentum : float, optional
+            A positive float that specifies the momentum factor. By default, it is set
+            to `0.0`, so no momentum is used.
+        centered : bool, optional
+            If `True`, compute the centered RMSProp, i.e., the gradient is normalized by
+            an estimation of its variance.
+        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
+            Specifies when to step the optimizer's learning rate's scheduler to decay
+            its value (see `step` method also). This allows to vary the rate over the
+            learning iterations. The options are:
+             - `on_update` steps the learning rate after each agent's update
+             - `on_episode_end` steps the learning rate after each episode's end
+             - `on_timestep_end` steps the learning rate after each env's timestep.
+
+            By default, 'on_update' is selected.
+        max_percentage_update : float, optional
+            A positive float that specifies the maximum percentage change the learnable
+            parameters can experience in each update. For example,
+            `max_percentage_update=0.5` means that the parameters can be updated by up
+            to 50% of their current value. By default, it is set to `+inf`. If
+            specified, the update becomes constrained and has to be solved as a QP,
+            which is inevitably slower than its unconstrained counterpart.
+        """
+        super().__init__(learning_rate, hook, max_percentage_update)
+        self.weight_decay = weight_decay
+        self.alpha = alpha
+        self.eps = eps
+        self.momentum = momentum
+        self.centered = centered
+
+    def set_learnable_parameters(self, pars: LearnableParametersDict[SymType]) -> None:
+        super().set_learnable_parameters(pars)
+        # initialize also running averages
+        n = pars.size
+        self._square_avg = np.zeros(n, dtype=float)
+        self._grad_avg = np.zeros(n, dtype=float) if self.centered else None
+        self._momentum_buf = np.zeros(n, dtype=float) if self.momentum > 0.0 else None
+
+    def _first_order_update(
+        self, gradient: npt.NDArray[np.floating]
+    ) -> tuple[npt.NDArray[np.floating], Optional[str]]:
+        theta = self.learnable_parameters.value
+
+        # compute candidate update
+        weight_decay = self.weight_decay
+        lr = self.lr_scheduler.value
+        if weight_decay > 0.0:
+            gradient = gradient + weight_decay * theta
+        dtheta, self._square_avg, self._grad_avg, self._momentum_buf = _rmsprop(
+            gradient,
+            self._square_avg,
+            lr,
+            self.alpha,
+            self.eps,
+            self.centered,
+            self._grad_avg,
+            self.momentum,
+            self._momentum_buf,
+        )
+
+        # if unconstrained, apply the update directly; otherwise, solve the QP
+        solver = self._update_solver
+        if solver is None:
+            return theta + dtheta, None
+        lbx, ubx = self._get_update_bounds(theta)
+        sol = solver(h=cs.DM.eye(theta.shape[0]), g=-dtheta, lbx=lbx, ubx=ubx)
+        dtheta = np.asarray(sol["x"].elements())
+        stats = solver.stats()
+        return theta + dtheta, None if stats["success"] else stats["return_status"]
+
+
+def _rmsprop(
+    grad: np.ndarray,
+    square_avg: np.ndarray,
+    lr: LrType,
+    alpha: float,
+    eps: float,
+    centered: bool,
+    grad_avg: Optional[np.ndarray],
+    momentum: float,
+    momentum_buffer: Optional[np.ndarray],
+) -> tuple[np.ndarray, np.ndarray, Optional[np.ndarray], Optional[np.ndarray]]:
+    """Computes the update's change according to Adam algorithm."""
+    square_avg = alpha * square_avg + (1 - alpha) * np.square(grad)
+
+    if centered:
+        grad_avg = alpha * grad_avg + (1 - alpha) * grad
+        avg = np.sqrt(square_avg - np.square(grad_avg))
+    else:
+        avg = np.sqrt(square_avg)
+    avg += eps
+
+    if momentum > 0.0:
+        momentum_buffer = momentum * momentum_buffer + grad / avg
+        dtheta = -lr * momentum_buffer
+    else:
+        dtheta = -lr * grad / avg
+    return dtheta, square_avg, grad_avg, momentum_buffer
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/util/control.py` & `mpcrl-1.2.0rc4/src/mpcrl/util/control.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-from typing import Callable, Optional, TypeVar
-
-import numpy as np
-import numpy.typing as npt
-from scipy.linalg import solve_discrete_are
-
-T = TypeVar("T")
-
-
-def dlqr(
-    A: npt.NDArray[np.floating],
-    B: npt.NDArray[np.floating],
-    Q: npt.NDArray[np.floating],
-    R: npt.NDArray[np.floating],
-    M: Optional[npt.NDArray[np.floating]] = None,
-) -> tuple[npt.NDArray[np.floating], npt.NDArray[np.floating]]:
-    """Get the discrete-time LQR for the given system. Stage costs are
-    ```
-        x'Qx + 2*x'Mu + u'Ru
-    ```
-    with `M = 0`, if not provided.
-
-    Parameters
-    ----------
-    A : array
-        State matrix.
-    B : array
-        Control input matrix.
-    Q : array
-        State weighting matrix.
-    R : array
-        Control input weighting matrix.
-    M : array, optional
-        Mixed state-input weighting matrix, by default None.
-
-    Returns
-    -------
-    tuple of two arrays
-        Returns the optimal state feedback matrix `K` and the quadratic terminal
-        cost-to-go matrix `P`.
-
-    Note
-    ----
-    Inspired by
-    https://bitbucket.org/rawlings-group/mpc-tools-casadi/src/master/mpctools/util.py.
-    """
-    if M is not None:
-        RinvMT = np.linalg.solve(R, M.T)
-        Atilde = A - B.dot(RinvMT)
-        Qtilde = Q - M.dot(RinvMT)
-    else:
-        Atilde = A
-        Qtilde = Q
-        M = np.zeros(B.shape)
-    P = solve_discrete_are(Atilde, B, Qtilde, R)
-    K = np.linalg.solve(B.T.dot(P).dot(B) + R, B.T.dot(P).dot(A) + M.T)
-    return K, P
-
-
-def rk4(f: Callable[[T], T], x0: T, dt: float = 1, M: int = 1) -> T:
-    """Computes the Runge-Kutta 4 integration of the given function `f` with initial
-    state x0.
-
-    Parameters
-    ----------
-    f : Callable[[casadi or array], casadi or array]
-        A function that takes a state as input and returns the derivative of the state,
-        i.e., continuous-time dynamics.
-    x0 : casadi or array
-        The initial state. Must be compatible as argument to `f`.
-    dt : float, optional
-        The discretization timestep, by default `1`.
-    M : int, optional
-        How many RK4 steps to take in one `dt` interval, by default `1`.
-
-    Returns
-    -------
-    new state : casadi or array
-        The new state after `dt` time, according to the discretization.
-
-    Note
-    ----
-    Inspired by
-    https://bitbucket.org/rawlings-group/mpc-tools-casadi/src/master/mpctools/util.py.
-    """
-    dt /= M
-    x = x0
-    for _ in range(M):
-        k1 = f(x)
-        k2 = f(x + k1 * dt / 2)  # type: ignore
-        k3 = f(x + k2 * dt / 2)  # type: ignore
-        k4 = f(x + k3 * dt)  # type: ignore
-        x = x + (k1 + 2 * k2 + 2 * k3 + k4) * dt / 6  # type: ignore
-    return x
+from typing import Callable, Optional, TypeVar
+
+import numpy as np
+import numpy.typing as npt
+from scipy.linalg import solve_discrete_are
+
+T = TypeVar("T")
+
+
+def dlqr(
+    A: npt.NDArray[np.floating],
+    B: npt.NDArray[np.floating],
+    Q: npt.NDArray[np.floating],
+    R: npt.NDArray[np.floating],
+    M: Optional[npt.NDArray[np.floating]] = None,
+) -> tuple[npt.NDArray[np.floating], npt.NDArray[np.floating]]:
+    """Get the discrete-time LQR for the given system. Stage costs are
+    ```
+        x'Qx + 2*x'Mu + u'Ru
+    ```
+    with `M = 0`, if not provided.
+
+    Parameters
+    ----------
+    A : array
+        State matrix.
+    B : array
+        Control input matrix.
+    Q : array
+        State weighting matrix.
+    R : array
+        Control input weighting matrix.
+    M : array, optional
+        Mixed state-input weighting matrix, by default None.
+
+    Returns
+    -------
+    tuple of two arrays
+        Returns the optimal state feedback matrix `K` and the quadratic terminal
+        cost-to-go matrix `P`.
+
+    Note
+    ----
+    Inspired by
+    https://bitbucket.org/rawlings-group/mpc-tools-casadi/src/master/mpctools/util.py.
+    """
+    if M is not None:
+        RinvMT = np.linalg.solve(R, M.T)
+        Atilde = A - B.dot(RinvMT)
+        Qtilde = Q - M.dot(RinvMT)
+    else:
+        Atilde = A
+        Qtilde = Q
+        M = np.zeros(B.shape)
+    P = solve_discrete_are(Atilde, B, Qtilde, R)
+    K = np.linalg.solve(B.T.dot(P).dot(B) + R, B.T.dot(P).dot(A) + M.T)
+    return K, P
+
+
+def rk4(f: Callable[[T], T], x0: T, dt: float = 1, M: int = 1) -> T:
+    """Computes the Runge-Kutta 4 integration of the given function `f` with initial
+    state x0.
+
+    Parameters
+    ----------
+    f : Callable[[casadi or array], casadi or array]
+        A function that takes a state as input and returns the derivative of the state,
+        i.e., continuous-time dynamics.
+    x0 : casadi or array
+        The initial state. Must be compatible as argument to `f`.
+    dt : float, optional
+        The discretization timestep, by default `1`.
+    M : int, optional
+        How many RK4 steps to take in one `dt` interval, by default `1`.
+
+    Returns
+    -------
+    new state : casadi or array
+        The new state after `dt` time, according to the discretization.
+
+    Note
+    ----
+    Inspired by
+    https://bitbucket.org/rawlings-group/mpc-tools-casadi/src/master/mpctools/util.py.
+    """
+    dt /= M
+    x = x0
+    for _ in range(M):
+        k1 = f(x)
+        k2 = f(x + k1 * dt / 2)  # type: ignore
+        k3 = f(x + k2 * dt / 2)  # type: ignore
+        k4 = f(x + k3 * dt)  # type: ignore
+        x = x + (k1 + 2 * k2 + 2 * k3 + k4) * dt / 6  # type: ignore
+    return x
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/util/iters.py` & `mpcrl-1.2.0rc4/src/mpcrl/util/iters.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from collections.abc import Iterator
-from itertools import chain, cycle, repeat
-
-
-def bool_cycle(frequency: int, starts_with: bool = False) -> Iterator[bool]:
-    """Creates an infinite iterator which cycles via boolean values, where `True`
-    appears with the given frequency.
-
-    Parameters
-    ----------
-    frequency : int
-        A positive int specifing the frequency at which `True` appears.
-    starts_with : bool, optional
-        Whether the first value should be `True` or `False`. By default `False`.
-
-    Returns
-    ------
-    Iterator of bool
-        An iterator with the given frequency of `True`.
-    """
-    iterator = cycle(chain(repeat(False, frequency - 1), (True,)))
-    if starts_with:
-        iterator = chain((True,), iterator)
-    return iterator
+from collections.abc import Iterator
+from itertools import chain, cycle, repeat
+
+
+def bool_cycle(frequency: int, starts_with: bool = False) -> Iterator[bool]:
+    """Creates an infinite iterator which cycles via boolean values, where `True`
+    appears with the given frequency.
+
+    Parameters
+    ----------
+    frequency : int
+        A positive int specifing the frequency at which `True` appears.
+    starts_with : bool, optional
+        Whether the first value should be `True` or `False`. By default `False`.
+
+    Returns
+    ------
+    Iterator of bool
+        An iterator with the given frequency of `True`.
+    """
+    iterator = cycle(chain(repeat(False, frequency - 1), (True,)))
+    if starts_with:
+        iterator = chain((True,), iterator)
+    return iterator
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/util/math.py` & `mpcrl-1.2.0rc4/src/mpcrl/util/math.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-from itertools import combinations
-from typing import Union
-
-import casadi as cs
-import numpy as np
-import numpy.typing as npt
-from csnlp.util.math import prod
-from scipy.special import comb
-
-
-def summarize_array(
-    a: npt.NDArray[np.floating], precision: int = 3, ddof: int = 0
-) -> str:
-    """Summarizes the stats of a given array.
-
-    Parameters
-    ----------
-    a : array
-        The numerical array to summarize.
-    precision : int, optional
-        The decimal precision, by default 3.
-    ddof : int, optional
-        Degrees of freedom used to compute the standard deviation, by default 0.
-
-    Returns
-    -------
-    str
-        The summarizing string.
-    """
-    s = a.shape
-    mean = a.mean()
-    std = a.std(ddof=ddof)
-    min = a.min()
-    max = a.max()
-    return (
-        f"s={s} x∈[{min:.{precision}f}, {max:.{precision}f}] "
-        f"μ={mean:.{precision}f} σ={std:.{precision}f}"
-    )
-
-
-def cholesky_added_multiple_identities(
-    A: npt.NDArray[np.floating], beta: float = 1e-3, maxiter: int = 1000
-) -> npt.NDArray[np.floating]:
-    """Lower Cholesky factorization with added multiple of the identity matrix to ensure
-    positive-definitiveness [1, Algorithm 3.3].
-
-    Parameters
-    ----------
-    A : array of double
-        The matrix to compute the cholesky factorization of.
-    beta : float, optional
-        Initial tolerance of the algorithm, by default 1e-3.
-    maxiter : int, optional
-        Maximum iterations of the algorithm, by default 1000.
-
-    Returns
-    -------
-    array of double
-        The lower cholesky factorization of the modified A (with the addition of
-        identity matrices to ensure that it is positive-definite).
-
-    Raises
-    ------
-    ValueError
-        If the factorization is unsuccessful for the maximum number of iterations.
-
-    References
-    ----------
-    [1] J. Nocedal, S. Wright. 2006. Numerical Optimization. Springer.
-    """
-    a_min = np.diag(A).min()
-    tau = 0 if a_min > 0 else -a_min + beta
-    identity = np.eye(A.shape[0])
-    for _ in range(maxiter):
-        try:
-            return np.linalg.cholesky(A + tau * identity)
-        except np.linalg.LinAlgError:
-            tau = max(1.05 * tau, beta)
-    raise ValueError("Maximum iterations reached.")
-
-
-def nchoosek(n: Union[int, npt.ArrayLike], k: int) -> Union[int, np.ndarray]:
-    """Emulates the `nchoosek` function from Matlab. Returns the binomial coefficient,
-    i.e.,  the number of combinations of `n` items taken `k` at a time. If `n` is an
-    array, then it is flatten and all possible combinations of its elements are
-    returned.
-
-    Parameters
-    ----------
-    n : int or array_like
-        Number of elements or array of elements to choose from.
-    k : int
-        Number of elements to choose.
-
-    Returns
-    -------
-    int or array
-        Depending on the type of input `n`, the output is either the total number of
-        combinations or the combinations in a matrix.
-    """
-    return (
-        comb(n, k, True)
-        if isinstance(n, int)
-        else np.row_stack(list(combinations(np.asarray(n).reshape(-1), k)))
-    )
-
-
-def monomial_powers(d: int, k: int) -> npt.NDArray[np.int64]:
-    """Computes the powers of all `d`-dimensional monomials of degree `k`.
-
-    Parameters
-    ----------
-    d : int
-        The number of monomial elements.
-    k : int
-        The degree of each monomial.
-
-    Returns
-    -------
-    array of ints
-        An array containing in each row the power of each index in order to obtain the
-        desired monomial of power `k`.
-    """
-    m = nchoosek(k + d - 1, d - 1)
-    dividers = np.column_stack(
-        (
-            np.zeros((m, 1), int),
-            np.row_stack(nchoosek(np.arange(1, k + d), d - 1)),
-            np.full((m, 1), k + d, int),
-        )
-    )
-    return np.flipud(np.diff(dividers, axis=1) - 1).astype(int)
-
-
-def monomials_basis_function(n_in: int, mindegree: int, maxdegree: int) -> cs.Function:
-    """Creates a function made of monomials as bases.
-
-    Parameters
-    ----------
-    ns : int
-        Number of states.
-    mindegree : int
-        Minimum degree of monomials (included).
-    maxdegree : int
-        Maximum degree of monomials (included).
-
-    Returns
-    -------
-    casadi.Function
-        A casadi function of the form `Phi(s)`, where `s` is the input and `Phi` the
-        basis vector.
-    """
-    s = cs.SX.sym("x", n_in, 1)  # prod is faster with SX, and during runtime
-    y = cs.vertcat(
-        *(
-            prod(s**p)
-            for k in range(mindegree, maxdegree + 1)
-            for p in monomial_powers(n_in, k)
-        )
-    )
-    return cs.Function("Phi", (s,), (y,), ("s",), ("Phi(s)",), {"cse": True})
+from itertools import combinations
+from typing import Union
+
+import casadi as cs
+import numpy as np
+import numpy.typing as npt
+from csnlp.util.math import prod
+from scipy.special import comb
+
+
+def summarize_array(
+    a: npt.NDArray[np.floating], precision: int = 3, ddof: int = 0
+) -> str:
+    """Summarizes the stats of a given array.
+
+    Parameters
+    ----------
+    a : array
+        The numerical array to summarize.
+    precision : int, optional
+        The decimal precision, by default 3.
+    ddof : int, optional
+        Degrees of freedom used to compute the standard deviation, by default 0.
+
+    Returns
+    -------
+    str
+        The summarizing string.
+    """
+    s = a.shape
+    mean = a.mean()
+    std = a.std(ddof=ddof)
+    min = a.min()
+    max = a.max()
+    return (
+        f"s={s} x∈[{min:.{precision}f}, {max:.{precision}f}] "
+        f"μ={mean:.{precision}f} σ={std:.{precision}f}"
+    )
+
+
+def cholesky_added_multiple_identities(
+    A: npt.NDArray[np.floating], beta: float = 1e-3, maxiter: int = 1000
+) -> npt.NDArray[np.floating]:
+    """Lower Cholesky factorization with added multiple of the identity matrix to ensure
+    positive-definitiveness [1, Algorithm 3.3].
+
+    Parameters
+    ----------
+    A : array of double
+        The matrix to compute the cholesky factorization of.
+    beta : float, optional
+        Initial tolerance of the algorithm, by default 1e-3.
+    maxiter : int, optional
+        Maximum iterations of the algorithm, by default 1000.
+
+    Returns
+    -------
+    array of double
+        The lower cholesky factorization of the modified A (with the addition of
+        identity matrices to ensure that it is positive-definite).
+
+    Raises
+    ------
+    ValueError
+        If the factorization is unsuccessful for the maximum number of iterations.
+
+    References
+    ----------
+    [1] J. Nocedal, S. Wright. 2006. Numerical Optimization. Springer.
+    """
+    a_min = np.diag(A).min()
+    tau = 0 if a_min > 0 else -a_min + beta
+    identity = np.eye(A.shape[0])
+    for _ in range(maxiter):
+        try:
+            return np.linalg.cholesky(A + tau * identity)
+        except np.linalg.LinAlgError:
+            tau = max(1.05 * tau, beta)
+    raise ValueError("Maximum iterations reached.")
+
+
+def nchoosek(n: Union[int, npt.ArrayLike], k: int) -> Union[int, np.ndarray]:
+    """Emulates the `nchoosek` function from Matlab. Returns the binomial coefficient,
+    i.e.,  the number of combinations of `n` items taken `k` at a time. If `n` is an
+    array, then it is flatten and all possible combinations of its elements are
+    returned.
+
+    Parameters
+    ----------
+    n : int or array_like
+        Number of elements or array of elements to choose from.
+    k : int
+        Number of elements to choose.
+
+    Returns
+    -------
+    int or array
+        Depending on the type of input `n`, the output is either the total number of
+        combinations or the combinations in a matrix.
+    """
+    return (
+        comb(n, k, True)
+        if isinstance(n, int)
+        else np.row_stack(list(combinations(np.asarray(n).reshape(-1), k)))
+    )
+
+
+def monomial_powers(d: int, k: int) -> npt.NDArray[np.int64]:
+    """Computes the powers of all `d`-dimensional monomials of degree `k`.
+
+    Parameters
+    ----------
+    d : int
+        The number of monomial elements.
+    k : int
+        The degree of each monomial.
+
+    Returns
+    -------
+    array of ints
+        An array containing in each row the power of each index in order to obtain the
+        desired monomial of power `k`.
+    """
+    m = nchoosek(k + d - 1, d - 1)
+    dividers = np.column_stack(
+        (
+            np.zeros((m, 1), int),
+            np.row_stack(nchoosek(np.arange(1, k + d), d - 1)),
+            np.full((m, 1), k + d, int),
+        )
+    )
+    return np.flipud(np.diff(dividers, axis=1) - 1).astype(int)
+
+
+def monomials_basis_function(n_in: int, mindegree: int, maxdegree: int) -> cs.Function:
+    """Creates a function made of monomials as bases.
+
+    Parameters
+    ----------
+    ns : int
+        Number of states.
+    mindegree : int
+        Minimum degree of monomials (included).
+    maxdegree : int
+        Maximum degree of monomials (included).
+
+    Returns
+    -------
+    casadi.Function
+        A casadi function of the form `Phi(s)`, where `s` is the input and `Phi` the
+        basis vector.
+    """
+    s = cs.SX.sym("x", n_in, 1)  # prod is faster with SX, and during runtime
+    y = cs.vertcat(
+        *(
+            prod(s**p)
+            for k in range(mindegree, maxdegree + 1)
+            for p in monomial_powers(n_in, k)
+        )
+    )
+    return cs.Function("Phi", (s,), (y,), ("s",), ("Phi(s)",), {"cse": True})
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/util/seeding.py` & `mpcrl-1.2.0rc4/src/mpcrl/util/seeding.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from collections.abc import Sequence
-from typing import Union
-
-import numpy as np
-from typing_extensions import TypeAlias
-
-RngType: TypeAlias = Union[
-    None,
-    int,
-    Sequence[int],
-    np.random.SeedSequence,
-    np.random.BitGenerator,
-    np.random.Generator,
-]
-
-
-MAX_SEED = np.iinfo(np.uint32).max + 1
-
-
-def mk_seed(rng: np.random.Generator) -> int:
-    """Generates a random seed.
-
-    Parameters
-    ----------
-    rng : np.random.Generator
-        RNG generator
-
-    Returns
-    -------
-    int
-        A random integer in the range [0, 2**32)
-    """
-    return int(rng.integers(MAX_SEED))
+from collections.abc import Sequence
+from typing import Union
+
+import numpy as np
+from typing_extensions import TypeAlias
+
+RngType: TypeAlias = Union[
+    None,
+    int,
+    Sequence[int],
+    np.random.SeedSequence,
+    np.random.BitGenerator,
+    np.random.Generator,
+]
+
+
+MAX_SEED = np.iinfo(np.uint32).max + 1
+
+
+def mk_seed(rng: np.random.Generator) -> int:
+    """Generates a random seed.
+
+    Parameters
+    ----------
+    rng : np.random.Generator
+        RNG generator
+
+    Returns
+    -------
+    int
+        A random integer in the range [0, 2**32)
+    """
+    return int(rng.integers(MAX_SEED))
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/wrappers/agents/log.py` & `mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/log.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-import logging
-from collections.abc import Iterable, Iterator
-from inspect import getmembers, isfunction
-from itertools import chain
-from operator import itemgetter
-from typing import Callable, Optional, TypeVar
-
-import numpy as np
-import numpy.typing as npt
-from gymnasium import Env
-
-from ...agents.common.agent import Agent
-from ...agents.common.learning_agent import LearningAgent
-from ...core.callbacks import (
-    AgentCallbackMixin,
-    LearningAgentCallbackMixin,
-    _failure_msg,
-)
-from ...util.iters import bool_cycle
-from .wrapper import SymType, Wrapper
-
-ObsType = TypeVar("ObsType")
-ActType = TypeVar("ActType")
-_MANDATORY_CALLBACKS = {
-    "on_mpc_failure",
-    "on_validation_start",
-    "on_validation_end",
-    "on_update_failure",
-    "on_training_start",
-    "on_training_end",
-}
-
-_pred = lambda o: isfunction(o) and o.__name__.startswith("on_")
-_AGENT_CALLBACKS = set(map(itemgetter(0), getmembers(AgentCallbackMixin, _pred)))
-_LEARNING_AGENT_CALLBACKS = set.difference(
-    set(map(itemgetter(0), getmembers(LearningAgentCallbackMixin, _pred))),
-    _AGENT_CALLBACKS,
-)
-del _pred
-
-
-def _generate_method_caller(m: Callable) -> Callable:
-    """Returns a method that calls the given method `m`."""
-
-    def method_caller(*args, **kwargs):
-        return m(*args, **kwargs)
-
-    return method_caller
-
-
-class Log(Wrapper[SymType]):
-    """A wrapper class for logging information about an agent."""
-
-    def __init__(
-        self,
-        agent: Agent[SymType],
-        log_name: Optional[str] = None,
-        level: int = logging.INFO,
-        to_file: bool = False,
-        mode: str = "a",
-        precision: int = 3,
-        log_frequencies: Optional[dict[str, int]] = None,
-        exclude_mandatory: Optional[Iterable[str]] = None,
-    ) -> None:
-        """Creates a logger wrapper.
-
-        Parameters
-        ----------
-        agent : LearningAgent or inheriting
-            Agent to wrap.
-        log_name : str, optional
-            Name of the logger. If not provided, the name of the agent is used.
-        level : int, optional
-            The logging level, by default `INFO`.
-        to_file : bool, optional
-            Whether to write the log also to a file in the current directory. By
-            default, `False`.
-        mode : str, optional
-            The mode for opening the logging faile, in case `to_file=True`.
-        precision : int, optional
-            Precision for printing floats, by default 3.
-        log_frequencies : int, optional
-            dict containing for each logging call its corresponding frequency. The calls
-            for which a frequency can be set are:
-             - `on_episode_start`
-             - `on_episode_end`
-             - `on_env_step`
-             - `on_timestep_end`
-             - `on_update`.
-
-            If an entry is not found in the dict, it is assumed that its call is never
-            logged.
-        exclude_mandatory : iterable of str, optional
-            An iterable of strings that contains the mandatory callbacks to be excluded.
-            The mandatory callbacks that can be excluded are:
-             - `on_mpc_failure`
-             - `on_validation_start`
-             - `on_validation_end`
-             - `on_update_failure`
-             - `on_training_start`
-             - `on_training_end`.
-        """
-        name = log_name if log_name is not None else agent.name
-        self.logger = logging.getLogger(name)
-        self.logger.setLevel(level)
-        formatter = logging.Formatter(
-            fmt="%(name)s@%(asctime)s> %(message)s", datefmt="%Y-%m-%d,%H:%M:%S"
-        )
-        ch = logging.StreamHandler()
-        ch.setLevel(level)
-        ch.setFormatter(formatter)
-        self.logger.addHandler(ch)
-        if to_file:
-            fh = logging.FileHandler(f"{name}.txt", mode=mode)
-            fh.setLevel(level)
-            fh.setFormatter(formatter)
-            self.logger.addHandler(fh)
-        self.precision = precision
-
-        # store excluded-mandatory-callbacks and callbacks-with-frequency
-        self.exclude_mandatory: set[str] = (
-            set() if exclude_mandatory is None else set(exclude_mandatory)
-        )
-        self.log_frequencies: dict[str, Iterator[bool]] = {}
-        if log_frequencies is not None:
-            for name, freq in log_frequencies.items():
-                if name not in _MANDATORY_CALLBACKS:
-                    self.log_frequencies[name] = bool_cycle(freq)
-
-        # if the agent is non-learning, make sure that both mandatory and callbacks with
-        # frequencies do not lead to callbacks reserved to only learning agents.
-        if not isinstance(agent.unwrapped, LearningAgent):
-            for cb in _LEARNING_AGENT_CALLBACKS:
-                self.exclude_mandatory.add(cb)
-                self.log_frequencies.pop(cb, None)
-        super().__init__(agent)
-
-    def establish_callback_hooks(self) -> None:
-        super().establish_callback_hooks()
-        # hook only the callbacks for which a frequency was given + the mandatory ones
-        repr_self = repr(self)
-        optional_cbs = self.log_frequencies.keys()
-        mandatory_cbs = _MANDATORY_CALLBACKS.difference(self.exclude_mandatory)
-        for name in chain(optional_cbs, mandatory_cbs):
-            method = getattr(self, f"_{name}")
-            self.hook_callback(repr_self, name, _generate_method_caller(method))
-
-    # callbacks for Agent
-
-    def _on_mpc_failure(
-        self, episode: int, timestep: Optional[int], status: str, raises: bool
-    ) -> None:
-        m = self.logger.error if raises else self.logger.warning
-        m(_failure_msg("mpc", self.agent.name, episode, timestep, status))
-
-    def _on_validation_start(self, env: Env[ObsType, ActType]) -> None:
-        self.logger.debug("validation of %s started.", env)
-
-    def _on_validation_end(
-        self, env: Env[ObsType, ActType], returns: npt.NDArray[np.floating]
-    ) -> None:
-        S = np.array2string(returns, precision=self.precision)
-        self.logger.info("validation of %s concluded with returns=%s.", env, S)
-
-    def _on_episode_start(
-        self, env: Env[ObsType, ActType], episode: int, state: ObsType
-    ) -> None:
-        if next(self.log_frequencies["on_episode_start"]):
-            S = np.array2string(state, precision=self.precision)
-            self.logger.debug("episode %d started with state=%s.", episode, S)
-
-    def _on_episode_end(
-        self, env: Env[ObsType, ActType], episode: int, rewards: float
-    ) -> None:
-        if next(self.log_frequencies["on_episode_end"]):
-            self.logger.info(
-                "episode %d ended with rewards=%.*f.", episode, self.precision, rewards
-            )
-
-    def _on_env_step(
-        self, env: Env[ObsType, ActType], episode: int, timestep: int
-    ) -> None:
-        if next(self.log_frequencies["on_env_step"]):
-            self.logger.debug(
-                "env stepped in episode %d at time %d.", episode, timestep
-            )
-
-    def _on_timestep_end(
-        self, env: Env[ObsType, ActType], episode: int, timestep: int
-    ) -> None:
-        if next(self.log_frequencies["on_timestep_end"]):
-            self.logger.debug("episode %d stepped at time %d.", episode, timestep)
-
-    # callbacks for LearningAgent
-
-    def _on_update_failure(
-        self, episode: int, timestep: Optional[int], errormsg: str, raises: bool
-    ) -> None:
-        (self.logger.error if raises else self.logger.warning)(
-            "_failure_msg('update', %s, %d, %s, %s)",
-            self.agent.name,
-            episode,
-            timestep,
-            errormsg,
-        )
-
-    def _on_training_start(self, env: Env[ObsType, ActType]) -> None:
-        self.logger.debug("training of %s started.", env)
-
-    def _on_training_end(
-        self, env: Env[ObsType, ActType], returns: npt.NDArray[np.floating]
-    ) -> None:
-        S = np.array2string(returns, precision=self.precision)
-        self.logger.info("training of %s concluded with returns=%s.", env, S)
-
-    def _on_update(self) -> None:
-        if next(self.log_frequencies["on_update"]):
-            S = self.agent.learnable_parameters.stringify()
-            self.logger.info("updated parameters: %s.", S)
+import logging
+from collections.abc import Iterable, Iterator
+from inspect import getmembers, isfunction
+from itertools import chain
+from operator import itemgetter
+from typing import Callable, Optional, TypeVar
+
+import numpy as np
+import numpy.typing as npt
+from gymnasium import Env
+
+from ...agents.common.agent import Agent
+from ...agents.common.learning_agent import LearningAgent
+from ...core.callbacks import (
+    AgentCallbackMixin,
+    LearningAgentCallbackMixin,
+    _failure_msg,
+)
+from ...util.iters import bool_cycle
+from .wrapper import SymType, Wrapper
+
+ObsType = TypeVar("ObsType")
+ActType = TypeVar("ActType")
+_MANDATORY_CALLBACKS = {
+    "on_mpc_failure",
+    "on_validation_start",
+    "on_validation_end",
+    "on_update_failure",
+    "on_training_start",
+    "on_training_end",
+}
+
+_pred = lambda o: isfunction(o) and o.__name__.startswith("on_")
+_AGENT_CALLBACKS = set(map(itemgetter(0), getmembers(AgentCallbackMixin, _pred)))
+_LEARNING_AGENT_CALLBACKS = set.difference(
+    set(map(itemgetter(0), getmembers(LearningAgentCallbackMixin, _pred))),
+    _AGENT_CALLBACKS,
+)
+del _pred
+
+
+def _generate_method_caller(m: Callable) -> Callable:
+    """Returns a method that calls the given method `m`."""
+
+    def method_caller(*args, **kwargs):
+        return m(*args, **kwargs)
+
+    return method_caller
+
+
+class Log(Wrapper[SymType]):
+    """A wrapper class for logging information about an agent."""
+
+    def __init__(
+        self,
+        agent: Agent[SymType],
+        log_name: Optional[str] = None,
+        level: int = logging.INFO,
+        to_file: bool = False,
+        mode: str = "a",
+        precision: int = 3,
+        log_frequencies: Optional[dict[str, int]] = None,
+        exclude_mandatory: Optional[Iterable[str]] = None,
+    ) -> None:
+        """Creates a logger wrapper.
+
+        Parameters
+        ----------
+        agent : LearningAgent or inheriting
+            Agent to wrap.
+        log_name : str, optional
+            Name of the logger. If not provided, the name of the agent is used.
+        level : int, optional
+            The logging level, by default `INFO`.
+        to_file : bool, optional
+            Whether to write the log also to a file in the current directory. By
+            default, `False`.
+        mode : str, optional
+            The mode for opening the logging faile, in case `to_file=True`.
+        precision : int, optional
+            Precision for printing floats, by default 3.
+        log_frequencies : int, optional
+            dict containing for each logging call its corresponding frequency. The calls
+            for which a frequency can be set are:
+             - `on_episode_start`
+             - `on_episode_end`
+             - `on_env_step`
+             - `on_timestep_end`
+             - `on_update`.
+
+            If an entry is not found in the dict, it is assumed that its call is never
+            logged.
+        exclude_mandatory : iterable of str, optional
+            An iterable of strings that contains the mandatory callbacks to be excluded.
+            The mandatory callbacks that can be excluded are:
+             - `on_mpc_failure`
+             - `on_validation_start`
+             - `on_validation_end`
+             - `on_update_failure`
+             - `on_training_start`
+             - `on_training_end`.
+        """
+        name = log_name if log_name is not None else agent.name
+        self.logger = logging.getLogger(name)
+        self.logger.setLevel(level)
+        formatter = logging.Formatter(
+            fmt="%(name)s@%(asctime)s> %(message)s", datefmt="%Y-%m-%d,%H:%M:%S"
+        )
+        ch = logging.StreamHandler()
+        ch.setLevel(level)
+        ch.setFormatter(formatter)
+        self.logger.addHandler(ch)
+        if to_file:
+            fh = logging.FileHandler(f"{name}.txt", mode=mode)
+            fh.setLevel(level)
+            fh.setFormatter(formatter)
+            self.logger.addHandler(fh)
+        self.precision = precision
+
+        # store excluded-mandatory-callbacks and callbacks-with-frequency
+        self.exclude_mandatory: set[str] = (
+            set() if exclude_mandatory is None else set(exclude_mandatory)
+        )
+        self.log_frequencies: dict[str, Iterator[bool]] = {}
+        if log_frequencies is not None:
+            for name, freq in log_frequencies.items():
+                if name not in _MANDATORY_CALLBACKS:
+                    self.log_frequencies[name] = bool_cycle(freq)
+
+        # if the agent is non-learning, make sure that both mandatory and callbacks with
+        # frequencies do not lead to callbacks reserved to only learning agents.
+        if not isinstance(agent.unwrapped, LearningAgent):
+            for cb in _LEARNING_AGENT_CALLBACKS:
+                self.exclude_mandatory.add(cb)
+                self.log_frequencies.pop(cb, None)
+        super().__init__(agent)
+
+    def establish_callback_hooks(self) -> None:
+        super().establish_callback_hooks()
+        # hook only the callbacks for which a frequency was given + the mandatory ones
+        repr_self = repr(self)
+        optional_cbs = self.log_frequencies.keys()
+        mandatory_cbs = _MANDATORY_CALLBACKS.difference(self.exclude_mandatory)
+        for name in chain(optional_cbs, mandatory_cbs):
+            method = getattr(self, f"_{name}")
+            self.hook_callback(repr_self, name, _generate_method_caller(method))
+
+    # callbacks for Agent
+
+    def _on_mpc_failure(
+        self, episode: int, timestep: Optional[int], status: str, raises: bool
+    ) -> None:
+        m = self.logger.error if raises else self.logger.warning
+        m(_failure_msg("mpc", self.agent.name, episode, timestep, status))
+
+    def _on_validation_start(self, env: Env[ObsType, ActType]) -> None:
+        self.logger.debug("validation of %s started.", env)
+
+    def _on_validation_end(
+        self, env: Env[ObsType, ActType], returns: npt.NDArray[np.floating]
+    ) -> None:
+        S = np.array2string(returns, precision=self.precision)
+        self.logger.info("validation of %s concluded with returns=%s.", env, S)
+
+    def _on_episode_start(
+        self, env: Env[ObsType, ActType], episode: int, state: ObsType
+    ) -> None:
+        if next(self.log_frequencies["on_episode_start"]):
+            S = np.array2string(state, precision=self.precision)
+            self.logger.debug("episode %d started with state=%s.", episode, S)
+
+    def _on_episode_end(
+        self, env: Env[ObsType, ActType], episode: int, rewards: float
+    ) -> None:
+        if next(self.log_frequencies["on_episode_end"]):
+            self.logger.info(
+                "episode %d ended with rewards=%.*f.", episode, self.precision, rewards
+            )
+
+    def _on_env_step(
+        self, env: Env[ObsType, ActType], episode: int, timestep: int
+    ) -> None:
+        if next(self.log_frequencies["on_env_step"]):
+            self.logger.debug(
+                "env stepped in episode %d at time %d.", episode, timestep
+            )
+
+    def _on_timestep_end(
+        self, env: Env[ObsType, ActType], episode: int, timestep: int
+    ) -> None:
+        if next(self.log_frequencies["on_timestep_end"]):
+            self.logger.debug("episode %d stepped at time %d.", episode, timestep)
+
+    # callbacks for LearningAgent
+
+    def _on_update_failure(
+        self, episode: int, timestep: Optional[int], errormsg: str, raises: bool
+    ) -> None:
+        (self.logger.error if raises else self.logger.warning)(
+            "_failure_msg('update', %s, %d, %s, %s)",
+            self.agent.name,
+            episode,
+            timestep,
+            errormsg,
+        )
+
+    def _on_training_start(self, env: Env[ObsType, ActType]) -> None:
+        self.logger.debug("training of %s started.", env)
+
+    def _on_training_end(
+        self, env: Env[ObsType, ActType], returns: npt.NDArray[np.floating]
+    ) -> None:
+        S = np.array2string(returns, precision=self.precision)
+        self.logger.info("training of %s concluded with returns=%s.", env, S)
+
+    def _on_update(self) -> None:
+        if next(self.log_frequencies["on_update"]):
+            S = self.agent.learnable_parameters.stringify()
+            self.logger.info("updated parameters: %s.", S)
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/wrappers/agents/record_updates.py` & `mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/record_updates.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import numpy as np
-import numpy.typing as npt
-
-from ...agents.common.learning_agent import ExpType, LearningAgent
-from .wrapper import LearningWrapper, SymType
-
-
-class RecordUpdates(LearningWrapper[SymType, ExpType]):
-    """Wrapper for recording the history of updates by the learning agent."""
-
-    def __init__(self, agent: LearningAgent[SymType, ExpType]) -> None:
-        """Instantiates the recorder.
-
-        Parameters
-        ----------
-        agent : LearningAgent or inheriting
-            The agent whose updates need recording.
-        """
-        super().__init__(agent)
-        self.updates_history: dict[str, list[npt.NDArray[np.floating]]] = {
-            p.name: [p.value] for p in agent.learnable_parameters.values()
-        }
-
-    def _on_update(self, *_, **__) -> None:
-        """Internal utility to store the current parameters in memory."""
-        for par in self.agent.learnable_parameters.values():
-            self.updates_history[par.name].append(par.value)
-
-    def establish_callback_hooks(self) -> None:
-        super().establish_callback_hooks()
-        # connect the agent's on_update callback to this wrapper storing action
-        self.hook_callback(repr(self), "on_update", self._on_update)
+import numpy as np
+import numpy.typing as npt
+
+from ...agents.common.learning_agent import ExpType, LearningAgent
+from .wrapper import LearningWrapper, SymType
+
+
+class RecordUpdates(LearningWrapper[SymType, ExpType]):
+    """Wrapper for recording the history of updates by the learning agent."""
+
+    def __init__(self, agent: LearningAgent[SymType, ExpType]) -> None:
+        """Instantiates the recorder.
+
+        Parameters
+        ----------
+        agent : LearningAgent or inheriting
+            The agent whose updates need recording.
+        """
+        super().__init__(agent)
+        self.updates_history: dict[str, list[npt.NDArray[np.floating]]] = {
+            p.name: [p.value] for p in agent.learnable_parameters.values()
+        }
+
+    def _on_update(self, *_, **__) -> None:
+        """Internal utility to store the current parameters in memory."""
+        for par in self.agent.learnable_parameters.values():
+            self.updates_history[par.name].append(par.value)
+
+    def establish_callback_hooks(self) -> None:
+        super().establish_callback_hooks()
+        # connect the agent's on_update callback to this wrapper storing action
+        self.hook_callback(repr(self), "on_update", self._on_update)
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/wrappers/agents/wrapper.py` & `mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/wrapper.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-from typing import Any, Callable, Generic, Union
-
-from csnlp.util.io import SupportsDeepcopyAndPickle
-
-from ...agents.common.agent import Agent, SymType
-from ...agents.common.learning_agent import ExpType, LearningAgent
-from ...core.callbacks import CallbackMixin
-
-
-class Wrapper(SupportsDeepcopyAndPickle, CallbackMixin, Generic[SymType]):
-    """Wraps a learning agent to allow a modular transformation of its methods. This
-    class is the base class for all wrappers. The subclass could override some methods
-    to change the behavior of the original agent without touching the original code."""
-
-    def __init__(self, agent: Agent[SymType]) -> None:
-        """Wraps an agent's instance.
-
-        Parameters
-        ----------
-        agent : Agent or subclass
-            The agent to wrap.
-        """
-        SupportsDeepcopyAndPickle.__init__(self)
-        CallbackMixin.__init__(self)
-        del self._hooks  # only keep one dict of hooks, i.e., the agent's one
-        self.agent = agent
-        self._hooked_callbacks: dict[str, list[str]] = {}
-        self.establish_callback_hooks()
-
-    @property
-    def unwrapped(self) -> Union[Agent[SymType], LearningAgent[SymType, ExpType]]:
-        """'Returns the original agent of the wrapper."""
-        return self.agent.unwrapped
-
-    def is_wrapped(self, wrapper_type: type["Wrapper[SymType]"]) -> bool:
-        """Gets whether the agent instance is wrapped or not by the wrapper type.
-
-        Parameters
-        ----------
-        wrapper_type : type of Wrapper
-            Type of wrapper to check if the agent is wrapped with.
-
-        Returns
-        -------
-        bool
-            `True` if wrapped by an instance of `wrapper_type`; `False`, otherwise.
-        """
-        if isinstance(self, wrapper_type):
-            return True
-        return self.agent.is_wrapped(wrapper_type)
-
-    def hook_callback(
-        self, attachername: str, callbackname: str, func: Callable[..., None]
-    ) -> None:
-        """See `LearningAgent.hook_callback`."""
-        # store the callback id for later removal via `detach_wrapper(s)`
-        self._hooked_callbacks.setdefault(callbackname, []).append(attachername)
-        self.unwrapped.hook_callback(attachername, callbackname, func)
-
-    def detach_wrapper(
-        self,
-    ) -> Union[Agent[SymType], LearningAgent[SymType, ExpType], "Wrapper[SymType]"]:
-        """Detaches the wrapper from the agent, returning the wrapped agent. De facto,
-        this method detaches all the hooks attached by this wrapper.
-
-        Returns
-        -------
-        Agent or Wrapper
-            Returns the wrapped agent (or other wrapper) instance. This instance has no
-            more active hooks attached by this wrapper.
-        """
-        hooks = self.unwrapped._hooks
-        hooked_callbacks = self._hooked_callbacks
-
-        # for each callback type, remove the hooks attached by this wrapper
-        for callbackname, attachernames in hooked_callbacks.items():
-            hook_group = hooks[callbackname]
-            for attachername in attachernames:
-                hook_group.pop(attachername)
-
-            # if the callback has no more hooks, remove it
-            if not hook_group:
-                hooks.pop(callbackname)
-
-        # clear hooked callbacks tracking
-        hooked_callbacks.clear()
-        return self.agent
-
-    def detach_wrappers(self) -> Union[Agent[SymType], LearningAgent[SymType, ExpType]]:
-        """Similar to `detach_wrapper`, but detaches all wrappers around the agent.
-
-        Returns
-        -------
-        Agent
-            Returns the wrapped agent instance. This instance has no more active hooks
-            attached by all the wrappers around it.
-        """
-        agent_ = self
-        while hasattr(agent_, "detach_wrapper") and callable(agent_.detach_wrapper):
-            agent_ = agent_.detach_wrapper()
-        return agent_
-
-    def __getattr__(self, name: str) -> Any:
-        """Reroutes attributes to the wrapped agent instance."""
-        if name.startswith("_"):
-            raise AttributeError(f"Accessing private attribute '{name}' is prohibited.")
-        return getattr(self.agent, name)
-
-    def __str__(self) -> str:
-        """Returns the wrapped agent string."""
-        return f"<{self.__class__.__name__}{self.agent.__str__()}>"
-
-    def __repr__(self) -> str:
-        """Returns the wrapped agent representation."""
-        return f"<{self.__class__.__name__}{self.agent.__repr__()}>"
-
-
-class LearningWrapper(Wrapper[SymType], Generic[SymType, ExpType]):
-    """Identical to `Wrapper`, but for learning agents."""
-
-    def __init__(self, agent: LearningAgent[SymType, ExpType]) -> None:
-        Wrapper.__init__(self, agent)
-        self.agent: LearningAgent[SymType, ExpType]
-
-    @property
-    def unwrapped(self) -> LearningAgent[SymType, ExpType]:
-        return self.agent.unwrapped
+from typing import Any, Callable, Generic, Union
+
+from csnlp.util.io import SupportsDeepcopyAndPickle
+
+from ...agents.common.agent import Agent, SymType
+from ...agents.common.learning_agent import ExpType, LearningAgent
+from ...core.callbacks import CallbackMixin
+
+
+class Wrapper(SupportsDeepcopyAndPickle, CallbackMixin, Generic[SymType]):
+    """Wraps a learning agent to allow a modular transformation of its methods. This
+    class is the base class for all wrappers. The subclass could override some methods
+    to change the behavior of the original agent without touching the original code."""
+
+    def __init__(self, agent: Agent[SymType]) -> None:
+        """Wraps an agent's instance.
+
+        Parameters
+        ----------
+        agent : Agent or subclass
+            The agent to wrap.
+        """
+        SupportsDeepcopyAndPickle.__init__(self)
+        CallbackMixin.__init__(self)
+        del self._hooks  # only keep one dict of hooks, i.e., the agent's one
+        self.agent = agent
+        self._hooked_callbacks: dict[str, list[str]] = {}
+        self.establish_callback_hooks()
+
+    @property
+    def unwrapped(self) -> Union[Agent[SymType], LearningAgent[SymType, ExpType]]:
+        """'Returns the original agent of the wrapper."""
+        return self.agent.unwrapped
+
+    def is_wrapped(self, wrapper_type: type["Wrapper[SymType]"]) -> bool:
+        """Gets whether the agent instance is wrapped or not by the wrapper type.
+
+        Parameters
+        ----------
+        wrapper_type : type of Wrapper
+            Type of wrapper to check if the agent is wrapped with.
+
+        Returns
+        -------
+        bool
+            `True` if wrapped by an instance of `wrapper_type`; `False`, otherwise.
+        """
+        if isinstance(self, wrapper_type):
+            return True
+        return self.agent.is_wrapped(wrapper_type)
+
+    def hook_callback(
+        self, attachername: str, callbackname: str, func: Callable[..., None]
+    ) -> None:
+        """See `LearningAgent.hook_callback`."""
+        # store the callback id for later removal via `detach_wrapper(s)`
+        self._hooked_callbacks.setdefault(callbackname, []).append(attachername)
+        self.unwrapped.hook_callback(attachername, callbackname, func)
+
+    def detach_wrapper(
+        self,
+    ) -> Union[Agent[SymType], LearningAgent[SymType, ExpType], "Wrapper[SymType]"]:
+        """Detaches the wrapper from the agent, returning the wrapped agent. De facto,
+        this method detaches all the hooks attached by this wrapper.
+
+        Returns
+        -------
+        Agent or Wrapper
+            Returns the wrapped agent (or other wrapper) instance. This instance has no
+            more active hooks attached by this wrapper.
+        """
+        hooks = self.unwrapped._hooks
+        hooked_callbacks = self._hooked_callbacks
+
+        # for each callback type, remove the hooks attached by this wrapper
+        for callbackname, attachernames in hooked_callbacks.items():
+            hook_group = hooks[callbackname]
+            for attachername in attachernames:
+                hook_group.pop(attachername)
+
+            # if the callback has no more hooks, remove it
+            if not hook_group:
+                hooks.pop(callbackname)
+
+        # clear hooked callbacks tracking
+        hooked_callbacks.clear()
+        return self.agent
+
+    def detach_wrappers(self) -> Union[Agent[SymType], LearningAgent[SymType, ExpType]]:
+        """Similar to `detach_wrapper`, but detaches all wrappers around the agent.
+
+        Returns
+        -------
+        Agent
+            Returns the wrapped agent instance. This instance has no more active hooks
+            attached by all the wrappers around it.
+        """
+        agent_ = self
+        while hasattr(agent_, "detach_wrapper") and callable(agent_.detach_wrapper):
+            agent_ = agent_.detach_wrapper()
+        return agent_
+
+    def __getattr__(self, name: str) -> Any:
+        """Reroutes attributes to the wrapped agent instance."""
+        if name.startswith("_"):
+            raise AttributeError(f"Accessing private attribute '{name}' is prohibited.")
+        return getattr(self.agent, name)
+
+    def __str__(self) -> str:
+        """Returns the wrapped agent string."""
+        return f"<{self.__class__.__name__}{self.agent.__str__()}>"
+
+    def __repr__(self) -> str:
+        """Returns the wrapped agent representation."""
+        return f"<{self.__class__.__name__}{self.agent.__repr__()}>"
+
+
+class LearningWrapper(Wrapper[SymType], Generic[SymType, ExpType]):
+    """Identical to `Wrapper`, but for learning agents."""
+
+    def __init__(self, agent: LearningAgent[SymType, ExpType]) -> None:
+        Wrapper.__init__(self, agent)
+        self.agent: LearningAgent[SymType, ExpType]
+
+    @property
+    def unwrapped(self) -> LearningAgent[SymType, ExpType]:
+        return self.agent.unwrapped
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/wrappers/envs/monitor_episodes.py` & `mpcrl-1.2.0rc4/src/mpcrl/wrappers/envs/monitor_episodes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,100 +1,110 @@
-from collections import deque
-from time import perf_counter
-from typing import Any, Deque, Optional, SupportsFloat, TypeVar
-
-import numpy as np
-import numpy.typing as npt
-from gymnasium import Env, Wrapper, utils
-
-ObsType = TypeVar("ObsType")
-ActType = TypeVar("ActType")
-
-
-class MonitorEpisodes(
-    Wrapper[ObsType, ActType, ObsType, ActType], utils.RecordConstructorArgs
-):
-    """This wrapper keeps track of
-        - observations
-        - actions
-        - costs/rewards
-        - episode length
-        - episode execution time
-    that the environment is subject to during the learning process.
-    """
-
-    def __init__(
-        self, env: Env[ObsType, ActType], deque_size: Optional[int] = None
-    ) -> None:
-        """This wrapper will keep track of observations, actions and rewards as well as
-        episode length and execution time.
-
-        Parameters
-        ----------
-        env : Env[ObsType, ActType]
-            The environment to apply the wrapper to.
-        deque_size : int, optional
-            The maximum number of episodes to hold as historical data in the internal
-            deques. By default, `None`, i.e., unlimited.
-        """
-        utils.RecordConstructorArgs.__init__(self, deque_size=deque_size)
-        Wrapper.__init__(self, env)
-        # long-term storages
-        self.observations: Deque[npt.NDArray[ObsType]] = deque(  # type: ignore
-            maxlen=deque_size
-        )
-        self.actions: Deque[npt.NDArray[ActType]] = deque(  # type: ignore
-            maxlen=deque_size
-        )
-        self.rewards: Deque[npt.NDArray[np.floating]] = deque(maxlen=deque_size)
-        self.episode_lengths: Deque[int] = deque(maxlen=deque_size)
-        self.exec_times: Deque[float] = deque(maxlen=deque_size)
-        # current-episode-storages
-        self.ep_observations: list[ObsType] = []
-        self.ep_actions: list[ActType] = []
-        self.ep_rewards: list[SupportsFloat] = []
-        self.t0: float = perf_counter()
-        self.ep_length: int = 0
-
-    def reset(
-        self, *, seed: Optional[int] = None, options: Optional[dict[str, Any]] = None
-    ) -> tuple[ObsType, dict[str, Any]]:
-        """Resets the environment and resets the current data accumulators."""
-        observation, info = super().reset(seed=seed, options=options)
-        self._clear_ep_data()
-        self.ep_observations.append(observation)
-        return observation, info
-
-    def step(
-        self, action: ActType
-    ) -> tuple[ObsType, SupportsFloat, bool, bool, dict[str, Any]]:
-        # sourcery skip: extract-method
-        """Steps through the environment, accumulating the episode data."""
-        obs, reward, terminated, truncated, info = super().step(action)
-
-        # accumulate data
-        self.ep_observations.append(obs)
-        self.ep_actions.append(action)
-        self.ep_rewards.append(reward)
-        self.ep_length += 1
-
-        # if episode is done, save the current data to history
-        if terminated or truncated:
-            # append data
-            self.observations.append(np.asarray(self.ep_observations))
-            self.actions.append(np.asarray(self.ep_actions))
-            self.rewards.append(np.asarray(self.ep_rewards))
-            self.episode_lengths.append(self.ep_length)
-            self.exec_times.append(perf_counter() - self.t0)
-
-            # clear this episode's data
-            self._clear_ep_data()
-
-        return obs, reward, terminated, truncated, info
-
-    def _clear_ep_data(self) -> None:
-        # clear this episode's lists and reset counters
-        self.ep_observations.clear()
-        self.ep_actions.clear()
-        self.ep_rewards.clear()
-        self.t0 = perf_counter()
-        self.ep_length = 0
+from collections import deque
+from time import perf_counter
+from typing import Any, Deque, Optional, SupportsFloat, TypeVar
+
+import numpy as np
+import numpy.typing as npt
+from gymnasium import Env, Wrapper, utils
+
+ObsType = TypeVar("ObsType")
+ActType = TypeVar("ActType")
+
+
+class MonitorEpisodes(
+    Wrapper[ObsType, ActType, ObsType, ActType], utils.RecordConstructorArgs
+):
+    """This wrapper keeps track of
+        - observations (``observations``)
+        - actions (``actions``)
+        - costs/rewards (``rewards``)
+        - episode length (``episode_lengths``)
+        - episode execution time (``exec_times``)
+    that the environment is subject to during the learning process. Note that these are
+    effectly saved in each corresponding field only when the episode is done (terminated
+    or truncated).
+
+    After the completion of an episode, these fields will look like this::
+
+        >>> env.observations = <deque of each episode's observations>
+        ... env.actions = <deque of each episode's actions>
+        ... env.rewards = <deque of each episode's rewards>
+        ... env.episode_lengths = <deque of each episode's episode length>
+        ... env.exec_times = <deque of each episode's execution time>
+    """
+
+    def __init__(
+        self, env: Env[ObsType, ActType], deque_size: Optional[int] = None
+    ) -> None:
+        """This wrapper will keep track of observations, actions and rewards as well as
+        episode length and execution time.
+
+        Parameters
+        ----------
+        env : Env[ObsType, ActType]
+            The environment to apply the wrapper to.
+        deque_size : int, optional
+            The maximum number of episodes to hold as historical data in the internal
+            deques. By default, `None`, i.e., unlimited.
+        """
+        utils.RecordConstructorArgs.__init__(self, deque_size=deque_size)
+        Wrapper.__init__(self, env)
+        # long-term storages
+        self.observations: Deque[npt.NDArray[ObsType]] = deque(  # type: ignore
+            maxlen=deque_size
+        )
+        self.actions: Deque[npt.NDArray[ActType]] = deque(  # type: ignore
+            maxlen=deque_size
+        )
+        self.rewards: Deque[npt.NDArray[np.floating]] = deque(maxlen=deque_size)
+        self.episode_lengths: Deque[int] = deque(maxlen=deque_size)
+        self.exec_times: Deque[float] = deque(maxlen=deque_size)
+        # current-episode-storages
+        self.ep_observations: list[ObsType] = []
+        self.ep_actions: list[ActType] = []
+        self.ep_rewards: list[SupportsFloat] = []
+        self.t0: float = perf_counter()
+        self.ep_length: int = 0
+
+    def reset(
+        self, *, seed: Optional[int] = None, options: Optional[dict[str, Any]] = None
+    ) -> tuple[ObsType, dict[str, Any]]:
+        """Resets the environment and resets the current data accumulators."""
+        observation, info = super().reset(seed=seed, options=options)
+        self._clear_ep_data()
+        self.ep_observations.append(observation)
+        return observation, info
+
+    def step(
+        self, action: ActType
+    ) -> tuple[ObsType, SupportsFloat, bool, bool, dict[str, Any]]:
+        # sourcery skip: extract-method
+        """Steps through the environment, accumulating the episode data."""
+        obs, reward, terminated, truncated, info = super().step(action)
+
+        # accumulate data
+        self.ep_observations.append(obs)
+        self.ep_actions.append(action)
+        self.ep_rewards.append(reward)
+        self.ep_length += 1
+
+        # if episode is done, save the current data to history
+        if terminated or truncated:
+            # append data
+            self.observations.append(np.asarray(self.ep_observations))
+            self.actions.append(np.asarray(self.ep_actions))
+            self.rewards.append(np.asarray(self.ep_rewards))
+            self.episode_lengths.append(self.ep_length)
+            self.exec_times.append(perf_counter() - self.t0)
+
+            # clear this episode's data
+            self._clear_ep_data()
+
+        return obs, reward, terminated, truncated, info
+
+    def _clear_ep_data(self) -> None:
+        # clear this episode's lists and reset counters
+        self.ep_observations.clear()
+        self.ep_actions.clear()
+        self.ep_rewards.clear()
+        self.t0 = perf_counter()
+        self.ep_length = 0
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl/wrappers/envs/monitor_infos.py` & `mpcrl-1.2.0rc4/src/mpcrl/wrappers/envs/monitor_infos.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-from collections import deque
-from collections.abc import Iterable
-from logging import warn
-from typing import Any, Deque, Optional, SupportsFloat, TypeVar
-
-from gymnasium import Env, Wrapper, utils
-
-ObsType = TypeVar("ObsType")
-ActType = TypeVar("ActType")
-
-
-def compact_dicts(
-    dicts: Iterable[dict[str, Any]], fill_value: Any = None
-) -> dict[str, list[Any]]:
-    """Compacts an iterable of dictionaries into a single dict with lists of entries. If
-    an entry is missing for any given dict, `fill_value` is used in place.
-
-    Parameters
-    ----------
-    dicts : iterable of dicts[str, any]
-        Dictionaries to be compacted into a single one.
-    fill_value : any, optional
-        The value to be used to fill in missing values.
-
-    Returns
-    -------
-    dict[str, list of any | fill_value]
-        A unique dictionary made from all the passed dicts.
-    """
-    out: dict[str, list[Any]] = {}
-    for i, dict_ in enumerate(dicts):
-        for k, v in dict_.items():
-            if k in out:
-                out[k].append(v)
-            else:
-                out[k] = [fill_value] * i + [v]
-        for k in out.keys() - dict_.keys():
-            out[k].append(fill_value)
-    return out
-
-
-class MonitorInfos(
-    Wrapper[ObsType, ActType, ObsType, ActType], utils.RecordConstructorArgs
-):
-    """This wrapper keeps track of the infos that are generated by the env when `reset`
-    and `step` are called."""
-
-    def __init__(
-        self, env: Env[ObsType, ActType], deque_size: Optional[int] = None
-    ) -> None:
-        """This wrapper will keep track of the reset/step information dicts.
-
-        Parameters
-        ----------
-        env : Env[ObsType, ActType]
-            The environment to apply the wrapper to.
-        deque_size : int, optional
-            The maximum number of episodes to hold as historical data in the internal
-            deques. By default, `None`, i.e., unlimited.
-        """
-        utils.RecordConstructorArgs.__init__(self, deque_size=deque_size)
-        Wrapper.__init__(self, env)
-        # long-term storages
-        self.reset_infos: Deque[dict[str, Any]] = deque(maxlen=deque_size)
-        self.step_infos: Deque[list[dict[str, Any]]] = deque(maxlen=deque_size)
-        # current-episode storages
-        self.ep_step_infos: list[dict[str, Any]] = []
-
-    def reset(
-        self, *, seed: Optional[int] = None, options: Optional[dict[str, Any]] = None
-    ) -> tuple[ObsType, dict[str, Any]]:
-        """Resets the environment and resets the current info accumulators."""
-        observation, info = super().reset(seed=seed, options=options)
-        self.ep_step_infos.clear()
-        self.reset_infos.append(info)
-        return observation, info
-
-    def step(
-        self, action: ActType
-    ) -> tuple[ObsType, SupportsFloat, bool, bool, dict[str, Any]]:
-        """Steps through the environment, accumulating the episode info dicts."""
-        obs, reward, terminated, truncated, info = super().step(action)
-        self.ep_step_infos.append(info)
-        if terminated or truncated:
-            self.step_infos.append(self.ep_step_infos.copy())
-            self.ep_step_infos.clear()
-        return obs, reward, terminated, truncated, info
-
-    def finalized_reset_infos(self, fill_value: Any = None) -> dict[str, list[Any]]:
-        """Returns a compacted final dictionary containing the reset infos. Missing
-        values are filled automatically.
-
-        Parameters
-        ----------
-        fill_value : Any, optional
-            The value to be used to fill in missing values.
-
-        Returns
-        -------
-        dict of (str, list)
-            A unique dict containing for each entry returned in the reset info the
-            corresponding list of entries, one per each reset call.
-        """
-        return compact_dicts(self.reset_infos, fill_value)
-
-    def finalized_step_infos(
-        self, fill_value: Any = None
-    ) -> dict[str, list[list[Any]]]:
-        """Returns a compacted final dictionary containing the step infos. Missing
-        values are filled automatically.
-
-        Parameters
-        ----------
-        fill_value : Any, optional
-            The value to be used to fill in missing values.
-
-        Returns
-        -------
-        dict of (str, list of lists)
-            A unique dict containing for each entry returned in the step info the
-            corresponding list of dicts per episode, with one entry per each step call.
-        """
-
-        if self.ep_step_infos:
-            warn(
-                "Internal buffer of step infos not empty, meaning that the last "
-                "episode did not terminate properly.",
-                RuntimeWarning,
-            )
-        return compact_dicts(
-            (compact_dicts(d, fill_value) for d in self.step_infos), fill_value
-        )
+from collections import deque
+from collections.abc import Iterable
+from logging import warn
+from typing import Any, Deque, Optional, SupportsFloat, TypeVar
+
+from gymnasium import Env, Wrapper, utils
+
+ObsType = TypeVar("ObsType")
+ActType = TypeVar("ActType")
+
+
+def compact_dicts(
+    dicts: Iterable[dict[str, Any]], fill_value: Any = None
+) -> dict[str, list[Any]]:
+    """Compacts an iterable of dictionaries into a single dict with lists of entries. If
+    an entry is missing for any given dict, `fill_value` is used in place.
+
+    Parameters
+    ----------
+    dicts : iterable of dicts[str, any]
+        Dictionaries to be compacted into a single one.
+    fill_value : any, optional
+        The value to be used to fill in missing values.
+
+    Returns
+    -------
+    dict[str, list of any | fill_value]
+        A unique dictionary made from all the passed dicts.
+    """
+    out: dict[str, list[Any]] = {}
+    for i, dict_ in enumerate(dicts):
+        for k, v in dict_.items():
+            if k in out:
+                out[k].append(v)
+            else:
+                out[k] = [fill_value] * i + [v]
+        for k in out.keys() - dict_.keys():
+            out[k].append(fill_value)
+    return out
+
+
+class MonitorInfos(
+    Wrapper[ObsType, ActType, ObsType, ActType], utils.RecordConstructorArgs
+):
+    """This wrapper keeps track of the infos that are generated by the env when `reset`
+    and `step` are called."""
+
+    def __init__(
+        self, env: Env[ObsType, ActType], deque_size: Optional[int] = None
+    ) -> None:
+        """This wrapper will keep track of the reset/step information dicts.
+
+        Parameters
+        ----------
+        env : Env[ObsType, ActType]
+            The environment to apply the wrapper to.
+        deque_size : int, optional
+            The maximum number of episodes to hold as historical data in the internal
+            deques. By default, `None`, i.e., unlimited.
+        """
+        utils.RecordConstructorArgs.__init__(self, deque_size=deque_size)
+        Wrapper.__init__(self, env)
+        # long-term storages
+        self.reset_infos: Deque[dict[str, Any]] = deque(maxlen=deque_size)
+        self.step_infos: Deque[list[dict[str, Any]]] = deque(maxlen=deque_size)
+        # current-episode storages
+        self.ep_step_infos: list[dict[str, Any]] = []
+
+    def reset(
+        self, *, seed: Optional[int] = None, options: Optional[dict[str, Any]] = None
+    ) -> tuple[ObsType, dict[str, Any]]:
+        """Resets the environment and resets the current info accumulators."""
+        observation, info = super().reset(seed=seed, options=options)
+        self.ep_step_infos.clear()
+        self.reset_infos.append(info)
+        return observation, info
+
+    def step(
+        self, action: ActType
+    ) -> tuple[ObsType, SupportsFloat, bool, bool, dict[str, Any]]:
+        """Steps through the environment, accumulating the episode info dicts."""
+        obs, reward, terminated, truncated, info = super().step(action)
+        self.ep_step_infos.append(info)
+        if terminated or truncated:
+            self.step_infos.append(self.ep_step_infos.copy())
+            self.ep_step_infos.clear()
+        return obs, reward, terminated, truncated, info
+
+    def finalized_reset_infos(self, fill_value: Any = None) -> dict[str, list[Any]]:
+        """Returns a compacted final dictionary containing the reset infos. Missing
+        values are filled automatically.
+
+        Parameters
+        ----------
+        fill_value : Any, optional
+            The value to be used to fill in missing values.
+
+        Returns
+        -------
+        dict of (str, list)
+            A unique dict containing for each entry returned in the reset info the
+            corresponding list of entries, one per each reset call.
+        """
+        return compact_dicts(self.reset_infos, fill_value)
+
+    def finalized_step_infos(
+        self, fill_value: Any = None
+    ) -> dict[str, list[list[Any]]]:
+        """Returns a compacted final dictionary containing the step infos. Missing
+        values are filled automatically.
+
+        Parameters
+        ----------
+        fill_value : Any, optional
+            The value to be used to fill in missing values.
+
+        Returns
+        -------
+        dict of (str, list of lists)
+            A unique dict containing for each entry returned in the step info the
+            corresponding list of dicts per episode, with one entry per each step call.
+        """
+
+        if self.ep_step_infos:
+            warn(
+                "Internal buffer of step infos not empty, meaning that the last "
+                "episode did not terminate properly.",
+                RuntimeWarning,
+            )
+        return compact_dicts(
+            (compact_dicts(d, fill_value) for d in self.step_infos), fill_value
+        )
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl.egg-info/PKG-INFO` & `mpcrl-1.2.0rc4/src/mpcrl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-Metadata-Version: 2.1
-Name: mpcrl
-Version: 1.2.0rc3
-Summary: Reinforcement Learning with Model Predictive Control
-Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/FilippoAiraldi/mpc-reinforcement-learning
-Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues
-Keywords: reinforcement-learning,model-predictive-control,optimization,casadi
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: typing_extensions>=4.5.0
-Requires-Dist: numba>=0.57.1
-Requires-Dist: csnlp>=1.5.8
-Requires-Dist: scipy>=1.11.0
-Requires-Dist: gymnasium>=0.28.1
-
-# Reinforcement Learning with Model Predictive Control
-
-**mpcrl** is a library for training model-based Reinforcement Learning (RL) agents with Model Predictive Control (MPC) as function approximation. This framework, also known as MPC-based RL, was first proposed in [[1]](#1) and has so far been shown effective in various applications and with different learning algorithms, e.g., [[2](#2),[3](#3)].
-
-[![PyPI version](https://badge.fury.io/py/mpcrl.svg)](https://badge.fury.io/py/mpcrl)
-[![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
-![Python 3.9](https://img.shields.io/badge/python->=3.9-green.svg)
-
-[![Tests](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml/badge.svg)](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml)
-[![Downloads](https://static.pepy.tech/badge/mpcrl)](https://www.pepy.tech/projects/mpcrl)
-[![Maintainability](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/maintainability)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/maintainability)
-[![Test Coverage](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/test_coverage)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/test_coverage)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
----
-
-## Introduction
-
-This framework merges two powerful control techinques into a single data-driven one
-
-- MPC, a well-known control methodology that exploits a prediction model to predict the future behaviour of the environment and compute the optimal action
-
-- and RL, a Machine Learning paradigm that showed many successes in recent years (with  games such as chess, Go, etc.) and is highly adaptable to unknown and complex-to-model environments.
-
-<div align="center">
-  <img src="https://raw.githubusercontent.com/FilippoAiraldi/mpc-reinforcement-learning/main/resources/mpcrl-diagram.png" alt="mpcrl-diagram" height="300">
-</div>
-
-The figure shows the main idea behind this learning-based control approach. The MPC controller, parametrized in $\vartheta$, acts both as policy provider (providing an action to the environment, given the current state) and as function approximation for the state and action value functions. Concurrently, an RL agent is employed to tune the parameters of the MPC in such a way to increase the controller's performance and achieve an (sub)optimal policy.
-
----
-
-## Installation
-
-To install the package, run
-
-```bash
-pip install mpcrl
-```
-
-**mpcrl** has the following dependencies
-
-- [csnlp](https://pypi.org/project/csnlp/)
-- [SciPy](https://scipy.org/)
-- [Gymnasium](https://gymnasium.farama.org/)
-- [Numba](https://numba.pydata.org/)
-- [typing_extensions](https://pypi.org/project/typing-extensions/)
-
-For playing around with the source code instead, run
-
-```bash
-git clone https://github.com/FilippoAiraldi/mpc-reinforcement-learning.git
-```
-
----
-
-## Examples
-
-Our [examples](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/tree/main/examples) subdirectory contains an example application on a small linear time-invariant (LTI) system, tackled both with Q-learning and Deterministic Policy Gradient (DPG).
-
----
-
-## License
-
-The repository is provided under the MIT License. See the LICENSE file included with this repository.
-
----
-
-## Author
-
-[Filippo Airaldi](https://www.tudelft.nl/staff/f.airaldi/), PhD Candidate [f.airaldi@tudelft.nl | filippoairaldi@gmail.com]
-
-> [Delft Center for Systems and Control](https://www.tudelft.nl/en/3me/about/departments/delft-center-for-systems-and-control/) in [Delft University of Technology](https://www.tudelft.nl/en/)
-
-Copyright (c) 2023 Filippo Airaldi.
-
-Copyright notice: Technische Universiteit Delft hereby disclaims all copyright interest in the program “mpcrl” (Reinforcement Learning with Model Predictive Control) written by the Author(s). Prof. Dr. Ir. Fred van Keulen, Dean of 3mE.
-
----
-
-## References
-
-<a id="1">[1]</a>
-S. Gros and M. Zanon, "Data-Driven Economic NMPC Using Reinforcement Learning," in _IEEE Transactions on Automatic Control_, vol. 65, no. 2, pp. 636-648, Feb. 2020, doi: 10.1109/TAC.2019.2913768.
-
-<a id="2">[2]</a>
-H. N. Esfahani, A. B. Kordabad and S. Gros, "Approximate Robust NMPC using Reinforcement Learning," _2021 European Control Conference (ECC)_, 2021, pp. 132-137, doi: 10.23919/ECC54610.2021.9655129.
-
-<a id="3">[3]</a>
-W. Cai, A. B. Kordabad, H. N. Esfahani, A. M. Lekkas and S. Gros, "MPC-based Reinforcement Learning for a Simplified Freight Mission of Autonomous Surface Vehicles," _2021 60th IEEE Conference on Decision and Control (CDC)_, 2021, pp. 2990-2995, doi: 10.1109/CDC45484.2021.9683750.
+Metadata-Version: 2.1
+Name: mpcrl
+Version: 1.2.0rc4
+Summary: Reinforcement Learning with Model Predictive Control
+Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/FilippoAiraldi/mpc-reinforcement-learning
+Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues
+Keywords: reinforcement-learning,model-predictive-control,optimization,casadi
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: typing_extensions>=4.5.0
+Requires-Dist: numba>=0.57.1
+Requires-Dist: csnlp>=1.5.10rc3
+Requires-Dist: scipy>=1.11.0
+Requires-Dist: gymnasium>=0.28.1
+
+# Reinforcement Learning with Model Predictive Control
+
+**mpcrl** is a library for training model-based Reinforcement Learning (RL) agents with Model Predictive Control (MPC) as function approximation. This framework, also known as MPC-based RL, was first proposed in [[1]](#1) and has so far been shown effective in various applications and with different learning algorithms, e.g., [[2](#2),[3](#3)].
+
+[![PyPI version](https://badge.fury.io/py/mpcrl.svg)](https://badge.fury.io/py/mpcrl)
+[![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
+![Python 3.9](https://img.shields.io/badge/python->=3.9-green.svg)
+
+[![Tests](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml/badge.svg)](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml)
+[![Downloads](https://static.pepy.tech/badge/mpcrl)](https://www.pepy.tech/projects/mpcrl)
+[![Maintainability](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/maintainability)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/test_coverage)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/test_coverage)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+---
+
+## Introduction
+
+This framework merges two powerful control techinques into a single data-driven one
+
+- MPC, a well-known control methodology that exploits a prediction model to predict the future behaviour of the environment and compute the optimal action
+
+- and RL, a Machine Learning paradigm that showed many successes in recent years (with  games such as chess, Go, etc.) and is highly adaptable to unknown and complex-to-model environments.
+
+<div align="center">
+  <img src="https://raw.githubusercontent.com/FilippoAiraldi/mpc-reinforcement-learning/main/resources/mpcrl-diagram.png" alt="mpcrl-diagram" height="300">
+</div>
+
+The figure shows the main idea behind this learning-based control approach. The MPC controller, parametrized in $\vartheta$, acts both as policy provider (providing an action to the environment, given the current state) and as function approximation for the state and action value functions. Concurrently, an RL agent is employed to tune the parameters of the MPC in such a way to increase the controller's performance and achieve an (sub)optimal policy.
+
+---
+
+## Installation
+
+To install the package, run
+
+```bash
+pip install mpcrl
+```
+
+**mpcrl** has the following dependencies
+
+- [csnlp](https://pypi.org/project/csnlp/)
+- [SciPy](https://scipy.org/)
+- [Gymnasium](https://gymnasium.farama.org/)
+- [Numba](https://numba.pydata.org/)
+- [typing_extensions](https://pypi.org/project/typing-extensions/)
+
+For playing around with the source code instead, run
+
+```bash
+git clone https://github.com/FilippoAiraldi/mpc-reinforcement-learning.git
+```
+
+---
+
+## Examples
+
+Our [examples](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/tree/main/examples) subdirectory contains an example application on a small linear time-invariant (LTI) system, tackled both with Q-learning and Deterministic Policy Gradient (DPG).
+
+---
+
+## License
+
+The repository is provided under the MIT License. See the LICENSE file included with this repository.
+
+---
+
+## Author
+
+[Filippo Airaldi](https://www.tudelft.nl/staff/f.airaldi/), PhD Candidate [f.airaldi@tudelft.nl | filippoairaldi@gmail.com]
+
+> [Delft Center for Systems and Control](https://www.tudelft.nl/en/3me/about/departments/delft-center-for-systems-and-control/) in [Delft University of Technology](https://www.tudelft.nl/en/)
+
+Copyright (c) 2023 Filippo Airaldi.
+
+Copyright notice: Technische Universiteit Delft hereby disclaims all copyright interest in the program “mpcrl” (Reinforcement Learning with Model Predictive Control) written by the Author(s). Prof. Dr. Ir. Fred van Keulen, Dean of 3mE.
+
+---
+
+## References
+
+<a id="1">[1]</a>
+S. Gros and M. Zanon, "Data-Driven Economic NMPC Using Reinforcement Learning," in _IEEE Transactions on Automatic Control_, vol. 65, no. 2, pp. 636-648, Feb. 2020, doi: 10.1109/TAC.2019.2913768.
+
+<a id="2">[2]</a>
+H. N. Esfahani, A. B. Kordabad and S. Gros, "Approximate Robust NMPC using Reinforcement Learning," _2021 European Control Conference (ECC)_, 2021, pp. 132-137, doi: 10.23919/ECC54610.2021.9655129.
+
+<a id="3">[3]</a>
+W. Cai, A. B. Kordabad, H. N. Esfahani, A. M. Lekkas and S. Gros, "MPC-based Reinforcement Learning for a Simplified Freight Mission of Autonomous Surface Vehicles," _2021 60th IEEE Conference on Decision and Control (CDC)_, 2021, pp. 2990-2995, doi: 10.1109/CDC45484.2021.9683750.
```

### Comparing `mpcrl-1.2.0rc3/src/mpcrl.egg-info/SOURCES.txt` & `mpcrl-1.2.0rc4/src/mpcrl.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 src/mpcrl.egg-info/requires.txt
 src/mpcrl.egg-info/top_level.txt
 src/mpcrl/agents/lstd_dpg.py
 src/mpcrl/agents/lstd_q_learning.py
 src/mpcrl/agents/common/agent.py
 src/mpcrl/agents/common/globopt_learning_agent.py
 src/mpcrl/agents/common/learning_agent.py
+src/mpcrl/agents/common/offpolicy_rl_agent copy.py
 src/mpcrl/agents/common/rl_learning_agent.py
 src/mpcrl/core/__init__.py
 src/mpcrl/core/callbacks.py
 src/mpcrl/core/errors.py
 src/mpcrl/core/experience.py
 src/mpcrl/core/exploration.py
 src/mpcrl/core/parameters.py
 src/mpcrl/core/schedulers.py
 src/mpcrl/core/update.py
+src/mpcrl/core/warmstart.py
 src/mpcrl/optim/__init__.py
 src/mpcrl/optim/adam.py
 src/mpcrl/optim/base_optimizer.py
 src/mpcrl/optim/gradient_based_optimizer.py
 src/mpcrl/optim/gradient_descent.py
 src/mpcrl/optim/gradient_free_optimizer.py
 src/mpcrl/optim/newton_method.py
```

### Comparing `mpcrl-1.2.0rc3/tests/test_core.py` & `mpcrl-1.2.0rc4/tests/test_core.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,566 +1,566 @@
-import pickle
-import unittest
-from collections.abc import Iterator
-from copy import deepcopy
-from itertools import product
-from random import shuffle
-from typing import Union
-from unittest.mock import Mock
-
-import casadi as cs
-import numpy as np
-from parameterized import parameterized
-
-from mpcrl import (
-    ExperienceReplay,
-    LearnableParameter,
-    LearnableParametersDict,
-    MpcSolverError,
-    MpcSolverWarning,
-    UpdateError,
-    UpdateStrategy,
-    UpdateWarning,
-)
-from mpcrl import exploration as E
-from mpcrl import schedulers as S
-from mpcrl.core.errors import (
-    raise_or_warn_on_mpc_failure,
-    raise_or_warn_on_update_failure,
-)
-
-
-def do_test_str_and_repr(testcase: unittest.TestCase, obj: S.Scheduler) -> None:
-    testcase.assertIn(obj.__class__.__name__, obj.__str__())
-    testcase.assertIn(obj.__class__.__name__, obj.__repr__())
-
-
-def do_test_similar_schedulers(
-    testcase: unittest.TestCase, obj1: S.Scheduler, obj2: S.Scheduler
-) -> None:
-    dict1 = obj1.__dict__
-    dict2 = obj2.__dict__
-    for name, val1 in dict1.items():
-        val2 = dict2[name]
-        if hasattr(val1, "__iter__"):
-            testcase.assertListEqual(
-                [next(val1) for _ in range(10)], [next(val2) for _ in range(10)]
-            )
-        else:
-            testcase.assertEqual(val1, val2)
-
-
-class TestErrors(unittest.TestCase):
-    @parameterized.expand([(False,), (True,)])
-    def test_raise_or_warn_on_mpc_failure__raises_or_warns(self, raises: bool):
-        msg = "This is a message"
-        context = (
-            self.assertRaisesRegex(MpcSolverError, msg)
-            if raises
-            else self.assertWarnsRegex(MpcSolverWarning, msg)
-        )
-        with context:
-            raise_or_warn_on_mpc_failure(msg, raises)
-
-    @parameterized.expand([(False,), (True,)])
-    def test_raise_or_warn_on_update_failure__raises_or_warns(self, raises: bool):
-        msg = "This is a message"
-        context = (
-            self.assertRaisesRegex(UpdateError, msg)
-            if raises
-            else self.assertWarnsRegex(UpdateWarning, msg)
-        )
-        with context:
-            raise_or_warn_on_update_failure(msg, raises)
-
-
-class TestExperienceReplay(unittest.TestCase):
-    def test_init__initializes_memory_correctly(self):
-        items = [object(), object(), object()]
-        maxlen = 2
-        mem = ExperienceReplay[object](items, maxlen=maxlen, seed=50)
-        self.assertEqual(mem.maxlen, maxlen)
-        self.assertNotIn(items[0], mem)
-        self.assertIn(items[1], mem)
-        self.assertIn(items[2], mem)
-        self.assertIsInstance(mem.np_random, np.random.Generator)
-
-    def test_sample__raises__with_no_maxlen_and_percentage_size(self):
-        mem = ExperienceReplay[tuple[np.ndarray, float]](maxlen=None, sample_size=0.0)
-        with self.assertRaises(AssertionError):
-            list(mem.sample())
-
-    @parameterized.expand([(0,), (float(0),)])
-    def test_sample__with_zero_samples__returns_no_samples(self, n: Union[int, float]):
-        mem = ExperienceReplay[tuple[np.ndarray, float]](maxlen=100, sample_size=n)
-        self.assertListEqual(list(mem.sample()), [])
-
-    @parameterized.expand([(10,), (0.1,)])
-    def test_sample__returns_right_sample_size(self, n: Union[int, float]):
-        N = 100
-        Nsample = 10
-        mem = ExperienceReplay[int](maxlen=N, sample_size=n)
-        mem.extend(range(N))
-        sample = list(mem.sample())
-        self.assertEqual(len(sample), Nsample)
-        for item in sample:
-            self.assertIn(item, mem)
-
-    @parameterized.expand([(20, 10), (20, 0.5), (0.2, 10), (0.2, 0.5)])
-    def test_sample__latest_n__includes_latest_n_items(
-        self, n: Union[int, float], last_n: Union[int, float]
-    ):
-        N = 100
-        Nsample = 20
-        Nlast = 10
-        mem = ExperienceReplay[int](maxlen=N, sample_size=n, include_latest=last_n)
-        mem.extend(range(N))
-        sample = list(mem.sample())
-        self.assertEqual(len(sample), Nsample)
-        for item in sample:
-            self.assertIn(item, mem)
-        for item in range(N - Nlast, N):
-            self.assertIn(item, sample)
-
-    def test_deepcopy(self):
-        maxlen = np.random.randint(10, 100)
-        sample_size, include_latest = np.random.uniform(size=2)
-        mem = ExperienceReplay[int](
-            maxlen=maxlen, sample_size=sample_size, include_latest=include_latest
-        )
-        mem_copy = deepcopy(mem)
-        self.assertEqual(mem.maxlen, mem_copy.maxlen)
-        self.assertEqual(mem.sample_size, mem_copy.sample_size)
-        self.assertEqual(mem.include_latest, mem_copy.include_latest)
-        self.assertIsInstance(mem_copy.np_random, np.random.Generator)
-
-
-class TestSchedulers(unittest.TestCase):
-    def test_no_scheduling__step__does_not_update_value(self):
-        scheduler = S.NoScheduling(init_value=None)
-        scheduler.step()
-        self.assertIsNone(scheduler.value)
-        do_test_str_and_repr(self, scheduler)
-
-    def test_exponential_scheduler__step__updates_value_correctly(self):
-        K = 20
-        x0 = np.random.randn()
-        factor = np.random.rand()
-        x_expected = x0 * factor ** np.arange(K)
-        scheduler = S.ExponentialScheduler(x0, factor)
-        x_actual = []
-        for _ in range(K):
-            x_actual.append(scheduler.value)
-            scheduler.step()
-        np.testing.assert_allclose(x_expected, x_actual)
-        do_test_str_and_repr(self, scheduler)
-
-    def test_linear_scheduler__step__updates_value_correctly(self):
-        # sourcery skip: class-extract-method
-        K = 20
-        x0 = np.random.rand() * 10
-        xf = np.random.rand() * 10
-        x_expected = np.linspace(x0, xf, K + 1)
-        scheduler = S.LinearScheduler(x0, xf, K)
-        x_actual = []
-        for _ in range(K):
-            x_actual.append(scheduler.value)
-            scheduler.step()
-        x_actual.append(scheduler.value)
-        with self.assertRaises(StopIteration):
-            scheduler.step()
-        np.testing.assert_allclose(x_expected, x_actual)
-        do_test_str_and_repr(self, scheduler)
-
-    def test_loglinear_scheduler__step__updates_value_correctly(self):
-        # sourcery skip: class-extract-method
-        K = 20
-        base = np.random.rand() + 1 * 10
-        x0 = np.random.randn() + 3
-        xf = np.random.randn()
-        x_expected = np.logspace(x0, xf, K + 1, base=base)
-        scheduler = S.LogLinearScheduler(base**x0, base**xf, K)
-        x_actual = []
-        for _ in range(K):
-            x_actual.append(scheduler.value)
-            scheduler.step()
-        x_actual.append(scheduler.value)
-        with self.assertRaises(StopIteration):
-            scheduler.step()
-        np.testing.assert_allclose(x_expected, x_actual)
-        do_test_str_and_repr(self, scheduler)
-
-    def test_deepcopy(self):
-        K = np.random.randint(10, 20)
-        base = np.random.rand() + 1 * 10
-        x0 = np.random.randn() + 3
-        xf = np.random.randn()
-        scheduler = S.LogLinearScheduler(base**x0, base**xf, K)
-        scheduler_copy = deepcopy(scheduler)
-        do_test_similar_schedulers(self, scheduler, scheduler_copy)
-
-    def test_chain(self):
-        # create a list of random schedulers
-        rd, ri = np.random.rand, np.random.randint
-        mk1 = lambda: (S.NoScheduling(rd()), ri(10, 100))
-        mk2 = lambda: (S.ExponentialScheduler(*rd(2)), ri(10, 100))
-        mk3 = lambda: S.LinearScheduler(*rd(2), ri(10, 100))
-        mk4 = lambda: S.LogLinearScheduler(*rd(2), ri(10, 100))
-        schedulers = []
-        for mk in (mk1, mk2, mk3, mk4):
-            for _ in range(ri(1, 5)):
-                schedulers.append(mk())
-        shuffle(schedulers)
-
-        # extract the expected values
-        values_expected = []
-        schedulers_ = deepcopy(schedulers)
-        for scheduler in schedulers_:
-            if isinstance(scheduler, tuple):
-                scheduler, K = scheduler
-                while True:
-                    values_expected.append(scheduler.value)
-                    scheduler.step()
-                    K -= 1
-                    if K == 0:
-                        break
-            else:
-                while True:
-                    values_expected.append(scheduler.value)
-                    try:
-                        scheduler.step()
-                    except StopIteration:
-                        break
-
-        # create the chain and extract the actual values
-        scheduler = S.Chain(schedulers)
-        values_actual = []
-        while True:
-            values_actual.append(scheduler.value)
-            try:
-                scheduler.step()
-            except StopIteration:
-                break
-
-        # test
-        steps_expected = sum(
-            sc[1] if isinstance(sc, tuple) else sc.total_steps + 1 for sc in schedulers
-        )
-        self.assertEqual(len(values_actual), steps_expected)
-        self.assertEqual(len(values_expected), len(values_actual))
-        np.testing.assert_array_equal(values_expected, values_actual)
-
-
-class TestExploration(unittest.TestCase):
-    def test_no_exploration__never_explores(self):
-        exploration = E.NoExploration()
-        self.assertFalse(exploration.can_explore())
-        with self.assertRaisesRegex(
-            NotImplementedError, "Perturbation not implemented in NoExploration"
-        ):
-            exploration.perturbation()
-        exploration.step()  # does nothing
-        do_test_str_and_repr(self, exploration)
-
-    def test_greedy_exploration__instantiates_np_random(self):
-        exploration = E.GreedyExploration(strength=0.5)
-        self.assertIsInstance(exploration.np_random, np.random.Generator)
-
-    def test_greedy_exploration__always_explores(self):
-        exploration = E.GreedyExploration(strength=0.5)
-        self.assertTrue(exploration.can_explore())
-        do_test_str_and_repr(self, exploration)
-
-    @parameterized.expand([("uniform",), ("normal",), ("standard_normal",)])
-    def test_greedy_exploration__perturbs(self, method: str):
-        exploration = E.GreedyExploration(strength=0.5)
-        exploration.perturbation(method)
-
-    def test_epsilon_greedy_exploration__properties_return_right_values(self):
-        epsilon, epsilon_decay_rate = 0.7, 0.75
-        strength, strength_decay_rate = 0.5, 0.75
-        epsilon_scheduler = S.ExponentialScheduler(epsilon, epsilon_decay_rate)
-        strength_scheduler = S.ExponentialScheduler(strength, strength_decay_rate)
-        exploration = E.EpsilonGreedyExploration(
-            epsilon=epsilon_scheduler, strength=strength_scheduler, seed=42
-        )
-        self.assertEqual(exploration.strength, strength)
-        self.assertEqual(exploration.epsilon, epsilon)
-        do_test_str_and_repr(self, exploration)
-
-    def test_epsilon_greedy_exploration__never_explores__with_zero_epsilon(self):
-        epsilon, epsilon_decay_rate = 0.0, 0.75
-        strength, strength_decay_rate = 0.5, 0.75
-        epsilon_scheduler = S.ExponentialScheduler(epsilon, epsilon_decay_rate)
-        strength_scheduler = S.ExponentialScheduler(strength, strength_decay_rate)
-        exploration = E.EpsilonGreedyExploration(
-            epsilon=epsilon_scheduler, strength=strength_scheduler, seed=42
-        )
-        self.assertFalse(any(exploration.can_explore() for _ in range(100)))
-
-    def test_epsilon_greedy_exploration__sometimes_explores(self):
-        epsilon, epsilon_decay_rate = 0.7, 0.75
-        strength, strength_decay_rate = 0.5, 0.75
-        epsilon_scheduler = S.ExponentialScheduler(epsilon, epsilon_decay_rate)
-        strength_scheduler = S.ExponentialScheduler(strength, strength_decay_rate)
-        exploration = E.EpsilonGreedyExploration(
-            epsilon=epsilon_scheduler, strength=strength_scheduler, seed=42
-        )
-        self.assertFalse(exploration.can_explore())
-        found_true, found_false = False, False
-        for _ in range(100):
-            explore = exploration.can_explore()
-            if explore:
-                found_true = True
-            else:
-                found_false = True
-            if found_true and found_false:
-                break
-        self.assertTrue(found_true and found_false)
-
-    def test_epsilon_greedy_exploration__decays_strength(self):
-        class MockScheduler(S.NoScheduling):
-            ...
-
-        epsilon_scheduler = MockScheduler(None)
-        strength_scheduler = MockScheduler(None)
-        epsilon_scheduler.step = Mock()
-        strength_scheduler.step = Mock()
-        exploration = E.EpsilonGreedyExploration(
-            epsilon=epsilon_scheduler, strength=strength_scheduler, seed=42
-        )
-
-        exploration.step()
-
-        epsilon_scheduler.step.assert_called_once()
-        strength_scheduler.step.assert_called_once()
-
-    def test_stepwise_exploration__has_same_hook_as_base_exploration(self):
-        hook = Mock()
-        base_exploration = Mock()
-        base_exploration.hook = hook
-        exploration = E.StepWiseExploration(base_exploration, 5, 10)
-        self.assertIs(exploration.hook, hook)
-
-    @parameterized.expand([(True,), (False,)])
-    def test_stepwise_exploration__turns_base_exploration_into_steps(
-        self, stepwise_step: bool
-    ):
-        base_exploration = E.EpsilonGreedyExploration(0.5, 0.5, seed=0)
-        base_exploration.step = Mock()
-        step_size = 5
-        cycles = 10
-        exploration = E.StepWiseExploration(base_exploration, step_size, stepwise_step)
-        can_explores, perturbations = [], []
-        for _ in range(cycles):
-            can_explores.append([])
-            perturbations.append([])
-            for _ in range(step_size):
-                can_explores[-1].append(exploration.can_explore())
-                perturbations[-1].append(exploration.perturbation("uniform"))
-                exploration.step()
-
-        for can_explores_cycle, perturbations_cycle in zip(can_explores, perturbations):
-            self.assertTrue(np.unique(can_explores_cycle).size == 1)
-            self.assertTrue(np.unique(perturbations_cycle).size == 1)
-        if stepwise_step:
-            self.assertTrue(len(base_exploration.step.mock_calls) == cycles)
-        else:
-            self.assertTrue(len(base_exploration.step.mock_calls) == cycles * step_size)
-
-    def test_deepcopy(self):
-        epsilon, epsilon_decay_rate = 0.0, 0.75
-        strength, strength_decay_rate = 0.5, 0.75
-        epsilon_scheduler = S.ExponentialScheduler(epsilon, epsilon_decay_rate)
-        strength_scheduler = S.ExponentialScheduler(strength, strength_decay_rate)
-        exploration = E.EpsilonGreedyExploration(
-            epsilon=epsilon_scheduler, strength=strength_scheduler, seed=42
-        )
-        exploration_copy = deepcopy(exploration)
-        self.assertEqual(exploration._hook, exploration_copy._hook)
-        do_test_similar_schedulers(
-            self, exploration.epsilon_scheduler, exploration_copy.epsilon_scheduler
-        )
-        do_test_similar_schedulers(
-            self, exploration.strength_scheduler, exploration_copy.strength_scheduler
-        )
-
-
-class TestParameters(unittest.TestCase):
-    @parameterized.expand(map(lambda i: (i,), range(3)))
-    def test_learnable_parameter_init__raises__with_unbroadcastable_args(self, i: int):
-        args = [5, 0, 10]
-        args[i] = np.random.rand(2, 2, 2)
-        with self.assertRaises(ValueError):
-            LearnableParameter("theta", 10, *args)
-
-    def test_learnable_parameter_init_and_update__raise__with_value_outside_range(self):
-        with self.assertRaises(ValueError):
-            LearnableParameter("theta", 10, -5, 0, 10)
-        par = LearnableParameter("theta", 10, 5, 0, 10)
-        with self.assertRaises(ValueError):
-            par._update_value(-5)
-
-    @parameterized.expand([(False,), (True,)])
-    def test_parameters_dict__init__initializes_properly(self, empty_init: bool):
-        p1 = LearnableParameter("theta1", 10, 0.0)
-        p2 = LearnableParameter("theta2", 11, 0.0)
-        PARS = [p1, p2]
-        if empty_init:
-            pars = LearnableParametersDict()
-            pars.update(iter(PARS))
-        else:
-            pars = LearnableParametersDict(iter(PARS))
-        self.assertEqual(len(pars), 2)
-        for p in PARS:
-            self.assertIn(p.name, pars)
-            self.assertIs(pars[p.name], p)
-
-    @parameterized.expand([(False,), (True,)])
-    def test_parameters_dict__setitem__raises_with_wrong_name(self, wrong_name: bool):
-        p = LearnableParameter("t", 10, 0.0)
-        pars = LearnableParametersDict()
-        if wrong_name:
-            with self.assertRaisesRegex(
-                AssertionError, r"Key 't_hello_there' must match parameter name 't'."
-            ):
-                pars[f"{p.name}_hello_there"] = p
-        else:
-            pars[p.name] = p
-
-    @parameterized.expand(
-        map(
-            lambda m: (m,),
-            ["setitem", "update", "setdefault", "delitem", "pop", "popitem", "clear"],
-        )
-    )
-    def test_parameters_dict__caches_get_cleared_properly(self, method: str):
-        array_equal = np.testing.assert_array_equal
-        cat = np.concatenate
-
-        def check(pars, PARS):
-            self.assertEqual(pars.size, sum(p.size for p in PARS))
-            if len(pars) > 0 and len(PARS) > 0:
-                array_equal(pars.lb, cat([p.lb.flatten("F") for p in PARS]))
-                array_equal(pars.ub, cat([p.ub.flatten("F") for p in PARS]))
-                array_equal(pars.value, cat([p.value.flatten("F") for p in PARS]))
-                sym1 = cs.veccat(*(p.sym for p in pars.values()))
-                sym2 = cs.veccat(*(p.sym for p in PARS))
-                array_equal(cs.evalf(cs.simplify(sym1 - sym2)), 0)
-            else:
-                self.assertTupleEqual(pars.lb.shape, (0,))
-                self.assertTupleEqual(pars.ub.shape, (0,))
-                self.assertTupleEqual(pars.value.shape, (0,))
-
-        p1 = LearnableParameter[float](
-            "t1", (4, 6), 1.0, -1.0, 2.0, cs.SX.sym("t1", 4, 6)
-        )
-        p2 = LearnableParameter[float]("t2", 2, 2.0, -2.0, 3.0, cs.SX.sym("t2", 2))
-        PARS = [p1, p2]
-        pars = LearnableParametersDict(PARS)
-        check(pars, PARS)
-
-        p3 = LearnableParameter[float]("t3", 3, 3.0, -3.0, 4.0, cs.SX.sym("t3", 3))
-        if method == "setitem":
-            pars[p3.name] = p3
-            PARS = [p1, p2, p3]
-        elif method == "update":
-            pars.update([p3])
-            PARS = [p1, p2, p3]
-        elif method == "setdefault":
-            pars.setdefault(p3)
-            PARS = [p1, p2, p3]
-        elif method == "delitem":
-            del pars[p2.name]
-            PARS = [p1]
-        elif method == "pop":
-            pars.pop(p1.name)
-            PARS = [p2]
-        elif method == "popitem":
-            pars.popitem()
-            PARS = [p1]
-        elif method == "clear":
-            pars.clear()
-            PARS = []
-
-        check(pars, PARS)
-
-    def test_parameters_dict__stringify(self):
-        p1 = LearnableParameter[None]("p1", 1, 1)
-        p2 = LearnableParameter[None]("p2", 1, 2.0)
-        p3 = LearnableParameter[None]("p3", 100, np.random.randint(0, 100, size=100))
-        p4 = LearnableParameter[None]("p4", 100, np.random.rand(100))
-        pars = LearnableParametersDict((p1, p2, p3, p4))
-        S = pars.stringify()
-        for p in [p1, p2, p3, p4]:
-            self.assertIn(p.name, S)
-
-    @parameterized.expand(product([cs.SX, cs.MX], [False, True]))
-    def test_deepcopy(self, cstype: Union[cs.SX, cs.MX], copy: bool):
-        shape = (5, 2)
-        theta_sym = cstype.sym("theta", shape)
-        f = theta_sym[0]
-        df = cs.evalf(cs.jacobian(f, theta_sym)[0])
-        p1 = LearnableParameter[float]("theta", shape, 1, -1, 2, sym={"v": theta_sym})
-        pars = LearnableParametersDict((p1,))
-        if copy:
-            new_pars = pars.copy(deep=True)
-        else:
-            new_pars: LearnableParametersDict = pickle.loads(pickle.dumps(pars))
-        p2: LearnableParameter = new_pars["theta"]
-        self.assertIsNot(p1, p2)
-        self.assertEqual(p1.name, p2.name)
-        self.assertEqual(p1.shape, p2.shape)
-        self.assertEqual(p1.size, p2.size)
-        np.testing.assert_array_equal(p1.value, p2.value)
-        np.testing.assert_array_equal(p1.lb, p2.lb)
-        np.testing.assert_array_equal(p1.ub, p2.ub)
-        np.testing.assert_equal(df, cs.evalf(cs.jacobian(f, p1.sym["v"])[0]))
-        if copy:
-            self.assertIsNot(p1.sym, p2.sym)
-            self.assertIsNot(p1.sym["v"], p2.sym["v"])
-            np.testing.assert_equal(df, cs.evalf(cs.jacobian(f, p2.sym["v"])[0]))
-        else:
-            self.assertFalse(hasattr(p2, "sym"))
-
-
-class TestUpdateStrategy(unittest.TestCase):
-    def test__is_iterable(self):
-        strategy = UpdateStrategy(5)
-        self.assertIsInstance(next(strategy), bool)
-        self.assertIsInstance(iter(strategy), Iterator)
-
-    def test_can_update__has_right_frequency(self):
-        N = 50
-        freq = 3
-        strategy = UpdateStrategy(freq)
-        flags = np.asarray([strategy.can_update() for _ in range(N)])
-        mask = np.asarray(([False] * (freq - 1) + [True]) * (N // freq + 1))[:N]
-        self.assertEqual(flags.sum(), N // freq)
-        self.assertTrue(flags[mask].all())
-        self.assertTrue((~flags[~mask]).all())
-
-    def test_can_update__with_skip_first__skips_first_updates_correctly(self):
-        N = 50
-        freq = 3
-        skip = 2
-        strategy = UpdateStrategy(freq, skip_first=skip)
-        flags = np.asarray([strategy.can_update() for _ in range(N)])
-        mask = np.asarray(([False] * (freq - 1) + [True]) * (N // freq + 1))[:N]
-        self.assertEqual(flags.sum(), N // freq - skip)
-        self.assertTrue((~flags[mask][:skip]).all())
-        self.assertTrue(flags[mask][skip:].all())
-        self.assertTrue((~flags[~mask]).all())
-
-    def test_deepcopy(self):
-        strategy = UpdateStrategy(5, "on_episode_end", 3)
-        strategy_copy = deepcopy(strategy)
-        self.assertEqual(strategy.frequency, strategy_copy.frequency)
-        self.assertEqual(strategy.hook, strategy_copy.hook)
-        self.assertListEqual(
-            [next(strategy._update_cycle) for _ in range(50)],
-            [next(strategy_copy._update_cycle) for _ in range(50)],
-        )
-
-
-if __name__ == "__main__":
-    unittest.main()
+import pickle
+import unittest
+from collections.abc import Iterator
+from copy import deepcopy
+from itertools import product
+from random import shuffle
+from typing import Union
+from unittest.mock import Mock
+
+import casadi as cs
+import numpy as np
+from parameterized import parameterized
+
+from mpcrl import (
+    ExperienceReplay,
+    LearnableParameter,
+    LearnableParametersDict,
+    MpcSolverError,
+    MpcSolverWarning,
+    UpdateError,
+    UpdateStrategy,
+    UpdateWarning,
+)
+from mpcrl import exploration as E
+from mpcrl import schedulers as S
+from mpcrl.core.errors import (
+    raise_or_warn_on_mpc_failure,
+    raise_or_warn_on_update_failure,
+)
+
+
+def do_test_str_and_repr(testcase: unittest.TestCase, obj: S.Scheduler) -> None:
+    testcase.assertIn(obj.__class__.__name__, obj.__str__())
+    testcase.assertIn(obj.__class__.__name__, obj.__repr__())
+
+
+def do_test_similar_schedulers(
+    testcase: unittest.TestCase, obj1: S.Scheduler, obj2: S.Scheduler
+) -> None:
+    dict1 = obj1.__dict__
+    dict2 = obj2.__dict__
+    for name, val1 in dict1.items():
+        val2 = dict2[name]
+        if hasattr(val1, "__iter__"):
+            testcase.assertListEqual(
+                [next(val1) for _ in range(10)], [next(val2) for _ in range(10)]
+            )
+        else:
+            testcase.assertEqual(val1, val2)
+
+
+class TestErrors(unittest.TestCase):
+    @parameterized.expand([(False,), (True,)])
+    def test_raise_or_warn_on_mpc_failure__raises_or_warns(self, raises: bool):
+        msg = "This is a message"
+        context = (
+            self.assertRaisesRegex(MpcSolverError, msg)
+            if raises
+            else self.assertWarnsRegex(MpcSolverWarning, msg)
+        )
+        with context:
+            raise_or_warn_on_mpc_failure(msg, raises)
+
+    @parameterized.expand([(False,), (True,)])
+    def test_raise_or_warn_on_update_failure__raises_or_warns(self, raises: bool):
+        msg = "This is a message"
+        context = (
+            self.assertRaisesRegex(UpdateError, msg)
+            if raises
+            else self.assertWarnsRegex(UpdateWarning, msg)
+        )
+        with context:
+            raise_or_warn_on_update_failure(msg, raises)
+
+
+class TestExperienceReplay(unittest.TestCase):
+    def test_init__initializes_memory_correctly(self):
+        items = [object(), object(), object()]
+        maxlen = 2
+        mem = ExperienceReplay[object](items, maxlen=maxlen, seed=50)
+        self.assertEqual(mem.maxlen, maxlen)
+        self.assertNotIn(items[0], mem)
+        self.assertIn(items[1], mem)
+        self.assertIn(items[2], mem)
+        self.assertIsInstance(mem.np_random, np.random.Generator)
+
+    def test_sample__raises__with_no_maxlen_and_percentage_size(self):
+        mem = ExperienceReplay[tuple[np.ndarray, float]](maxlen=None, sample_size=0.0)
+        with self.assertRaises(AssertionError):
+            list(mem.sample())
+
+    @parameterized.expand([(0,), (float(0),)])
+    def test_sample__with_zero_samples__returns_no_samples(self, n: Union[int, float]):
+        mem = ExperienceReplay[tuple[np.ndarray, float]](maxlen=100, sample_size=n)
+        self.assertListEqual(list(mem.sample()), [])
+
+    @parameterized.expand([(10,), (0.1,)])
+    def test_sample__returns_right_sample_size(self, n: Union[int, float]):
+        N = 100
+        Nsample = 10
+        mem = ExperienceReplay[int](maxlen=N, sample_size=n)
+        mem.extend(range(N))
+        sample = list(mem.sample())
+        self.assertEqual(len(sample), Nsample)
+        for item in sample:
+            self.assertIn(item, mem)
+
+    @parameterized.expand([(20, 10), (20, 0.5), (0.2, 10), (0.2, 0.5)])
+    def test_sample__latest_n__includes_latest_n_items(
+        self, n: Union[int, float], last_n: Union[int, float]
+    ):
+        N = 100
+        Nsample = 20
+        Nlast = 10
+        mem = ExperienceReplay[int](maxlen=N, sample_size=n, include_latest=last_n)
+        mem.extend(range(N))
+        sample = list(mem.sample())
+        self.assertEqual(len(sample), Nsample)
+        for item in sample:
+            self.assertIn(item, mem)
+        for item in range(N - Nlast, N):
+            self.assertIn(item, sample)
+
+    def test_deepcopy(self):
+        maxlen = np.random.randint(10, 100)
+        sample_size, include_latest = np.random.uniform(size=2)
+        mem = ExperienceReplay[int](
+            maxlen=maxlen, sample_size=sample_size, include_latest=include_latest
+        )
+        mem_copy = deepcopy(mem)
+        self.assertEqual(mem.maxlen, mem_copy.maxlen)
+        self.assertEqual(mem.sample_size, mem_copy.sample_size)
+        self.assertEqual(mem.include_latest, mem_copy.include_latest)
+        self.assertIsInstance(mem_copy.np_random, np.random.Generator)
+
+
+class TestSchedulers(unittest.TestCase):
+    def test_no_scheduling__step__does_not_update_value(self):
+        scheduler = S.NoScheduling(init_value=None)
+        scheduler.step()
+        self.assertIsNone(scheduler.value)
+        do_test_str_and_repr(self, scheduler)
+
+    def test_exponential_scheduler__step__updates_value_correctly(self):
+        K = 20
+        x0 = np.random.randn()
+        factor = np.random.rand()
+        x_expected = x0 * factor ** np.arange(K)
+        scheduler = S.ExponentialScheduler(x0, factor)
+        x_actual = []
+        for _ in range(K):
+            x_actual.append(scheduler.value)
+            scheduler.step()
+        np.testing.assert_allclose(x_expected, x_actual)
+        do_test_str_and_repr(self, scheduler)
+
+    def test_linear_scheduler__step__updates_value_correctly(self):
+        # sourcery skip: class-extract-method
+        K = 20
+        x0 = np.random.rand() * 10
+        xf = np.random.rand() * 10
+        x_expected = np.linspace(x0, xf, K + 1)
+        scheduler = S.LinearScheduler(x0, xf, K)
+        x_actual = []
+        for _ in range(K):
+            x_actual.append(scheduler.value)
+            scheduler.step()
+        x_actual.append(scheduler.value)
+        with self.assertRaises(StopIteration):
+            scheduler.step()
+        np.testing.assert_allclose(x_expected, x_actual)
+        do_test_str_and_repr(self, scheduler)
+
+    def test_loglinear_scheduler__step__updates_value_correctly(self):
+        # sourcery skip: class-extract-method
+        K = 20
+        base = np.random.rand() + 1 * 10
+        x0 = np.random.randn() + 3
+        xf = np.random.randn()
+        x_expected = np.logspace(x0, xf, K + 1, base=base)
+        scheduler = S.LogLinearScheduler(base**x0, base**xf, K)
+        x_actual = []
+        for _ in range(K):
+            x_actual.append(scheduler.value)
+            scheduler.step()
+        x_actual.append(scheduler.value)
+        with self.assertRaises(StopIteration):
+            scheduler.step()
+        np.testing.assert_allclose(x_expected, x_actual)
+        do_test_str_and_repr(self, scheduler)
+
+    def test_deepcopy(self):
+        K = np.random.randint(10, 20)
+        base = np.random.rand() + 1 * 10
+        x0 = np.random.randn() + 3
+        xf = np.random.randn()
+        scheduler = S.LogLinearScheduler(base**x0, base**xf, K)
+        scheduler_copy = deepcopy(scheduler)
+        do_test_similar_schedulers(self, scheduler, scheduler_copy)
+
+    def test_chain(self):
+        # create a list of random schedulers
+        rd, ri = np.random.rand, np.random.randint
+        mk1 = lambda: (S.NoScheduling(rd()), ri(10, 100))
+        mk2 = lambda: (S.ExponentialScheduler(*rd(2)), ri(10, 100))
+        mk3 = lambda: S.LinearScheduler(*rd(2), ri(10, 100))
+        mk4 = lambda: S.LogLinearScheduler(*rd(2), ri(10, 100))
+        schedulers = []
+        for mk in (mk1, mk2, mk3, mk4):
+            for _ in range(ri(1, 5)):
+                schedulers.append(mk())
+        shuffle(schedulers)
+
+        # extract the expected values
+        values_expected = []
+        schedulers_ = deepcopy(schedulers)
+        for scheduler in schedulers_:
+            if isinstance(scheduler, tuple):
+                scheduler, K = scheduler
+                while True:
+                    values_expected.append(scheduler.value)
+                    scheduler.step()
+                    K -= 1
+                    if K == 0:
+                        break
+            else:
+                while True:
+                    values_expected.append(scheduler.value)
+                    try:
+                        scheduler.step()
+                    except StopIteration:
+                        break
+
+        # create the chain and extract the actual values
+        scheduler = S.Chain(schedulers)
+        values_actual = []
+        while True:
+            values_actual.append(scheduler.value)
+            try:
+                scheduler.step()
+            except StopIteration:
+                break
+
+        # test
+        steps_expected = sum(
+            sc[1] if isinstance(sc, tuple) else sc.total_steps + 1 for sc in schedulers
+        )
+        self.assertEqual(len(values_actual), steps_expected)
+        self.assertEqual(len(values_expected), len(values_actual))
+        np.testing.assert_array_equal(values_expected, values_actual)
+
+
+class TestExploration(unittest.TestCase):
+    def test_no_exploration__never_explores(self):
+        exploration = E.NoExploration()
+        self.assertFalse(exploration.can_explore())
+        with self.assertRaisesRegex(
+            NotImplementedError, "Perturbation not implemented in NoExploration"
+        ):
+            exploration.perturbation()
+        exploration.step()  # does nothing
+        do_test_str_and_repr(self, exploration)
+
+    def test_greedy_exploration__instantiates_np_random(self):
+        exploration = E.GreedyExploration(strength=0.5)
+        self.assertIsInstance(exploration.np_random, np.random.Generator)
+
+    def test_greedy_exploration__always_explores(self):
+        exploration = E.GreedyExploration(strength=0.5)
+        self.assertTrue(exploration.can_explore())
+        do_test_str_and_repr(self, exploration)
+
+    @parameterized.expand([("uniform",), ("normal",), ("standard_normal",)])
+    def test_greedy_exploration__perturbs(self, method: str):
+        exploration = E.GreedyExploration(strength=0.5)
+        exploration.perturbation(method)
+
+    def test_epsilon_greedy_exploration__properties_return_right_values(self):
+        epsilon, epsilon_decay_rate = 0.7, 0.75
+        strength, strength_decay_rate = 0.5, 0.75
+        epsilon_scheduler = S.ExponentialScheduler(epsilon, epsilon_decay_rate)
+        strength_scheduler = S.ExponentialScheduler(strength, strength_decay_rate)
+        exploration = E.EpsilonGreedyExploration(
+            epsilon=epsilon_scheduler, strength=strength_scheduler, seed=42
+        )
+        self.assertEqual(exploration.strength, strength)
+        self.assertEqual(exploration.epsilon, epsilon)
+        do_test_str_and_repr(self, exploration)
+
+    def test_epsilon_greedy_exploration__never_explores__with_zero_epsilon(self):
+        epsilon, epsilon_decay_rate = 0.0, 0.75
+        strength, strength_decay_rate = 0.5, 0.75
+        epsilon_scheduler = S.ExponentialScheduler(epsilon, epsilon_decay_rate)
+        strength_scheduler = S.ExponentialScheduler(strength, strength_decay_rate)
+        exploration = E.EpsilonGreedyExploration(
+            epsilon=epsilon_scheduler, strength=strength_scheduler, seed=42
+        )
+        self.assertFalse(any(exploration.can_explore() for _ in range(100)))
+
+    def test_epsilon_greedy_exploration__sometimes_explores(self):
+        epsilon, epsilon_decay_rate = 0.7, 0.75
+        strength, strength_decay_rate = 0.5, 0.75
+        epsilon_scheduler = S.ExponentialScheduler(epsilon, epsilon_decay_rate)
+        strength_scheduler = S.ExponentialScheduler(strength, strength_decay_rate)
+        exploration = E.EpsilonGreedyExploration(
+            epsilon=epsilon_scheduler, strength=strength_scheduler, seed=42
+        )
+        self.assertFalse(exploration.can_explore())
+        found_true, found_false = False, False
+        for _ in range(100):
+            explore = exploration.can_explore()
+            if explore:
+                found_true = True
+            else:
+                found_false = True
+            if found_true and found_false:
+                break
+        self.assertTrue(found_true and found_false)
+
+    def test_epsilon_greedy_exploration__decays_strength(self):
+        class MockScheduler(S.NoScheduling):
+            ...
+
+        epsilon_scheduler = MockScheduler(None)
+        strength_scheduler = MockScheduler(None)
+        epsilon_scheduler.step = Mock()
+        strength_scheduler.step = Mock()
+        exploration = E.EpsilonGreedyExploration(
+            epsilon=epsilon_scheduler, strength=strength_scheduler, seed=42
+        )
+
+        exploration.step()
+
+        epsilon_scheduler.step.assert_called_once()
+        strength_scheduler.step.assert_called_once()
+
+    def test_stepwise_exploration__has_same_hook_as_base_exploration(self):
+        hook = Mock()
+        base_exploration = Mock()
+        base_exploration.hook = hook
+        exploration = E.StepWiseExploration(base_exploration, 5, 10)
+        self.assertIs(exploration.hook, hook)
+
+    @parameterized.expand([(True,), (False,)])
+    def test_stepwise_exploration__turns_base_exploration_into_steps(
+        self, stepwise_step: bool
+    ):
+        base_exploration = E.EpsilonGreedyExploration(0.5, 0.5, seed=0)
+        base_exploration.step = Mock()
+        step_size = 5
+        cycles = 10
+        exploration = E.StepWiseExploration(base_exploration, step_size, stepwise_step)
+        can_explores, perturbations = [], []
+        for _ in range(cycles):
+            can_explores.append([])
+            perturbations.append([])
+            for _ in range(step_size):
+                can_explores[-1].append(exploration.can_explore())
+                perturbations[-1].append(exploration.perturbation("uniform"))
+                exploration.step()
+
+        for can_explores_cycle, perturbations_cycle in zip(can_explores, perturbations):
+            self.assertTrue(np.unique(can_explores_cycle).size == 1)
+            self.assertTrue(np.unique(perturbations_cycle).size == 1)
+        if stepwise_step:
+            self.assertTrue(len(base_exploration.step.mock_calls) == cycles)
+        else:
+            self.assertTrue(len(base_exploration.step.mock_calls) == cycles * step_size)
+
+    def test_deepcopy(self):
+        epsilon, epsilon_decay_rate = 0.0, 0.75
+        strength, strength_decay_rate = 0.5, 0.75
+        epsilon_scheduler = S.ExponentialScheduler(epsilon, epsilon_decay_rate)
+        strength_scheduler = S.ExponentialScheduler(strength, strength_decay_rate)
+        exploration = E.EpsilonGreedyExploration(
+            epsilon=epsilon_scheduler, strength=strength_scheduler, seed=42
+        )
+        exploration_copy = deepcopy(exploration)
+        self.assertEqual(exploration._hook, exploration_copy._hook)
+        do_test_similar_schedulers(
+            self, exploration.epsilon_scheduler, exploration_copy.epsilon_scheduler
+        )
+        do_test_similar_schedulers(
+            self, exploration.strength_scheduler, exploration_copy.strength_scheduler
+        )
+
+
+class TestParameters(unittest.TestCase):
+    @parameterized.expand(map(lambda i: (i,), range(3)))
+    def test_learnable_parameter_init__raises__with_unbroadcastable_args(self, i: int):
+        args = [5, 0, 10]
+        args[i] = np.random.rand(2, 2, 2)
+        with self.assertRaises(ValueError):
+            LearnableParameter("theta", 10, *args)
+
+    def test_learnable_parameter_init_and_update__raise__with_value_outside_range(self):
+        with self.assertRaises(ValueError):
+            LearnableParameter("theta", 10, -5, 0, 10)
+        par = LearnableParameter("theta", 10, 5, 0, 10)
+        with self.assertRaises(ValueError):
+            par._update_value(-5)
+
+    @parameterized.expand([(False,), (True,)])
+    def test_parameters_dict__init__initializes_properly(self, empty_init: bool):
+        p1 = LearnableParameter("theta1", 10, 0.0)
+        p2 = LearnableParameter("theta2", 11, 0.0)
+        PARS = [p1, p2]
+        if empty_init:
+            pars = LearnableParametersDict()
+            pars.update(iter(PARS))
+        else:
+            pars = LearnableParametersDict(iter(PARS))
+        self.assertEqual(len(pars), 2)
+        for p in PARS:
+            self.assertIn(p.name, pars)
+            self.assertIs(pars[p.name], p)
+
+    @parameterized.expand([(False,), (True,)])
+    def test_parameters_dict__setitem__raises_with_wrong_name(self, wrong_name: bool):
+        p = LearnableParameter("t", 10, 0.0)
+        pars = LearnableParametersDict()
+        if wrong_name:
+            with self.assertRaisesRegex(
+                AssertionError, r"Key 't_hello_there' must match parameter name 't'."
+            ):
+                pars[f"{p.name}_hello_there"] = p
+        else:
+            pars[p.name] = p
+
+    @parameterized.expand(
+        map(
+            lambda m: (m,),
+            ["setitem", "update", "setdefault", "delitem", "pop", "popitem", "clear"],
+        )
+    )
+    def test_parameters_dict__caches_get_cleared_properly(self, method: str):
+        array_equal = np.testing.assert_array_equal
+        cat = np.concatenate
+
+        def check(pars, PARS):
+            self.assertEqual(pars.size, sum(p.size for p in PARS))
+            if len(pars) > 0 and len(PARS) > 0:
+                array_equal(pars.lb, cat([p.lb.flatten("F") for p in PARS]))
+                array_equal(pars.ub, cat([p.ub.flatten("F") for p in PARS]))
+                array_equal(pars.value, cat([p.value.flatten("F") for p in PARS]))
+                sym1 = cs.veccat(*(p.sym for p in pars.values()))
+                sym2 = cs.veccat(*(p.sym for p in PARS))
+                array_equal(cs.evalf(cs.simplify(sym1 - sym2)), 0)
+            else:
+                self.assertTupleEqual(pars.lb.shape, (0,))
+                self.assertTupleEqual(pars.ub.shape, (0,))
+                self.assertTupleEqual(pars.value.shape, (0,))
+
+        p1 = LearnableParameter[float](
+            "t1", (4, 6), 1.0, -1.0, 2.0, cs.SX.sym("t1", 4, 6)
+        )
+        p2 = LearnableParameter[float]("t2", 2, 2.0, -2.0, 3.0, cs.SX.sym("t2", 2))
+        PARS = [p1, p2]
+        pars = LearnableParametersDict(PARS)
+        check(pars, PARS)
+
+        p3 = LearnableParameter[float]("t3", 3, 3.0, -3.0, 4.0, cs.SX.sym("t3", 3))
+        if method == "setitem":
+            pars[p3.name] = p3
+            PARS = [p1, p2, p3]
+        elif method == "update":
+            pars.update([p3])
+            PARS = [p1, p2, p3]
+        elif method == "setdefault":
+            pars.setdefault(p3)
+            PARS = [p1, p2, p3]
+        elif method == "delitem":
+            del pars[p2.name]
+            PARS = [p1]
+        elif method == "pop":
+            pars.pop(p1.name)
+            PARS = [p2]
+        elif method == "popitem":
+            pars.popitem()
+            PARS = [p1]
+        elif method == "clear":
+            pars.clear()
+            PARS = []
+
+        check(pars, PARS)
+
+    def test_parameters_dict__stringify(self):
+        p1 = LearnableParameter[None]("p1", 1, 1)
+        p2 = LearnableParameter[None]("p2", 1, 2.0)
+        p3 = LearnableParameter[None]("p3", 100, np.random.randint(0, 100, size=100))
+        p4 = LearnableParameter[None]("p4", 100, np.random.rand(100))
+        pars = LearnableParametersDict((p1, p2, p3, p4))
+        S = pars.stringify()
+        for p in [p1, p2, p3, p4]:
+            self.assertIn(p.name, S)
+
+    @parameterized.expand(product([cs.SX, cs.MX], [False, True]))
+    def test_deepcopy(self, cstype: Union[cs.SX, cs.MX], copy: bool):
+        shape = (5, 2)
+        theta_sym = cstype.sym("theta", shape)
+        f = theta_sym[0]
+        df = cs.evalf(cs.jacobian(f, theta_sym)[0])
+        p1 = LearnableParameter[float]("theta", shape, 1, -1, 2, sym={"v": theta_sym})
+        pars = LearnableParametersDict((p1,))
+        if copy:
+            new_pars = pars.copy(deep=True)
+        else:
+            new_pars: LearnableParametersDict = pickle.loads(pickle.dumps(pars))
+        p2: LearnableParameter = new_pars["theta"]
+        self.assertIsNot(p1, p2)
+        self.assertEqual(p1.name, p2.name)
+        self.assertEqual(p1.shape, p2.shape)
+        self.assertEqual(p1.size, p2.size)
+        np.testing.assert_array_equal(p1.value, p2.value)
+        np.testing.assert_array_equal(p1.lb, p2.lb)
+        np.testing.assert_array_equal(p1.ub, p2.ub)
+        np.testing.assert_equal(df, cs.evalf(cs.jacobian(f, p1.sym["v"])[0]))
+        if copy:
+            self.assertIsNot(p1.sym, p2.sym)
+            self.assertIsNot(p1.sym["v"], p2.sym["v"])
+            np.testing.assert_equal(df, cs.evalf(cs.jacobian(f, p2.sym["v"])[0]))
+        else:
+            self.assertFalse(hasattr(p2, "sym"))
+
+
+class TestUpdateStrategy(unittest.TestCase):
+    def test__is_iterable(self):
+        strategy = UpdateStrategy(5)
+        self.assertIsInstance(next(strategy), bool)
+        self.assertIsInstance(iter(strategy), Iterator)
+
+    def test_can_update__has_right_frequency(self):
+        N = 50
+        freq = 3
+        strategy = UpdateStrategy(freq)
+        flags = np.asarray([strategy.can_update() for _ in range(N)])
+        mask = np.asarray(([False] * (freq - 1) + [True]) * (N // freq + 1))[:N]
+        self.assertEqual(flags.sum(), N // freq)
+        self.assertTrue(flags[mask].all())
+        self.assertTrue((~flags[~mask]).all())
+
+    def test_can_update__with_skip_first__skips_first_updates_correctly(self):
+        N = 50
+        freq = 3
+        skip = 2
+        strategy = UpdateStrategy(freq, skip_first=skip)
+        flags = np.asarray([strategy.can_update() for _ in range(N)])
+        mask = np.asarray(([False] * (freq - 1) + [True]) * (N // freq + 1))[:N]
+        self.assertEqual(flags.sum(), N // freq - skip)
+        self.assertTrue((~flags[mask][:skip]).all())
+        self.assertTrue(flags[mask][skip:].all())
+        self.assertTrue((~flags[~mask]).all())
+
+    def test_deepcopy(self):
+        strategy = UpdateStrategy(5, "on_episode_end", 3)
+        strategy_copy = deepcopy(strategy)
+        self.assertEqual(strategy.frequency, strategy_copy.frequency)
+        self.assertEqual(strategy.hook, strategy_copy.hook)
+        self.assertListEqual(
+            [next(strategy._update_cycle) for _ in range(50)],
+            [next(strategy_copy._update_cycle) for _ in range(50)],
+        )
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `mpcrl-1.2.0rc3/tests/test_optim.py` & `mpcrl-1.2.0rc4/tests/test_optim.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,461 +1,461 @@
-import unittest
-from itertools import product
-from unittest.mock import Mock
-
-import casadi as cs
-import numpy as np
-import torch
-from parameterized import parameterized
-
-from mpcrl import LearnableParameter, LearnableParametersDict
-from mpcrl import optim as O
-from mpcrl import schedulers as S
-from mpcrl.optim.gradient_based_optimizer import GradientBasedOptimizer
-
-np.random.seed(10)
-torch.manual_seed(0)
-torch.use_deterministic_algorithms(True)
-
-SMALL = 1e-270
-N_PARAMS = 5
-pars = np.random.randn(N_PARAMS)
-LEARNABLE_PARS = LearnableParametersDict(
-    [LearnableParameter(f"p{i}", 1, pars[i]) for i in range(N_PARAMS)]
-)
-
-
-class DummyOptimizer(GradientBasedOptimizer):
-    _hessian_sparsity = "dense"
-    _update_solver = None
-
-    def update(self, *args, **kwargs):
-        pass
-
-
-class TestGradientBasedOptimizer(unittest.TestCase):
-    def test_init_and_step(self):
-        lr = object()
-        perc = object()
-        opt = DummyOptimizer(learning_rate=lr, max_percentage_update=perc)
-        self.assertIsInstance(opt.lr_scheduler, S.Scheduler)
-        self.assertIs(opt.lr_scheduler.value, lr)
-        self.assertIsNone(opt.hook)
-        self.assertIs(opt.max_percentage_update, perc)
-        self.assertIsNone(opt.learnable_parameters)
-        self.assertIsNone(opt._update_solver)
-
-    def test_init__with_scheduler(self):
-        hook = object()
-        learning_rate = S.ExponentialScheduler(0.56, 0.99)
-        learning_rate.step = Mock()
-
-        opt = DummyOptimizer(learning_rate, hook=hook)
-        opt.step()
-
-        self.assertIsInstance(opt.lr_scheduler, S.Scheduler)
-        self.assertEqual(opt.lr_scheduler.value, 0.56)
-        self.assertIs(opt.hook, hook)
-        learning_rate.step.assert_called_once_with()
-
-    def test_set_learnable_parameters(self):
-        opt = DummyOptimizer(0.1)
-        opt.set_learnable_parameters(LEARNABLE_PARS)
-        self.assertIs(opt.learnable_parameters, LEARNABLE_PARS)
-        self.assertIsNone(opt._update_solver)
-
-    def test_set_learnable_parameters__with_solver(self):
-        opt = DummyOptimizer(0.1, max_percentage_update=0.5)
-        opt.set_learnable_parameters(LEARNABLE_PARS)
-        self.assertIs(opt.learnable_parameters, LEARNABLE_PARS)
-        self.assertIsInstance(opt._update_solver, cs.Function)
-
-    def test_init__creates_update_solver(self):
-        learnable_pars = LEARNABLE_PARS.copy(deep=True)
-        learnable_pars.lb = -np.arange(1, N_PARAMS + 1, dtype=float)
-        learnable_pars.ub = np.arange(1, N_PARAMS + 1, dtype=float)
-        opt = DummyOptimizer(0.1)
-        opt.set_learnable_parameters(learnable_pars)
-        self.assertIsNotNone(opt._update_solver)
-
-    def test_get_update_bounds__raises__with_no_learnable_parameters(self):
-        opt = DummyOptimizer(learning_rate=0.1)
-        msg = "'NoneType' object has no attribute 'lb'"
-        with self.assertRaises(AttributeError, msg=msg):
-            opt._get_update_bounds(np.random.rand(N_PARAMS))
-
-    def test_get_update_bounds(self):
-        learnable_pars = LEARNABLE_PARS.copy(deep=True)
-        lb = -np.arange(1, N_PARAMS + 1, dtype=float)
-        ub = theta = np.arange(1, N_PARAMS + 1, dtype=float)
-        learnable_pars.lb = lb
-        learnable_pars.ub = ub
-        opt = DummyOptimizer(learning_rate=0.1)
-        opt.set_learnable_parameters(learnable_pars)
-        lb_dtheta, ub_dtheta = opt._get_update_bounds(theta)
-        np.testing.assert_array_equal(lb_dtheta, lb - theta)
-        np.testing.assert_array_equal(ub_dtheta, 0)
-
-    def test_get_update_bounds__with_maximum_update_percentage(self):
-        learnable_pars = LEARNABLE_PARS.copy(deep=True)
-        lb = theta = -np.arange(1, N_PARAMS + 1, dtype=float)
-        ub = np.arange(1, N_PARAMS + 1, dtype=float)
-        learnable_pars.lb = lb
-        learnable_pars.ub = ub
-        opt = DummyOptimizer(learning_rate=0.1, max_percentage_update=0.5)
-        opt.set_learnable_parameters(learnable_pars)
-        lb_dtheta, ub_dtheta = opt._get_update_bounds(theta)
-        np.testing.assert_array_equal(lb_dtheta, 0)
-        np.testing.assert_array_equal(ub_dtheta, 0.5 * np.abs(theta))
-
-
-class TestGradientDescent(unittest.TestCase):
-    @parameterized.expand([(False,), (True,)])
-    def test_update__unconstrained(self, nesterov: bool):
-        opt = O.GradientDescent(
-            learning_rate=0.1,
-            weight_decay=SMALL,
-            momentum=SMALL,
-            dampening=SMALL,
-            nesterov=nesterov,
-        )
-        learnable_pars = LEARNABLE_PARS.copy(deep=True)
-        learnable_pars.value = theta = np.random.randn(N_PARAMS)
-        opt.set_learnable_parameters(learnable_pars)
-        g = np.random.randn(N_PARAMS)
-        status = opt.update(g)
-        self.assertIsNone(status)
-        np.testing.assert_array_almost_equal(learnable_pars.value, theta - 0.1 * g)
-
-    @parameterized.expand([(False,), (True,)])
-    def test_update__constrained__with_small_bounds(self, nesterov: bool):
-        opt = O.GradientDescent(
-            learning_rate=0.1,
-            weight_decay=SMALL,
-            momentum=SMALL,
-            dampening=SMALL,
-            nesterov=nesterov,
-        )
-        learnable_pars = LEARNABLE_PARS.copy(deep=True)
-        learnable_pars.value = theta = np.random.randn(N_PARAMS)
-        lb = learnable_pars.lb = theta - np.abs(theta) * 5e-2
-        ub = learnable_pars.ub = theta + np.abs(theta) * 5e-2
-        opt.set_learnable_parameters(learnable_pars)
-        g = np.random.randn(N_PARAMS) * 100
-        status = opt.update(g)
-        theta_new = learnable_pars.value
-        self.assertIsNone(status)
-        self.assertTrue(
-            np.where(theta_new >= lb, True, np.isclose(theta_new, lb)).all()
-        )
-        self.assertTrue(
-            np.where(theta_new <= ub, True, np.isclose(theta_new, ub)).all()
-        )
-
-    @parameterized.expand([(False,), (True,)])
-    def test_update__constrained__with_large_bounds(self, nesterov: bool):
-        opt = O.GradientDescent(
-            learning_rate=0.1,
-            weight_decay=SMALL,
-            momentum=SMALL,
-            dampening=SMALL,
-            nesterov=nesterov,
-        )
-        learnable_pars = LEARNABLE_PARS.copy(deep=True)
-        learnable_pars.value = theta = np.random.randn(N_PARAMS)
-        learnable_pars.lb = -np.abs(theta) * 100
-        learnable_pars.ub = np.abs(theta) * 100
-        opt.set_learnable_parameters(learnable_pars)
-        g = np.random.randn(N_PARAMS) / 100
-        status = opt.update(g)
-        self.assertIsNone(status)
-        np.testing.assert_array_equal(learnable_pars.value, theta - 0.1 * g)
-
-
-class TestNetwonMethod(unittest.TestCase):
-    @parameterized.expand(product((0.0, SMALL), (False, True)))
-    def test_update__unconstrained(self, w: float, cho_before_update: bool):
-        opt = O.NetwonMethod(0.1, weight_decay=w, cho_before_update=cho_before_update)
-        learnable_pars = LEARNABLE_PARS.copy(deep=True)
-        learnable_pars.value = theta = np.random.randn(N_PARAMS)
-        opt.set_learnable_parameters(learnable_pars)
-        g = np.random.randn(N_PARAMS)
-        H = np.random.randn(N_PARAMS, N_PARAMS)
-        H = H @ H.T + np.eye(N_PARAMS)
-        status = opt.update(g, H)
-        self.assertIsNone(status)
-        np.testing.assert_array_almost_equal(
-            learnable_pars.value, theta - 0.1 * np.linalg.solve(H, g)
-        )
-
-    @parameterized.expand(product((0.0, SMALL), (False, True)))
-    def test_update__unconstrained__with_identity_hessian(
-        self, w: float, cho_before_update: bool
-    ):
-        opt = O.NetwonMethod(0.1, weight_decay=w, cho_before_update=cho_before_update)
-        learnable_pars = LEARNABLE_PARS.copy(deep=True)
-        learnable_pars.value = theta = np.random.randn(N_PARAMS)
-        opt.set_learnable_parameters(learnable_pars)
-        g = np.random.randn(N_PARAMS)
-        H = np.eye(N_PARAMS)
-        status = opt.update(g, H)
-        self.assertIsNone(status)
-        np.testing.assert_array_almost_equal(learnable_pars.value, theta - 0.1 * g)
-
-    @parameterized.expand(product((0.0, SMALL), (False, True)))
-    def test_update__constrained__with_large_bounds_with_identity_hessian(
-        self, w: float, cho_before_update: bool
-    ):
-        opt = O.NetwonMethod(0.1, weight_decay=w, cho_before_update=cho_before_update)
-        learnable_pars = LEARNABLE_PARS.copy(deep=True)
-        learnable_pars.value = theta = np.random.randn(N_PARAMS)
-        learnable_pars.lb = -np.abs(theta) * 100
-        learnable_pars.ub = np.abs(theta) * 100
-        opt.set_learnable_parameters(learnable_pars)
-        g = np.random.randn(N_PARAMS) / 100
-        H = np.eye(N_PARAMS)
-        status = opt.update(g, H)
-        self.assertIsNone(status)
-        np.testing.assert_array_equal(learnable_pars.value, theta - 0.1 * g)
-
-    @parameterized.expand(product((0.0, SMALL), (False, True)))
-    def test_update__constrained__with_small_bounds(
-        self, w: float, cho_before_update: bool
-    ):
-        opt = O.NetwonMethod(0.1, weight_decay=w, cho_before_update=cho_before_update)
-        learnable_pars = LEARNABLE_PARS.copy(deep=True)
-        learnable_pars.value = theta = np.random.randn(N_PARAMS)
-        lb = learnable_pars.lb = theta - np.abs(theta) * 5e-2
-        ub = learnable_pars.ub = theta + np.abs(theta) * 5e-2
-        opt.set_learnable_parameters(learnable_pars)
-        g = np.random.randn(N_PARAMS) * 100
-        H = np.random.randn(N_PARAMS, N_PARAMS)
-        H = H @ H.T
-        status = opt.update(g, H)
-        theta_new = learnable_pars.value
-        self.assertIsNone(status)
-        self.assertTrue(
-            np.where(theta_new >= lb, True, np.isclose(theta_new, lb)).all()
-        )
-        self.assertTrue(
-            np.where(theta_new <= ub, True, np.isclose(theta_new, ub)).all()
-        )
-
-
-class TestAdam(unittest.TestCase):
-    @parameterized.expand(product((0, 0.01), (False, True), (False, True)))
-    def test(self, weight_decay: float, decouple_weight_decay: bool, amsgrad: bool):
-        # prepare data
-        betas = tuple(np.random.uniform(0.9, 1.0, size=2))
-        eps = np.random.uniform(1e-8, 1e-6)
-        lr = np.random.uniform(1e-4, 1e-3)
-
-        # prepare torch elements
-        x = torch.linspace(-np.pi, np.pi, 2, dtype=torch.float64)
-        xx_torch = x.unsqueeze(-1).pow(torch.tensor([1, 2, 3]))
-        y_actual_torch = torch.sin(x)
-        model_torch = torch.nn.Linear(3, 1, dtype=torch.float64)
-        loss_fn_torch = torch.nn.MSELoss(reduction="sum")
-        cls = torch.optim.AdamW if decouple_weight_decay else torch.optim.Adam
-        optimizer_torch = cls(
-            params=model_torch.parameters(),
-            lr=lr,
-            betas=betas,
-            eps=eps,
-            weight_decay=weight_decay,
-            amsgrad=amsgrad,
-        )
-
-        # prepare mpcrl elements
-        xx_dm = cs.DM(xx_torch.detach().numpy())
-        A_sym = cs.MX.sym("A", *model_torch.weight.shape)
-        b_sym = cs.MX.sym("b", *model_torch.bias.shape)
-        y_pred_sym = xx_dm @ A_sym.T + b_sym
-        y_actual_dm = cs.DM(y_actual_torch.detach().clone().numpy())
-        loss_sym = cs.sumsqr(y_pred_sym - y_actual_dm)
-        p_sym = cs.veccat(A_sym, b_sym)
-        dldp_sym = cs.gradient(loss_sym, p_sym)
-        model_mpcrl = cs.Function(
-            "F", [p_sym], [y_pred_sym, loss_sym, dldp_sym], ["p"], ["y", "l", "dldp"]
-        )
-        A_mpcrl = model_torch.weight.data.detach().clone().numpy().flatten()
-        b_mpcrl = model_torch.bias.data.detach().clone().numpy()
-        learnable_pars = LearnableParametersDict(
-            [
-                LearnableParameter("A", A_mpcrl.size, A_mpcrl),
-                LearnableParameter("b", b_mpcrl.size, b_mpcrl),
-            ]
-        )
-        optimizer_mpcrl = O.Adam(
-            learning_rate=lr,
-            max_percentage_update=1e4,  # test constrained
-            betas=betas,
-            eps=eps,
-            weight_decay=weight_decay,
-            decoupled_weight_decay=decouple_weight_decay,
-            amsgrad=amsgrad,
-        )
-        optimizer_mpcrl.set_learnable_parameters(learnable_pars)
-
-        # run test
-        cmp = lambda x, y, msg: np.testing.assert_allclose(
-            x, y, rtol=1e-6, atol=1e-6, err_msg=msg
-        )
-        for i in range(20):
-            # torch
-            y_pred_torch = model_torch(xx_torch).flatten()
-            loss_torch = loss_fn_torch(y_pred_torch, y_actual_torch)
-            optimizer_torch.zero_grad()
-            loss_torch.backward()
-            optimizer_torch.step()
-            grad_torch = np.concatenate(
-                [
-                    model_torch.weight.grad.detach().clone().numpy(),
-                    model_torch.bias.grad.detach().clone().numpy(),
-                ],
-                None,
-            )
-
-            # mpcrl
-            y_pred_mpcrl, loss_mpcrl, grad_mpcrl = model_mpcrl(
-                np.concatenate([A_mpcrl, b_mpcrl], None)
-            )
-            grad_mpcrl = grad_mpcrl.full().flatten()
-            status = optimizer_mpcrl.update(grad_mpcrl)
-            p_new = learnable_pars.value
-            A_mpcrl, b_mpcrl = np.array_split(p_new, [A_mpcrl.size])
-
-            # check
-            self.assertIsNone(status)
-            cmp(
-                y_pred_mpcrl.full().flatten(),
-                y_pred_torch.detach().clone().numpy(),
-                f"prediction mismatch at iteration {i}",
-            )
-            cmp(
-                float(loss_mpcrl),
-                loss_torch.detach().clone().item(),
-                f"loss mismatch at iteration {i}",
-            )
-            cmp(grad_mpcrl, grad_torch, f"gradient mismatch at iteration {i}")
-            cmp(
-                A_mpcrl,
-                model_torch.weight.detach().clone().numpy().reshape(A_mpcrl.shape),
-                f"`A` mismatch at iteration {i}",
-            )
-            cmp(
-                b_mpcrl,
-                model_torch.bias.detach().clone().numpy().reshape(b_mpcrl.shape),
-                f"`b` mismatch at iteration {i}",
-            )
-
-
-class TestRMSprop(unittest.TestCase):
-    @parameterized.expand(product((0, 0.1), (0, 0.9), (False, True)))
-    def test(self, weight_decay: float, momentum: float, centered: bool):
-        # prepare data
-        alpha = np.random.uniform(0.9, 0.99)
-        eps = np.random.uniform(1e-8, 1e-6)
-        lr = np.random.uniform(1e-4, 1e-3)
-
-        # prepare torch elements
-        x = torch.linspace(-np.pi, np.pi, 2, dtype=torch.float64)
-        xx_torch = x.unsqueeze(-1).pow(torch.tensor([1, 2, 3]))
-        y_actual_torch = torch.sin(x)
-        model_torch = torch.nn.Linear(3, 1, dtype=torch.float64)
-        loss_fn_torch = torch.nn.MSELoss(reduction="sum")
-        optimizer_torch = torch.optim.RMSprop(
-            params=model_torch.parameters(),
-            lr=lr,
-            alpha=alpha,
-            eps=eps,
-            weight_decay=weight_decay,
-            momentum=momentum,
-            centered=centered,
-        )
-
-        # prepare mpcrl elements
-        xx_dm = cs.DM(xx_torch.detach().numpy())
-        A_sym = cs.MX.sym("A", *model_torch.weight.shape)
-        b_sym = cs.MX.sym("b", *model_torch.bias.shape)
-        y_pred_sym = xx_dm @ A_sym.T + b_sym
-        y_actual_dm = cs.DM(y_actual_torch.detach().clone().numpy())
-        loss_sym = cs.sumsqr(y_pred_sym - y_actual_dm)
-        p_sym = cs.veccat(A_sym, b_sym)
-        dldp_sym = cs.gradient(loss_sym, p_sym)
-        model_mpcrl = cs.Function(
-            "F", [p_sym], [y_pred_sym, loss_sym, dldp_sym], ["p"], ["y", "l", "dldp"]
-        )
-        A_mpcrl = model_torch.weight.data.detach().clone().numpy().flatten()
-        b_mpcrl = model_torch.bias.data.detach().clone().numpy()
-        learnable_pars = LearnableParametersDict(
-            [
-                LearnableParameter("A", A_mpcrl.size, A_mpcrl),
-                LearnableParameter("b", b_mpcrl.size, b_mpcrl),
-            ]
-        )
-        optimizer_mpcrl = O.RMSprop(
-            learning_rate=lr,
-            alpha=alpha,
-            eps=eps,
-            weight_decay=weight_decay,
-            momentum=momentum,
-            centered=centered,
-            max_percentage_update=1e4,  # test constrained
-        )
-        optimizer_mpcrl.set_learnable_parameters(learnable_pars)
-
-        # run test
-        cmp = lambda x, y, msg: np.testing.assert_allclose(
-            x, y, rtol=1e-6, atol=1e-6, err_msg=msg
-        )
-        for i in range(20):
-            # torch
-            y_pred_torch = model_torch(xx_torch).flatten()
-            loss_torch = loss_fn_torch(y_pred_torch, y_actual_torch)
-            optimizer_torch.zero_grad()
-            loss_torch.backward()
-            optimizer_torch.step()
-            grad_torch = np.concatenate(
-                [
-                    model_torch.weight.grad.detach().clone().numpy(),
-                    model_torch.bias.grad.detach().clone().numpy(),
-                ],
-                None,
-            )
-
-            # mpcrl
-            y_pred_mpcrl, loss_mpcrl, grad_mpcrl = model_mpcrl(
-                np.concatenate([A_mpcrl, b_mpcrl], None)
-            )
-            grad_mpcrl = grad_mpcrl.full().flatten()
-            status = optimizer_mpcrl.update(grad_mpcrl)
-            p_new = learnable_pars.value
-            A_mpcrl, b_mpcrl = np.array_split(p_new, [A_mpcrl.size])
-
-            # check
-            self.assertIsNone(status)
-            cmp(
-                y_pred_mpcrl.full().flatten(),
-                y_pred_torch.detach().clone().numpy(),
-                f"prediction mismatch at iteration {i}",
-            )
-            cmp(
-                float(loss_mpcrl),
-                loss_torch.detach().clone().item(),
-                f"loss mismatch at iteration {i}",
-            )
-            cmp(grad_mpcrl, grad_torch, f"gradient mismatch at iteration {i}")
-            cmp(
-                A_mpcrl,
-                model_torch.weight.detach().clone().numpy().reshape(A_mpcrl.shape),
-                f"`A` mismatch at iteration {i}",
-            )
-            cmp(
-                b_mpcrl,
-                model_torch.bias.detach().clone().numpy().reshape(b_mpcrl.shape),
-                f"`b` mismatch at iteration {i}",
-            )
-
-
-if __name__ == "__main__":
-    unittest.main()
+import unittest
+from itertools import product
+from unittest.mock import Mock
+
+import casadi as cs
+import numpy as np
+import torch
+from parameterized import parameterized
+
+from mpcrl import LearnableParameter, LearnableParametersDict
+from mpcrl import optim as O
+from mpcrl import schedulers as S
+from mpcrl.optim.gradient_based_optimizer import GradientBasedOptimizer
+
+np.random.seed(10)
+torch.manual_seed(0)
+torch.use_deterministic_algorithms(True)
+
+SMALL = 1e-270
+N_PARAMS = 5
+pars = np.random.randn(N_PARAMS)
+LEARNABLE_PARS = LearnableParametersDict(
+    [LearnableParameter(f"p{i}", 1, pars[i]) for i in range(N_PARAMS)]
+)
+
+
+class DummyOptimizer(GradientBasedOptimizer):
+    _hessian_sparsity = "dense"
+    _update_solver = None
+
+    def update(self, *args, **kwargs):
+        pass
+
+
+class TestGradientBasedOptimizer(unittest.TestCase):
+    def test_init_and_step(self):
+        lr = object()
+        perc = object()
+        opt = DummyOptimizer(learning_rate=lr, max_percentage_update=perc)
+        self.assertIsInstance(opt.lr_scheduler, S.Scheduler)
+        self.assertIs(opt.lr_scheduler.value, lr)
+        self.assertIsNone(opt.hook)
+        self.assertIs(opt.max_percentage_update, perc)
+        self.assertIsNone(opt.learnable_parameters)
+        self.assertIsNone(opt._update_solver)
+
+    def test_init__with_scheduler(self):
+        hook = object()
+        learning_rate = S.ExponentialScheduler(0.56, 0.99)
+        learning_rate.step = Mock()
+
+        opt = DummyOptimizer(learning_rate, hook=hook)
+        opt.step()
+
+        self.assertIsInstance(opt.lr_scheduler, S.Scheduler)
+        self.assertEqual(opt.lr_scheduler.value, 0.56)
+        self.assertIs(opt.hook, hook)
+        learning_rate.step.assert_called_once_with()
+
+    def test_set_learnable_parameters(self):
+        opt = DummyOptimizer(0.1)
+        opt.set_learnable_parameters(LEARNABLE_PARS)
+        self.assertIs(opt.learnable_parameters, LEARNABLE_PARS)
+        self.assertIsNone(opt._update_solver)
+
+    def test_set_learnable_parameters__with_solver(self):
+        opt = DummyOptimizer(0.1, max_percentage_update=0.5)
+        opt.set_learnable_parameters(LEARNABLE_PARS)
+        self.assertIs(opt.learnable_parameters, LEARNABLE_PARS)
+        self.assertIsInstance(opt._update_solver, cs.Function)
+
+    def test_init__creates_update_solver(self):
+        learnable_pars = LEARNABLE_PARS.copy(deep=True)
+        learnable_pars.lb = -np.arange(1, N_PARAMS + 1, dtype=float)
+        learnable_pars.ub = np.arange(1, N_PARAMS + 1, dtype=float)
+        opt = DummyOptimizer(0.1)
+        opt.set_learnable_parameters(learnable_pars)
+        self.assertIsNotNone(opt._update_solver)
+
+    def test_get_update_bounds__raises__with_no_learnable_parameters(self):
+        opt = DummyOptimizer(learning_rate=0.1)
+        msg = "'NoneType' object has no attribute 'lb'"
+        with self.assertRaises(AttributeError, msg=msg):
+            opt._get_update_bounds(np.random.rand(N_PARAMS))
+
+    def test_get_update_bounds(self):
+        learnable_pars = LEARNABLE_PARS.copy(deep=True)
+        lb = -np.arange(1, N_PARAMS + 1, dtype=float)
+        ub = theta = np.arange(1, N_PARAMS + 1, dtype=float)
+        learnable_pars.lb = lb
+        learnable_pars.ub = ub
+        opt = DummyOptimizer(learning_rate=0.1)
+        opt.set_learnable_parameters(learnable_pars)
+        lb_dtheta, ub_dtheta = opt._get_update_bounds(theta)
+        np.testing.assert_array_equal(lb_dtheta, lb - theta)
+        np.testing.assert_array_equal(ub_dtheta, 0)
+
+    def test_get_update_bounds__with_maximum_update_percentage(self):
+        learnable_pars = LEARNABLE_PARS.copy(deep=True)
+        lb = theta = -np.arange(1, N_PARAMS + 1, dtype=float)
+        ub = np.arange(1, N_PARAMS + 1, dtype=float)
+        learnable_pars.lb = lb
+        learnable_pars.ub = ub
+        opt = DummyOptimizer(learning_rate=0.1, max_percentage_update=0.5)
+        opt.set_learnable_parameters(learnable_pars)
+        lb_dtheta, ub_dtheta = opt._get_update_bounds(theta)
+        np.testing.assert_array_equal(lb_dtheta, 0)
+        np.testing.assert_array_equal(ub_dtheta, 0.5 * np.abs(theta))
+
+
+class TestGradientDescent(unittest.TestCase):
+    @parameterized.expand([(False,), (True,)])
+    def test_update__unconstrained(self, nesterov: bool):
+        opt = O.GradientDescent(
+            learning_rate=0.1,
+            weight_decay=SMALL,
+            momentum=SMALL,
+            dampening=SMALL,
+            nesterov=nesterov,
+        )
+        learnable_pars = LEARNABLE_PARS.copy(deep=True)
+        learnable_pars.value = theta = np.random.randn(N_PARAMS)
+        opt.set_learnable_parameters(learnable_pars)
+        g = np.random.randn(N_PARAMS)
+        status = opt.update(g)
+        self.assertIsNone(status)
+        np.testing.assert_array_almost_equal(learnable_pars.value, theta - 0.1 * g)
+
+    @parameterized.expand([(False,), (True,)])
+    def test_update__constrained__with_small_bounds(self, nesterov: bool):
+        opt = O.GradientDescent(
+            learning_rate=0.1,
+            weight_decay=SMALL,
+            momentum=SMALL,
+            dampening=SMALL,
+            nesterov=nesterov,
+        )
+        learnable_pars = LEARNABLE_PARS.copy(deep=True)
+        learnable_pars.value = theta = np.random.randn(N_PARAMS)
+        lb = learnable_pars.lb = theta - np.abs(theta) * 5e-2
+        ub = learnable_pars.ub = theta + np.abs(theta) * 5e-2
+        opt.set_learnable_parameters(learnable_pars)
+        g = np.random.randn(N_PARAMS) * 100
+        status = opt.update(g)
+        theta_new = learnable_pars.value
+        self.assertIsNone(status)
+        self.assertTrue(
+            np.where(theta_new >= lb, True, np.isclose(theta_new, lb)).all()
+        )
+        self.assertTrue(
+            np.where(theta_new <= ub, True, np.isclose(theta_new, ub)).all()
+        )
+
+    @parameterized.expand([(False,), (True,)])
+    def test_update__constrained__with_large_bounds(self, nesterov: bool):
+        opt = O.GradientDescent(
+            learning_rate=0.1,
+            weight_decay=SMALL,
+            momentum=SMALL,
+            dampening=SMALL,
+            nesterov=nesterov,
+        )
+        learnable_pars = LEARNABLE_PARS.copy(deep=True)
+        learnable_pars.value = theta = np.random.randn(N_PARAMS)
+        learnable_pars.lb = -np.abs(theta) * 100
+        learnable_pars.ub = np.abs(theta) * 100
+        opt.set_learnable_parameters(learnable_pars)
+        g = np.random.randn(N_PARAMS) / 100
+        status = opt.update(g)
+        self.assertIsNone(status)
+        np.testing.assert_array_equal(learnable_pars.value, theta - 0.1 * g)
+
+
+class TestNetwonMethod(unittest.TestCase):
+    @parameterized.expand(product((0.0, SMALL), (False, True)))
+    def test_update__unconstrained(self, w: float, cho_before_update: bool):
+        opt = O.NetwonMethod(0.1, weight_decay=w, cho_before_update=cho_before_update)
+        learnable_pars = LEARNABLE_PARS.copy(deep=True)
+        learnable_pars.value = theta = np.random.randn(N_PARAMS)
+        opt.set_learnable_parameters(learnable_pars)
+        g = np.random.randn(N_PARAMS)
+        H = np.random.randn(N_PARAMS, N_PARAMS)
+        H = H @ H.T + np.eye(N_PARAMS)
+        status = opt.update(g, H)
+        self.assertIsNone(status)
+        np.testing.assert_array_almost_equal(
+            learnable_pars.value, theta - 0.1 * np.linalg.solve(H, g)
+        )
+
+    @parameterized.expand(product((0.0, SMALL), (False, True)))
+    def test_update__unconstrained__with_identity_hessian(
+        self, w: float, cho_before_update: bool
+    ):
+        opt = O.NetwonMethod(0.1, weight_decay=w, cho_before_update=cho_before_update)
+        learnable_pars = LEARNABLE_PARS.copy(deep=True)
+        learnable_pars.value = theta = np.random.randn(N_PARAMS)
+        opt.set_learnable_parameters(learnable_pars)
+        g = np.random.randn(N_PARAMS)
+        H = np.eye(N_PARAMS)
+        status = opt.update(g, H)
+        self.assertIsNone(status)
+        np.testing.assert_array_almost_equal(learnable_pars.value, theta - 0.1 * g)
+
+    @parameterized.expand(product((0.0, SMALL), (False, True)))
+    def test_update__constrained__with_large_bounds_with_identity_hessian(
+        self, w: float, cho_before_update: bool
+    ):
+        opt = O.NetwonMethod(0.1, weight_decay=w, cho_before_update=cho_before_update)
+        learnable_pars = LEARNABLE_PARS.copy(deep=True)
+        learnable_pars.value = theta = np.random.randn(N_PARAMS)
+        learnable_pars.lb = -np.abs(theta) * 100
+        learnable_pars.ub = np.abs(theta) * 100
+        opt.set_learnable_parameters(learnable_pars)
+        g = np.random.randn(N_PARAMS) / 100
+        H = np.eye(N_PARAMS)
+        status = opt.update(g, H)
+        self.assertIsNone(status)
+        np.testing.assert_array_equal(learnable_pars.value, theta - 0.1 * g)
+
+    @parameterized.expand(product((0.0, SMALL), (False, True)))
+    def test_update__constrained__with_small_bounds(
+        self, w: float, cho_before_update: bool
+    ):
+        opt = O.NetwonMethod(0.1, weight_decay=w, cho_before_update=cho_before_update)
+        learnable_pars = LEARNABLE_PARS.copy(deep=True)
+        learnable_pars.value = theta = np.random.randn(N_PARAMS)
+        lb = learnable_pars.lb = theta - np.abs(theta) * 5e-2
+        ub = learnable_pars.ub = theta + np.abs(theta) * 5e-2
+        opt.set_learnable_parameters(learnable_pars)
+        g = np.random.randn(N_PARAMS) * 100
+        H = np.random.randn(N_PARAMS, N_PARAMS)
+        H = H @ H.T
+        status = opt.update(g, H)
+        theta_new = learnable_pars.value
+        self.assertIsNone(status)
+        self.assertTrue(
+            np.where(theta_new >= lb, True, np.isclose(theta_new, lb)).all()
+        )
+        self.assertTrue(
+            np.where(theta_new <= ub, True, np.isclose(theta_new, ub)).all()
+        )
+
+
+class TestAdam(unittest.TestCase):
+    @parameterized.expand(product((0, 0.01), (False, True), (False, True)))
+    def test(self, weight_decay: float, decouple_weight_decay: bool, amsgrad: bool):
+        # prepare data
+        betas = tuple(np.random.uniform(0.9, 1.0, size=2))
+        eps = np.random.uniform(1e-8, 1e-6)
+        lr = np.random.uniform(1e-4, 1e-3)
+
+        # prepare torch elements
+        x = torch.linspace(-np.pi, np.pi, 2, dtype=torch.float64)
+        xx_torch = x.unsqueeze(-1).pow(torch.tensor([1, 2, 3]))
+        y_actual_torch = torch.sin(x)
+        model_torch = torch.nn.Linear(3, 1, dtype=torch.float64)
+        loss_fn_torch = torch.nn.MSELoss(reduction="sum")
+        cls = torch.optim.AdamW if decouple_weight_decay else torch.optim.Adam
+        optimizer_torch = cls(
+            params=model_torch.parameters(),
+            lr=lr,
+            betas=betas,
+            eps=eps,
+            weight_decay=weight_decay,
+            amsgrad=amsgrad,
+        )
+
+        # prepare mpcrl elements
+        xx_dm = cs.DM(xx_torch.detach().numpy())
+        A_sym = cs.MX.sym("A", *model_torch.weight.shape)
+        b_sym = cs.MX.sym("b", *model_torch.bias.shape)
+        y_pred_sym = xx_dm @ A_sym.T + b_sym
+        y_actual_dm = cs.DM(y_actual_torch.detach().clone().numpy())
+        loss_sym = cs.sumsqr(y_pred_sym - y_actual_dm)
+        p_sym = cs.veccat(A_sym, b_sym)
+        dldp_sym = cs.gradient(loss_sym, p_sym)
+        model_mpcrl = cs.Function(
+            "F", [p_sym], [y_pred_sym, loss_sym, dldp_sym], ["p"], ["y", "l", "dldp"]
+        )
+        A_mpcrl = model_torch.weight.data.detach().clone().numpy().flatten()
+        b_mpcrl = model_torch.bias.data.detach().clone().numpy()
+        learnable_pars = LearnableParametersDict(
+            [
+                LearnableParameter("A", A_mpcrl.size, A_mpcrl),
+                LearnableParameter("b", b_mpcrl.size, b_mpcrl),
+            ]
+        )
+        optimizer_mpcrl = O.Adam(
+            learning_rate=lr,
+            max_percentage_update=1e4,  # test constrained
+            betas=betas,
+            eps=eps,
+            weight_decay=weight_decay,
+            decoupled_weight_decay=decouple_weight_decay,
+            amsgrad=amsgrad,
+        )
+        optimizer_mpcrl.set_learnable_parameters(learnable_pars)
+
+        # run test
+        cmp = lambda x, y, msg: np.testing.assert_allclose(
+            x, y, rtol=1e-6, atol=1e-6, err_msg=msg
+        )
+        for i in range(20):
+            # torch
+            y_pred_torch = model_torch(xx_torch).flatten()
+            loss_torch = loss_fn_torch(y_pred_torch, y_actual_torch)
+            optimizer_torch.zero_grad()
+            loss_torch.backward()
+            optimizer_torch.step()
+            grad_torch = np.concatenate(
+                [
+                    model_torch.weight.grad.detach().clone().numpy(),
+                    model_torch.bias.grad.detach().clone().numpy(),
+                ],
+                None,
+            )
+
+            # mpcrl
+            y_pred_mpcrl, loss_mpcrl, grad_mpcrl = model_mpcrl(
+                np.concatenate([A_mpcrl, b_mpcrl], None)
+            )
+            grad_mpcrl = grad_mpcrl.full().flatten()
+            status = optimizer_mpcrl.update(grad_mpcrl)
+            p_new = learnable_pars.value
+            A_mpcrl, b_mpcrl = np.array_split(p_new, [A_mpcrl.size])
+
+            # check
+            self.assertIsNone(status)
+            cmp(
+                y_pred_mpcrl.full().flatten(),
+                y_pred_torch.detach().clone().numpy(),
+                f"prediction mismatch at iteration {i}",
+            )
+            cmp(
+                float(loss_mpcrl),
+                loss_torch.detach().clone().item(),
+                f"loss mismatch at iteration {i}",
+            )
+            cmp(grad_mpcrl, grad_torch, f"gradient mismatch at iteration {i}")
+            cmp(
+                A_mpcrl,
+                model_torch.weight.detach().clone().numpy().reshape(A_mpcrl.shape),
+                f"`A` mismatch at iteration {i}",
+            )
+            cmp(
+                b_mpcrl,
+                model_torch.bias.detach().clone().numpy().reshape(b_mpcrl.shape),
+                f"`b` mismatch at iteration {i}",
+            )
+
+
+class TestRMSprop(unittest.TestCase):
+    @parameterized.expand(product((0, 0.1), (0, 0.9), (False, True)))
+    def test(self, weight_decay: float, momentum: float, centered: bool):
+        # prepare data
+        alpha = np.random.uniform(0.9, 0.99)
+        eps = np.random.uniform(1e-8, 1e-6)
+        lr = np.random.uniform(1e-4, 1e-3)
+
+        # prepare torch elements
+        x = torch.linspace(-np.pi, np.pi, 2, dtype=torch.float64)
+        xx_torch = x.unsqueeze(-1).pow(torch.tensor([1, 2, 3]))
+        y_actual_torch = torch.sin(x)
+        model_torch = torch.nn.Linear(3, 1, dtype=torch.float64)
+        loss_fn_torch = torch.nn.MSELoss(reduction="sum")
+        optimizer_torch = torch.optim.RMSprop(
+            params=model_torch.parameters(),
+            lr=lr,
+            alpha=alpha,
+            eps=eps,
+            weight_decay=weight_decay,
+            momentum=momentum,
+            centered=centered,
+        )
+
+        # prepare mpcrl elements
+        xx_dm = cs.DM(xx_torch.detach().numpy())
+        A_sym = cs.MX.sym("A", *model_torch.weight.shape)
+        b_sym = cs.MX.sym("b", *model_torch.bias.shape)
+        y_pred_sym = xx_dm @ A_sym.T + b_sym
+        y_actual_dm = cs.DM(y_actual_torch.detach().clone().numpy())
+        loss_sym = cs.sumsqr(y_pred_sym - y_actual_dm)
+        p_sym = cs.veccat(A_sym, b_sym)
+        dldp_sym = cs.gradient(loss_sym, p_sym)
+        model_mpcrl = cs.Function(
+            "F", [p_sym], [y_pred_sym, loss_sym, dldp_sym], ["p"], ["y", "l", "dldp"]
+        )
+        A_mpcrl = model_torch.weight.data.detach().clone().numpy().flatten()
+        b_mpcrl = model_torch.bias.data.detach().clone().numpy()
+        learnable_pars = LearnableParametersDict(
+            [
+                LearnableParameter("A", A_mpcrl.size, A_mpcrl),
+                LearnableParameter("b", b_mpcrl.size, b_mpcrl),
+            ]
+        )
+        optimizer_mpcrl = O.RMSprop(
+            learning_rate=lr,
+            alpha=alpha,
+            eps=eps,
+            weight_decay=weight_decay,
+            momentum=momentum,
+            centered=centered,
+            max_percentage_update=1e4,  # test constrained
+        )
+        optimizer_mpcrl.set_learnable_parameters(learnable_pars)
+
+        # run test
+        cmp = lambda x, y, msg: np.testing.assert_allclose(
+            x, y, rtol=1e-6, atol=1e-6, err_msg=msg
+        )
+        for i in range(20):
+            # torch
+            y_pred_torch = model_torch(xx_torch).flatten()
+            loss_torch = loss_fn_torch(y_pred_torch, y_actual_torch)
+            optimizer_torch.zero_grad()
+            loss_torch.backward()
+            optimizer_torch.step()
+            grad_torch = np.concatenate(
+                [
+                    model_torch.weight.grad.detach().clone().numpy(),
+                    model_torch.bias.grad.detach().clone().numpy(),
+                ],
+                None,
+            )
+
+            # mpcrl
+            y_pred_mpcrl, loss_mpcrl, grad_mpcrl = model_mpcrl(
+                np.concatenate([A_mpcrl, b_mpcrl], None)
+            )
+            grad_mpcrl = grad_mpcrl.full().flatten()
+            status = optimizer_mpcrl.update(grad_mpcrl)
+            p_new = learnable_pars.value
+            A_mpcrl, b_mpcrl = np.array_split(p_new, [A_mpcrl.size])
+
+            # check
+            self.assertIsNone(status)
+            cmp(
+                y_pred_mpcrl.full().flatten(),
+                y_pred_torch.detach().clone().numpy(),
+                f"prediction mismatch at iteration {i}",
+            )
+            cmp(
+                float(loss_mpcrl),
+                loss_torch.detach().clone().item(),
+                f"loss mismatch at iteration {i}",
+            )
+            cmp(grad_mpcrl, grad_torch, f"gradient mismatch at iteration {i}")
+            cmp(
+                A_mpcrl,
+                model_torch.weight.detach().clone().numpy().reshape(A_mpcrl.shape),
+                f"`A` mismatch at iteration {i}",
+            )
+            cmp(
+                b_mpcrl,
+                model_torch.bias.detach().clone().numpy().reshape(b_mpcrl.shape),
+                f"`b` mismatch at iteration {i}",
+            )
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `mpcrl-1.2.0rc3/tests/test_util.py` & `mpcrl-1.2.0rc4/tests/test_util.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-import unittest
-
-import casadi as cs
-import numpy as np
-from parameterized import parameterized, parameterized_class
-
-from mpcrl.util import control, iters, math, named, seeding
-
-
-class DummyAgent(named.Named):
-    ...
-
-
-class TestNamedAgent(unittest.TestCase):
-    def test_init__with_given_name__saves_name_correctly(self):
-        dummy = DummyAgent(name="ciao")
-        self.assertEqual(dummy.name, "ciao")
-
-    def test_init__without_name__creates_name_with_class(self):
-        dummy0 = DummyAgent()
-        dummy1 = DummyAgent()
-        self.assertEqual(dummy0.name, "DummyAgent0")
-        self.assertEqual(dummy1.name, "DummyAgent1")
-
-    def test_str_and_repr(self):
-        name = "ciao"
-        dummy = DummyAgent(name=name)
-        S = dummy.__str__()
-        self.assertIn(name, S)
-        S = dummy.__repr__()
-        self.assertIn(name, S)
-        self.assertIn(DummyAgent.__name__, S)
-
-
-class TestMath(unittest.TestCase):
-    def test_cholesky_added_multiple_identities__performs_correct_factorization(self):
-        n = 5
-        A = np.random.rand(n, n) + np.eye(n) * 5
-        A = 0.5 * (A + A.T)
-        L = math.cholesky_added_multiple_identities(A)
-        np.testing.assert_allclose(A, L @ L.T)
-
-    def test_cholesky_added_multiple_identities__raises__max_iterations_reached(self):
-        n = 5
-        A = np.random.rand(n, n) - np.eye(n) * 5
-        A = 0.5 * (A + A.T)
-        with self.assertRaisesRegex(ValueError, "Maximum iterations reached."):
-            math.cholesky_added_multiple_identities(A, maxiter=1)
-
-    @parameterized.expand(
-        [
-            ((1, 1), 1),
-            ((5, 4), 5),
-            (
-                (np.arange(2, 11, 2), 4),
-                np.asarray(
-                    [
-                        [2, 4, 6, 8],
-                        [2, 4, 6, 10],
-                        [2, 4, 8, 10],
-                        [2, 6, 8, 10],
-                        [4, 6, 8, 10],
-                    ]
-                ),
-            ),
-            ((np.asarray([10, 20, 30]), 2), np.asarray([[10, 20], [10, 30], [20, 30]])),
-        ]
-    )
-    def test_nchoosek__computes_correct_combinations(
-        self, inp: tuple[int, int], out: int
-    ):
-        out_ = math.nchoosek(*inp)
-        np.testing.assert_allclose(out_, out)
-
-    @parameterized.expand([(1, 4, 4), (10, 1, np.eye(10)), (4, 3, None)])
-    def test_monomial_powers__computes_correct_powers(self, n, k, out):
-        p = math.monomial_powers(n, k)
-        self.assertEqual(p.shape[1], n)
-        np.testing.assert_allclose(p.sum(axis=1), k)
-        if out is not None:
-            np.testing.assert_allclose(p, out)
-
-
-class TestControl(unittest.TestCase):
-    def test_dlqr__returns_correctly(self):
-        K_exp = np.array([[1.075936290787970, 1.824593914133278]])
-        P_exp = np.array(
-            [
-                [6.783278637425703, 2.903698804441288],
-                [2.903698804441288, 5.026668672843932],
-            ]
-        )
-        A = np.array([[1, 0.25], [0, 1]])
-        B = np.array([[0.03], [0.25]])
-        Q = np.eye(2)
-        R = 0.5
-        K, P = control.dlqr(A, B, Q, R)
-        np.testing.assert_allclose(K, K_exp)
-        np.testing.assert_allclose(P, P_exp)
-
-    def test_dlqr__with_M__returns_correctly(self):
-        K_exp = np.array([[1.132928272226698, 1.820247185260309]])
-        P_exp = np.array(
-            [
-                [6.426698776552665, 2.359469798498852],
-                [2.359469798498852, 3.806839220681791],
-            ]
-        )
-        A = np.array([[1, 0.25], [0, 1]])
-        B = np.array([[0.03], [0.25]])
-        Q = np.eye(2)
-        R = np.atleast_2d(0.5)
-        M = np.array([[0.1], [0.2]])
-        K, P = control.dlqr(A, B, Q, R, M)
-        np.testing.assert_allclose(K, K_exp)
-        np.testing.assert_allclose(P, P_exp)
-
-    def test_rk4__returns_correcly(self):
-        def f(x):
-            return -3 * x
-
-        dt = 0.01
-        x = cs.SX.sym("x")
-        fd = cs.Function("fd", [x], [control.rk4(f, x, dt)])
-
-        Y = [1]
-        for _ in range(100):
-            Y.append(fd(Y[-1]))
-        Y = cs.hcat(Y).full().squeeze()
-        Y_exact = np.exp(-3 * (np.arange(Y.size) * dt))
-        np.testing.assert_allclose(Y, Y_exact)
-
-
-@parameterized_class("starts_with", [(False,), (True,)])
-class TestIters(unittest.TestCase):
-    @parameterized.expand([(5,), (1,), (22,)])
-    def test_bool_cycle(self, frequency: int):
-        T = frequency * 10
-        cycle = iters.bool_cycle(frequency, self.starts_with)
-        cycle = [next(cycle) for _ in range(T)]
-        self.assertEqual(cycle[0], self.starts_with or frequency == 1)
-        self.assertEqual(T // frequency, sum(cycle))
-
-
-class TestSeeding(unittest.TestCase):
-    def test_mk_seed(self):
-        rng = np.random.default_rng()
-        self.assertTrue(0 <= seeding.mk_seed(rng) < 2**32)
-
-
-if __name__ == "__main__":
-    unittest.main()
+import unittest
+
+import casadi as cs
+import numpy as np
+from parameterized import parameterized, parameterized_class
+
+from mpcrl.util import control, iters, math, named, seeding
+
+
+class DummyAgent(named.Named):
+    ...
+
+
+class TestNamedAgent(unittest.TestCase):
+    def test_init__with_given_name__saves_name_correctly(self):
+        dummy = DummyAgent(name="ciao")
+        self.assertEqual(dummy.name, "ciao")
+
+    def test_init__without_name__creates_name_with_class(self):
+        dummy0 = DummyAgent()
+        dummy1 = DummyAgent()
+        self.assertEqual(dummy0.name, "DummyAgent0")
+        self.assertEqual(dummy1.name, "DummyAgent1")
+
+    def test_str_and_repr(self):
+        name = "ciao"
+        dummy = DummyAgent(name=name)
+        S = dummy.__str__()
+        self.assertIn(name, S)
+        S = dummy.__repr__()
+        self.assertIn(name, S)
+        self.assertIn(DummyAgent.__name__, S)
+
+
+class TestMath(unittest.TestCase):
+    def test_cholesky_added_multiple_identities__performs_correct_factorization(self):
+        n = 5
+        A = np.random.rand(n, n) + np.eye(n) * 5
+        A = 0.5 * (A + A.T)
+        L = math.cholesky_added_multiple_identities(A)
+        np.testing.assert_allclose(A, L @ L.T)
+
+    def test_cholesky_added_multiple_identities__raises__max_iterations_reached(self):
+        n = 5
+        A = np.random.rand(n, n) - np.eye(n) * 5
+        A = 0.5 * (A + A.T)
+        with self.assertRaisesRegex(ValueError, "Maximum iterations reached."):
+            math.cholesky_added_multiple_identities(A, maxiter=1)
+
+    @parameterized.expand(
+        [
+            ((1, 1), 1),
+            ((5, 4), 5),
+            (
+                (np.arange(2, 11, 2), 4),
+                np.asarray(
+                    [
+                        [2, 4, 6, 8],
+                        [2, 4, 6, 10],
+                        [2, 4, 8, 10],
+                        [2, 6, 8, 10],
+                        [4, 6, 8, 10],
+                    ]
+                ),
+            ),
+            ((np.asarray([10, 20, 30]), 2), np.asarray([[10, 20], [10, 30], [20, 30]])),
+        ]
+    )
+    def test_nchoosek__computes_correct_combinations(
+        self, inp: tuple[int, int], out: int
+    ):
+        out_ = math.nchoosek(*inp)
+        np.testing.assert_allclose(out_, out)
+
+    @parameterized.expand([(1, 4, 4), (10, 1, np.eye(10)), (4, 3, None)])
+    def test_monomial_powers__computes_correct_powers(self, n, k, out):
+        p = math.monomial_powers(n, k)
+        self.assertEqual(p.shape[1], n)
+        np.testing.assert_allclose(p.sum(axis=1), k)
+        if out is not None:
+            np.testing.assert_allclose(p, out)
+
+
+class TestControl(unittest.TestCase):
+    def test_dlqr__returns_correctly(self):
+        K_exp = np.array([[1.075936290787970, 1.824593914133278]])
+        P_exp = np.array(
+            [
+                [6.783278637425703, 2.903698804441288],
+                [2.903698804441288, 5.026668672843932],
+            ]
+        )
+        A = np.array([[1, 0.25], [0, 1]])
+        B = np.array([[0.03], [0.25]])
+        Q = np.eye(2)
+        R = 0.5
+        K, P = control.dlqr(A, B, Q, R)
+        np.testing.assert_allclose(K, K_exp)
+        np.testing.assert_allclose(P, P_exp)
+
+    def test_dlqr__with_M__returns_correctly(self):
+        K_exp = np.array([[1.132928272226698, 1.820247185260309]])
+        P_exp = np.array(
+            [
+                [6.426698776552665, 2.359469798498852],
+                [2.359469798498852, 3.806839220681791],
+            ]
+        )
+        A = np.array([[1, 0.25], [0, 1]])
+        B = np.array([[0.03], [0.25]])
+        Q = np.eye(2)
+        R = np.atleast_2d(0.5)
+        M = np.array([[0.1], [0.2]])
+        K, P = control.dlqr(A, B, Q, R, M)
+        np.testing.assert_allclose(K, K_exp)
+        np.testing.assert_allclose(P, P_exp)
+
+    def test_rk4__returns_correcly(self):
+        def f(x):
+            return -3 * x
+
+        dt = 0.01
+        x = cs.SX.sym("x")
+        fd = cs.Function("fd", [x], [control.rk4(f, x, dt)])
+
+        Y = [1]
+        for _ in range(100):
+            Y.append(fd(Y[-1]))
+        Y = cs.hcat(Y).full().squeeze()
+        Y_exact = np.exp(-3 * (np.arange(Y.size) * dt))
+        np.testing.assert_allclose(Y, Y_exact)
+
+
+@parameterized_class("starts_with", [(False,), (True,)])
+class TestIters(unittest.TestCase):
+    @parameterized.expand([(5,), (1,), (22,)])
+    def test_bool_cycle(self, frequency: int):
+        T = frequency * 10
+        cycle = iters.bool_cycle(frequency, self.starts_with)
+        cycle = [next(cycle) for _ in range(T)]
+        self.assertEqual(cycle[0], self.starts_with or frequency == 1)
+        self.assertEqual(T // frequency, sum(cycle))
+
+
+class TestSeeding(unittest.TestCase):
+    def test_mk_seed(self):
+        rng = np.random.default_rng()
+        self.assertTrue(0 <= seeding.mk_seed(rng) < 2**32)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `mpcrl-1.2.0rc3/tests/test_wrappers.py` & `mpcrl-1.2.0rc4/tests/test_wrappers.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,406 +1,406 @@
-import logging
-import os
-import unittest
-from functools import lru_cache
-from typing import Any
-from unittest.mock import Mock, call
-
-import casadi as cs
-import gymnasium as gym
-import numpy as np
-from csnlp import Nlp, scaling
-from csnlp.multistart import StackedMultistartNlp
-from csnlp.wrappers import Mpc, NlpScaling
-
-from mpcrl import (
-    Agent,
-    LearnableParameter,
-    LearnableParametersDict,
-    LearningAgent,
-    wrappers_agents,
-    wrappers_envs,
-)
-from mpcrl.wrappers.envs.monitor_infos import compact_dicts
-
-
-@lru_cache
-def get_dynamics(g: float, alpha: float, dt: float) -> cs.Function:
-    x, u, d = cs.SX.sym("x", 3), cs.SX.sym("u", 2), cs.SX.sym("d", 3)
-    x_next = x + cs.vertcat(x[1], u[0] / x[2] - g, -alpha * u[0]) * dt + d * 0
-    return cs.Function("F", [x, u, d], [x_next], ["x", "u", "d"], ["x+"])
-
-
-def get_mpc(horizon: int, multistart: bool):
-    N = horizon
-    T = 100
-    K = 3
-    dt = T / N
-    yT = 100000
-    g = 9.81
-    alpha = 1 / (300 * g)
-    y_nom = 1e5
-    v_nom = 2e3
-    m_nom = 3e5
-    u_nom = 1e8
-    scaler = scaling.Scaler()
-    scaler.register("y", scale=y_nom)
-    scaler.register("y_0", scale=y_nom)
-    scaler.register("v", scale=v_nom)
-    scaler.register("v_0", scale=v_nom)
-    scaler.register("m", scale=m_nom)
-    scaler.register("m_0", scale=m_nom)
-    scaler.register("u1", scale=u_nom)
-    scaler.register("u2", scale=u_nom)
-    nlp = (
-        StackedMultistartNlp[cs.MX](sym_type="MX", starts=K)
-        if multistart
-        else Nlp[cs.MX](sym_type="MX")
-    )
-    nlp = NlpScaling[cs.MX](nlp, scaler=scaler)
-    mpc = Mpc[cs.MX](nlp, prediction_horizon=N)
-    y, _ = mpc.state("y")
-    _, _ = mpc.state("v")
-    m, _ = mpc.state("m", lb=0)
-    mpc.action("u1", lb=0, ub=5e7)
-    u2, _ = mpc.action("u2", lb=0, ub=5e7)
-    mpc.disturbance("d", 3)
-    mpc.set_dynamics(get_dynamics(g, alpha, dt))
-    mpc.constraint("yT", y[-1], "==", yT)
-    mpc.minimize(m[0] - m[-1] + cs.sum2(u2))
-    mpc.init_solver()
-    return mpc
-
-
-class DummyAgent(Agent):
-    ...
-
-
-class DummyLearningAgent(LearningAgent):
-    def update(self, *args, **kwargs):
-        return
-
-    def train_one_episode(self, *args, **kwargs):
-        return
-
-
-def mk_agent() -> DummyLearningAgent:
-    return DummyLearningAgent(
-        mpc=get_mpc(3, False),
-        learnable_parameters=LearnableParametersDict(),
-        update_strategy=1,
-    )
-
-
-class SimpleEnv(gym.Env[object, object]):
-    T_MAX = 10
-
-    def __init__(self, *args: Any, **kwargs: Any):
-        super().__init__(*args, **kwargs)
-        self.INTERNAL_RESET_INFOS = []
-        self.INTERNAL_FINALIZED_RESET_INFOS = {"reset_info": []}
-        self.INTERNAL_STEP_INFOS = []
-        self.INTERNAL_FINALIZED_STEP_INFOS = {"step_info": []}
-        self.INTERNAL_OBSERVATIONS = []
-        self.INTERNAL_ACTIONS = []
-        self.INTERNAL_REWARDS = []
-
-    def reset(self, *args: Any, **kwargs: Any) -> tuple[object, dict[str, Any]]:
-        super().reset(*args, **kwargs)
-        self.t = 0
-        obs = object()
-        info = {"reset_info": object()}
-        self.INTERNAL_RESET_INFOS.append(info)
-        self.INTERNAL_FINALIZED_RESET_INFOS["reset_info"].append(info["reset_info"])
-        self.INTERNAL_STEP_INFOS.append([])
-        self.INTERNAL_FINALIZED_STEP_INFOS["step_info"].append([])
-        self.INTERNAL_OBSERVATIONS.append([obs])
-        self.INTERNAL_ACTIONS.append([])
-        self.INTERNAL_REWARDS.append([])
-        return obs, info
-
-    def step(self, action: object) -> tuple[object, float, bool, bool, dict[str, Any]]:
-        self.t += 1
-        obs = object()
-        reward = np.random.rand()
-        terminated = self.t >= self.T_MAX
-        info = {"step_info": object()}
-        self.INTERNAL_STEP_INFOS[-1].append(info)
-        self.INTERNAL_FINALIZED_STEP_INFOS["step_info"][-1].append(info["step_info"])
-        self.INTERNAL_OBSERVATIONS[-1].append(obs)
-        self.INTERNAL_ACTIONS[-1].append(action)
-        self.INTERNAL_REWARDS[-1].append(reward)
-        return obs, reward, terminated, False, info
-
-
-class TestWrapperAndLearningWrapper(unittest.TestCase):
-    def test_attr__raises__when_accessing_private_attrs(self):
-        wrapped = wrappers_agents.LearningWrapper(mk_agent())
-        with self.assertRaisesRegex(
-            AttributeError, "Accessing private attribute '_x' is prohibited."
-        ):
-            wrapped._x
-
-    def test_unwrapped__unwraps_nlp_correctly(self):
-        agent = mk_agent()
-        wrapped = wrappers_agents.LearningWrapper(agent)
-        self.assertIs(agent, wrapped.unwrapped)
-
-    def test_str_and_repr(self):
-        agent = mk_agent()
-        wrapped = wrappers_agents.LearningWrapper(agent)
-        S = wrapped.__str__()
-        self.assertIn(wrappers_agents.LearningWrapper.__name__, S)
-        self.assertIn(agent.__str__(), S)
-        S = wrapped.__repr__()
-        self.assertIn(wrappers_agents.LearningWrapper.__name__, S)
-        self.assertIn(agent.__repr__(), S)
-
-    def test_is_wrapped(self):
-        agent = mk_agent()
-        self.assertFalse(agent.is_wrapped())
-
-        wrapped = wrappers_agents.LearningWrapper(agent)
-        self.assertTrue(wrapped.is_wrapped(wrappers_agents.LearningWrapper))
-        self.assertFalse(wrapped.is_wrapped(cs.SX))
-
-    def test_detach_wrapper(self):
-        agent = mk_agent()
-        wrapped_intermediate = wrappers_agents.RecordUpdates(agent)
-        original_hooks = agent._hooks.copy()
-        wrapped = wrappers_agents.Log(
-            wrapped_intermediate,
-            level=logging.DEBUG,
-            log_frequencies={"on_timestep_end": 1000},
-        )
-        with self.assertRaises(AssertionError):
-            self.assertDictEqual(agent._hooks, original_hooks)
-        wrapped.detach_wrapper()
-        self.assertDictEqual(agent._hooks, original_hooks)
-
-    def test_detach_wrappers(self):
-        agent = mk_agent()
-        original_hooks = agent._hooks.copy()
-        wrapped = wrappers_agents.Log(
-            wrappers_agents.RecordUpdates(agent),
-            level=logging.DEBUG,
-            log_frequencies={"on_timestep_end": 1000},
-        )
-        with self.assertRaises(AssertionError):
-            self.assertDictEqual(agent._hooks, original_hooks)
-        wrapped.detach_wrappers()
-        self.assertDictEqual(agent._hooks, original_hooks)
-
-
-class TestLog(unittest.TestCase):
-    def setUp(self):
-        self.agent = mk_agent()
-        self.env = SimpleEnv()
-        self.name = "test_logger"
-        self.log = None
-
-    def tearDown(self) -> None:
-        # remove logging files with name "DummyLearningAgent*.txt"
-        for handler in self.log.logger.handlers:
-            if isinstance(handler, logging.FileHandler):
-                handler.close()
-                if os.path.isfile(handler.baseFilename):
-                    os.remove(handler.baseFilename)
-
-    def test_init__to_file__creates_log_file(self):
-        self.log = wrappers_agents.Log(self.agent, to_file=True)
-        found = False
-        for handler in self.log.logger.handlers:
-            if isinstance(
-                handler, logging.FileHandler
-            ) and handler.baseFilename.endswith(f"{self.agent.name}.txt"):
-                found = True
-                break
-        self.assertTrue(found)
-
-    def test_init__establishes_correct_hooks(self):
-        agent = DummyAgent(get_mpc(3, False))
-        log_frequencies = {
-            "on_episode_start": 2,
-            "on_episode_end": 3,
-            "on_env_step": 4,
-            "on_timestep_end": 5,
-            "on_update": 6,
-        }
-        exclude_mandatory = ["on_mpc_failure", "on_validation_start"]
-        self.log = wrappers_agents.Log(
-            agent, log_frequencies=log_frequencies, exclude_mandatory=exclude_mandatory
-        )
-
-        expected_hooks = {
-            "on_episode_start",
-            "on_episode_end",
-            "on_env_step",
-            "on_timestep_end",
-            "on_validation_end",
-        }
-        actual_hooks = set(self.log.unwrapped._hooks.keys())
-        self.assertEqual(len(set.difference(expected_hooks, actual_hooks)), 0)
-
-    def test_on_mpc_failure(self):
-        episode = 1
-        timestep = 10
-        status = "failed"
-        raises = False
-        self.log = wrappers_agents.Log(self.agent)
-        with self.assertLogs(self.log.logger, logging.WARNING):
-            self.log.on_mpc_failure(episode, timestep, status, raises)
-
-    def test_on_validation_start(self):
-        self.log = wrappers_agents.Log(self.agent)
-        with self.assertLogs(self.log.logger, logging.DEBUG):
-            self.log.on_validation_start(self.env)
-
-    def test_on_validation_end(self):
-        returns = np.array([1.0, 2.0, 3.0])
-        self.log = wrappers_agents.Log(self.agent)
-        with self.assertLogs(self.log.logger, logging.INFO):
-            self.log.on_validation_end(self.env, returns)
-
-    def test_on_episode_start(self):
-        episode = 1
-        state = np.array([1, 2, 3])
-        self.log = wrappers_agents.Log(
-            self.agent, log_frequencies={"on_episode_start": 1}
-        )
-        with self.assertLogs(self.log.logger, logging.DEBUG):
-            self.log.on_episode_start(self.env, episode, state)
-
-    def test_on_episode_end(self):
-        episode = 1
-        rewards = 10.0
-        self.log = wrappers_agents.Log(
-            self.agent, log_frequencies={"on_episode_end": 1}
-        )
-        with self.assertLogs(self.log.logger, logging.INFO):
-            self.log.on_episode_end(self.env, episode, rewards)
-
-    def test_on_env_step(self):
-        episode = 1
-        timestep = 10
-        self.log = wrappers_agents.Log(self.agent, log_frequencies={"on_env_step": 1})
-        with self.assertLogs(self.log.logger, logging.DEBUG):
-            self.log.on_env_step(self.env, episode, timestep)
-
-    def test_on_timestep_end(self):
-        episode = 1
-        timestep = 10
-        self.log = wrappers_agents.Log(
-            self.agent, log_frequencies={"on_timestep_end": 1}
-        )
-        with self.assertLogs(self.log.logger, logging.DEBUG):
-            self.log.on_timestep_end(self.env, episode, timestep)
-
-    def test_on_update_failure(self):
-        episode = 1
-        timestep = 10
-        errormsg = "update failed"
-        raises = False
-        self.log = wrappers_agents.Log(self.agent)
-        with self.assertLogs(self.log.logger, logging.WARNING):
-            self.log.on_update_failure(episode, timestep, errormsg, raises)
-
-    def test_on_training_start(self):
-        self.log = wrappers_agents.Log(self.agent)
-        with self.assertLogs(self.log.logger, logging.DEBUG):
-            self.log.on_training_start(self.env)
-
-    def test_on_training_end(self):
-        returns = np.array([1.0, 2.0, 3.0])
-        self.log = wrappers_agents.Log(self.agent)
-        with self.assertLogs(self.log.logger, logging.INFO):
-            self.log.on_training_end(self.env, returns)
-
-    def test_on_update(self):
-        self.log = wrappers_agents.Log(self.agent, log_frequencies={"on_update": 1})
-        with self.assertLogs(self.log.logger, logging.INFO):
-            self.log.on_update()
-
-
-class TestRecordUpdates(unittest.TestCase):
-    def test__update__records_learnable_parameters_correctly(self):
-        n_params, n_updates = 3, 10
-        pars = np.random.rand(n_updates + 1, n_params)
-        parsdict = LearnableParametersDict(
-            [LearnableParameter(f"p{i}", 1, pars[0, i]) for i in range(n_params)]
-        )
-        agent = mk_agent()
-        agent._learnable_pars = parsdict
-        on_update_original = agent.on_update
-        pars_iter = iter(pars[1:])
-
-        def side_effect():
-            agent.learnable_parameters.update_values(next(pars_iter))
-            on_update_original()
-
-        agent.on_update = Mock(return_value=None, side_effect=side_effect)
-        wrapped = wrappers_agents.RecordUpdates(agent)
-
-        for _ in range(n_updates):
-            wrapped.on_update()
-
-        agent.on_update.assert_has_calls([call()] * n_updates)
-        self.assertListEqual(
-            [f"p{i}" for i in range(n_params)], list(wrapped.updates_history.keys())
-        )
-        pars_actual = np.squeeze(list(wrapped.updates_history.values())).T
-        np.testing.assert_equal(pars_actual, pars)
-
-
-class TestMonitorEpisodesAndInfos(unittest.TestCase):
-    def test__compact_dicts(self):
-        act = compact_dicts(
-            [
-                {"a": 3, "b": 2},
-                {"b": 3, "c": 2},
-                {"a": 3, "c": 2},
-                {"c": 3, "d": 2},
-                {"a": 3, "d": 2},
-            ],
-            fill_value=np.nan,
-        )
-        exp = {
-            "a": [3, np.nan, 3, np.nan, 3],
-            "b": [2, 3, np.nan, np.nan, np.nan],
-            "c": [np.nan, 2, 2, 3, np.nan],
-            "d": [np.nan, np.nan, np.nan, 2, 2],
-        }
-        self.assertDictEqual(act, exp)
-
-    def test_monitor_infos__records_infos_correctly(self):
-        env = wrappers_envs.MonitorInfos(SimpleEnv())
-        n_episodes = 3
-        for _ in range(n_episodes):
-            env.reset()
-            terminated = truncated = False
-            while not (terminated or truncated):
-                _, _, terminated, truncated, _ = env.step(object())
-        self.assertListEqual(list(env.reset_infos), env.INTERNAL_RESET_INFOS)
-        self.assertDictEqual(
-            env.finalized_reset_infos(), env.INTERNAL_FINALIZED_RESET_INFOS
-        )
-        self.assertListEqual(list(env.step_infos), env.INTERNAL_STEP_INFOS)
-        self.assertDictEqual(
-            env.finalized_step_infos(), env.INTERNAL_FINALIZED_STEP_INFOS
-        )
-
-    def test_monitor_episodes__records_episodes_correctly(self):
-        env = wrappers_envs.MonitorEpisodes(SimpleEnv())
-        n_episodes = 3
-        for _ in range(n_episodes):
-            env.reset()
-            terminated = truncated = False
-            while not (terminated or truncated):
-                _, _, terminated, truncated, _ = env.step(object())
-        np.testing.assert_array_equal(env.observations, env.INTERNAL_OBSERVATIONS)
-        np.testing.assert_array_equal(env.actions, env.INTERNAL_ACTIONS)
-        np.testing.assert_array_equal(env.rewards, env.INTERNAL_REWARDS)
-        self.assertListEqual(list(env.episode_lengths), [env.T_MAX] * n_episodes)
-
-
-if __name__ == "__main__":
-    unittest.main()
+import logging
+import os
+import unittest
+from functools import lru_cache
+from typing import Any
+from unittest.mock import Mock, call
+
+import casadi as cs
+import gymnasium as gym
+import numpy as np
+from csnlp import Nlp, scaling
+from csnlp.multistart import StackedMultistartNlp
+from csnlp.wrappers import Mpc, NlpScaling
+
+from mpcrl import (
+    Agent,
+    LearnableParameter,
+    LearnableParametersDict,
+    LearningAgent,
+    wrappers_agents,
+    wrappers_envs,
+)
+from mpcrl.wrappers.envs.monitor_infos import compact_dicts
+
+
+@lru_cache
+def get_dynamics(g: float, alpha: float, dt: float) -> cs.Function:
+    x, u, d = cs.SX.sym("x", 3), cs.SX.sym("u", 2), cs.SX.sym("d", 3)
+    x_next = x + cs.vertcat(x[1], u[0] / x[2] - g, -alpha * u[0]) * dt + d * 0
+    return cs.Function("F", [x, u, d], [x_next], ["x", "u", "d"], ["x+"])
+
+
+def get_mpc(horizon: int, multistart: bool):
+    N = horizon
+    T = 100
+    K = 3
+    dt = T / N
+    yT = 100000
+    g = 9.81
+    alpha = 1 / (300 * g)
+    y_nom = 1e5
+    v_nom = 2e3
+    m_nom = 3e5
+    u_nom = 1e8
+    scaler = scaling.Scaler()
+    scaler.register("y", scale=y_nom)
+    scaler.register("y_0", scale=y_nom)
+    scaler.register("v", scale=v_nom)
+    scaler.register("v_0", scale=v_nom)
+    scaler.register("m", scale=m_nom)
+    scaler.register("m_0", scale=m_nom)
+    scaler.register("u1", scale=u_nom)
+    scaler.register("u2", scale=u_nom)
+    nlp = (
+        StackedMultistartNlp[cs.MX](sym_type="MX", starts=K)
+        if multistart
+        else Nlp[cs.MX](sym_type="MX")
+    )
+    nlp = NlpScaling[cs.MX](nlp, scaler=scaler)
+    mpc = Mpc[cs.MX](nlp, prediction_horizon=N)
+    y, _ = mpc.state("y")
+    _, _ = mpc.state("v")
+    m, _ = mpc.state("m", lb=0)
+    mpc.action("u1", lb=0, ub=5e7)
+    u2, _ = mpc.action("u2", lb=0, ub=5e7)
+    mpc.disturbance("d", 3)
+    mpc.set_dynamics(get_dynamics(g, alpha, dt))
+    mpc.constraint("yT", y[-1], "==", yT)
+    mpc.minimize(m[0] - m[-1] + cs.sum2(u2))
+    mpc.init_solver()
+    return mpc
+
+
+class DummyAgent(Agent):
+    ...
+
+
+class DummyLearningAgent(LearningAgent):
+    def update(self, *args, **kwargs):
+        return
+
+    def train_one_episode(self, *args, **kwargs):
+        return
+
+
+def mk_agent() -> DummyLearningAgent:
+    return DummyLearningAgent(
+        mpc=get_mpc(3, False),
+        learnable_parameters=LearnableParametersDict(),
+        update_strategy=1,
+    )
+
+
+class SimpleEnv(gym.Env[object, object]):
+    T_MAX = 10
+
+    def __init__(self, *args: Any, **kwargs: Any):
+        super().__init__(*args, **kwargs)
+        self.INTERNAL_RESET_INFOS = []
+        self.INTERNAL_FINALIZED_RESET_INFOS = {"reset_info": []}
+        self.INTERNAL_STEP_INFOS = []
+        self.INTERNAL_FINALIZED_STEP_INFOS = {"step_info": []}
+        self.INTERNAL_OBSERVATIONS = []
+        self.INTERNAL_ACTIONS = []
+        self.INTERNAL_REWARDS = []
+
+    def reset(self, *args: Any, **kwargs: Any) -> tuple[object, dict[str, Any]]:
+        super().reset(*args, **kwargs)
+        self.t = 0
+        obs = object()
+        info = {"reset_info": object()}
+        self.INTERNAL_RESET_INFOS.append(info)
+        self.INTERNAL_FINALIZED_RESET_INFOS["reset_info"].append(info["reset_info"])
+        self.INTERNAL_STEP_INFOS.append([])
+        self.INTERNAL_FINALIZED_STEP_INFOS["step_info"].append([])
+        self.INTERNAL_OBSERVATIONS.append([obs])
+        self.INTERNAL_ACTIONS.append([])
+        self.INTERNAL_REWARDS.append([])
+        return obs, info
+
+    def step(self, action: object) -> tuple[object, float, bool, bool, dict[str, Any]]:
+        self.t += 1
+        obs = object()
+        reward = np.random.rand()
+        terminated = self.t >= self.T_MAX
+        info = {"step_info": object()}
+        self.INTERNAL_STEP_INFOS[-1].append(info)
+        self.INTERNAL_FINALIZED_STEP_INFOS["step_info"][-1].append(info["step_info"])
+        self.INTERNAL_OBSERVATIONS[-1].append(obs)
+        self.INTERNAL_ACTIONS[-1].append(action)
+        self.INTERNAL_REWARDS[-1].append(reward)
+        return obs, reward, terminated, False, info
+
+
+class TestWrapperAndLearningWrapper(unittest.TestCase):
+    def test_attr__raises__when_accessing_private_attrs(self):
+        wrapped = wrappers_agents.LearningWrapper(mk_agent())
+        with self.assertRaisesRegex(
+            AttributeError, "Accessing private attribute '_x' is prohibited."
+        ):
+            wrapped._x
+
+    def test_unwrapped__unwraps_nlp_correctly(self):
+        agent = mk_agent()
+        wrapped = wrappers_agents.LearningWrapper(agent)
+        self.assertIs(agent, wrapped.unwrapped)
+
+    def test_str_and_repr(self):
+        agent = mk_agent()
+        wrapped = wrappers_agents.LearningWrapper(agent)
+        S = wrapped.__str__()
+        self.assertIn(wrappers_agents.LearningWrapper.__name__, S)
+        self.assertIn(agent.__str__(), S)
+        S = wrapped.__repr__()
+        self.assertIn(wrappers_agents.LearningWrapper.__name__, S)
+        self.assertIn(agent.__repr__(), S)
+
+    def test_is_wrapped(self):
+        agent = mk_agent()
+        self.assertFalse(agent.is_wrapped())
+
+        wrapped = wrappers_agents.LearningWrapper(agent)
+        self.assertTrue(wrapped.is_wrapped(wrappers_agents.LearningWrapper))
+        self.assertFalse(wrapped.is_wrapped(cs.SX))
+
+    def test_detach_wrapper(self):
+        agent = mk_agent()
+        wrapped_intermediate = wrappers_agents.RecordUpdates(agent)
+        original_hooks = agent._hooks.copy()
+        wrapped = wrappers_agents.Log(
+            wrapped_intermediate,
+            level=logging.DEBUG,
+            log_frequencies={"on_timestep_end": 1000},
+        )
+        with self.assertRaises(AssertionError):
+            self.assertDictEqual(agent._hooks, original_hooks)
+        wrapped.detach_wrapper()
+        self.assertDictEqual(agent._hooks, original_hooks)
+
+    def test_detach_wrappers(self):
+        agent = mk_agent()
+        original_hooks = agent._hooks.copy()
+        wrapped = wrappers_agents.Log(
+            wrappers_agents.RecordUpdates(agent),
+            level=logging.DEBUG,
+            log_frequencies={"on_timestep_end": 1000},
+        )
+        with self.assertRaises(AssertionError):
+            self.assertDictEqual(agent._hooks, original_hooks)
+        wrapped.detach_wrappers()
+        self.assertDictEqual(agent._hooks, original_hooks)
+
+
+class TestLog(unittest.TestCase):
+    def setUp(self):
+        self.agent = mk_agent()
+        self.env = SimpleEnv()
+        self.name = "test_logger"
+        self.log = None
+
+    def tearDown(self) -> None:
+        # remove logging files with name "DummyLearningAgent*.txt"
+        for handler in self.log.logger.handlers:
+            if isinstance(handler, logging.FileHandler):
+                handler.close()
+                if os.path.isfile(handler.baseFilename):
+                    os.remove(handler.baseFilename)
+
+    def test_init__to_file__creates_log_file(self):
+        self.log = wrappers_agents.Log(self.agent, to_file=True)
+        found = False
+        for handler in self.log.logger.handlers:
+            if isinstance(
+                handler, logging.FileHandler
+            ) and handler.baseFilename.endswith(f"{self.agent.name}.txt"):
+                found = True
+                break
+        self.assertTrue(found)
+
+    def test_init__establishes_correct_hooks(self):
+        agent = DummyAgent(get_mpc(3, False))
+        log_frequencies = {
+            "on_episode_start": 2,
+            "on_episode_end": 3,
+            "on_env_step": 4,
+            "on_timestep_end": 5,
+            "on_update": 6,
+        }
+        exclude_mandatory = ["on_mpc_failure", "on_validation_start"]
+        self.log = wrappers_agents.Log(
+            agent, log_frequencies=log_frequencies, exclude_mandatory=exclude_mandatory
+        )
+
+        expected_hooks = {
+            "on_episode_start",
+            "on_episode_end",
+            "on_env_step",
+            "on_timestep_end",
+            "on_validation_end",
+        }
+        actual_hooks = set(self.log.unwrapped._hooks.keys())
+        self.assertEqual(len(set.difference(expected_hooks, actual_hooks)), 0)
+
+    def test_on_mpc_failure(self):
+        episode = 1
+        timestep = 10
+        status = "failed"
+        raises = False
+        self.log = wrappers_agents.Log(self.agent)
+        with self.assertLogs(self.log.logger, logging.WARNING):
+            self.log.on_mpc_failure(episode, timestep, status, raises)
+
+    def test_on_validation_start(self):
+        self.log = wrappers_agents.Log(self.agent)
+        with self.assertLogs(self.log.logger, logging.DEBUG):
+            self.log.on_validation_start(self.env)
+
+    def test_on_validation_end(self):
+        returns = np.array([1.0, 2.0, 3.0])
+        self.log = wrappers_agents.Log(self.agent)
+        with self.assertLogs(self.log.logger, logging.INFO):
+            self.log.on_validation_end(self.env, returns)
+
+    def test_on_episode_start(self):
+        episode = 1
+        state = np.array([1, 2, 3])
+        self.log = wrappers_agents.Log(
+            self.agent, log_frequencies={"on_episode_start": 1}
+        )
+        with self.assertLogs(self.log.logger, logging.DEBUG):
+            self.log.on_episode_start(self.env, episode, state)
+
+    def test_on_episode_end(self):
+        episode = 1
+        rewards = 10.0
+        self.log = wrappers_agents.Log(
+            self.agent, log_frequencies={"on_episode_end": 1}
+        )
+        with self.assertLogs(self.log.logger, logging.INFO):
+            self.log.on_episode_end(self.env, episode, rewards)
+
+    def test_on_env_step(self):
+        episode = 1
+        timestep = 10
+        self.log = wrappers_agents.Log(self.agent, log_frequencies={"on_env_step": 1})
+        with self.assertLogs(self.log.logger, logging.DEBUG):
+            self.log.on_env_step(self.env, episode, timestep)
+
+    def test_on_timestep_end(self):
+        episode = 1
+        timestep = 10
+        self.log = wrappers_agents.Log(
+            self.agent, log_frequencies={"on_timestep_end": 1}
+        )
+        with self.assertLogs(self.log.logger, logging.DEBUG):
+            self.log.on_timestep_end(self.env, episode, timestep)
+
+    def test_on_update_failure(self):
+        episode = 1
+        timestep = 10
+        errormsg = "update failed"
+        raises = False
+        self.log = wrappers_agents.Log(self.agent)
+        with self.assertLogs(self.log.logger, logging.WARNING):
+            self.log.on_update_failure(episode, timestep, errormsg, raises)
+
+    def test_on_training_start(self):
+        self.log = wrappers_agents.Log(self.agent)
+        with self.assertLogs(self.log.logger, logging.DEBUG):
+            self.log.on_training_start(self.env)
+
+    def test_on_training_end(self):
+        returns = np.array([1.0, 2.0, 3.0])
+        self.log = wrappers_agents.Log(self.agent)
+        with self.assertLogs(self.log.logger, logging.INFO):
+            self.log.on_training_end(self.env, returns)
+
+    def test_on_update(self):
+        self.log = wrappers_agents.Log(self.agent, log_frequencies={"on_update": 1})
+        with self.assertLogs(self.log.logger, logging.INFO):
+            self.log.on_update()
+
+
+class TestRecordUpdates(unittest.TestCase):
+    def test__update__records_learnable_parameters_correctly(self):
+        n_params, n_updates = 3, 10
+        pars = np.random.rand(n_updates + 1, n_params)
+        parsdict = LearnableParametersDict(
+            [LearnableParameter(f"p{i}", 1, pars[0, i]) for i in range(n_params)]
+        )
+        agent = mk_agent()
+        agent._learnable_pars = parsdict
+        on_update_original = agent.on_update
+        pars_iter = iter(pars[1:])
+
+        def side_effect():
+            agent.learnable_parameters.update_values(next(pars_iter))
+            on_update_original()
+
+        agent.on_update = Mock(return_value=None, side_effect=side_effect)
+        wrapped = wrappers_agents.RecordUpdates(agent)
+
+        for _ in range(n_updates):
+            wrapped.on_update()
+
+        agent.on_update.assert_has_calls([call()] * n_updates)
+        self.assertListEqual(
+            [f"p{i}" for i in range(n_params)], list(wrapped.updates_history.keys())
+        )
+        pars_actual = np.squeeze(list(wrapped.updates_history.values())).T
+        np.testing.assert_equal(pars_actual, pars)
+
+
+class TestMonitorEpisodesAndInfos(unittest.TestCase):
+    def test__compact_dicts(self):
+        act = compact_dicts(
+            [
+                {"a": 3, "b": 2},
+                {"b": 3, "c": 2},
+                {"a": 3, "c": 2},
+                {"c": 3, "d": 2},
+                {"a": 3, "d": 2},
+            ],
+            fill_value=np.nan,
+        )
+        exp = {
+            "a": [3, np.nan, 3, np.nan, 3],
+            "b": [2, 3, np.nan, np.nan, np.nan],
+            "c": [np.nan, 2, 2, 3, np.nan],
+            "d": [np.nan, np.nan, np.nan, 2, 2],
+        }
+        self.assertDictEqual(act, exp)
+
+    def test_monitor_infos__records_infos_correctly(self):
+        env = wrappers_envs.MonitorInfos(SimpleEnv())
+        n_episodes = 3
+        for _ in range(n_episodes):
+            env.reset()
+            terminated = truncated = False
+            while not (terminated or truncated):
+                _, _, terminated, truncated, _ = env.step(object())
+        self.assertListEqual(list(env.reset_infos), env.INTERNAL_RESET_INFOS)
+        self.assertDictEqual(
+            env.finalized_reset_infos(), env.INTERNAL_FINALIZED_RESET_INFOS
+        )
+        self.assertListEqual(list(env.step_infos), env.INTERNAL_STEP_INFOS)
+        self.assertDictEqual(
+            env.finalized_step_infos(), env.INTERNAL_FINALIZED_STEP_INFOS
+        )
+
+    def test_monitor_episodes__records_episodes_correctly(self):
+        env = wrappers_envs.MonitorEpisodes(SimpleEnv())
+        n_episodes = 3
+        for _ in range(n_episodes):
+            env.reset()
+            terminated = truncated = False
+            while not (terminated or truncated):
+                _, _, terminated, truncated, _ = env.step(object())
+        np.testing.assert_array_equal(env.observations, env.INTERNAL_OBSERVATIONS)
+        np.testing.assert_array_equal(env.actions, env.INTERNAL_ACTIONS)
+        np.testing.assert_array_equal(env.rewards, env.INTERNAL_REWARDS)
+        self.assertListEqual(list(env.episode_lengths), [env.T_MAX] * n_episodes)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

