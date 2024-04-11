# Comparing `tmp/bakabakabaka-0.8.5.tar.gz` & `tmp/bakabakabaka-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bakabakabaka-0.8.5.tar", last modified: Tue Apr  9 15:29:07 2024, max compression
+gzip compressed data, was "bakabakabaka-0.8.6.tar", last modified: Thu Apr 11 06:08:24 2024, max compression
```

## Comparing `bakabakabaka-0.8.5.tar` & `bakabakabaka-0.8.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:29:07.069207 bakabakabaka-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 15:28:58.000000 bakabakabaka-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-09 15:29:07.069207 bakabakabaka-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-09 15:28:58.000000 bakabakabaka-0.8.5/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    32916 2024-04-09 15:28:58.000000 bakabakabaka-0.8.5/baka.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:29:07.069207 bakabakabaka-0.8.5/bakabakabaka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-09 15:29:07.000000 bakabakabaka-0.8.5/bakabakabaka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 15:29:07.000000 bakabakabaka-0.8.5/bakabakabaka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:29:07.000000 bakabakabaka-0.8.5/bakabakabaka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 15:29:07.000000 bakabakabaka-0.8.5/bakabakabaka.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 15:29:07.000000 bakabakabaka-0.8.5/bakabakabaka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:29:07.069207 bakabakabaka-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-09 15:28:58.000000 bakabakabaka-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:08:24.196810 bakabakabaka-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 06:08:15.000000 bakabakabaka-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-11 06:08:24.196810 bakabakabaka-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-11 06:08:15.000000 bakabakabaka-0.8.6/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33020 2024-04-11 06:08:15.000000 bakabakabaka-0.8.6/baka.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:08:24.196810 bakabakabaka-0.8.6/bakabakabaka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-11 06:08:24.000000 bakabakabaka-0.8.6/bakabakabaka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-11 06:08:24.000000 bakabakabaka-0.8.6/bakabakabaka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 06:08:24.000000 bakabakabaka-0.8.6/bakabakabaka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 06:08:24.000000 bakabakabaka-0.8.6/bakabakabaka.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 06:08:24.000000 bakabakabaka-0.8.6/bakabakabaka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 06:08:24.196810 bakabakabaka-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-11 06:08:15.000000 bakabakabaka-0.8.6/setup.py
```

### Comparing `bakabakabaka-0.8.5/LICENSE` & `bakabakabaka-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bakabakabaka-0.8.5/PKG-INFO` & `bakabakabaka-0.8.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakabakabaka
-Version: 0.8.5
+Version: 0.8.6
 Summary: the stupid configuration tracker using the stupid content tracker
 Home-page: https://github.com/elesiuta/baka
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,19 +28,19 @@
   --untrack ...  untrack path(s) from git
   --install ...  install package(s) and commit changes
   --remove ...   remove package(s) and commit changes
   --upgrade      upgrade packages on system and commit changes
   --docker ...   usage: --docker <up|down|pull> <all|names...>
   --podman ...   usage: --podman <up|down|pull> <all|names...>
   --file ...     usage: --file <save|restore> <all|names...>
-  --job name     run commands for job with name
+  --job name     run commands for job with name (modifiers: -i, -e, -y)
   --list         show list of jobs
   --sysck        run commands for system checks and commits output
   --scan         run commands for scanning system, prints and commits output
   --diff         show git diff --color-words
   --log          show pretty git log
   --show         show most recent commit
-  -e             toggles 'exit_non_zero' setting for current run of job
-  -y             supplies 'y' to job commands, similar to yes | job
   -i             force job to run in interactive mode
+  -e             job interactive mode after error (non zero exit code)
+  -y             supplies 'y' to job commands, similar to yes | job
   -n, --dry-run  print commands instead of executing them
 ```
```

