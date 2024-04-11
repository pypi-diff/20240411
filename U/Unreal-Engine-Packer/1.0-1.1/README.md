# Comparing `tmp/Unreal_Engine_Packer-1.0-py3-none-any.whl.zip` & `tmp/Unreal_Engine_Packer-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2828 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     3229 b- defN 24-Apr-10 17:04 Source/UePack.py
--rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-10 17:04 Source/__init__.py
--rw-rw-rw-  2.0 fat      387 b- defN 24-Apr-10 17:09 Unreal_Engine_Packer-1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 17:09 Unreal_Engine_Packer-1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       49 b- defN 24-Apr-10 17:09 Unreal_Engine_Packer-1.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-10 17:09 Unreal_Engine_Packer-1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      592 b- defN 24-Apr-10 17:09 Unreal_Engine_Packer-1.0.dist-info/RECORD
-7 files, 4378 bytes uncompressed, 1760 bytes compressed:  59.8%
+Zip file size: 3456 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     3830 b- defN 24-Apr-11 07:52 Source/UePack.py
+-rw-r--r--  2.0 unx       21 b- defN 24-Apr-11 07:52 Source/__init__.py
+-rw-r--r--  2.0 unx     1309 b- defN 24-Apr-11 07:53 Unreal_Engine_Packer-1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 07:53 Unreal_Engine_Packer-1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 24-Apr-11 07:53 Unreal_Engine_Packer-1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-11 07:53 Unreal_Engine_Packer-1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      593 b- defN 24-Apr-11 07:53 Unreal_Engine_Packer-1.1.dist-info/RECORD
+7 files, 5900 bytes uncompressed, 2388 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: Source/UePack.py
 Comment: 
 
 Filename: Source/__init__.py
 Comment: 
 
-Filename: Unreal_Engine_Packer-1.0.dist-info/METADATA
+Filename: Unreal_Engine_Packer-1.1.dist-info/METADATA
 Comment: 
 
-Filename: Unreal_Engine_Packer-1.0.dist-info/WHEEL
+Filename: Unreal_Engine_Packer-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: Unreal_Engine_Packer-1.0.dist-info/entry_points.txt
+Filename: Unreal_Engine_Packer-1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: Unreal_Engine_Packer-1.0.dist-info/top_level.txt
+Filename: Unreal_Engine_Packer-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: Unreal_Engine_Packer-1.0.dist-info/RECORD
+Filename: Unreal_Engine_Packer-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Source/UePack.py

