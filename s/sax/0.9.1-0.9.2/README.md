# Comparing `tmp/sax-0.9.1.tar.gz` & `tmp/sax-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sax-0.9.1.tar", last modified: Sun Aug 20 19:13:52 2023, max compression
+gzip compressed data, was "sax-0.9.2.tar", last modified: Thu Aug 24 14:30:13 2023, max compression
```

## Comparing `sax-0.9.1.tar` & `sax-0.9.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-20 19:13:52.319024 sax-0.9.1/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-08-20 19:13:01.000000 sax-0.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      838 2023-08-20 19:13:52.315024 sax-0.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4864 2023-08-20 19:13:01.000000 sax-0.9.1/README.md
--rw-r--r--   0 root         (0) root         (0)     2011 2023-08-20 19:13:01.000000 sax-0.9.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-20 19:13:52.311025 sax-0.9.1/sax/
--rw-r--r--   0 root         (0) root         (0)     2939 2023-08-20 19:13:01.000000 sax-0.9.1/sax/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6699 2023-08-20 19:13:01.000000 sax-0.9.1/sax/_nbdev.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-20 19:13:52.315024 sax-0.9.1/sax/backends/
--rw-r--r--   0 root         (0) root         (0)      774 2023-08-20 19:13:01.000000 sax-0.9.1/sax/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-08-20 19:13:01.000000 sax-0.9.1/sax/backends/additive.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-08-20 19:13:01.000000 sax-0.9.1/sax/backends/default.py
--rw-r--r--   0 root         (0) root         (0)     3945 2023-08-20 19:13:01.000000 sax-0.9.1/sax/backends/klu.py
--rw-r--r--   0 root         (0) root         (0)    11955 2023-08-20 19:13:01.000000 sax-0.9.1/sax/circuit.py
--rw-r--r--   0 root         (0) root         (0)     8000 2023-08-20 19:13:01.000000 sax-0.9.1/sax/make_docs.py
--rw-r--r--   0 root         (0) root         (0)     8813 2023-08-20 19:13:01.000000 sax-0.9.1/sax/models.py
--rw-r--r--   0 root         (0) root         (0)     5770 2023-08-20 19:13:01.000000 sax-0.9.1/sax/multimode.py
--rw-r--r--   0 root         (0) root         (0)    10269 2023-08-20 19:13:01.000000 sax-0.9.1/sax/netlist.py
--rw-r--r--   0 root         (0) root         (0)     2751 2023-08-20 19:13:01.000000 sax-0.9.1/sax/netlist_cleaning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-20 19:13:52.315024 sax-0.9.1/sax/nn/
--rw-r--r--   0 root         (0) root         (0)      971 2023-08-20 19:13:01.000000 sax-0.9.1/sax/nn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2749 2023-08-20 19:13:01.000000 sax-0.9.1/sax/nn/core.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-08-20 19:13:01.000000 sax-0.9.1/sax/nn/io.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-08-20 19:13:01.000000 sax-0.9.1/sax/nn/loss.py
--rw-r--r--   0 root         (0) root         (0)     2000 2023-08-20 19:13:01.000000 sax-0.9.1/sax/nn/utils.py
--rw-r--r--   0 root         (0) root         (0)     1775 2023-08-20 19:13:01.000000 sax-0.9.1/sax/patched.py
--rw-r--r--   0 root         (0) root         (0)    10223 2023-08-20 19:13:01.000000 sax-0.9.1/sax/typing_.py
--rw-r--r--   0 root         (0) root         (0)    18468 2023-08-20 19:13:01.000000 sax-0.9.1/sax/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-20 19:13:52.311025 sax-0.9.1/sax.egg-info/
--rw-r--r--   0 root         (0) root         (0)      838 2023-08-20 19:13:52.000000 sax-0.9.1/sax.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      513 2023-08-20 19:13:52.000000 sax-0.9.1/sax.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-20 19:13:52.000000 sax-0.9.1/sax.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      520 2023-08-20 19:13:52.000000 sax-0.9.1/sax.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-08-20 19:13:52.000000 sax-0.9.1/sax.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-20 19:13:52.319024 sax-0.9.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-24 14:30:13.913032 sax-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-08-24 14:29:33.000000 sax-0.9.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      838 2023-08-24 14:30:13.913032 sax-0.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-08-24 14:29:33.000000 sax-0.9.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-08-24 14:29:33.000000 sax-0.9.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-24 14:30:13.909032 sax-0.9.2/sax/
+-rw-r--r--   0 root         (0) root         (0)     2939 2023-08-24 14:29:33.000000 sax-0.9.2/sax/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6699 2023-08-24 14:29:33.000000 sax-0.9.2/sax/_nbdev.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-24 14:30:13.913032 sax-0.9.2/sax/backends/
+-rw-r--r--   0 root         (0) root         (0)      774 2023-08-24 14:29:33.000000 sax-0.9.2/sax/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-08-24 14:29:33.000000 sax-0.9.2/sax/backends/additive.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-08-24 14:29:33.000000 sax-0.9.2/sax/backends/default.py
+-rw-r--r--   0 root         (0) root         (0)     3945 2023-08-24 14:29:33.000000 sax-0.9.2/sax/backends/klu.py
+-rw-r--r--   0 root         (0) root         (0)    12130 2023-08-24 14:29:33.000000 sax-0.9.2/sax/circuit.py
+-rw-r--r--   0 root         (0) root         (0)     8000 2023-08-24 14:29:33.000000 sax-0.9.2/sax/make_docs.py
+-rw-r--r--   0 root         (0) root         (0)     8813 2023-08-24 14:29:33.000000 sax-0.9.2/sax/models.py
+-rw-r--r--   0 root         (0) root         (0)     5770 2023-08-24 14:29:33.000000 sax-0.9.2/sax/multimode.py
+-rw-r--r--   0 root         (0) root         (0)    10761 2023-08-24 14:29:33.000000 sax-0.9.2/sax/netlist.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-08-24 14:29:33.000000 sax-0.9.2/sax/netlist_cleaning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-24 14:30:13.913032 sax-0.9.2/sax/nn/
+-rw-r--r--   0 root         (0) root         (0)      971 2023-08-24 14:29:33.000000 sax-0.9.2/sax/nn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-08-24 14:29:33.000000 sax-0.9.2/sax/nn/core.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-08-24 14:29:33.000000 sax-0.9.2/sax/nn/io.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-08-24 14:29:33.000000 sax-0.9.2/sax/nn/loss.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-08-24 14:29:33.000000 sax-0.9.2/sax/nn/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2023-08-24 14:29:33.000000 sax-0.9.2/sax/patched.py
+-rw-r--r--   0 root         (0) root         (0)    10223 2023-08-24 14:29:33.000000 sax-0.9.2/sax/typing_.py
+-rw-r--r--   0 root         (0) root         (0)    18468 2023-08-24 14:29:33.000000 sax-0.9.2/sax/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-24 14:30:13.909032 sax-0.9.2/sax.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      838 2023-08-24 14:30:13.000000 sax-0.9.2/sax.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2023-08-24 14:30:13.000000 sax-0.9.2/sax.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-24 14:30:13.000000 sax-0.9.2/sax.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      517 2023-08-24 14:30:13.000000 sax-0.9.2/sax.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-08-24 14:30:13.000000 sax-0.9.2/sax.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-24 14:30:13.913032 sax-0.9.2/setup.cfg
```

### Comparing `sax-0.9.1/LICENSE` & `sax-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/PKG-INFO` & `sax-0.9.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sax
-Version: 0.9.1
+Version: 0.9.2
 Summary: Autograd and XLA for S-parameters
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `sax-0.9.1/README.md` & `sax-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/pyproject.toml` & `sax-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "pip", "build", "wheel", "pybind11"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sax"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Autograd and XLA for S-parameters"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
@@ -27,15 +27,15 @@
   "black",
   "fastcore",
   "h5py",
   "natsort",
   "networkx",
   "numpy",
   "orjson",
-  "pydantic>=2",
+  "pydantic",
   "pyyaml",
   "tables",
   "tqdm",
 ]
 
 [project.optional-dependencies]
 nojax = ["sax"]
```

