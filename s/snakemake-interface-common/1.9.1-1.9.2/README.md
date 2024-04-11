# Comparing `tmp/snakemake_interface_common-1.9.1.tar.gz` & `tmp/snakemake_interface_common-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_interface_common-1.9.1.tar", max compression
+gzip compressed data, was "snakemake_interface_common-1.9.2.tar", max compression
```

## Comparing `snakemake_interface_common-1.9.1.tar` & `snakemake_interface_common-1.9.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1076 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/LICENSE
--rw-r--r--   0        0        0       89 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/README.md
--rw-r--r--   0        0        0      888 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/snakemake_interface_common/__init__.py
--rw-r--r--   0        0        0     4576 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/snakemake_interface_common/_common.py
--rw-r--r--   0        0        0     1974 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/snakemake_interface_common/exceptions.py
--rw-r--r--   0        0        0      281 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/snakemake_interface_common/logging.py
--rw-r--r--   0        0        0     4307 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/snakemake_interface_common/plugin_registry/__init__.py
--rw-r--r--   0        0        0      643 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/snakemake_interface_common/plugin_registry/attribute_types.py
--rw-r--r--   0        0        0     8706 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/snakemake_interface_common/plugin_registry/plugin.py
--rw-r--r--   0        0        0     1701 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/snakemake_interface_common/plugin_registry/tests.py
--rw-r--r--   0        0        0      318 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/snakemake_interface_common/rules.py
--rw-r--r--   0        0        0     1210 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/snakemake_interface_common/settings.py
--rw-r--r--   0        0        0      835 2023-09-26 13:03:12.052373 snakemake_interface_common-1.9.1/snakemake_interface_common/utils.py
--rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 snakemake_interface_common-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/LICENSE
+-rw-r--r--   0        0        0       89 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/README.md
+-rw-r--r--   0        0        0      912 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/snakemake_interface_common/__init__.py
+-rw-r--r--   0        0        0     4576 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/snakemake_interface_common/_common.py
+-rw-r--r--   0        0        0     1974 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/snakemake_interface_common/exceptions.py
+-rw-r--r--   0        0        0      281 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/snakemake_interface_common/logging.py
+-rw-r--r--   0        0        0     4307 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/snakemake_interface_common/plugin_registry/__init__.py
+-rw-r--r--   0        0        0      643 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/snakemake_interface_common/plugin_registry/attribute_types.py
+-rw-r--r--   0        0        0     8842 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/snakemake_interface_common/plugin_registry/plugin.py
+-rw-r--r--   0        0        0     1964 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/snakemake_interface_common/plugin_registry/tests.py
+-rw-r--r--   0        0        0      318 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/snakemake_interface_common/rules.py
+-rw-r--r--   0        0        0     1210 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/snakemake_interface_common/settings.py
+-rw-r--r--   0        0        0      835 2023-09-26 13:36:18.156761 snakemake_interface_common-1.9.2/snakemake_interface_common/utils.py
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 snakemake_interface_common-1.9.2/PKG-INFO
```

### Comparing `snakemake_interface_common-1.9.1/LICENSE` & `snakemake_interface_common-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_interface_common-1.9.1/pyproject.toml` & `snakemake_interface_common-1.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "snakemake-interface-common"
-version = "1.9.1"
+version = "1.9.2"
 description = "Common functions and classes for Snakemake and its plugins"
 authors = ["Johannes Koester <johannes.koester@uni-due.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 argparse-dataclass = "^2.0.0"
+ConfigArgParse = "^1.7"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 coverage = {extras = ["toml"], version = "^6.3.1"}
 flake8 = "^4.0.1"
 flake8-bugbear = "^22.1.11"
 pytest = "^7.0"
```

### Comparing `snakemake_interface_common-1.9.1/snakemake_interface_common/_common.py` & `snakemake_interface_common-1.9.2/snakemake_interface_common/_common.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_common-1.9.1/snakemake_interface_common/exceptions.py` & `snakemake_interface_common-1.9.2/snakemake_interface_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_common-1.9.1/snakemake_interface_common/plugin_registry/__init__.py` & `snakemake_interface_common-1.9.2/snakemake_interface_common/plugin_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_common-1.9.1/snakemake_interface_common/plugin_registry/attribute_types.py` & `snakemake_interface_common-1.9.2/snakemake_interface_common/plugin_registry/attribute_types.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_common-1.9.1/snakemake_interface_common/plugin_registry/plugin.py` & `snakemake_interface_common-1.9.2/snakemake_interface_common/plugin_registry/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
                 )
             else:
                 msg = (
                     "No untagged settings available for the plugin {self.plugin_name}."
                 )
             raise WorkflowError(msg)
 