```diff
@@ -1,101 +1,106 @@
-import os;
-import argparse;
-import json;
-import winreg;
-
-argument_parser = argparse.ArgumentParser()
-
-argument_parser.add_argument('-manifest')
-argument_parser.add_argument('-type', choices=['application', 'plugin'])
-argument_parser.add_argument('-engine')
-argument_parser.add_argument('-output')
-argument_parser.add_argument('-platform', default="Win64")
-argument_parser.add_argument('-config', default="Shipping")
-
-arguments = argument_parser.parse_args()
-
-if arguments.manifest is None:
-    print('Project/plugin manifest path not set')
-    exit(-1)
-
-manifest = os.path.abspath(arguments.manifest)
-
-if not os.path.isfile(manifest):
-    print('Could not find project/plugin manifest: ' + manifest)
-    exit(-1)
-
-if arguments.type is not None:
-    package_type = arguments.type
-else:
-    manfest_name, manifest_extension = os.path.splitext(manifest)
-    if manifest_extension == '.uproject':
-        package_type = 'application'
-    elif manifest_extension == '.uplugin':
-        package_type = 'plugin'
-    else:
-        print('Could not identify manifest type: ' + manifest_extension)
-        exit(-1)
-
-if arguments.engine is not None:
-    engine_version = arguments.engine
-elif package_type == 'application':
-    manifest_file = open(manifest, 'r')
-    manifest_json = json.loads(manifest_file.read())
-    engine_version = manifest_json['EngineAssociation']
-else:
-    print('Could not engine version')
-    exit(-1)
-
-if arguments.output is not None:
-    output_directory = os.path.abspath(arguments.output)
-else:
-    output_directory = os.getcwd()
-
-try:
-    engine_key = winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, 'SOFTWARE\\EpicGames\\Unreal Engine\\' + engine_version, 0, winreg.KEY_READ | winreg.KEY_WOW64_64KEY)
-    engine_location = engine_installed = winreg.QueryValueEx(engine_key, 'InstalledDirectory')[0]
-    winreg.CloseKey(engine_key)
-except Exception as ex:
-    print('Could not find UE' + engine_version)
-    exit(-1)
-
-print('Manifest: ' + manifest)
-print('Type: ' + package_type)
-print('Engine version: ' + engine_version)
-print('Engine location: ' + engine_location)
-print('Output directory: ' + output_directory)
-
-uat_path = engine_location + '\\Engine\\Build\\BatchFiles\\RunUAT.bat'
-
-command = '"' + uat_path + '"'
-
-if package_type == 'application':
-    command += ' BuildCookRun'
-    command += ' -project="' + manifest + '"'
-    command += ' -platform="' + arguments.platform + '"'
-    command += ' -clientconfig="' + arguments.config + '"'
-    command += ' -serverconfig="' + arguments.config + '"'
-    command += ' -noP4'
-    command += ' -Compressed'
-    command += ' -cook'
-    command += ' -allmaps'
-    command += ' -build'
-    command += ' -stage'
-    command += ' -pak'
-    command += ' -archive'
-    command += ' -prereqs'
-    command += ' -archivedirectory="' + output_directory + '"'
-
-elif package_type == 'plugin':
-    command += ' BuildPlugin'
-    command += ' -Plugin="' + manifest + '"'
-    command += ' -Package="' + output_directory + '"'
-    command += ' -CreateSubFolders'
-
-print(command)
-
-return_code = os.system('"' + command + '"')
-if return_code != 0:
-    exit(return_code)
-
-exit(0)
+import os;
+import argparse;
+import json;
+import winreg;
+import sys;
+
+argument_parser = argparse.ArgumentParser(description='An automation tool to package Unreal Engine projects or plugins.')
+
+argument_parser.add_argument('-manifest', help="Path to the project or plugin manifest. This is a .uproject or .uplugin file.")
+argument_parser.add_argument('-type', choices=['application', 'plugin'], help="Override automatic type detection based on the manifest. This controls whether a project will be packaged, or a plugin.")
+argument_parser.add_argument('-engine', help="Set the engine version to use. For projects this is automatically detected, but can be overridden. For plugins this argument is required.")
+argument_parser.add_argument('-output', help="Output directory where the package will be generated.")
+argument_parser.add_argument('-platform', default="Win64", help="Target platform. Only required for projects.")
+argument_parser.add_argument('-config', default="Shipping", help="Target configuration. Only required for projects.")
+
+if len(sys.argv) == 1:
+    argument_parser.print_help(sys.stderr)
+    exit(1)
+
+arguments = argument_parser.parse_args()
+
+if arguments.manifest is None:
+    print('Project/plugin manifest path not set')
+    exit(-1)
+
+manifest = os.path.abspath(arguments.manifest)
+
+if not os.path.isfile(manifest):
+    print('Could not find project/plugin manifest: ' + manifest)
+    exit(-1)
+
+if arguments.type is not None:
+    package_type = arguments.type
+else:
+    manfest_name, manifest_extension = os.path.splitext(manifest)
+    if manifest_extension == '.uproject':
+        package_type = 'application'
+    elif manifest_extension == '.uplugin':
+        package_type = 'plugin'
+    else:
+        print('Could not identify manifest type: ' + manifest_extension)
+        exit(-1)
+
+if arguments.engine is not None:
+    engine_version = arguments.engine
+elif package_type == 'application':
+    manifest_file = open(manifest, 'r')
+    manifest_json = json.loads(manifest_file.read())
+    engine_version = manifest_json['EngineAssociation']
+else:
+    print('Could not engine version')
+    exit(-1)
+
+if arguments.output is not None:
+    output_directory = os.path.abspath(arguments.output)
+else:
+    output_directory = os.getcwd()
+
+try:
+    engine_key = winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, 'SOFTWARE\\EpicGames\\Unreal Engine\\' + engine_version, 0, winreg.KEY_READ | winreg.KEY_WOW64_64KEY)
+    engine_location = engine_installed = winreg.QueryValueEx(engine_key, 'InstalledDirectory')[0]
+    winreg.CloseKey(engine_key)
+except Exception as ex:
+    print('Could not find UE' + engine_version)
+    exit(-1)
+
+print('Manifest: ' + manifest)
+print('Type: ' + package_type)
+print('Engine version: ' + engine_version)
+print('Engine location: ' + engine_location)
+print('Output directory: ' + output_directory)
+
+uat_path = engine_location + '\\Engine\\Build\\BatchFiles\\RunUAT.bat'
+
+command = '"' + uat_path + '"'
+
+if package_type == 'application':
+    command += ' BuildCookRun'
+    command += ' -project="' + manifest + '"'
+    command += ' -platform="' + arguments.platform + '"'
+    command += ' -clientconfig="' + arguments.config + '"'
+    command += ' -serverconfig="' + arguments.config + '"'
+    command += ' -noP4'
+    command += ' -Compressed'
+    command += ' -cook'
+    command += ' -allmaps'
+    command += ' -build'
+    command += ' -stage'
+    command += ' -pak'
+    command += ' -archive'
+    command += ' -prereqs'
+    command += ' -archivedirectory="' + output_directory + '"'
+
+elif package_type == 'plugin':
+    command += ' BuildPlugin'
+    command += ' -Plugin="' + manifest + '"'
+    command += ' -Package="' + output_directory + '"'
+    command += ' -CreateSubFolders'
+
+print(command)
+
+return_code = os.system('"' + command + '"')
+if return_code != 0:
+    exit(return_code)
+
+exit(0)
```

