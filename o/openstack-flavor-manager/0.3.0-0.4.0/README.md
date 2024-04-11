# Comparing `tmp/openstack-flavor-manager-0.3.0.tar.gz` & `tmp/openstack-flavor-manager-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstack-flavor-manager-0.3.0.tar", last modified: Tue Oct 24 15:07:53 2023, max compression
+gzip compressed data, was "openstack-flavor-manager-0.4.0.tar", last modified: Tue Nov 21 09:50:02 2023, max compression
```

## Comparing `openstack-flavor-manager-0.3.0.tar` & `openstack-flavor-manager-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-24 15:07:53.411718 openstack-flavor-manager-0.3.0/
--rw-r--r--   0 zuul      (1000) zuul      (1000)    11357 2023-10-24 15:07:03.000000 openstack-flavor-manager-0.3.0/LICENSE
--rw-r--r--   0 zuul      (1000) zuul      (1000)    14573 2023-10-24 15:07:53.411718 openstack-flavor-manager-0.3.0/PKG-INFO
--rw-r--r--   0 zuul      (1000) zuul      (1000)      442 2023-10-24 15:07:03.000000 openstack-flavor-manager-0.3.0/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-24 15:07:53.411718 openstack-flavor-manager-0.3.0/openstack_flavor_manager/
--rw-r--r--   0 zuul      (1000) zuul      (1000)        0 2023-10-24 15:07:03.000000 openstack-flavor-manager-0.3.0/openstack_flavor_manager/__init__.py
--rw-r--r--   0 zuul      (1000) zuul      (1000)     4909 2023-10-24 15:07:03.000000 openstack-flavor-manager-0.3.0/openstack_flavor_manager/main.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-24 15:07:53.411718 openstack-flavor-manager-0.3.0/openstack_flavor_manager.egg-info/
--rw-r--r--   0 zuul      (1000) zuul      (1000)    14573 2023-10-24 15:07:53.000000 openstack-flavor-manager-0.3.0/openstack_flavor_manager.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2023-10-24 15:07:53.000000 openstack-flavor-manager-0.3.0/openstack_flavor_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-10-24 15:07:53.000000 openstack-flavor-manager-0.3.0/openstack_flavor_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-10-24 15:07:53.000000 openstack-flavor-manager-0.3.0/openstack_flavor_manager.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-10-24 15:07:53.000000 openstack-flavor-manager-0.3.0/openstack_flavor_manager.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2023-10-24 15:07:53.000000 openstack-flavor-manager-0.3.0/openstack_flavor_manager.egg-info/top_level.txt
--rw-r--r--   0 zuul      (1000) zuul      (1000)     1459 2023-10-24 15:07:03.000000 openstack-flavor-manager-0.3.0/pyproject.toml
--rw-r--r--   0 zuul      (1000) zuul      (1000)       83 2023-10-24 15:07:04.000000 openstack-flavor-manager-0.3.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-10-24 15:07:53.411718 openstack-flavor-manager-0.3.0/setup.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-21 09:50:02.006964 openstack-flavor-manager-0.4.0/
+-rw-r--r--   0 zuul      (1000) zuul      (1000)    11357 2023-11-21 09:49:26.000000 openstack-flavor-manager-0.4.0/LICENSE
+-rw-r--r--   0 zuul      (1000) zuul      (1000)    14573 2023-11-21 09:50:02.006964 openstack-flavor-manager-0.4.0/PKG-INFO
+-rw-r--r--   0 zuul      (1000) zuul      (1000)      442 2023-11-21 09:49:26.000000 openstack-flavor-manager-0.4.0/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-21 09:50:02.006964 openstack-flavor-manager-0.4.0/openstack_flavor_manager/
+-rw-r--r--   0 zuul      (1000) zuul      (1000)        0 2023-11-21 09:49:26.000000 openstack-flavor-manager-0.4.0/openstack_flavor_manager/__init__.py
+-rw-r--r--   0 zuul      (1000) zuul      (1000)     5560 2023-11-21 09:49:26.000000 openstack-flavor-manager-0.4.0/openstack_flavor_manager/main.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-21 09:50:02.006964 openstack-flavor-manager-0.4.0/openstack_flavor_manager.egg-info/
+-rw-r--r--   0 zuul      (1000) zuul      (1000)    14573 2023-11-21 09:50:01.000000 openstack-flavor-manager-0.4.0/openstack_flavor_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2023-11-21 09:50:02.000000 openstack-flavor-manager-0.4.0/openstack_flavor_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-11-21 09:50:01.000000 openstack-flavor-manager-0.4.0/openstack_flavor_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-11-21 09:50:01.000000 openstack-flavor-manager-0.4.0/openstack_flavor_manager.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-11-21 09:50:01.000000 openstack-flavor-manager-0.4.0/openstack_flavor_manager.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2023-11-21 09:50:01.000000 openstack-flavor-manager-0.4.0/openstack_flavor_manager.egg-info/top_level.txt
+-rw-r--r--   0 zuul      (1000) zuul      (1000)     1459 2023-11-21 09:49:26.000000 openstack-flavor-manager-0.4.0/pyproject.toml
+-rw-r--r--   0 zuul      (1000) zuul      (1000)       83 2023-11-21 09:49:26.000000 openstack-flavor-manager-0.4.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-11-21 09:50:02.006964 openstack-flavor-manager-0.4.0/setup.cfg
```

### Comparing `openstack-flavor-manager-0.3.0/LICENSE` & `openstack-flavor-manager-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openstack-flavor-manager-0.3.0/PKG-INFO` & `openstack-flavor-manager-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstack-flavor-manager
-Version: 0.3.0
+Version: 0.4.0
 Summary: OpenStack flavor manager
 Author-email: OSISM community <info@osism.tech>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `openstack-flavor-manager-0.3.0/openstack_flavor_manager/main.py` & `openstack-flavor-manager-0.4.0/openstack_flavor_manager/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,17 @@
         value = defaults[key_string]
     # If disc is not present then it is a flavor without disc.
     elif key_string == "disk":
         value = 0
     # By default a flavor should be public
     elif key_string == "public":
         value = True
+    # If no flavorid is given, automatically assign one (OpenStack SDK feature)
+    elif key_string == "flavorid":
+        value = "auto"
     else:
         raise ValueError(f"Unknown key_string '{key_string}'")
 
     return value
 
 
 class Cloud:
@@ -34,41 +37,49 @@
 
     def set_flavor(self, flavor_spec: dict, defaults: dict) -> Flavor | None:
         flavor_name = get_spec_or_default(
             key_string="name", flavor_spec=flavor_spec, defaults=defaults
         )
 
         if flavor_name in self.existing_flavor_names:
-            logger.info(
-                f"Flavor '{flavor_name}' already exists."
-            )
+            logger.info(f"Flavor '{flavor_name}' already exists.")
             return None
 
         flavor = self.conn.create_flavor(
             name=flavor_name,
             ram=get_spec_or_default(
                 key_string="ram", flavor_spec=flavor_spec, defaults=defaults
             ),
             vcpus=get_spec_or_default(
                 key_string="cpus", flavor_spec=flavor_spec, defaults=defaults
             ),
-
             disk=get_spec_or_default(
                 key_string="disk", flavor_spec=flavor_spec, defaults=defaults
             ),
             ephemeral=0,
             swap=0,
             rxtx_factor=1.0,
             is_public=get_spec_or_default(
                 key_string="public", flavor_spec=flavor_spec, defaults=defaults
             ),
+            flavorid=get_spec_or_default(
+                key_string="flavorid", flavor_spec=flavor_spec, defaults=defaults
+            ),
         )
+        extra_specs = {
+            key: value
+            for key, value in flavor_spec.items()
+            # we could exclude keys explicitly, like so:
+            # if key not in ('name', 'ram', 'cpus', 'disk', 'public', 'disabled')
+            # but the extra specs should be prefixed, so we can as well do it like so:
+            if ":" in key
+        }
         self.conn.set_flavor_specs(
             flavor_id=flavor.id,
-            extra_specs={},
+            extra_specs=extra_specs,
         )
         return flavor
 
 
 class FlavorManager:
     def __init__(
         self, cloud: Cloud, definitions: dict, recommended: bool = False
@@ -88,15 +99,17 @@
             try:
                 flavor = self.cloud.set_flavor(
                     flavor_spec=required_flavor, defaults=self.defaults_dict
                 )
                 if flavor:
                     logger.info(f"Flavor '{required_flavor['name']}' created.")
             except Exception as e:
-                logger.error(f"Flavor '{required_flavor['name']}' could not be created.")
+                logger.error(
+                    f"Flavor '{required_flavor['name']}' could not be created."
+                )
                 logger.error(e)
 
 
 def get_flavor_definitions(name: str) -> dict:
     url = None
     if name == "scs":
         url = "https://raw.githubusercontent.com/SovereignCloudStack/standards/main/Tests/iaas/SCS-Spec.MandatoryFlavors.verbose.yaml"  # noqa: E501
@@ -117,15 +130,14 @@
     name: str = typer.Option("scs", "--name", help="Name of flavor definitions."),
     debug: bool = typer.Option(False, "--debug", help="Enable debug logging."),
     cloud: str = typer.Option("admin", "--cloud", help="Cloud name in clouds.yaml."),
     recommended: bool = typer.Option(
         False, "--recommended", help="Create recommended flavors."
     ),
 ) -> None:
-
     if debug:
         level = "DEBUG"
         log_fmt = (
             "<green>{time:YYYY-MM-DD HH:mm:ss}</green> | <level>{level: <8}</level> | "
             "<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>"
         )
     else:
```

### Comparing `openstack-flavor-manager-0.3.0/openstack_flavor_manager.egg-info/PKG-INFO` & `openstack-flavor-manager-0.4.0/openstack_flavor_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstack-flavor-manager
-Version: 0.3.0
+Version: 0.4.0
 Summary: OpenStack flavor manager
 Author-email: OSISM community <info@osism.tech>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `openstack-flavor-manager-0.3.0/pyproject.toml` & `openstack-flavor-manager-0.4.0/pyproject.toml`

 * *Files identical despite different names*

