# Comparing `tmp/seapopym-0.0.1.1.tar.gz` & `tmp/seapopym-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seapopym-0.0.1.1.tar", max compression
+gzip compressed data, was "seapopym-0.0.1.3.tar", max compression
```

## Comparing `seapopym-0.0.1.1.tar` & `seapopym-0.0.1.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1070 2024-03-11 23:18:12.538968 seapopym-0.0.1.1/LICENSE
--rw-r--r--   0        0        0     1182 2024-04-08 05:08:29.595843 seapopym-0.0.1.1/README.md
--rw-r--r--   0        0        0      782 2024-04-08 05:08:50.626539 seapopym-0.0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.497608 seapopym-0.0.1.1/seapopym/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.497704 seapopym-0.0.1.1/seapopym/configuration/__init__.py
--rw-r--r--   0        0        0      927 2024-04-08 03:07:38.627785 seapopym-0.0.1.1/seapopym/configuration/base_configuration.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.497941 seapopym-0.0.1.1/seapopym/configuration/no_transport/__init__.py
--rw-r--r--   0        0        0     1852 2024-04-08 03:07:38.627988 seapopym-0.0.1.1/seapopym/configuration/no_transport/configuration.py
--rw-r--r--   0        0        0     7665 2024-04-08 02:54:52.889502 seapopym-0.0.1.1/seapopym/configuration/no_transport/configuration_to_dataset.py
--rw-r--r--   0        0        0     8015 2024-04-02 02:55:48.498567 seapopym-0.0.1.1/seapopym/configuration/no_transport/parameter.py
--rw-r--r--   0        0        0        0 2024-04-08 03:07:38.628025 seapopym-0.0.1.1/seapopym/configuration/parameters/__init__.py
--rw-r--r--   0        0        0     8036 2024-04-04 23:35:32.421245 seapopym-0.0.1.1/seapopym/configuration/parameters/parameter_environment.py
--rw-r--r--   0        0        0     6949 2024-04-08 03:07:38.628273 seapopym-0.0.1.1/seapopym/configuration/parameters/parameter_forcing.py
--rw-r--r--   0        0        0     5664 2024-04-02 02:55:48.499108 seapopym-0.0.1.1/seapopym/configuration/parameters/parameter_functional_group.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.499152 seapopym-0.0.1.1/seapopym/exception/__init__.py
--rw-r--r--   0        0        0     1981 2024-04-02 02:55:48.499367 seapopym-0.0.1.1/seapopym/exception/parameter_exception.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.499420 seapopym-0.0.1.1/seapopym/function/core/__init__.py
--rw-r--r--   0        0        0     2989 2024-04-08 03:07:38.628408 seapopym-0.0.1.1/seapopym/function/core/kernel.py
--rw-r--r--   0        0        0     7161 2024-04-08 03:07:38.628595 seapopym-0.0.1.1/seapopym/function/core/template.py
--rw-r--r--   0        0        0      556 2024-04-08 03:07:38.628847 seapopym-0.0.1.1/seapopym/function/generator/__init__.py
--rw-r--r--   0        0        0     4473 2024-04-08 03:07:38.629054 seapopym-0.0.1.1/seapopym/function/generator/apply_coefficient_to_primary_production.py
--rw-r--r--   0        0        0     3706 2024-04-08 03:07:38.629377 seapopym-0.0.1.1/seapopym/function/generator/average_temperature.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.500744 seapopym-0.0.1.1/seapopym/function/generator/biomass/__init__.py
--rw-r--r--   0        0        0     2778 2024-04-08 03:07:38.629650 seapopym-0.0.1.1/seapopym/function/generator/biomass/biomass.py
--rw-r--r--   0        0        0     1695 2024-04-02 02:55:48.501086 seapopym-0.0.1.1/seapopym/function/generator/biomass/compiled_functions.py
--rw-r--r--   0        0        0     6252 2024-04-08 03:07:38.629846 seapopym-0.0.1.1/seapopym/function/generator/cell_area.py
--rw-r--r--   0        0        0     5285 2024-04-08 03:07:38.630030 seapopym-0.0.1.1/seapopym/function/generator/day_length.py
--rw-r--r--   0        0        0     3729 2024-04-08 03:07:38.630168 seapopym-0.0.1.1/seapopym/function/generator/mask.py
--rw-r--r--   0        0        0     2280 2024-04-08 03:07:38.630364 seapopym-0.0.1.1/seapopym/function/generator/mask_temperature.py
--rw-r--r--   0        0        0     1754 2024-04-08 03:07:38.630541 seapopym-0.0.1.1/seapopym/function/generator/min_temperature.py
--rw-r--r--   0        0        0     2173 2024-04-08 03:07:38.630718 seapopym-0.0.1.1/seapopym/function/generator/mortality_field.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.502336 seapopym-0.0.1.1/seapopym/function/generator/production/__init__.py
--rw-r--r--   0        0        0     4543 2024-04-04 23:35:32.425733 seapopym-0.0.1.1/seapopym/function/generator/production/compiled_functions.py
--rw-r--r--   0        0        0     7885 2024-04-08 03:07:38.630936 seapopym-0.0.1.1/seapopym/function/generator/production/production.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.502858 seapopym-0.0.1.1/seapopym/logging/__init__.py
--rw-r--r--   0        0        0     2079 2024-04-02 02:55:48.503073 seapopym-0.0.1.1/seapopym/logging/custom_logger.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.503115 seapopym-0.0.1.1/seapopym/model/__init__.py
--rw-r--r--   0        0        0     1793 2024-04-08 03:07:38.631293 seapopym-0.0.1.1/seapopym/model/base_model.py
--rw-r--r--   0        0        0     5433 2024-04-08 03:07:38.631565 seapopym-0.0.1.1/seapopym/model/no_transport_model.py
--rw-r--r--   0        0        0        0 2024-04-08 03:07:38.631613 seapopym-0.0.1.1/seapopym/plotter/__init__.py
--rw-r--r--   0        0        0     1138 2024-04-08 03:07:38.631874 seapopym-0.0.1.1/seapopym/plotter/base_functions.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.503531 seapopym-0.0.1.1/seapopym/standard/__init__.py
--rw-r--r--   0        0        0     3707 2024-04-02 02:55:48.503717 seapopym-0.0.1.1/seapopym/standard/attributs.py
--rw-r--r--   0        0        0     2688 2024-04-02 02:55:48.503855 seapopym-0.0.1.1/seapopym/standard/coordinates.py
--rw-r--r--   0        0        0     3251 2024-04-08 03:07:38.632076 seapopym-0.0.1.1/seapopym/standard/labels.py
--rw-r--r--   0        0        0      880 2024-04-08 03:07:38.632268 seapopym-0.0.1.1/seapopym/standard/types.py
--rw-r--r--   0        0        0     2202 2024-04-02 02:55:48.504254 seapopym-0.0.1.1/seapopym/standard/units.py
--rw-r--r--   0        0        0        0 2024-04-04 23:35:32.426610 seapopym-0.0.1.1/seapopym/writer/__init__.py
--rw-r--r--   0        0        0     3073 2024-04-08 03:07:38.632464 seapopym-0.0.1.1/seapopym/writer/base_functions.py
--rw-r--r--   0        0        0     1977 1970-01-01 00:00:00.000000 seapopym-0.0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-11 23:18:12.538968 seapopym-0.0.1.3/LICENSE
+-rw-r--r--   0        0        0     1170 2024-04-08 23:04:02.855468 seapopym-0.0.1.3/README.md
+-rw-r--r--   0        0        0     1240 2024-04-10 21:47:32.273762 seapopym-0.0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.497608 seapopym-0.0.1.3/seapopym/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.497704 seapopym-0.0.1.3/seapopym/configuration/__init__.py
+-rw-r--r--   0        0        0     1110 2024-04-09 05:02:49.187954 seapopym-0.0.1.3/seapopym/configuration/base_configuration.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.497941 seapopym-0.0.1.3/seapopym/configuration/no_transport/__init__.py
+-rw-r--r--   0        0        0     2144 2024-04-09 05:03:52.135501 seapopym-0.0.1.3/seapopym/configuration/no_transport/configuration.py
+-rw-r--r--   0        0        0     7665 2024-04-08 02:54:52.889502 seapopym-0.0.1.3/seapopym/configuration/no_transport/configuration_to_dataset.py
+-rw-r--r--   0        0        0     8718 2024-04-10 00:16:49.797960 seapopym-0.0.1.3/seapopym/configuration/no_transport/parameter.py
+-rw-r--r--   0        0        0        0 2024-04-08 03:07:38.628025 seapopym-0.0.1.3/seapopym/configuration/parameters/__init__.py
+-rw-r--r--   0        0        0     8303 2024-04-10 06:02:33.805896 seapopym-0.0.1.3/seapopym/configuration/parameters/parameter_environment.py
+-rw-r--r--   0        0        0     6922 2024-04-10 06:03:03.659858 seapopym-0.0.1.3/seapopym/configuration/parameters/parameter_forcing.py
+-rw-r--r--   0        0        0     5664 2024-04-02 02:55:48.499108 seapopym-0.0.1.3/seapopym/configuration/parameters/parameter_functional_group.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.499152 seapopym-0.0.1.3/seapopym/exception/__init__.py
+-rw-r--r--   0        0        0     1981 2024-04-02 02:55:48.499367 seapopym-0.0.1.3/seapopym/exception/parameter_exception.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.499420 seapopym-0.0.1.3/seapopym/function/core/__init__.py
+-rw-r--r--   0        0        0     3134 2024-04-10 05:43:21.984226 seapopym-0.0.1.3/seapopym/function/core/kernel.py
+-rw-r--r--   0        0        0     7161 2024-04-08 03:07:38.628595 seapopym-0.0.1.3/seapopym/function/core/template.py
+-rw-r--r--   0        0        0      556 2024-04-08 03:07:38.628847 seapopym-0.0.1.3/seapopym/function/generator/__init__.py
+-rw-r--r--   0        0        0     3279 2024-04-08 23:41:33.783430 seapopym-0.0.1.3/seapopym/function/generator/apply_coefficient_to_primary_production.py
+-rw-r--r--   0        0        0     2884 2024-04-08 23:42:36.914042 seapopym-0.0.1.3/seapopym/function/generator/average_temperature.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.500744 seapopym-0.0.1.3/seapopym/function/generator/biomass/__init__.py
+-rw-r--r--   0        0        0     2266 2024-04-10 05:54:56.523895 seapopym-0.0.1.3/seapopym/function/generator/biomass/biomass.py
+-rw-r--r--   0        0        0     1695 2024-04-02 02:55:48.501086 seapopym-0.0.1.3/seapopym/function/generator/biomass/compiled_functions.py
+-rw-r--r--   0        0        0     6252 2024-04-08 03:07:38.629846 seapopym-0.0.1.3/seapopym/function/generator/cell_area.py
+-rw-r--r--   0        0        0     5285 2024-04-09 05:17:25.721091 seapopym-0.0.1.3/seapopym/function/generator/day_length.py
+-rw-r--r--   0        0        0     3729 2024-04-08 03:07:38.630168 seapopym-0.0.1.3/seapopym/function/generator/mask.py
+-rw-r--r--   0        0        0     2280 2024-04-08 03:07:38.630364 seapopym-0.0.1.3/seapopym/function/generator/mask_temperature.py
+-rw-r--r--   0        0        0     1766 2024-04-08 23:40:17.869043 seapopym-0.0.1.3/seapopym/function/generator/min_temperature.py
+-rw-r--r--   0        0        0     2173 2024-04-08 03:07:38.630718 seapopym-0.0.1.3/seapopym/function/generator/mortality_field.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.502336 seapopym-0.0.1.3/seapopym/function/generator/production/__init__.py
+-rw-r--r--   0        0        0     7571 2024-04-10 03:59:53.391409 seapopym-0.0.1.3/seapopym/function/generator/production/compiled_functions.py
+-rw-r--r--   0        0        0     6580 2024-04-10 05:54:40.556574 seapopym-0.0.1.3/seapopym/function/generator/production/production.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.502858 seapopym-0.0.1.3/seapopym/logging/__init__.py
+-rw-r--r--   0        0        0     2079 2024-04-02 02:55:48.503073 seapopym-0.0.1.3/seapopym/logging/custom_logger.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.503115 seapopym-0.0.1.3/seapopym/model/__init__.py
+-rw-r--r--   0        0        0     1793 2024-04-08 03:07:38.631293 seapopym-0.0.1.3/seapopym/model/base_model.py
+-rw-r--r--   0        0        0     4461 2024-04-10 21:46:19.171146 seapopym-0.0.1.3/seapopym/model/no_transport_model.py
+-rw-r--r--   0        0        0        0 2024-04-08 03:07:38.631613 seapopym-0.0.1.3/seapopym/plotter/__init__.py
+-rw-r--r--   0        0        0     1138 2024-04-08 03:07:38.631874 seapopym-0.0.1.3/seapopym/plotter/base_functions.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.503531 seapopym-0.0.1.3/seapopym/standard/__init__.py
+-rw-r--r--   0        0        0     3707 2024-04-02 02:55:48.503717 seapopym-0.0.1.3/seapopym/standard/attributs.py
+-rw-r--r--   0        0        0     2688 2024-04-02 02:55:48.503855 seapopym-0.0.1.3/seapopym/standard/coordinates.py
+-rw-r--r--   0        0        0     3251 2024-04-08 03:07:38.632076 seapopym-0.0.1.3/seapopym/standard/labels.py
+-rw-r--r--   0        0        0      880 2024-04-08 03:07:38.632268 seapopym-0.0.1.3/seapopym/standard/types.py
+-rw-r--r--   0        0        0     2202 2024-04-02 02:55:48.504254 seapopym-0.0.1.3/seapopym/standard/units.py
+-rw-r--r--   0        0        0        0 2024-04-04 23:35:32.426610 seapopym-0.0.1.3/seapopym/writer/__init__.py
+-rw-r--r--   0        0        0     3666 2024-04-10 03:53:43.521606 seapopym-0.0.1.3/seapopym/writer/base_functions.py
+-rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 seapopym-0.0.1.3/PKG-INFO
```

### Comparing `seapopym-0.0.1.1/LICENSE` & `seapopym-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/README.md` & `seapopym-0.0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 
 ```bash
 poetry install
 ```
 
 ## Documentation
 
