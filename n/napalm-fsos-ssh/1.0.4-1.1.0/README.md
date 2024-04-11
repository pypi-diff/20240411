# Comparing `tmp/napalm_fsos_ssh-1.0.4.tar.gz` & `tmp/napalm_fsos_ssh-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm_fsos_ssh-1.0.4.tar", max compression
+gzip compressed data, was "napalm_fsos_ssh-1.1.0.tar", max compression
```

## Comparing `napalm_fsos_ssh-1.0.4.tar` & `napalm_fsos_ssh-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    22294 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/LICENSE
--rw-r--r--   0        0        0    23504 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/LICENSE.fr
--rw-r--r--   0        0        0     2055 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/README.md
--rw-r--r--   0        0        0      319 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/__init__.py
--rw-r--r--   0        0        0    25296 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/fsos.py
--rw-r--r--   0        0        0     1601 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/index
--rw-r--r--   0        0        0      313 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/ping.textfsm
--rw-r--r--   0        0        0      151 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_arp.textfsm
--rw-r--r--   0        0        0      242 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      835 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_interfaces_counters.textfsm
--rw-r--r--   0        0        0      225 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0      331 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_ip_route.textfsm
--rw-r--r--   0        0        0      180 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_ipv6_interface_brief.textfsm
--rw-r--r--   0        0        0      196 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      270 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_ipv6_route.textfsm
--rw-r--r--   0        0        0      175 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_lldp_neighbor.textfsm
--rw-r--r--   0        0        0      395 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_lldp_neighbor_interface.textfsm
--rw-r--r--   0        0        0      135 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_memory.textfsm
--rw-r--r--   0        0        0       71 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_ntp.textfsm
--rw-r--r--   0        0        0      190 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_snmp_server.textfsm
--rw-r--r--   0        0        0       95 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_snmp_server_engine_id.textfsm
--rw-r--r--   0        0        0      432 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_system.textfsm
--rw-r--r--   0        0        0      418 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_transceiver.textfsm
--rw-r--r--   0        0        0      107 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_users.textfsm
--rw-r--r--   0        0        0      163 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_version.textfsm
--rw-r--r--   0        0        0     1049 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_vlan_all.textfsm
--rw-r--r--   0        0        0      221 2024-01-03 10:25:05.778809 napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/traceroute.textfsm
--rw-r--r--   0        0        0     1083 2024-01-03 10:25:27.299070 napalm_fsos_ssh-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 napalm_fsos_ssh-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    22294 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/LICENSE
+-rw-r--r--   0        0        0    23504 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/LICENSE.fr
+-rw-r--r--   0        0        0     2057 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/README.md
+-rw-r--r--   0        0        0      319 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/__init__.py
+-rw-r--r--   0        0        0    25366 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/fsos.py
+-rw-r--r--   0        0        0     1601 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/index
+-rw-r--r--   0        0        0      313 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/ping.textfsm
+-rw-r--r--   0        0        0      151 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_arp.textfsm
+-rw-r--r--   0        0        0      242 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      835 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_interfaces_counters.textfsm
+-rw-r--r--   0        0        0      225 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0      331 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_ip_route.textfsm
+-rw-r--r--   0        0        0      180 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_ipv6_interface_brief.textfsm
+-rw-r--r--   0        0        0      196 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      270 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_ipv6_route.textfsm
+-rw-r--r--   0        0        0      175 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_lldp_neighbor.textfsm
+-rw-r--r--   0        0        0      395 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_lldp_neighbor_interface.textfsm
+-rw-r--r--   0        0        0      135 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_memory.textfsm
+-rw-r--r--   0        0        0       71 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_ntp.textfsm
+-rw-r--r--   0        0        0      190 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_snmp_server.textfsm
+-rw-r--r--   0        0        0       95 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_snmp_server_engine_id.textfsm
+-rw-r--r--   0        0        0      432 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_system.textfsm
+-rw-r--r--   0        0        0      418 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_transceiver.textfsm
+-rw-r--r--   0        0        0      107 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_users.textfsm
+-rw-r--r--   0        0        0      163 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_version.textfsm
+-rw-r--r--   0        0        0     1049 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_vlan_all.textfsm
+-rw-r--r--   0        0        0      221 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/traceroute.textfsm
+-rw-r--r--   0        0        0     1099 2024-04-11 17:49:39.759933 napalm_fsos_ssh-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 napalm_fsos_ssh-1.1.0/PKG-INFO
```

### Comparing `napalm_fsos_ssh-1.0.4/LICENSE` & `napalm_fsos_ssh-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm_fsos_ssh-1.0.4/LICENSE.fr` & `napalm_fsos_ssh-1.1.0/LICENSE.fr`

 * *Files identical despite different names*

### Comparing `napalm_fsos_ssh-1.0.4/README.md` & `napalm_fsos_ssh-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 # Install
 ```
 pip install napalm-fsos-ssh
 ```
 
 # Dev
-# Devcontainer
+## Devcontainer
 A devcontainer is available
 
