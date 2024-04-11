# Comparing `tmp/pyfakefs-5.4.0.tar.gz` & `tmp/pyfakefs-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfakefs-5.4.0.tar", last modified: Sun Apr  7 07:12:53 2024, max compression
+gzip compressed data, was "pyfakefs-5.4.1.tar", last modified: Thu Apr 11 18:13:39 2024, max compression
```

## Comparing `pyfakefs-5.4.0.tar` & `pyfakefs-5.4.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:12:53.179854 pyfakefs-5.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    49615 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/COPYING
--rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-04-07 07:12:53.179854 pyfakefs-5.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/extra_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:12:53.167855 pyfakefs-5.4.0/pyfakefs/
--rwxr-xr-x   0 runner    (1001) docker     (127)       56 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/extra_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    49019 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/fake_file.py
--rw-r--r--   0 runner    (1001) docker     (127)   123400 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/fake_filesystem.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3756 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/fake_filesystem_shutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    45083 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/fake_filesystem_unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/fake_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    14251 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/fake_open.py
--rw-r--r--   0 runner    (1001) docker     (127)    53434 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/fake_os.py
--rw-r--r--   0 runner    (1001) docker     (127)    18284 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/fake_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    34844 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/fake_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/fake_scandir.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/mox3_stubout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/patched_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:12:53.171855 pyfakefs-5.4.0/pyfakefs/pytest_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_tests/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_tests/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_doctest_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_fixture_param_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_fixture_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_module_fixture_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_plugin_failing_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_reload_pandas_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/pytest_tests/unhashable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:12:53.175855 pyfakefs-5.4.0/pyfakefs/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/all_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/all_tests_without_extra_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/dynamic_patch_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/example_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fake_filesystem_glob_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22626 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fake_filesystem_shutil_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   110189 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fake_filesystem_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    35456 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fake_filesystem_unittest_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29767 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fake_filesystem_vs_real_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    87621 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fake_open_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   244617 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fake_os_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    52726 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fake_pathlib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22479 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fake_stat_time_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fake_tempfile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:12:53.179854 pyfakefs-5.4.0/pyfakefs/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fixtures/config_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fixtures/deprecated_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/fixtures/module_with_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/import_as_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/logsio.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/mox3_stubout_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/mox3_stubout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/patched_packages_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/performance_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyfakefs/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:12:53.179854 pyfakefs-5.4.0/pyfakefs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-04-07 07:12:53.000000 pyfakefs-5.4.0/pyfakefs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-07 07:12:53.000000 pyfakefs-5.4.0/pyfakefs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 07:12:53.000000 pyfakefs-5.4.0/pyfakefs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-07 07:12:53.000000 pyfakefs-5.4.0/pyfakefs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 07:12:53.000000 pyfakefs-5.4.0/pyfakefs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-07 07:12:53.179854 pyfakefs-5.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-07 07:12:47.000000 pyfakefs-5.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:39.719081 pyfakefs-5.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    49861 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/COPYING
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-04-11 18:13:39.719081 pyfakefs-5.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/extra_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:39.711081 pyfakefs-5.4.1/pyfakefs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       56 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/extra_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49019 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123400 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_filesystem.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3756 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_filesystem_shutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45083 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_filesystem_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13893 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53434 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_os.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18284 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34844 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_scandir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/mox3_stubout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/patched_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:39.715081 pyfakefs-5.4.1/pyfakefs/pytest_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_doctest_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_fixture_param_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_fixture_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_module_fixture_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_plugin_failing_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_reload_pandas_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/unhashable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:39.719081 pyfakefs-5.4.1/pyfakefs/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/all_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/all_tests_without_extra_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/dynamic_patch_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/example_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_glob_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22626 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_shutil_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110189 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35456 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_unittest_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29767 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_vs_real_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87621 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_open_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   244080 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_os_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52726 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_pathlib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22479 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_stat_time_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_tempfile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:39.719081 pyfakefs-5.4.1/pyfakefs/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fixtures/config_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fixtures/deprecated_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fixtures/module_with_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/import_as_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/logsio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/mox3_stubout_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/mox3_stubout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/patched_packages_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:39.719081 pyfakefs-5.4.1/pyfakefs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-04-11 18:13:39.000000 pyfakefs-5.4.1/pyfakefs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-11 18:13:39.000000 pyfakefs-5.4.1/pyfakefs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:13:39.000000 pyfakefs-5.4.1/pyfakefs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-11 18:13:39.000000 pyfakefs-5.4.1/pyfakefs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 18:13:39.000000 pyfakefs-5.4.1/pyfakefs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-11 18:13:39.723081 pyfakefs-5.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/tox.ini
```

### Comparing `pyfakefs-5.4.0/CHANGES.md` & `pyfakefs-5.4.1/CHANGES.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # pyfakefs Release Notes
 The released versions correspond to PyPI releases.
 
