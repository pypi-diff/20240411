# Comparing `tmp/btrview-0.4.0.tar.gz` & `tmp/btrview-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrview-0.4.0.tar", last modified: Wed Apr  3 01:49:02 2024, max compression
+gzip compressed data, was "btrview-0.5.0.tar", last modified: Wed Apr 10 20:48:29 2024, max compression
```

## Comparing `btrview-0.4.0.tar` & `btrview-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-03 01:49:02.182009 btrview-0.4.0/
--rw-r--r--   0 chris     (1000) chris     (1000)     1069 2023-05-17 21:10:51.000000 btrview-0.4.0/LICENSE.md
--rw-r--r--   0 chris     (1000) chris     (1000)     7557 2024-04-03 01:49:02.182009 btrview-0.4.0/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     5932 2024-04-02 00:28:22.000000 btrview-0.4.0/README.md
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-03 01:49:02.182009 btrview-0.4.0/btrview/
--rw-r--r--   0 chris     (1000) chris     (1000)       65 2024-04-03 01:44:27.000000 btrview-0.4.0/btrview/__init__.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     2402 2024-04-03 01:44:21.000000 btrview-0.4.0/btrview/__main__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6911 2024-04-03 01:22:12.000000 btrview-0.4.0/btrview/btrfs.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-03 01:49:02.182009 btrview-0.4.0/btrview/scripts/
--rwxr-xr-x   0 chris     (1000) chris     (1000)     1660 2024-03-12 18:06:35.000000 btrview-0.4.0/btrview/scripts/btrsend.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     2402 2024-04-03 01:44:21.000000 btrview-0.4.0/btrview/scripts/btrview.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7202 2024-04-03 01:44:27.000000 btrview-0.4.0/btrview/subvolume.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-04-03 01:10:36.000000 btrview-0.4.0/btrview/utils.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-03 01:49:02.182009 btrview-0.4.0/btrview.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     7557 2024-04-03 01:49:02.000000 btrview-0.4.0/btrview.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)      372 2024-04-03 01:49:02.000000 btrview-0.4.0/btrview.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-04-03 01:49:02.000000 btrview-0.4.0/btrview.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-04-03 01:49:02.000000 btrview-0.4.0/btrview.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-04-03 01:49:02.000000 btrview-0.4.0/btrview.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-04-03 01:49:02.000000 btrview-0.4.0/btrview.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)      923 2024-04-03 01:44:27.000000 btrview-0.4.0/pyproject.toml
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-04-03 01:49:02.182009 btrview-0.4.0/setup.cfg
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-10 20:48:29.356026 btrview-0.5.0/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1069 2023-05-17 21:10:51.000000 btrview-0.5.0/LICENSE.md
+-rw-r--r--   0 chris     (1000) chris     (1000)     5948 2024-04-10 20:48:29.356026 btrview-0.5.0/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     4067 2024-04-10 20:27:39.000000 btrview-0.5.0/README.md
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-10 20:48:29.356026 btrview-0.5.0/btrview/
+-rw-r--r--   0 chris     (1000) chris     (1000)       77 2024-04-10 20:36:39.000000 btrview-0.5.0/btrview/__init__.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     1843 2024-04-10 20:33:52.000000 btrview-0.5.0/btrview/__main__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6935 2024-04-10 16:19:25.000000 btrview-0.5.0/btrview/btrfs.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-10 20:48:29.356026 btrview-0.5.0/btrview/scripts/
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     1660 2024-04-10 13:31:52.000000 btrview-0.5.0/btrview/scripts/btrsend.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     1843 2024-04-10 20:33:52.000000 btrview-0.5.0/btrview/scripts/btrview.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7642 2024-04-10 20:22:21.000000 btrview-0.5.0/btrview/subvolume.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-04-10 13:31:52.000000 btrview-0.5.0/btrview/utils.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-10 20:48:29.356026 btrview-0.5.0/btrview.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     5948 2024-04-10 20:48:29.000000 btrview-0.5.0/btrview.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)      372 2024-04-10 20:48:29.000000 btrview-0.5.0/btrview.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-04-10 20:48:29.000000 btrview-0.5.0/btrview.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-04-10 20:48:29.000000 btrview-0.5.0/btrview.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       64 2024-04-10 20:48:29.000000 btrview-0.5.0/btrview.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-04-10 20:48:29.000000 btrview-0.5.0/btrview.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)     1072 2024-04-10 20:48:24.000000 btrview-0.5.0/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-04-10 20:48:29.356026 btrview-0.5.0/setup.cfg
```

### Comparing `btrview-0.4.0/LICENSE.md` & `btrview-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `btrview-0.4.0/btrview/__main__.py` & `btrview-0.5.0/btrview/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,53 @@
 #!/usr/bin/env python
-
 import argparse
-import textwrap
-from itertools import zip_longest
 
 import btrview
 from btrview.utils import check_root
-from btrview.btrfs import Btrfs, get_forest
+from btrview.rich_output import logic
 
 def parser() -> argparse.ArgumentParser:
     """Returns the argument parser for the command line arguments"""
     arg_parser = argparse.ArgumentParser(
             description = "Better way to view btrfs filesystems.",
             epilog = f"btrview version {btrview.__version__}, created by Chris Copley")
 
     arg_parser.add_argument(
             "--labels",
-            help="The label of the filesystem to view",
+            help="The label of the filesystem(s) to view",
             nargs="+",)
 
     arg_parser.add_argument(
             "--include",
-            help = "Types of subvolumes to include in the tree",
+            help = "Types of subvolumes to include in the tree. Default are root and unreachable.",
             nargs = "*",
             choices = ("root","deleted","unreachable"),
             default = ("root","unreachable"))
 
     arg_parser.add_argument(
             "--property",
-            help = "The subvolume property to print out in the tree",
-            default = None)
+            help = "The subvolume property to print out in the tree. These are the keys from the `btrfs subvolume show` command.",)
 
-    return arg_parser
+    arg_parser.add_argument(
+            "--fold",
+            help = "Fold child output greater than N lines.",
+            metavar = "N",
+            type = int)
 
-def logic(labels: list[str], root, deleted, unreachable, prop) -> None:
-    check_root()
-    filesystems = Btrfs.get_filesystems(labels)
-    for fs in filesystems:
-        print(f"{fs}")
-        subvols = fs.subvolumes(root,deleted,unreachable)
-        subvol_tree = get_forest([s for s in subvols if not s.deleted],"subvol")
-        subvol_str = get_forest_string(subvol_tree, "Subvolumes", prop)
-
-        snap_tree = get_forest(subvols,"snap")
-        snap_str = get_forest_string(snap_tree, "Snapshots", prop)
-
-        zipper = zip_longest(subvol_str.splitlines(),snap_str.splitlines(),fillvalue="")
-        for subvol_line, snap_line in zipper:
-            print(f"{subvol_line:<50}{snap_line:}")
-
-def get_forest_string(forest, header, prop: str = ""):
-    forest_str = f"{header}:\n"
-    for tree in forest:
-        #stdout=False is only needed because of bug
-        #see https://github.com/caesar0301/treelib/issues/221
-        tree_str = tree.show(data_property=prop, stdout=False)
-        forest_str += textwrap.indent(str(tree_str), "  ")
-    return forest_str
+    arg_parser.add_argument(
+            "--export",
+            choices = ("text","svg","html"),
+            help = "Export the specifed type instead of a rich table. Using this flag will still write to stdout. If you wish to save to a file use shell redirection.",)
+
+    return arg_parser
 
 def main():
+    check_root()
     args = parser().parse_args()
     root = "root" in args.include
     deleted = "deleted" in args.include
     unreachable = "unreachable" in args.include
-    logic(args.labels, root ,deleted, unreachable, args.property)
-    
+    output = logic(args.labels, root, deleted, unreachable, args.property, args.fold, args.export)
+    print(output)
+ 
 if __name__ == "__main__":
     main()
-
```

