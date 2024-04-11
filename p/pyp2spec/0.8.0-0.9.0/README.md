# Comparing `tmp/pyp2spec-0.8.0.tar.gz` & `tmp/pyp2spec-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyp2spec-0.8.0.tar", last modified: Wed Oct 11 11:46:59 2023, max compression
+gzip compressed data, was "pyp2spec-0.9.0.tar", last modified: Thu Apr 11 13:56:58 2024, max compression
```

## Comparing `pyp2spec-0.8.0.tar` & `pyp2spec-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-10-11 11:46:59.661657 pyp2spec-0.8.0/
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1103 2022-12-02 12:41:04.000000 pyp2spec-0.8.0/LICENSE-MIT
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      954 2022-12-02 12:41:04.000000 pyp2spec-0.8.0/LICENSE-MIT-0
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)       64 2023-05-03 08:15:20.000000 pyp2spec-0.8.0/MANIFEST.in
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6780 2023-10-11 11:46:59.661657 pyp2spec-0.8.0/PKG-INFO
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     5652 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/README.md
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-10-11 11:46:59.657657 pyp2spec-0.8.0/pyp2spec/
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)        0 2022-12-02 12:41:04.000000 pyp2spec-0.8.0/pyp2spec/__init__.py
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     5862 2023-04-25 08:18:22.000000 pyp2spec-0.8.0/pyp2spec/classifiers_to_fedora.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6102 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/pyp2spec/conf2spec.py
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6903 2023-10-05 11:30:17.000000 pyp2spec-0.8.0/pyp2spec/license_processor.py
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    18192 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/pyp2spec/pyp2conf.py
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      784 2023-09-01 09:28:30.000000 pyp2spec-0.8.0/pyp2spec/pyp2spec.py
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     2604 2023-02-09 12:00:51.000000 pyp2spec-0.8.0/pyp2spec/rpmversion.py
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1955 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/pyp2spec/template.spec
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)       89 2023-10-04 11:36:17.000000 pyp2spec-0.8.0/pyp2spec/utils.py
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-10-11 11:46:59.657657 pyp2spec-0.8.0/pyp2spec.egg-info/
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6780 2023-10-11 11:46:59.000000 pyp2spec-0.8.0/pyp2spec.egg-info/PKG-INFO
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1751 2023-10-11 11:46:59.000000 pyp2spec-0.8.0/pyp2spec.egg-info/SOURCES.txt
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)        1 2023-10-11 11:46:59.000000 pyp2spec-0.8.0/pyp2spec.egg-info/dependency_links.txt
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      122 2023-10-11 11:46:59.000000 pyp2spec-0.8.0/pyp2spec.egg-info/entry_points.txt
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      135 2023-10-11 11:46:59.000000 pyp2spec-0.8.0/pyp2spec.egg-info/requires.txt
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)        9 2023-10-11 11:46:59.000000 pyp2spec-0.8.0/pyp2spec.egg-info/top_level.txt
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)       89 2022-12-02 12:41:04.000000 pyp2spec-0.8.0/pyproject.toml
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1244 2023-10-11 11:46:59.661657 pyp2spec-0.8.0/setup.cfg
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-10-11 11:46:59.658657 pyp2spec-0.8.0/tests/
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      608 2023-10-10 12:25:32.000000 pyp2spec-0.8.0/tests/conftest.py
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-10-11 11:46:59.658657 pyp2spec-0.8.0/tests/expected_specfiles/
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1233 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/tests/expected_specfiles/python-click.spec
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1626 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/tests/expected_specfiles/python-markdown-it-py.spec
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1223 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/tests/expected_specfiles/python-numpy.spec
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1536 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/tests/expected_specfiles/python-sphinx.spec
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     8236 2023-04-25 08:18:22.000000 pyp2spec-0.8.0/tests/fedora_license_data.json
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-10-11 11:46:59.655657 pyp2spec-0.8.0/tests/fixtures/
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-10-11 11:46:59.659657 pyp2spec-0.8.0/tests/fixtures/cassettes/
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    12682 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/tests/fixtures/cassettes/test_pyp2conf.test_archful_package.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     7419 2023-10-10 12:20:29.000000 pyp2spec-0.8.0/tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[aionotion-2.0.3].json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6449 2023-10-10 12:20:29.000000 pyp2spec-0.8.0/tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[click-7.1.2].json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)   542126 2023-10-10 12:20:29.000000 pyp2spec-0.8.0/tests/fixtures/cassettes/test_pyp2conf.test_config_with_customization_is_valid.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     2869 2023-04-26 08:33:53.000000 pyp2spec-0.8.0/tests/fixtures/cassettes/test_pyp2conf.test_non_existent_package.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)   107244 2023-10-10 14:22:07.000000 pyp2spec-0.8.0/tests/fixtures/cassettes/test_pyp2conf.test_package_with_extras.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     4490 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/tests/test_conf2spec.py
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-10-11 11:46:59.660657 pyp2spec-0.8.0/tests/test_configs/
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      415 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/tests/test_configs/customized_aionotion.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      624 2023-04-26 08:33:53.000000 pyp2spec-0.8.0/tests/test_configs/customized_boutdata.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      690 2023-10-10 14:22:07.000000 pyp2spec-0.8.0/tests/test_configs/customized_click.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      731 2023-10-10 14:22:07.000000 pyp2spec-0.8.0/tests/test_configs/customized_jupyter-packaging.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      798 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/tests/test_configs/customized_markdown-it-py.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      385 2023-10-10 14:22:07.000000 pyp2spec-0.8.0/tests/test_configs/customized_python-sphinx.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      474 2023-04-26 08:33:53.000000 pyp2spec-0.8.0/tests/test_configs/customized_tornado.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      400 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/tests/test_configs/default_python-aionotion.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      379 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/tests/test_configs/default_python-click.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      360 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/tests/test_configs/default_python-numpy.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     4130 2023-09-01 09:28:30.000000 pyp2spec-0.8.0/tests/test_license_processor.py
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    12495 2023-10-11 08:49:48.000000 pyp2spec-0.8.0/tests/test_pyp2conf.py
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2024-04-11 13:56:58.190776 pyp2spec-0.9.0/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1103 2022-12-02 12:41:04.000000 pyp2spec-0.9.0/LICENSE-MIT
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      954 2022-12-02 12:41:04.000000 pyp2spec-0.9.0/LICENSE-MIT-0
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)       64 2023-05-03 08:15:20.000000 pyp2spec-0.9.0/MANIFEST.in
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     7058 2024-04-11 13:56:58.190776 pyp2spec-0.9.0/PKG-INFO
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     5828 2024-04-11 10:40:19.000000 pyp2spec-0.9.0/README.md
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2024-04-11 13:56:58.185776 pyp2spec-0.9.0/pyp2spec/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)        0 2022-12-02 12:41:04.000000 pyp2spec-0.9.0/pyp2spec/__init__.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     5862 2023-04-25 08:18:22.000000 pyp2spec-0.9.0/pyp2spec/classifiers_to_fedora.json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6357 2024-04-11 10:40:19.000000 pyp2spec-0.9.0/pyp2spec/conf2spec.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6903 2023-10-05 11:30:17.000000 pyp2spec-0.9.0/pyp2spec/license_processor.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)    19327 2024-04-11 10:40:19.000000 pyp2spec-0.9.0/pyp2spec/pyp2conf.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      784 2024-04-11 10:18:04.000000 pyp2spec-0.9.0/pyp2spec/pyp2spec.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     2604 2023-02-09 12:00:51.000000 pyp2spec-0.9.0/pyp2spec/rpmversion.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     2202 2024-04-11 10:40:19.000000 pyp2spec-0.9.0/pyp2spec/template.spec
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)       89 2023-10-04 11:36:17.000000 pyp2spec-0.9.0/pyp2spec/utils.py
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2024-04-11 13:56:58.190776 pyp2spec-0.9.0/pyp2spec.egg-info/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     7058 2024-04-11 13:56:58.000000 pyp2spec-0.9.0/pyp2spec.egg-info/PKG-INFO
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1967 2024-04-11 13:56:58.000000 pyp2spec-0.9.0/pyp2spec.egg-info/SOURCES.txt
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)        1 2024-04-11 13:56:58.000000 pyp2spec-0.9.0/pyp2spec.egg-info/dependency_links.txt
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      122 2024-04-11 13:56:58.000000 pyp2spec-0.9.0/pyp2spec.egg-info/entry_points.txt
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      135 2024-04-11 13:56:58.000000 pyp2spec-0.9.0/pyp2spec.egg-info/requires.txt
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)        9 2024-04-11 13:56:58.000000 pyp2spec-0.9.0/pyp2spec.egg-info/top_level.txt
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)       89 2022-12-02 12:41:04.000000 pyp2spec-0.9.0/pyproject.toml
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1324 2024-04-11 13:56:58.190776 pyp2spec-0.9.0/setup.cfg
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2024-04-11 13:56:58.187776 pyp2spec-0.9.0/tests/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      608 2024-04-05 10:59:20.000000 pyp2spec-0.9.0/tests/conftest.py
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2024-04-11 13:56:58.187776 pyp2spec-0.9.0/tests/expected_specfiles/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1233 2024-04-11 09:38:34.000000 pyp2spec-0.9.0/tests/expected_specfiles/python-click.spec
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1626 2024-04-11 09:38:34.000000 pyp2spec-0.9.0/tests/expected_specfiles/python-markdown-it-py.spec
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1223 2024-04-11 09:38:34.000000 pyp2spec-0.9.0/tests/expected_specfiles/python-numpy.spec
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1536 2024-04-11 09:38:34.000000 pyp2spec-0.9.0/tests/expected_specfiles/python-sphinx.spec
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1514 2024-04-11 10:40:19.000000 pyp2spec-0.9.0/tests/expected_specfiles/python3.9-pello.spec
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     8236 2023-04-25 08:18:22.000000 pyp2spec-0.9.0/tests/fedora_license_data.json
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2024-04-11 13:56:58.183776 pyp2spec-0.9.0/tests/fixtures/
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2024-04-11 13:56:58.188776 pyp2spec-0.9.0/tests/fixtures/cassettes/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)    12682 2023-10-12 08:41:00.000000 pyp2spec-0.9.0/tests/fixtures/cassettes/test_pyp2conf.test_archful_package.json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     7419 2023-10-12 08:41:00.000000 pyp2spec-0.9.0/tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[aionotion-2.0.3].json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6449 2023-10-12 08:41:00.000000 pyp2spec-0.9.0/tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[click-7.1.2].json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6362 2024-04-11 10:40:19.000000 pyp2spec-0.9.0/tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_with_alt_python_is_valid[Pello-1.0.4-3.9].json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)   542126 2023-10-12 08:41:00.000000 pyp2spec-0.9.0/tests/fixtures/cassettes/test_pyp2conf.test_config_with_customization_is_valid.json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     2869 2023-04-26 08:33:53.000000 pyp2spec-0.9.0/tests/fixtures/cassettes/test_pyp2conf.test_non_existent_package.json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)   107244 2023-10-12 08:41:00.000000 pyp2spec-0.9.0/tests/fixtures/cassettes/test_pyp2conf.test_package_with_extras.json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     4531 2024-04-11 10:40:19.000000 pyp2spec-0.9.0/tests/test_conf2spec.py
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2024-04-11 13:56:58.190776 pyp2spec-0.9.0/tests/test_configs/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      415 2024-04-02 08:45:44.000000 pyp2spec-0.9.0/tests/test_configs/customized_aionotion.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      624 2024-04-02 08:45:44.000000 pyp2spec-0.9.0/tests/test_configs/customized_boutdata.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      690 2024-04-02 08:45:44.000000 pyp2spec-0.9.0/tests/test_configs/customized_click.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      731 2024-04-02 08:45:44.000000 pyp2spec-0.9.0/tests/test_configs/customized_jupyter-packaging.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      798 2024-04-02 08:45:44.000000 pyp2spec-0.9.0/tests/test_configs/customized_markdown-it-py.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      385 2024-04-02 08:45:44.000000 pyp2spec-0.9.0/tests/test_configs/customized_python-sphinx.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      474 2024-04-02 08:45:44.000000 pyp2spec-0.9.0/tests/test_configs/customized_tornado.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      400 2024-04-02 08:45:41.000000 pyp2spec-0.9.0/tests/test_configs/default_python-aionotion.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      379 2023-10-12 11:34:17.000000 pyp2spec-0.9.0/tests/test_configs/default_python-click.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      360 2023-10-12 08:41:00.000000 pyp2spec-0.9.0/tests/test_configs/default_python-numpy.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      414 2024-04-11 10:40:19.000000 pyp2spec-0.9.0/tests/test_configs/default_python3.9-pello.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     4130 2023-09-01 09:28:30.000000 pyp2spec-0.9.0/tests/test_license_processor.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)    13813 2024-04-11 10:40:19.000000 pyp2spec-0.9.0/tests/test_pyp2conf.py
```

### Comparing `pyp2spec-0.8.0/LICENSE-MIT` & `pyp2spec-0.9.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/LICENSE-MIT-0` & `pyp2spec-0.9.0/LICENSE-MIT-0`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/PKG-INFO` & `pyp2spec-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pyp2spec
-Version: 0.8.0
+Version: 0.9.0
 Summary: Generate a valid Fedora specfile from Python package from PyPI
 Home-page: https://github.com/befeleme/pyp2spec/
 Author: Karolina Surma
 Author-email: ksurma@redhat.com
 License: MIT, MIT-0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE-MIT
@@ -108,25 +110,26 @@
 ### Mandatory fields
 
 - Generated by pyp2conf
 
 | Field  | Description | Type |
 | -------- | -------- | -------- |
 | pypi_name | package name as stored in PyPI  | string   |
-| python_name | pypi_name prepended with `python-` | string |
+| python_name | pypi_name prepended with `python-` and alternative Python version, if `python_alt_version` is defined| string |
 | archive_name | source tarball name, stripped of version and file extension  | string |
 | version | package version to create spec file for (RPM format) | string |
 | pypi_version | package version string as in PyPI, '%{version}' if the same as version | string
 | summary | short package summary | string |
 | license | license name | string |
 | url | project URL | string |
 | source | %{pypi_source} macro with optional arguments (tarball URL can be used instead) | string |
 | description | long package description | multiline string |
 | extras | extra subpackages names | list of strings |
-| archful | package contains compiled extensions, implies not using `BuildArch: noarch` and adding `BuildRequires: gcc` | bool
+| archful | package contains compiled extensions, implies not using `BuildArch: noarch` and adding `BuildRequires: gcc` | bool |
+| python_alt_version | specific Python version to create the spec file for, e.g. 3.9, 3.10, 3.12 | string |
 
 
 ### Optional fields
 
 - Not generated by pyp2conf
 - Can be also added to config files generated by pyp2conf
```

