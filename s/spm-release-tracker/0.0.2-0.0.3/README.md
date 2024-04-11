# Comparing `tmp/spm_release_tracker-0.0.2.tar.gz` & `tmp/spm_release_tracker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spm_release_tracker-0.0.2.tar", last modified: Tue Apr  9 23:30:57 2024, max compression
+gzip compressed data, was "spm_release_tracker-0.0.3.tar", last modified: Thu Apr 11 20:53:19 2024, max compression
```

## Comparing `spm_release_tracker-0.0.2.tar` & `spm_release_tracker-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hugovanderlei   (501) staff       (20)        0 2024-04-09 23:30:57.457300 spm_release_tracker-0.0.2/
--rw-r--r--   0 hugovanderlei   (501) staff       (20)     1071 2024-04-02 20:08:10.000000 spm_release_tracker-0.0.2/LICENSE
--rw-r--r--   0 hugovanderlei   (501) staff       (20)      203 2024-04-09 23:30:57.457095 spm_release_tracker-0.0.2/PKG-INFO
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       21 2024-04-02 20:08:10.000000 spm_release_tracker-0.0.2/README.md
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       38 2024-04-09 23:30:57.457343 spm_release_tracker-0.0.2/setup.cfg
--rw-r--r--   0 hugovanderlei   (501) staff       (20)      378 2024-04-09 23:29:12.000000 spm_release_tracker-0.0.2/setup.py
-drwxr-xr-x   0 hugovanderlei   (501) staff       (20)        0 2024-04-09 23:30:57.455978 spm_release_tracker-0.0.2/spm_release_tracker/
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       90 2024-04-09 20:58:00.000000 spm_release_tracker-0.0.2/spm_release_tracker/__init__.py
--rw-r--r--   0 hugovanderlei   (501) staff       (20)     7467 2024-04-09 20:58:00.000000 spm_release_tracker-0.0.2/spm_release_tracker/spm_release_tracker.py
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       22 2024-04-09 23:30:52.000000 spm_release_tracker-0.0.2/spm_release_tracker/version.py
-drwxr-xr-x   0 hugovanderlei   (501) staff       (20)        0 2024-04-09 23:30:57.456887 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/
--rw-r--r--   0 hugovanderlei   (501) staff       (20)      203 2024-04-09 23:30:57.000000 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/PKG-INFO
--rw-r--r--   0 hugovanderlei   (501) staff       (20)      392 2024-04-09 23:30:57.000000 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 hugovanderlei   (501) staff       (20)        1 2024-04-09 23:30:57.000000 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       57 2024-04-09 23:30:57.000000 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/entry_points.txt
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       43 2024-04-09 23:30:57.000000 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/requires.txt
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       20 2024-04-09 23:30:57.000000 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 hugovanderlei   (501) staff       (20)        0 2024-04-11 20:53:19.061616 spm_release_tracker-0.0.3/
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)     1071 2024-04-02 20:08:10.000000 spm_release_tracker-0.0.3/LICENSE
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)      203 2024-04-11 20:53:19.061416 spm_release_tracker-0.0.3/PKG-INFO
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)     2897 2024-04-11 20:35:33.000000 spm_release_tracker-0.0.3/README.md
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)       38 2024-04-11 20:53:19.061657 spm_release_tracker-0.0.3/setup.cfg
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)      378 2024-04-11 20:31:56.000000 spm_release_tracker-0.0.3/setup.py
+drwxr-xr-x   0 hugovanderlei   (501) staff       (20)        0 2024-04-11 20:53:19.060346 spm_release_tracker-0.0.3/spm_release_tracker/
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)       90 2024-04-09 20:58:00.000000 spm_release_tracker-0.0.3/spm_release_tracker/__init__.py
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)     7918 2024-04-11 20:21:32.000000 spm_release_tracker-0.0.3/spm_release_tracker/spm_release_tracker.py
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)       22 2024-04-11 20:24:37.000000 spm_release_tracker-0.0.3/spm_release_tracker/version.py
+drwxr-xr-x   0 hugovanderlei   (501) staff       (20)        0 2024-04-11 20:53:19.061217 spm_release_tracker-0.0.3/spm_release_tracker.egg-info/
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)      203 2024-04-11 20:53:19.000000 spm_release_tracker-0.0.3/spm_release_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)      392 2024-04-11 20:53:19.000000 spm_release_tracker-0.0.3/spm_release_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)        1 2024-04-11 20:53:19.000000 spm_release_tracker-0.0.3/spm_release_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)       57 2024-04-11 20:53:19.000000 spm_release_tracker-0.0.3/spm_release_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)       43 2024-04-11 20:53:19.000000 spm_release_tracker-0.0.3/spm_release_tracker.egg-info/requires.txt
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)       20 2024-04-11 20:53:19.000000 spm_release_tracker-0.0.3/spm_release_tracker.egg-info/top_level.txt
```

### Comparing `spm_release_tracker-0.0.2/LICENSE` & `spm_release_tracker-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spm_release_tracker-0.0.2/spm_release_tracker/spm_release_tracker.py` & `spm_release_tracker-0.0.3/spm_release_tracker/spm_release_tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,18 +37,26 @@
         )
         parser.add_argument(
             "--all",
             action="store_true",
             help="Show release notes for all versions, regardless of whether they are newer than those in Package.resolved.",
         )
         parser.add_argument(
-            "--version", action="version", version=f"%(prog)s {__version__}"
+            "--version", action="version",
+              version=f"%(prog)s {__version__}"
+        )
+        parser.add_argument(
+            "--simple",
+            action="store_true",
+            help="Display a simplified list without release notes."
         )
 
         args = parser.parse_args()
+        simple_output = args.simple
+
 
         all_versions = args.all
         header_text = (
             "All versions and their release notes:"
             if all_versions
             else "Versions different from those in your Package.resolved:"
         )
@@ -97,19 +105,29 @@
                 console.print(
                     f"[yellow]{name} ({version}) {version_status}\n", style="bold"
                 )
 
             if version != current_version:
                 console.print(f"[red]Current version: {current_version}", style="bold")
 
-            console.print(
-                Markdown(
-                    f"Release notes:\n\n{processed_notes}\n\n[{url}]({url})\n\n---"
+
+            if simple_output:
+                console.print("")
+                console.print(Markdown("---"))
+                console.print("")
+
+            else:
+                console.print(
+                    Markdown(
+                        f"Release notes:\n\n{processed_notes}\n\n[{url}]({url})\n\n---\n"
+                    )
                 )
-            )
+                console.print("")
+
+             
 
     except KeyboardInterrupt:
         console.print("\nOperation cancelled by the user.\n", style="bold yellow")
         sys.exit(1)
 
 
 def find_package_resolved(base_path="."):
```