### Comparing `bakabakabaka-0.8.5/README.md` & `bakabakabaka-0.8.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -17,19 +17,19 @@
   --untrack ...  untrack path(s) from git
   --install ...  install package(s) and commit changes
   --remove ...   remove package(s) and commit changes
   --upgrade      upgrade packages on system and commit changes
   --docker ...   usage: --docker <up|down|pull> <all|names...>
   --podman ...   usage: --podman <up|down|pull> <all|names...>
   --file ...     usage: --file <save|restore> <all|names...>
-  --job name     run commands for job with name
+  --job name     run commands for job with name (modifiers: -i, -e, -y)
   --list         show list of jobs
   --sysck        run commands for system checks and commits output
   --scan         run commands for scanning system, prints and commits output
   --diff         show git diff --color-words
   --log          show pretty git log
   --show         show most recent commit
-  -e             toggles 'exit_non_zero' setting for current run of job
-  -y             supplies 'y' to job commands, similar to yes | job
   -i             force job to run in interactive mode
+  -e             job interactive mode after error (non zero exit code)
+  -y             supplies 'y' to job commands, similar to yes | job
   -n, --dry-run  print commands instead of executing them
 ```
```

### Comparing `bakabakabaka-0.8.5/baka.py` & `bakabakabaka-0.8.6/baka.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import smtplib
 import socket
 import subprocess
 import sys
 import time
 import typing
 
-__version__: typing.Final[str] = "0.8.5"
+__version__: typing.Final[str] = "0.8.6"
 BASE_PATH: typing.Final[str] = os.path.expanduser("~/.baka")
 
 
 def init_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(description="the stupid configuration tracker using the stupid content tracker",
                                      usage="%(prog)s [--dry-run] <argument>")
     parser.add_argument("--version", action="version", version=__version__)
@@ -61,33 +61,33 @@
     maingrp.add_argument("--docker", dest="docker", nargs=argparse.REMAINDER,
                          help="usage: --docker <up|down|pull> <all|names...>")
     maingrp.add_argument("--podman", dest="podman", nargs=argparse.REMAINDER,
                          help="usage: --podman <up|down|pull> <all|names...>")
     maingrp.add_argument("--file", dest="file", nargs=argparse.REMAINDER,
                          help="usage: --file <save|restore> <all|names...>")
     maingrp.add_argument("--job", dest="job", type=str, metavar="name",
-                         help="run commands for job with name")
+                         help="run commands for job with name (modifiers: -i, -e, -y)")
     maingrp.add_argument("--list", dest="list", action="store_true",
                          help="show list of jobs")
     maingrp.add_argument("--sysck", dest="system_checks", action="store_true",
                          help="run commands for system checks and commits output")
     maingrp.add_argument("--scan", dest="system_scans", action="store_true",
                          help="run commands for scanning system, prints and commits output")
     maingrp.add_argument("--diff", dest="diff", action="store_true",
                          help="show git diff --color-words")
     maingrp.add_argument("--log", dest="log", action="store_true",
                          help="show pretty git log")
     maingrp.add_argument("--show", dest="show", action="store_true",
                          help="show most recent commit")
-    parser.add_argument("-e", dest="exit_zero_toggle", action="store_true",
-                        help="toggles 'exit_non_zero' setting for current run of job")
-    parser.add_argument("-y", dest="yes", action="store_true",
-                        help="supplies 'y' to job commands, similar to yes | job")
     parser.add_argument("-i", dest="interactive", action="store_true",
                         help="force job to run in interactive mode")
+    parser.add_argument("-e", dest="error_interactive", action="store_true",
+                        help="job interactive mode after error (non zero exit code)")
+    parser.add_argument("-y", dest="yes", action="store_true",
+                        help="supplies 'y' to job commands, similar to yes | job")
     parser.add_argument("-n", "--dry-run", dest="dry_run", action="store_true",
                         help="print commands instead of executing them")
     return parser
 
 
 class Config:
     def __init__(self):
