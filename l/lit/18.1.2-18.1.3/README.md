# Comparing `tmp/lit-18.1.2.tar.gz` & `tmp/lit-18.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lit-18.1.2.tar", last modified: Thu Mar 21 17:55:34 2024, max compression
+gzip compressed data, was "lit-18.1.3.tar", last modified: Thu Apr 11 19:00:19 2024, max compression
```

## Comparing `lit-18.1.2.tar` & `lit-18.1.3.tar`

### file list

```diff
@@ -1,637 +1,637 @@
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.677331 lit-18.1.2/
--rw-r--r--   0 tstellar (101195) tstellar (101195)    15141 2024-01-29 23:23:40.000000 lit-18.1.2/LICENSE.TXT
--rw-r--r--   0 tstellar (101195) tstellar (101195)      242 2024-01-29 23:23:40.000000 lit-18.1.2/MANIFEST.in
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2516 2024-03-21 17:55:34.677331 lit-18.1.2/PKG-INFO
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1874 2024-01-29 23:23:40.000000 lit-18.1.2/README.rst
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.647331 lit-18.1.2/examples/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      236 2024-01-29 23:23:40.000000 lit-18.1.2/examples/README.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.647331 lit-18.1.2/examples/many-tests/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      549 2024-01-29 23:23:40.000000 lit-18.1.2/examples/many-tests/ManyTests.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      382 2024-01-29 23:23:40.000000 lit-18.1.2/examples/many-tests/README.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      147 2024-01-29 23:23:40.000000 lit-18.1.2/examples/many-tests/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.650331 lit-18.1.2/lit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)    12039 2024-01-29 23:23:40.000000 lit-18.1.2/lit/BooleanExpression.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     8431 2024-01-29 23:23:40.000000 lit-18.1.2/lit/LitConfig.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1593 2024-01-29 23:23:40.000000 lit-18.1.2/lit/LitTestCase.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    11087 2024-01-29 23:23:40.000000 lit-18.1.2/lit/ProgressBar.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     3242 2024-01-29 23:23:40.000000 lit-18.1.2/lit/ShCommands.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     8811 2024-01-29 23:23:40.000000 lit-18.1.2/lit/ShUtil.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    13734 2024-01-29 23:23:40.000000 lit-18.1.2/lit/Test.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    84905 2024-01-29 23:23:40.000000 lit-18.1.2/lit/TestRunner.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1629 2024-01-29 23:23:40.000000 lit-18.1.2/lit/TestTimes.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     8690 2024-01-29 23:23:40.000000 lit-18.1.2/lit/TestingConfig.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      191 2024-03-21 17:55:25.000000 lit-18.1.2/lit/__init__.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.650331 lit-18.1.2/lit/builtin_commands/
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/lit/builtin_commands/__init__.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1892 2024-01-29 23:23:40.000000 lit-18.1.2/lit/builtin_commands/cat.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     9802 2024-01-29 23:23:40.000000 lit-18.1.2/lit/builtin_commands/diff.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    11174 2024-01-29 23:23:40.000000 lit-18.1.2/lit/cl_arguments.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     9618 2024-01-29 23:23:40.000000 lit-18.1.2/lit/discovery.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     5987 2024-01-29 23:23:40.000000 lit-18.1.2/lit/display.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.651331 lit-18.1.2/lit/formats/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      215 2024-01-29 23:23:40.000000 lit-18.1.2/lit/formats/__init__.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2299 2024-01-29 23:23:40.000000 lit-18.1.2/lit/formats/base.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    14953 2024-01-29 23:23:40.000000 lit-18.1.2/lit/formats/googletest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      992 2024-01-29 23:23:40.000000 lit-18.1.2/lit/formats/shtest.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.651331 lit-18.1.2/lit/llvm/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      176 2024-01-29 23:23:40.000000 lit-18.1.2/lit/llvm/__init__.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    32023 2024-01-29 23:23:40.000000 lit-18.1.2/lit/llvm/config.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     5430 2024-01-29 23:23:40.000000 lit-18.1.2/lit/llvm/subst.py
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)    11855 2024-01-29 23:23:40.000000 lit-18.1.2/lit/main.py
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)    11056 2024-01-29 23:23:40.000000 lit-18.1.2/lit/reports.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     4692 2024-01-29 23:23:40.000000 lit-18.1.2/lit/run.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    17299 2024-01-29 23:23:40.000000 lit-18.1.2/lit/util.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2666 2024-01-29 23:23:40.000000 lit-18.1.2/lit/worker.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.650331 lit-18.1.2/lit.egg-info/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     2516 2024-03-21 17:55:34.000000 lit-18.1.2/lit.egg-info/PKG-INFO
--rw-rw-r--   0 tstellar (101195) tstellar (101195)    22457 2024-03-21 17:55:34.000000 lit-18.1.2/lit.egg-info/SOURCES.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        1 2024-03-21 17:55:34.000000 lit-18.1.2/lit.egg-info/dependency_links.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       38 2024-03-21 17:55:34.000000 lit-18.1.2/lit.egg-info/entry_points.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        1 2023-04-10 18:12:43.000000 lit-18.1.2/lit.egg-info/not-zip-safe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        4 2024-03-21 17:55:34.000000 lit-18.1.2/lit.egg-info/top_level.txt
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)       89 2024-01-29 23:23:40.000000 lit-18.1.2/lit.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)       81 2024-01-29 23:23:40.000000 lit-18.1.2/pyproject.toml
--rw-r--r--   0 tstellar (101195) tstellar (101195)       38 2024-03-21 17:55:34.677331 lit-18.1.2/setup.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1295 2024-01-29 23:23:40.000000 lit-18.1.2/setup.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.655331 lit-18.1.2/tests/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      152 2024-01-29 23:23:40.000000 lit-18.1.2/tests/.coveragerc
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.655331 lit-18.1.2/tests/Inputs/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.655331 lit-18.1.2/tests/Inputs/allow-retries/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       33 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/allow-retries/does-not-succeed-within-limit.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      337 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/allow-retries/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       51 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/allow-retries/more-than-one-allow-retries-lines.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)       45 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/allow-retries/not-a-valid-integer.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      573 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/allow-retries/succeeds-within-limit.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.655331 lit-18.1.2/tests/Inputs/config-map-discovery/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      434 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/config-map-discovery/driver.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/config-map-discovery/invalid-test.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      297 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/config-map-discovery/lit.alt.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.655331 lit-18.1.2/tests/Inputs/config-map-discovery/main-config/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       33 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/config-map-discovery/main-config/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.655331 lit-18.1.2/tests/Inputs/config-map-discovery/tests/
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/config-map-discovery/tests/test1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/config-map-discovery/tests/test2.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.656331 lit-18.1.2/tests/Inputs/custom-result-category/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      467 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/custom-result-category/format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      247 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/custom-result-category/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/custom-result-category/test1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/custom-result-category/test2.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.656331 lit-18.1.2/tests/Inputs/discovery/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      762 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/discovery/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.656331 lit-18.1.2/tests/Inputs/discovery/subdir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      141 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/discovery/subdir/lit.local.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/discovery/subdir/test-three.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.656331 lit-18.1.2/tests/Inputs/discovery/subsuite/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      175 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/discovery/subsuite/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/discovery/subsuite/test-one.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/discovery/subsuite/test-two.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/discovery/test-one.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/discovery/test-two.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/discovery/test.not-txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.656331 lit-18.1.2/tests/Inputs/discovery-getTestsForPath/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      538 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/discovery-getTestsForPath/custom_format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      270 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/discovery-getTestsForPath/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/discovery-getTestsForPath/x.test
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.656331 lit-18.1.2/tests/Inputs/exec-discovery/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      292 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/exec-discovery/lit.site.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.656331 lit-18.1.2/tests/Inputs/exec-discovery-in-tree/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      308 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/exec-discovery-in-tree/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.656331 lit-18.1.2/tests/Inputs/exec-discovery-in-tree/obj/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      205 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/exec-discovery-in-tree/obj/lit.site.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/exec-discovery-in-tree/test-one.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/fake-externals/
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/fake-externals/cd
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/fake-externals/diff
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/fake-externals/env
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/fake-externals/export
--rw-r--r--   0 tstellar (101195) tstellar (101195)      208 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/fake-externals/fake_external.py
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/fake-externals/mkdir
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/fake-externals/rm
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/googletest-cmd-wrapper/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/googletest-cmd-wrapper/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1267 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-cmd-wrapper/DummySubDir/OneTest.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)      189 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-cmd-wrapper/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/googletest-crash/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/googletest-crash/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1424 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-crash/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      120 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-crash/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/googletest-detect-duplicate/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/googletest-detect-duplicate/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1350 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-detect-duplicate/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      131 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-detect-duplicate/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/googletest-discovery-failed/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-discovery-failed/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/googletest-discovery-failed/subdir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       80 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-discovery-failed/subdir/OneTest.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/googletest-format/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/googletest-format/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2741 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-format/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-format/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2742 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.657331 lit-18.1.2/tests/Inputs/googletest-no-sharding/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.658331 lit-18.1.2/tests/Inputs/googletest-no-sharding/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2562 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-no-sharding/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-no-sharding/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.658331 lit-18.1.2/tests/Inputs/googletest-sanitizer-error/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.658331 lit-18.1.2/tests/Inputs/googletest-sanitizer-error/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1506 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-sanitizer-error/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      130 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-sanitizer-error/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.658331 lit-18.1.2/tests/Inputs/googletest-timeout/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.658331 lit-18.1.2/tests/Inputs/googletest-timeout/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1685 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-timeout/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      397 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/googletest-timeout/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.658331 lit-18.1.2/tests/Inputs/ignore-fail/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/ignore-fail/fail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      177 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/ignore-fail/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/ignore-fail/unresolved.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       20 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/ignore-fail/xfail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       19 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/ignore-fail/xpass.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.658331 lit-18.1.2/tests/Inputs/lit-opts/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      253 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lit-opts/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       17 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lit-opts/test.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      223 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.659331 lit-18.1.2/tests/Inputs/lld-features/
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lld-features/ld.lld
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lld-features/ld.lld.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)       31 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lld-features/ld.lld.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lld-features/ld64.lld
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lld-features/ld64.lld.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)       33 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lld-features/ld64.lld.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      714 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lld-features/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lld-features/lld-link
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lld-features/lld-link.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)       33 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lld-features/lld-link.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lld-features/wasm-ld
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lld-features/wasm-ld.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)       32 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/lld-features/wasm-ld.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.659331 lit-18.1.2/tests/Inputs/max-failures/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/max-failures/fail1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/max-failures/fail2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/max-failures/fail3.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      178 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/max-failures/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.659331 lit-18.1.2/tests/Inputs/max-time/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       10 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/max-time/fast.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      251 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/max-time/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      128 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/max-time/slow.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.659331 lit-18.1.2/tests/Inputs/parallelism-groups/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      474 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/parallelism-groups/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/parallelism-groups/test1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/parallelism-groups/test2.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.659331 lit-18.1.2/tests/Inputs/per-test-coverage/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      337 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/per-test-coverage/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      354 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/per-test-coverage/per-test-coverage.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.659331 lit-18.1.2/tests/Inputs/per-test-coverage-by-lit-cfg/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      384 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/per-test-coverage-by-lit-cfg/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      365 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/per-test-coverage-by-lit-cfg/per-test-coverage-by-lit-cfg.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.660331 lit-18.1.2/tests/Inputs/progress-bar/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      178 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/progress-bar/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/progress-bar/test-1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/progress-bar/test-2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/progress-bar/test-3.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/progress-bar/test-4.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.660331 lit-18.1.2/tests/Inputs/py-config-discovery/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      299 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/py-config-discovery/lit.site.cfg.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.660331 lit-18.1.2/tests/Inputs/reorder/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/reorder/aaa.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/reorder/bbb.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/reorder/fff.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      173 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/reorder/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       78 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/reorder/lit_test_times
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/reorder/new-test.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.660331 lit-18.1.2/tests/Inputs/reorder/subdir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/reorder/subdir/ccc.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.660331 lit-18.1.2/tests/Inputs/show-result-codes/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/show-result-codes/fail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      183 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/show-result-codes/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       10 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/show-result-codes/pass.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       36 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/show-result-codes/unsupported.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       20 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/show-result-codes/xfail.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.660331 lit-18.1.2/tests/Inputs/show-used-features/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      184 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/show-used-features/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      267 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/show-used-features/mixed.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       35 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/show-used-features/requires.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       42 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/show-used-features/unsupported.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       30 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/show-used-features/xfail.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.661331 lit-18.1.2/tests/Inputs/shtest-define/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.661331 lit-18.1.2/tests/Inputs/shtest-define/errors/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.662331 lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      227 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/before-name.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      282 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/between-name-equals.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      209 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/braces-empty.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      530 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/braces-with-dot.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      267 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/braces-with-equals.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      239 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/braces-with-newline.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      513 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/braces-with-number.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      230 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/braces-with-ws.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      208 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/empty.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      219 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/no-equals.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      208 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/no-name.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      245 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/ws-only.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.663331 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      295 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/empty.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      352 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/end-in-double-backslash.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      443 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/unterminated-define-bad-redefine.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      312 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/unterminated-define-continuation.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      450 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/unterminated-define-redefine.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      252 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/unterminated-define-run.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      277 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/unterminated-define.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      447 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-bad-define.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      336 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-continuation.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      447 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-define.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      276 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-run.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      291 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      239 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/unterminated-run-define.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      257 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/unterminated-run-redefine.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      336 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/continuation/ws-only.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.663331 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      342 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/define-already-by-config.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      341 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/define-already-by-test.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      347 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/define-inside-pattern.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      432 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/define-multiple-exact.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      459 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/define-multiple-once-exact.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      356 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/define-prefixes-pattern.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      345 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/define-suffixes-pattern.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      422 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/redefine-inside-pattern.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      634 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-exact.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      608 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-once-exact.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/redefine-none.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      431 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/redefine-prefixes-pattern.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      420 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/redefine-suffixes-pattern.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      296 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/location-range.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      209 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/errors/no-run.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.663331 lit-18.1.2/tests/Inputs/shtest-define/examples/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1808 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/examples/param-subst.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1718 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/expansion-order.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1262 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/line-number-substitutions.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2668 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      703 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/name-chars.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      296 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/recursiveExpansionLimit.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      723 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/shared-substs-0.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      723 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/shared-substs-1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      921 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/value-equals.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      538 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/value-escaped.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)     4018 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-define/ws-and-continuations.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.664331 lit-18.1.2/tests/Inputs/shtest-env/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       17 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-args-last-is-assign.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       18 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-args-last-is-u-arg.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       14 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-args-last-is-u.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       19 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-args-nested-none.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-args-none.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       34 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-calls-cd.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       26 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-calls-colon.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       41 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-calls-echo.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      875 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-calls-env.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       37 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-calls-export.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       37 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-calls-mkdir.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      198 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-calls-not-builtin.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       34 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-calls-rm.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      687 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env-u.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      465 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/env.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      310 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      585 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/mixed.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      188 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-env/print_environment.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.664331 lit-18.1.2/tests/Inputs/shtest-external-shell-kill/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      153 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-external-shell-kill/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       92 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-external-shell-kill/test.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.665331 lit-18.1.2/tests/Inputs/shtest-format/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.666331 lit-18.1.2/tests/Inputs/shtest-format/external_shell/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      181 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/external_shell/fail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      107 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/external_shell/fail_with_bad_encoding.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      191 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/external_shell/fail_with_control_chars.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       83 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/external_shell/lit.local.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/external_shell/pass.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       61 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/external_shell/utf8_command.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      138 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/external_shell/write-bad-encoding.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      146 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/external_shell/write-control-chars.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      104 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/fail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      414 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)        9 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/no-test-line.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/pass.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      128 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/requires-missing.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      122 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/requires-present.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       49 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/requires-star.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      114 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/requires-triple.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      218 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/unsupported-expr-false.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      174 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/unsupported-expr-true.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       52 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/unsupported-star.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.666331 lit-18.1.2/tests/Inputs/shtest-format/unsupported_dir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       26 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/unsupported_dir/lit.local.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/unsupported_dir/some-test.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      147 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/xfail-expr-false.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      151 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/xfail-expr-true.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       40 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/xfail-feature.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       38 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/xfail-target.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       20 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/xfail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       37 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format/xpass.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.665331 lit-18.1.2/tests/Inputs/shtest-format-argv0/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      320 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format-argv0/argv0.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      233 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-format-argv0/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.666331 lit-18.1.2/tests/Inputs/shtest-if-else/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      267 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-if-else/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       93 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-if-else/test-neg1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       87 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-if-else/test-neg2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      103 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-if-else/test-neg3.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      106 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-if-else/test-neg4.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)     3487 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-if-else/test.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.666331 lit-18.1.2/tests/Inputs/shtest-inject/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      314 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-inject/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      109 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-inject/test-empty.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      183 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-inject/test-many.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-inject/test-one.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.667331 lit-18.1.2/tests/Inputs/shtest-keyword-parse-errors/
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-keyword-parse-errors/empty.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      133 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-keyword-parse-errors/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       44 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-keyword-parse-errors/multiple-allow-retries.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       29 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-keyword-parse-errors/unterminated-run.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.668331 lit-18.1.2/tests/Inputs/shtest-not/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/exclamation-args-nested-none.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)        9 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/exclamation-args-none.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      211 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/exclamation-calls-external.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      100 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/fail.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      100 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/fail2.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       19 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-args-last-is-crash.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       19 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-args-nested-none.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-args-none.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       85 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-calls-cd.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       68 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-calls-colon.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      252 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-calls-diff-with-crash.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      413 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-calls-diff.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      103 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-calls-echo.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      207 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-calls-env-builtin.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       97 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-calls-export.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1933 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-calls-external.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      142 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-calls-fail2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       59 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-calls-mkdir.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       46 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/not-calls-rm.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/pass.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      159 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-not/print_environment.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.668331 lit-18.1.2/tests/Inputs/shtest-output-printing/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      125 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-output-printing/basic.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      216 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-output-printing/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      127 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-output-printing/write-a-lot.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.668331 lit-18.1.2/tests/Inputs/shtest-pushd-popd/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      145 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-pushd-popd/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       19 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-pushd-popd/popd-args.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-pushd-popd/popd-no-stack.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      223 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-pushd-popd/pushd-popd-ok.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       16 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-pushd-popd/pushd-too-many-args.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.646331 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.668331 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      340 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       18 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.668331 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      380 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       18 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.668331 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/escaping/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/escaping/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       28 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/escaping/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.669331 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/negative-integer/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      218 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/negative-integer/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/negative-integer/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.669331 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/not-an-integer/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      230 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/not-an-integer/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/not-an-integer/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.669331 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/set-to-none/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      215 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/set-to-none/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/set-to-none/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.669331 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      372 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       18 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.669331 lit-18.1.2/tests/Inputs/shtest-run-at-line/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.669331 lit-18.1.2/tests/Inputs/shtest-run-at-line/external-shell/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      125 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-run-at-line/external-shell/basic.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       50 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-run-at-line/external-shell/empty-run-line.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      253 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-run-at-line/external-shell/line-continuation.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      180 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-run-at-line/external-shell/lit.local.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       42 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-run-at-line/external-shell/run-line-with-newline.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.669331 lit-18.1.2/tests/Inputs/shtest-run-at-line/internal-shell/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       37 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-run-at-line/internal-shell/basic.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       50 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-run-at-line/internal-shell/empty-run-line.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      221 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-run-at-line/internal-shell/line-continuation.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      181 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-run-at-line/internal-shell/lit.local.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       42 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-run-at-line/internal-shell/run-line-with-newline.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       62 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-run-at-line/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.672331 lit-18.1.2/tests/Inputs/shtest-shell/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       75 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/cat-error-0.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       87 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/cat-error-1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      269 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/cat_nonprinting.bin
--rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/check_args.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      622 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/check_path.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)       94 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/colon-error.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      373 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/continuations.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      513 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/dev-null.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      274 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-I.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      181 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-b.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      622 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-encodings.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      102 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-error-1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       81 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-error-2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      106 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-error-3.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      141 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-error-4.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       76 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-error-5.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       92 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-error-6.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       26 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-in.bin
--rw-r--r--   0 tstellar (101195) tstellar (101195)       55 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-in.dos
--rw-r--r--   0 tstellar (101195) tstellar (101195)       50 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-in.unix
--rw-r--r--   0 tstellar (101195) tstellar (101195)       24 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-in.utf16
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-in.utf8
--rw-r--r--   0 tstellar (101195) tstellar (101195)      734 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-pipes.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      274 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-r-error-0.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      346 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-r-error-1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-r-error-2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      251 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-r-error-3.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      273 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-r-error-4.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      282 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-r-error-5.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      271 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-r-error-6.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       61 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-r-error-7.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       61 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-r-error-8.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      675 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-r.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      358 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-strip-trailing-cr.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      976 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-unified.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      236 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/diff-w.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       17 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/echo-at-redirect-stderr.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       30 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/echo-at-redirect-stdin.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       16 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/echo-redirect-stderr.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       29 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/echo-redirect-stdin.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       95 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/error-0.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       71 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/error-1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       68 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/error-2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      248 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      106 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/mkdir-error-0.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      102 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/mkdir-error-1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       74 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/mkdir-error-2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1215 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/redirects.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      102 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/rm-error-0.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       92 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/rm-error-1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      128 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/rm-error-2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      120 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/rm-error-3.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      204 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/rm-unicode-0.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      738 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/sequencing-0.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       32 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/sequencing-1.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      157 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/stdout-encoding.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)     7169 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/valid-shell.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       94 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/write-to-stderr.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      153 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-shell/write-to-stdout-and-stderr.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.673331 lit-18.1.2/tests/Inputs/shtest-timeout/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       41 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-timeout/infinite_loop.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1217 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-timeout/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       82 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/shtest-timeout/short.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.673331 lit-18.1.2/tests/Inputs/standalone-tests/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/standalone-tests/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/standalone-tests/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.673331 lit-18.1.2/tests/Inputs/standalone-tests-with-excludes/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      154 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/standalone-tests-with-excludes/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/standalone-tests-with-excludes/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.673331 lit-18.1.2/tests/Inputs/standalone-tests-with-suffixes/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      153 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/standalone-tests-with-suffixes/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/standalone-tests-with-suffixes/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.673331 lit-18.1.2/tests/Inputs/test-data/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1172 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/test-data/dummy_format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/test-data/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       94 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/test-data/metrics.ini
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.673331 lit-18.1.2/tests/Inputs/test-data-micro/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1907 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/test-data-micro/dummy_format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/test-data-micro/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      220 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/test-data-micro/micro-tests.ini
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.673331 lit-18.1.2/tests/Inputs/test_retry_attempts/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      374 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/test_retry_attempts/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      553 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/test_retry_attempts/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.674331 lit-18.1.2/tests/Inputs/testrunner-custom-parsers/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      380 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/testrunner-custom-parsers/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      573 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/testrunner-custom-parsers/test.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.674331 lit-18.1.2/tests/Inputs/unittest-adaptor/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      182 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/unittest-adaptor/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/unittest-adaptor/test-one.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/unittest-adaptor/test-two.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.674331 lit-18.1.2/tests/Inputs/unparsed-requirements/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       76 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/unparsed-requirements/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.674331 lit-18.1.2/tests/Inputs/use-llvm-tool/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.675331 lit-18.1.2/tests/Inputs/use-llvm-tool/build/
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/build/case10
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/build/case10.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/build/case2
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/build/case2.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/build/case3
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/build/case3.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/build/case6
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/build/case6.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/build/case7
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/build/case7.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/build/case9
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/build/case9.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/env-case1
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/env-case6
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1435 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.675331 lit-18.1.2/tests/Inputs/use-llvm-tool/path/
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/path/case10
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/path/case10.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/path/case4
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/path/case4.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/path/case5
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/path/case5.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/path/case6
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/path/case6.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/path/case7
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/path/case7.exe
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.675331 lit-18.1.2/tests/Inputs/use-llvm-tool/search1/
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/search1/empty
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.675331 lit-18.1.2/tests/Inputs/use-llvm-tool/search2/
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/search2/case9
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/search2/case9.exe
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.675331 lit-18.1.2/tests/Inputs/use-llvm-tool/search3/
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/search3/case9
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/search3/case9.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.674331 lit-18.1.2/tests/Inputs/use-llvm-tool-required/
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool-required/found
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool-required/found.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)      483 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool-required/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/use-llvm-tool-required/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.675331 lit-18.1.2/tests/Inputs/xfail-cl/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.676331 lit-18.1.2/tests/Inputs/xfail-cl/a/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xfail-cl/a/false.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xfail-cl/a/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       23 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xfail-cl/a/test-xfail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xfail-cl/a/test.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.676331 lit-18.1.2/tests/Inputs/xfail-cl/b/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xfail-cl/b/false.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xfail-cl/b/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       24 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xfail-cl/b/test-xfail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xfail-cl/b/test.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xfail-cl/false.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xfail-cl/false2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xfail-cl/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       23 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xfail-cl/true-xfail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xfail-cl/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.676331 lit-18.1.2/tests/Inputs/xunit-output/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       95 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xunit-output/bad&name.ini
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1387 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xunit-output/dummy_format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)       69 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xunit-output/excluded.ini
--rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xunit-output/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      106 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xunit-output/missing_feature.ini
--rw-r--r--   0 tstellar (101195) tstellar (101195)       65 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xunit-output/pass.ini
--rw-r--r--   0 tstellar (101195) tstellar (101195)       72 2024-01-29 23:23:40.000000 lit-18.1.2/tests/Inputs/xunit-output/unsupported.ini
--rw-r--r--   0 tstellar (101195) tstellar (101195)     3312 2024-01-29 23:23:40.000000 lit-18.1.2/tests/allow-retries.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.2/tests/boolean-parsing.py
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)      199 2024-01-29 23:23:40.000000 lit-18.1.2/tests/check-tested-lit-timeout-ability
--rw-r--r--   0 tstellar (101195) tstellar (101195)      484 2024-01-29 23:23:40.000000 lit-18.1.2/tests/custom-result-category.py
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)    10036 2024-01-29 23:23:40.000000 lit-18.1.2/tests/discovery.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2024-01-29 23:23:40.000000 lit-18.1.2/tests/googletest-cmd-wrapper.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1009 2024-01-29 23:23:40.000000 lit-18.1.2/tests/googletest-crash.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      502 2024-01-29 23:23:40.000000 lit-18.1.2/tests/googletest-detect-duplicate.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      337 2024-01-29 23:23:40.000000 lit-18.1.2/tests/googletest-discovery-failed.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      800 2024-01-29 23:23:40.000000 lit-18.1.2/tests/googletest-format-respect-gtest-sharding-env-vars.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1432 2024-01-29 23:23:40.000000 lit-18.1.2/tests/googletest-format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1398 2024-01-29 23:23:40.000000 lit-18.1.2/tests/googletest-no-sharding.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1234 2024-01-29 23:23:40.000000 lit-18.1.2/tests/googletest-sanitizer-error.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2561 2024-01-29 23:23:40.000000 lit-18.1.2/tests/googletest-timeout.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      769 2024-01-29 23:23:40.000000 lit-18.1.2/tests/ignore-fail.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1103 2024-01-29 23:23:40.000000 lit-18.1.2/tests/lit-opts.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     5617 2024-01-29 23:23:40.000000 lit-18.1.2/tests/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      410 2024-01-29 23:23:40.000000 lit-18.1.2/tests/lit.site.cfg.in
--rw-r--r--   0 tstellar (101195) tstellar (101195)      176 2024-01-29 23:23:40.000000 lit-18.1.2/tests/lld-features.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1001 2024-01-29 23:23:40.000000 lit-18.1.2/tests/max-failures.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      234 2024-01-29 23:23:40.000000 lit-18.1.2/tests/max-time.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      558 2024-01-29 23:23:40.000000 lit-18.1.2/tests/parallelism-groups.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1061 2024-01-29 23:23:40.000000 lit-18.1.2/tests/per-test-coverage-by-lit-cfg.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      970 2024-01-29 23:23:40.000000 lit-18.1.2/tests/per-test-coverage.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      538 2024-01-29 23:23:40.000000 lit-18.1.2/tests/progress-bar.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      732 2024-01-29 23:23:40.000000 lit-18.1.2/tests/reorder.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     6440 2024-01-29 23:23:40.000000 lit-18.1.2/tests/selecting.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)       67 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shell-parsing.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      847 2024-01-29 23:23:40.000000 lit-18.1.2/tests/show-result-codes.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      512 2024-01-29 23:23:40.000000 lit-18.1.2/tests/show-used-features.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     6660 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-define.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)       72 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-encoding.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     5554 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-env.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1224 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-external-shell-kill.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      588 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-format-argv0.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     7589 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      751 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-if-else.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1468 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-inject.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      581 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-keyword-parse-errors.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     8088 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-not.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1954 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-output-printing.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      713 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-pushd-popd.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1593 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-recursive-substitution.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     3624 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-run-at-line.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    22636 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-shell.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     3498 2024-01-29 23:23:40.000000 lit-18.1.2/tests/shtest-timeout.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      679 2024-01-29 23:23:40.000000 lit-18.1.2/tests/test-data-micro.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      353 2024-01-29 23:23:40.000000 lit-18.1.2/tests/test-data.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2380 2024-01-29 23:23:40.000000 lit-18.1.2/tests/test-output-micro-resultdb.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1624 2024-01-29 23:23:40.000000 lit-18.1.2/tests/test-output-micro.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1546 2024-01-29 23:23:40.000000 lit-18.1.2/tests/test-output-resultdb.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      552 2024-01-29 23:23:40.000000 lit-18.1.2/tests/test-output.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-03-21 17:55:34.676331 lit-18.1.2/tests/unit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     4360 2024-01-29 23:23:40.000000 lit-18.1.2/tests/unit/ShUtil.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    14388 2024-01-29 23:23:40.000000 lit-18.1.2/tests/unit/TestRunner.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      460 2024-01-29 23:23:40.000000 lit-18.1.2/tests/unittest-adaptor.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      816 2024-01-29 23:23:40.000000 lit-18.1.2/tests/unparsed-requirements.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2024-01-29 23:23:40.000000 lit-18.1.2/tests/usage.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2077 2024-01-29 23:23:40.000000 lit-18.1.2/tests/use-llvm-tool.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1860 2024-01-29 23:23:40.000000 lit-18.1.2/tests/xfail-cl.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1486 2024-01-29 23:23:40.000000 lit-18.1.2/tests/xunit-output.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.568621 lit-18.1.3/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    15141 2024-01-29 23:23:40.000000 lit-18.1.3/LICENSE.TXT
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      242 2024-01-29 23:23:40.000000 lit-18.1.3/MANIFEST.in
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2516 2024-04-11 19:00:19.567621 lit-18.1.3/PKG-INFO
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1874 2024-01-29 23:23:40.000000 lit-18.1.3/README.rst
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.537621 lit-18.1.3/examples/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      236 2024-01-29 23:23:40.000000 lit-18.1.3/examples/README.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.537621 lit-18.1.3/examples/many-tests/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      549 2024-01-29 23:23:40.000000 lit-18.1.3/examples/many-tests/ManyTests.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      382 2024-01-29 23:23:40.000000 lit-18.1.3/examples/many-tests/README.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      147 2024-01-29 23:23:40.000000 lit-18.1.3/examples/many-tests/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.539621 lit-18.1.3/lit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    12039 2024-01-29 23:23:40.000000 lit-18.1.3/lit/BooleanExpression.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     8431 2024-01-29 23:23:40.000000 lit-18.1.3/lit/LitConfig.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1593 2024-01-29 23:23:40.000000 lit-18.1.3/lit/LitTestCase.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    11087 2024-01-29 23:23:40.000000 lit-18.1.3/lit/ProgressBar.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     3242 2024-01-29 23:23:40.000000 lit-18.1.3/lit/ShCommands.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     8811 2024-01-29 23:23:40.000000 lit-18.1.3/lit/ShUtil.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    13734 2024-01-29 23:23:40.000000 lit-18.1.3/lit/Test.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    84905 2024-01-29 23:23:40.000000 lit-18.1.3/lit/TestRunner.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1629 2024-01-29 23:23:40.000000 lit-18.1.3/lit/TestTimes.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     8690 2024-01-29 23:23:40.000000 lit-18.1.3/lit/TestingConfig.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      191 2024-04-11 18:59:56.000000 lit-18.1.3/lit/__init__.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.540621 lit-18.1.3/lit/builtin_commands/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/lit/builtin_commands/__init__.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1892 2024-01-29 23:23:40.000000 lit-18.1.3/lit/builtin_commands/cat.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     9802 2024-01-29 23:23:40.000000 lit-18.1.3/lit/builtin_commands/diff.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    11174 2024-01-29 23:23:40.000000 lit-18.1.3/lit/cl_arguments.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     9618 2024-01-29 23:23:40.000000 lit-18.1.3/lit/discovery.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     5987 2024-01-29 23:23:40.000000 lit-18.1.3/lit/display.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.541621 lit-18.1.3/lit/formats/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      215 2024-01-29 23:23:40.000000 lit-18.1.3/lit/formats/__init__.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2299 2024-01-29 23:23:40.000000 lit-18.1.3/lit/formats/base.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    14953 2024-01-29 23:23:40.000000 lit-18.1.3/lit/formats/googletest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      992 2024-01-29 23:23:40.000000 lit-18.1.3/lit/formats/shtest.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.541621 lit-18.1.3/lit/llvm/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      176 2024-01-29 23:23:40.000000 lit-18.1.3/lit/llvm/__init__.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    32023 2024-01-29 23:23:40.000000 lit-18.1.3/lit/llvm/config.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     5430 2024-01-29 23:23:40.000000 lit-18.1.3/lit/llvm/subst.py
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)    11855 2024-01-29 23:23:40.000000 lit-18.1.3/lit/main.py
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)    11056 2024-01-29 23:23:40.000000 lit-18.1.3/lit/reports.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     4692 2024-01-29 23:23:40.000000 lit-18.1.3/lit/run.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    17299 2024-01-29 23:23:40.000000 lit-18.1.3/lit/util.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2666 2024-01-29 23:23:40.000000 lit-18.1.3/lit/worker.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.540621 lit-18.1.3/lit.egg-info/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     2516 2024-04-11 19:00:19.000000 lit-18.1.3/lit.egg-info/PKG-INFO
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)    22457 2024-04-11 19:00:19.000000 lit-18.1.3/lit.egg-info/SOURCES.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        1 2024-04-11 19:00:19.000000 lit-18.1.3/lit.egg-info/dependency_links.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       38 2024-04-11 19:00:19.000000 lit-18.1.3/lit.egg-info/entry_points.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        1 2023-04-10 18:12:43.000000 lit-18.1.3/lit.egg-info/not-zip-safe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        4 2024-04-11 19:00:19.000000 lit-18.1.3/lit.egg-info/top_level.txt
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)       89 2024-01-29 23:23:40.000000 lit-18.1.3/lit.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       81 2024-01-29 23:23:40.000000 lit-18.1.3/pyproject.toml
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       38 2024-04-11 19:00:19.568621 lit-18.1.3/setup.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1295 2024-01-29 23:23:40.000000 lit-18.1.3/setup.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.545621 lit-18.1.3/tests/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      152 2024-01-29 23:23:40.000000 lit-18.1.3/tests/.coveragerc
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.545621 lit-18.1.3/tests/Inputs/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.545621 lit-18.1.3/tests/Inputs/allow-retries/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       33 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/allow-retries/does-not-succeed-within-limit.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      337 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/allow-retries/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       51 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/allow-retries/more-than-one-allow-retries-lines.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       45 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/allow-retries/not-a-valid-integer.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      573 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/allow-retries/succeeds-within-limit.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.545621 lit-18.1.3/tests/Inputs/config-map-discovery/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      434 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/config-map-discovery/driver.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/config-map-discovery/invalid-test.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      297 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/config-map-discovery/lit.alt.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.545621 lit-18.1.3/tests/Inputs/config-map-discovery/main-config/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       33 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/config-map-discovery/main-config/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.546621 lit-18.1.3/tests/Inputs/config-map-discovery/tests/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/config-map-discovery/tests/test1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/config-map-discovery/tests/test2.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.546621 lit-18.1.3/tests/Inputs/custom-result-category/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      467 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/custom-result-category/format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      247 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/custom-result-category/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/custom-result-category/test1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/custom-result-category/test2.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.546621 lit-18.1.3/tests/Inputs/discovery/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      762 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/discovery/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.546621 lit-18.1.3/tests/Inputs/discovery/subdir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      141 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/discovery/subdir/lit.local.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/discovery/subdir/test-three.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.546621 lit-18.1.3/tests/Inputs/discovery/subsuite/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      175 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/discovery/subsuite/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/discovery/subsuite/test-one.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/discovery/subsuite/test-two.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/discovery/test-one.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/discovery/test-two.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/discovery/test.not-txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.546621 lit-18.1.3/tests/Inputs/discovery-getTestsForPath/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      538 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/discovery-getTestsForPath/custom_format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      270 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/discovery-getTestsForPath/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/discovery-getTestsForPath/x.test
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.546621 lit-18.1.3/tests/Inputs/exec-discovery/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      292 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/exec-discovery/lit.site.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.547621 lit-18.1.3/tests/Inputs/exec-discovery-in-tree/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      308 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/exec-discovery-in-tree/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.547621 lit-18.1.3/tests/Inputs/exec-discovery-in-tree/obj/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      205 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/exec-discovery-in-tree/obj/lit.site.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/exec-discovery-in-tree/test-one.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.547621 lit-18.1.3/tests/Inputs/fake-externals/
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/fake-externals/cd
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/fake-externals/diff
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/fake-externals/env
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/fake-externals/export
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      208 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/fake-externals/fake_external.py
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/fake-externals/mkdir
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/fake-externals/rm
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.547621 lit-18.1.3/tests/Inputs/googletest-cmd-wrapper/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.547621 lit-18.1.3/tests/Inputs/googletest-cmd-wrapper/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1267 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-cmd-wrapper/DummySubDir/OneTest.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      189 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-cmd-wrapper/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.547621 lit-18.1.3/tests/Inputs/googletest-crash/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.547621 lit-18.1.3/tests/Inputs/googletest-crash/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1424 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-crash/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      120 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-crash/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.547621 lit-18.1.3/tests/Inputs/googletest-detect-duplicate/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.547621 lit-18.1.3/tests/Inputs/googletest-detect-duplicate/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1350 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-detect-duplicate/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      131 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-detect-duplicate/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.547621 lit-18.1.3/tests/Inputs/googletest-discovery-failed/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-discovery-failed/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.547621 lit-18.1.3/tests/Inputs/googletest-discovery-failed/subdir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       80 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-discovery-failed/subdir/OneTest.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.547621 lit-18.1.3/tests/Inputs/googletest-format/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.548621 lit-18.1.3/tests/Inputs/googletest-format/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2741 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-format/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-format/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.547621 lit-18.1.3/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.548621 lit-18.1.3/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2742 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.548621 lit-18.1.3/tests/Inputs/googletest-no-sharding/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.548621 lit-18.1.3/tests/Inputs/googletest-no-sharding/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2562 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-no-sharding/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-no-sharding/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.548621 lit-18.1.3/tests/Inputs/googletest-sanitizer-error/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.548621 lit-18.1.3/tests/Inputs/googletest-sanitizer-error/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1506 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-sanitizer-error/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      130 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-sanitizer-error/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.548621 lit-18.1.3/tests/Inputs/googletest-timeout/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.548621 lit-18.1.3/tests/Inputs/googletest-timeout/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1685 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-timeout/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      397 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/googletest-timeout/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.548621 lit-18.1.3/tests/Inputs/ignore-fail/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/ignore-fail/fail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      177 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/ignore-fail/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/ignore-fail/unresolved.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       20 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/ignore-fail/xfail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       19 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/ignore-fail/xpass.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.548621 lit-18.1.3/tests/Inputs/lit-opts/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      253 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lit-opts/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       17 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lit-opts/test.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      223 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.549621 lit-18.1.3/tests/Inputs/lld-features/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lld-features/ld.lld
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lld-features/ld.lld.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       31 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lld-features/ld.lld.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lld-features/ld64.lld
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lld-features/ld64.lld.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       33 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lld-features/ld64.lld.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      714 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lld-features/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lld-features/lld-link
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lld-features/lld-link.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       33 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lld-features/lld-link.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lld-features/wasm-ld
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lld-features/wasm-ld.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       32 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/lld-features/wasm-ld.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.549621 lit-18.1.3/tests/Inputs/max-failures/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/max-failures/fail1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/max-failures/fail2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/max-failures/fail3.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      178 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/max-failures/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.549621 lit-18.1.3/tests/Inputs/max-time/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       10 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/max-time/fast.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      251 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/max-time/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      128 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/max-time/slow.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.549621 lit-18.1.3/tests/Inputs/parallelism-groups/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      474 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/parallelism-groups/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/parallelism-groups/test1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/parallelism-groups/test2.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.549621 lit-18.1.3/tests/Inputs/per-test-coverage/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      337 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/per-test-coverage/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      354 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/per-test-coverage/per-test-coverage.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.550621 lit-18.1.3/tests/Inputs/per-test-coverage-by-lit-cfg/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      384 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/per-test-coverage-by-lit-cfg/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      365 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/per-test-coverage-by-lit-cfg/per-test-coverage-by-lit-cfg.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.550621 lit-18.1.3/tests/Inputs/progress-bar/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      178 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/progress-bar/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/progress-bar/test-1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/progress-bar/test-2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/progress-bar/test-3.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/progress-bar/test-4.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.550621 lit-18.1.3/tests/Inputs/py-config-discovery/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      299 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/py-config-discovery/lit.site.cfg.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.550621 lit-18.1.3/tests/Inputs/reorder/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/reorder/aaa.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/reorder/bbb.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/reorder/fff.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      173 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/reorder/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       78 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/reorder/lit_test_times
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/reorder/new-test.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.550621 lit-18.1.3/tests/Inputs/reorder/subdir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/reorder/subdir/ccc.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.551621 lit-18.1.3/tests/Inputs/show-result-codes/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/show-result-codes/fail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      183 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/show-result-codes/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       10 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/show-result-codes/pass.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       36 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/show-result-codes/unsupported.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       20 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/show-result-codes/xfail.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.551621 lit-18.1.3/tests/Inputs/show-used-features/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      184 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/show-used-features/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      267 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/show-used-features/mixed.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       35 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/show-used-features/requires.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       42 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/show-used-features/unsupported.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       30 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/show-used-features/xfail.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.551621 lit-18.1.3/tests/Inputs/shtest-define/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.551621 lit-18.1.3/tests/Inputs/shtest-define/errors/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.552621 lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      227 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/before-name.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      282 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/between-name-equals.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      209 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/braces-empty.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      530 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/braces-with-dot.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      267 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/braces-with-equals.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      239 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/braces-with-newline.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      513 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/braces-with-number.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      230 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/braces-with-ws.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      208 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/empty.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      219 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/no-equals.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      208 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/no-name.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      245 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/ws-only.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.553621 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      295 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/empty.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      352 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/end-in-double-backslash.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      443 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/unterminated-define-bad-redefine.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      312 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/unterminated-define-continuation.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      450 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/unterminated-define-redefine.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      252 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/unterminated-define-run.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      277 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/unterminated-define.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      447 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-bad-define.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      336 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-continuation.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      447 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-define.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      276 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-run.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      291 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      239 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/unterminated-run-define.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      257 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/unterminated-run-redefine.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      336 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/continuation/ws-only.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.554621 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      342 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/define-already-by-config.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      341 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/define-already-by-test.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      347 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/define-inside-pattern.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      432 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/define-multiple-exact.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      459 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/define-multiple-once-exact.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      356 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/define-prefixes-pattern.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      345 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/define-suffixes-pattern.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      422 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/redefine-inside-pattern.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      634 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-exact.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      608 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-once-exact.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/redefine-none.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      431 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/redefine-prefixes-pattern.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      420 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/redefine-suffixes-pattern.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      296 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/location-range.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      209 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/errors/no-run.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.554621 lit-18.1.3/tests/Inputs/shtest-define/examples/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1808 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/examples/param-subst.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1718 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/expansion-order.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1262 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/line-number-substitutions.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2668 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      703 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/name-chars.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      296 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/recursiveExpansionLimit.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      723 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/shared-substs-0.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      723 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/shared-substs-1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      921 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/value-equals.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      538 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/value-escaped.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     4018 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-define/ws-and-continuations.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.555621 lit-18.1.3/tests/Inputs/shtest-env/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       17 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-args-last-is-assign.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       18 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-args-last-is-u-arg.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       14 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-args-last-is-u.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       19 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-args-nested-none.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-args-none.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       34 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-calls-cd.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       26 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-calls-colon.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       41 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-calls-echo.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      875 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-calls-env.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       37 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-calls-export.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       37 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-calls-mkdir.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      198 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-calls-not-builtin.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       34 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-calls-rm.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      687 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env-u.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      465 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/env.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      310 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      585 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/mixed.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      188 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-env/print_environment.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.555621 lit-18.1.3/tests/Inputs/shtest-external-shell-kill/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      153 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-external-shell-kill/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       92 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-external-shell-kill/test.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.556621 lit-18.1.3/tests/Inputs/shtest-format/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.556621 lit-18.1.3/tests/Inputs/shtest-format/external_shell/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      181 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/external_shell/fail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      107 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/external_shell/fail_with_bad_encoding.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      191 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/external_shell/fail_with_control_chars.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       83 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/external_shell/lit.local.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/external_shell/pass.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       61 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/external_shell/utf8_command.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      138 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/external_shell/write-bad-encoding.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      146 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/external_shell/write-control-chars.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      104 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/fail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      414 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        9 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/no-test-line.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/pass.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      128 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/requires-missing.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      122 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/requires-present.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       49 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/requires-star.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      114 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/requires-triple.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      218 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/unsupported-expr-false.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      174 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/unsupported-expr-true.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       52 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/unsupported-star.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.556621 lit-18.1.3/tests/Inputs/shtest-format/unsupported_dir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       26 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/unsupported_dir/lit.local.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/unsupported_dir/some-test.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      147 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/xfail-expr-false.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      151 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/xfail-expr-true.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       40 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/xfail-feature.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       38 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/xfail-target.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       20 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/xfail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       37 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format/xpass.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.556621 lit-18.1.3/tests/Inputs/shtest-format-argv0/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      320 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format-argv0/argv0.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      233 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-format-argv0/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.557621 lit-18.1.3/tests/Inputs/shtest-if-else/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      267 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-if-else/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       93 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-if-else/test-neg1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       87 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-if-else/test-neg2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      103 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-if-else/test-neg3.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      106 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-if-else/test-neg4.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     3487 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-if-else/test.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.557621 lit-18.1.3/tests/Inputs/shtest-inject/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      314 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-inject/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      109 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-inject/test-empty.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      183 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-inject/test-many.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-inject/test-one.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.557621 lit-18.1.3/tests/Inputs/shtest-keyword-parse-errors/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-keyword-parse-errors/empty.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      133 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-keyword-parse-errors/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       44 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-keyword-parse-errors/multiple-allow-retries.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       29 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-keyword-parse-errors/unterminated-run.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.558621 lit-18.1.3/tests/Inputs/shtest-not/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/exclamation-args-nested-none.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        9 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/exclamation-args-none.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      211 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/exclamation-calls-external.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      100 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/fail.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      100 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/fail2.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       19 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-args-last-is-crash.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       19 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-args-nested-none.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-args-none.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       85 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-calls-cd.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       68 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-calls-colon.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      252 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-calls-diff-with-crash.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      413 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-calls-diff.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      103 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-calls-echo.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      207 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-calls-env-builtin.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       97 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-calls-export.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1933 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-calls-external.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      142 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-calls-fail2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       59 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-calls-mkdir.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       46 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/not-calls-rm.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       77 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/pass.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      159 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-not/print_environment.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.558621 lit-18.1.3/tests/Inputs/shtest-output-printing/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      125 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-output-printing/basic.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      216 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-output-printing/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      127 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-output-printing/write-a-lot.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.559621 lit-18.1.3/tests/Inputs/shtest-pushd-popd/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      145 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-pushd-popd/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       19 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-pushd-popd/popd-args.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       11 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-pushd-popd/popd-no-stack.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      223 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-pushd-popd/pushd-popd-ok.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       16 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-pushd-popd/pushd-too-many-args.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.536621 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.559621 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      340 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       18 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.559621 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      380 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       18 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.559621 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/escaping/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/escaping/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       28 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/escaping/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.559621 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/negative-integer/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      218 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/negative-integer/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/negative-integer/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.559621 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/not-an-integer/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      230 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/not-an-integer/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/not-an-integer/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.559621 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/set-to-none/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      215 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/set-to-none/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/set-to-none/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.559621 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      372 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       18 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.560621 lit-18.1.3/tests/Inputs/shtest-run-at-line/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.560621 lit-18.1.3/tests/Inputs/shtest-run-at-line/external-shell/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      125 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-run-at-line/external-shell/basic.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       50 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-run-at-line/external-shell/empty-run-line.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      253 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-run-at-line/external-shell/line-continuation.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      180 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-run-at-line/external-shell/lit.local.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       42 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-run-at-line/external-shell/run-line-with-newline.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.560621 lit-18.1.3/tests/Inputs/shtest-run-at-line/internal-shell/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       37 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-run-at-line/internal-shell/basic.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       50 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-run-at-line/internal-shell/empty-run-line.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      221 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-run-at-line/internal-shell/line-continuation.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      181 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-run-at-line/internal-shell/lit.local.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       42 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-run-at-line/internal-shell/run-line-with-newline.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       62 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-run-at-line/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.563621 lit-18.1.3/tests/Inputs/shtest-shell/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       75 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/cat-error-0.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       87 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/cat-error-1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      269 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/cat_nonprinting.bin
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/check_args.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      622 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/check_path.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       94 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/colon-error.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      373 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/continuations.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      513 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/dev-null.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      274 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-I.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      181 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-b.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      622 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-encodings.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      102 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-error-1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       81 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-error-2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      106 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-error-3.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      141 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-error-4.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       76 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-error-5.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       92 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-error-6.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       26 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-in.bin
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       55 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-in.dos
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       50 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-in.unix
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       24 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-in.utf16
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-in.utf8
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      734 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-pipes.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      274 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-r-error-0.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      346 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-r-error-1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-r-error-2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      251 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-r-error-3.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      273 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-r-error-4.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      282 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-r-error-5.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      271 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-r-error-6.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       61 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-r-error-7.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       61 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-r-error-8.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      675 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-r.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      358 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-strip-trailing-cr.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      976 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-unified.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      236 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/diff-w.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       17 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/echo-at-redirect-stderr.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       30 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/echo-at-redirect-stdin.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       16 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/echo-redirect-stderr.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       29 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/echo-redirect-stdin.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       95 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/error-0.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       71 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/error-1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       68 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/error-2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      248 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      106 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/mkdir-error-0.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      102 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/mkdir-error-1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       74 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/mkdir-error-2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1215 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/redirects.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      102 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/rm-error-0.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       92 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/rm-error-1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      128 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/rm-error-2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      120 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/rm-error-3.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      204 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/rm-unicode-0.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      738 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/sequencing-0.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       32 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/sequencing-1.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      157 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/stdout-encoding.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     7169 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/valid-shell.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       94 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/write-to-stderr.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      153 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-shell/write-to-stdout-and-stderr.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.563621 lit-18.1.3/tests/Inputs/shtest-timeout/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       41 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-timeout/infinite_loop.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1217 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-timeout/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       82 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/shtest-timeout/short.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.563621 lit-18.1.3/tests/Inputs/standalone-tests/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/standalone-tests/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/standalone-tests/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.564621 lit-18.1.3/tests/Inputs/standalone-tests-with-excludes/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      154 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/standalone-tests-with-excludes/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/standalone-tests-with-excludes/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.564621 lit-18.1.3/tests/Inputs/standalone-tests-with-suffixes/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      153 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/standalone-tests-with-suffixes/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/standalone-tests-with-suffixes/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.564621 lit-18.1.3/tests/Inputs/test-data/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1172 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/test-data/dummy_format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/test-data/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       94 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/test-data/metrics.ini
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.564621 lit-18.1.3/tests/Inputs/test-data-micro/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1907 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/test-data-micro/dummy_format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/test-data-micro/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      220 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/test-data-micro/micro-tests.ini
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.564621 lit-18.1.3/tests/Inputs/test_retry_attempts/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      374 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/test_retry_attempts/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      553 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/test_retry_attempts/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.564621 lit-18.1.3/tests/Inputs/testrunner-custom-parsers/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      380 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/testrunner-custom-parsers/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      573 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/testrunner-custom-parsers/test.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.564621 lit-18.1.3/tests/Inputs/unittest-adaptor/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      182 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/unittest-adaptor/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/unittest-adaptor/test-one.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/unittest-adaptor/test-two.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.564621 lit-18.1.3/tests/Inputs/unparsed-requirements/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       76 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/unparsed-requirements/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.565621 lit-18.1.3/tests/Inputs/use-llvm-tool/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.565621 lit-18.1.3/tests/Inputs/use-llvm-tool/build/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/build/case10
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/build/case10.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/build/case2
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/build/case2.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/build/case3
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/build/case3.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/build/case6
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/build/case6.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/build/case7
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/build/case7.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/build/case9
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/build/case9.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/env-case1
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/env-case6
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1435 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.566621 lit-18.1.3/tests/Inputs/use-llvm-tool/path/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/path/case10
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/path/case10.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/path/case4
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/path/case4.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/path/case5
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/path/case5.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/path/case6
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/path/case6.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/path/case7
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/path/case7.exe
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.566621 lit-18.1.3/tests/Inputs/use-llvm-tool/search1/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/search1/empty
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.566621 lit-18.1.3/tests/Inputs/use-llvm-tool/search2/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/search2/case9
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/search2/case9.exe
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.566621 lit-18.1.3/tests/Inputs/use-llvm-tool/search3/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/search3/case9
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/search3/case9.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.565621 lit-18.1.3/tests/Inputs/use-llvm-tool-required/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool-required/found
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool-required/found.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      483 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool-required/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/use-llvm-tool-required/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.566621 lit-18.1.3/tests/Inputs/xfail-cl/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.566621 lit-18.1.3/tests/Inputs/xfail-cl/a/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xfail-cl/a/false.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xfail-cl/a/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       23 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xfail-cl/a/test-xfail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xfail-cl/a/test.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.567621 lit-18.1.3/tests/Inputs/xfail-cl/b/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xfail-cl/b/false.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xfail-cl/b/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       24 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xfail-cl/b/test-xfail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xfail-cl/b/test.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xfail-cl/false.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       13 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xfail-cl/false2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xfail-cl/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       23 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xfail-cl/true-xfail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       12 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xfail-cl/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.567621 lit-18.1.3/tests/Inputs/xunit-output/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       95 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xunit-output/bad&name.ini
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1387 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xunit-output/dummy_format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       69 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xunit-output/excluded.ini
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xunit-output/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      106 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xunit-output/missing_feature.ini
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       65 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xunit-output/pass.ini
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       72 2024-01-29 23:23:40.000000 lit-18.1.3/tests/Inputs/xunit-output/unsupported.ini
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     3312 2024-01-29 23:23:40.000000 lit-18.1.3/tests/allow-retries.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2024-01-29 23:23:40.000000 lit-18.1.3/tests/boolean-parsing.py
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)      199 2024-01-29 23:23:40.000000 lit-18.1.3/tests/check-tested-lit-timeout-ability
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      484 2024-01-29 23:23:40.000000 lit-18.1.3/tests/custom-result-category.py
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)    10036 2024-01-29 23:23:40.000000 lit-18.1.3/tests/discovery.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2024-01-29 23:23:40.000000 lit-18.1.3/tests/googletest-cmd-wrapper.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1009 2024-01-29 23:23:40.000000 lit-18.1.3/tests/googletest-crash.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      502 2024-01-29 23:23:40.000000 lit-18.1.3/tests/googletest-detect-duplicate.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      337 2024-01-29 23:23:40.000000 lit-18.1.3/tests/googletest-discovery-failed.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      800 2024-01-29 23:23:40.000000 lit-18.1.3/tests/googletest-format-respect-gtest-sharding-env-vars.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1432 2024-01-29 23:23:40.000000 lit-18.1.3/tests/googletest-format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1398 2024-01-29 23:23:40.000000 lit-18.1.3/tests/googletest-no-sharding.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1234 2024-01-29 23:23:40.000000 lit-18.1.3/tests/googletest-sanitizer-error.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2561 2024-01-29 23:23:40.000000 lit-18.1.3/tests/googletest-timeout.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      769 2024-01-29 23:23:40.000000 lit-18.1.3/tests/ignore-fail.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1103 2024-01-29 23:23:40.000000 lit-18.1.3/tests/lit-opts.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     5617 2024-01-29 23:23:40.000000 lit-18.1.3/tests/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      410 2024-01-29 23:23:40.000000 lit-18.1.3/tests/lit.site.cfg.in
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      176 2024-01-29 23:23:40.000000 lit-18.1.3/tests/lld-features.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1001 2024-01-29 23:23:40.000000 lit-18.1.3/tests/max-failures.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      234 2024-01-29 23:23:40.000000 lit-18.1.3/tests/max-time.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      558 2024-01-29 23:23:40.000000 lit-18.1.3/tests/parallelism-groups.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1061 2024-01-29 23:23:40.000000 lit-18.1.3/tests/per-test-coverage-by-lit-cfg.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      970 2024-01-29 23:23:40.000000 lit-18.1.3/tests/per-test-coverage.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      538 2024-01-29 23:23:40.000000 lit-18.1.3/tests/progress-bar.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      732 2024-01-29 23:23:40.000000 lit-18.1.3/tests/reorder.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     6440 2024-01-29 23:23:40.000000 lit-18.1.3/tests/selecting.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       67 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shell-parsing.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      847 2024-01-29 23:23:40.000000 lit-18.1.3/tests/show-result-codes.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      512 2024-01-29 23:23:40.000000 lit-18.1.3/tests/show-used-features.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     6660 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-define.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       72 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-encoding.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     5554 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-env.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1224 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-external-shell-kill.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      588 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-format-argv0.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     7589 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      751 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-if-else.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1468 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-inject.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      581 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-keyword-parse-errors.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     8088 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-not.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1954 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-output-printing.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      713 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-pushd-popd.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1593 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-recursive-substitution.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     3624 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-run-at-line.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    22636 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-shell.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     3498 2024-01-29 23:23:40.000000 lit-18.1.3/tests/shtest-timeout.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      679 2024-01-29 23:23:40.000000 lit-18.1.3/tests/test-data-micro.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      353 2024-01-29 23:23:40.000000 lit-18.1.3/tests/test-data.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2380 2024-01-29 23:23:40.000000 lit-18.1.3/tests/test-output-micro-resultdb.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1624 2024-01-29 23:23:40.000000 lit-18.1.3/tests/test-output-micro.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1546 2024-01-29 23:23:40.000000 lit-18.1.3/tests/test-output-resultdb.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      552 2024-01-29 23:23:40.000000 lit-18.1.3/tests/test-output.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2024-04-11 19:00:19.567621 lit-18.1.3/tests/unit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     4360 2024-01-29 23:23:40.000000 lit-18.1.3/tests/unit/ShUtil.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    14388 2024-01-29 23:23:40.000000 lit-18.1.3/tests/unit/TestRunner.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      460 2024-01-29 23:23:40.000000 lit-18.1.3/tests/unittest-adaptor.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      816 2024-01-29 23:23:40.000000 lit-18.1.3/tests/unparsed-requirements.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2024-01-29 23:23:40.000000 lit-18.1.3/tests/usage.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2077 2024-01-29 23:23:40.000000 lit-18.1.3/tests/use-llvm-tool.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1860 2024-01-29 23:23:40.000000 lit-18.1.3/tests/xfail-cl.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1486 2024-01-29 23:23:40.000000 lit-18.1.3/tests/xunit-output.py
```

### Comparing `lit-18.1.2/LICENSE.TXT` & `lit-18.1.3/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/PKG-INFO` & `lit-18.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit
-Version: 18.1.2
+Version: 18.1.3
 Summary: A Software Testing Tool
 Home-page: http://llvm.org
 Author: Daniel Dunbar
 Author-email: daniel@minormatter.com
 License: Apache-2.0 with LLVM exception
 Keywords: test C++ automatic discovery
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lit-18.1.2/README.rst` & `lit-18.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/examples/many-tests/ManyTests.py` & `lit-18.1.3/examples/many-tests/ManyTests.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/BooleanExpression.py` & `lit-18.1.3/lit/BooleanExpression.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/LitConfig.py` & `lit-18.1.3/lit/LitConfig.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/LitTestCase.py` & `lit-18.1.3/lit/LitTestCase.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/ProgressBar.py` & `lit-18.1.3/lit/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/ShCommands.py` & `lit-18.1.3/lit/ShCommands.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/ShUtil.py` & `lit-18.1.3/lit/ShUtil.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/Test.py` & `lit-18.1.3/lit/Test.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/TestRunner.py` & `lit-18.1.3/lit/TestRunner.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/TestTimes.py` & `lit-18.1.3/lit/TestTimes.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/TestingConfig.py` & `lit-18.1.3/lit/TestingConfig.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/builtin_commands/cat.py` & `lit-18.1.3/lit/builtin_commands/cat.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/builtin_commands/diff.py` & `lit-18.1.3/lit/builtin_commands/diff.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/cl_arguments.py` & `lit-18.1.3/lit/cl_arguments.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/discovery.py` & `lit-18.1.3/lit/discovery.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/display.py` & `lit-18.1.3/lit/display.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/formats/base.py` & `lit-18.1.3/lit/formats/base.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/formats/googletest.py` & `lit-18.1.3/lit/formats/googletest.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/formats/shtest.py` & `lit-18.1.3/lit/formats/shtest.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/llvm/config.py` & `lit-18.1.3/lit/llvm/config.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/llvm/subst.py` & `lit-18.1.3/lit/llvm/subst.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/main.py` & `lit-18.1.3/lit/main.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/reports.py` & `lit-18.1.3/lit/reports.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/run.py` & `lit-18.1.3/lit/run.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/util.py` & `lit-18.1.3/lit/util.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit/worker.py` & `lit-18.1.3/lit/worker.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/lit.egg-info/PKG-INFO` & `lit-18.1.3/lit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit
-Version: 18.1.2
+Version: 18.1.3
 Summary: A Software Testing Tool
 Home-page: http://llvm.org
 Author: Daniel Dunbar
 Author-email: daniel@minormatter.com
 License: Apache-2.0 with LLVM exception
 Keywords: test C++ automatic discovery
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lit-18.1.2/lit.egg-info/SOURCES.txt` & `lit-18.1.3/lit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/setup.py` & `lit-18.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/allow-retries/succeeds-within-limit.py` & `lit-18.1.3/tests/Inputs/allow-retries/succeeds-within-limit.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/discovery/lit.cfg` & `lit-18.1.3/tests/Inputs/discovery/lit.cfg`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/discovery-getTestsForPath/custom_format.py` & `lit-18.1.3/tests/Inputs/discovery-getTestsForPath/custom_format.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/googletest-cmd-wrapper/DummySubDir/OneTest.exe` & `lit-18.1.3/tests/Inputs/googletest-cmd-wrapper/DummySubDir/OneTest.exe`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/googletest-crash/DummySubDir/OneTest.py` & `lit-18.1.3/tests/Inputs/googletest-crash/DummySubDir/OneTest.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/googletest-detect-duplicate/DummySubDir/OneTest.py` & `lit-18.1.3/tests/Inputs/googletest-detect-duplicate/DummySubDir/OneTest.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/googletest-format/DummySubDir/OneTest.py` & `lit-18.1.3/tests/Inputs/googletest-format/DummySubDir/OneTest.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/OneTest.py` & `lit-18.1.3/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/OneTest.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/googletest-no-sharding/DummySubDir/OneTest.py` & `lit-18.1.3/tests/Inputs/googletest-no-sharding/DummySubDir/OneTest.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/googletest-sanitizer-error/DummySubDir/OneTest.py` & `lit-18.1.3/tests/Inputs/googletest-sanitizer-error/DummySubDir/OneTest.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/googletest-timeout/DummySubDir/OneTest.py` & `lit-18.1.3/tests/Inputs/googletest-timeout/DummySubDir/OneTest.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/lld-features/lit.cfg` & `lit-18.1.3/tests/Inputs/lld-features/lit.cfg`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/braces-with-dot.txt` & `lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/braces-with-dot.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/errors/assignment/braces-with-number.txt` & `lit-18.1.3/tests/Inputs/shtest-define/errors/assignment/braces-with-number.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-exact.txt` & `lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-exact.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-once-exact.txt` & `lit-18.1.3/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-once-exact.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/examples/param-subst.txt` & `lit-18.1.3/tests/Inputs/shtest-define/examples/param-subst.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/expansion-order.txt` & `lit-18.1.3/tests/Inputs/shtest-define/expansion-order.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/line-number-substitutions.txt` & `lit-18.1.3/tests/Inputs/shtest-define/line-number-substitutions.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/lit.cfg` & `lit-18.1.3/tests/Inputs/shtest-define/lit.cfg`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/name-chars.txt` & `lit-18.1.3/tests/Inputs/shtest-define/name-chars.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/shared-substs-0.txt` & `lit-18.1.3/tests/Inputs/shtest-define/shared-substs-0.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/shared-substs-1.txt` & `lit-18.1.3/tests/Inputs/shtest-define/shared-substs-1.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/value-equals.txt` & `lit-18.1.3/tests/Inputs/shtest-define/value-equals.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/value-escaped.txt` & `lit-18.1.3/tests/Inputs/shtest-define/value-escaped.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-define/ws-and-continuations.txt` & `lit-18.1.3/tests/Inputs/shtest-define/ws-and-continuations.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-env/env-calls-env.txt` & `lit-18.1.3/tests/Inputs/shtest-env/env-calls-env.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-env/env-u.txt` & `lit-18.1.3/tests/Inputs/shtest-env/env-u.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-env/mixed.txt` & `lit-18.1.3/tests/Inputs/shtest-env/mixed.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-if-else/test.txt` & `lit-18.1.3/tests/Inputs/shtest-if-else/test.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-not/not-calls-external.txt` & `lit-18.1.3/tests/Inputs/shtest-not/not-calls-external.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-shell/check_path.py` & `lit-18.1.3/tests/Inputs/shtest-shell/check_path.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-shell/dev-null.txt` & `lit-18.1.3/tests/Inputs/shtest-shell/dev-null.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-shell/diff-encodings.txt` & `lit-18.1.3/tests/Inputs/shtest-shell/diff-encodings.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-shell/diff-pipes.txt` & `lit-18.1.3/tests/Inputs/shtest-shell/diff-pipes.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-shell/diff-r.txt` & `lit-18.1.3/tests/Inputs/shtest-shell/diff-r.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-shell/diff-unified.txt` & `lit-18.1.3/tests/Inputs/shtest-shell/diff-unified.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-shell/redirects.txt` & `lit-18.1.3/tests/Inputs/shtest-shell/redirects.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-shell/sequencing-0.txt` & `lit-18.1.3/tests/Inputs/shtest-shell/sequencing-0.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-shell/valid-shell.txt` & `lit-18.1.3/tests/Inputs/shtest-shell/valid-shell.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/shtest-timeout/lit.cfg` & `lit-18.1.3/tests/Inputs/shtest-timeout/lit.cfg`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/test-data/dummy_format.py` & `lit-18.1.3/tests/Inputs/test-data/dummy_format.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/test-data-micro/dummy_format.py` & `lit-18.1.3/tests/Inputs/test-data-micro/dummy_format.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/test_retry_attempts/test.py` & `lit-18.1.3/tests/Inputs/test_retry_attempts/test.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/testrunner-custom-parsers/test.txt` & `lit-18.1.3/tests/Inputs/testrunner-custom-parsers/test.txt`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/use-llvm-tool/lit.cfg` & `lit-18.1.3/tests/Inputs/use-llvm-tool/lit.cfg`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/Inputs/xunit-output/dummy_format.py` & `lit-18.1.3/tests/Inputs/xunit-output/dummy_format.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/allow-retries.py` & `lit-18.1.3/tests/allow-retries.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/discovery.py` & `lit-18.1.3/tests/discovery.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/googletest-crash.py` & `lit-18.1.3/tests/googletest-crash.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/googletest-format-respect-gtest-sharding-env-vars.py` & `lit-18.1.3/tests/googletest-format-respect-gtest-sharding-env-vars.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/googletest-format.py` & `lit-18.1.3/tests/googletest-format.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/googletest-no-sharding.py` & `lit-18.1.3/tests/googletest-no-sharding.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/googletest-sanitizer-error.py` & `lit-18.1.3/tests/googletest-sanitizer-error.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/googletest-timeout.py` & `lit-18.1.3/tests/googletest-timeout.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/ignore-fail.py` & `lit-18.1.3/tests/ignore-fail.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/lit-opts.py` & `lit-18.1.3/tests/lit-opts.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/lit.cfg` & `lit-18.1.3/tests/lit.cfg`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/max-failures.py` & `lit-18.1.3/tests/max-failures.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/parallelism-groups.py` & `lit-18.1.3/tests/parallelism-groups.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/per-test-coverage-by-lit-cfg.py` & `lit-18.1.3/tests/per-test-coverage-by-lit-cfg.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/per-test-coverage.py` & `lit-18.1.3/tests/per-test-coverage.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/progress-bar.py` & `lit-18.1.3/tests/progress-bar.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/reorder.py` & `lit-18.1.3/tests/reorder.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/selecting.py` & `lit-18.1.3/tests/selecting.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/show-result-codes.py` & `lit-18.1.3/tests/show-result-codes.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/show-used-features.py` & `lit-18.1.3/tests/show-used-features.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-define.py` & `lit-18.1.3/tests/shtest-define.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-env.py` & `lit-18.1.3/tests/shtest-env.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-external-shell-kill.py` & `lit-18.1.3/tests/shtest-external-shell-kill.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-format-argv0.py` & `lit-18.1.3/tests/shtest-format-argv0.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-format.py` & `lit-18.1.3/tests/shtest-format.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-if-else.py` & `lit-18.1.3/tests/shtest-if-else.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-inject.py` & `lit-18.1.3/tests/shtest-inject.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-keyword-parse-errors.py` & `lit-18.1.3/tests/shtest-keyword-parse-errors.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-not.py` & `lit-18.1.3/tests/shtest-not.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-output-printing.py` & `lit-18.1.3/tests/shtest-output-printing.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-pushd-popd.py` & `lit-18.1.3/tests/shtest-pushd-popd.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-recursive-substitution.py` & `lit-18.1.3/tests/shtest-recursive-substitution.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-run-at-line.py` & `lit-18.1.3/tests/shtest-run-at-line.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-shell.py` & `lit-18.1.3/tests/shtest-shell.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/shtest-timeout.py` & `lit-18.1.3/tests/shtest-timeout.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/test-data-micro.py` & `lit-18.1.3/tests/test-data-micro.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/test-output-micro-resultdb.py` & `lit-18.1.3/tests/test-output-micro-resultdb.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/test-output-micro.py` & `lit-18.1.3/tests/test-output-micro.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/test-output-resultdb.py` & `lit-18.1.3/tests/test-output-resultdb.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/test-output.py` & `lit-18.1.3/tests/test-output.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/unit/ShUtil.py` & `lit-18.1.3/tests/unit/ShUtil.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/unit/TestRunner.py` & `lit-18.1.3/tests/unit/TestRunner.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/unparsed-requirements.py` & `lit-18.1.3/tests/unparsed-requirements.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/use-llvm-tool.py` & `lit-18.1.3/tests/use-llvm-tool.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/xfail-cl.py` & `lit-18.1.3/tests/xfail-cl.py`

 * *Files identical despite different names*

### Comparing `lit-18.1.2/tests/xunit-output.py` & `lit-18.1.3/tests/xunit-output.py`

 * *Files identical despite different names*

