# Comparing `tmp/intecomm-rando-0.1.8.tar.gz` & `tmp/intecomm-rando-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intecomm-rando-0.1.8.tar", last modified: Fri May 12 04:22:54 2023, max compression
+gzip compressed data, was "intecomm-rando-0.1.9.tar", last modified: Mon Jul 10 16:16:08 2023, max compression
```

## Comparing `intecomm-rando-0.1.8.tar` & `intecomm-rando-0.1.9.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.860658 intecomm-rando-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       64 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.850397 intecomm-rando-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.854064 intecomm-rando-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-04-22 18:11:43.000000 intecomm-rando-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-18 00:53:59.000000 intecomm-rando-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-05-12 04:22:54.860742 intecomm-rando-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      825 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.855952 intecomm-rando-0.1.8/intecomm_rando/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:17:21.000000 intecomm-rando-0.1.8/intecomm_rando/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/intecomm_rando/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)       72 2023-01-25 03:01:52.000000 intecomm-rando-0.1.8/intecomm_rando/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      103 2022-11-23 01:14:40.000000 intecomm-rando-0.1.8/intecomm_rando/exceptions.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2749 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/intecomm_rando/group_eligibility.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1116 2022-11-20 02:31:32.000000 intecomm-rando-0.1.8/intecomm_rando/group_identifier.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.857303 intecomm-rando-0.1.8/intecomm_rando/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    24521 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/intecomm_rando/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3304 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:31:32.000000 intecomm-rando-0.1.8/intecomm_rando/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.857969 intecomm-rando-0.1.8/intecomm_rando/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      154 2023-05-03 01:50:00.000000 intecomm-rando-0.1.8/intecomm_rando/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      524 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/intecomm_rando/models/randomization_list.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1849 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/intecomm_rando/models/registered_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3153 2023-05-12 04:22:47.000000 intecomm-rando-0.1.8/intecomm_rando/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4962 2023-05-04 03:04:38.000000 intecomm-rando-0.1.8/intecomm_rando/randomize_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1328 2023-05-12 04:22:47.000000 intecomm-rando-0.1.8/intecomm_rando/randomizers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.858356 intecomm-rando-0.1.8/intecomm_rando/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:16:20.000000 intecomm-rando-0.1.8/intecomm_rando/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.860145 intecomm-rando-0.1.8/intecomm_rando/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      391 2023-01-25 03:01:52.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/randomization_list.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      303 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/intecomm_rando/tests/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      294 2022-11-20 02:31:32.000000 intecomm-rando-0.1.8/intecomm_rando/tests/sites.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.860404 intecomm-rando-0.1.8/intecomm_rando/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-23 01:14:40.000000 intecomm-rando-0.1.8/intecomm_rando/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12293 2023-05-04 03:04:20.000000 intecomm-rando-0.1.8/intecomm_rando/tests/tests/test_rando_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/intecomm_rando/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.856801 intecomm-rando-0.1.8/intecomm_rando.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-05-12 04:22:54.000000 intecomm-rando-0.1.8/intecomm_rando.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1605 2023-05-12 04:22:54.000000 intecomm-rando-0.1.8/intecomm_rando.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-12 04:22:54.000000 intecomm-rando-0.1.8/intecomm_rando.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-18 01:20:40.000000 intecomm-rando-0.1.8/intecomm_rando.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       15 2023-05-12 04:22:54.000000 intecomm-rando-0.1.8/intecomm_rando.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1753 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1711 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1159 2023-05-12 04:22:54.861053 intecomm-rando-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:16:08.595657 intecomm-rando-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       64 2022-11-18 01:20:32.000000 intecomm-rando-0.1.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-18 01:20:32.000000 intecomm-rando-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:16:08.584954 intecomm-rando-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:16:08.588264 intecomm-rando-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1737 2023-07-10 16:16:01.000000 intecomm-rando-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-11-20 14:10:06.000000 intecomm-rando-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-07-10 16:16:01.000000 intecomm-rando-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-18 01:20:32.000000 intecomm-rando-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-11-18 01:20:32.000000 intecomm-rando-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-18 01:20:32.000000 intecomm-rando-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-18 00:53:59.000000 intecomm-rando-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-18 01:20:32.000000 intecomm-rando-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-07-10 16:16:08.595748 intecomm-rando-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      825 2022-11-18 01:20:32.000000 intecomm-rando-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-18 01:20:32.000000 intecomm-rando-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:16:08.590116 intecomm-rando-0.1.9/intecomm_rando/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:17:21.000000 intecomm-rando-0.1.9/intecomm_rando/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-11-18 01:20:32.000000 intecomm-rando-0.1.9/intecomm_rando/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       72 2023-01-25 03:01:52.000000 intecomm-rando-0.1.9/intecomm_rando/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      103 2022-11-23 01:14:40.000000 intecomm-rando-0.1.9/intecomm_rando/exceptions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2749 2023-03-31 00:48:41.000000 intecomm-rando-0.1.9/intecomm_rando/group_eligibility.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1116 2022-11-20 02:31:32.000000 intecomm-rando-0.1.9/intecomm_rando/group_identifier.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:16:08.592057 intecomm-rando-0.1.9/intecomm_rando/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    24521 2023-03-31 00:48:41.000000 intecomm-rando-0.1.9/intecomm_rando/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3304 2023-03-31 00:48:41.000000 intecomm-rando-0.1.9/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1509 2023-07-10 16:16:01.000000 intecomm-rando-0.1.9/intecomm_rando/migrations/0003_alter_randomizationlist_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:31:32.000000 intecomm-rando-0.1.9/intecomm_rando/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:16:08.592982 intecomm-rando-0.1.9/intecomm_rando/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      154 2023-05-03 01:50:00.000000 intecomm-rando-0.1.9/intecomm_rando/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      524 2023-03-31 00:48:41.000000 intecomm-rando-0.1.9/intecomm_rando/models/randomization_list.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1849 2023-03-31 00:48:41.000000 intecomm-rando-0.1.9/intecomm_rando/models/registered_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3153 2023-05-12 04:22:47.000000 intecomm-rando-0.1.9/intecomm_rando/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4962 2023-05-04 03:04:38.000000 intecomm-rando-0.1.9/intecomm_rando/randomize_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1328 2023-05-12 04:22:47.000000 intecomm-rando-0.1.9/intecomm_rando/randomizers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:16:08.593525 intecomm-rando-0.1.9/intecomm_rando/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:16:20.000000 intecomm-rando-0.1.9/intecomm_rando/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:16:08.595190 intecomm-rando-0.1.9/intecomm_rando/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      391 2023-01-25 03:01:52.000000 intecomm-rando-0.1.9/intecomm_rando/tests/etc/randomization_list.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.9/intecomm_rando/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.9/intecomm_rando/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-20 14:10:06.000000 intecomm-rando-0.1.9/intecomm_rando/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.9/intecomm_rando/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-20 14:10:06.000000 intecomm-rando-0.1.9/intecomm_rando/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.9/intecomm_rando/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.9/intecomm_rando/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.9/intecomm_rando/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      303 2023-03-31 00:48:41.000000 intecomm-rando-0.1.9/intecomm_rando/tests/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      294 2022-11-20 02:31:32.000000 intecomm-rando-0.1.9/intecomm_rando/tests/sites.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:16:08.595411 intecomm-rando-0.1.9/intecomm_rando/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-23 01:14:40.000000 intecomm-rando-0.1.9/intecomm_rando/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12293 2023-05-04 03:04:20.000000 intecomm-rando-0.1.9/intecomm_rando/tests/tests/test_rando_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-18 01:20:32.000000 intecomm-rando-0.1.9/intecomm_rando/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:16:08.591081 intecomm-rando-0.1.9/intecomm_rando.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-07-10 16:16:08.000000 intecomm-rando-0.1.9/intecomm_rando.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1680 2023-07-10 16:16:08.000000 intecomm-rando-0.1.9/intecomm_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-10 16:16:08.000000 intecomm-rando-0.1.9/intecomm_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-18 01:20:40.000000 intecomm-rando-0.1.9/intecomm_rando.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       15 2023-07-10 16:16:08.000000 intecomm-rando-0.1.9/intecomm_rando.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1783 2023-07-10 16:16:01.000000 intecomm-rando-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1711 2023-03-31 00:48:41.000000 intecomm-rando-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1159 2023-07-10 16:16:08.596089 intecomm-rando-0.1.9/setup.cfg
```

### Comparing `intecomm-rando-0.1.8/.github/workflows/build.yml` & `intecomm-rando-0.1.9/.github/workflows/build.yml`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,18 @@
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.10', '3.11']
-        django-version: ['4.1', 'dev']
-
+        django-version: ['4.1', '4.2', 'dev']
+        exclude:
+          - python-version: '3.10'
+            django-version: 'dev'
     steps:
       - name: Install pycups and words dependency
         run: |
           sudo sed -i 's/azure\.//' /etc/apt/sources.list
           sudo apt-get -y update
           sudo apt-get install libcups2-dev wamerican
```