### Comparing `pyp2spec-0.8.0/README.md` & `pyp2spec-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,25 +76,26 @@
 ### Mandatory fields
 
 - Generated by pyp2conf
 
 | Field  | Description | Type |
 | -------- | -------- | -------- |
 | pypi_name | package name as stored in PyPI  | string   |
-| python_name | pypi_name prepended with `python-` | string |
+| python_name | pypi_name prepended with `python-` and alternative Python version, if `python_alt_version` is defined| string |
 | archive_name | source tarball name, stripped of version and file extension  | string |
 | version | package version to create spec file for (RPM format) | string |
 | pypi_version | package version string as in PyPI, '%{version}' if the same as version | string
 | summary | short package summary | string |
 | license | license name | string |
 | url | project URL | string |
 | source | %{pypi_source} macro with optional arguments (tarball URL can be used instead) | string |
 | description | long package description | multiline string |
 | extras | extra subpackages names | list of strings |
-| archful | package contains compiled extensions, implies not using `BuildArch: noarch` and adding `BuildRequires: gcc` | bool
+| archful | package contains compiled extensions, implies not using `BuildArch: noarch` and adding `BuildRequires: gcc` | bool |
+| python_alt_version | specific Python version to create the spec file for, e.g. 3.9, 3.10, 3.12 | string |
 
 
 ### Optional fields
 
 - Not generated by pyp2conf
 - Can be also added to config files generated by pyp2conf