### Comparing `btrview-0.4.0/btrview/btrfs.py` & `btrview-0.5.0/btrview/btrfs.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,19 +59,22 @@
         return filesystems
 
     @classmethod
     def _get_deleted_subvols(cls, subvols: list[Subvolume]) -> list[Subvolume]:
         """Returns a list of deleted subvolumes"""
         uuids = {s.id("snap") for s in subvols}
         puuids = set()
+        deleted_subvols = []
         for subvol in subvols:
             puuid = subvol.parent("snap")
-            if puuid and (puuid not in uuids):
+            if puuid and (puuid not in uuids) and (puuid not in puuids):
                 puuids.add(puuid)
-        return [Subvolume({"UUID":puuid}, tuple(), deleted=True) for puuid in puuids]
+                deleted_dict = {"UUID":puuid,"Subvolume ID":puuid, "Name":puuid}
+                deleted_subvols.append(Subvolume(deleted_dict,tuple(),deleted=True))
+        return deleted_subvols
             
     def subvolumes(self, root: bool, deleted: bool, unreachable: bool,) -> list[Subvolume]:
         """Return a list of subvolumes on the file system"""
         mount_point = self.mounts[0].target 
         out = run(f"sudo btrfs subvolume list -apcguqR {mount_point}")
 
         subvols = []
