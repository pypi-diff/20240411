# Comparing `tmp/geo_parameters-0.1.1.tar.gz` & `tmp/geo_parameters-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_parameters-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geo_parameters-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geo_parameters-0.1.1.tar` & `geo_parameters-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1776 2024-04-05 14:06:58.740313 geo_parameters-0.1.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0     3140 2024-04-05 14:06:58.740313 geo_parameters-0.1.1/.gitignore
--rw-r--r--   0        0        0     1079 2024-04-05 14:06:58.740313 geo_parameters-0.1.1/LICENSE
--rw-r--r--   0        0        0     3646 2024-04-05 14:06:58.740313 geo_parameters-0.1.1/README.md
--rw-r--r--   0        0        0       91 2024-04-05 14:06:58.740313 geo_parameters-0.1.1/environment.yml
--rw-r--r--   0        0        0       90 2024-04-05 14:06:58.740313 geo_parameters-0.1.1/geo_parameters/__init__.py
--rw-r--r--   0        0        0     2419 2024-04-05 14:06:58.740313 geo_parameters-0.1.1/geo_parameters/metaparameter.py
--rw-r--r--   0        0        0     1312 2024-04-05 14:06:58.740313 geo_parameters-0.1.1/geo_parameters/ocean.py
--rw-r--r--   0        0        0     1135 2024-04-05 14:06:58.744313 geo_parameters-0.1.1/geo_parameters/parameter_funcs.py
--rw-r--r--   0        0        0    10549 2024-04-05 14:06:58.744313 geo_parameters-0.1.1/geo_parameters/wave.py
--rw-r--r--   0        0        0     1417 2024-04-05 14:06:58.744313 geo_parameters-0.1.1/geo_parameters/wind.py
--rw-r--r--   0        0        0      450 2024-04-05 14:06:58.744313 geo_parameters-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 14:06:58.744313 geo_parameters-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1869 2024-04-05 14:06:58.744313 geo_parameters-0.1.1/tests/test_doc.py
--rw-r--r--   0        0        0     1020 2024-04-05 14:06:58.744313 geo_parameters-0.1.1/tests/test_funcs.py
--rw-r--r--   0        0        0      836 2024-04-05 14:06:58.744313 geo_parameters-0.1.1/tests/test_names.py
--rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 geo_parameters-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1776 2024-04-11 11:58:25.751571 geo_parameters-0.2.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3140 2024-04-11 11:58:25.751571 geo_parameters-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1079 2024-04-11 11:58:25.751571 geo_parameters-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3386 2024-04-11 11:58:25.751571 geo_parameters-0.2.1/README.md
+-rw-r--r--   0        0        0       91 2024-04-11 11:58:25.751571 geo_parameters-0.2.1/environment.yml
+-rw-r--r--   0        0        0       90 2024-04-11 11:58:25.751571 geo_parameters-0.2.1/geo_parameters/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-11 11:58:25.751571 geo_parameters-0.2.1/geo_parameters/grid.py
+-rw-r--r--   0        0        0     1967 2024-04-11 11:58:25.751571 geo_parameters-0.2.1/geo_parameters/metaparameter.py
+-rw-r--r--   0        0        0     1298 2024-04-11 11:58:25.751571 geo_parameters-0.2.1/geo_parameters/ocean.py
+-rw-r--r--   0        0        0     1124 2024-04-11 11:58:25.751571 geo_parameters-0.2.1/geo_parameters/parameter_funcs.py
+-rw-r--r--   0        0        0    10240 2024-04-11 11:58:25.751571 geo_parameters-0.2.1/geo_parameters/wave.py
+-rw-r--r--   0        0        0     1388 2024-04-11 11:58:25.751571 geo_parameters-0.2.1/geo_parameters/wind.py
+-rw-r--r--   0        0        0      450 2024-04-11 11:58:25.751571 geo_parameters-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 11:58:25.755571 geo_parameters-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1810 2024-04-11 11:58:25.755571 geo_parameters-0.2.1/tests/test_doc.py
+-rw-r--r--   0        0        0     1020 2024-04-11 11:58:25.755571 geo_parameters-0.2.1/tests/test_funcs.py
+-rw-r--r--   0        0        0      808 2024-04-11 11:58:25.755571 geo_parameters-0.2.1/tests/test_names.py
+-rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 geo_parameters-0.2.1/PKG-INFO
```

### Comparing `geo_parameters-0.1.1/.github/workflows/tests.yml` & `geo_parameters-0.2.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.1.1/.gitignore` & `geo_parameters-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.1.1/LICENSE` & `geo_parameters-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.1.1/README.md` & `geo_parameters-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,38 +11,32 @@
 
 These classes have information about the parameter:
 
 ```python
 Hs.standard_name()
 'sea_surface_wave_significant_height'
 ```
