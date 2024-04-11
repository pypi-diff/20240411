# Comparing `tmp/fosslight_yocto-3.1.27.tar.gz` & `tmp/fosslight_yocto-3.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fosslight_yocto-3.1.27.tar", last modified: Tue Apr  9 13:29:56 2024, max compression
+gzip compressed data, was "fosslight_yocto-3.1.28.tar", last modified: Thu Apr 11 00:38:52 2024, max compression
```

## Comparing `fosslight_yocto-3.1.27.tar` & `fosslight_yocto-3.1.28.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:29:56.692864 fosslight_yocto-3.1.27/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-09 13:29:56.692864 fosslight_yocto-3.1.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:29:56.692864 fosslight_yocto-3.1.27/files_for_preparation/
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/files_for_preparation/bom.bbclass
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:29:56.692864 fosslight_yocto-3.1.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:29:56.688864 fosslight_yocto-3.1.27/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:29:56.692864 fosslight_yocto-3.1.27/src/fosslight_yocto/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/_help.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6050 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/_overwrite_yaml.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10182 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/_package_item.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3947 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/_write_result_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/_zip_source_works.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46678 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/create_oss_report_for_yocto.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8200 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/parsing_meta_doubleopen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:29:56.692864 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-09 13:29:56.000000 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-09 13:29:56.000000 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:29:56.000000 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-09 13:29:56.000000 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 13:29:56.000000 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 13:29:56.000000 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:52.235054 fosslight_yocto-3.1.28/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-11 00:38:52.235054 fosslight_yocto-3.1.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:52.235054 fosslight_yocto-3.1.28/files_for_preparation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/files_for_preparation/bom.bbclass
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:38:52.235054 fosslight_yocto-3.1.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:52.231054 fosslight_yocto-3.1.28/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:52.235054 fosslight_yocto-3.1.28/src/fosslight_yocto/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/_help.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6050 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/_overwrite_yaml.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10182 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/_package_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3947 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/_write_result_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/_zip_source_works.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46686 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/create_oss_report_for_yocto.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8200 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/parsing_meta_doubleopen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:52.235054 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-11 00:38:51.000000 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-11 00:38:52.000000 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:38:51.000000 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 00:38:51.000000 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 00:38:51.000000 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 00:38:51.000000 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/top_level.txt
```

### Comparing `fosslight_yocto-3.1.27/LICENSE` & `fosslight_yocto-3.1.28/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.27/PKG-INFO` & `fosslight_yocto-3.1.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight_yocto
-Version: 3.1.27
+Version: 3.1.28
 Summary: FOSSLight Yocto
 Home-page: https://github.com/fosslight/fosslight_yocto_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_yocto_scanner
 Description: <!--
         SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight_yocto Version: 3.1.27 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight_yocto Version: 3.1.28 Summary: FOSSLight
 Yocto Home-page: https://github.com/fosslight/fosslight_yocto_scanner Author:
 LG Electronics License: Apache-2.0 Download-URL: https://github.com/fosslight/
 fosslight_yocto_scanner Description:
                                                                        _[_K_o_r_e_a_n_]
 # FOSSLight Yocto Scanner [FOSSLight Yocto Scanner is released under the
 Apache-2.0 License.][Current python package version.][https://img.shields.io/
 pypi/pyversions/fosslight_yocto][![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_yocto-3.1.27/README.md` & `fosslight_yocto-3.1.28/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.27/files_for_preparation/bom.bbclass` & `fosslight_yocto-3.1.28/files_for_preparation/bom.bbclass`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.27/setup.py` & `fosslight_yocto-3.1.28/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 if __name__ == "__main__":
     setup(
         name='fosslight_yocto',
-        version='3.1.27',
+        version='3.1.28',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Yocto',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         author='LG Electronics',
```

### Comparing `fosslight_yocto-3.1.27/src/fosslight_yocto/_help.py` & `fosslight_yocto-3.1.28/src/fosslight_yocto/_help.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.27/src/fosslight_yocto/_overwrite_yaml.py` & `fosslight_yocto-3.1.28/src/fosslight_yocto/_overwrite_yaml.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.27/src/fosslight_yocto/_package_item.py` & `fosslight_yocto-3.1.28/src/fosslight_yocto/_package_item.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.27/src/fosslight_yocto/_write_result_file.py` & `fosslight_yocto-3.1.28/src/fosslight_yocto/_write_result_file.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.27/src/fosslight_yocto/_zip_source_works.py` & `fosslight_yocto-3.1.28/src/fosslight_yocto/_zip_source_works.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.27/src/fosslight_yocto/create_oss_report_for_yocto.py` & `fosslight_yocto-3.1.28/src/fosslight_yocto/create_oss_report_for_yocto.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
                             else:
                                 buildhistory_latest_pkg[recipe_name] = pkg_name
                     match = re.search(r'PKG(\s)*=(\s)*([^\n]+)', file_contents)
                     if match:
                         pkg = match.group(3).strip()
                         for pkg_name in pkg.split():
                             re_pkg_name = re.escape(pkg_name)
-                            r = re.compile(f"^{re_pkg_name}-{pv}-{pr}")
+                            r = re.compile(f"^{re_pkg_name}(-|_){pv}(-|_){pr}")
                             installed_pkg_verified = list(filter(r.match, installed_pkg_version_lines))
                             if installed_pkg_verified:
                                 nested_pkg_name[pkg_name] = recipe_name
                             else:
                                 not_installed_pkg[pkg_name] = recipe_name
                 except Exception as ex:
                     logger.debug(f"Failed to parsing latest_{root}:{ex}")
```

### Comparing `fosslight_yocto-3.1.27/src/fosslight_yocto/parsing_meta_doubleopen.py` & `fosslight_yocto-3.1.28/src/fosslight_yocto/parsing_meta_doubleopen.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/PKG-INFO` & `fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight-yocto
-Version: 3.1.27
+Version: 3.1.28
 Summary: FOSSLight Yocto
 Home-page: https://github.com/fosslight/fosslight_yocto_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_yocto_scanner
 Description: <!--
         SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight-yocto Version: 3.1.27 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight-yocto Version: 3.1.28 Summary: FOSSLight
 Yocto Home-page: https://github.com/fosslight/fosslight_yocto_scanner Author:
 LG Electronics License: Apache-2.0 Download-URL: https://github.com/fosslight/
 fosslight_yocto_scanner Description:
                                                                        _[_K_o_r_e_a_n_]
 # FOSSLight Yocto Scanner [FOSSLight Yocto Scanner is released under the
 Apache-2.0 License.][Current python package version.][https://img.shields.io/
 pypi/pyversions/fosslight_yocto][![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/SOURCES.txt` & `fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