@@ -82,16 +85,16 @@
             match_dict = {}
             for key,val in key_dict.items():
                 match = re.search(f"\\b{key}\\s+(\\S+)",line)
                 if match and match.group(1) == "-":
                     match_dict[val] = None
                 elif match :
                     match_dict[val] = match.group(1)
-            path_match = re.search(r"path\s*(.*)",line).group(1).removeprefix("<FS_TREE>")
-            match_dict["btrfs Path"] = Path(f"/{path_match}".replace("//","/",1))
+            path_match = re.search(r"path\s*(.*)",line).group(1).removeprefix("<FS_TREE>/")
+            match_dict["btrfs Path"] = Path(f"/{path_match}")
             match_dict["Name"] = match_dict["btrfs Path"].name
             subvols.append(Subvolume(match_dict,self.mounts))
         if not unreachable:
             to_remove = []
             for subvol in subvols:
                 if not subvol.mounted:
                     to_remove.append(subvol)
@@ -107,22 +110,18 @@
             subvols.extend(self._get_deleted_subvols(subvols))
         return subvols
 
     def forest(self, snapshots = False, root = True, deleted = False, unreachable = True,) -> list[Tree]:
         """Returns a forest of subvolumes with parent/child relationships
         being based on subvolume layout or snapshots."""
         kind = "snap" if snapshots else "subvol"
-        if kind == "subvol":
-            deleted = False
         return get_forest(self.subvolumes(root, deleted, unreachable), kind)
         
     def __str__(self) -> str:
-        label =  f"Label: {self.label}"
-        uuid = f"UUID: {self.uuid}"
-        return f"{label}\n{uuid}"
+        return f"{self.label or self.uuid}"
 
 def subvol_in_list(ID: str, subvolumes: list[Subvolume], kind = "subvol") -> Subvolume | None:
     """Returns a subvolume from a list if there, else returns None."""
     for subvolume in subvolumes:
         if subvolume.id(kind) == ID:
             return subvolume
     return None
```

### Comparing `btrview-0.4.0/btrview/scripts/btrsend.py` & `btrview-0.5.0/btrview/scripts/btrsend.py`

 * *Files identical despite different names*

### Comparing `btrview-0.4.0/btrview/scripts/btrview.py` & `btrview-0.5.0/btrview/scripts/btrview.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,53 @@
 #!/usr/bin/env python
-
 import argparse
-import textwrap
-from itertools import zip_longest
 
 import btrview
 from btrview.utils import check_root
-from btrview.btrfs import Btrfs, get_forest
+from btrview.rich_output import logic
 
 def parser() -> argparse.ArgumentParser:
     """Returns the argument parser for the command line arguments"""
     arg_parser = argparse.ArgumentParser(
             description = "Better way to view btrfs filesystems.",
             epilog = f"btrview version {btrview.__version__}, created by Chris Copley")
 
     arg_parser.add_argument(
             "--labels",
-            help="The label of the filesystem to view",
+            help="The label of the filesystem(s) to view",
             nargs="+",)
 
     arg_parser.add_argument(
             "--include",
-            help = "Types of subvolumes to include in the tree",
+            help = "Types of subvolumes to include in the tree. Default are root and unreachable.",
             nargs = "*",
             choices = ("root","deleted","unreachable"),
             default = ("root","unreachable"))
 
     arg_parser.add_argument(
             "--property",
-            help = "The subvolume property to print out in the tree",
-            default = None)
+            help = "The subvolume property to print out in the tree. These are the keys from the `btrfs subvolume show` command.",)
 
-    return arg_parser
+    arg_parser.add_argument(
+            "--fold",
+            help = "Fold child output greater than N lines.",
+            metavar = "N",
+            type = int)
 
