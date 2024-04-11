# Comparing `tmp/sponet-2.0.0.tar.gz` & `tmp/sponet-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sponet-2.0.0.tar", max compression
+gzip compressed data, was "sponet-2.1.0.tar", max compression
```

## Comparing `sponet-2.0.0.tar` & `sponet-2.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35823 2023-09-15 13:06:59.296676 sponet-2.0.0/LICENSE
--rw-r--r--   0        0        0     1179 2023-12-05 12:41:15.587980 sponet-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     7248 2023-10-13 13:05:27.269509 sponet-2.0.0/README.md
--rw-r--r--   0        0        0      323 2023-12-05 12:40:13.920724 sponet-2.0.0/sponet/__init__.py
--rw-r--r--   0        0        0       65 2023-09-15 12:01:58.035010 sponet-2.0.0/sponet/cntm/__init__.py
--rw-r--r--   0        0        0      296 2023-09-15 12:17:38.270985 sponet-2.0.0/sponet/cntm/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4747 2023-11-30 16:52:47.741405 sponet-2.0.0/sponet/cntm/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0     1471 2023-09-15 10:09:44.694324 sponet-2.0.0/sponet/cntm/__pycache__/parameters.cpython-311.pyc
--rw-r--r--   0        0        0     3463 2023-11-27 16:05:49.305015 sponet-2.0.0/sponet/cntm/model.py
--rw-r--r--   0        0        0      716 2023-09-15 10:00:00.042086 sponet-2.0.0/sponet/cntm/parameters.py
--rw-r--r--   0        0        0      153 2023-12-05 12:40:13.921720 sponet-2.0.0/sponet/cnvm/__init__.py
--rw-r--r--   0        0        0      427 2023-12-04 13:31:39.859542 sponet-2.0.0/sponet/cnvm/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1866 2023-10-27 07:04:14.127956 sponet-2.0.0/sponet/cnvm/__pycache__/distr_sampling.cpython-311.pyc
--rw-r--r--   0        0        0    10403 2023-11-27 16:03:00.367350 sponet-2.0.0/sponet/cnvm/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0    12482 2023-09-15 09:53:50.188410 sponet-2.0.0/sponet/cnvm/__pycache__/parameters.cpython-311.pyc
--rw-r--r--   0        0        0      174 2023-12-05 12:40:13.921720 sponet-2.0.0/sponet/cnvm/approximations/__init__.py
--rw-r--r--   0        0        0      433 2023-12-04 13:31:39.876215 sponet-2.0.0/sponet/cnvm/approximations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4928 2023-12-04 15:03:30.404902 sponet-2.0.0/sponet/cnvm/approximations/__pycache__/chemical_langevin_equation.cpython-311.pyc
--rw-r--r--   0        0        0     2275 2023-12-04 12:52:28.609082 sponet-2.0.0/sponet/cnvm/approximations/__pycache__/reaction_rate_equation.cpython-311.pyc
--rw-r--r--   0        0        0     5180 2023-12-05 09:21:25.957577 sponet-2.0.0/sponet/cnvm/approximations/__pycache__/stochastic_approximation.cpython-311.pyc
--rw-r--r--   0        0        0     3388 2023-12-05 12:40:13.922717 sponet-2.0.0/sponet/cnvm/approximations/chemical_langevin_equation.py
--rw-r--r--   0        0        0     1501 2023-12-05 12:40:13.922717 sponet-2.0.0/sponet/cnvm/approximations/reaction_rate_equation.py
--rw-r--r--   0        0        0     3560 2023-12-05 12:40:13.922717 sponet-2.0.0/sponet/cnvm/approximations/stochastic_approximation.py
--rw-r--r--   0        0        0     8074 2023-11-27 16:02:59.305263 sponet-2.0.0/sponet/cnvm/model.py
--rw-r--r--   0        0        0     9559 2023-09-15 09:53:49.775246 sponet-2.0.0/sponet/cnvm/parameters.py
--rw-r--r--   0        0        0     9589 2023-09-15 09:53:49.760295 sponet-2.0.0/sponet/collective_variables.py
--rw-r--r--   0        0        0     5260 2023-12-05 12:40:13.922717 sponet-2.0.0/sponet/multiprocessing.py
--rw-r--r--   0        0        0    13548 2023-11-30 17:12:28.017482 sponet-2.0.0/sponet/network_generator.py
--rw-r--r--   0        0        0      766 2023-09-15 09:53:49.781226 sponet-2.0.0/sponet/parameters.py
--rw-r--r--   0        0        0     1601 2023-12-05 12:40:13.923714 sponet-2.0.0/sponet/plotting.py
--rw-r--r--   0        0        0     3260 2023-11-27 16:01:22.351959 sponet-2.0.0/sponet/sampling.py
--rw-r--r--   0        0        0     1007 2023-12-05 12:40:13.923714 sponet-2.0.0/sponet/utils.py
--rw-r--r--   0        0        0     8174 1970-01-01 00:00:00.000000 sponet-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-09-15 13:06:59.296676 sponet-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1179 2024-04-11 14:32:35.526918 sponet-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7252 2024-04-10 20:09:40.061228 sponet-2.1.0/README.md
+-rw-r--r--   0        0        0      323 2023-12-05 12:40:13.920724 sponet-2.1.0/sponet/__init__.py
+-rw-r--r--   0        0        0       65 2023-09-15 12:01:58.035010 sponet-2.1.0/sponet/cntm/__init__.py
+-rw-r--r--   0        0        0      296 2023-09-15 12:17:38.270985 sponet-2.1.0/sponet/cntm/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4747 2023-11-30 16:52:47.741405 sponet-2.1.0/sponet/cntm/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0        0        0     1471 2023-09-15 10:09:44.694324 sponet-2.1.0/sponet/cntm/__pycache__/parameters.cpython-311.pyc
+-rw-r--r--   0        0        0     3463 2023-11-27 16:05:49.305015 sponet-2.1.0/sponet/cntm/model.py
+-rw-r--r--   0        0        0      716 2023-09-15 10:00:00.042086 sponet-2.1.0/sponet/cntm/parameters.py
+-rw-r--r--   0        0        0      153 2023-12-05 12:40:13.921720 sponet-2.1.0/sponet/cnvm/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-10 17:18:46.857252 sponet-2.1.0/sponet/cnvm/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1866 2023-10-27 07:04:14.127956 sponet-2.1.0/sponet/cnvm/__pycache__/distr_sampling.cpython-311.pyc
+-rw-r--r--   0        0        0    10403 2023-11-27 16:03:00.367350 sponet-2.1.0/sponet/cnvm/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0        0        0    12482 2023-09-15 09:53:50.188410 sponet-2.1.0/sponet/cnvm/__pycache__/parameters.cpython-311.pyc
+-rw-r--r--   0        0        0      174 2023-12-05 12:40:13.921720 sponet-2.1.0/sponet/cnvm/approximations/__init__.py
+-rw-r--r--   0        0        0      433 2024-04-10 17:18:46.894809 sponet-2.1.0/sponet/cnvm/approximations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4928 2024-04-10 17:18:46.896806 sponet-2.1.0/sponet/cnvm/approximations/__pycache__/chemical_langevin_equation.cpython-311.pyc
+-rw-r--r--   0        0        0     2275 2024-04-10 17:18:46.897806 sponet-2.1.0/sponet/cnvm/approximations/__pycache__/reaction_rate_equation.cpython-311.pyc
+-rw-r--r--   0        0        0     5597 2024-04-10 17:18:47.423921 sponet-2.1.0/sponet/cnvm/approximations/__pycache__/stochastic_approximation.cpython-311.pyc
+-rw-r--r--   0        0        0     3388 2023-12-05 12:40:13.922717 sponet-2.1.0/sponet/cnvm/approximations/chemical_langevin_equation.py
+-rw-r--r--   0        0        0     1501 2023-12-05 12:40:13.922717 sponet-2.1.0/sponet/cnvm/approximations/reaction_rate_equation.py
+-rw-r--r--   0        0        0     3560 2023-12-05 12:40:13.922717 sponet-2.1.0/sponet/cnvm/approximations/stochastic_approximation.py
+-rw-r--r--   0        0        0     8074 2023-11-27 16:02:59.305263 sponet-2.1.0/sponet/cnvm/model.py
+-rw-r--r--   0        0        0     9559 2023-09-15 09:53:49.775246 sponet-2.1.0/sponet/cnvm/parameters.py
+-rw-r--r--   0        0        0     9591 2024-04-10 20:10:36.719875 sponet-2.1.0/sponet/collective_variables.py
+-rw-r--r--   0        0        0     5260 2023-12-05 12:40:13.922717 sponet-2.1.0/sponet/multiprocessing.py
+-rw-r--r--   0        0        0    14327 2024-04-11 14:32:35.527918 sponet-2.1.0/sponet/network_generator.py
+-rw-r--r--   0        0        0      766 2023-09-15 09:53:49.781226 sponet-2.1.0/sponet/parameters.py
+-rw-r--r--   0        0        0     1601 2023-12-05 12:40:13.923714 sponet-2.1.0/sponet/plotting.py
+-rw-r--r--   0        0        0     3288 2024-04-10 20:10:36.653358 sponet-2.1.0/sponet/sampling.py
+-rw-r--r--   0        0        0     1007 2023-12-05 12:40:13.923714 sponet-2.1.0/sponet/utils.py
+-rw-r--r--   0        0        0     8178 1970-01-01 00:00:00.000000 sponet-2.1.0/PKG-INFO
```

### Comparing `sponet-2.0.0/LICENSE` & `sponet-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/pyproject.toml` & `sponet-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sponet"
-version = "2.0.0"
+version = "2.1.0"
 description = "Spreading Processes on Networks"
 license = "GPL-3.0-or-later"
 authors = ["Marvin Lücke"]
 readme = "README.md"
 repository = "https://github.com/lueckem/SPoNet"
 keywords = [
     "voter model",
@@ -33,15 +33,15 @@
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
-black = "^23.3.0"
+black = "^24.3.0"
 
 
 [tool.poetry.group.notebooks]
 optional = true
 
 [tool.poetry.group.notebooks.dependencies]
 ipykernel = "^6.22.0"
```

### Comparing `sponet-2.0.0/README.md` & `sponet-2.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Spreading Processes on Networks (SPoNet)
 
-[![build](https://github.com/lueckem/cnvm/actions/workflows/build.yml/badge.svg)](https://github.com/lueckem/cnvm/actions/workflows/build.yml)
+[![build](https://github.com/lueckem/SPoNet/actions/workflows/build.yml/badge.svg)](https://github.com/lueckem/SPoNet/actions/workflows/build.yml)
 
 This package provides an efficient implementation of popular discrete-state spreading processes on networks of interacting *agents*.
 They can be used to simulate how opinions about certain issues develop over time within a population, or how an infectious disease spreads.
 The simulation loop is just-in-time compiled using `numba`, which makes performance comparable with compiled languages like C++.
 
 Available models:
 - continuous-time noisy voter model (CNVM)
```

### Comparing `sponet-2.0.0/sponet/cntm/__pycache__/model.cpython-311.pyc` & `sponet-2.1.0/sponet/cntm/__pycache__/model.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/cntm/__pycache__/parameters.cpython-311.pyc` & `sponet-2.1.0/sponet/cntm/__pycache__/parameters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/cntm/model.py` & `sponet-2.1.0/sponet/cntm/model.py`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/cntm/parameters.py` & `sponet-2.1.0/sponet/cntm/parameters.py`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/cnvm/__pycache__/distr_sampling.cpython-311.pyc` & `sponet-2.1.0/sponet/cnvm/__pycache__/distr_sampling.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/cnvm/__pycache__/model.cpython-311.pyc` & `sponet-2.1.0/sponet/cnvm/__pycache__/model.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/cnvm/__pycache__/parameters.cpython-311.pyc` & `sponet-2.1.0/sponet/cnvm/__pycache__/parameters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/cnvm/approximations/__pycache__/chemical_langevin_equation.cpython-311.pyc` & `sponet-2.1.0/sponet/cnvm/approximations/__pycache__/chemical_langevin_equation.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xe9e86d65 (Mon Dec  4 14:57:45 2023 UTC)
+moddate:  0x2d1a6f65 (Tue Dec  5 12:40:13 2023 UTC)
 files sz: 3388
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 21
    flags     : 0
    code
```

### Comparing `sponet-2.0.0/sponet/cnvm/approximations/__pycache__/reaction_rate_equation.cpython-311.pyc` & `sponet-2.1.0/sponet/cnvm/approximations/__pycache__/reaction_rate_equation.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x77ca6d65 (Mon Dec  4 12:47:51 2023 UTC)
+moddate:  0x2d1a6f65 (Tue Dec  5 12:40:13 2023 UTC)
 files sz: 1501
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `sponet-2.0.0/sponet/cnvm/approximations/__pycache__/stochastic_approximation.cpython-311.pyc` & `sponet-2.1.0/sponet/cnvm/approximations/__pycache__/stochastic_approximation.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x95eb6e65 (Tue Dec  5 09:21:25 2023 UTC)
-files sz: 3135
+moddate:  0x2d1a6f65 (Tue Dec  5 12:40:13 2023 UTC)
+files sz: 3560
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 15
    flags     : 0
    code
       0x9700640064016c005a01640064026c026d035a036d045a040100640364
@@ -83,143 +83,143 @@
                110 BINARY_SUBSCR
    
      8         120 BUILD_TUPLE             12
                122 LOAD_CONST              13 (<code object sample_stochastic_approximation, file "C:\Users\Marvin\PycharmProjects\SPoNet\sponet\cnvm\approximations\stochastic_approximation.py", line 8>)
                124 MAKE_FUNCTION            4 (annotations)
                126 STORE_NAME              13 (sample_stochastic_approximation)
    
-    42         128 PUSH_NULL
+    51         128 PUSH_NULL
                130 LOAD_NAME                3 (njit)
                132 LOAD_CONST              14 (True)
                134 KW_NAMES                15
                136 PRECALL                  1
                140 CALL                     1
    
-    43         150 LOAD_CONST               8 ('initial_state')
+    52         150 LOAD_CONST               8 ('initial_state')
    
-    44         152 LOAD_NAME                1 (np)
+    53         152 LOAD_NAME                1 (np)
                154 LOAD_ATTR                9 (ndarray)
    
-    43         164 LOAD_CONST              16 ('t_max')
+    52         164 LOAD_CONST              16 ('t_max')
    
-    45         166 LOAD_NAME               10 (float)
+    54         166 LOAD_NAME               10 (float)
    
-    43         168 LOAD_CONST              17 ('num_agents')
+    52         168 LOAD_CONST              17 ('num_agents')
    
-    46         170 LOAD_NAME               11 (int)
+    55         170 LOAD_NAME               11 (int)
    
-    43         172 LOAD_CONST              18 ('r')
+    52         172 LOAD_CONST              18 ('r')
    
-    47         174 LOAD_NAME                1 (np)
+    56         174 LOAD_NAME                1 (np)
                176 LOAD_ATTR                9 (ndarray)
    
-    43         186 LOAD_CONST              19 ('r_tilde')
+    52         186 LOAD_CONST              19 ('r_tilde')
    
-    48         188 LOAD_NAME                1 (np)
+    57         188 LOAD_NAME                1 (np)
                190 LOAD_ATTR                9 (ndarray)
    
-    43         200 LOAD_CONST              10 ('num_timesteps')
+    52         200 LOAD_CONST              10 ('num_timesteps')
    
-    49         202 LOAD_NAME               11 (int)
+    58         202 LOAD_NAME               11 (int)
    
-    43         204 LOAD_CONST              11 ('num_samples')
+    52         204 LOAD_CONST              11 ('num_samples')
    
-    50         206 LOAD_NAME               11 (int)
+    59         206 LOAD_NAME               11 (int)
    
-    43         208 BUILD_TUPLE             14
-               210 LOAD_CONST              20 (<code object _sample_many, file "C:\Users\Marvin\PycharmProjects\SPoNet\sponet\cnvm\approximations\stochastic_approximation.py", line 42>)
+    52         208 BUILD_TUPLE             14
+               210 LOAD_CONST              20 (<code object _sample_many, file "C:\Users\Marvin\PycharmProjects\SPoNet\sponet\cnvm\approximations\stochastic_approximation.py", line 51>)
                212 MAKE_FUNCTION            4 (annotations)
    
-    42         214 PRECALL                  0
+    51         214 PRECALL                  0
                218 CALL                     0
    
-    43         228 STORE_NAME              14 (_sample_many)
+    52         228 STORE_NAME              14 (_sample_many)
    
-    74         230 LOAD_NAME                3 (njit)
+    83         230 LOAD_NAME                3 (njit)
    
-    75         232 LOAD_CONST               8 ('initial_state')
+    84         232 LOAD_CONST               8 ('initial_state')
    
-    76         234 LOAD_NAME                1 (np)
+    85         234 LOAD_NAME                1 (np)
                236 LOAD_ATTR                9 (ndarray)
    
-    75         246 LOAD_CONST              16 ('t_max')
+    84         246 LOAD_CONST              16 ('t_max')
    
-    77         248 LOAD_NAME               10 (float)
+    86         248 LOAD_NAME               10 (float)
    
-    75         250 LOAD_CONST              21 ('t_delta')
+    84         250 LOAD_CONST              21 ('t_delta')
    
-    78         252 LOAD_NAME               10 (float)
+    87         252 LOAD_NAME               10 (float)
    
-    75         254 LOAD_CONST              17 ('num_agents')
+    84         254 LOAD_CONST              17 ('num_agents')
    
-    79         256 LOAD_NAME               11 (int)
+    88         256 LOAD_NAME               11 (int)
    
-    75         258 LOAD_CONST              18 ('r')
+    84         258 LOAD_CONST              18 ('r')
    
-    80         260 LOAD_NAME                1 (np)
+    89         260 LOAD_NAME                1 (np)
                262 LOAD_ATTR                9 (ndarray)
    
-    75         272 LOAD_CONST              19 ('r_tilde')
+    84         272 LOAD_CONST              19 ('r_tilde')
    
-    81         274 LOAD_NAME                1 (np)
+    90         274 LOAD_NAME                1 (np)
                276 LOAD_ATTR                9 (ndarray)
    
-    75         286 BUILD_TUPLE             12
-               288 LOAD_CONST              22 (<code object _simulate, file "C:\Users\Marvin\PycharmProjects\SPoNet\sponet\cnvm\approximations\stochastic_approximation.py", line 74>)
+    84         286 BUILD_TUPLE             12
+               288 LOAD_CONST              22 (<code object _simulate, file "C:\Users\Marvin\PycharmProjects\SPoNet\sponet\cnvm\approximations\stochastic_approximation.py", line 83>)
                290 MAKE_FUNCTION            4 (annotations)
    
-    74         292 PRECALL                  0
+    83         292 PRECALL                  0
                296 CALL                     0
    
-    75         306 STORE_NAME              15 (_simulate)
+    84         306 STORE_NAME              15 (_simulate)
    
-   112         308 LOAD_NAME                3 (njit)
+   121         308 LOAD_NAME                3 (njit)
    
-   113         310 LOAD_CONST              23 ('props')
+   122         310 LOAD_CONST              23 ('props')
    
-   114         312 LOAD_NAME                1 (np)
+   123         312 LOAD_NAME                1 (np)
                314 LOAD_ATTR                9 (ndarray)
    
-   113         324 LOAD_CONST              18 ('r')
+   122         324 LOAD_CONST              18 ('r')
    
-   115         326 LOAD_NAME                1 (np)
+   124         326 LOAD_NAME                1 (np)
                328 LOAD_ATTR                9 (ndarray)
    
-   113         338 LOAD_CONST              19 ('r_tilde')
+   122         338 LOAD_CONST              19 ('r_tilde')
    
-   116         340 LOAD_NAME                1 (np)
+   125         340 LOAD_NAME                1 (np)
                342 LOAD_ATTR                9 (ndarray)
    
-   113         352 LOAD_CONST              24 ('c')
+   122         352 LOAD_CONST              24 ('c')
    
-   117         354 LOAD_NAME                1 (np)
+   126         354 LOAD_NAME                1 (np)
                356 LOAD_ATTR                9 (ndarray)
    
-   113         366 LOAD_CONST              17 ('num_agents')
+   122         366 LOAD_CONST              17 ('num_agents')
    
-   118         368 LOAD_NAME               11 (int)
+   127         368 LOAD_NAME               11 (int)
    
-   113         370 BUILD_TUPLE             10
-               372 LOAD_CONST              25 (<code object _update_propensities, file "C:\Users\Marvin\PycharmProjects\SPoNet\sponet\cnvm\approximations\stochastic_approximation.py", line 112>)
+   122         370 BUILD_TUPLE             10
+               372 LOAD_CONST              25 (<code object _update_propensities, file "C:\Users\Marvin\PycharmProjects\SPoNet\sponet\cnvm\approximations\stochastic_approximation.py", line 121>)
                374 MAKE_FUNCTION            4 (annotations)
    
-   112         376 PRECALL                  0
+   121         376 PRECALL                  0
                380 CALL                     0
    
-   113         390 STORE_NAME              16 (_update_propensities)
+   122         390 STORE_NAME              16 (_update_propensities)
    
-   128         392 LOAD_NAME                3 (njit)
+   137         392 LOAD_NAME                3 (njit)
    
-   129         394 LOAD_CONST              26 (<code object make_2d, file "C:\Users\Marvin\PycharmProjects\SPoNet\sponet\cnvm\approximations\stochastic_approximation.py", line 128>)
+   138         394 LOAD_CONST              26 (<code object make_2d, file "C:\Users\Marvin\PycharmProjects\SPoNet\sponet\cnvm\approximations\stochastic_approximation.py", line 137>)
                396 MAKE_FUNCTION            0
    
-   128         398 PRECALL                  0
+   137         398 PRECALL                  0
                402 CALL                     0
    
-   129         412 STORE_NAME              17 (make_2d)
+   138         412 STORE_NAME              17 (make_2d)
                414 LOAD_CONST               1 (None)
                416 RETURN_VALUE
    consts
       0
       None
       ('njit', 'prange')
       2
@@ -239,46 +239,46 @@
          flags     : 3
          code
             0x97007401000000000000000000007c017c027c006a0100000000000000
             007c006a0200000000000000007c006a0300000000000000007c037c04a6
             070000ab0700000000000000005300
            8           0 RESUME                   0
          
-          31           2 LOAD_GLOBAL              1 (NULL + _sample_many)
+          40           2 LOAD_GLOBAL              1 (NULL + _sample_many)
          
-          32          14 LOAD_FAST                1 (initial_state)
+          41          14 LOAD_FAST                1 (initial_state)
          
-          33          16 LOAD_FAST                2 (max_time)
+          42          16 LOAD_FAST                2 (max_time)
          
-          34          18 LOAD_FAST                0 (params)
+          43          18 LOAD_FAST                0 (params)
                       20 LOAD_ATTR                1 (num_agents)
          
-          35          30 LOAD_FAST                0 (params)
+          44          30 LOAD_FAST                0 (params)
                       32 LOAD_ATTR                2 (r)
          
-          36          42 LOAD_FAST                0 (params)
+          45          42 LOAD_FAST                0 (params)
                       44 LOAD_ATTR                3 (r_tilde)
          
-          37          54 LOAD_FAST                3 (num_timesteps)
+          46          54 LOAD_FAST                3 (num_timesteps)
          
-          38          56 LOAD_FAST                4 (num_samples)
+          47          56 LOAD_FAST                4 (num_samples)
          
-          31          58 PRECALL                  7
+          40          58 PRECALL                  7
                       62 CALL                     7
                       72 RETURN_VALUE
          consts
-            '\n\n    Parameters\n    ----------\n    params : CNVMParameters\n    initial_state : np.ndarray\n        Initial shares c.\n    max_time : float\n    num_timesteps : int\n        Number of states to return, at equidistant times.\n    num_samples: int\n\n    Returns\n    -------\n    tuple[np.ndarray, np.ndarray]\n    '
+            '\n    Simulate the opinion shares directly.\n\n    Assumes well-mixedness in the sense that the propensity of\n    reaction m -> n is given by\n    c[m] * (r[m, n] * c[n] + r_tilde[m, n]).\n\n    This is only true for complete networks.\n    For other networks the quality of this approximation may vary.\n\n    Parameters\n    ----------\n    params : CNVMParameters\n    initial_state : np.ndarray\n        Initial shares c of shape (num_opinions,).\n    max_time : float\n    num_timesteps : int\n        Number of states in returned trajectory, at equidistant times.\n    num_samples: int\n\n    Returns\n    -------\n    tuple[np.ndarray, np.ndarray]\n        t with shape (num_timesteps,), c with shape (num_timesteps, num_opinions)\n    '
          names      ('_sample_many', 'num_agents', 'r', 'r_tilde')
          varnames   ('params', 'initial_state', 'max_time', 'num_timesteps', 'num_samples')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\Marvin\\PycharmProjects\\SPoNet\\sponet\\cnvm\\approximations\\stochastic_approximation.py'
          name       'sample_stochastic_approximation'
          firstlineno 8
-         lnotab 0x02170c01020102010c010c010c01020102f9
+         lnotab 0x02200c01020102010c010c010c01020102f9
       True
       ('parallel',)
       't_max'
       'num_agents'
       'r'
       'r_tilde'
       code
@@ -296,35 +296,35 @@
             0000000000000044005d5b7d0a740b000000000000000000007c007c017c
             077c027c037c04a6060000ab0600000000000000005c0200007d0b7d0c74
             01000000000000000000006a0600000000000000007c0ba6010000ab0100
             000000000000007d0b740f000000000000000000007c0ca6010000ab0100
             000000000000007d0c7411000000000000000000007c087c0ba6020000ab
             0200000000000000007d0d7c0c7c0d640064008502660219000000000000
             0000007c097c0a3c0000008c5c7c087c0966025300
-          42           0 RESUME                   0
+          51           0 RESUME                   0
          
-          52           2 LOAD_FAST                1 (t_max)
+          61           2 LOAD_FAST                1 (t_max)
                        4 LOAD_CONST               1 (5)
                        6 LOAD_FAST                5 (num_timesteps)
                        8 BINARY_OP                5 (*)
                       12 BINARY_OP               11 (/)
                       16 STORE_FAST               7 (t_delta)
          
-          53          18 LOAD_GLOBAL              1 (NULL + np)
+          62          18 LOAD_GLOBAL              1 (NULL + np)
                       30 LOAD_ATTR                1 (linspace)
                       40 LOAD_CONST               2 (0)
                       42 LOAD_FAST                1 (t_max)
                       44 LOAD_FAST                5 (num_timesteps)
                       46 LOAD_CONST               3 (1)
                       48 BINARY_OP                0 (+)
                       52 PRECALL                  3
                       56 CALL                     3
                       66 STORE_FAST               8 (t_out)
          
-          54          68 LOAD_GLOBAL              1 (NULL + np)
+          63          68 LOAD_GLOBAL              1 (NULL + np)
                       80 LOAD_ATTR                2 (zeros)
                       90 LOAD_FAST                6 (num_samples)
                       92 LOAD_FAST                8 (t_out)
                       94 LOAD_ATTR                3 (shape)
                      104 LOAD_CONST               2 (0)
                      106 BINARY_SUBSCR
                      116 LOAD_FAST                0 (initial_state)
@@ -332,90 +332,90 @@
                      128 LOAD_CONST               2 (0)
                      130 BINARY_SUBSCR
                      140 BUILD_TUPLE              3
                      142 PRECALL                  1
                      146 CALL                     1
                      156 STORE_FAST               9 (c_out)
          
-          56         158 LOAD_GLOBAL              9 (NULL + prange)
+          65         158 LOAD_GLOBAL              9 (NULL + prange)
                      170 LOAD_FAST                6 (num_samples)
                      172 PRECALL                  1
                      176 CALL                     1
                      186 GET_ITER
                  >>  188 FOR_ITER                91 (to 372)
                      190 STORE_FAST              10 (i)
          
-          57         192 LOAD_GLOBAL             11 (NULL + _simulate)
+          66         192 LOAD_GLOBAL             11 (NULL + _simulate)
          
-          58         204 LOAD_FAST                0 (initial_state)
+          67         204 LOAD_FAST                0 (initial_state)
          
-          59         206 LOAD_FAST                1 (t_max)
+          68         206 LOAD_FAST                1 (t_max)
          
-          60         208 LOAD_FAST                7 (t_delta)
+          69         208 LOAD_FAST                7 (t_delta)
          
-          61         210 LOAD_FAST                2 (num_agents)
+          70         210 LOAD_FAST                2 (num_agents)
          
-          62         212 LOAD_FAST                3 (r)
+          71         212 LOAD_FAST                3 (r)
          
-          63         214 LOAD_FAST                4 (r_tilde)
+          72         214 LOAD_FAST                4 (r_tilde)
          
-          57         216 PRECALL                  6
+          66         216 PRECALL                  6
                      220 CALL                     6
                      230 UNPACK_SEQUENCE          2
                      234 STORE_FAST              11 (t)
                      236 STORE_FAST              12 (c)
          
-          65         238 LOAD_GLOBAL              1 (NULL + np)
+          74         238 LOAD_GLOBAL              1 (NULL + np)
                      250 LOAD_ATTR                6 (array)
                      260 LOAD_FAST               11 (t)
                      262 PRECALL                  1
                      266 CALL                     1
                      276 STORE_FAST              11 (t)
          
-          66         278 LOAD_GLOBAL             15 (NULL + make_2d)
+          75         278 LOAD_GLOBAL             15 (NULL + make_2d)
                      290 LOAD_FAST               12 (c)
                      292 PRECALL                  1
                      296 CALL                     1
                      306 STORE_FAST              12 (c)
          
-          68         308 LOAD_GLOBAL             17 (NULL + argmatch)
+          77         308 LOAD_GLOBAL             17 (NULL + argmatch)
                      320 LOAD_FAST                8 (t_out)
                      322 LOAD_FAST               11 (t)
                      324 PRECALL                  2
                      328 CALL                     2
                      338 STORE_FAST              13 (t_ind)
          
-          69         340 LOAD_FAST               12 (c)
+          78         340 LOAD_FAST               12 (c)
                      342 LOAD_FAST               13 (t_ind)
                      344 LOAD_CONST               0 (None)
                      346 LOAD_CONST               0 (None)
                      348 BUILD_SLICE              2
                      350 BUILD_TUPLE              2
                      352 BINARY_SUBSCR
                      362 LOAD_FAST                9 (c_out)
                      364 LOAD_FAST               10 (i)
                      366 STORE_SUBSCR
                      370 JUMP_BACKWARD           92 (to 188)
          
-          71     >>  372 LOAD_FAST                8 (t_out)
+          80     >>  372 LOAD_FAST                8 (t_out)
                      374 LOAD_FAST                9 (c_out)
                      376 BUILD_TUPLE              2
                      378 RETURN_VALUE
          consts
             None
             5
             0
             1
          names      ('np', 'linspace', 'zeros', 'shape', 'prange', '_simulate', 'array', 'make_2d', 'argmatch')
          varnames   ('initial_state', 't_max', 'num_agents', 'r', 'r_tilde', 'num_timesteps', 'num_samples', 't_delta', 't_out', 'c_out', 'i', 't', 'c', 't_ind')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\Marvin\\PycharmProjects\\SPoNet\\sponet\\cnvm\\approximations\\stochastic_approximation.py'
          name       '_sample_many'
-         firstlineno 42
+         firstlineno 51
          lnotab
             0x020a100132015a0222010c010201020102010201020102fa160828011e
             0220012002
       't_delta'
       code
          argcount  : 6
          nlocals   : 18
@@ -443,181 +443,181 @@
             007c077c11780278021900000000000000000064027c037a0b00007a0d00
             00630363023c0000007c067c0c6b050000000072417c0c7c027a0d00007d
             0c7c09a00a00000000000000000000000000000000000000007c06a60100
             00ab01000000000000000001007c0aa00a00000000000000000000000000
             000000000000007c07a00000000000000000000000000000000000000000
             00a6000000ab000000000000000000a6010000ab01000000000000000001
             007c067c016b00000000009001b0147c097c0a66025300
-          74           0 RESUME                   0
+          83           0 RESUME                   0
          
-          83           2 LOAD_CONST               1 (0)
+          92           2 LOAD_CONST               1 (0)
                        4 STORE_FAST               6 (t)
          
-          84           6 LOAD_FAST                0 (initial_state)
+          93           6 LOAD_FAST                0 (initial_state)
                        8 LOAD_METHOD              0 (copy)
                       30 PRECALL                  0
                       34 CALL                     0
                       44 STORE_FAST               7 (c)
          
-          85          46 LOAD_FAST                7 (c)
+          94          46 LOAD_FAST                7 (c)
                       48 LOAD_ATTR                1 (shape)
                       58 LOAD_CONST               1 (0)
                       60 BINARY_SUBSCR
                       70 STORE_FAST               8 (num_opinions)
          
-          87          72 LOAD_CONST               1 (0)
+          96          72 LOAD_CONST               1 (0)
                       74 BUILD_LIST               1
                       76 STORE_FAST               9 (t_list)
          
-          88          78 LOAD_FAST                0 (initial_state)
+          97          78 LOAD_FAST                0 (initial_state)
                       80 LOAD_METHOD              0 (copy)
                      102 PRECALL                  0
                      106 CALL                     0
                      116 BUILD_LIST               1
                      118 STORE_FAST              10 (c_list)
          
-          89         120 LOAD_GLOBAL              5 (NULL + np)
+          98         120 LOAD_GLOBAL              5 (NULL + np)
                      132 LOAD_ATTR                3 (zeros)
                      142 LOAD_FAST                8 (num_opinions)
                      144 LOAD_FAST                8 (num_opinions)
                      146 BUILD_TUPLE              2
                      148 PRECALL                  1
                      152 CALL                     1
                      162 STORE_FAST              11 (props)
          
-          91         164 LOAD_FAST                2 (t_delta)
+         100         164 LOAD_FAST                2 (t_delta)
                      166 STORE_FAST              12 (t_store)
          
-          92         168 LOAD_FAST                6 (t)
+         101         168 LOAD_FAST                6 (t)
                      170 LOAD_FAST                1 (t_max)
                      172 COMPARE_OP               0 (<)
                      178 EXTENDED_ARG             1
                      180 POP_JUMP_FORWARD_IF_FALSE   276 (to 734)
          
-          93     >>  182 LOAD_GLOBAL              9 (NULL + _update_propensities)
+         102     >>  182 LOAD_GLOBAL              9 (NULL + _update_propensities)
                      194 LOAD_FAST               11 (props)
                      196 LOAD_FAST                4 (r)
                      198 LOAD_FAST                5 (r_tilde)
                      200 LOAD_FAST                7 (c)
                      202 LOAD_FAST                3 (num_agents)
                      204 PRECALL                  5
                      208 CALL                     5
                      218 POP_TOP
          
-          95         220 LOAD_GLOBAL              5 (NULL + np)
+         104         220 LOAD_GLOBAL              5 (NULL + np)
                      232 LOAD_ATTR                5 (sum)
                      242 LOAD_FAST               11 (props)
                      244 PRECALL                  1
                      248 CALL                     1
                      258 STORE_FAST              13 (sum_props)
          
-          96         260 LOAD_FAST                6 (t)
+         105         260 LOAD_FAST                6 (t)
                      262 LOAD_GLOBAL              4 (np)
                      274 LOAD_ATTR                6 (random)
                      284 LOAD_METHOD              7 (exponential)
                      306 LOAD_CONST               2 (1)
                      308 LOAD_FAST               13 (sum_props)
                      310 BINARY_OP               11 (/)
                      314 PRECALL                  1
                      318 CALL                     1
                      328 BINARY_OP               13 (+=)
                      332 STORE_FAST               6 (t)
          
-          98         334 LOAD_GLOBAL              5 (NULL + np)
+         107         334 LOAD_GLOBAL              5 (NULL + np)
                      346 LOAD_ATTR                8 (cumsum)
                      356 LOAD_FAST               11 (props)
                      358 LOAD_FAST               13 (sum_props)
                      360 BINARY_OP               11 (/)
                      364 PRECALL                  1
                      368 CALL                     1
                      378 STORE_FAST              14 (cum_sum)
          
-          99         380 LOAD_GLOBAL              5 (NULL + np)
+         108         380 LOAD_GLOBAL              5 (NULL + np)
                      392 LOAD_ATTR                9 (searchsorted)
                      402 LOAD_FAST               14 (cum_sum)
                      404 LOAD_GLOBAL              4 (np)
                      416 LOAD_ATTR                6 (random)
                      426 LOAD_METHOD              6 (random)
                      448 PRECALL                  0
                      452 CALL                     0
                      462 LOAD_CONST               3 ('right')
                      464 KW_NAMES                 4
                      466 PRECALL                  3
                      470 CALL                     3
                      480 STORE_FAST              15 (reaction)
          
-         100         482 LOAD_FAST               15 (reaction)
+         109         482 LOAD_FAST               15 (reaction)
                      484 LOAD_FAST                8 (num_opinions)
                      486 BINARY_OP                2 (//)
                      490 LOAD_FAST               15 (reaction)
                      492 LOAD_FAST                8 (num_opinions)
                      494 BINARY_OP                6 (%)
                      498 STORE_FAST              17 (n)
                      500 STORE_FAST              16 (m)
          
-         101         502 LOAD_FAST                7 (c)
+         110         502 LOAD_FAST                7 (c)
                      504 LOAD_FAST               16 (m)
                      506 COPY                     2
                      508 COPY                     2
                      510 BINARY_SUBSCR
                      520 LOAD_CONST               2 (1)
                      522 LOAD_FAST                3 (num_agents)
                      524 BINARY_OP               11 (/)
                      528 BINARY_OP               23 (-=)
                      532 SWAP                     3
                      534 SWAP                     2
                      536 STORE_SUBSCR
          
-         102         540 LOAD_FAST                7 (c)
+         111         540 LOAD_FAST                7 (c)
                      542 LOAD_FAST               17 (n)
                      544 COPY                     2
                      546 COPY                     2
                      548 BINARY_SUBSCR
                      558 LOAD_CONST               2 (1)
                      560 LOAD_FAST                3 (num_agents)
                      562 BINARY_OP               11 (/)
                      566 BINARY_OP               13 (+=)
                      570 SWAP                     3
                      572 SWAP                     2
                      574 STORE_SUBSCR
          
-         104         578 LOAD_FAST                6 (t)
+         113         578 LOAD_FAST                6 (t)
                      580 LOAD_FAST               12 (t_store)
                      582 COMPARE_OP               5 (>=)
                      588 POP_JUMP_FORWARD_IF_FALSE    65 (to 720)
          
-         105         590 LOAD_FAST               12 (t_store)
+         114         590 LOAD_FAST               12 (t_store)
                      592 LOAD_FAST                2 (t_delta)
                      594 BINARY_OP               13 (+=)
                      598 STORE_FAST              12 (t_store)
          
-         106         600 LOAD_FAST                9 (t_list)
+         115         600 LOAD_FAST                9 (t_list)
                      602 LOAD_METHOD             10 (append)
                      624 LOAD_FAST                6 (t)
                      626 PRECALL                  1
                      630 CALL                     1
                      640 POP_TOP
          
-         107         642 LOAD_FAST               10 (c_list)
+         116         642 LOAD_FAST               10 (c_list)
                      644 LOAD_METHOD             10 (append)
                      666 LOAD_FAST                7 (c)
                      668 LOAD_METHOD              0 (copy)
                      690 PRECALL                  0
                      694 CALL                     0
                      704 PRECALL                  1
                      708 CALL                     1
                      718 POP_TOP
          
-          92     >>  720 LOAD_FAST                6 (t)
+         101     >>  720 LOAD_FAST                6 (t)
                      722 LOAD_FAST                1 (t_max)
                      724 COMPARE_OP               0 (<)
                      730 EXTENDED_ARG             1
                      732 POP_JUMP_BACKWARD_IF_TRUE   276 (to 182)
          
-         109     >>  734 LOAD_FAST                9 (t_list)
+         118     >>  734 LOAD_FAST                9 (t_list)
                      736 LOAD_FAST               10 (c_list)
                      738 BUILD_TUPLE              2
                      740 RETURN_VALUE
          consts
             None
             0
             1
@@ -625,15 +625,15 @@
             ('side',)
          names      ('copy', 'shape', 'np', 'zeros', '_update_propensities', 'sum', 'random', 'exponential', 'cumsum', 'searchsorted', 'append')
          varnames   ('initial_state', 't_max', 't_delta', 'num_agents', 'r', 'r_tilde', 't', 'c', 'num_opinions', 't_list', 'c_list', 'props', 't_store', 'sum_props', 'cum_sum', 'reaction', 'm', 'n')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\Marvin\\PycharmProjects\\SPoNet\\sponet\\cnvm\\approximations\\stochastic_approximation.py'
          name       '_simulate'
-         firstlineno 74
+         firstlineno 83
          lnotab
             0x0209040128011a0206012a012c0204010e01260228014a022e01660114
             01260126020c010a012a014ef10e11
       'props'
       'c'
       code
          argcount  : 5
@@ -645,46 +645,46 @@
             000000000000000000a6010000ab01000000000000000044005d527d0574
             01000000000000000000007c006a01000000000000000064021900000000
             0000000000a6010000ab01000000000000000044005d357d067c057c066b
             020000000072018c097c037c05190000000000000000007c017c057c0666
             02190000000000000000007c037c06190000000000000000007a0500007c
             027c057c066602190000000000000000007a0000007a0500007c007c057c
             0666023c0000008c368c537c007c047a1200007d0064005300
-         112           0 RESUME                   0
+         121           0 RESUME                   0
          
-         120           2 LOAD_GLOBAL              1 (NULL + range)
+         129           2 LOAD_GLOBAL              1 (NULL + range)
                       14 LOAD_FAST                0 (props)
                       16 LOAD_ATTR                1 (shape)
                       26 LOAD_CONST               1 (0)
                       28 BINARY_SUBSCR
                       38 PRECALL                  1
                       42 CALL                     1
                       52 GET_ITER
                  >>   54 FOR_ITER                82 (to 220)
                       56 STORE_FAST               5 (m)
          
-         121          58 LOAD_GLOBAL              1 (NULL + range)
+         130          58 LOAD_GLOBAL              1 (NULL + range)
                       70 LOAD_FAST                0 (props)
                       72 LOAD_ATTR                1 (shape)
                       82 LOAD_CONST               2 (1)
                       84 BINARY_SUBSCR
                       94 PRECALL                  1
                       98 CALL                     1
                      108 GET_ITER
                  >>  110 FOR_ITER                53 (to 218)
                      112 STORE_FAST               6 (n)
          
-         122         114 LOAD_FAST                5 (m)
+         131         114 LOAD_FAST                5 (m)
                      116 LOAD_FAST                6 (n)
                      118 COMPARE_OP               2 (==)
                      124 POP_JUMP_FORWARD_IF_FALSE     1 (to 128)
          
-         123         126 JUMP_BACKWARD            9 (to 110)
+         132         126 JUMP_BACKWARD            9 (to 110)
          
-         124     >>  128 LOAD_FAST                3 (c)
+         133     >>  128 LOAD_FAST                3 (c)
                      130 LOAD_FAST                5 (m)
                      132 BINARY_SUBSCR
                      142 LOAD_FAST                1 (r)
                      144 LOAD_FAST                5 (m)
                      146 LOAD_FAST                6 (n)
                      148 BUILD_TUPLE              2
                      150 BINARY_SUBSCR
@@ -702,17 +702,17 @@
                      204 LOAD_FAST                0 (props)
                      206 LOAD_FAST                5 (m)
                      208 LOAD_FAST                6 (n)
                      210 BUILD_TUPLE              2
                      212 STORE_SUBSCR
                      216 JUMP_BACKWARD           54 (to 110)
          
-         121     >>  218 JUMP_BACKWARD           83 (to 54)
+         130     >>  218 JUMP_BACKWARD           83 (to 54)
          
-         125     >>  220 LOAD_FAST                0 (props)
+         134     >>  220 LOAD_FAST                0 (props)
                      222 LOAD_FAST                4 (num_agents)
                      224 BINARY_OP               18 (*=)
                      228 STORE_FAST               0 (props)
                      230 LOAD_CONST               0 (None)
                      232 RETURN_VALUE
          consts
             None
@@ -720,88 +720,88 @@
             1
          names      ('range', 'shape')
          varnames   ('props', 'r', 'r_tilde', 'c', 'num_agents', 'm', 'n')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\Marvin\\PycharmProjects\\SPoNet\\sponet\\cnvm\\approximations\\stochastic_approximation.py'
          name       '_update_propensities'
-         firstlineno 112
+         firstlineno 121
          lnotab 0x0208380138010c0102015afd0204
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             007d017c006401190000000000000000006a010000000000000000640119
             0000000000000000007d027405000000000000000000006a030000000000
             0000007c017c026602a6010000ab0100000000000000007d037409000000
             000000000000007c01a6010000ab01000000000000000044005d0d7d047c
             007c04190000000000000000007c037c043c0000008c0e7c035300
-         128           0 RESUME                   0
+         137           0 RESUME                   0
          
-         130           2 LOAD_GLOBAL              1 (NULL + len)
+         139           2 LOAD_GLOBAL              1 (NULL + len)
                       14 LOAD_FAST                0 (arraylist)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               1 (n)
          
-         131          32 LOAD_FAST                0 (arraylist)
+         140          32 LOAD_FAST                0 (arraylist)
                       34 LOAD_CONST               1 (0)
                       36 BINARY_SUBSCR
                       46 LOAD_ATTR                1 (shape)
                       56 LOAD_CONST               1 (0)
                       58 BINARY_SUBSCR
                       68 STORE_FAST               2 (k)
          
-         132          70 LOAD_GLOBAL              5 (NULL + np)
+         141          70 LOAD_GLOBAL              5 (NULL + np)
                       82 LOAD_ATTR                3 (zeros)
                       92 LOAD_FAST                1 (n)
                       94 LOAD_FAST                2 (k)
                       96 BUILD_TUPLE              2
                       98 PRECALL                  1
                      102 CALL                     1
                      112 STORE_FAST               3 (a2d)
          
-         133         114 LOAD_GLOBAL              9 (NULL + range)
+         142         114 LOAD_GLOBAL              9 (NULL + range)
                      126 LOAD_FAST                1 (n)
                      128 PRECALL                  1
                      132 CALL                     1
                      142 GET_ITER
                  >>  144 FOR_ITER                13 (to 172)
                      146 STORE_FAST               4 (i)
          
-         134         148 LOAD_FAST                0 (arraylist)
+         143         148 LOAD_FAST                0 (arraylist)
                      150 LOAD_FAST                4 (i)
                      152 BINARY_SUBSCR
                      162 LOAD_FAST                3 (a2d)
                      164 LOAD_FAST                4 (i)
                      166 STORE_SUBSCR
                      170 JUMP_BACKWARD           14 (to 144)
          
-         135     >>  172 LOAD_FAST                3 (a2d)
+         144     >>  172 LOAD_FAST                3 (a2d)
                      174 RETURN_VALUE
          consts
             None
             0
          names      ('len', 'shape', 'np', 'zeros', 'range')
          varnames   ('arraylist', 'n', 'k', 'a2d', 'i')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\Marvin\\PycharmProjects\\SPoNet\\sponet\\cnvm\\approximations\\stochastic_approximation.py'
          name       'make_2d'
-         firstlineno 128
+         firstlineno 137
          lnotab 0x02021e0126012c0122011801
    names      ('numpy', 'np', 'numba', 'njit', 'prange', 'parameters', 'CNVMParameters', 'utils', 'argmatch', 'ndarray', 'float', 'int', 'tuple', 'sample_stochastic_approximation', '_sample_many', '_simulate', '_update_propensities', 'make_2d')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\Marvin\\PycharmProjects\\SPoNet\\sponet\\cnvm\\approximations\\stochastic_approximation.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080110020c010c03020102ff02020cfe020302fd020402fc02
-      0502fb020626fa0822160102010cff020202fe020302fd02040cfc02050c
+      0502fb020626fa082b160102010cff020202fe020302fd02040cfc02050c
       fb020602fa020702f906ff0e01021f020102010cff020202fe020302fd02
       0402fc02050cfb02060cfa06ff0e010225020102010cff02020cfe02030c
       fd02040cfc020502fb06ff0e01020f020104ff0e01
```

### Comparing `sponet-2.0.0/sponet/cnvm/approximations/chemical_langevin_equation.py` & `sponet-2.1.0/sponet/cnvm/approximations/chemical_langevin_equation.py`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/cnvm/approximations/reaction_rate_equation.py` & `sponet-2.1.0/sponet/cnvm/approximations/reaction_rate_equation.py`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/cnvm/approximations/stochastic_approximation.py` & `sponet-2.1.0/sponet/cnvm/approximations/stochastic_approximation.py`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/cnvm/model.py` & `sponet-2.1.0/sponet/cnvm/model.py`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/cnvm/parameters.py` & `sponet-2.1.0/sponet/cnvm/parameters.py`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/collective_variables.py` & `sponet-2.1.0/sponet/collective_variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,17 +143,17 @@
         for i, deg in enumerate(self.degrees):
             weights = np.zeros(num_agents)
             weights[np.nonzero(self.degrees_of_nodes == deg)] = 1
             x_agg = _opinion_shares_numba(x_traj_int, self.num_opinions, weights)
             x_agg = x_agg[:, self.idx_to_return]
             if self.normalize:
                 x_agg /= np.sum(weights)
-            cv[
-                :, i * len(self.idx_to_return) : (i + 1) * len(self.idx_to_return)
-            ] = np.copy(x_agg)
+            cv[:, i * len(self.idx_to_return) : (i + 1) * len(self.idx_to_return)] = (
+                np.copy(x_agg)
+            )
 
         return cv
 
 
 class CompositeCollectiveVariable:
     def __init__(self, collective_variables: list[CollectiveVariable]):
         """
```

### Comparing `sponet-2.0.0/sponet/multiprocessing.py` & `sponet-2.1.0/sponet/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/network_generator.py` & `sponet-2.1.0/sponet/network_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 class ErdosRenyiGenerator:
     def __init__(
         self,
         num_agents: int,
         p: float,
         max_sample_time: float = 10,
         rng: Generator = default_rng(),
+        force_no_isolates: bool = False,
     ):
         """
         Generate Erdös-Renyi (binomial) random graphs.
 
         The random graph may contain isolated vertices, which is not allowed.
         In that case, the Generator samples until a valid network is found,
         or until max_sample_time seconds pass, in which case a RuntimeError is raised.
@@ -37,28 +38,36 @@
         ----------
         num_agents : int
         p : float
         max_sample_time : float, optional
             In seconds.
         rng : Generator, optional
             random number generator
+        force_no_isolates : bool, optional
+            If set to true, one random edge will be added to each isolated vertex,
+            resulting in a network without isolates.
         """
         self.num_agents = num_agents
         self.p = p
         self.max_sample_time = max_sample_time
         self.rng = rng
+        self.force_no_isolates = force_no_isolates
 
     def __call__(self) -> nx.Graph:
         gnp_fun = nx.erdos_renyi_graph if self.p > 0.2 else nx.fast_gnp_random_graph
         start = time.time()
         while True:
             network = gnp_fun(self.num_agents, self.p, seed=self.rng)
             if nx.number_of_isolates(network) == 0:
                 return network
 
+            if self.force_no_isolates:
+                _unisolate_vertices(network)
+                return network
+
             if time.time() - start > self.max_sample_time:
                 raise RuntimeError(
                     "Timeout. Could not generate a graph without isolated vertices."
                 )
 
     def __repr__(self) -> str:
         return f"Erdos-Renyi random graph with p={self.p} on {self.num_agents} nodes"
@@ -399,7 +408,23 @@
         return g
 
     def __repr__(self) -> str:
         return f"Bianconi-Barabasi random graph on {self.num_agents} nodes"
 
     def abrv(self):
         return f"bianconi_barabasi_m{self.m}_N{self.num_agents}"
+
+
+def _unisolate_vertices(network: nx.Graph) -> None:
+    """
+    Make isolated vertices un-isolated by adding one edge to a random node.
+
+    Parameters
+    ----------
+    network : nx.Graph
+    """
+    for i in nx.isolates(network):
+        j = i
+        while j == i:
+            j = np.random.randint(0, network.number_of_nodes())
+
+        network.add_edge(i, j)
```

### Comparing `sponet-2.0.0/sponet/parameters.py` & `sponet-2.1.0/sponet/parameters.py`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/plotting.py` & `sponet-2.1.0/sponet/plotting.py`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/sponet/sampling.py` & `sponet-2.1.0/sponet/sampling.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,16 +50,18 @@
     while small_ids and large_ids:
         small_id = small_ids.pop()
         large_id = large_ids.pop()
 
         table_alias[small_id] = large_id
         table_prob[large_id] = table_prob[large_id] + table_prob[small_id] - 1
 
-        small_ids.append(large_id) if table_prob[large_id] < 1 else large_ids.append(
-            large_id
+        (
+            small_ids.append(large_id)
+            if table_prob[large_id] < 1
+            else large_ids.append(large_id)
         )
 
     while large_ids:
         table_prob[large_ids.pop()] = 1
 
     while small_ids:
         table_prob[small_ids.pop()] = 1
```

### Comparing `sponet-2.0.0/sponet/utils.py` & `sponet-2.1.0/sponet/utils.py`

 * *Files identical despite different names*

### Comparing `sponet-2.0.0/PKG-INFO` & `sponet-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sponet
-Version: 2.0.0
+Version: 2.1.0
 Summary: Spreading Processes on Networks
 Home-page: https://github.com/lueckem/SPoNet
 License: GPL-3.0-or-later
 Keywords: voter model,threshold model,social dynamics,opinion dynamics,statistical physics,agent-based model,epidemiology,interacting particle system
 Author: Marvin Lücke
 Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Science/Research
@@ -21,15 +21,15 @@
 Requires-Dist: numpy (>=1.21)
 Requires-Dist: scipy (>=1.9.3)
 Project-URL: Repository, https://github.com/lueckem/SPoNet
 Description-Content-Type: text/markdown
 
 # Spreading Processes on Networks (SPoNet)
 
-[![build](https://github.com/lueckem/cnvm/actions/workflows/build.yml/badge.svg)](https://github.com/lueckem/cnvm/actions/workflows/build.yml)
+[![build](https://github.com/lueckem/SPoNet/actions/workflows/build.yml/badge.svg)](https://github.com/lueckem/SPoNet/actions/workflows/build.yml)
 
 This package provides an efficient implementation of popular discrete-state spreading processes on networks of interacting *agents*.
 They can be used to simulate how opinions about certain issues develop over time within a population, or how an infectious disease spreads.
 The simulation loop is just-in-time compiled using `numba`, which makes performance comparable with compiled languages like C++.
 
 Available models:
 - continuous-time noisy voter model (CNVM)
```