### Comparing `sax-0.9.1/sax/__init__.py` & `sax-0.9.2/sax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 __all__ = []
 
 # Internal Cell
 #nbdev_comment from __future__ import annotations
 
 __author__ = "Floris Laporte"
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 # Cell
 from functools import partial as partial
 from math import pi as pi
 
 from scipy.constants import c as c
```

### Comparing `sax-0.9.1/sax/_nbdev.py` & `sax-0.9.2/sax/_nbdev.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/backends/__init__.py` & `sax-0.9.2/sax/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/backends/additive.py` & `sax-0.9.2/sax/backends/additive.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/backends/default.py` & `sax-0.9.2/sax/backends/default.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/backends/klu.py` & `sax-0.9.2/sax/backends/klu.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/circuit.py` & `sax-0.9.2/sax/circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,50 +15,55 @@
 import sys
 from functools import partial
 from typing import Any, Dict, List, NamedTuple, Optional, Tuple, TypedDict, Union
 
 import black
 import networkx as nx
 import numpy as np
-from pydantic import ValidationError
 from sax import reciprocal
 from .backends import circuit_backends
 from .multimode import multimode, singlemode
 from .netlist import Netlist, RecursiveNetlist
 from .netlist_cleaning import remove_unused_instances
 from .typing_ import Model, Settings, SType
 from .utils import _replace_kwargs, get_settings, merge_dicts, update_settings
 
 # Cell