@@ -206,38 +206,41 @@
     old_hashes = {}
     omitted = {}
     if os.path.exists(os.path.join(BASE_PATH, "sha256.json")):
         with open(os.path.join(BASE_PATH, "sha256.json"), "r", encoding="utf-8", errors="surrogateescape") as json_file:
             old_hashes = json.load(json_file)
     for tracked_path in config.tracked_paths:
         # set default values (no conditions) and load conditions for which files to track/copy
-        conditions = {"exclude": [], "file_starts_with": "", "path_starts_with": "", "max_depth": None, "max_size": None, "test_utf_readable": True}
+        conditions = {"exclude": [], "include": [], "file_starts_with": "", "path_starts_with": "", "max_depth": None, "max_size": None, "test_utf_readable": True}
         for condition in config.tracked_paths[tracked_path]:
             conditions[condition] = config.tracked_paths[tracked_path][condition]
         for root, dirs, files in os.walk(tracked_path, followlinks=False):
             # check conditions
             relpath = os.path.relpath(root, tracked_path)
             # ~/.baka is a subfolder of the path to track
             if root.startswith(BASE_PATH):
                 del dirs
                 continue
-            if conditions["path_starts_with"] and not (relpath.startswith(conditions["path_starts_with"]) or conditions["path_starts_with"].startswith(relpath)):
+            if conditions["path_starts_with"] and not relpath.startswith(conditions["path_starts_with"]):
                 omitted[root] = "path_starts_with"
                 del dirs
                 continue
             if conditions["max_depth"] and relpath.count("/") > conditions["max_depth"]:
                 omitted[root] = "max_depth"
                 del dirs
                 continue
             for file in files:
                 file_path = os.path.join(root, file)
                 file_relpath = os.path.relpath(file_path, tracked_path)
                 if conditions["exclude"] and any(e in file_relpath for e in conditions["exclude"]):
                     omitted[file_path] = "exclude"
                     continue
+                if conditions["include"] and not any(i in file_relpath for i in conditions["include"]):
+                    omitted[file_path] = "include"
+                    continue
                 if conditions["file_starts_with"] and not file.startswith(conditions["file_starts_with"]):
                     omitted[file_path] = "file_starts_with"
                     continue
                 if conditions["path_starts_with"] and not file_relpath.startswith(conditions["path_starts_with"]):
                     omitted[file_path] = "path_starts_with"
                     continue
                 try:
@@ -469,17 +472,14 @@
                 if "src" in file_key.split("_"):
                     cmds.append([*copy_command, os.path.join(BASE_PATH, config.hostname, file), config.files[file][file_key]])
         cmds.append(["git", "add", "--ignore-errors", "--all"])
         cmds.append(["git", "commit", "-m", f"baka file {config.hostname}"])
     elif args.job:
         if args.interactive:
             config.jobs[args.job]["interactive"] = True
