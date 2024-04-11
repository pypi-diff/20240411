# Comparing `tmp/eve2cml-0.1.0b1.tar.gz` & `tmp/eve2cml-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eve2cml-0.1.0b1.tar", last modified: Wed Mar 13 11:44:01 2024, max compression
+gzip compressed data, was "eve2cml-0.1.0b2.tar", last modified: Thu Apr 11 10:50:48 2024, max compression
```

## Comparing `eve2cml-0.1.0b1.tar` & `eve2cml-0.1.0b2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1088 2024-03-12 12:50:05.022091 eve2cml-0.1.0b1/LICENSE
--rw-r--r--   0        0        0     5416 2024-03-13 11:33:43.054845 eve2cml-0.1.0b1/README.md
--rw-r--r--   0        0        0     1279 2024-03-13 11:44:01.793188 eve2cml-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-08 09:09:17.161399 eve2cml-0.1.0b1/src/eve2cml/__init__.py
--rw-r--r--   0        0        0       23 2024-03-13 11:44:01.785188 eve2cml-0.1.0b1/src/eve2cml/_version.py
--rw-r--r--   0        0        0      446 2024-03-12 10:40:45.713918 eve2cml-0.1.0b1/src/eve2cml/eve/__init__.py
--rw-r--r--   0        0        0      805 2024-03-08 12:06:50.314821 eve2cml-0.1.0b1/src/eve2cml/eve/config.py
--rw-r--r--   0        0        0      854 2024-03-08 12:06:46.366807 eve2cml-0.1.0b1/src/eve2cml/eve/configset.py
--rw-r--r--   0        0        0      367 2024-03-08 10:48:43.230941 eve2cml-0.1.0b1/src/eve2cml/eve/decode.py
--rw-r--r--   0        0        0     2433 2024-03-08 16:27:31.705916 eve2cml-0.1.0b1/src/eve2cml/eve/interface.py
--rw-r--r--   0        0        0     7874 2024-03-13 11:26:23.429205 eve2cml-0.1.0b1/src/eve2cml/eve/lab.py
--rw-r--r--   0        0        0     1179 2024-03-08 12:06:46.370807 eve2cml-0.1.0b1/src/eve2cml/eve/network.py
--rw-r--r--   0        0        0     5937 2024-03-12 08:18:39.899336 eve2cml-0.1.0b1/src/eve2cml/eve/node.py
--rw-r--r--   0        0        0     2107 2024-03-12 08:36:10.681337 eve2cml-0.1.0b1/src/eve2cml/eve/objects.py
--rw-r--r--   0        0        0     1077 2024-03-08 16:31:50.754881 eve2cml-0.1.0b1/src/eve2cml/eve/task.py
--rw-r--r--   0        0        0     9961 2024-03-12 08:40:57.396562 eve2cml-0.1.0b1/src/eve2cml/eve/textobject.py
--rw-r--r--   0        0        0      417 2024-03-08 14:08:19.532357 eve2cml-0.1.0b1/src/eve2cml/eve/topology.py
--rw-r--r--   0        0        0     1674 2024-03-12 07:59:30.375216 eve2cml-0.1.0b1/src/eve2cml/log.py
--rw-r--r--   0        0        0     7301 2024-03-13 10:42:16.954687 eve2cml-0.1.0b1/src/eve2cml/main.py
--rw-r--r--   0        0        0        0 2024-03-11 11:57:30.331045 eve2cml-0.1.0b1/src/eve2cml/map_data/__init__.py
--rw-r--r--   0        0        0     5300 2024-03-12 12:33:25.279864 eve2cml-0.1.0b1/src/eve2cml/map_data/default.yaml
--rw-r--r--   0        0        0     3275 2024-03-13 10:17:07.238473 eve2cml-0.1.0b1/src/eve2cml/mapper.py
--rw-r--r--   0        0        0        0 2024-03-05 09:48:58.793209 eve2cml-0.1.0b1/tests/__init__.py
--rw-r--r--   0        0        0      516 2024-03-13 11:35:39.763285 eve2cml-0.1.0b1/tests/requirements.txt
--rw-r--r--   0        0        0      447 2024-03-12 09:36:41.602131 eve2cml-0.1.0b1/tests/test_decode.py
--rw-r--r--   0        0        0     1845 2024-03-13 11:14:11.862480 eve2cml-0.1.0b1/tests/test_integration.py
--rw-r--r--   0        0        0     1058 2024-03-12 09:37:55.879401 eve2cml-0.1.0b1/tests/test_logging.py
--rw-r--r--   0        0        0     1043 2024-03-12 09:25:02.378964 eve2cml-0.1.0b1/tests/test_rgb_to_hex.py
--rw-r--r--   0        0        0     1961 2024-03-12 09:08:23.088301 eve2cml-0.1.0b1/tests/testdata/hub.unl
--rw-r--r--   0        0        0     1291 2024-03-13 11:25:57.501109 eve2cml-0.1.0b1/tests/testdata/nat.unl
--rw-r--r--   0        0        0     1036 2024-03-13 10:05:43.853858 eve2cml-0.1.0b1/tests/testdata/pnet.unl
--rw-r--r--   0        0        0     3405 2024-03-13 10:03:13.597125 eve2cml-0.1.0b1/tests/testdata/test.unl
--rw-r--r--   0        0        0     1494 2024-03-12 10:13:29.869315 eve2cml-0.1.0b1/tests/testdata/test.zip
--rw-r--r--   0        0        0     5752 1970-01-01 00:00:00.000000 eve2cml-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-03-12 12:50:05.022091 eve2cml-0.1.0b2/LICENSE
+-rw-r--r--   0        0        0     6176 2024-04-11 10:48:57.012784 eve2cml-0.1.0b2/README.md
+-rw-r--r--   0        0        0     1279 2024-04-11 10:50:48.724868 eve2cml-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-08 09:09:17.161399 eve2cml-0.1.0b2/src/eve2cml/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-11 10:50:48.720868 eve2cml-0.1.0b2/src/eve2cml/_version.py
+-rw-r--r--   0        0        0      446 2024-03-12 10:40:45.713918 eve2cml-0.1.0b2/src/eve2cml/eve/__init__.py
+-rw-r--r--   0        0        0      805 2024-03-08 12:06:50.314821 eve2cml-0.1.0b2/src/eve2cml/eve/config.py
+-rw-r--r--   0        0        0      854 2024-03-08 12:06:46.366807 eve2cml-0.1.0b2/src/eve2cml/eve/configset.py
+-rw-r--r--   0        0        0      367 2024-03-08 10:48:43.230941 eve2cml-0.1.0b2/src/eve2cml/eve/decode.py
+-rw-r--r--   0        0        0     2534 2024-04-11 10:48:57.012784 eve2cml-0.1.0b2/src/eve2cml/eve/interface.py
+-rw-r--r--   0        0        0     7874 2024-03-13 11:26:23.429205 eve2cml-0.1.0b2/src/eve2cml/eve/lab.py
+-rw-r--r--   0        0        0     1179 2024-03-08 12:06:46.370807 eve2cml-0.1.0b2/src/eve2cml/eve/network.py
+-rw-r--r--   0        0        0     6107 2024-04-11 10:48:57.012784 eve2cml-0.1.0b2/src/eve2cml/eve/node.py
+-rw-r--r--   0        0        0     2107 2024-03-12 08:36:10.681337 eve2cml-0.1.0b2/src/eve2cml/eve/objects.py
+-rw-r--r--   0        0        0     1077 2024-03-08 16:31:50.754881 eve2cml-0.1.0b2/src/eve2cml/eve/task.py
+-rw-r--r--   0        0        0     9961 2024-03-12 08:40:57.396562 eve2cml-0.1.0b2/src/eve2cml/eve/textobject.py
+-rw-r--r--   0        0        0      417 2024-03-08 14:08:19.532357 eve2cml-0.1.0b2/src/eve2cml/eve/topology.py
+-rw-r--r--   0        0        0     1674 2024-03-12 07:59:30.375216 eve2cml-0.1.0b2/src/eve2cml/log.py
+-rw-r--r--   0        0        0     7301 2024-03-13 10:42:16.954687 eve2cml-0.1.0b2/src/eve2cml/main.py
+-rw-r--r--   0        0        0        0 2024-03-11 11:57:30.331045 eve2cml-0.1.0b2/src/eve2cml/map_data/__init__.py
+-rw-r--r--   0        0        0     5803 2024-04-11 10:48:57.012784 eve2cml-0.1.0b2/src/eve2cml/map_data/default.yaml
+-rw-r--r--   0        0        0     3275 2024-03-13 10:17:07.238473 eve2cml-0.1.0b2/src/eve2cml/mapper.py
+-rw-r--r--   0        0        0        0 2024-03-05 09:48:58.793209 eve2cml-0.1.0b2/tests/__init__.py
+-rw-r--r--   0        0        0      516 2024-03-13 11:35:39.763285 eve2cml-0.1.0b2/tests/requirements.txt
+-rw-r--r--   0        0        0      447 2024-03-12 09:36:41.602131 eve2cml-0.1.0b2/tests/test_decode.py
+-rw-r--r--   0        0        0     1845 2024-03-13 11:14:11.862480 eve2cml-0.1.0b2/tests/test_integration.py
+-rw-r--r--   0        0        0     1058 2024-03-12 09:37:55.879401 eve2cml-0.1.0b2/tests/test_logging.py
+-rw-r--r--   0        0        0     1043 2024-03-12 09:25:02.378964 eve2cml-0.1.0b2/tests/test_rgb_to_hex.py
+-rw-r--r--   0        0        0     1961 2024-03-12 09:08:23.088301 eve2cml-0.1.0b2/tests/testdata/hub.unl
+-rw-r--r--   0        0        0     1291 2024-03-13 11:25:57.501109 eve2cml-0.1.0b2/tests/testdata/nat.unl
+-rw-r--r--   0        0        0     1036 2024-03-13 10:05:43.853858 eve2cml-0.1.0b2/tests/testdata/pnet.unl
+-rw-r--r--   0        0        0     3405 2024-03-13 10:03:13.597125 eve2cml-0.1.0b2/tests/testdata/test.unl
+-rw-r--r--   0        0        0     1494 2024-03-12 10:13:29.869315 eve2cml-0.1.0b2/tests/testdata/test.zip
+-rw-r--r--   0        0        0     6512 1970-01-01 00:00:00.000000 eve2cml-0.1.0b2/PKG-INFO
```

### Comparing `eve2cml-0.1.0b1/LICENSE` & `eve2cml-0.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/README.md` & `eve2cml-0.1.0b2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,23 @@
+Metadata-Version: 2.1
+Name: eve2cml
+Version: 0.1.0b2
+Summary: A CLI tool to convert EVE-NG XML topology data into CML2 topology data as YAML
+Author-Email: Ralph Schmieder <rschmied@cisco.com>
+License: MIT
+Requires-Python: >=3.8
+Requires-Dist: beautifulsoup4>=4.12.3
+Requires-Dist: pyyaml>=6.0.1
+Description-Content-Type: text/markdown
+
 # eve2cml
 
 [![PyPI version](https://badge.fury.io/py/eve2cml.svg)](https://pypi.org/project/eve2cml/) [![Coverage Status](https://coveralls.io/repos/github/CiscoDevNet/eve2cml/badge.svg?branch=main)](https://coveralls.io/github/CiscoDevNet/eve2cml?branch=main) [![GH workflow](https://github.com/CiscoDevNet/eve2cml/actions/workflows/python-package.yml/badge.svg)](https://github.com/CiscoDevNet/eve2cml/actions/workflows/python-package.yml)
 
-![image showing a topology conversion](./assets/header.png)
+![image showing a topology conversion](https://raw.githubusercontent.com/CiscoDevNet/eve2cml/main/assets/header.png)
 
 Convert EVE-NG topology files either in ZIP format or in plain-text XML (.unl) to CML2 YAML format.
 
 > [!CAUTION]
 >
 > This is considered "beta" as in "it works for me but might have bugs or things don't work as you expect them to work."  So, use with care and at your own risk.
 
@@ -22,15 +33,15 @@
 
 - `map`: Maps EVE node types into CML node and image definitions.  The map key is an EVE node type where the format is "eve-node-type:eve-node-template:eve-node-image" (separated by colons).  An example is `qemu:linux`.  When the image part is missing then the CML default image for the mapped node type is used.  The value for each key is of the form:
 
   - `image_def`: the CML image definition ID for this node definition ID (can safely be null/undefined)
   - `node_def`: the mapped CML node definition ID
   - `override`: a boolean. It determines whether values like CPU or memory should be taken from the EVE definition.  If `true` then the EVE values will not be used, the default values from CML for this particular node type will then be used instead
 
-  There's a specific "corner case" where the type is identical to the template (e.g. "iol:iol" or "docker:docker").  In this particular case, mapper keys are searched for partial matches where the map key matches the beginning of the provided EVE image.  For example, "iol:iol:i86bi_linux_l2-ipbasek9:" matches all IOL images that start with `i86bi_linux-ipbasek9` and maps them (by default) into `ioll2-xe`.
+  There's a specific "corner case" where the type is identical to the template (e.g. "iol:iol" or "docker:docker").  In this particular case, mapper keys are searched for partial matches where the map key matches the beginning of the provided EVE image.  For example, "iol:iol:i86bi_linux_l2:" matches all IOL images that start with `i86bi_linux_l2` and maps them (by default) into `ioll2-xe`.
 
 After modification / adding more or different node type mappings to the exported map YAML, use the file via the `--mapper modified_map.yaml` flag.
 
 Disclaimer:  There's certainly things out there which do not properly translate.  If you encounter anything then raise an issue in the issue tracker and I'll look into it.
 
 ### Usage
 
@@ -63,17 +74,25 @@
 
 If you have a more complete map file with additional or more specific node type mappings or if you have improved the code, fixed a bug or a typo or added a new feature then I more than welcome you to raise a pull request!
 
 ### Issues
 
 If you encounter any issues with the converter then please open a issue in the [GitHub issue tracker](https://github.com/CiscoDevNet/eve2cml/issues).
 
+#### IOL interfaces
+
+There's a known issue with the maximum number of interfaces defined in the shipping node definitions for IOL and IOL-L2.  As for the released version of CML 2.7.0, the maximum number of interfaces is 16.  If you have topologies which use more interfaces (`Ethernet4/0` and up) then you need to add the additional interfaces to the node definition in CML (Tools -> Node and image definitions -> IOL / IOL-L2).  In the interface section, add the required interfaces and name them properly.  Don't forget to click "Update" at the bottom when done.
+
+This is likely fixed in the 2.7.1 release, once available.
+
+The converter has now 32 interfaces defined in the mapper (`Ethernet0/0` to `Ethernet7/3`).
+
 #### Known issues
 
-There's a few things which are known to cause issues.  Some of them might be addressable by code changes in the converter and/or changes on the CML side of things.  And some might just not be possible at all.  
+There's a few things which are known to cause issues.  Some of them might be addressable by code changes in the converter and/or changes on the CML side of things.  And some might just not be possible at all.
 
 - Rotation of annotation only works for text.  Ellipses and rectangles don't support rotation on the CML side of things.  To be addressed in a future CML release
 - Text objects in EVE can have a background color.  The converter adds additional rectangles behind the text object in CML.  It "guesses" the size of these rectangles.  Those guesses are inaccurate.
 - Font (names) might not translate well.  I think there's a general issue with serif vs. sans-serif mapping.
 - Images (PNGs) as part of a topology are ignored as there's no representation for them in CML.
 - More complex text boxes in EVE do not translate well into the more simple text annotation of CML.  For color, size and font name, the first occurrence is used for the entire text object.  Things like bullet lists etc. are completely ignored.
 - EVE multi-point networks are represented by unmanaged switches in CML.  They have max 32 ports.  That might not be enough.
```

### Comparing `eve2cml-0.1.0b1/pyproject.toml` & `eve2cml-0.1.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 dependencies = [
     "beautifulsoup4>=4.12.3",
     "pyyaml>=6.0.1",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.1.0b1"
+version = "0.1.0b2"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 eve2cml = "eve2cml.main:main"
```

### Comparing `eve2cml-0.1.0b1/src/eve2cml/eve/config.py` & `eve2cml-0.1.0b2/src/eve2cml/eve/config.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/src/eve2cml/eve/configset.py` & `eve2cml-0.1.0b2/src/eve2cml/eve/configset.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/src/eve2cml/eve/interface.py` & `eve2cml-0.1.0b2/src/eve2cml/eve/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,17 @@
         # private, for linking
         self.node_id = node_id
         self.slot = slot
 
     def __str__(self):
         return f"ID: {self.id}, Name: {self.name}, Type: {self.obj_type}, NetID: {self.network_id}"
 
+    def __repr__(self):
+        return f"{self.__class__.__name__}(id={self.id}, slot={self.slot})"
+
     def as_cml_dict(self, idx, node_def, lab):
         return {
             "id": f"i{idx}",
             "label": lab.mapper.cml_iface_label(self.slot, node_def, self.name),
             "slot": self.slot,
             "type": "physical",
         }
```

### Comparing `eve2cml-0.1.0b1/src/eve2cml/eve/lab.py` & `eve2cml-0.1.0b2/src/eve2cml/eve/lab.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/src/eve2cml/eve/network.py` & `eve2cml-0.1.0b2/src/eve2cml/eve/network.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/src/eve2cml/eve/node.py` & `eve2cml-0.1.0b2/src/eve2cml/eve/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,27 +70,32 @@
     def as_cml_dict(self, node_id: int, lab: "Lab"):
         nd_map = lab.mapper.node_def(self.obj_type, self.template, self.image)
 
         temp_list: List[Interface] = []
         prev = 0
         for idx, iface in enumerate(self.interfaces):
             delta = iface.slot - prev
+            _LOGGER.debug(
+                "idx, slot, prev, delta %d/%d/%d/%d", idx, iface.slot, prev, delta
+            )
             for idx2 in range(delta):
                 temp_list.append(
                     Interface(
                         id=idx + idx2,
                         obj_type=self.obj_type,
                         network_id=999999,
                         name="filler",
-                        slot=idx + idx2,
+                        slot=prev + idx2,
                     )
                 )
             temp_list.append(iface)
             prev = iface.slot + 1
 
+        _LOGGER.debug("list %s", temp_list)
+
         iface_count = len(temp_list)
         iface_diff = int(self.ethernet) - iface_count
         if iface_diff > 0:
             _LOGGER.info(
                 "Filler interfaces needed for Node %d/%s, add %d",
                 self.id,
                 self.name,
```

### Comparing `eve2cml-0.1.0b1/src/eve2cml/eve/objects.py` & `eve2cml-0.1.0b2/src/eve2cml/eve/objects.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/src/eve2cml/eve/task.py` & `eve2cml-0.1.0b2/src/eve2cml/eve/task.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/src/eve2cml/eve/textobject.py` & `eve2cml-0.1.0b2/src/eve2cml/eve/textobject.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/src/eve2cml/log.py` & `eve2cml-0.1.0b2/src/eve2cml/log.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/src/eve2cml/main.py` & `eve2cml-0.1.0b2/src/eve2cml/main.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/src/eve2cml/map_data/default.yaml` & `eve2cml-0.1.0b2/src/eve2cml/map_data/default.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,30 @@
   - Ethernet2/1
   - Ethernet2/2
   - Ethernet2/3
   - Ethernet3/0
   - Ethernet3/1
   - Ethernet3/2
   - Ethernet3/3
+  - Ethernet4/0
+  - Ethernet4/1
+  - Ethernet4/2
+  - Ethernet4/3
+  - Ethernet5/0
+  - Ethernet5/1
+  - Ethernet5/2
+  - Ethernet5/3
+  - Ethernet6/0
+  - Ethernet6/1
+  - Ethernet6/2
+  - Ethernet6/3
+  - Ethernet7/0
+  - Ethernet7/1
+  - Ethernet7/2
+  - Ethernet7/3
   ioll2-xe:
   - Ethernet0/0
   - Ethernet0/1
   - Ethernet0/2
   - Ethernet0/3
   - Ethernet1/0
   - Ethernet1/1
@@ -101,14 +117,30 @@
   - Ethernet2/1
   - Ethernet2/2
   - Ethernet2/3
   - Ethernet3/0
   - Ethernet3/1
   - Ethernet3/2
   - Ethernet3/3
+  - Ethernet4/0
+  - Ethernet4/1
+  - Ethernet4/2
+  - Ethernet4/3
+  - Ethernet5/0
+  - Ethernet5/1
+  - Ethernet5/2
+  - Ethernet5/3
+  - Ethernet6/0
+  - Ethernet6/1
+  - Ethernet6/2
+  - Ethernet6/3
+  - Ethernet7/0
+  - Ethernet7/1
+  - Ethernet7/2
+  - Ethernet7/3
   iosv:
   - GigabitEthernet0/0
   - GigabitEthernet0/1
   - GigabitEthernet0/2
   - GigabitEthernet0/3
   - GigabitEthernet0/4
   - GigabitEthernet0/5
@@ -267,15 +299,15 @@
     image_def: null
     node_def: unmanaged_switch
     override: true
   docker:docker:
     image_def: null
     node_def: desktop
     override: true
-  iol:iol:i86bi_linux_l2-ipbasek9:
+  iol:iol:i86bi_linux_l2:
     image_def: null
     node_def: ioll2-xe
     override: false
   iol:iol:
     image_def: null
     node_def: iol-xe
     override: false
```

### Comparing `eve2cml-0.1.0b1/src/eve2cml/mapper.py` & `eve2cml-0.1.0b2/src/eve2cml/mapper.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/tests/requirements.txt` & `eve2cml-0.1.0b2/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/tests/test_integration.py` & `eve2cml-0.1.0b2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/tests/test_logging.py` & `eve2cml-0.1.0b2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/tests/test_rgb_to_hex.py` & `eve2cml-0.1.0b2/tests/test_rgb_to_hex.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/tests/testdata/hub.unl` & `eve2cml-0.1.0b2/tests/testdata/hub.unl`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/tests/testdata/nat.unl` & `eve2cml-0.1.0b2/tests/testdata/nat.unl`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/tests/testdata/pnet.unl` & `eve2cml-0.1.0b2/tests/testdata/pnet.unl`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/tests/testdata/test.unl` & `eve2cml-0.1.0b2/tests/testdata/test.unl`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/tests/testdata/test.zip` & `eve2cml-0.1.0b2/tests/testdata/test.zip`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b1/PKG-INFO` & `eve2cml-0.1.0b2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,12 @@
-Metadata-Version: 2.1
-Name: eve2cml
-Version: 0.1.0b1
-Summary: A CLI tool to convert EVE-NG XML topology data into CML2 topology data as YAML
-Author-Email: Ralph Schmieder <rschmied@cisco.com>
-License: MIT
-Requires-Python: >=3.8
-Requires-Dist: beautifulsoup4>=4.12.3
-Requires-Dist: pyyaml>=6.0.1
-Description-Content-Type: text/markdown
-
 # eve2cml
 
 [![PyPI version](https://badge.fury.io/py/eve2cml.svg)](https://pypi.org/project/eve2cml/) [![Coverage Status](https://coveralls.io/repos/github/CiscoDevNet/eve2cml/badge.svg?branch=main)](https://coveralls.io/github/CiscoDevNet/eve2cml?branch=main) [![GH workflow](https://github.com/CiscoDevNet/eve2cml/actions/workflows/python-package.yml/badge.svg)](https://github.com/CiscoDevNet/eve2cml/actions/workflows/python-package.yml)
 
-![image showing a topology conversion](./assets/header.png)
+![image showing a topology conversion](https://raw.githubusercontent.com/CiscoDevNet/eve2cml/main/assets/header.png)
 
 Convert EVE-NG topology files either in ZIP format or in plain-text XML (.unl) to CML2 YAML format.
 
 > [!CAUTION]
 >
 > This is considered "beta" as in "it works for me but might have bugs or things don't work as you expect them to work."  So, use with care and at your own risk.
 
@@ -33,15 +22,15 @@
 
 - `map`: Maps EVE node types into CML node and image definitions.  The map key is an EVE node type where the format is "eve-node-type:eve-node-template:eve-node-image" (separated by colons).  An example is `qemu:linux`.  When the image part is missing then the CML default image for the mapped node type is used.  The value for each key is of the form:
 
   - `image_def`: the CML image definition ID for this node definition ID (can safely be null/undefined)
   - `node_def`: the mapped CML node definition ID
   - `override`: a boolean. It determines whether values like CPU or memory should be taken from the EVE definition.  If `true` then the EVE values will not be used, the default values from CML for this particular node type will then be used instead
 
-  There's a specific "corner case" where the type is identical to the template (e.g. "iol:iol" or "docker:docker").  In this particular case, mapper keys are searched for partial matches where the map key matches the beginning of the provided EVE image.  For example, "iol:iol:i86bi_linux_l2-ipbasek9:" matches all IOL images that start with `i86bi_linux-ipbasek9` and maps them (by default) into `ioll2-xe`.
+  There's a specific "corner case" where the type is identical to the template (e.g. "iol:iol" or "docker:docker").  In this particular case, mapper keys are searched for partial matches where the map key matches the beginning of the provided EVE image.  For example, "iol:iol:i86bi_linux_l2:" matches all IOL images that start with `i86bi_linux_l2` and maps them (by default) into `ioll2-xe`.
 
 After modification / adding more or different node type mappings to the exported map YAML, use the file via the `--mapper modified_map.yaml` flag.
 
 Disclaimer:  There's certainly things out there which do not properly translate.  If you encounter anything then raise an issue in the issue tracker and I'll look into it.
 
 ### Usage
 
@@ -74,17 +63,25 @@
 
 If you have a more complete map file with additional or more specific node type mappings or if you have improved the code, fixed a bug or a typo or added a new feature then I more than welcome you to raise a pull request!
 
 ### Issues
 
 If you encounter any issues with the converter then please open a issue in the [GitHub issue tracker](https://github.com/CiscoDevNet/eve2cml/issues).
 
+#### IOL interfaces
+
+There's a known issue with the maximum number of interfaces defined in the shipping node definitions for IOL and IOL-L2.  As for the released version of CML 2.7.0, the maximum number of interfaces is 16.  If you have topologies which use more interfaces (`Ethernet4/0` and up) then you need to add the additional interfaces to the node definition in CML (Tools -> Node and image definitions -> IOL / IOL-L2).  In the interface section, add the required interfaces and name them properly.  Don't forget to click "Update" at the bottom when done.
+
+This is likely fixed in the 2.7.1 release, once available.
+
+The converter has now 32 interfaces defined in the mapper (`Ethernet0/0` to `Ethernet7/3`).
+
 #### Known issues
 
-There's a few things which are known to cause issues.  Some of them might be addressable by code changes in the converter and/or changes on the CML side of things.  And some might just not be possible at all.  
+There's a few things which are known to cause issues.  Some of them might be addressable by code changes in the converter and/or changes on the CML side of things.  And some might just not be possible at all.
 
 - Rotation of annotation only works for text.  Ellipses and rectangles don't support rotation on the CML side of things.  To be addressed in a future CML release
 - Text objects in EVE can have a background color.  The converter adds additional rectangles behind the text object in CML.  It "guesses" the size of these rectangles.  Those guesses are inaccurate.
 - Font (names) might not translate well.  I think there's a general issue with serif vs. sans-serif mapping.
 - Images (PNGs) as part of a topology are ignored as there's no representation for them in CML.
 - More complex text boxes in EVE do not translate well into the more simple text annotation of CML.  For color, size and font name, the first occurrence is used for the entire text object.  Things like bullet lists etc. are completely ignored.
 - EVE multi-point networks are represented by unmanaged switches in CML.  They have max 32 ports.  That might not be enough.
```