### Comparing `intecomm-rando-0.1.8/.gitignore` & `intecomm-rando-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/.pre-commit-config.yaml` & `intecomm-rando-0.1.9/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -43,12 +43,12 @@
 
   - repo: https://github.com/rstcheck/rstcheck
     rev: v6.1.2
     hooks:
       - id: rstcheck
 
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.30.0
+    rev: v1.32.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `intecomm-rando-0.1.8/LICENSE` & `intecomm-rando-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/PKG-INFO` & `intecomm-rando-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-rando
-Version: 0.1.8
+Version: 0.1.9
 Summary: INTECOMM EDC randomization
 Home-page: https://github.com/intecomm-trial/intecomm-rando
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC randomization,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-rando-0.1.8/README.rst` & `intecomm-rando-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/intecomm_rando/group_eligibility.py` & `intecomm-rando-0.1.9/intecomm_rando/group_eligibility.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/intecomm_rando/group_identifier.py` & `intecomm-rando-0.1.9/intecomm_rando/group_identifier.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/intecomm_rando/migrations/0001_initial.py` & `intecomm-rando-0.1.9/intecomm_rando/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py` & `intecomm-rando-0.1.9/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/intecomm_rando/models/randomization_list.py` & `intecomm-rando-0.1.9/intecomm_rando/models/randomization_list.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/intecomm_rando/models/registered_group.py` & `intecomm-rando-0.1.9/intecomm_rando/models/registered_group.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/intecomm_rando/models/signals.py` & `intecomm-rando-0.1.9/intecomm_rando/models/signals.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/intecomm_rando/randomize_group.py` & `intecomm-rando-0.1.9/intecomm_rando/randomize_group.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/intecomm_rando/randomizers.py` & `intecomm-rando-0.1.9/intecomm_rando/randomizers.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-rsa-local-private.pem` & `intecomm-rando-0.1.9/intecomm_rando/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-rsa-restricted-private.pem` & `intecomm-rando-0.1.9/intecomm_rando/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/intecomm_rando/tests/tests/test_rando_group.py` & `intecomm-rando-0.1.9/intecomm_rando/tests/tests/test_rando_group.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/intecomm_rando.egg-info/PKG-INFO` & `intecomm-rando-0.1.9/intecomm_rando.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-rando
-Version: 0.1.8
+Version: 0.1.9
 Summary: INTECOMM EDC randomization
 Home-page: https://github.com/intecomm-trial/intecomm-rando
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC randomization,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-rando-0.1.8/intecomm_rando.egg-info/SOURCES.txt` & `intecomm-rando-0.1.9/intecomm_rando.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 intecomm_rando.egg-info/PKG-INFO
 intecomm_rando.egg-info/SOURCES.txt
 intecomm_rando.egg-info/dependency_links.txt
 intecomm_rando.egg-info/not-zip-safe
 intecomm_rando.egg-info/top_level.txt
 intecomm_rando/migrations/0001_initial.py
 intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py
+intecomm_rando/migrations/0003_alter_randomizationlist_options_and_more.py
 intecomm_rando/migrations/__init__.py
 intecomm_rando/models/__init__.py
 intecomm_rando/models/randomization_list.py
 intecomm_rando/models/registered_group.py
 intecomm_rando/models/signals.py
 intecomm_rando/tests/__init__.py
 intecomm_rando/tests/models.py
```

### Comparing `intecomm-rando-0.1.8/pyproject.toml` & `intecomm-rando-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,37 +32,38 @@
   "if TYPE_CHECKING:",
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{310,311}-dj{41,dev},
+    py{310,311}-dj{41,42,dev},
     lint
 
 isolated_build = true
 
 [gh-actions]
 python =
     3.10: py310
     3.11: py311, lint
 
 [gh-actions:env]
 DJANGO =
-    4.0: dj40
-    4.1: dj41, lint
+    4.1: dj41
+    4.2: dj42, lint
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
     dj41: Django>=4.1,<4.2
+    dj42: Django>=4.2,<5.0
     djdev: https://github.com/django/django/tarball/main
 
 commands =
     pip install -U pip
     pip --version
     pip install -U intecomm_form_validators
     pip freeze
```

### Comparing `intecomm-rando-0.1.8/runtests.py` & `intecomm-rando-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.8/setup.cfg` & `intecomm-rando-0.1.9/setup.cfg`

 * *Files identical despite different names*