-        if args.exit_zero_toggle:
-            exit_non_zero = "exit_non_zero" in config.jobs[args.job] and config.jobs[args.job]["exit_non_zero"]
-            config.jobs[args.job]["exit_non_zero"] = not exit_non_zero
         cmds = config.jobs[args.job]["commands"]
     elif args.list:
         cmds = [
             ["echo", "Prompt\tExit!0\tJob Name\n========================"],
             *[["echo", "%s\t%s\t%s" % ("interactive" in config.jobs[job] and config.jobs[job]["interactive"],
                                        "exit_non_zero" in config.jobs[job] and config.jobs[job]["exit_non_zero"],
                                        job)] for job in config.jobs]
@@ -539,45 +539,48 @@
             # execute command if not dry-run
             if args.job:
                 # run command as part of job, otherwise run command normally
                 capture_output = bool(
                     ("write" in config.jobs[args.job] and config.jobs[args.job]["write"]) or
                     ("email" in config.jobs[args.job] and config.jobs[args.job]["email"] and config.jobs[args.job]["email"]["to"])
                 )
-                verbosity = ""
-                if "verbosity" in config.jobs[args.job] and config.jobs[args.job]["verbosity"]:
-                    verbosity = config.jobs[args.job]["verbosity"].lower()
-                if verbosity not in ["debug", "info", "error", "silent"]:
-                    verbosity = "debug"
+                verbosity = config.jobs[args.job].get("verbosity", "debug")
+                verbosity = verbosity if verbosity else "debug"
+                verbosity = verbosity.lower()
+                assert verbosity in ["debug", "info", "error", "silent"]
                 if verbosity in ["debug"]:
                     print("\033[94m%s\033[0m" % shlex.join(cmd))
-                if "interactive" in config.jobs[args.job] and config.jobs[args.job]["interactive"]:
+                if config.jobs[args.job].get("interactive", False):
                     response = input("\033[92mContinue (yes/no/skip)?\033[0m ")
                     if response.strip().lower().startswith("y"):
                         pass
                     elif response.strip().lower().startswith("n"):
                         break
                     elif response.strip().lower().startswith("s"):
                         continue
                     else:
                         print("\033[91mInvalid response, exiting\033[0m")
                         break
-                proc_input = "y\n" if args.yes else None
+                proc_input = b"y\n" if args.yes else None
                 proc_out = subprocess.PIPE
                 proc_err = subprocess.PIPE
                 if not capture_output:
                     if verbosity in ["debug", "info"]:
                         proc_out = sys.stdout
                     if verbosity in ["debug", "info", "error"]:
                         proc_err = sys.stderr
                 proc = subprocess.run(cmd, stdout=proc_out, stderr=proc_err, input=proc_input)
                 if proc.returncode != 0:
-                    if "exit_non_zero" in config.jobs[args.job] and config.jobs[args.job]["exit_non_zero"]:
+                    if args.error_interactive:
+                        return_code += 1
+                        print(f"Error: exit {proc.returncode} for `{shlex.join(cmd)}`, continuing in interactive mode")
+                        config.jobs[args.job]["interactive"] = True
+                    elif config.jobs[args.job].get("exit_non_zero", False):
                         return_code = proc.returncode
-                        error_message = "Error: baka job encountered a non-zero return code for `%s`, exiting" % shlex.join(cmd)
+                        error_message = "Error: baka job encountered a non-zero exit code for `%s`, exiting" % shlex.join(cmd)
                         command_output.append(error_message)
                         print(error_message, file=sys.stderr)
                         break
                     else:
                         return_code += 1
                 if capture_output:
                     if verbosity in ["debug", "info"]:
```

### Comparing `bakabakabaka-0.8.5/bakabakabaka.egg-info/PKG-INFO` & `bakabakabaka-0.8.6/bakabakabaka.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakabakabaka
-Version: 0.8.5
+Version: 0.8.6
 Summary: the stupid configuration tracker using the stupid content tracker
 Home-page: https://github.com/elesiuta/baka
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,19 +28,19 @@
   --untrack ...  untrack path(s) from git
   --install ...  install package(s) and commit changes
   --remove ...   remove package(s) and commit changes
   --upgrade      upgrade packages on system and commit changes
   --docker ...   usage: --docker <up|down|pull> <all|names...>
   --podman ...   usage: --podman <up|down|pull> <all|names...>
   --file ...     usage: --file <save|restore> <all|names...>
-  --job name     run commands for job with name
+  --job name     run commands for job with name (modifiers: -i, -e, -y)
   --list         show list of jobs
   --sysck        run commands for system checks and commits output
   --scan         run commands for scanning system, prints and commits output
   --diff         show git diff --color-words
   --log          show pretty git log
   --show         show most recent commit
-  -e             toggles 'exit_non_zero' setting for current run of job
-  -y             supplies 'y' to job commands, similar to yes | job
   -i             force job to run in interactive mode
+  -e             job interactive mode after error (non zero exit code)
+  -y             supplies 'y' to job commands, similar to yes | job
   -n, --dry-run  print commands instead of executing them
 ```
```

### Comparing `bakabakabaka-0.8.5/setup.py` & `bakabakabaka-0.8.6/setup.py`

 * *Files identical despite different names*