-def logic(labels: list[str], root, deleted, unreachable, prop) -> None:
-    check_root()
-    filesystems = Btrfs.get_filesystems(labels)
-    for fs in filesystems:
-        print(f"{fs}")
-        subvols = fs.subvolumes(root,deleted,unreachable)
-        subvol_tree = get_forest([s for s in subvols if not s.deleted],"subvol")
-        subvol_str = get_forest_string(subvol_tree, "Subvolumes", prop)
-
-        snap_tree = get_forest(subvols,"snap")
-        snap_str = get_forest_string(snap_tree, "Snapshots", prop)
-
-        zipper = zip_longest(subvol_str.splitlines(),snap_str.splitlines(),fillvalue="")
-        for subvol_line, snap_line in zipper:
-            print(f"{subvol_line:<50}{snap_line:}")
-
-def get_forest_string(forest, header, prop: str = ""):
-    forest_str = f"{header}:\n"
-    for tree in forest:
-        #stdout=False is only needed because of bug
-        #see https://github.com/caesar0301/treelib/issues/221
-        tree_str = tree.show(data_property=prop, stdout=False)
-        forest_str += textwrap.indent(str(tree_str), "  ")
-    return forest_str
+    arg_parser.add_argument(
+            "--export",
+            choices = ("text","svg","html"),
+            help = "Export the specifed type instead of a rich table. Using this flag will still write to stdout. If you wish to save to a file use shell redirection.",)
+
+    return arg_parser
 
 def main():
+    check_root()
     args = parser().parse_args()
     root = "root" in args.include
     deleted = "deleted" in args.include
     unreachable = "unreachable" in args.include
-    logic(args.labels, root ,deleted, unreachable, args.property)
-    
+    output = logic(args.labels, root, deleted, unreachable, args.property, args.fold, args.export)
+    print(output)
+ 
 if __name__ == "__main__":
     main()
-
```

### Comparing `btrview-0.4.0/btrview/subvolume.py` & `btrview-0.5.0/btrview/subvolume.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,18 @@
         self._show = show
 
     @property
     def paths(self) -> list[Path]:
         if not self["btrfs Path"]:
             return []
         btr_path = Path(self["btrfs Path"])
-        return [mount.resolve(btr_path) for mount in self.mounts if btr_path.is_relative_to(mount.fsroot)]
+        paths = [mount.resolve(btr_path) for mount in self.mounts if btr_path.is_relative_to(mount.fsroot)]
+        paths = [path for path in paths if path.exists()]
+        return paths
+
 
     @property
     def mounted(self) -> bool:
         return bool(self.paths)
 
     @property
     def mount_points(self) -> tuple[Path, ...]:
@@ -123,28 +126,39 @@
         response = run(f"btrfs filesystem usage '{path}'")
         return response.returncode == 0
 
     def __getitem__(self, key: str) -> str | None:
         """Returns the item from the props dictionary, but instead
         of throwing a key error, returns None"""
         if key in self.props:
-            return self.props.get(key)
-        elif not self._show and not self.deleted:
+            return self.props[key]
+        elif self.deleted:
+            #just assume it's None for deleted subvols. #could cause problems
+            #in that deleted Subvolumes won't throw KeyError
+            return None
+        elif not self._show:
             cmd = f"btrfs subvolume show -u {self['UUID']} {self.mounts[0].target}"
             props = self._run_cmd(cmd)
             self.props |= props
             self._show = True
-        return self.props.get(key)
+        try:
+            return self.props[key]
+        except KeyError:
+            pass
+        try:
+            return getattr(self, key)
+        except AttributeError:
+            raise KeyError(f"Subvolume has no attribute or key '{key}'")
 
     def __str__(self) -> str:
-        string = self["Name"] or str(self["UUID"])
+        string = self["Name"]
         if mps := self.mount_points:
             mp_string = ", ".join(str(mp) for mp in mps)
             string = f"{string} on: {mp_string}"
-        return string
+        return str(string)
 
     def __hash__(self) -> int:
         return hash(self["UUID"])
 
     def __eq__(self, other) -> bool:
         return self["UUID"] == other["UUID"]
```

### Comparing `btrview-0.4.0/btrview/utils.py` & `btrview-0.5.0/btrview/utils.py`

 * *Files identical despite different names*

### Comparing `btrview-0.4.0/pyproject.toml` & `btrview-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 [project]
 name = "btrview"
-version = "0.4.0"
+version = "0.5.0"
 description = "View btrfs snapshot trees"
 readme = "README.md"
 authors = [{name = "Chris Copley"}]
 license = {file = "LICENSE.md"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["btrfs"]
 requires-python = ">=3.11"
 dependencies = [
-	"treelib"
+	"treelib",
+	"rich"
 ]
 
+[project.optional-dependencies]
+build = ["build","twine"]
+dev = ["bumpver","mypy","pip-tools"]
+
 [project.scripts]
 btrview = "btrview.scripts.btrview:main"
 
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.4.0"
+current_version = "0.5.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
 
+[tool.setuptools]
+py-modules = ["btrview"]
+
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"',
 ]
 "btrview/__init__.py" = ["{version}"]
```