+try:
+    from pydantic.v1 import ValidationError
+except ImportError:
+    from pydantic import ValidationError
+
+# Cell
 def create_dag(
     netlist: RecursiveNetlist,
     models: Optional[Dict[str, Any]] = None,
 ):
     if models is None:
         models = {}
     assert isinstance(models, dict)
 
     all_models = {}
     g = nx.DiGraph()
 
-    for model_name, subnetlist in netlist.dict().items():
+    for model_name, subnetlist in netlist.dict()["__root__"].items():
         if not model_name in all_models:
             all_models[model_name] = models.get(model_name, subnetlist)
             g.add_node(model_name)
         if model_name in models:
             continue
         for instance in subnetlist["instances"].values():
             component = instance["component"]
             if not component in all_models:
                 all_models[component] = models.get(component, None)
                 g.add_node(component)
             g.add_edge(model_name, component)
 
     # we only need the nodes that depend on the parent...
-    parent_node = next(iter(netlist.root.keys()))
+    parent_node = next(iter(netlist.__root__.keys()))
     nodes = [parent_node, *nx.descendants(g, parent_node)]
     g = nx.induced_subgraph(g, nodes)
 
     return g
 
 # Cell
 
@@ -198,15 +203,15 @@
     current_models = {}
     model_names = list(nx.topological_sort(dependency_dag))[::-1]
     for model_name in model_names:
         if model_name in models:
             new_models[model_name] = models[model_name]
             continue
 
-        flatnet = recnet.root[model_name]
+        flatnet = recnet.__root__[model_name]
 
         connections, ports, new_models = _make_singlemode_or_multimode(
             flatnet, modes, new_models
         )
         current_models.update(new_models)
         new_models = {}
 
@@ -231,14 +236,16 @@
     dag: nx.DiGraph
     models: Dict[str, Model]
 
 
 def _ensure_recursive_netlist_dict(netlist):
     if not isinstance(netlist, dict):
         netlist = netlist.dict()
+    if "__root__" in netlist:
+        netlist = netlist["__root__"]
     if "instances" in netlist:
         netlist = {"top_level": netlist}
     netlist = {**netlist}
     for k, v in netlist.items():
         netlist[k] = {**v}
     return netlist
 