+    def __iter__(self):
+        return iter(self._inner.values())
+
 
 class PluginBase(ABC):
     @property
     @abstractmethod
     def name(self) -> str:
         ...
 
@@ -162,14 +165,17 @@
         # These fields will have the executor prefix
         for thefield in fields(dc):
             name, value = get_name_and_value(thefield)
             field_names[name] = thefield.name
             if thefield.metadata.get("required"):
                 required_args.add(name)
 
+            if value is None:
+                continue
+
             def extract_values(value, thefield, name, tag=None):
                 # This will only add instantiated values, and
                 # skip over dataclasses._MISSING_TYPE and similar
                 if isinstance(value, ArgTypes):
                     # If a parsing function is defined, we pass the arg value to it
                     # in order to get the correct type back.
                     parse_func = thefield.metadata.get("parse_func")
@@ -205,20 +211,20 @@
                 raise WorkflowError(
                     f"The following required arguments are missing for "
                     f"plugin {self.name}{tag_phrase}: {', '.join(cli_args)}."
                 )
 
         # convert into the dataclass
         if self.support_tagged_values:
-            tagged_settings = TaggedSettings()
+            tagged_settings = TaggedSettings(self.name)
             for tag, kwargs in kwargs_tagged.items():
                 check_required(kwargs, tag=tag)
                 tagged_settings.register_settings(dc(**kwargs), tag=tag)
             try:
-                check_required(kwargs)
+                check_required(kwargs_all)
                 tagged_settings.register_settings(dc(kwargs_all))
             except WorkflowError:
                 # if untagged settings are not complete, do not register them
                 pass
             return tagged_settings
         else:
             check_required(kwargs)
```

### Comparing `snakemake_interface_common-1.9.1/snakemake_interface_common/plugin_registry/tests.py` & `snakemake_interface_common-1.9.2/snakemake_interface_common/plugin_registry/tests.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from abc import ABC, abstractmethod
-import argparse
+import configargparse
 
-from snakemake_interface_common.plugin_registry.plugin import PluginBase, SettingsBase
+from snakemake_interface_common.plugin_registry.plugin import (
+    PluginBase,
+    SettingsBase,
+    TaggedSettings,
+)
 from snakemake_interface_common.plugin_registry import PluginRegistryBase
 
 
 class TestRegistryBase(ABC):
     __test__ = False
 
     @abstractmethod
@@ -30,25 +34,29 @@
             len(registry.plugins) == 1
         ), "we assume that only one plugin is installed in test environment"
         plugin = registry.get_plugin(self.get_test_plugin_name())
         self.validate_plugin(plugin)
 
     def test_registry_register_cli_args(self):
         registry = self.get_registry()
-        parser = argparse.ArgumentParser()
+        parser = configargparse.ArgumentParser()
         registry.register_cli_args(parser)
         prefix = registry.get_plugin(self.get_test_plugin_name()).cli_prefix
         for action in parser._actions:
             if not action.dest == "help":
-                assert action.dest.startswith(prefix)
+                assert action.dest.startswith(
+                    prefix.replace("-", "_")
+                ), f"{prefix} is not a prefix of {action.dest}"
 
     def test_registry_cli_args_to_settings(self):
         registry = self.get_registry()
 
-        parser = argparse.ArgumentParser()
+        parser = configargparse.ArgumentParser()
         registry.register_cli_args(parser)
         args = parser.parse_args([])
 
         plugin = registry.get_plugin(self.get_test_plugin_name())
         settings = plugin.get_settings(args)
-
-        self.validate_settings(settings, plugin)
+        if not isinstance(settings, TaggedSettings):
+            settings = [settings]
+        for s in settings:
+            self.validate_settings(s, plugin)
```

### Comparing `snakemake_interface_common-1.9.1/snakemake_interface_common/settings.py` & `snakemake_interface_common-1.9.2/snakemake_interface_common/settings.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_common-1.9.1/snakemake_interface_common/utils.py` & `snakemake_interface_common-1.9.2/snakemake_interface_common/utils.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_common-1.9.1/PKG-INFO` & `snakemake_interface_common-1.9.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: snakemake-interface-common
-Version: 1.9.1
+Version: 1.9.2
 Summary: Common functions and classes for Snakemake and its plugins
 Author: Johannes Koester
 Author-email: johannes.koester@uni-due.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ConfigArgParse (>=1.7,<2.0)
 Requires-Dist: argparse-dataclass (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # snakemake-interface-common
 
 Common functions and classes for Snakemake and its plugins.
```