-# Standard
+## Standard
 Install [Poetry](https://python-poetry.org/docs/master/#installing-with-the-official-installer)
 
 Install and setup dependencies
 ```
 poetry install
 poetry shell
 pre-commit install
```

### Comparing `napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/fsos.py` & `napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/fsos.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,19 @@
                 raise ValueError(f"Unable to execute command {command}")
             cli_output.setdefault(command, {})
             cli_output[command] = output
 
         return cli_output
 
     def get_config(
-        self, retrieve: str = "all", full: bool = False, sanitized: bool = False
+        self,
+        retrieve: str = "all",
+        full: bool = False,
+        sanitized: bool = False,
+        format="text",
     ) -> models.ConfigDict:
         data = {
             "startup": "",
             "running": "",
             "candidate": "",
         }
 
@@ -422,28 +426,28 @@
                 }
             )
 
         return data
 
     def get_lldp_neighbors_detail(
         self, interface: str = ""
-    ) -> models.LLDPNeighborsDetailDict:
+    ) -> Dict[str, List[models.LLDPNeighborDetailDict]]:
         commands = {}
         if interface == "":
             command = "show lldp neighbor"
             output = self._send_command(command, use_textfsm=True)
 
             for entry in output:
                 if "Group" in entry["interface"]:
                     entry["interface"] = entry["interface"].replace(
                         "Group", "port-channel"
                     )
-                commands[
-                    entry["interface"]
-                ] = f"show lldp neighbor {entry['interface']}"
+                commands[entry["interface"]] = (
+                    f"show lldp neighbor {entry['interface']}"
+                )
         else:
             commands[interface] = [f"show lldp neighbor {interface}"]
 
         output = {}
         for k in commands:
             output[k] = self._send_command(commands[k], use_textfsm=True)
```

### Comparing `napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/index` & `napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/index`

 * *Files identical despite different names*

### Comparing `napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_interfaces_counters.textfsm` & `napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_interfaces_counters.textfsm`

 * *Files identical despite different names*

### Comparing `napalm_fsos_ssh-1.0.4/napalm_fsos_ssh/utils/textfsm_templates/show_vlan_all.textfsm` & `napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_vlan_all.textfsm`

 * *Files identical despite different names*

### Comparing `napalm_fsos_ssh-1.0.4/pyproject.toml` & `napalm_fsos_ssh-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "napalm-fsos-ssh"
-version = "v1.0.4"
+version = "v1.1.0"
 description = "Napalm driver for FSOS through SSH"
 authors = ["Ludovic Ortega <ludovic.ortega@adminafk.fr>"]
 license = "CeCILL"
 readme = "README.md"
 homepage = "https://github.com/napalm-automation-community/napalm-fsos-ssh"
 repository = "https://github.com/napalm-automation-community/napalm-fsos-ssh"
 keywords = ["napalm", "fsos", "netmiko"]
@@ -21,16 +21,16 @@
 include = [
     "LICENSE",
     "LICENSE.fr",
 ]
 
 [tool.poetry.dependencies]
 python = ">3.8,<3.12"
-napalm = ">=4.0,<4.2"
+napalm = ">=4.0,<5.1"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "~7.4.4"
-ruff = "~0.1.11"
+pytest = ">=7.4.4,<8.2.0"
+ruff = ">=0.1.11,<0.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `napalm_fsos_ssh-1.0.4/PKG-INFO` & `napalm_fsos_ssh-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-fsos-ssh
-Version: 1.0.4
+Version: 1.1.0
 Summary: Napalm driver for FSOS through SSH
 Home-page: https://github.com/napalm-automation-community/napalm-fsos-ssh
 License: CeCILL
 Keywords: napalm,fsos,netmiko
 Author: Ludovic Ortega
 Author-email: ludovic.ortega@adminafk.fr
 Requires-Python: >3.8,<3.12
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
-Requires-Dist: napalm (>=4.0,<4.2)
+Requires-Dist: napalm (>=4.0,<5.1)
 Project-URL: Repository, https://github.com/napalm-automation-community/napalm-fsos-ssh
 Description-Content-Type: text/markdown
 
 Napalm driver for FSOS using SSH
 
 [![PyPI](https://img.shields.io/pypi/v/napalm-fsos-ssh.svg)](https://pypi.python.org/pypi/napalm-fsos-ssh)
 [![PyPI versions](https://img.shields.io/pypi/pyversions/napalm-fsos-ssh.svg)](https://pypi.python.org/pypi/napalm-fsos-ssh)
@@ -34,18 +34,18 @@
 
 # Install
 ```
 pip install napalm-fsos-ssh
 ```
 
 # Dev
-# Devcontainer
+## Devcontainer
 A devcontainer is available
 
-# Standard
+## Standard
 Install [Poetry](https://python-poetry.org/docs/master/#installing-with-the-official-installer)
 
 Install and setup dependencies
 ```
 poetry install
 poetry shell
 pre-commit install
```