```

### Comparing `pyp2spec-0.8.0/pyp2spec/classifiers_to_fedora.json` & `pyp2spec-0.9.0/pyp2spec/classifiers_to_fedora.json`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/pyp2spec/conf2spec.py` & `pyp2spec-0.9.0/pyp2spec/conf2spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,14 +129,19 @@
     """
     return fill(
         config.get_string("description"),
         width=79,
         break_long_words=False
     )
 
+
+def python3_pkgversion_or_3(config):
+    return "%{python3_pkgversion}" if config.get_string("python_alt_version") else "3"
+
+
 def fill_in_template(config):
     """Return template rendered with data from config file."""
 
     with (files("pyp2spec") / TEMPLATE_FILENAME).open("r", encoding="utf-8") as f:
         spec_template = Template(f.read())
 
     result = spec_template.render(
@@ -148,18 +153,20 @@
         doc_files=" ".join(config.get_list("doc_files")),
         extras=",".join(config.get_list("extras")),
         license_files=" ".join(config.get_list("license_files")),
         license=config.get_string("license"),
         name=config.get_string("pypi_name"),
         python_name=config.get_string("python_name"),
         pypi_version=config.get_string("pypi_version"),
+        python_alt_version=config.get_string("python_alt_version"),
         source=config.get_string("source"),
         summary=config.get_string("summary"),
         test_method=generate_check(config),
         test_top_level=config.get_bool("test_top_level"),
+        python3_pkgversion=python3_pkgversion_or_3(config),
         url=config.get_string("url"),
         version=config.get_string("version"),
     )
 
     return result
```