-Every parameters has a pre-defined short_name
+Every parameters has a pre-defined name
 
 ```python
-Hs.short_name()
+Hs.name
 'hs'
 ```
 If you want to define some other names for the parameters, then you can create an instance. By default the name of the instance is the short name, but this can be changed:
 
 ```python
 hsig = Hs()
-hsig.name()
+hsig.name
 'hs'
 
 hsig = Hs(name='hsig')
-hsig.name()
+hsig.name
 'hsig'
 ```
 
-The string value of an instant is also the name, so the instance can conveniently be used almost interchangeably with string identifiers
-
-```python
-assert str(Hs(name='hsig')) == str('hsig')
-```
-
 
 The instance still contains the standard name (and some long name that doesn't follow any standard):
 
 ```python
 hsig.standard_name() 
 'sea_surface_wave_significant_height'
 
@@ -103,19 +97,18 @@
 where the keywords define what string will serve as key in the dictonary (the value is always the parameter class).
 
 If an xarray Dataset has standard_name attributes, the correct key can be found using the class-method:
 
 ```python
 ds
 <xarray.Dataset> Size: 1kB
-Dimensions:              (lat: 11, lont: 6, lon: 6)
+Dimensions:              (lat: 11, lon: 6)
 Coordinates:
   * lon                  (lon) float64 48B 5.0 6.0 7.0 8.0 9.0 10.0
   * lat                  (lat) float64 88B 50.0 51.0 52.0 ... 58.0 59.0 60.0
-Dimensions without coordinates: lont
 Data variables:
     interesting_hs_name  (lat, lon) float64 528B 0.0 0.0 0.0 ... 0.0 0.0 0.0
     peak_period          (lat, lon) float64 528B 1.0 1.0 1.0 1.0 ... 1.0 1.0 1.0
 ```
 ```python
 ds.interesting_hs_name
 <xarray.DataArray 'interesting_hs_name' (lat: 11, lon: 6)> Size: 528B
```

### Comparing `geo_parameters-0.1.1/geo_parameters/metaparameter.py` & `geo_parameters-0.2.1/geo_parameters/metaparameter.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,15 @@
 from pint import Unit
 
 
 class MetaParameter(ABC):
     _cf = True
 
     def __init__(self, name: str = ""):
-        self._name = name or self.short_name()
-
-    @staticmethod
-    @abstractmethod
-    def _short_name() -> str:
-        pass
+        self.name = name or self.name
 
     @staticmethod
     @abstractmethod
     def _long_name() -> str:
         pass
 
     @staticmethod
@@ -31,18 +26,14 @@
         pass
 
     @classmethod
     def cf(cls) -> bool:
         return cls._cf
 
     @classmethod
-    def short_name(cls) -> str:
-        return cls._short_name
-
-    @classmethod
     def long_name(cls) -> str:
         return cls._long_name
 
     @classmethod
     def standard_name(cls, strict: bool = False, alias: bool = False) -> str:
         names = np.atleast_1d(cls._standard_name)
         if cls.cf() or not strict:
@@ -59,36 +50,25 @@
 
         return [""]
 
     @classmethod
     def unit(cls) -> Unit:
         return cls._unit
 
-    def __repr__(self):
-        return self.name()
-
     def quantify(self):
         return self * self.unit()
 
-    def set_name(self, name: str = None) -> None:
-        if name is None:
-            self._name = self.short_name()
-        self._name = name
-
-    def name(self) -> str:
-        return self._name or self.short_name()
-
     @classmethod
     def cf(cls) -> str:
         return cls._cf
 
     @classmethod
     def meta_dict(cls, alias: bool = False) -> dict:
         return {
-            "short_name": cls.short_name(),
+            "short_name": cls.name,
             "long_name": cls.long_name(),
             "standard_name": cls.standard_name(alias=alias),
             "unit": str(cls.unit()),
         }
 
     @classmethod
     def find_me_in_ds(cls, ds) -> Union[str, None]:
```

### Comparing `geo_parameters-0.1.1/geo_parameters/ocean.py` & `geo_parameters-0.2.1/geo_parameters/ocean.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 from .metaparameter import MetaParameter
 import pint
 
 ureg = pint.UnitRegistry()
 
+ureg.default_format = "~C"
+
 
 class WaterDepth(MetaParameter):
-    _short_name = "depth"
+    name = "depth"
     _long_name = "water_depth"
     _standard_name = "sea_floor_depth_below_sea_surface"
     _unit = ureg.m
 
+
 class SeaLevel(MetaParameter):
-    _short_name = "eta"
+    name = "eta"
     _long_name = "sea_surface_height"
     _standard_name = [
         "sea_surface_elevation",
         "sea_surface_elevation_anomaly",
         "sea_surface_height_above_geoid",
     ]
     _unit = ureg.m
 
 
 class XCurrent(MetaParameter):
-    _short_name = "x_current"
+    name = "x_current"
     _long_name = "eastward_current_component"
     _standard_name = [
         "sea_water_x_velocity",
         "x_sea_water_velocity",
     ]
     _unit = ureg.m / ureg.s
 
 
 class YCurrent(MetaParameter):
-    _short_name = "y_current"
+    name = "y_current"
     _long_name = "northward_current_component"
     _standard_name = [
         "sea_water_y_velocity",
         "y_sea_water_velocity",
     ]
     _unit = ureg.m / ureg.s
 
 
 class IceFraction(MetaParameter):
-    _short_name = "ice_fraction"
+    name = "ice_fraction"
     _long_name = "sea_ice_fraction"
     _standard_name = "sea_ice_area_fraction"
     _unit = ureg.percent
 
 
 class IceThickness(MetaParameter):
-    _short_name = "ice_thickness"
+    name = "ice_thickness"
     _long_name = "sea_ice_thickness"
     _standard_name = "sea_ice_thickness"
     _unit = ureg.m
-
```

### Comparing `geo_parameters-0.1.1/geo_parameters/parameter_funcs.py` & `geo_parameters-0.2.1/geo_parameters/parameter_funcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                 if issubclass(obj, MetaParameter) and not obj == MetaParameter:
                     parameter_list.append(obj)
     return parameter_list
 
 
 def dict_of_parameters(short: bool = False, alias: bool = False) -> dict:
     if short:
-        return {c.short_name(): c for c in list_of_parameters()}
+        return {c.name: c for c in list_of_parameters()}
     return {c.standard_name(alias=alias): c for c in list_of_parameters()}
 
 
 def get(key: str):
     return (
         dict_of_parameters().get(key)
         or dict_of_parameters(alias=True).get(key)
@@ -31,10 +31,7 @@
 def create_parameter_dict(parameter_strings: list[str]):
     metaparameter_dict = {}
     for param in parameter_strings:
         val = get(param)
         if val is not None:
             metaparameter_dict[param] = val
     return metaparameter_dict
-
-
-
```

### Comparing `geo_parameters-0.1.1/geo_parameters/wave.py` & `geo_parameters-0.2.1/geo_parameters/wave.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,384 +1,385 @@
 from .metaparameter import MetaParameter
 import pint
 
 ureg = pint.UnitRegistry()
+ureg.default_format = "~C"
 
 
 ## Wave heights
 class Hs(MetaParameter):
-    _short_name = "hs"
+    name = "hs"
     _long_name = "significant_wave_height"
     _standard_name = [
         "sea_surface_wave_significant_height",
         "significant_height_of_wind_and_swell_waves",
     ]
     _unit = ureg.m
 
 
 class HsSwell(MetaParameter):
-    _short_name = "hs_swell"
+    name = "hs_swell"
     _long_name = "significant_swell_height"
     _standard_name = [
         "sea_surface_swell_wave_significant_height",
         "significant_height_of_swell_waves",
     ]
     _unit = ureg.m
 
 
 class HsSwell1(MetaParameter):
-    _short_name = "hs_swell1"
+    name = "hs_swell1"
     _long_name = "significant_primary_swell_height"
     _standard_name = "sea_surface_primary_swell_wave_significant_height"
     _unit = ureg.m
 
 
 class HsSwell2(MetaParameter):
-    _short_name = "hs_swell12"
+    name = "hs_swell12"
     _long_name = "significant_secondary_swell_height"
     _standard_name = "sea_surface_secondary_swell_wave_significant_height"
     _unit = ureg.m
 
 
 class HsSwell3(MetaParameter):
-    _short_name = "hs_swell13"
+    name = "hs_swell13"
     _long_name = "significant_tertiary_swell_height"
     _standard_name = "sea_surface_tertiary_swell_wave_significant_height"
     _unit = ureg.m
 
 
 class HsSea(MetaParameter):
-    _short_name = "hs_sea"
+    name = "hs_sea"
     _long_name = "significant_wind_sea_height"
     _standard_name = [
         "sea_surface_wind_wave_significant_height",
         "significant_height_of_wind_waves",
     ]
     _unit = ureg.m
 
 
 class HsIG(MetaParameter):
-    _short_name = "hs_ig"
+    name = "hs_ig"
     _long_name = "significant_infragravity_wave_height"
     _standard_name = "sea_surface_infragravity_wave_significant_height"
     _unit = ureg.m
 
 
 class HsMax(MetaParameter):
-    _short_name = "hs_max"
+    name = "hs_max"
     _long_name = "maximum_wave_heigh"
     _standard_name = "sea_surface_wave_maximum_height"
     _unit = ureg.m
 
 
 class EtaMax(MetaParameter):
-    _short_name = "eta_max"
+    name = "eta_max"
     _long_name = "maximum_crest_heigh"
     _standard_name = "sea_surface_wave_maximum_crest_height"
     _unit = ureg.m
 
 
 class Hs110(MetaParameter):
-    _short_name = "hs_110"
+    name = "hs_110"
     _long_name = "highest_tenth_wave_heigh"
     _standard_name = "sea_surface_wave_mean_height_of_highest_tenth"
     _unit = ureg.m
 
 
 ## Wave periods
 class Tp(MetaParameter):
-    _short_name = "tp"
+    name = "tp"
     _long_name = "peak_wave_period"
     _standard_name = "sea_surface_wave_period_at_variance_spectral_density_maximum"
     _unit = ureg.s
 
 
 class Tz(MetaParameter):
-    _short_name = "tz"
+    name = "tz"
     _long_name = "zero_upcrossing_period"
     _standard_name = [
         "sea_surface_wave_mean_period",
         "sea_surface_wave_zero_upcrossing_period",
     ]
     _unit = ureg.s
 
 
 class T13(MetaParameter):
-    _short_name = "t13"
+    name = "t13"
     _long_name = "significant_wave_period"
     _standard_name = "sea_surface_wave_significant_period"
     _unit = ureg.s
 
 
 class T110(MetaParameter):
-    _short_name = "t110"
+    name = "t110"
     _long_name = "highest_tenth_wave_period"
     _standard_name = "sea_surface_wave_mean_period_of_highest_tenth"
     _unit = ureg.s
 
 
 class Tm01(MetaParameter):
-    _short_name = "tm01"
+    name = "tm01"
     _long_name = "first_moment_mean_wave_period"
     _standard_name = "sea_surface_wave_mean_period_from_variance_spectral_density_first_frequency_moment"
     _unit = ureg.s
 
 
 class Tm_10(MetaParameter):
-    _short_name = "tm_10"
+    name = "tm_10"
     _long_name = "inverse_moment_mean_wave_period"
     _standard_name = "sea_surface_wave_mean_period_from_variance_spectral_density_inverse_frequency_moment"
     _unit = ureg.s
 
 
 class Tm02(MetaParameter):
-    _short_name = "tm02"
+    name = "tm02"
     _long_name = "second_moment_mean_wave_period"
     _standard_name = "sea_surface_wave_mean_period_from_variance_spectral_density_second_frequency_moment"
     _unit = ureg.s
 
 
 class TpSwell(MetaParameter):
-    _short_name = "tp_swell"
+    name = "tp_swell"
     _long_name = "peak_wave_period_of_swell"
     _standard_name = (
         "sea_surface_swell_wave_period_at_variance_spectral_density_maximum"
     )
     _unit = ureg.s
 
 
 class Tm01Swell(MetaParameter):
-    _short_name = "tm01_swell"
+    name = "tm01_swell"
     _long_name = "first_moment_mean_wave_period_of_swell"
     _standard_name = "sea_surface_swell_wave_mean_period_from_variance_spectral_density_first_frequency_moment"
     _unit = ureg.s
 
 
 class Tm_10Swell(MetaParameter):
-    _short_name = "tm_10_swell"
+    name = "tm_10_swell"
     _long_name = "inverse_moment_mean_wave_period_of_swell"
     _standard_name = "sea_surface_swell_wave_mean_period_from_variance_spectral_density_inverse_frequency_moment"
     _unit = ureg.s
 
 
 class Tm02Swell(MetaParameter):
-    _short_name = "tm02_swell"
+    name = "tm02_swell"
     _long_name = "second_moment_mean_wave_period_of_swell"
     _standard_name = "sea_surface_swell_wave_mean_period_from_variance_spectral_density_second_frequency_moment"
     _unit = ureg.s
 
 
 class TpSwell1(MetaParameter):
-    _short_name = "tp_swell1"
+    name = "tp_swell1"
     _long_name = "peak_wave_period_of_primary_swell"
     _standard_name = (
         "sea_surface_primary_swell_wave_period_at_variance_spectral_density_maximum"
     )
     _unit = ureg.s
 
 
 class TpSwell2(MetaParameter):
-    _short_name = "tp_swell2"
+    name = "tp_swell2"
     _long_name = "peak_wave_period_of_secondary_swell"
     _standard_name = (
         "sea_surface_secondary_swell_wave_period_at_variance_spectral_density_maximum"
     )
     _unit = ureg.s
 
 
 class TpSwell3(MetaParameter):
-    _short_name = "tp_swell3"
+    name = "tp_swell3"
     _long_name = "peak_wave_period_of_tertiary_swell"
     _standard_name = (
         "sea_surface_tertiary_swell_wave_period_at_variance_spectral_density_maximum"
     )
     _unit = ureg.s
 
 
 class Tm01Sea(MetaParameter):
-    _short_name = "tm01_sea"
+    name = "tm01_sea"
     _long_name = "first_moment_mean_wave_period_of_wind_sea"
     _standard_name = "sea_surface_wind_wave_mean_period_from_variance_spectral_density_first_frequency_moment"
     _unit = ureg.s
 
 
 class Tm_10Sea(MetaParameter):
-    _short_name = "tm_10_sea"
+    name = "tm_10_sea"
     _long_name = "inverse_moment_mean_wave_period_of_wind_sea"
     _standard_name = "sea_surface_wind_wave_mean_period_from_variance_spectral_density_inverse_frequency_moment"
     _unit = ureg.s
 
 
 class Tm02Sea(MetaParameter):
-    _short_name = "tm02_sea"
+    name = "tm02_sea"
     _long_name = "second_moment_mean_wave_period_of_wind_swa"
     _standard_name = "sea_surface_wind_wave_mean_period_from_variance_spectral_density_second_frequency_moment"
     _unit = ureg.s
 
 
 ## Directions
 class Dirm(MetaParameter):
-    _short_name = "dirm"
+    name = "dirm"
     _long_name = "mean_wave_direction"
     _standard_name = "sea_surface_wave_from_direction"
     _unit = ureg.deg
 
 
 class Dirp(MetaParameter):
-    _short_name = "dirp"
+    name = "dirp"
     _long_name = "peak_wave_direction"
     _standard_name = (
         "sea_surface_wave_from_direction_at_variance_spectral_density_maximum"
     )
     _unit = ureg.deg
 
 
 class DirmSwell(MetaParameter):
-    _short_name = "dirm_swell"
+    name = "dirm_swell"
     _long_name = "mean_swell_direction"
     _standard_name = "sea_surface_swell_wave_from_direction"
     _unit = ureg.deg
 
 
 class DirpSwell(MetaParameter):
-    _short_name = "dirp_swell"
+    name = "dirp_swell"
     _long_name = "peak_swell_direction"
     _standard_name = (
         "sea_surface_swell_wave_from_direction_at_variance_spectral_density_maximum"
     )
     _unit = ureg.deg
 
 
 class DirmSea(MetaParameter):
-    _short_name = "dirm_sea"
+    name = "dirm_sea"
     _long_name = "mean_wind_sea_direction"
     _standard_name = "sea_surface_wind_wave_from_direction"
     _unit = ureg.deg
 
 
 class DirpSea(MetaParameter):
-    _short_name = "dirp_sea"
+    name = "dirp_sea"
     _long_name = "peak_wind_sea_direction"
     _standard_name = (
         "sea_surface_wind_wave_from_direction_at_variance_spectral_density_maximum"
     )
     _unit = ureg.deg
 
 
 class Spr(MetaParameter):
-    _short_name = "spr"
+    name = "spr"
     _long_name = "wave_directional_spread"
     _standard_name = "sea_surface_wave_directional_spread"
     _unit = ureg.deg
 
 
 class SprP(MetaParameter):
-    _short_name = "sprp"
+    name = "sprp"
     _long_name = "peak_wave_directional_spread"
     _standard_name = (
         "sea_surface_wave_directional_spread_at_variance_spectral_density_maximum"
     )
     _unit = ureg.deg
 
 
 class SprSwell(MetaParameter):
-    _short_name = "spr_swell"
+    name = "spr_swell"
     _long_name = "swell_directional_spread"
     _standard_name = "sea_surface_swell_wave_directional_spread"
     _unit = ureg.deg
 
 
 class SprPSwell(MetaParameter):
-    _short_name = "sprp_swell"
+    name = "sprp_swell"
     _long_name = "peak_swell_directional_spread"
     _standard_name = (
         "sea_surface_swell_wave_from_direction_at_variance_spectral_density_maximum"
     )
     _unit = ureg.deg
 
 
 class SprSea(MetaParameter):
-    _short_name = "spr_sea"
+    name = "spr_sea"
     _long_name = "wind_sea_directional_spread"
     _standard_name = "sea_surface_wind_wave_directional_spread"
     _unit = ureg.deg
 
 
 class SprPSea(MetaParameter):
-    _short_name = "sprp_sea"
+    name = "sprp_sea"
     _long_name = "peak_wind_sea_directional_spread"
     _standard_name = (
         "sea_surface_wind_wave_from_direction_at_variance_spectral_density_maximum"
     )
     _unit = ureg.deg
 
 
 ## Spectral
 class Ef(MetaParameter):
-    _short_name = "ef"
+    name = "ef"
     _long_name = "spectral_density"
     _standard_name = "sea_surface_wave_variance_spectral_density"
     _unit = ureg.m * ureg.m * ureg.s
 
 
 class Efth(MetaParameter):
-    _short_name = "efth"
+    name = "efth"
     _long_name = "directional_spectral_density"
     _standard_name = "sea_surface_wave_directional_variance_spectral_density"
     _unit = ureg.m * ureg.m * ureg.s / ureg.rad
 
 
 ## Moments (non-standard)
 class M0(MetaParameter):
-    _short_name = "m0"
+    name = "m0"
     _long_name = "zeroth_wave_moment"
     _standard_name = "sea_surface_zeroth_wave_moment"
     _unit = ureg.m**2
     _cf = False
 
 
 class M1(MetaParameter):
-    _short_name = "m1"
+    name = "m1"
     _long_name = "first_wave_moment"
     _standard_name = "sea_surface_first_wave_moment"
     _unit = ureg.m**2 / ureg.s
     _cf = False
 
 
 class M_1(MetaParameter):
-    _short_name = "m_1"
+    name = "m_1"
     _long_name = "first_inverse_wave_moment"
     _standard_name = "sea_surface_first_inverse_wave_moment"
     _unit = ureg.m**2 * ureg.s
     _cf = False
 
 
 class M2(MetaParameter):
-    _short_name = "m2"
+    name = "m2"
     _long_name = "second_wave_moment"
     _standard_name = "sea_surface_second_wave_moment"
     _unit = ureg.m**2 / ureg.s**2
     _cf = False
 
 
 class M3(MetaParameter):
-    _short_name = "m3"
+    name = "m3"
     _long_name = "thirds_wave_moment"
     _standard_name = "sea_surface_thirds_wave_moment"
     _unit = ureg.m**2 / ureg.s**3
     _cf = False
 
 
 class M4(MetaParameter):
-    _short_name = "m4"
+    name = "m4"
     _long_name = "fourth_wave_moment"
     _standard_name = "sea_surface_fourth_wave_moment"
     _unit = ureg.m**2 / ureg.s**4
     _cf = False
 
 
 class M5(MetaParameter):
-    _short_name = "m5"
+    name = "m5"
     _long_name = "fifth_wave_moment"
     _standard_name = "sea_surface_fifth_wave_moment"
     _unit = ureg.m**2 / ureg.s**5
     _cf = False
```

### Comparing `geo_parameters-0.1.1/geo_parameters/wind.py` & `geo_parameters-0.2.1/geo_parameters/wind.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 from .metaparameter import MetaParameter
 import pint
 
 ureg = pint.UnitRegistry()
+ureg.default_format = "~C"
 
 
 class XWind(MetaParameter):
-    _short_name = "x_wind"
+    name = "x_wind"
     _long_name = "x_wind_component"
     _standard_name = [
         "x_wind",
         "grid_eastward_wind",
     ]
     _unit = ureg.m / ureg.s
 
 
 class YWind(MetaParameter):
-    _short_name = "y_wind"
+    name = "y_wind"
     _long_name = "y_wind_component"
     _standard_name = [
         "y_wind",
         "grid_northward_wind",
     ]
     _unit = ureg.m / ureg.s
 
 
 class Wind(MetaParameter):
-    _short_name = "wind"
+    name = "wind"
     _long_name = "wind_speed"
     _standard_name = "wind_speed"
     _unit = ureg.m / ureg.s
 
 
 class WindDir(MetaParameter):
-    _short_name = "wind_dir"
+    name = "wind_dir"
     _long_name = "wind_direction"
     _standard_name = "wind_from_direction"
     _unit = ureg.deg
 
 
 class XGust(MetaParameter):
-    _short_name = "x_gust"
+    name = "x_gust"
     _long_name = "x_gust_component"
     _standard_name = "x_wind_gust"
     _unit = ureg.m / ureg.s
 
 
 class YGust(MetaParameter):
-    _short_name = "y_gust"
+    name = "y_gust"
     _long_name = "y_gust_component"
     _standard_name = "y_wind_gust"
     _unit = ureg.m / ureg.s
 
 
 class Gust(MetaParameter):
-    _short_name = "gust"
+    name = "gust"
     _long_name = "wind_gust"
     _standard_name = "wind_speed_of_gust"
     _unit = ureg.m / ureg.s
 
 
 class GustDir(MetaParameter):
-    _short_name = "gust_dir"
+    name = "gust_dir"
     _long_name = "wind_gust_direction"
     _standard_name = "wind_gust_from_direction"
     _unit = ureg.deg
```

### Comparing `geo_parameters-0.1.1/tests/test_doc.py` & `geo_parameters-0.2.1/tests/test_doc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from geo_parameters.wave import Hs, Tp
 from geo_parameters import get as gpget
 from geo_parameters import dict_of_parameters
 
 
 def test_names():
     assert Hs.standard_name() == "sea_surface_wave_significant_height"
-    assert Hs.short_name() == "hs"
+    assert Hs.name == "hs"
     hsig = Hs()
-    assert hsig.name() == "hs"
+    assert hsig.name == "hs"
 
     hsig = Hs(name="hsig")
-    assert hsig.name() == "hsig"
-    assert str(Hs(name="hsig")) == str("hsig")
+    assert hsig.name == "hsig"
 
     assert hsig.standard_name() == "sea_surface_wave_significant_height"
     assert hsig.long_name() == "significant_wave_height"
 
     assert (
         hsig.standard_name(alias=True) == "significant_height_of_wind_and_swell_waves"
     )
```

### Comparing `geo_parameters-0.1.1/tests/test_funcs.py` & `geo_parameters-0.2.1/tests/test_funcs.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.1.1/tests/test_names.py` & `geo_parameters-0.2.1/tests/test_names.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from geo_parameters.wave import Hs
 
 
 def test_name_of_class():
-    assert Hs.short_name() == "hs"
+    assert Hs.name == "hs"
     assert Hs.long_name() == "significant_wave_height"
     assert Hs.standard_name() == "sea_surface_wave_significant_height"
     assert Hs.standard_name(alias=True) == "significant_height_of_wind_and_swell_waves"
 
 
 def test_units_of_class():
-    assert str(Hs.unit()) == "meter"
+    assert str(Hs.unit()) == "m"
 
 
 def test_name_of_instance():
-    assert Hs().short_name() == "hs"
-    assert Hs(name="hsig").name() == "hsig"
-    assert Hs("hsig").name() == "hsig"
+    assert Hs().name == "hs"
+    assert Hs(name="hsig").name == "hsig"
+    assert Hs("hsig").name == "hsig"
     assert Hs().long_name() == "significant_wave_height"
     assert Hs().standard_name() == "sea_surface_wave_significant_height"
     assert (
         Hs().standard_name(alias=True) == "significant_height_of_wind_and_swell_waves"
     )
 
 
 def test_units_of_instance():
-    assert str(Hs().unit()) == "meter"
+    assert str(Hs().unit()) == "m"
```