-The documentation is available [here](https://seapodym-lmtl-python.readthedocs.io/en/latest/).
+The documentation is available [here](https://seapopym.readthedocs.io/en/latest/).
```

### Comparing `seapopym-0.0.1.1/seapopym/configuration/base_configuration.py` & `seapopym-0.0.1.3/seapopym/configuration/base_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,7 +25,12 @@
     def model_parameters(self: BaseConfiguration) -> xr.Dataset:
         """The xarray.Dataset that stores all the model parameters and forcing."""
 
     @property
     @abc.abstractmethod
     def environment_parameters(self: BaseConfiguration) -> attrs.Attribute:
         """The attrs dataclass that stores all the environment parameters."""
+
+    @property
+    @abc.abstractmethod
+    def kernel_parameters(self: BaseConfiguration) -> attrs.Attribute:
+        """The attrs dataclass that stores all the kernel parameters."""
```

### Comparing `seapopym-0.0.1.1/seapopym/configuration/no_transport/configuration.py` & `seapopym-0.0.1.3/seapopym/configuration/no_transport/configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from __future__ import annotations
 
 from typing import IO, TYPE_CHECKING
 
 from seapopym.configuration.base_configuration import BaseConfiguration
 from seapopym.configuration.no_transport.configuration_to_dataset import as_dataset
+from seapopym.configuration.no_transport.parameter import KernelParameters
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     import xarray as xr
 
     from seapopym.configuration.no_transport.parameter import NoTransportParameters
@@ -35,12 +36,17 @@
         )
 
     @property
     def environment_parameters(self: NoTransportConfiguration) -> EnvironmentParameter:
         """The attrs dataclass that stores all the environment parameters."""
         return self._parameters.environment_parameters
 
+    @property
+    def kernel_parameters(self: NoTransportConfiguration) -> KernelParameters:
+        """The attrs dataclass that stores all the kernel parameters."""
+        return self._parameters.kernel_parameters
+
     @classmethod
     def parse(cls: NoTransportConfiguration, configuration_file: str | Path | IO) -> NoTransportConfiguration:  # noqa: ARG003
         """Parse the configuration file and create a NoTransportConfiguration object."""
         msg = "This method is not implemented yet."
         raise NotImplementedError(msg)
```

### Comparing `seapopym-0.0.1.1/seapopym/configuration/no_transport/configuration_to_dataset.py` & `seapopym-0.0.1.3/seapopym/configuration/no_transport/configuration_to_dataset.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/configuration/no_transport/parameter.py` & `seapopym-0.0.1.3/seapopym/configuration/no_transport/parameter.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,27 +146,48 @@
         """This method is used to check the consistency of the functional groups."""
         if not all(isinstance(fgroup, FunctionalGroupUnit) for fgroup in value):
             msg = "All the functional groups must be instance of FunctionalGroupUnit."
             raise TypeError(msg)
 
 
 @frozen(kw_only=True)
+class KernelParameters:
+    """This data class is used to store the parameters of the kernel."""
+
+    angle_horizon_sun: float = field(
+        default=0.0, metadata={"description": "The angle between the horizon and the sun in degrees."}
+    )
+
+    compute_initial_conditions: bool = field(
+        default=False, metadata={"description": "If True, the initial conditions are computed."}
+    )
+
+    compute_preproduction: bool = field(
+        default=False, metadata={"description": "If True, the pre-production is computed."}
+    )
+
+
+@frozen(kw_only=True)
 class NoTransportParameters:
     """This is the main data class. It is used to store the model configuration parameters."""
 
     forcing_parameters: ForcingParameters = field(metadata={"description": "All the paths to the forcings."})
 
     functional_groups_parameters: FunctionalGroups = field(
         metadata={"description": "Parameters of all functional groups."}
     )
 
     environment_parameters: EnvironmentParameter = field(
         factory=EnvironmentParameter, metadata={"description": "Parameters of the environment."}
     )
 
+    kernel_parameters: KernelParameters = field(
+        factory=KernelParameters, metadata={"description": "Parameters of the kernel."}
+    )
+
     def __attrs_post_init__(self: NoTransportParameters) -> None:
         """
         Check that the timestep of the functional groups is consistent (ie. multiple of) with the timestep of the
         forcings.
         """
         global_timestep = self.forcing_parameters.timestep
         for fgroup in self.functional_groups_parameters.functional_groups:
```

### Comparing `seapopym-0.0.1.1/seapopym/configuration/parameters/parameter_environment.py` & `seapopym-0.0.1.3/seapopym/configuration/parameters/parameter_environment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
+"""A module to manage the environment parameters of the simulation."""
 from __future__ import annotations
 
-from pathlib import Path
-from typing import Iterable, Literal
+from typing import Literal
 
 import numpy as np
 from attrs import define, field, frozen, validators
 from dask.distributed import Client
 
 from seapopym.logging.custom_logger import logger
 
 
 @frozen
 class ChunkParameter:
     """The chunk size of the different dimensions."""
 
-    functional_group: str | int | None = field(
-        default="auto",
+    functional_group: Literal["auto"] | int | None = field(
+        default=1,
         validator=validators.optional(validators.instance_of((str, int))),
         metadata={"description": "The chunk size of the functional group dimension."},
     )
-    latitude: str | int | None = field(
+    latitude: Literal["auto"] | int | None = field(
         default=None,
         validator=validators.optional(validators.instance_of((str, int))),
         metadata={"description": "The chunk size of the latitude dimension."},
     )
-    longitude: str | int | None = field(
+    longitude: Literal["auto"] | int | None = field(
         default=None,
         validator=validators.optional(validators.instance_of((str, int))),
         metadata={"description": "The chunk size of the longitude dimension."},
     )
     time: None = field(
         init=False,
         default=None,
@@ -51,17 +51,18 @@
             chunks["longitude"] = self.longitude
         return chunks
 
 
 @define
 class ClientParameter:
     """
+    The client parameter for the Dask client.
+
     If an address is provided, the client will be initialized with this address and other parameters will be ignored.
     If no address is provided, a LocalCluster will be initialized with the other parameters.
-
     For more information about this class check the Dask documentation about LocalCluster and Client.
     """
 
     n_workers: int | None = field(
         default=None,
         validator=validators.optional(validators.instance_of(int)),
         metadata={"description": "The number of workers."},
@@ -127,86 +128,87 @@
         else:
             self.client.cluster.close()
         self.client.close()
         del self.client
         self.client = None
 
 
-@frozen(kw_only=True)
-class BaseOuputForcingParameter:
-    """A base class for the output forcing parameter."""
-
-    path: str | Path = field(
-        default=Path("./output.nc"),
-        converter=Path,
-        metadata={"description": "The path where the forcing will be stored."},
-    )
-    with_parameter: bool = field(
-        default=True,
-        validator=validators.instance_of(bool),
-        metadata={"description": "If True, the forcing will be computed with the parameter forcing."},
-    )
-    with_forcing: bool = field(
-        default=False,
-        validator=validators.instance_of(bool),
-        metadata={"description": "If True, forcing will be added to the output dataset."},
-    )
-
-
-@frozen(kw_only=True)
-class BiomassParameter(BaseOuputForcingParameter):
-    """The output parameter for the biomass forcing."""
-
-
-@frozen(kw_only=True)
-class ProductionParameter(BaseOuputForcingParameter):
-    """The output parameter for the production forcing."""
-
-
-@frozen(kw_only=True)
-class PreProductionParameter(BaseOuputForcingParameter):
-    """The output parameter for the pre-production forcing (i.e. with cohorts)."""
-
-    timestamps: Iterable[str] | Iterable[int] | Literal["all"] = field(
-        default=[-1],
-        converter=lambda x: [x] if x != "all" and isinstance(x, (int, str)) else x,
-        metadata={"description": "The timestamps for the pre-production forcing."},
-    )
-
-    @timestamps.validator
-    def _validate_timestamps(
-        self: PreProductionParameter, attribute: str, value: Iterable[str] | Iterable[int]
-    ) -> None:
-        if value == "all":
-            return
-
-        msg = "The timestamps must be either 'all' or a list of integers (time index) or a list of strings (datetime)."
-        if not isinstance(value, Iterable):
-            raise TypeError(msg)
-        if all(isinstance(x, int) for x in value):
-            return
-        if all(isinstance(x, str) for x in value):
-            return
-        raise TypeError(msg)
-
-
-@frozen(kw_only=True)
-class OutputParameter:
-    """The output parameter that manage the backup of the output forcings."""
-
-    biomass: BiomassParameter = field(
-        factory=BiomassParameter,
-        validator=validators.instance_of(BiomassParameter),
-        metadata={"description": "The output parameter for the biomass forcing."},
-    )
-    pre_production: PreProductionParameter = field(
-        default=None,
-        validator=validators.optional(validators.instance_of(PreProductionParameter)),
-        metadata={"description": "The output parameter for the pre-production forcing."},
-    )
+# @frozen(kw_only=True)
+# class BaseOuputForcingParameter:
+#     """A base class for the output forcing parameter."""
+
+#     path: str | Path = field(
+#         default=Path("./output.nc"),
+#         converter=Path,
+#         metadata={"description": "The path where the forcing will be stored."},
+#     )
+#     with_parameter: bool = field(
+#         default=True,
+#         validator=validators.instance_of(bool),
+#         metadata={"description": "If True, the forcing will be computed with the parameter forcing."},
+#     )
+#     with_forcing: bool = field(
+#         default=False,
+#         validator=validators.instance_of(bool),
+#         metadata={"description": "If True, forcing will be added to the output dataset."},
+#     )
+
+
+# @frozen(kw_only=True)
+# class BiomassParameter(BaseOuputForcingParameter):
+#     """The output parameter for the biomass forcing."""
+
+
+# @frozen(kw_only=True)
+# class ProductionParameter(BaseOuputForcingParameter):
+#     """The output parameter for the production forcing."""
+
+
+# @frozen(kw_only=True)
+# class PreProductionParameter(BaseOuputForcingParameter):
+#     """The output parameter for the pre-production forcing (i.e. with cohorts)."""
+
+#     timestamps: Iterable[str] | Iterable[int] | Literal["all"] = field(
+#         default=[-1],
+#         converter=lambda x: [x] if x != "all" and isinstance(x, (int, str)) else x,
+#         metadata={"description": "The timestamps for the pre-production forcing."},
+#     )
+
+#     @timestamps.validator
+#     def _validate_timestamps(
+#         self: PreProductionParameter, attribute: str, value: Iterable[str] | Iterable[int]
+#     ) -> None:
+#         if value == "all":
+#             return
+
+#         msg = "The timestamps must be either 'all' or a list of integers (time index) or a list of strings (datetime)."
+#         if not isinstance(value, Iterable):
+#             raise TypeError(msg)
+#         if all(isinstance(x, int) for x in value):
+#             return
+#         if all(isinstance(x, str) for x in value):
+#             return
+#         raise TypeError(msg)
+
+
+# @frozen(kw_only=True)
+# class OutputParameter:
+#     """The output parameter that manage the backup of the output forcings."""
+
+#     biomass: BiomassParameter = field(
+#         factory=BiomassParameter,
+#         validator=validators.instance_of(BiomassParameter),
+#         metadata={"description": "The output parameter for the biomass forcing."},
+#     )
+#     pre_production: PreProductionParameter = field(
+#         default=None,
+#         validator=validators.optional(validators.instance_of(PreProductionParameter)),
+#         metadata={"description": "The output parameter for the pre-production forcing."},
+#     )
+#     initial_conditions:
 
 
 @frozen(kw_only=True)
 class EnvironmentParameter:
     """Manage the different environment parameters of the simulation."""
 
     chunk: ChunkParameter = field(
@@ -215,12 +217,12 @@
         metadata={"description": "The chunk size of the different dimensions."},
     )
     client: ClientParameter = field(
         factory=ClientParameter,
         validator=validators.instance_of(ClientParameter),
         metadata={"description": "The client parameter."},
     )
-    output: OutputParameter = field(
-        factory=OutputParameter,
-        validator=validators.instance_of(OutputParameter),
-        metadata={"description": "The output parameter."},
-    )
+    # output: OutputParameter = field(
+    #     factory=OutputParameter,
+    #     validator=validators.instance_of(OutputParameter),
+    #     metadata={"description": "The output parameter."},
+    # )
```

### Comparing `seapopym-0.0.1.1/seapopym/configuration/parameters/parameter_forcing.py` & `seapopym-0.0.1.3/seapopym/configuration/parameters/parameter_forcing.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
         message = f"DataArray {name} is not in the Dataset.\nAccepted values are : {", ".join(list(forcing))}"
         raise ValueError(message)
 
 
 @frozen(kw_only=True)
 class ForcingUnit:
     """
-    TODO(Jules): Refactor.
     This data class is used to store a forcing field and its resolution and timestep.
 
     Parameters
     ----------
     forcing: xr.DataArray
         Forcing field.
     resolution: tuple[float, float] | None
```

### Comparing `seapopym-0.0.1.1/seapopym/configuration/parameters/parameter_functional_group.py` & `seapopym-0.0.1.3/seapopym/configuration/parameters/parameter_functional_group.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/exception/parameter_exception.py` & `seapopym-0.0.1.3/seapopym/exception/parameter_exception.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/function/core/kernel.py` & `seapopym-0.0.1.3/seapopym/function/core/kernel.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,69 +5,70 @@
 from typing import Callable, Iterable, ParamSpecArgs, ParamSpecKwargs
 
 import xarray as xr
 from attrs import define, field
 
 from seapopym.function.core.template import BaseTemplate, ForcingTemplate, StateTemplate
 from seapopym.logging.custom_logger import logger
-from seapopym.standard import types
+from seapopym.standard.types import SeapopymForcing, SeapopymState
 
 
 @define
 class KernelUnits:
     name: str
     template: BaseTemplate
-    function: Callable[
-        [types.SeapopymState, ParamSpecArgs, ParamSpecKwargs], types.SeapopymState | types.SeapopymForcing
-    ]
+    function: Callable[[SeapopymState, ParamSpecArgs, ParamSpecKwargs], SeapopymState | SeapopymForcing]
     args: ParamSpecArgs = field(factory=tuple)
     kwargs: ParamSpecKwargs = field(factory=dict)
 
-    def _map_block_without_dask(self: KernelUnits, state: types.SeapopymState):
+    def _map_block_without_dask(self: KernelUnits, state: SeapopymState):
         logger.debug(f"Direct computation for {self.function.__name__}.")
         results = self.function(state, *self.args, **self.kwargs)
 
         if isinstance(self.template, ForcingTemplate):
-            if isinstance(results, types.SeapopymState):
+            if isinstance(results, SeapopymState):
                 msg = "When the function returns a xarray.Dataset, the template attribut should be a ForcingTemplate."
                 raise TypeError(msg)
             results.name = self.template.name
             return results.assign_attrs(self.template.attrs)
 
         if isinstance(self.template, StateTemplate):
-            if isinstance(results, types.SeapopymForcing):
+            if isinstance(results, SeapopymForcing):
                 msg = "When the function returns a xarray.Dataset, the template attribut should be a StateTemplate."
                 raise TypeError(msg)
             for template in self.template.template:
                 if template.name not in results:
                     msg = f"Variable {template.name} is not in the results."
                     raise ValueError(msg)
                 results[template.name] = results[template.name].assign_attrs(template.attrs)
             return results
 
         msg = "The template attribut should be a ForcingTemplate or a StateTemplate."
         raise TypeError(msg)
 
-    def _map_block_with_dask(self: KernelUnits, state: types.SeapopymState):
+    def _map_block_with_dask(self: KernelUnits, state: SeapopymState) -> SeapopymForcing | SeapopymState:
         logger.debug(f"Creating template for {self.function.__name__}.")
 
         result_template = self.template.generate(state)
 
         logger.debug(f"Applying map_blocks to {self.function.__name__}.")
         return xr.map_blocks(self.function, state, template=result_template, args=self.args, kwargs=self.kwargs)
 
-    def run(self: KernelUnits, state: types.SeapopymState) -> types.SeapopymState | types.SeapopymForcing:
+    def run(self: KernelUnits, state: SeapopymState) -> SeapopymState | SeapopymForcing:
         if len(state.chunks) == 0:
             return self._map_block_without_dask(state)
 
         return self._map_block_with_dask(state)
 
 
 class Kernel:
     def __init__(self: Kernel, functions: Iterable[KernelUnits]) -> None:
         self._kernels = functions
 
-    def run(self: Kernel, state: types.SeapopymState) -> types.SeapopymState:
+    def run(self: Kernel, state: SeapopymState) -> SeapopymState:
         for kernel in self._kernels:
             results = kernel.run(state)
             state = state.merge(results)
         return state
+
+    def template(self: Kernel, state: SeapopymState) -> SeapopymState:
+        return xr.merge([unit.template.generate(state) for unit in self._kernels] + [state])
```

### Comparing `seapopym-0.0.1.1/seapopym/function/core/template.py` & `seapopym-0.0.1.3/seapopym/function/core/template.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/function/generator/__init__.py` & `seapopym-0.0.1.3/seapopym/function/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/function/generator/apply_coefficient_to_primary_production.py` & `seapopym-0.0.1.3/seapopym/function/generator/apply_coefficient_to_primary_production.py`

 * *Files 16% similar despite different names*

```diff
@@ -58,37 +58,14 @@
     - primary_production [functional_group, time, latitude, longitude]
     """
     primary_production = check_units(state[ForcingLabels.primary_production], StandardUnitsLabels.production.units)
     pp_by_fgroup_gen = (i * primary_production for i in state[ConfigurationLabels.energy_transfert])
     return xr.concat(pp_by_fgroup_gen, dim=CoordinatesLabels.functional_group)
 
 
-# def apply_coefficient_to_primary_production(
-#     state: xr.Dataset, chunk: dict | None = None, lazy: ForcingName | None = None
-# ) -> SeapopymForcing:
-#     """Wrap the application of the transfert cooeficient to primary production with a map_block function."""
-#     template = Template(
-#         name=ForcingLabels.primary_production_by_fgroup,
-#         dims=[CoordinatesLabels.functional_group, CoordinatesLabels.time, CoordinatesLabels.Y, CoordinatesLabels.X],
-#         attributs=apply_coefficient_to_primary_production_desc,
-#         chunk=chunk,
-#     )
-#     class_type = Template if lazy is None else TemplateLazy
-#     template_attributs = {
-#         "name": ForcingLabels.primary_production_by_fgroup,
-#         "dims": [CoordinatesLabels.functional_group, CoordinatesLabels.time, CoordinatesLabels.Y, CoordinatesLabels.X],
-#         "attributs": apply_coefficient_to_primary_production_desc,
-#         "chunk": chunk,
-#     }
-#     if lazy is not None:
-#         template_attributs["model_name"] = lazy
-#     template = class_type(**template_attributs)
-#     return apply_map_block(function=_apply_coefficient_to_primary_production_helper, state=state, template=template)
-
-
 def apply_coefficient_to_primary_production_template(chunk: dict | None = None) -> ForcingTemplate:
     return ForcingTemplate(
         name=ForcingLabels.primary_production_by_fgroup,
         dims=[CoordinatesLabels.functional_group, CoordinatesLabels.time, CoordinatesLabels.Y, CoordinatesLabels.X],
         attrs=apply_coefficient_to_primary_production_desc,
         chunks=chunk,
     )
```

### Comparing `seapopym-0.0.1.1/seapopym/function/generator/average_temperature.py` & `seapopym-0.0.1.3/seapopym/function/generator/mask_temperature.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,69 @@
-"""An average temperature by fgroup computation wrapper. Use xarray.map_block."""
+"""A temperature mask computation wrapper. Use xarray.map_block."""
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 import cf_xarray  # noqa: F401
-import xarray as xr
 
 from seapopym.function.core.kernel import KernelUnits
 from seapopym.function.core.template import ForcingTemplate
-from seapopym.standard.attributs import average_temperature_by_fgroup_desc
-from seapopym.standard.labels import ConfigurationLabels, CoordinatesLabels, ForcingLabels
+from seapopym.standard.attributs import mask_temperature_desc
+from seapopym.standard.labels import CoordinatesLabels, ForcingLabels
 from seapopym.standard.units import StandardUnitsLabels, check_units
 
+if TYPE_CHECKING:
+    import xarray as xr
+
 
-def _average_temperature(state: xr.Dataset) -> xr.DataArray:
+def _mask_temperature_helper(state: xr.Dataset) -> xr.DataArray:
     """
-    Depend on:
-    - compute_daylength
-    - mask_by_fgroup.
+    It uses the min_temperature.
+
+    Depend on
+    ---------
+    - min_temperature()
+    - average_temperature()
 
     Input
     -----
-    - mask_by_fgroup()      [time, latitude, longitude]
-    - compute_daylength()   [functional_group, latitude, longitude] in day
-    - day/night_layer       [functional_group]
-    - temperature           [time, latitude, longitude, layer] in degC
+    - min_temperature [cohort_age]
+    - average_temperature [functional_group, time, latitude, longitude]
 
     Output
     ------
-    - avg_temperature [functional_group, time, latitude, longitude] in degC
-    """
-    temperature = check_units(state[ForcingLabels.temperature], StandardUnitsLabels.temperature.units)
-    day_length = check_units(state[ForcingLabels.day_length], StandardUnitsLabels.time.units)
-    mask_by_fgroup = state[ForcingLabels.mask_by_fgroup]
-    day_layer = state[ConfigurationLabels.day_layer]
-    night_layer = state[ConfigurationLabels.night_layer]
-
-    average_temperature = []
-    for fgroup in day_layer[CoordinatesLabels.functional_group]:
-        day_temperature = temperature.cf.sel(Z=day_layer.sel({CoordinatesLabels.functional_group: fgroup}))
-        night_temperature = temperature.cf.sel(Z=night_layer.sel({CoordinatesLabels.functional_group: fgroup}))
-        mean_temperature = (day_length * day_temperature) + ((1 - day_length) * night_temperature)
-        if "Z" in mean_temperature.cf:
-            mean_temperature = mean_temperature.cf.drop_vars("Z")
-        mean_temperature = mean_temperature.where(mask_by_fgroup.sel({CoordinatesLabels.functional_group: fgroup}))
-        average_temperature.append(mean_temperature)
-
-    return xr.concat(average_temperature, dim=CoordinatesLabels.functional_group.value)
-
-
-# def average_temperature(
-#     state: xr.Dataset, chunk: dict | None = None, lazy: ForcingName | None = None
-# ) -> SeapopymForcing:
-#     """Wrap the average temperature by functional group computation with a map_block function."""
-#     class_type = Template if lazy is None else TemplateLazy
-#     template_attributs = {
-#         "name": ForcingLabels.avg_temperature_by_fgroup,
-#         "dims": [CoordinatesLabels.functional_group, CoordinatesLabels.time, CoordinatesLabels.Y, CoordinatesLabels.X],
-#         "attributs": average_temperature_by_fgroup_desc,
-#         "chunk": chunk,
-#     }
-#     if lazy is not None:
-#         template_attributs["model_name"] = lazy
-#     template = class_type(**template_attributs)
+    - mask_temperature_by_cohort_by_functional_group [functional_group, time, latitude, longitude, cohort_age]
 
-#     return apply_map_block(function=_average_temperature, state=state, template=template)
+    NOTE(Jules): Warning : average temperature by functional group (because of daily vertical migration) and not by
+    layer. We therefore have a function with a high cost in terms of computation and memory space.
+
+    """
+    average_temperature = check_units(
+        state[ForcingLabels.avg_temperature_by_fgroup], StandardUnitsLabels.temperature.units
+    )
+    min_temperature = check_units(state[ForcingLabels.min_temperature], StandardUnitsLabels.temperature.units)
+    return average_temperature >= min_temperature
 
 
-def average_temperature_template(chunk: dict | None = None) -> ForcingTemplate:
+def mask_temperature_template(chunk: dict | None = None) -> ForcingTemplate:
     return ForcingTemplate(
-        name=ForcingLabels.avg_temperature_by_fgroup,
-        dims=[CoordinatesLabels.functional_group, CoordinatesLabels.time, CoordinatesLabels.Y, CoordinatesLabels.X],
-        attrs=average_temperature_by_fgroup_desc,
+        name=ForcingLabels.mask_temperature,
+        dims=[
+            CoordinatesLabels.functional_group,
+            CoordinatesLabels.time,
+            CoordinatesLabels.Y,
+            CoordinatesLabels.X,
+            CoordinatesLabels.cohort,
+        ],
+        attrs=mask_temperature_desc,
         chunks=chunk,
     )
 
 
-def average_temperature_kernel(*, chunk: dict | None = None, template: ForcingTemplate | None = None) -> KernelUnits:
+def mask_temperature_kernel(*, chunk: dict | None = None, template: ForcingTemplate | None = None) -> KernelUnits:
     if template is None:
-        template = average_temperature_template(chunk=chunk)
+        template = mask_temperature_template(chunk=chunk)
     return KernelUnits(
-        name=ForcingLabels.avg_temperature_by_fgroup,
+        name=ForcingLabels.mask_temperature,
         template=template,
-        function=_average_temperature,
+        function=_mask_temperature_helper,
     )
```

### Comparing `seapopym-0.0.1.1/seapopym/function/generator/biomass/biomass.py` & `seapopym-0.0.1.3/seapopym/function/generator/biomass/biomass.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,52 +9,39 @@
 import xarray as xr
 
 from seapopym.function.core.kernel import KernelUnits
 from seapopym.function.core.template import ForcingTemplate
 from seapopym.function.generator.biomass.compiled_functions import biomass_sequence
 from seapopym.standard.attributs import biomass_desc
 from seapopym.standard.labels import ConfigurationLabels, CoordinatesLabels, ForcingLabels
+from seapopym.standard.types import SeapopymForcing
 
 
 def _biomass_helper(state: xr.Dataset) -> xr.DataArray:
     """Wrap the biomass computation arround the Numba function `biomass_sequence`."""
 
-    def _format_fields(state: xr.Dataset) -> xr.Dataset:
+    def _format_fields(forcing: SeapopymForcing) -> SeapopymForcing:
         """Format the fields to be used in the biomass computation."""
-        return np.nan_to_num(state.data, 0.0).astype(np.float64)
+        return np.nan_to_num(forcing.data, 0.0).astype(np.float64)
 
-    state = state.cf.transpose(*CoordinatesLabels.ordered(), missing_dims="ignore")
-    recruited = state[ForcingLabels.recruited].sum(CoordinatesLabels.cohort)
-    recruited = _format_fields(recruited)
+    state = CoordinatesLabels.order_data(state)
+    recruited = _format_fields(state[ForcingLabels.recruited])
     mortality = _format_fields(state[ForcingLabels.mortality_field])
     if ConfigurationLabels.initial_condition_biomass in state:
         initial_conditions = _format_fields(state[ConfigurationLabels.initial_condition_biomass])
     else:
         initial_conditions = None
-
     biomass = biomass_sequence(recruited=recruited, mortality=mortality, initial_conditions=initial_conditions)
-
     return xr.DataArray(
         dims=state[ForcingLabels.mortality_field].dims,
         coords=state[ForcingLabels.mortality_field].coords,
         data=biomass,
     )
 
 
-# def biomass(state: xr.Dataset, chunk: dict | None = None) -> xr.DataArray:
-#     """Wrap the biomass cumputation with a map_block function."""
-#     template = Template(
-#         name=ForcingLabels.biomass,
-#         dims=[CoordinatesLabels.functional_group, CoordinatesLabels.time, CoordinatesLabels.Y, CoordinatesLabels.X],
-#         attributs=biomass_desc,
-#         chunks=chunk,
-#     )
-#     return apply_map_block(function=_biomass_helper, state=state, template=template)
-
-
 def biomass_template(chunk: dict | None = None) -> ForcingTemplate:
     return ForcingTemplate(
         name=ForcingLabels.biomass,
         dims=[CoordinatesLabels.functional_group, CoordinatesLabels.time, CoordinatesLabels.Y, CoordinatesLabels.X],
         attrs=biomass_desc,
         chunks=chunk,
     )
```

### Comparing `seapopym-0.0.1.1/seapopym/function/generator/biomass/compiled_functions.py` & `seapopym-0.0.1.3/seapopym/function/generator/biomass/compiled_functions.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/function/generator/cell_area.py` & `seapopym-0.0.1.3/seapopym/function/generator/cell_area.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/function/generator/day_length.py` & `seapopym-0.0.1.3/seapopym/function/generator/day_length.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/function/generator/mask.py` & `seapopym-0.0.1.3/seapopym/function/generator/mask.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/function/generator/mask_temperature.py` & `seapopym-0.0.1.3/seapopym/function/generator/mortality_field.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,62 @@
 """A temperature mask computation wrapper. Use xarray.map_block."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import cf_xarray  # noqa: F401
+import numpy as np
 
 from seapopym.function.core.kernel import KernelUnits
 from seapopym.function.core.template import ForcingTemplate
-from seapopym.standard.attributs import mask_temperature_desc
-from seapopym.standard.labels import CoordinatesLabels, ForcingLabels
+from seapopym.standard.attributs import mortality_field_desc
+from seapopym.standard.labels import ConfigurationLabels, CoordinatesLabels, ForcingLabels
 from seapopym.standard.units import StandardUnitsLabels, check_units
 
 if TYPE_CHECKING:
     import xarray as xr
 
 
-def _mask_temperature_helper(state: xr.Dataset) -> xr.DataArray:
+def _mortality_field_helper(state: xr.Dataset) -> xr.DataArray:
     """
-    It uses the min_temperature.
+    Use the relation between temperature and mortality to generate the mortality field.
 
     Depend on
     ---------
-    - min_temperature()
     - average_temperature()
 
     Input
-    -----
-    - min_temperature [cohort_age]
+    ------
     - average_temperature [functional_group, time, latitude, longitude]
+    - inv_lambda_max [functional_group]
+    - inv_lambda_rate [functional_group]
 
     Output
     ------
-    - mask_temperature_by_cohort_by_functional_group [functional_group, time, latitude, longitude, cohort_age]
-
-    NOTE(Jules): Warning : average temperature by functional group (because of daily vertical migration) and not by
-    layer. We therefore have a function with a high cost in terms of computation and memory space.
-
+    - mortality_field [functional_group, time, latitude, longitude]
     """
-    average_temperature = check_units(
-        state[ForcingLabels.avg_temperature_by_fgroup], StandardUnitsLabels.temperature.units
-    )
-    min_temperature = check_units(state[ForcingLabels.min_temperature], StandardUnitsLabels.temperature.units)
-    return average_temperature >= min_temperature
+    average_temperature = state[ForcingLabels.avg_temperature_by_fgroup]
+    inv_lambda_max = state[ConfigurationLabels.inv_lambda_max]
+    inv_lambda_rate = state[ConfigurationLabels.inv_lambda_rate]
+    timestep = state[ConfigurationLabels.timestep]
+
+    average_temperature = check_units(average_temperature, StandardUnitsLabels.temperature)
+    return np.exp(-timestep * (np.exp(inv_lambda_rate * average_temperature) / inv_lambda_max))
 
 
-def mask_temperature_template(chunk: dict | None = None) -> ForcingTemplate:
+def mortality_field_template(chunk: dict | None = None) -> ForcingTemplate:
     return ForcingTemplate(
-        name=ForcingLabels.mask_temperature,
-        dims=[
-            CoordinatesLabels.functional_group,
-            CoordinatesLabels.time,
-            CoordinatesLabels.Y,
-            CoordinatesLabels.X,
-            CoordinatesLabels.cohort,
-        ],
-        attrs=mask_temperature_desc,
+        name=ForcingLabels.mortality_field,
+        dims=[CoordinatesLabels.functional_group, CoordinatesLabels.time, CoordinatesLabels.Y, CoordinatesLabels.X],
+        attrs=mortality_field_desc,
         chunks=chunk,
     )
 
 
-def mask_temperature_kernel(*, chunk: dict | None = None, template: ForcingTemplate | None = None) -> KernelUnits:
+def mortality_field_kernel(*, chunk: dict | None = None, template: ForcingTemplate | None = None) -> KernelUnits:
     if template is None:
-        template = mask_temperature_template(chunk=chunk)
+        template = mortality_field_template(chunk=chunk)
     return KernelUnits(
-        name=ForcingLabels.mask_temperature,
+        name=ForcingLabels.mortality_field,
         template=template,
-        function=_mask_temperature_helper,
+        function=_mortality_field_helper,
     )
```

### Comparing `seapopym-0.0.1.1/seapopym/function/generator/min_temperature.py` & `seapopym-0.0.1.3/seapopym/function/generator/min_temperature.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
     Output
     ------
     - min_temperature [functional_group, cohort_age] : a datarray with cohort_age as coordinate and
     minimum temperature as value.
     """
     return (
-        np.log(state[ConfigurationLabels.mean_timestep] / state[ForcingLabels.temperature_recruitment_max])
-        / state[ForcingLabels.temperature_recruitment_rate]
+        np.log(state[ConfigurationLabels.mean_timestep] / state[ConfigurationLabels.temperature_recruitment_max])
+        / state[ConfigurationLabels.temperature_recruitment_rate]
     )
 
 
 def min_temperature_template(chunk: dict | None = None) -> ForcingTemplate:
     return ForcingTemplate(
         name=ForcingLabels.min_temperature,
         dims=[CoordinatesLabels.functional_group, CoordinatesLabels.cohort],
```

### Comparing `seapopym-0.0.1.1/seapopym/function/generator/mortality_field.py` & `seapopym-0.0.1.3/seapopym/function/generator/average_temperature.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,66 @@
-"""A temperature mask computation wrapper. Use xarray.map_block."""
+"""An average temperature by fgroup computation wrapper. Use xarray.map_block."""
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
-
 import cf_xarray  # noqa: F401
-import numpy as np
+import xarray as xr
 
 from seapopym.function.core.kernel import KernelUnits
 from seapopym.function.core.template import ForcingTemplate
-from seapopym.standard.attributs import mortality_field_desc
+from seapopym.standard.attributs import average_temperature_by_fgroup_desc
 from seapopym.standard.labels import ConfigurationLabels, CoordinatesLabels, ForcingLabels
 from seapopym.standard.units import StandardUnitsLabels, check_units
 
-if TYPE_CHECKING:
-    import xarray as xr
-
 
-def _mortality_field_helper(state: xr.Dataset) -> xr.DataArray:
+def _average_temperature(state: xr.Dataset) -> xr.DataArray:
     """
-    Use the relation between temperature and mortality to generate the mortality field.
-
-    Depend on
-    ---------
-    - average_temperature()
+    Depend on:
+    - compute_daylength
+    - mask_by_fgroup.
 
     Input
-    ------
-    - average_temperature [functional_group, time, latitude, longitude]
-    - inv_lambda_max [functional_group]
-    - inv_lambda_rate [functional_group]
+    -----
+    - mask_by_fgroup()      [time, latitude, longitude]
+    - compute_daylength()   [functional_group, latitude, longitude] in day
+    - day/night_layer       [functional_group]
+    - temperature           [time, latitude, longitude, layer] in degC
 
     Output
     ------
-    - mortality_field [functional_group, time, latitude, longitude]
+    - avg_temperature [functional_group, time, latitude, longitude] in degC
     """
-    average_temperature = state[ForcingLabels.avg_temperature_by_fgroup]
-    inv_lambda_max = state[ConfigurationLabels.inv_lambda_max]
-    inv_lambda_rate = state[ConfigurationLabels.inv_lambda_rate]
-    timestep = state[ConfigurationLabels.timestep]
+    temperature = check_units(state[ForcingLabels.temperature], StandardUnitsLabels.temperature.units)
+    day_length = check_units(state[ForcingLabels.day_length], StandardUnitsLabels.time.units)
+    mask_by_fgroup = state[ForcingLabels.mask_by_fgroup]
+    day_layer = state[ConfigurationLabels.day_layer]
+    night_layer = state[ConfigurationLabels.night_layer]
+
+    average_temperature = []
+    for fgroup in day_layer[CoordinatesLabels.functional_group]:
+        day_temperature = temperature.cf.sel(Z=day_layer.sel({CoordinatesLabels.functional_group: fgroup}))
+        night_temperature = temperature.cf.sel(Z=night_layer.sel({CoordinatesLabels.functional_group: fgroup}))
+        mean_temperature = (day_length * day_temperature) + ((1 - day_length) * night_temperature)
+        if "Z" in mean_temperature.cf:
+            mean_temperature = mean_temperature.cf.drop_vars("Z")
+        mean_temperature = mean_temperature.where(mask_by_fgroup.sel({CoordinatesLabels.functional_group: fgroup}))
+        average_temperature.append(mean_temperature)
 
-    average_temperature = check_units(average_temperature, StandardUnitsLabels.temperature)
-    return np.exp(-timestep * (np.exp(inv_lambda_rate * average_temperature) / inv_lambda_max))
+    return xr.concat(average_temperature, dim=CoordinatesLabels.functional_group.value)
 
 
-def mortality_field_template(chunk: dict | None = None) -> ForcingTemplate:
+def average_temperature_template(chunk: dict | None = None) -> ForcingTemplate:
     return ForcingTemplate(
-        name=ForcingLabels.mortality_field,
+        name=ForcingLabels.avg_temperature_by_fgroup,
         dims=[CoordinatesLabels.functional_group, CoordinatesLabels.time, CoordinatesLabels.Y, CoordinatesLabels.X],
-        attrs=mortality_field_desc,
+        attrs=average_temperature_by_fgroup_desc,
         chunks=chunk,
     )
 
 
-def mortality_field_kernel(*, chunk: dict | None = None, template: ForcingTemplate | None = None) -> KernelUnits:
+def average_temperature_kernel(*, chunk: dict | None = None, template: ForcingTemplate | None = None) -> KernelUnits:
     if template is None:
-        template = mortality_field_template(chunk=chunk)
+        template = average_temperature_template(chunk=chunk)
     return KernelUnits(
-        name=ForcingLabels.mortality_field,
+        name=ForcingLabels.avg_temperature_by_fgroup,
         template=template,
-        function=_mortality_field_helper,
+        function=_average_temperature,
     )
```

### Comparing `seapopym-0.0.1.1/seapopym/function/generator/production/production.py` & `seapopym-0.0.1.3/seapopym/function/generator/production/production.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 """
 This module contains the function used to compute the recruited population in  the NotTransport model.
 They are run in sequence in timeseries order.
 """
 
 from __future__ import annotations
 
+from typing import Iterable
+
 import cf_xarray  # noqa: F401
 import numpy as np
 import xarray as xr
 
 from seapopym.function.core.kernel import KernelUnits
 from seapopym.function.core.template import ForcingTemplate, StateTemplate
-from seapopym.function.generator.production.compiled_functions import time_loop
-from seapopym.logging.custom_logger import logger
+from seapopym.function.generator.production.compiled_functions import (
+    production,
+    production_export_initial,
+    production_export_preproduction,
+)
 from seapopym.standard.attributs import preproduction_desc, recruited_desc
 from seapopym.standard.labels import ConfigurationLabels, CoordinatesLabels, ForcingLabels
-from seapopym.standard.types import SeapopymForcing
+from seapopym.standard.types import SeapopymDims, SeapopymForcing, SeapopymState
+
+PRODUCTION_DIMS = [CoordinatesLabels.time, CoordinatesLabels.Y, CoordinatesLabels.X]
+INITIAL_CONDITION_DIMS = [CoordinatesLabels.Y, CoordinatesLabels.X, CoordinatesLabels.cohort]
+PREPRODUCTION_DIMS = [CoordinatesLabels.time, CoordinatesLabels.Y, CoordinatesLabels.X, CoordinatesLabels.cohort]
 
 
-def _init_forcing(fgroup_data: xr.Dataset, export_preproduction: np.ndarray | None) -> dict[str, np.ndarray]:
+def _production_helper_init_forcing(fgroup_data: xr.Dataset) -> dict[str, np.ndarray]:
     """Initialise the forcing data used in the Numba function that compute production."""
 
     def standardize_forcing(forcing: xr.DataArray, nan: object = 0.0, dtype: type = np.float64) -> np.ndarray:
         """Refer to Numba documentation about array typing."""
         return np.nan_to_num(x=forcing.data, nan=nan).astype(dtype)
 
     if ConfigurationLabels.initial_condition_production not in fgroup_data:
         initial_condition = None
     else:
         initial_condition = standardize_forcing(fgroup_data[ConfigurationLabels.initial_condition_production])
-    # TODO(Jules): Use standard labels instead of strings
-    return {
+    return {  # NOTE(Jules): the keys correspond to the parameters of the numba functions
         "primary_production": standardize_forcing(fgroup_data[ForcingLabels.primary_production_by_fgroup]),
         "mask_temperature": standardize_forcing(fgroup_data[ForcingLabels.mask_temperature]),
         "timestep_number": standardize_forcing(fgroup_data[ConfigurationLabels.timesteps_number], False, bool),
         "initial_production": initial_condition,
-        "export_preproduction": export_preproduction,
     }
 
 
-def _format_output(
-    fgroup_data: xr.Dataset, data: np.ndarray, *, export_preproduction: np.ndarray | None = None
-) -> xr.DataArray:
+def _production_helper_format_output(
+    fgroup_data: SeapopymState, dims: Iterable[SeapopymDims], data: np.ndarray
+) -> SeapopymForcing:
     """Convert the output of the Numba function to a DataArray."""
-    template = fgroup_data[ForcingLabels.mask_temperature]
-    if export_preproduction is not None:
-        template = template.cf.isel(T=export_preproduction)
-    return xr.DataArray(coords=template.coords, dims=template.dims, data=data)
+    coords = {fgroup_data.cf[dim_name].name: fgroup_data.cf[dim_name] for dim_name in dims}
+    formated_data = xr.DataArray(coords=coords, dims=coords.keys())
+    formated_data = CoordinatesLabels.order_data(formated_data)
+    formated_data.data = data
+    return formated_data
 
 
-def _production_helper(data: xr.Dataset, *, export_preproduction: np.ndarray | None = None) -> xr.DataArray:
+def _production_helper(
+    data: SeapopymState,
+    *,
+    export_preproduction: bool = False,
+    export_initial_production: bool = False,
+) -> SeapopymState:
     """
     Compute the production using a numba jit function.
 
     Parameters
     ----------
     data : xr.Dataset
         The input dataset.
@@ -65,141 +78,86 @@
     -------
     output : xr.Dataset
         The output dataset.
 
     """
     data = data.cf.transpose(*CoordinatesLabels.ordered(), missing_dims="ignore")
     results_recruited = []
-    if export_preproduction is not None:
-        results_preproduction = []
+    if export_preproduction or export_initial_production:
+        results_extra = []
 
     for fgroup in data[CoordinatesLabels.functional_group]:
-        logger.info(f"Computing production for Cohort {int(fgroup)}")
-
         fgroup_data = data.sel({CoordinatesLabels.functional_group: fgroup}).dropna(CoordinatesLabels.cohort)
-        output_recruited, output_preproduction = time_loop(**_init_forcing(fgroup_data, export_preproduction))
+        param = _production_helper_init_forcing(fgroup_data)
 
-        results_recruited.append(_format_output(fgroup_data, output_recruited))
-        if export_preproduction is not None:
-            results_preproduction.append(
-                _format_output(fgroup_data, output_preproduction, export_preproduction=export_preproduction)
-            )
-
-    results = {ForcingLabels.recruited: xr.concat(results_recruited, dim=CoordinatesLabels.functional_group)}
-    if export_preproduction is not None:
-        results[ForcingLabels.preproduction] = xr.concat(results_preproduction, dim=CoordinatesLabels.functional_group)
+        if export_preproduction:
+            output_recruited, output_extra = production_export_preproduction(**param)
+            results_extra.append(_production_helper_format_output(fgroup_data, PREPRODUCTION_DIMS, output_extra))
+
+        # NOTE(Jules):  Implicite -> if both are True then export_preproduction  PREPRODUCTION_DIMSis prioritized
+        #               because init is included
+        elif export_initial_production:
+            output_recruited, output_extra = production_export_initial(**param)
+            results_extra.append(_production_helper_format_output(fgroup_data, INITIAL_CONDITION_DIMS, output_extra))
+
+        else:
+            output_recruited = production(**param)
+
+        results_recruited.append(_production_helper_format_output(fgroup_data, PRODUCTION_DIMS, output_recruited))
+    results = {ForcingLabels.recruited: xr.concat(results_recruited, dim=data[CoordinatesLabels.functional_group])}
+    if export_preproduction or export_initial_production:
+        results[ForcingLabels.preproduction] = xr.concat(results_extra, dim=data[CoordinatesLabels.functional_group])
     return xr.Dataset(results)
 
 
-# def production(
-#     state: xr.Dataset,
-#     chunk: dict[str, int | Literal["auto"]] | None = None,
-#     *,
-#     export_preproduction: np.ndarray | None = None,
-# ) -> xr.Dataset:
-#     """
-#     The main fonction to compute the production. It is a wrapper around the `compute_preproduction_numba` function.
-
-#     Parameters
-#     ----------
-#     state : xr.Dataset
-#         The input dataset.
-#     chunk : dict[str, int | Literal["auto"]] | None
-#         The chunk size for the computation. If None, the default chunk size is used {CoordinatesLabels.functional_group: 1}.
-#     export_preproduction : np.ndarray | None
-#         An array (dtype=int) containing the time-index (i.e. timestamps) to export the pre-production. If None, the
-#         pre-production is not exported.
-
-#     Returns
-#     -------
-#     output : xr.Dataset
-#         The output dataset.
-
-#     Warning:
-#     --------
-#     - Valide chunk keys are : `{CoordinatesLabels.functional_group:..., "X":..., "Y":...}`. Priority should be given to
-#     the functional group dimension.
-
-#     """
-#     template = []
-#     template_recruited = Template(
-#         name=ForcingLabels.recruited,
-#         dims=(
-#             CoordinatesLabels.functional_group,
-#             CoordinatesLabels.time,
-#             CoordinatesLabels.Y,
-#             CoordinatesLabels.X,
-#             CoordinatesLabels.cohort,
-#         ),
-#         attributs=recruited_desc,
-#         chunks=chunk,
-#     )
-#     template.append(template_recruited)
-
-#     if export_preproduction is not None:
-#         template_preprod = Template(
-#             name=ForcingLabels.preproduction,
-#             dims=(
-#                 CoordinatesLabels.functional_group,
-#                 (CoordinatesLabels.time, state.cf["T"].cf.isel(T=export_preproduction)),
-#                 CoordinatesLabels.Y,
-#                 CoordinatesLabels.X,
-#                 CoordinatesLabels.cohort,
-#             ),
-#             attributs=preproduction_desc,
-#             chunks=chunk,
-#         )
-#         template.append(template_preprod)
-
-#     return apply_map_block(
-#         function=_production_helper, state=state, template=template, export_preproduction=export_preproduction
-#     )
-
-
 def production_template(
-    chunk: dict | None = None, preproduction_time_coords: SeapopymForcing | None = None
+    chunk: dict | None = None,
+    *,
+    export_preproduction: bool = False,
+    export_initial_production: bool = False,
 ) -> StateTemplate:
     template_recruited = ForcingTemplate(
         name=ForcingLabels.recruited,
-        dims=(
-            CoordinatesLabels.functional_group,
-            CoordinatesLabels.time,
-            CoordinatesLabels.Y,
-            CoordinatesLabels.X,
-            CoordinatesLabels.cohort,
-        ),
+        dims=[CoordinatesLabels.functional_group, *PRODUCTION_DIMS],
         attrs=recruited_desc,
         chunks=chunk,
     )
-    if preproduction_time_coords is not None:
+    if export_preproduction:
         template_preprod = ForcingTemplate(
             name=ForcingLabels.preproduction,
-            dims=(
-                CoordinatesLabels.functional_group,
-                preproduction_time_coords,
-                CoordinatesLabels.Y,
-                CoordinatesLabels.X,
-                CoordinatesLabels.cohort,
-            ),
+            dims=[CoordinatesLabels.functional_group, *PREPRODUCTION_DIMS],
             attrs=preproduction_desc,
             chunks=chunk,
         )
         return StateTemplate(template=[template_recruited, template_preprod])
 
+    if export_initial_production:
+        template_init = ForcingTemplate(
+            name=ForcingLabels.preproduction,
+            dims=[CoordinatesLabels.functional_group, *INITIAL_CONDITION_DIMS],
+            attrs=preproduction_desc,
+            chunks=chunk,
+        )
+        return StateTemplate(template=[template_recruited, template_init])
+
     return StateTemplate(template=[template_recruited])
 
 
 def production_kernel(
     *,
-    chunk: dict | None = None,
     template: StateTemplate | None = None,
-    preproduction_time_coords: SeapopymForcing | None = None,
-    preproduction_time_index: np.ndarray | None = None,
+    chunk: dict | None = None,
+    export_preproduction: bool = False,
+    export_initial_production: bool = False,
 ) -> KernelUnits:
+    kwargs = {
+        "export_preproduction": export_preproduction,
+        "export_initial_production": export_initial_production,
+    }
     if template is None:
-        template = production_template(chunk=chunk, preproduction_time_coords=preproduction_time_coords)
+        template = production_template(chunk=chunk, **kwargs)
     return KernelUnits(
         name="production",
         template=template,
         function=_production_helper,
-        kwargs={"export_preproduction": preproduction_time_index},
+        kwargs=kwargs,
     )
```

### Comparing `seapopym-0.0.1.1/seapopym/logging/custom_logger.py` & `seapopym-0.0.1.3/seapopym/logging/custom_logger.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/model/base_model.py` & `seapopym-0.0.1.3/seapopym/model/base_model.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/model/no_transport_model.py` & `seapopym-0.0.1.3/seapopym/model/no_transport_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,116 +1,100 @@
 """The LMTL model without ADRE equations."""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-import numpy as np
-
 from seapopym.function import generator
 from seapopym.function.core.kernel import Kernel
 from seapopym.function.generator.mask import apply_mask_to_state
 from seapopym.logging.custom_logger import logger
 from seapopym.model.base_model import BaseModel
 from seapopym.plotter import base_functions as pfunctions
 from seapopym.standard.coordinates import reorder_dims
+from seapopym.standard.types import SeapopymState
 from seapopym.writer import base_functions as wfunctions
 
 if TYPE_CHECKING:
-    import xarray as xr
     from dask.distributed import Client
 
     from seapopym.configuration.no_transport.configuration import NoTransportConfiguration
 
 
 class NoTransportModel(BaseModel):
     """Implement the LMTL model without the transport (Advection-Diffusion)."""
 
     def __init__(self: NoTransportModel, configuration: NoTransportConfiguration) -> None:
         """The constructor of the model allows the user to overcome the default parameters and client behaviors."""
         self._configuration = configuration
         self.state = apply_mask_to_state(reorder_dims(configuration.model_parameters))
 
-    @property
-    def configuration(self: NoTransportModel) -> NoTransportConfiguration:
-        """The configuration getter."""
-        return self._configuration
-
-    @property
-    def client(self: NoTransportModel) -> Client | None:
-        """The dask Client getter."""
-        return self._configuration.environment_parameters.client.client
-
-    # TODO(Jules): Include angle_horizon_sun in the configuration. Then kernel will be a property.
-    def kernel(self: NoTransportModel, angle_horizon_sun: float = 0) -> Kernel:
-        """The kernel getter."""
-
-        def _preproduction_converter() -> tuple[np.ndarray, xr.DataArray] | tuple[None, None]:
-            """
-            The production process requires a specific format, we then convert parameters to a np.ndarray that contains
-            the indices of the timestamps to export. None is returned if no timestamps are provided.
-            """
-            if self.configuration.environment_parameters.output.pre_production is None:
-                return (None, None)
-
-            timestamps = self.configuration.environment_parameters.output.pre_production.timestamps
-            data = self.state.cf["T"]
-
-            if timestamps is None:
-                return (None, None)
-            if timestamps == "all":
-                return (np.arange(data.size), data.cf["T"])
-            if np.all([isinstance(x, int) for x in timestamps]):
-                selected_dates = data.cf.isel(T=timestamps)
-            elif np.all([isinstance(x, str) for x in timestamps]):
-                selected_dates = data.cf.sel(T=timestamps, method="nearest")
-            else:
-                msg = "The timestamps must be either 'all', a list of integers or a list of strings."
-                raise TypeError(msg)
-            index = np.arange(data.size)[data.isin(selected_dates)]
-            coords = data.cf.isel(T=index)
-            return (index, coords)
-
-        preproduction_time_index, preproduction_time_coords = _preproduction_converter()
-
         chunk = self.configuration.environment_parameters.chunk.as_dict()
 
-        return Kernel(
+        self._kernel = Kernel(
             [
                 generator.global_mask_kernel(chunk=chunk),
                 generator.mask_by_fgroup_kernel(chunk=chunk),
-                generator.day_length_kernel(chunk=chunk, angle_horizon_sun=angle_horizon_sun),
+                generator.day_length_kernel(
+                    chunk=chunk, angle_horizon_sun=configuration.kernel_parameters.angle_horizon_sun
+                ),
                 generator.average_temperature_kernel(chunk=chunk),
                 generator.apply_coefficient_to_primary_production_kernel(chunk=chunk),
                 generator.min_temperature_kernel(chunk=chunk),
                 generator.mask_temperature_kernel(chunk=chunk),
                 generator.cell_area_kernel(chunk=chunk),
                 generator.mortality_field_kernel(chunk=chunk),
                 generator.production_kernel(
                     chunk=chunk,
-                    preproduction_time_coords=preproduction_time_coords,
-                    preproduction_time_index=preproduction_time_index,
+                    export_preproduction=configuration.kernel_parameters.compute_preproduction,
+                    export_initial_production=configuration.kernel_parameters.compute_initial_conditions,
                 ),
                 generator.biomass_kernel(chunk=chunk),
             ]
         )
 
+    @property
+    def configuration(self: NoTransportModel) -> NoTransportConfiguration:
+        """The configuration getter."""
+        return self._configuration
+
+    @property
+    def client(self: NoTransportModel) -> Client | None:
+        """The dask Client getter."""
+        return self._configuration.environment_parameters.client.client
+
+    @property
+    def kernel(self: NoTransportModel) -> Kernel:
+        """The kernel getter."""
+        return self._kernel
+
+    @property
+    def template(self: NoTransportModel) -> SeapopymState:
+        """The template getter."""
+        return self.kernel.template(self.state)
+
+    @property
+    def expected_memory_usage(self: NoTransportModel) -> int:
+        """The expected memory usage getter."""
+        return f"The expected memory usage is {self.template.nbytes / 1e6:.2f} MB."
+
     def initialize_dask(self: NoTransportModel) -> None:
         """Initialize the client and configure the model to run in distributed mode."""
         logger.info("Initializing the client.")
         self.configuration.environment_parameters.client.initialize_client()
         chunk = self.configuration.environment_parameters.chunk.as_dict()
         self.state = self.state.chunk(chunk)
         logger.info("Scattering the data to the workers.")
         self.client.scatter(self.state)
 
     def run(self: NoTransportModel) -> None:
         """Run the model. Wrapper of the pre-production, production and post-production processes."""
-        self.state = self.kernel().run(self.state)
-        self.state.persist()
+        self.state = self.kernel.run(self.state)
+        if self.client is not None:
+            self.client.persist(self.state)
 
     def close(self: NoTransportModel) -> None:
         """Clean up the system. For example, it can be used to close dask.Client."""
         self.configuration.environment_parameters.client.close_client()
 
     # --- Export functions --- #
```

### Comparing `seapopym-0.0.1.1/seapopym/plotter/base_functions.py` & `seapopym-0.0.1.3/seapopym/plotter/base_functions.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/standard/attributs.py` & `seapopym-0.0.1.3/seapopym/standard/attributs.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/standard/coordinates.py` & `seapopym-0.0.1.3/seapopym/standard/coordinates.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/standard/labels.py` & `seapopym-0.0.1.3/seapopym/standard/labels.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/standard/types.py` & `seapopym-0.0.1.3/seapopym/standard/types.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/standard/units.py` & `seapopym-0.0.1.3/seapopym/standard/units.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.1/seapopym/writer/base_functions.py` & `seapopym-0.0.1.3/seapopym/writer/base_functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from pathlib import Path
 from typing import TYPE_CHECKING, Literal
 
 import xarray as xr
 
 from seapopym.standard.labels import ConfigurationLabels, ForcingLabels
+from seapopym.standard.types import SeapopymForcing, SeapopymState
 
 if TYPE_CHECKING:
     from seapopym.model.no_transport_model import NoTransportModel
 
 
 def _helper_export_data(
     data: xr.Dataset,
@@ -59,43 +60,58 @@
     _helper_check_state(model)
 
     _helper_export_data(model.state, path, engine, mode)
 
 
 def export_initial_conditions(
     model: NoTransportModel,
-    path: str | Path,
+    path: str | Path | None = None,
     engine: Literal["zarr", "netcdf"] = "zarr",
     mode: Literal["w", "a"] = "w",
-) -> None:
+) -> SeapopymState | None:
     """Export the initial conditions to a file."""
     _helper_check_state(model)
     if ForcingLabels.preproduction not in model.state:
         msg = "The model does not have production to export."
         raise ValueError(msg)
     if ForcingLabels.biomass not in model.state:
         msg = "The model does not have biomass to export."
         raise ValueError(msg)
 
+    if "T" in model.state[ForcingLabels.preproduction].cf.coords:
+        # NOTE(Jules): if production_export_preproduction have been used
+        init_prod = model.state[ForcingLabels.preproduction].cf.isel(T=-1)
+    else:
+        # NOTE(Jules): if production_export_initial have been used
+        init_prod = model.state[ForcingLabels.preproduction]
+
     data_to_export = xr.Dataset(
         {
-            ConfigurationLabels.initial_condition_production: model.state[ForcingLabels.preproduction].cf.isel(T=-1),
+            ConfigurationLabels.initial_condition_production: init_prod,
             ConfigurationLabels.initial_condition_biomass: model.state[ForcingLabels.biomass].cf.isel(T=-1),
         }
     )
 
+    if path is None:
+        return data_to_export
+
     _helper_export_data(data_to_export, path, engine, mode)
+    return None
 
 
 def export_biomass(
     model: NoTransportModel,
-    path: str | Path,
+    path: str | Path | None = None,
     engine: Literal["zarr", "netcdf"] = "zarr",
     mode: Literal["w", "a"] = "w",
-) -> None:
+) -> SeapopymForcing | None:
     """Export the biomass to a file."""
     _helper_check_state(model)
     if ForcingLabels.biomass not in model.state:
         msg = "The model does not have biomass to export."
         raise ValueError(msg)
 
+    if path is None:
+        return model.state[ForcingLabels.biomass]
+
     _helper_export_data(model.state[ForcingLabels.biomass], path, engine, mode)
+    return None
```