@@ -289,19 +296,19 @@
     else:
         raise ValueError(f"Invalid modes given: {modes}")
 
 
 def _validate_net(netlist: Union[Netlist, RecursiveNetlist]) -> RecursiveNetlist:
     if isinstance(netlist, dict):
         try:
-            netlist = Netlist.model_validate(netlist)
+            netlist = Netlist.parse_obj(netlist)
         except ValidationError:
-            netlist = RecursiveNetlist.model_validate(netlist)
+            netlist = RecursiveNetlist.parse_obj(netlist)
     elif isinstance(netlist, Netlist):
-        netlist = RecursiveNetlist(root={"top_level": netlist})
+        netlist = RecursiveNetlist(__root__={"top_level": netlist})
     return netlist
 
 
 def _validate_dag(dag):
     nodes = find_root(dag)
     if len(nodes) > 1:
         raise ValueError(f"Multiple top_levels found in netlist: {nodes}")
@@ -353,15 +360,15 @@
     netlist, instance_models = _extract_instance_models(netlist)
     recnet: RecursiveNetlist = _validate_net(netlist)
 
     missing_models = {}
     missing_model_names = []
     g = nx.DiGraph()
 
-    for model_name, subnetlist in recnet.dict().items():
+    for model_name, subnetlist in recnet.dict()["__root__"].items():
         if not model_name in missing_models:
             missing_models[model_name] = models.get(model_name, subnetlist)
             g.add_node(model_name)
         if model_name in models:
             continue
         for instance in subnetlist["instances"].values():
             component = instance["component"]
```

### Comparing `sax-0.9.1/sax/make_docs.py` & `sax-0.9.2/sax/make_docs.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/models.py` & `sax-0.9.2/sax/models.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/multimode.py` & `sax-0.9.2/sax/multimode.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/netlist.py` & `sax-0.9.2/sax/netlist.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,25 +10,31 @@
 from enum import Enum
 from functools import lru_cache, partial
 from typing import Any, Callable, Dict, Optional, Union
 
 import black
 import numpy as np
 import yaml
-from pydantic import BaseModel as _BaseModel, RootModel
-from pydantic import ConfigDict, Field, ValidationError, field_validator
 from .utils import clean_string, get_settings, hash_dict
 
-# Internal Cell
+# Cell
+try:
+    from pydantic.v1 import BaseModel as _BaseModel
+    from pydantic.v1 import Extra, Field, ValidationError, validator
+except ImportError:
+    from pydantic import BaseModel as _BaseModel
+    from pydantic import Extra, Field, ValidationError, validator
 
+# Internal Cell
 class BaseModel(_BaseModel):
-    model_config = ConfigDict(
-        extra="ignore",
-        frozen=True,
-    )
+    class Config:
+        extra = Extra.ignore
+        allow_mutation = False
+        frozen = True
+        json_encoders = {np.ndarray: lambda arr: np.round(arr, 12).tolist()}
 
     def __repr__(self):
         s = super().__repr__()
         s = black.format_str(s, mode=black.Mode())
         return s
 
     def __str__(self):
@@ -36,25 +42,25 @@
 
     def __hash__(self):
         return hash_dict(self.dict())
 
 # Cell
 
 class Component(BaseModel):
-    model_config = ConfigDict(
-        extra="ignore",
-        frozen=True,
-    )
+    class Config:
+        extra = Extra.ignore
+        allow_mutation = False
+        frozen = True
+        json_encoders = {np.ndarray: lambda arr: np.round(arr, 12).tolist()}
 
     component: Union[str, Dict[str, Any]] = Field(..., title="Component")
     settings: Optional[Dict[str, Any]] = Field(None, title="Settings")
 
     # this was added:
-    @field_validator("component")
-    @classmethod
+    @validator("component")
     def validate_component_name(cls, value):
         if "," in value:
             raise ValueError(
                 f"Invalid component string. Should not contain ','. Got: {value}"
             )
         return clean_string(value)
 