### Comparing `pyp2spec-0.8.0/pyp2spec/license_processor.py` & `pyp2spec-0.9.0/pyp2spec/license_processor.py`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/pyp2spec/pyp2conf.py` & `pyp2spec-0.9.0/pyp2spec/pyp2conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,19 +83,38 @@
         return package_metadata["info"]["version"]
 
     def _get_package_version_metadata(self):
         pkg_index = f"https://pypi.org/pypi/{self.package_name}/{self.version}/json"
         error_str = f"Package `{self.package_name}` or version `{self.version}` was not found on PyPI"
         return self._get_from_url(pkg_index, error_str)
 
-    def python_name(self):
+    def python_name(self, *, python_alt_version=None):
+        """Create a component name for the specfile.
+
+        Prepend the name with 'python' (unless it already starts with it).
+        Add the Python alternative version, if it's defined.
+
+        Valid outcomes:
+        package name: foo, python_alt_version: 3.11
+        -> python3.11-foo
+
+        package name: foo, python_alt_version: None
+        -> python-foo
+
+        package name: python-foo, python_alt_version: 3.12
+        -> python3.12-foo
+
+        package name: python-foo, python_alt_version: None
+        -> python-foo
+        """
+
+        alt_version = "" if python_alt_version is None else python_alt_version
         if self.pypi_name.startswith("python"):
