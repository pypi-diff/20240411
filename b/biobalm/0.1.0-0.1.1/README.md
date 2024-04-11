# Comparing `tmp/biobalm-0.1.0.tar.gz` & `tmp/biobalm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobalm-0.1.0.tar", last modified: Wed Apr 10 19:22:18 2024, max compression
+gzip compressed data, was "biobalm-0.1.1.tar", last modified: Thu Apr 11 16:06:15 2024, max compression
```

## Comparing `biobalm-0.1.0.tar` & `biobalm-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:22:18.337083 biobalm-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-10 19:22:14.000000 biobalm-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-10 19:22:18.337083 biobalm-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-10 19:22:14.000000 biobalm-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:22:18.333083 biobalm-0.1.0/biobalm/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:22:18.333083 biobalm-0.1.0/biobalm/_sd_algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/_sd_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/_sd_algorithms/compute_attractor_seeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/_sd_algorithms/expand_attractor_seeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/_sd_algorithms/expand_bfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/_sd_algorithms/expand_dfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/_sd_algorithms/expand_minimal_spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/_sd_algorithms/expand_source_SCCs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/_sd_algorithms/expand_to_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/control.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/interaction_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17167 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/motif_avoidant.py
--rw-r--r--   0 runner    (1001) docker     (127)    16211 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/petri_net_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    17225 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/space_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37095 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/succession_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/symbolic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19392 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/trappist_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-10 19:22:14.000000 biobalm-0.1.0/biobalm/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:22:18.333083 biobalm-0.1.0/biobalm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-10 19:22:18.000000 biobalm-0.1.0/biobalm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-10 19:22:18.000000 biobalm-0.1.0/biobalm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:22:18.000000 biobalm-0.1.0/biobalm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-10 19:22:18.000000 biobalm-0.1.0/biobalm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 19:22:18.000000 biobalm-0.1.0/biobalm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-10 19:22:14.000000 biobalm-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-10 19:22:18.337083 biobalm-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:06:15.880384 biobalm-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-11 16:06:07.000000 biobalm-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-11 16:06:15.880384 biobalm-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-11 16:06:07.000000 biobalm-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:06:15.880384 biobalm-0.1.1/biobalm/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:06:15.880384 biobalm-0.1.1/biobalm/_sd_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/compute_attractor_seeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/expand_attractor_seeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/expand_bfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/expand_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/expand_minimal_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/expand_source_SCCs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/expand_to_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/interaction_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17167 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/motif_avoidant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16211 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/petri_net_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17225 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/space_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37095 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/succession_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/symbolic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19392 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/trappist_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:06:15.880384 biobalm-0.1.1/biobalm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-11 16:06:15.000000 biobalm-0.1.1/biobalm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-11 16:06:15.000000 biobalm-0.1.1/biobalm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:06:15.000000 biobalm-0.1.1/biobalm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 16:06:15.000000 biobalm-0.1.1/biobalm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 16:06:15.000000 biobalm-0.1.1/biobalm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-11 16:06:07.000000 biobalm-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-11 16:06:15.880384 biobalm-0.1.1/setup.cfg
```

### Comparing `biobalm-0.1.0/LICENSE` & `biobalm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/PKG-INFO` & `biobalm-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobalm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Boolean Attractor Landscape Mapper
 Author-email: Jordan Rozum <jrozum@binghamton.edu>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: biodivine_aeon==1.0.0a4
 Requires-Dist: clingo>=5.6.2
```

### Comparing `biobalm-0.1.0/README.md` & `biobalm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/_sd_algorithms/__init__.py` & `biobalm-0.1.1/biobalm/_sd_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/_sd_algorithms/compute_attractor_seeds.py` & `biobalm-0.1.1/biobalm/_sd_algorithms/compute_attractor_seeds.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/_sd_algorithms/expand_attractor_seeds.py` & `biobalm-0.1.1/biobalm/_sd_algorithms/expand_attractor_seeds.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/_sd_algorithms/expand_bfs.py` & `biobalm-0.1.1/biobalm/_sd_algorithms/expand_bfs.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/_sd_algorithms/expand_dfs.py` & `biobalm-0.1.1/biobalm/_sd_algorithms/expand_dfs.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/_sd_algorithms/expand_minimal_spaces.py` & `biobalm-0.1.1/biobalm/_sd_algorithms/expand_minimal_spaces.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/_sd_algorithms/expand_source_SCCs.py` & `biobalm-0.1.1/biobalm/_sd_algorithms/expand_source_SCCs.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/_sd_algorithms/expand_to_target.py` & `biobalm-0.1.1/biobalm/_sd_algorithms/expand_to_target.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/control.py` & `biobalm-0.1.1/biobalm/control.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/drivers.py` & `biobalm-0.1.1/biobalm/drivers.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/interaction_graph_utils.py` & `biobalm-0.1.1/biobalm/interaction_graph_utils.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/motif_avoidant.py` & `biobalm-0.1.1/biobalm/motif_avoidant.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/petri_net_translation.py` & `biobalm-0.1.1/biobalm/petri_net_translation.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/space_utils.py` & `biobalm-0.1.1/biobalm/space_utils.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/succession_diagram.py` & `biobalm-0.1.1/biobalm/succession_diagram.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/symbolic_utils.py` & `biobalm-0.1.1/biobalm/symbolic_utils.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/trappist_core.py` & `biobalm-0.1.1/biobalm/trappist_core.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm/types.py` & `biobalm-0.1.1/biobalm/types.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/biobalm.egg-info/PKG-INFO` & `biobalm-0.1.1/biobalm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobalm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Boolean Attractor Landscape Mapper
 Author-email: Jordan Rozum <jrozum@binghamton.edu>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: biodivine_aeon==1.0.0a4
 Requires-Dist: clingo>=5.6.2
```

### Comparing `biobalm-0.1.0/biobalm.egg-info/SOURCES.txt` & `biobalm-0.1.1/biobalm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.0/pyproject.toml` & `biobalm-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 requires-python = ">=3.11"
 dependencies = [
     'biodivine_aeon ==1.0.0a4',
     'clingo >=5.6.2',
     'networkx>=2.8.8',
     'pypint>=1.6.2',
 ]
-version = "0.1.0"
+version = "0.1.1"
 
 
 [tool.setuptools]
 packages = ['biobalm', 'biobalm._sd_algorithms']
 
 
 [tool.pyright]
```