+## [Version 5.4.1](https://pypi.python.org/pypi/pyfakefs/5.4.0) (2024-04-11)
+Fixes a regression.
+
+### Fixes
+* fixed a regression from version 5.4.0 that incorrectly handled files opened twice via file descriptor
+  (see [#997](../../issues/997))
+
 ## [Version 5.4.0](https://pypi.python.org/pypi/pyfakefs/5.4.0) (2024-04-07)
 Improves permission handling.
 
 ### Changes
 * the handling of file permissions under Posix should now mostly match the behavior
   of the real filesystem, which may change the behavior of some tests
 * removed the argument `module_cleanup_mode`, that was introduced as a temporary workaround
```

### Comparing `pyfakefs-5.4.0/CONTRIBUTING.md` & `pyfakefs-5.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/COPYING` & `pyfakefs-5.4.1/COPYING`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/PKG-INFO` & `pyfakefs-5.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfakefs
-Version: 5.4.0
+Version: 5.4.1
 Summary: pyfakefs implements a fake file system that mocks the Python file system modules.
 Home-page: https://github.com/pytest-dev/pyfakefs
 Author: Google
 Author-email: google-pyfakefs@google.com
 Maintainer: John McGehee
 Maintainer-email: pyfakefs@johnnado.com
 License: http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyfakefs-5.4.0/README.md` & `pyfakefs-5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/extra_requirements.txt` & `pyfakefs-5.4.1/extra_requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 scandir>=1.8
 
 # pandas + xlrd are used to test pandas-specific patches to allow
 # pyfakefs to work with pandas
 # we use the latest version to see any problems with new versions
 pandas==1.3.5; python_version == '3.7' # pyup: ignore
 pandas==2.0.3; python_version == '3.8' # pyup: ignore
-pandas==2.2.1; python_version > '3.8'
+pandas==2.2.2; python_version > '3.8'
 xlrd==2.0.1
 openpyxl==3.1.2
```

### Comparing `pyfakefs-5.4.0/mypy.ini` & `pyfakefs-5.4.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/extra_packages.py` & `pyfakefs-5.4.1/pyfakefs/extra_packages.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/fake_file.py` & `pyfakefs-5.4.1/pyfakefs/fake_file.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/fake_filesystem.py` & `pyfakefs-5.4.1/pyfakefs/fake_filesystem.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/fake_filesystem_shutil.py` & `pyfakefs-5.4.1/pyfakefs/fake_filesystem_shutil.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/fake_filesystem_unittest.py` & `pyfakefs-5.4.1/pyfakefs/fake_filesystem_unittest.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/fake_io.py` & `pyfakefs-5.4.1/pyfakefs/fake_io.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/fake_open.py` & `pyfakefs-5.4.1/pyfakefs/fake_open.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,20 +140,14 @@
         binary = "b" in mode
 
         if binary and encoding:
             raise ValueError("binary mode doesn't take an encoding argument")
 
         newline, open_modes = self._handle_file_mode(mode, newline, open_modes)
         opened_as_fd = isinstance(file_, int)
-        if opened_as_fd and not helpers.IS_PYPY:
-            fd: int = cast(int, file_)
-            # cannot open the same file descriptor twice, except in PyPy
-            for f in self.filesystem.get_open_files(fd):
-                if isinstance(f, FakeFileWrapper) and f.opened_as_fd:
-                    raise OSError(errno.EBADF, "Bad file descriptor")
 
         # the pathlib opener is defined in a Path instance that may not be
         # patched under some circumstances; as it just calls standard open(),
         # we may ignore it, as it would not change the behavior
         if opener is not None and opener.__module__ != "pathlib":
             # opener shall return a file descriptor, which will be handled
             # here as if directly passed
```

### Comparing `pyfakefs-5.4.0/pyfakefs/fake_os.py` & `pyfakefs-5.4.1/pyfakefs/fake_os.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/fake_path.py` & `pyfakefs-5.4.1/pyfakefs/fake_path.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/fake_pathlib.py` & `pyfakefs-5.4.1/pyfakefs/fake_pathlib.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/fake_scandir.py` & `pyfakefs-5.4.1/pyfakefs/fake_scandir.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/helpers.py` & `pyfakefs-5.4.1/pyfakefs/helpers.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/mox3_stubout.py` & `pyfakefs-5.4.1/pyfakefs/mox3_stubout.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/patched_packages.py` & `pyfakefs-5.4.1/pyfakefs/patched_packages.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/pytest_plugin.py` & `pyfakefs-5.4.1/pyfakefs/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/pytest_tests/conftest.py` & `pyfakefs-5.4.1/pyfakefs/pytest_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/pytest_tests/example.py` & `pyfakefs-5.4.1/pyfakefs/pytest_tests/example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py` & `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_doctest_test.py` & `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_doctest_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_fixture_param_test.py` & `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_fixture_param_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_fixture_test.py` & `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_fixture_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_module_fixture_test.py` & `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_module_fixture_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_plugin_test.py` & `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_plugin_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/pytest_tests/pytest_reload_pandas_test.py` & `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_reload_pandas_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/all_tests.py` & `pyfakefs-5.4.1/pyfakefs/tests/all_tests.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/all_tests_without_extra_packages.py` & `pyfakefs-5.4.1/pyfakefs/tests/all_tests_without_extra_packages.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/dynamic_patch_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/dynamic_patch_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/example.py` & `pyfakefs-5.4.1/pyfakefs/tests/example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/example_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/example_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/fake_filesystem_glob_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_glob_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/fake_filesystem_shutil_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_shutil_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/fake_filesystem_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/fake_filesystem_unittest_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_unittest_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/fake_filesystem_vs_real_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_vs_real_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/fake_open_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/fake_open_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/fake_os_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/fake_os_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,26 +227,26 @@
             self.assertFalse(f is fake_file1)
         with self.os.fdopen(fileno3, encoding="utf8") as f:
             self.assertFalse(f is fake_file3)
         kwargs = {"encoding": "utf8"}
         self.assert_raises_os_error(errno.EBADF, self.os.fdopen, fileno2, **kwargs)
 
     def test_fdopen_twice(self):
+        # regression test for #997
         file_path = self.make_path("some_file1")
         self.create_file(file_path, contents="contents here1")
         fake_file = self.open(file_path, "r", encoding="utf8")
         fd = fake_file.fileno()
-        self.open(fd, encoding="utf8")
-        if not IS_PYPY:
-            with self.assertRaises(OSError) as cm:
-                self.open(fd, encoding="utf8")
-            self.assertEqual(errno.EBADF, cm.exception.errno)
-        else:
-            self.open(fd, encoding="utf8")
-            self.os.close(fd)
+        # note: we need to assign the files to objects,
+        # otherwise the file will be closed immediately in the CPython implementation
+        # note that this case is not (and will probably not be) handled in pyfakefs
+        file1 = self.open(fd, encoding="utf8")  # noqa: F841
+        file2 = self.open(fd, encoding="utf8")  # noqa: F841
+
+        self.os.close(fd)
 
     def test_open_fd_write_mode_for_ro_file(self):
         # Create a writable file handle to a read-only file, see #967
         file_path = self.make_path("file.txt")
         fd = self.os.open(file_path, os.O_CREAT | os.O_WRONLY, 0o555)
         with self.open(fd, "w", encoding="utf8") as out:
             out.write("hey")
@@ -3155,30 +3155,14 @@
         with self.assertRaises(PermissionError):
             self.os.scandir(directory)
         # we can access the file if we know the file name
         assert self.os.stat(file_path).st_mode & 0o777 == 0o755
         with self.open(file_path, encoding="utf8") as f:
             assert f.read() == "hey"
 
-    def test_fdopen_twice(self):
-        file_path1 = self.make_path("some_file1")
-        file_path2 = self.make_path("SOME_file1")
-        self.create_file(file_path1, contents="contents here1")
-
-        fake_file1 = self.open(file_path2, "r", encoding="utf8")
-        fileno1 = fake_file1.fileno()
-        self.os.fdopen(fileno1, encoding="utf8")
-        if not IS_PYPY:
-            with self.assertRaises(OSError) as cm:
-                self.open(fileno1, encoding="utf8")
-            self.assertEqual(errno.EBADF, cm.exception.errno)
-        else:
-            self.open(fileno1, encoding="utf8")
-            self.os.close(fileno1)
-
     def test_stat(self):
         directory = self.make_path("xyzzy")
         directory1 = self.make_path("XYZZY")
         file_path = self.os.path.join(directory, "plugh")
         self.create_file(file_path, contents="ABCDE")
         self.assertTrue(stat.S_IFDIR & self.os.stat(directory1)[stat.ST_MODE])
         file_path1 = self.os.path.join(directory1, "Plugh")
```

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/fake_pathlib_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/fake_pathlib_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/fake_stat_time_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/fake_stat_time_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/fake_tempfile_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/fake_tempfile_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/fixtures/deprecated_property.py` & `pyfakefs-5.4.1/pyfakefs/tests/fixtures/deprecated_property.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/fixtures/module_with_attributes.py` & `pyfakefs-5.4.1/pyfakefs/tests/fixtures/module_with_attributes.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/import_as_example.py` & `pyfakefs-5.4.1/pyfakefs/tests/import_as_example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/logsio.py` & `pyfakefs-5.4.1/pyfakefs/tests/logsio.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/mox3_stubout_example.py` & `pyfakefs-5.4.1/pyfakefs/tests/mox3_stubout_example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/mox3_stubout_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/mox3_stubout_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/patched_packages_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/patched_packages_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/performance_test.py` & `pyfakefs-5.4.1/pyfakefs/tests/performance_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs/tests/test_utils.py` & `pyfakefs-5.4.1/pyfakefs/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/pyfakefs.egg-info/PKG-INFO` & `pyfakefs-5.4.1/pyfakefs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfakefs
-Version: 5.4.0
+Version: 5.4.1
 Summary: pyfakefs implements a fake file system that mocks the Python file system modules.
 Home-page: https://github.com/pytest-dev/pyfakefs
 Author: Google
 Author-email: google-pyfakefs@google.com
 Maintainer: John McGehee
 Maintainer-email: pyfakefs@johnnado.com
 License: http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyfakefs-5.4.0/pyfakefs.egg-info/SOURCES.txt` & `pyfakefs-5.4.1/pyfakefs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.0/setup.cfg` & `pyfakefs-5.4.1/setup.cfg`

 * *Files identical despite different names*