@@ -69,18 +75,19 @@
     se = "se"
     sw = "sw"
     center = "center"
     cc = "cc"
 
 
 class Placement(BaseModel):
-    model_config = ConfigDict(
-        extra="ignore",
-        frozen=True,
-    )
+    class Config:
+        extra = Extra.ignore
+        allow_mutation = False
+        frozen = True
+        json_encoders = {np.ndarray: lambda arr: np.round(arr, 12).tolist()}
 
     x: Optional[Union[str, float]] = Field(0, title="X")
     y: Optional[Union[str, float]] = Field(0, title="Y")
     xmin: Optional[Union[str, float]] = Field(None, title="Xmin")
     ymin: Optional[Union[str, float]] = Field(None, title="Ymin")
     xmax: Optional[Union[str, float]] = Field(None, title="Xmax")
     ymax: Optional[Union[str, float]] = Field(None, title="Ymax")
@@ -88,29 +95,31 @@
     dy: Optional[float] = Field(0, title="Dy")
     port: Optional[Union[str, PortEnum]] = Field(None, title="Port")
     rotation: Optional[int] = Field(0, title="Rotation")
     mirror: Optional[bool] = Field(False, title="Mirror")
 
 
 class Route(BaseModel):
-    model_config = ConfigDict(
-        extra="ignore",
-        frozen=True,
-    )
+    class Config:
+        extra = Extra.ignore
+        allow_mutation = False
+        frozen = True
+        json_encoders = {np.ndarray: lambda arr: np.round(arr, 12).tolist()}
 
     links: Dict[str, str] = Field(..., title="Links")
     settings: Optional[Dict[str, Any]] = Field(None, title="Settings")
     routing_strategy: Optional[str] = Field(None, title="Routing Strategy")
 
 
 class Netlist(BaseModel):
-    model_config = ConfigDict(
-        extra="ignore",
-        frozen=True,
-    )
+    class Config:
+        extra = Extra.ignore
+        allow_mutation = False
+        frozen = True
+        json_encoders = {np.ndarray: lambda arr: np.round(arr, 12).tolist()}
 
     instances: Dict[str, Component] = Field(..., title="Instances")
     connections: Optional[Dict[str, str]] = Field(None, title="Connections")
     ports: Optional[Dict[str, str]] = Field(None, title="Ports")
     placements: Optional[Dict[str, Placement]] = Field(None, title="Placements")
 
     # these were removed (irrelevant for SAX):
@@ -119,16 +128,15 @@
     # name: Optional[str] = Field(None, title='Name')
     # info: Optional[Dict[str, Any]] = Field(None, title='Info')
     # settings: Optional[Dict[str, Any]] = Field(None, title='Settings')
     # pdk: Optional[str] = Field(None, title='Pdk')
 
     # these are extra additions:
 