## Source/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from . import UePack
+from . import UePack
```

## Comparing `Unreal_Engine_Packer-1.0.dist-info/RECORD` & `Unreal_Engine_Packer-1.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Source/UePack.py,sha256=50THMoFa45PfS7t6UWbOeMnCdsU3tQ1PoX8r4msUrUo,3229
-Source/__init__.py,sha256=kL1nGzPQHb_lkTVJPB5zqaNRpMjd38LvY_U7v7DtEgM,22
-Unreal_Engine_Packer-1.0.dist-info/METADATA,sha256=1M-4TZEMwX1_4Sihz17C67j9qQ9tkcx2kMGMTzivy9A,387
-Unreal_Engine_Packer-1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-Unreal_Engine_Packer-1.0.dist-info/entry_points.txt,sha256=FDTp14h1nyoc5IhGgXJ5POZE4q9dCG6qyg4CteBhWzs,49
-Unreal_Engine_Packer-1.0.dist-info/top_level.txt,sha256=d_GLf16TqGXe2Ir7Ik0T32QaFEWUJNAst0P15Au9aqE,7
-Unreal_Engine_Packer-1.0.dist-info/RECORD,,
+Source/UePack.py,sha256=6WGcvqU7gKiyDjNiVEf0wWym46LFyoR_J37DOPRTuxE,3830
+Source/__init__.py,sha256=6iS4TH5A7DUBAWyZTR6jgXvoLyf2fGdzFXC8H4LYTWQ,21
+Unreal_Engine_Packer-1.1.dist-info/METADATA,sha256=zb17u3cr8NpbDbnLA4XqxLKidDUT-e7C0OrPiLp6cM0,1309
+Unreal_Engine_Packer-1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+Unreal_Engine_Packer-1.1.dist-info/entry_points.txt,sha256=5yQyHAhN_ac8jFOSEksU8si2BY6KS8dhdJh4mgvMDKc,48
+Unreal_Engine_Packer-1.1.dist-info/top_level.txt,sha256=d_GLf16TqGXe2Ir7Ik0T32QaFEWUJNAst0P15Au9aqE,7
+Unreal_Engine_Packer-1.1.dist-info/RECORD,,
```