-            return self.pypi_name
-        else:
-            return f"python-{self.pypi_name}"
+            return self.pypi_name.replace("python", f"python{alt_version}")
+        return f"python{alt_version}-{self.pypi_name}"
 
     def source(self):
         """Return valid pypi_source RPM macro.
 
         %pypi_source takes three optional arguments:
         <name>, <version> and <file_extension>.
         <name> is always passed, it's spelled as the name of the archive file:
@@ -331,14 +350,15 @@
     description=None,
     version=None,
     summary=None,
     session=None,
     license=None,
     compliant=False,
     top_level=False,
+    python_alt_version=None,
 ):
     """Use `package` and provided kwargs to create the whole config contents.
     Return contents dictionary.
     """
     contents = {}
 
     # a package name was given as the `package`, look for it on PyPI
@@ -368,22 +388,26 @@
     if top_level:
         click.secho("Only top-level modules will be checked", fg="yellow")
         contents["test_top_level"] = True
 
     if archful := pkg.is_archful():
         click.secho("Package is archful - you may need to specify additional build requirements", fg="magenta")
 
+    if python_alt_version is not None:
+        click.secho(f"Assuming build for Python: {python_alt_version}", fg="yellow")
+        contents["python_alt_version"] = python_alt_version
+
     contents["archful"] = archful
     contents["description"] = description
     contents["summary"] = summary
     contents["version"] = convert_version_to_rpm_scheme(pkg.version)
     contents["pypi_version"] = pkg.pypi_version_or_macro()
     contents["license"] = license
     contents["pypi_name"] = pkg.pypi_name
-    contents["python_name"] = pkg.python_name()
+    contents["python_name"] = pkg.python_name(python_alt_version=python_alt_version)
     contents["url"] = pkg.project_url()
     contents["source"] = pkg.source()
     contents["archive_name"] = pkg.archive_name()
     contents["extras"] = pkg.extras()
 
     return contents
 
@@ -410,14 +434,15 @@
         options["package"],
         description=options["description"],
         version=options["version"],
         summary=options["summary"],
         license=options["license"],
         compliant=options["fedora_compliant"],
         top_level=options["top_level"],
+        python_alt_version=options["python_alt_version"]
     )
     return save_config(contents, options["config_output"])
 
 
 def pypconf_args(func):
     @click.argument("package")
     @click.option(
@@ -444,14 +469,18 @@
         "--fedora-compliant", is_flag=True,
         help="Check whether license is compliant with Fedora",
     )
     @click.option(
         "--top-level", "-t", is_flag=True,
         help="Test only top-level modules in %check",
     )
+    @click.option(
+        "--python-alt-version", "-p",
+        help="Provide specific Python version to build for, e.g 3.11",
+    )
     @wraps(func)
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs)
     return wrapper
 
 @click.command()
 @pypconf_args
```

### Comparing `pyp2spec-0.8.0/pyp2spec/pyp2spec.py` & `pyp2spec-0.9.0/pyp2spec/pyp2spec.py`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/pyp2spec/rpmversion.py` & `pyp2spec-0.9.0/pyp2spec/rpmversion.py`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/pyp2spec/template.spec` & `pyp2spec-0.9.0/pyp2spec/template.spec`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,46 @@
+{% if python_alt_version -%}
+%global python3_pkgversion {{ python_alt_version }}
+
+{% endif -%}
 Name:           {{python_name}}
 Version:        {{version}}
 Release:        %autorelease
 Summary:        {{summary}}
 
 # Check if the automatically generated License and its spelling is correct for Fedora
 # https://docs.fedoraproject.org/en-US/packaging-guidelines/LicensingGuidelines/
 License:        {{license}}
 URL:            {{url}}
 Source:         {{source}}
 {% if not archful %}
 BuildArch:      noarch
 {%- endif %}
-BuildRequires:  python3-devel
+BuildRequires:  python{{python3_pkgversion}}-devel
 {% for br in additional_build_requires -%}
 BuildRequires:  {{br}}
 {% endfor %}
 
 # Fill in the actual package description to submit package to Fedora
 %global _description %{expand:
 {{description}}}
 
 %description %_description
 
-%package -n     python3-{{name}}
+{% if not python_alt_version -%}
+%package -n     python{{python3_pkgversion}}-{{name}}
 Summary:        %{summary}
 
-%description -n python3-{{name}} %_description
+%description -n python{{python3_pkgversion}}-{{name}} %_description
+{% endif -%}
+
 {% if extras %}
 # For official Fedora packages, review which extras should be actually packaged
 # See: https://docs.fedoraproject.org/en-US/packaging-guidelines/Python/#Extras
-%pyproject_extras_subpkg -n python3-{{name}} {{extras}}
+%pyproject_extras_subpkg -n python{{python3_pkgversion}}-{{name}} {{extras}}
 {% endif %}
 
 %prep
 %autosetup -p1 -n {{archive_name}}-{{pypi_version}}
 
 
 %generate_buildrequires
@@ -56,15 +63,15 @@
 
 %check
 %pyproject_check_import{% if test_top_level %} -t{% endif %}
 {% if test_method -%}
 {{test_method}}
 {% endif %}
 
-%files -n python3-{{name}} -f %{pyproject_files}
+%files -n python{{python3_pkgversion}}-{{name}} -f %{pyproject_files}
 {% if doc_files -%}
 %doc {{doc_files}}
 {% endif -%}
 {% if license_files -%}
 %license {{license_files}}
 {% endif -%}
 {% if binary_files -%}
```

### Comparing `pyp2spec-0.8.0/pyp2spec.egg-info/PKG-INFO` & `pyp2spec-0.9.0/pyp2spec.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pyp2spec
-Version: 0.8.0
+Version: 0.9.0
 Summary: Generate a valid Fedora specfile from Python package from PyPI
 Home-page: https://github.com/befeleme/pyp2spec/
 Author: Karolina Surma
 Author-email: ksurma@redhat.com
 License: MIT, MIT-0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE-MIT
@@ -108,25 +110,26 @@
 ### Mandatory fields
 
 - Generated by pyp2conf
 
 | Field  | Description | Type |
 | -------- | -------- | -------- |
 | pypi_name | package name as stored in PyPI  | string   |
-| python_name | pypi_name prepended with `python-` | string |
+| python_name | pypi_name prepended with `python-` and alternative Python version, if `python_alt_version` is defined| string |
 | archive_name | source tarball name, stripped of version and file extension  | string |
 | version | package version to create spec file for (RPM format) | string |
 | pypi_version | package version string as in PyPI, '%{version}' if the same as version | string
 | summary | short package summary | string |
 | license | license name | string |
 | url | project URL | string |
 | source | %{pypi_source} macro with optional arguments (tarball URL can be used instead) | string |
 | description | long package description | multiline string |
 | extras | extra subpackages names | list of strings |
-| archful | package contains compiled extensions, implies not using `BuildArch: noarch` and adding `BuildRequires: gcc` | bool
+| archful | package contains compiled extensions, implies not using `BuildArch: noarch` and adding `BuildRequires: gcc` | bool |
+| python_alt_version | specific Python version to create the spec file for, e.g. 3.9, 3.10, 3.12 | string |
 
 
 ### Optional fields
 
 - Not generated by pyp2conf
 - Can be also added to config files generated by pyp2conf
```

### Comparing `pyp2spec-0.8.0/pyp2spec.egg-info/SOURCES.txt` & `pyp2spec-0.9.0/pyp2spec.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -24,23 +24,26 @@
 tests/test_conf2spec.py
 tests/test_license_processor.py
 tests/test_pyp2conf.py
 tests/expected_specfiles/python-click.spec
 tests/expected_specfiles/python-markdown-it-py.spec
 tests/expected_specfiles/python-numpy.spec
 tests/expected_specfiles/python-sphinx.spec
+tests/expected_specfiles/python3.9-pello.spec
 tests/fixtures/cassettes/test_pyp2conf.test_archful_package.json
 tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[aionotion-2.0.3].json
 tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[click-7.1.2].json
+tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_with_alt_python_is_valid[Pello-1.0.4-3.9].json
 tests/fixtures/cassettes/test_pyp2conf.test_config_with_customization_is_valid.json
 tests/fixtures/cassettes/test_pyp2conf.test_non_existent_package.json
 tests/fixtures/cassettes/test_pyp2conf.test_package_with_extras.json
 tests/test_configs/customized_aionotion.conf
 tests/test_configs/customized_boutdata.conf
 tests/test_configs/customized_click.conf
 tests/test_configs/customized_jupyter-packaging.conf
 tests/test_configs/customized_markdown-it-py.conf
 tests/test_configs/customized_python-sphinx.conf
 tests/test_configs/customized_tornado.conf
 tests/test_configs/default_python-aionotion.conf
 tests/test_configs/default_python-click.conf
-tests/test_configs/default_python-numpy.conf
+tests/test_configs/default_python-numpy.conf
+tests/test_configs/default_python3.9-pello.conf
```

### Comparing `pyp2spec-0.8.0/setup.cfg` & `pyp2spec-0.9.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyp2spec
-version = 0.8.0
+version = 0.9.0
 author = Karolina Surma
 author_email = ksurma@redhat.com
 description = Generate a valid Fedora specfile from Python package from PyPI
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT, MIT-0
 license_files = 
@@ -12,14 +12,16 @@
 	LICENSE-MIT-0
 url = https://github.com/befeleme/pyp2spec/
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
+	Programming Language :: Python :: 3.13
 	Operating System :: POSIX :: Linux
 	License :: OSI Approved :: MIT License
 	License :: OSI Approved :: MIT No Attribution License (MIT-0)
 	Development Status :: 3 - Alpha
 
 [options]
 packages = find:
```

### Comparing `pyp2spec-0.8.0/tests/conftest.py` & `pyp2spec-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/expected_specfiles/python-click.spec` & `pyp2spec-0.9.0/tests/expected_specfiles/python-click.spec`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/expected_specfiles/python-markdown-it-py.spec` & `pyp2spec-0.9.0/tests/expected_specfiles/python-markdown-it-py.spec`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/expected_specfiles/python-numpy.spec` & `pyp2spec-0.9.0/tests/expected_specfiles/python-numpy.spec`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/expected_specfiles/python-sphinx.spec` & `pyp2spec-0.9.0/tests/expected_specfiles/python-sphinx.spec`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/fedora_license_data.json` & `pyp2spec-0.9.0/tests/fedora_license_data.json`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/fixtures/cassettes/test_pyp2conf.test_archful_package.json` & `pyp2spec-0.9.0/tests/fixtures/cassettes/test_pyp2conf.test_archful_package.json`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[aionotion-2.0.3].json` & `pyp2spec-0.9.0/tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[aionotion-2.0.3].json`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[click-7.1.2].json` & `pyp2spec-0.9.0/tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[click-7.1.2].json`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/fixtures/cassettes/test_pyp2conf.test_config_with_customization_is_valid.json` & `pyp2spec-0.9.0/tests/fixtures/cassettes/test_pyp2conf.test_config_with_customization_is_valid.json`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/fixtures/cassettes/test_pyp2conf.test_non_existent_package.json` & `pyp2spec-0.9.0/tests/fixtures/cassettes/test_pyp2conf.test_non_existent_package.json`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/fixtures/cassettes/test_pyp2conf.test_package_with_extras.json` & `pyp2spec-0.9.0/tests/fixtures/cassettes/test_pyp2conf.test_package_with_extras.json`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/test_conf2spec.py` & `pyp2spec-0.9.0/tests/test_conf2spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,16 @@
 
 
 @pytest.mark.parametrize(
     "conf", [
         "default_python-click.conf",
         "customized_markdown-it-py.conf",
         "customized_python-sphinx.conf",
-        "default_python-numpy.conf"
+        "default_python-numpy.conf",
+        "default_python3.9-pello.conf",
     ]
 )
 def test_default_generated_specfile(file_regression, config_dir, conf):
     # Run the conf2spec converter
     rendered_file = conf2spec.create_spec_file(config_dir + conf)
 
     # Compare the results
```

### Comparing `pyp2spec-0.8.0/tests/test_configs/customized_boutdata.conf` & `pyp2spec-0.9.0/tests/test_configs/customized_boutdata.conf`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/test_configs/customized_click.conf` & `pyp2spec-0.9.0/tests/test_configs/customized_click.conf`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/test_configs/customized_jupyter-packaging.conf` & `pyp2spec-0.9.0/tests/test_configs/customized_jupyter-packaging.conf`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/test_configs/customized_markdown-it-py.conf` & `pyp2spec-0.9.0/tests/test_configs/customized_markdown-it-py.conf`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/test_license_processor.py` & `pyp2spec-0.9.0/tests/test_license_processor.py`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.8.0/tests/test_pyp2conf.py` & `pyp2spec-0.9.0/tests/test_pyp2conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,36 @@
 
     with open(f"tests/test_configs/default_python-{package}.conf", "rb") as config_file:
         loaded_contents = tomllib.load(config_file)
 
     assert config == loaded_contents
 
 
+@pytest.mark.parametrize("package, version, alt_python",
+    [
+        ("Pello", "1.0.4", "3.9"),
+    ]
+)
+def test_automatically_generated_config_with_alt_python_is_valid(
+        betamax_parametrized_session, package, version, alt_python
+    ):
+    """Run the config rendering in fully automated mode and compare the results"""
+    config = create_config_contents(
+        package=package,
+        version=version,
+        python_alt_version=alt_python,
+        session=betamax_parametrized_session,
+    )
+
+    with open(f"tests/test_configs/default_python{alt_python}-{package.lower()}.conf", "rb") as config_file:
+        loaded_contents = tomllib.load(config_file)
+
+    assert config == loaded_contents
+
+
 def test_config_with_customization_is_valid(betamax_session):
     """Get the upstream metadata and modify some fields to get the custom config file.
     This also tests the compliance with Fedora Legal data by making
     a request to the remote resource.
     """
     package = "aionotion"
     config = create_config_contents(
@@ -221,14 +243,30 @@
     fake_pkg_data = {"info": {"name": "Awesome_TestPkg"}}
     pkg = PypiPackage("Awesome_TestPkg", version="1.2.3",package_metadata=fake_pkg_data)
     assert pkg.pypi_name == "awesome-testpkg"
     assert pkg.python_name() == "python-awesome-testpkg"
 
 
 @pytest.mark.parametrize(
+    ("pypi_name", "alt_version", "expected"), [
+        ("foo", "3.10", "python3.10-foo"),
+        ("python-foo", "3.9", "python3.9-foo"),
+        ("python_foo", "3.12", "python3.12-foo"),
+        ("foo", None, "python-foo"),
+        ("python-foo", None, "python-foo"),
+        ("python_foo", None, "python-foo"),
+    ]
+)
+def test_python_name(pypi_name, alt_version, expected):
+    fake_pkg_data = {"info": {"name": pypi_name}}
+    pkg = PypiPackage(pypi_name, version="1.2.3", package_metadata=fake_pkg_data)
+    assert pkg.python_name(python_alt_version=alt_version) == expected
+
+
+@pytest.mark.parametrize(
     ("pypi_version", "rpm_version"), [
         ("1.1.0", "1.1.0"),
         ("1!0.2.13", "1:0.2.13"),
         ("0.0.2-beta1", "0.0.2~b1"),
         ("0.5.40-0", "0.5.40^post0"),
     ]
 )
```