-    @field_validator("instances", mode="before")
-    @classmethod
+    @validator("instances", pre=True)
     def coerce_different_type_instance_into_component_model(cls, instances):
         new_instances = {}
         for k, v in instances.items():
             if isinstance(v, str):
                 v = {
                     "component": v,
                     "settings": {},
@@ -141,85 +149,85 @@
     def clean_instance_string(value):
         if "," in value:
             raise ValueError(
                 f"Invalid instance string. Should not contain ','. Got: {value}"
             )
         return clean_string(value)
 
-    @field_validator("instances")
-    @classmethod
+    @validator("instances")
     def validate_instance_names(cls, instances):
         return {cls.clean_instance_string(k): v for k, v in instances.items()}
 
-    @field_validator("placements")
-    @classmethod
+    @validator("placements")
     def validate_placement_names(cls, placements):
         return {cls.clean_instance_string(k): v for k, v in placements.items()}
 
     @classmethod
     def clean_connection_string(cls, value):
         *comp, port = value.split(",")
         comp = cls.clean_instance_string(",".join(comp))
         return f"{comp},{port}"
 
-    @field_validator("connections")
-    @classmethod
+    @validator("connections")
     def validate_connection_names(cls, connections):
         return {
             cls.clean_connection_string(k): cls.clean_connection_string(v)
             for k, v in connections.items()
         }
 
-    @field_validator("ports")
-    @classmethod
+    @validator("ports")
     def validate_port_names(cls, ports):
         return {
             cls.clean_instance_string(k): cls.clean_connection_string(v)
             for k, v in ports.items()
         }
 
 # Cell
 
-class RecursiveNetlist(RootModel):
-    model_config = ConfigDict(extra="ignore", frozen=True)
-    root: Dict[str, Netlist]
+class RecursiveNetlist(BaseModel):
+    class Config:
+        extra = Extra.ignore
+        allow_mutation = False
+        frozen = True
+
+    __root__: Dict[str, Netlist]
 
 # Cell
 
 def netlist(dic: Dict) -> RecursiveNetlist:
     if isinstance(dic, RecursiveNetlist):
         return dic
     elif isinstance(dic, Netlist):
         dic = dic.dict()
     try:
-        flat_net = Netlist.model_validate(dic)
-        net = RecursiveNetlist.model_validate({'top_level': flat_net})
+        flat_net = Netlist.parse_obj(dic)
+        net = RecursiveNetlist.parse_obj({'top_level': flat_net})
     except ValidationError:
-        net = RecursiveNetlist.model_validate(dic)
+        net = RecursiveNetlist.parse_obj(dic)
     return net
 
 # Cell
 @lru_cache()
 def load_netlist(pic_path) -> Netlist:
     with open(pic_path, "r") as file:
         net = yaml.safe_load(file.read())
-    return Netlist.model_validate(net)
+    return Netlist.parse_obj(net)
 
 # Cell
 @lru_cache()
 def load_recursive_netlist(pic_path, ext='.yml'):
     folder_path = os.path.dirname(os.path.abspath(pic_path))
     _clean_string = lambda path: clean_string(re.sub(ext, "", os.path.split(path)[-1]))
     netlists = {_clean_string(pic_path): None} # the circuit we're interested in should come first.
     for filename in os.listdir(folder_path):
         path = os.path.join(folder_path, filename)
         if not os.path.isfile(path) or not path.endswith(ext):
             continue
         netlists[_clean_string(path)] = load_netlist(path)
-    return RecursiveNetlist.model_validate(netlists)
+    return RecursiveNetlist.parse_obj(netlists)
 
 # Cell
 def get_netlist_instances_by_prefix(
         recursive_netlist: RecursiveNetlist,
         prefix: str,
 ):
     """
```

### Comparing `sax-0.9.1/sax/netlist_cleaning.py` & `sax-0.9.2/sax/netlist_cleaning.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/nn/__init__.py` & `sax-0.9.2/sax/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/nn/core.py` & `sax-0.9.2/sax/nn/core.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/nn/io.py` & `sax-0.9.2/sax/nn/io.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/nn/loss.py` & `sax-0.9.2/sax/nn/loss.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/nn/utils.py` & `sax-0.9.2/sax/nn/utils.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/patched.py` & `sax-0.9.2/sax/patched.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/typing_.py` & `sax-0.9.2/sax/typing_.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax/utils.py` & `sax-0.9.2/sax/utils.py`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax.egg-info/PKG-INFO` & `sax-0.9.2/sax.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sax
-Version: 0.9.1
+Version: 0.9.2
 Summary: Autograd and XLA for S-parameters
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `sax-0.9.1/sax.egg-info/SOURCES.txt` & `sax-0.9.2/sax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sax-0.9.1/sax.egg-info/requires.txt` & `sax-0.9.2/sax.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 black
 fastcore
 h5py
 natsort
 networkx
 numpy
 orjson
-pydantic>=2
+pydantic
 pyyaml
 tables
 tqdm
 
 [dev]
 sax[full]
 bump2version
```

