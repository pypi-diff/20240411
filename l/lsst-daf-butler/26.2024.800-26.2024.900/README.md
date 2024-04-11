# Comparing `tmp/lsst-daf-butler-26.2024.800.tar.gz` & `tmp/lsst-daf-butler-26.2024.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-daf-butler-26.2024.800.tar", last modified: Thu Feb 22 10:52:16 2024, max compression
+gzip compressed data, was "lsst-daf-butler-26.2024.900.tar", last modified: Thu Feb 29 10:30:36 2024, max compression
```

## Comparing `lsst-daf-butler-26.2024.800.tar` & `lsst-daf-butler-26.2024.900.tar`

### file list

```diff
@@ -1,401 +1,405 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.474043 lsst-daf-butler-26.2024.800/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-02-22 10:52:16.474043 lsst-daf-butler-26.2024.800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.410043 lsst-daf-butler-26.2024.800/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.418043 lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/
--rw-r--r--   0 runner    (1001) docker     (127)    54247 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/concreteStorageClasses.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/configuring.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/datastores.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/dimensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22653 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/formatters.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/organizing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/queries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/use-in-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/writing-subcommands.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.414043 lsst-daf-butler-26.2024.800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.418043 lsst-daf-butler-26.2024.800/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.418043 lsst-daf-butler-26.2024.800/python/lsst/daf/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.426043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73722 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_butler_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_butler_instance_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_butler_repo_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_column_categorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_column_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    52100 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_config_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_dataset_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_dataset_existence.py
--rw-r--r--   0 runner    (1001) docker     (127)    32097 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_dataset_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)    30001 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_deferredDatasetHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_file_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_file_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30151 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_labeled_butler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_limited_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_location.py
--rw-r--r--   0 runner    (1001) docker     (127)    19541 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_named.py
--rw-r--r--   0 runner    (1001) docker     (127)    25574 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_quantum.py
--rw-r--r--   0 runner    (1001) docker     (127)    32289 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_quantum_backed.py
--rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    27865 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_query_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_registry_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)    37492 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    14504 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_storage_class_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)    23115 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_timespan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.426043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_utilities/locked_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_utilities/named_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_utilities/thread_safe_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/arrow_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.430043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14768 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/cliLog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.430043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/cmd/_remove_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/cmd/_remove_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.430043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/opt/optionGroups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    44064 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/column_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.430043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/datastore.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.430043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/datastores/composites.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/datastores/formatters.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15088 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/dimensions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/registry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/repo_transfer_formats.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14810 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/storageClasses.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.434043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57431 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    41721 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/composites.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    31187 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/file_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/generic_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/record_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/stored_file_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.434043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/chainedDatastore.py
--rw-r--r--   0 runner    (1001) docker     (127)   120435 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/fileDatastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/fileDatastoreClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.434043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/file_datastore/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/file_datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22032 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/file_datastore/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    27060 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/inMemoryDatastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/ddl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.434043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/delegates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/delegates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/delegates/arrowastropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/delegates/arrownumpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/delegates/arrownumpydict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/delegates/arrowtable.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/delegates/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.438043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25254 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    55439 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)    35795 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py
--rw-r--r--   0 runner    (1001) docker     (127)    15002 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    23173 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_governor.py
--rw-r--r--   0 runner    (1001) docker     (127)    22849 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    20363 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_packer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_record_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_record_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    19854 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_records.py
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_skypix.py
--rw-r--r--   0 runner    (1001) docker     (127)    24448 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_universe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/construction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/record_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    97583 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/direct_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/direct_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/direct_query_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.438043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/astropyTable.py
--rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    42219 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    18310 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/mapping_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/nonempty_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/persistence_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    19630 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10226 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/pydantic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.442043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_caching_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_collection_record_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_collection_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_collection_summary_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_collection_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_dataset_type_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    60805 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_registry_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.442043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/bridge/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (127)    16738 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/bridge/monolithic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.442043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/collections/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/collections/nameKey.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/collections/synthIntKey.py
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/connectionString.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.442043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/databases/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22479 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/databases/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/databases/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.442043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.446043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/byDimensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24029 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    40134 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py
--rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.446043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/dimensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/dimensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42986 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/dimensions/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.446043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    21076 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    79781 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    24143 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13309 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_obscore.py
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_opaque.py
--rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)    21369 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/nameShrinker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.446043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16298 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/_records.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/default_spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/pgsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/opaque.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.450043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    49430 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    33946 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_query_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_query_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    39207 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    16320 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_sql_query_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    25438 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_sql_query_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/butler_sql_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.450043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22509 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/categorize.py
--rw-r--r--   0 runner    (1001) docker     (127)    22911 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/check.py
--rw-r--r--   0 runner    (1001) docker     (127)    41024 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/normalForm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.450043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py
--rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.454043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/ply/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/ply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43384 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py
--rw-r--r--   0 runner    (1001) docker     (127)   137077 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/find_first_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)   114994 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/sql_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.454043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64443 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/tests/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)   174114 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/tests/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/versions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/wildcards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.454043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    28071 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/_remote_butler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.454043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.454043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/handlers/_external.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/repo_relocation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.458043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/_associate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/_pruneDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/butlerImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/certifyCalibrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/collectionChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/configDump.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/configValidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/createRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/exportCalibs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/ingest_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/queryCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/queryDataIds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/queryDatasetTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/queryDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/queryDimensionRecords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/register_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/removeCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/removeDatasetType.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/removeRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/retrieveArtifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/transferDatasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.462043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/_datasetsHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/_dummyRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/_examplePythonTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23754 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/_testRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)    67398 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/butler_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/cliCmdTestBase.py
--rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/cliLogTestBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/deferredFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/dict_convertible_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/hybrid_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/server_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/testFormatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24816 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/timespan_database_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.462043 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/transfers/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16954 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/transfers/_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/transfers/_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/transfers/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 10:52:16.000000 lsst-daf-butler-26.2024.800/python/lsst/daf/butler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.474043 lsst-daf-butler-26.2024.800/python/lsst_daf_butler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-02-22 10:52:16.000000 lsst-daf-butler-26.2024.800/python/lsst_daf_butler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-02-22 10:52:16.000000 lsst-daf-butler-26.2024.800/python/lsst_daf_butler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:52:16.000000 lsst-daf-butler-26.2024.800/python/lsst_daf_butler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-22 10:52:16.000000 lsst-daf-butler-26.2024.800/python/lsst_daf_butler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-22 10:52:16.000000 lsst-daf-butler-26.2024.800/python/lsst_daf_butler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 10:52:16.000000 lsst-daf-butler-26.2024.800/python/lsst_daf_butler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:52:15.000000 lsst-daf-butler-26.2024.800/python/lsst_daf_butler.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-22 10:52:16.474043 lsst-daf-butler-26.2024.800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:52:16.474043 lsst-daf-butler-26.2024.800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_astropyTableFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)   116274 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_butler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_butler_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdAssociate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdConfigDump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdConfigValidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdCreate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdIngestFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdPruneDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12885 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdQueryCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdQueryDataIds.py
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdQueryDatasetTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdQueryDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdQueryDimensionRecords.py
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdRemoveCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdRemoveRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliCmdRetrieveArtifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliLog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliPluginLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliUtilSplitCommas.py
--rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliUtilSplitKv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliUtilToUpper.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_cliUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_composites.py
--rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_connectionString.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    29972 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    82916 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_ddl.py
--rw-r--r--   0 runner    (1001) docker     (127)    17831 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_dimension_record_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    45092 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_exprParserLex.py
--rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_exprParserYacc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15893 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_logFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_matplotlibFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_nonempty_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_normalFormExpression.py
--rw-r--r--   0 runner    (1001) docker     (127)    26817 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_obscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    80609 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_pydantic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_quantumBackedButler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15477 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_query_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_remote_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    17539 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    33656 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_simpleButler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_storageClass.py
--rw-r--r--   0 runner    (1001) docker     (127)    17542 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_testRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_time_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_timespan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-02-22 10:52:06.000000 lsst-daf-butler-26.2024.800/tests/test_versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:36.014124 lsst-daf-butler-26.2024.900/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-02-29 10:30:36.014124 lsst-daf-butler-26.2024.900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.942124 lsst-daf-butler-26.2024.900/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.950123 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/
+-rw-r--r--   0 runner    (1001) docker     (127)    54247 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/concreteStorageClasses.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/configuring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/datastores.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/dimensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22653 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/formatters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/organizing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/queries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/use-in-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/writing-subcommands.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.946123 lsst-daf-butler-26.2024.900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.950123 lsst-daf-butler-26.2024.900/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.950123 lsst-daf-butler-26.2024.900/python/lsst/daf/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.958124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73722 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler_instance_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler_repo_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_column_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_column_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52100 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_config_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_existence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32097 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30001 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_deferredDatasetHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_file_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_file_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30151 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_labeled_butler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_limited_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19541 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_named.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25574 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32289 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_quantum_backed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27865 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_query_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_registry_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37492 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14504 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_storage_class_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23419 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_timespan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.958124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/locked_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/named_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/thread_safe_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/arrow_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.958124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14768 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cliLog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.962123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/_remove_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/_remove_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.962123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/optionGroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44064 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/column_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.962123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastore.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.962123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/composites.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/formatters.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15088 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/dimensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/registry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/repo_transfer_formats.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14810 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/storageClasses.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.966123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57431 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41721 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31187 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/file_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/generic_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/record_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/stored_file_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.966123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/chainedDatastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120549 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/fileDatastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/fileDatastoreClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.966123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/file_datastore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/file_datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22032 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/file_datastore/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27060 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/inMemoryDatastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/ddl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.966123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrowastropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrownumpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrownumpydict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrowtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.970124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25254 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55439 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35795 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15002 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23173 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_governor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22849 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20363 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_packer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_record_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_record_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19854 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_skypix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24448 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_universe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/record_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97583 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/direct_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/direct_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/direct_query_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.970124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/astropyTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42219 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18310 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/mapping_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/nonempty_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/persistence_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19630 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10226 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/pydantic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.974124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_caching_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_record_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_summary_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_dataset_type_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60805 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_registry_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.978124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16738 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/monolithic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.978124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/nameKey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/synthIntKey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/connectionString.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.978124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22479 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.978124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.978124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24029 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40134 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.978124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/dimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/dimensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42986 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/dimensions/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.982123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21076 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79781 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24143 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13309 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_obscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_opaque.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21369 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/nameShrinker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.982123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/default_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/pgsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/opaque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.986124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49430 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33946 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_query_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_query_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39207 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16320 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_sql_query_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25438 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_sql_query_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/butler_sql_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.986124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22509 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/categorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22911 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41024 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/normalForm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.986124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.986124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43384 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137077 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/find_first_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114994 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/sql_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.990124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64443 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)   174129 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/wildcards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.990124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_collection_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11891 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30211 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_remote_butler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.990124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.990124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/handlers/_external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/repo_relocation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.994124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/_associate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/_pruneDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/butlerImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/certifyCalibrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/collectionChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/configDump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/configValidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/createRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/exportCalibs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/ingest_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDataIds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDatasetTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDimensionRecords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/register_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/removeCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/removeDatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/removeRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/retrieveArtifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/transferDatasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.998124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_datasetsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_dummyRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_examplePythonTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23754 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_testRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67398 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/butler_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/cliCmdTestBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/cliLogTestBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/deferredFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/dict_convertible_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/hybrid_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/hybrid_butler_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/server_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/testFormatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24816 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/timespan_database_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.998124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16954 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:36.014124 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16019 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-29 10:30:36.014124 lsst-daf-butler-26.2024.900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:36.014124 lsst-daf-butler-26.2024.900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_astropyTableFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116669 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_butler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_butler_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdAssociate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdConfigDump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdConfigValidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdCreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdIngestFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdPruneDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12885 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDataIds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDatasetTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDimensionRecords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdRemoveCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdRemoveRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdRetrieveArtifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliLog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliPluginLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliUtilSplitCommas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliUtilSplitKv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliUtilToUpper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_connectionString.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29972 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82916 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_ddl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17831 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_dimension_record_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45092 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_exprParserLex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_exprParserYacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15893 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_logFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_matplotlibFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_nonempty_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_normalFormExpression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26817 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_obscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80609 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_pydantic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_quantumBackedButler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15477 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_query_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_remote_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17539 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33656 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_simpleButler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_storageClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17542 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_testRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_timespan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_versioning.py
```

### Comparing `lsst-daf-butler-26.2024.800/PKG-INFO` & `lsst-daf-butler-26.2024.900/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-daf-butler
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: An abstraction layer for reading and writing astronomical data to datastores.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/daf_butler
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-daf-butler-26.2024.800/README.md` & `lsst-daf-butler-26.2024.900/README.md`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/bsd_license.txt` & `lsst-daf-butler-26.2024.900/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/CHANGES.rst` & `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/concreteStorageClasses.rst` & `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/concreteStorageClasses.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/configuring.rst` & `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/configuring.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/datastores.rst` & `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/datastores.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/dimensions.rst` & `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/dimensions.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/formatters.rst` & `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/formatters.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/index.rst` & `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/organizing.rst` & `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/organizing.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/queries.rst` & `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/queries.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/use-in-tests.rst` & `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/use-in-tests.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/doc/lsst.daf.butler/writing-subcommands.rst` & `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/writing-subcommands.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/gpl-v3.0.txt` & `lsst-daf-butler-26.2024.900/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/pyproject.toml` & `lsst-daf-butler-26.2024.900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_butler.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_butler_config.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_butler_instance_options.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler_instance_options.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_butler_repo_index.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler_repo_index.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_column_categorization.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_column_categorization.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_column_tags.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_column_tags.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_column_type_info.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_column_type_info.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_config.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_config_support.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_config_support.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_dataset_association.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_association.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_dataset_existence.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_existence.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_dataset_ref.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_ref.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_dataset_type.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_type.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_deferredDatasetHandle.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_deferredDatasetHandle.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_exceptions.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_file_dataset.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_file_dataset.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_file_descriptor.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_file_descriptor.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_formatter.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_formatter.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_labeled_butler_factory.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_labeled_butler_factory.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_limited_butler.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_limited_butler.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_location.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_location.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_named.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_named.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_quantum.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_quantum.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_quantum_backed.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_quantum_backed.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_query.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_query.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_query_results.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_query_results.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_registry_shim.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_registry_shim.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_storage_class.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_storage_class.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_storage_class_delegate.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_storage_class_delegate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_timespan.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_timespan.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,24 +22,28 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-__all__ = ("Timespan",)
+__all__ = (
+    "SerializedTimespan",
+    "Timespan",
+)
 
 import enum
 import warnings
 from collections.abc import Generator
-from typing import TYPE_CHECKING, Any, ClassVar, Union
+from typing import TYPE_CHECKING, Annotated, Any, ClassVar, Union
 
 import astropy.time
 import astropy.utils.exceptions
 import yaml
+from pydantic import Field
 
 # As of astropy 4.2, the erfa interface is shipped independently and
 # ErfaWarning is no longer an AstropyWarning
 try:
     import erfa
 except ImportError:
     erfa = None
@@ -65,14 +69,19 @@
     """The value used for both `Timespan.begin` and `Timespan.end` for empty
     Timespans that contain no points.
     """
 
 
 TimespanBound = Union[astropy.time.Time, _SpecialTimespanBound, None]
 
+SerializedTimespan = Annotated[list[int], Field(min_length=2, max_length=2)]
+"""JSON-serializable representation of the Timespan class, as a list of two
+integers ``[begin, end]`` in nanoseconds since the epoch.
+"""
+
 
 class Timespan:
     """A half-open time interval with nanosecond precision.
 
     Parameters
     ----------
     begin : `astropy.time.Time`, `Timespan.EMPTY`, or `None`
@@ -479,15 +488,15 @@
             yield from ()
         else:
             if intersection._nsec[0] > self._nsec[0]:
                 yield Timespan(None, None, _nsec=(self._nsec[0], intersection._nsec[0]))
             if intersection._nsec[1] < self._nsec[1]:
                 yield Timespan(None, None, _nsec=(intersection._nsec[1], self._nsec[1]))
 
-    def to_simple(self, minimal: bool = False) -> list[int]:
+    def to_simple(self, minimal: bool = False) -> SerializedTimespan:
         """Return simple python type form suitable for serialization.
 
         Parameters
         ----------
         minimal : `bool`, optional
             Use minimal serialization. Has no effect on for this class.
 
@@ -498,15 +507,15 @@
         """
         # Return the internal nanosecond form rather than astropy ISO string
         return list(self._nsec)
 
     @classmethod
     def from_simple(
         cls,
-        simple: list[int] | None,
+        simple: SerializedTimespan | None,
         universe: DimensionUniverse | None = None,
         registry: Registry | None = None,
     ) -> Timespan | None:
         """Construct a new object from simplified form.
 
         Designed to use the data returned from the `to_simple` method.
```

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_topology.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_topology.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_utilities/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_utilities/locked_object.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/locked_object.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_utilities/named_locks.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/named_locks.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/_utilities/thread_safe_cache.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/thread_safe_cache.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/arrow_utils.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/arrow_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/butler.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/butler.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/cliLog.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cliLog.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/cmd/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/cmd/_remove_collections.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/_remove_collections.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/cmd/_remove_runs.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/_remove_runs.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/cmd/commands.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/opt/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/opt/arguments.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/opt/optionGroups.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/optionGroups.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/opt/options.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/options.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/progress.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/progress.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/cli/utils.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/column_spec.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/column_spec.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/datastores/composites.yaml` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/composites.yaml`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/datastores/formatters.yaml` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/formatters.yaml`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/dimensions.yaml` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/dimensions.yaml`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/registry.yaml` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/registry.yaml`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/configs/storageClasses.yaml` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/storageClasses.yaml`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/_datastore.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/_datastore.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/cache_manager.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/cache_manager.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/composites.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/composites.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/constraints.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/constraints.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/file_templates.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/file_templates.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/generic_base.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/generic_base.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/record_data.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/record_data.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastore/stored_file_info.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/stored_file_info.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/chainedDatastore.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/chainedDatastore.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/fileDatastore.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/fileDatastore.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,17 @@
 from lsst.daf.butler.datastore.stored_file_info import StoredDatastoreItemInfo, StoredFileInfo
 from lsst.daf.butler.datastores.file_datastore.get import (
     DatasetLocationInformation,
     DatastoreFileGetInformation,
     generate_datastore_get_information,
     get_dataset_as_python_object_from_get_info,
 )
+from lsst.daf.butler.datastores.file_datastore.retrieve_artifacts import (
+    determine_destination_for_retrieved_artifact,
+)
 from lsst.daf.butler.datastores.fileDatastoreClient import (
     FileDatastoreGetPayload,
     FileDatastoreGetPayloadFileInfo,
 )
 from lsst.daf.butler.registry.interfaces import (
     DatabaseInsertMode,
     DatastoreRegistryBridge,
@@ -1972,24 +1975,17 @@
         # that will map to the same underlying file transfer.
         to_transfer: dict[ResourcePath, ResourcePath] = {}
 
         for ref in refs:
             locations = self._get_dataset_locations_info(ref)
             for location, _ in locations:
                 source_uri = location.uri
-                target_path: ResourcePathExpression
-                if preserve_path:
-                    target_path = location.pathInStore
-                    if target_path.isabs():
-                        # This is an absolute path to an external file.
-                        # Use the full path.
-                        target_path = target_path.relativeToPathRoot
-                else:
-                    target_path = source_uri.basename()
-                target_uri = destination.join(target_path)
+                target_uri = determine_destination_for_retrieved_artifact(
+                    destination, location.pathInStore, preserve_path
+                )
                 to_transfer[source_uri] = target_uri
 
         # In theory can now parallelize the transfer
         log.debug("Number of artifacts to transfer to %s: %d", str(destination), len(to_transfer))
         for source_uri, target_uri in to_transfer.items():
             target_uri.transfer_from(source_uri, transfer=transfer, overwrite=overwrite)
 
@@ -2051,30 +2047,21 @@
         # these URLs expire.
         # From a strictly technical standpoint there is no reason this
         # shouldn't be a day or more, but there seems to be a political issue
         # where people think there is a risk of end users posting presigned
         # URLs for people without access rights to download.
         url_expiration_time_seconds = 1 * 60 * 60
 
-        def to_file_info_payload(info: DatasetLocationInformation) -> FileDatastoreGetPayloadFileInfo:
-            location, file_info = info
-            return FileDatastoreGetPayloadFileInfo(
-                url=location.uri.generate_presigned_get_url(
-                    expiration_time_seconds=url_expiration_time_seconds
-                ),
-                datastoreRecords=file_info.to_simple(),
-            )
-
         locations = self._get_dataset_locations_info(ref)
         if len(locations) == 0:
             return None
 
         return FileDatastoreGetPayload(
             datastore_type="file",
-            file_info=[to_file_info_payload(info) for info in locations],
+            file_info=[_to_file_info_payload(info, url_expiration_time_seconds) for info in locations],
         )
 
     @transactional
     def put(self, inMemoryDataset: Any, ref: DatasetRef) -> None:
         """Write a InMemoryDataset with a given `DatasetRef` to the store.
 
         Parameters
@@ -2845,7 +2832,29 @@
         if dataset_type is not None:
             ref = ref.overrideStorageClass(dataset_type.storageClass)
         return ref
 
     def get_opaque_table_definitions(self) -> Mapping[str, DatastoreOpaqueTable]:
         # Docstring inherited from the base class.
         return {self._opaque_table_name: DatastoreOpaqueTable(self.makeTableSpec(ddl.GUID), StoredFileInfo)}
+
+
+def _to_file_info_payload(
+    info: DatasetLocationInformation, url_expiration_time_seconds: int
+) -> FileDatastoreGetPayloadFileInfo:
+    location, file_info = info
+
+    # Make sure that we send only relative paths, to avoid leaking
+    # details of our configuration to the client.
+    path = location.pathInStore
+    if path.isabs():
+        relative_path = path.relativeToPathRoot
+    else:
+        relative_path = str(path)
+
+    datastoreRecords = file_info.to_simple()
+    datastoreRecords.path = relative_path
+
+    return FileDatastoreGetPayloadFileInfo(
+        url=location.uri.generate_presigned_get_url(expiration_time_seconds=url_expiration_time_seconds),
+        datastoreRecords=datastoreRecords,
+    )
```

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/file_datastore/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/file_datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/file_datastore/get.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/file_datastore/get.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/datastores/inMemoryDatastore.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/inMemoryDatastore.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/ddl.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/ddl.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/delegates/arrowastropy.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrowastropy.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/delegates/arrownumpy.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrownumpy.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/delegates/arrownumpydict.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrownumpydict.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/delegates/arrowtable.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrowtable.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/delegates/dataframe.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/dataframe.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_config.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_coordinate.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_coordinate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_database.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_database.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_elements.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_elements.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_governor.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_governor.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_graph.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_graph.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_group.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_group.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_packer.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_packer.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_record_set.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_record_set.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_record_table.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_record_table.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_records.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_records.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_schema.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_schema.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_skypix.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_skypix.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/_universe.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_universe.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/construction.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/construction.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/dimensions/record_cache.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/record_cache.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/direct_butler.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/direct_butler.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/direct_query.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/direct_query.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/direct_query_results.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/direct_query_results.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/astropyTable.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/astropyTable.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/file.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/file.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/json.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/json.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/logs.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/logs.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/matplotlib.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/matplotlib.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/packages.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/packages.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/parquet.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/parquet.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/pickle.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/pickle.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/formatters/yaml.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/yaml.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/json.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/json.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/logging.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/logging.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/mapping_factory.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/mapping_factory.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/nonempty_mapping.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/nonempty_mapping.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/persistence_context.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/persistence_context.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/progress.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/progress.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/pydantic_utils.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_caching_context.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_caching_context.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_collection_record_cache.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_record_cache.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_collection_summary.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_summary.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_collection_summary_cache.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_summary_cache.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_collection_type.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_type.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_config.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_dataset_type_cache.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_dataset_type_cache.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_defaults.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_defaults.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_exceptions.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_registry.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_registry.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/_registry_factory.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_registry_factory.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/attributes.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/attributes.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/bridge/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/bridge/ephemeral.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/ephemeral.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/bridge/monolithic.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/monolithic.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/collections/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/collections/_base.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/_base.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/collections/nameKey.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/nameKey.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/collections/synthIntKey.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/synthIntKey.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/connectionString.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/connectionString.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/databases/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/databases/postgresql.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/postgresql.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/databases/sqlite.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/sqlite.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/dimensions/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/dimensions/static.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/dimensions/static.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_attributes.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_attributes.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_bridge.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_bridge.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_collections.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_collections.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_database.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_database.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_datasets.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_datasets.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_dimensions.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_dimensions.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_obscore.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_obscore.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_opaque.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_opaque.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/interfaces/_versioning.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_versioning.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/managers.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/managers.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/nameShrinker.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/nameShrinker.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/_config.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/_manager.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_manager.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/_records.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_records.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/_schema.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_schema.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/_spatial.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_spatial.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/default_spatial.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/default_spatial.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/obscore/pgsphere.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/pgsphere.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/opaque.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/opaque.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_builder.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_builder.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_query.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_query.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_query_backend.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_query_backend.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_query_context.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_query_context.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_readers.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_readers.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_results.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_results.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_sql_query_backend.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_sql_query_backend.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_sql_query_context.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_sql_query_context.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/_structs.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_structs.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/butler_sql_engine.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/butler_sql_engine.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/_predicate.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/_predicate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/categorize.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/categorize.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/check.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/check.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/normalForm.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/normalForm.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/queries/find_first_dataset.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/find_first_dataset.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/sql_registry.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/sql_registry.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/tests/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/tests/_database.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/_database.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/tests/_registry.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     DatasetTypeExpressionError,
     InconsistentDataIdError,
     MissingCollectionError,
     MissingDatasetTypeError,
     NoDefaultCollectionError,
     OrphanedRecordError,
 )
+from .._registry import Registry
 from ..interfaces import ButlerAttributeExistsError
 
 if TYPE_CHECKING:
     from ..sql_registry import SqlRegistry
 
 
 class RegistryTests(ABC):
@@ -118,27 +119,27 @@
         if self.collectionsManager:
             config["managers", "collections"] = self.collectionsManager
         if self.datasetsManager:
             config["managers", "datasets"] = self.datasetsManager
         return config
 
     @abstractmethod
-    def makeRegistry(self, share_repo_with: SqlRegistry | None = None) -> SqlRegistry | None:
-        """Return the SqlRegistry instance to be tested.
+    def makeRegistry(self, share_repo_with: Registry | None = None) -> Registry | None:
+        """Return the Registry instance to be tested.
 
         Parameters
         ----------
-        share_repo_with : `SqlRegistry`, optional
+        share_repo_with : `Registry`, optional
             If provided, the new registry should point to the same data
             repository as this existing registry.
 
         Returns
         -------
-        registry : `SqlRegistry`
-            New `SqlRegistry` instance, or `None` *only* if `share_repo_with`
+        registry : `Registry`
+            New `Registry` instance, or `None` *only* if `share_repo_with`
             is not `None` and this test case does not support that argument
             (e.g. it is impossible with in-memory SQLite DBs).
         """
         raise NotImplementedError()
 
     def loadData(self, registry: SqlRegistry, filename: str) -> None:
         """Load registry test data from ``getDataDir/<filename>``,
```

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/versions.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/versions.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/registry/wildcards.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/wildcards.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/_authentication.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_authentication.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/_config.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/_factory.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_factory.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/_remote_butler.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_remote_butler.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,58 +36,64 @@
 from contextlib import AbstractContextManager
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, TextIO, TypeVar, cast
 from uuid import uuid4
 
 import httpx
 from lsst.daf.butler import __version__
+from lsst.daf.butler.datastores.file_datastore.retrieve_artifacts import (
+    determine_destination_for_retrieved_artifact,
+)
 from lsst.daf.butler.datastores.fileDatastoreClient import (
     FileDatastoreGetPayload,
     get_dataset_as_python_object,
 )
 from lsst.resources import ResourcePath, ResourcePathExpression
 from pydantic import BaseModel, TypeAdapter
 
 from .._butler import Butler
 from .._butler_instance_options import ButlerInstanceOptions
 from .._dataset_existence import DatasetExistence
 from .._dataset_ref import DatasetId, DatasetRef, SerializedDatasetRef
 from .._dataset_type import DatasetType, SerializedDatasetType
 from .._deferredDatasetHandle import DeferredDatasetHandle
-from .._storage_class import StorageClass
+from .._storage_class import StorageClass, StorageClassFactory
 from .._utilities.locked_object import LockedObject
 from ..datastore import DatasetRefURIs
 from ..dimensions import DataCoordinate, DataIdValue, DimensionConfig, DimensionUniverse, SerializedDataId
-from ..registry import MissingDatasetTypeError, NoDefaultCollectionError, RegistryDefaults
-from ..registry.wildcards import CollectionWildcard
+from ..registry import (
+    CollectionArgType,
+    MissingDatasetTypeError,
+    NoDefaultCollectionError,
+    Registry,
+    RegistryDefaults,
+)
 from ._authentication import get_authentication_headers
+from ._collection_args import convert_collection_arg_to_glob_string_list
 from .server_models import (
     CLIENT_REQUEST_ID_HEADER_NAME,
     CollectionList,
     DatasetTypeName,
-    FindDatasetModel,
+    FindDatasetRequestModel,
+    FindDatasetResponseModel,
     GetFileByDataIdRequestModel,
     GetFileResponseModel,
 )
 
 if TYPE_CHECKING:
     from .._file_dataset import FileDataset
     from .._limited_butler import LimitedButler
     from .._query import Query
     from .._timespan import Timespan
     from ..dimensions import DataId, DimensionGroup, DimensionRecord
-    from ..registry import CollectionArgType, Registry
     from ..transfers import RepoExportContext
 
 
 _AnyPydanticModel = TypeVar("_AnyPydanticModel", bound=BaseModel)
 """Generic type variable that accepts any Pydantic model class."""
-_InputCollectionList = str | Sequence[str] | None
-"""The possible types of the ``collections`` parameter of most Butler methods.
-"""
 
 _SERIALIZED_DATA_ID_TYPE_ADAPTER = TypeAdapter(SerializedDataId)
 
 
 class RemoteButler(Butler):  # numpydoc ignore=PR02
     """A `Butler` that can be used to connect through a remote server.
 
@@ -114,14 +120,15 @@
 
     _registry_defaults: RegistryDefaults
     _client: httpx.Client
     _server_url: str
     _access_token: str
     _headers: dict[str, str]
     _cache: RemoteButlerCache
+    _registry: Registry
 
     # This is __new__ instead of __init__ because we have to support
     # instantiation via the legacy constructor Butler.__new__(), which
     # reads the configuration and selects which subclass to instantiate.  The
     # interaction between __new__ and __init__ is kind of wacky in Python.  If
     # we were using __init__ here, __init__ would be called twice (once when
     # the RemoteButler instance is constructed inside Butler.from_config(), and
@@ -133,14 +140,15 @@
         server_url: str,
         options: ButlerInstanceOptions,
         http_client: httpx.Client,
         access_token: str,
         cache: RemoteButlerCache,
     ) -> RemoteButler:
         self = cast(RemoteButler, super().__new__(cls))
+        self.storageClasses = StorageClassFactory()
 
         self._client = http_client
         self._server_url = server_url
         self._cache = cache
         self._access_token = access_token
 
         # TODO: RegistryDefaults should have finish() called on it, but this
@@ -150,14 +158,19 @@
         )
 
         auth_headers = get_authentication_headers(access_token)
         headers = {"user-agent": f"RemoteButler/{__version__}"}
 
         self._headers = auth_headers | headers
 
+        # Avoid a circular import by deferring this import.
+        from ._registry import RemoteButlerRegistry
+
+        self._registry = RemoteButlerRegistry(self)
+
         return self
 
     def isWriteable(self) -> bool:
         # Docstring inherited.
         return False
 
     @property
@@ -257,68 +270,62 @@
         collections: Any = None,
         storageClass: StorageClass | str | None = None,
         **kwargs: Any,
     ) -> Any:
         # Docstring inherited.
         model = self._get_file_info(datasetRefOrType, dataId, collections, kwargs)
 
-        # If the caller provided a DatasetRef or DatasetType, they may have
-        # overridden the storage class on it.  We need to respect this, if they
-        # haven't asked to re-override it.
-        explicitDatasetType = _extract_dataset_type(datasetRefOrType)
-        if explicitDatasetType is not None:
-            if storageClass is None:
-                storageClass = explicitDatasetType.storageClass
-
+        ref = DatasetRef.from_simple(model.dataset_ref, universe=self.dimensions)
         # If the caller provided a DatasetRef, they may have overridden the
         # component on it.  We need to explicitly handle this because we did
         # not send the DatasetType to the server in this case.
-        componentOverride = None
         if isinstance(datasetRefOrType, DatasetRef):
             componentOverride = datasetRefOrType.datasetType.component()
+            if componentOverride:
+                ref = ref.makeComponentRef(componentOverride)
+        ref = _apply_storage_class_override(ref, datasetRefOrType, storageClass)
 
-        ref = DatasetRef.from_simple(model.dataset_ref, universe=self.dimensions)
         return get_dataset_as_python_object(
             ref,
             _to_file_payload(model),
             parameters=parameters,
-            storageClass=storageClass,
-            component=componentOverride,
         )
 
     def _get_file_info(
         self,
         datasetRefOrType: DatasetRef | DatasetType | str,
         dataId: DataId | None,
-        collections: _InputCollectionList,
+        collections: CollectionArgType,
         kwargs: dict[str, DataIdValue],
     ) -> GetFileResponseModel:
         """Send a request to the server for the file URLs and metadata
         associated with a dataset.
         """
         if isinstance(datasetRefOrType, DatasetRef):
             if dataId is not None:
                 raise ValueError("DatasetRef given, cannot use dataId as well")
-            dataset_id = datasetRefOrType.id
-            response = self._get(f"get_file/{dataset_id}", expected_errors=(404,))
-            if response.status_code == 404:
-                raise FileNotFoundError(f"Dataset not found: {datasetRefOrType}")
+            return self._get_file_info_for_ref(datasetRefOrType)
         else:
             request = GetFileByDataIdRequestModel(
                 dataset_type_name=self._normalize_dataset_type_name(datasetRefOrType),
                 collections=self._normalize_collections(collections),
                 data_id=self._simplify_dataId(dataId, kwargs),
             )
             response = self._post("get_file_by_data_id", request, expected_errors=(404,))
             if response.status_code == 404:
                 raise FileNotFoundError(
                     f"Dataset not found with DataId: {dataId} DatasetType: {datasetRefOrType}"
                     f" collections: {collections}"
                 )
+            return self._parse_model(response, GetFileResponseModel)
 
+    def _get_file_info_for_ref(self, ref: DatasetRef) -> GetFileResponseModel:
+        response = self._get(f"get_file/{ref.id}", expected_errors=(404,))
+        if response.status_code == 404:
+            raise FileNotFoundError(f"Dataset not found: {ref.id}")
         return self._parse_model(response, GetFileResponseModel)
 
     def getURIs(
         self,
         datasetRefOrType: DatasetRef | DatasetType | str,
         /,
         dataId: DataId | None = None,
@@ -394,46 +401,64 @@
         storage_class: str | StorageClass | None = None,
         dimension_records: bool = False,
         datastore_records: bool = False,
         **kwargs: Any,
     ) -> DatasetRef | None:
         if datastore_records:
             raise ValueError("Datastore records can not yet be returned in client/server butler.")
-        if timespan:
-            raise ValueError("Timespan can not yet be used in butler client/server.")
 
-        dataset_type = self._normalize_dataset_type_name(dataset_type)
-
-        query = FindDatasetModel(
+        query = FindDatasetRequestModel(
             data_id=self._simplify_dataId(data_id, kwargs),
             collections=self._normalize_collections(collections),
+            timespan=timespan.to_simple() if timespan is not None else None,
             dimension_records=dimension_records,
             datastore_records=datastore_records,
         )
 
-        path = f"find_dataset/{dataset_type}"
+        dataset_type_name = self._normalize_dataset_type_name(dataset_type)
+        path = f"find_dataset/{dataset_type_name}"
         response = self._post(path, query)
 
-        ref = DatasetRef.from_simple(
-            self._parse_model(response, SerializedDatasetRef), universe=self.dimensions
-        )
-        if storage_class is not None:
-            ref = ref.overrideStorageClass(storage_class)
-        return ref
+        model = self._parse_model(response, FindDatasetResponseModel)
+        if model.dataset_ref is None:
+            return None
+
+        ref = DatasetRef.from_simple(model.dataset_ref, universe=self.dimensions)
+        return _apply_storage_class_override(ref, dataset_type, storage_class)
 
     def retrieveArtifacts(
         self,
         refs: Iterable[DatasetRef],
         destination: ResourcePathExpression,
         transfer: str = "auto",
         preserve_path: bool = True,
         overwrite: bool = False,
     ) -> list[ResourcePath]:
-        # Docstring inherited.
-        raise NotImplementedError()
+        destination = ResourcePath(destination).abspath()
+        if not destination.isdir():
+            raise ValueError(f"Destination location must refer to a directory. Given {destination}.")
+
+        if transfer not in ("auto", "copy"):
+            raise ValueError("Only 'copy' and 'auto' transfer modes are supported.")
+
+        output_uris: list[ResourcePath] = []
+        for ref in refs:
+            file_info = _to_file_payload(self._get_file_info_for_ref(ref)).file_info
+            for file in file_info:
+                source_uri = ResourcePath(str(file.url))
+                relative_path = ResourcePath(file.datastoreRecords.path, forceAbsolute=False)
+                target_uri = determine_destination_for_retrieved_artifact(
+                    destination, relative_path, preserve_path
+                )
+                # Because signed URLs expire, we want to do the transfer soon
+                # after retrieving the URL.
+                target_uri.transfer_from(source_uri, transfer="copy", overwrite=overwrite)
+                output_uris.append(target_uri)
+
+        return output_uris
 
     def exists(
         self,
         dataset_ref_or_type: DatasetRef | DatasetType | str,
         /,
         data_id: DataId | None = None,
         *,
@@ -543,16 +568,15 @@
     @property
     def run(self) -> str | None:
         # Docstring inherited.
         return self._registry_defaults.run
 
     @property
     def registry(self) -> Registry:
-        # Docstring inherited.
-        raise NotImplementedError()
+        return self._registry
 
     def _query(self) -> AbstractContextManager[Query]:
         # Docstring inherited.
         raise NotImplementedError()
 
     def _query_data_ids(
         self,
@@ -678,29 +702,25 @@
         except httpx.HTTPError as e:
             raise ButlerServerError(request_id) from e
 
     def _parse_model(self, response: httpx.Response, model: type[_AnyPydanticModel]) -> _AnyPydanticModel:
         """Deserialize a Pydantic model from the body of an HTTP response."""
         return model.model_validate_json(response.content)
 
-    def _normalize_collections(self, collections: _InputCollectionList) -> CollectionList:
+    def _normalize_collections(self, collections: CollectionArgType | None) -> CollectionList:
         """Convert the ``collections`` parameter in the format used by Butler
         methods to a standardized format for the REST API.
         """
         if collections is None:
             if not self.collections:
                 raise NoDefaultCollectionError(
                     "No collections provided, and no defaults from butler construction."
                 )
             collections = self.collections
-        # Temporary hack. Assume strings for collections. In future
-        # want to construct CollectionWildcard and filter it through collection
-        # cache to generate list of collection names.
-        wildcards = CollectionWildcard.from_expression(collections)
-        return CollectionList(list(wildcards.strings))
+        return convert_collection_arg_to_glob_string_list(collections)
 
     def _normalize_dataset_type_name(self, datasetTypeOrName: DatasetType | str) -> DatasetTypeName:
         """Convert DatasetType parameters in the format used by Butler methods
         to a standardized string name for the REST API.
         """
         if isinstance(datasetTypeOrName, DatasetType):
             return DatasetTypeName(datasetTypeOrName.name)
@@ -741,14 +761,45 @@
         return datasetRefOrType
     elif isinstance(datasetRefOrType, DatasetRef):
         return datasetRefOrType.datasetType
     else:
         return None
 
 
+def _apply_storage_class_override(
+    ref: DatasetRef,
+    original_dataset_ref_or_type: DatasetRef | DatasetType | str,
+    explicit_storage_class: StorageClass | str | None,
+) -> DatasetRef:
+    """Return a DatasetRef with its storage class overridden to match the
+    StorageClass supplied by the user as input to one of the search functions.
+
+    Parameters
+    ----------
+    ref : `DatasetRef`
+        The ref to which we will apply the StorageClass override.
+    original_dataset_ref_or_type : `DatasetRef` | `DatasetType` | `str`
+        The ref or type that was input to the search, which may contain a
+        storage class override.
+    explicit_storage_class : `StorageClass` | `str` | `None`
+        A storage class that the user explicitly requested as an override.
+    """
+    if explicit_storage_class is not None:
+        return ref.overrideStorageClass(explicit_storage_class)
+
+    # If the caller provided a DatasetRef or DatasetType, they may have
+    # overridden the storage class on it, and we need to propagate that to the
+    # output.
+    dataset_type = _extract_dataset_type(original_dataset_ref_or_type)
+    if dataset_type is not None:
+        return ref.overrideStorageClass(dataset_type.storageClass)
+
+    return ref
+
+
 def _to_file_payload(get_file_response: GetFileResponseModel) -> FileDatastoreGetPayload:
     if get_file_response.artifact is None:
         ref = get_file_response.dataset_ref
         raise FileNotFoundError(f"Dataset is known, but artifact is not available. (datasetId='{ref.id}')")
 
     return get_file_response.artifact
```

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/_dependencies.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_dependencies.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/_exceptions.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/_factory.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_factory.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/_server.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_server.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/handlers/_external.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/handlers/_external.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,17 +27,18 @@
 
 __all__ = ()
 
 import uuid
 from typing import Any
 
 from fastapi import APIRouter, Depends
-from lsst.daf.butler import Butler, DatasetRef, SerializedDatasetRef, SerializedDatasetType
+from lsst.daf.butler import Butler, DatasetRef, SerializedDatasetRef, SerializedDatasetType, Timespan
 from lsst.daf.butler.remote_butler.server_models import (
-    FindDatasetModel,
+    FindDatasetRequestModel,
+    FindDatasetResponseModel,
     GetFileByDataIdRequestModel,
     GetFileResponseModel,
 )
 
 from .._dependencies import factory_dependency
 from .._exceptions import NotFoundException
 from .._factory import Factory
@@ -117,41 +118,35 @@
     if ref is not None:
         return ref.to_simple()
     # This could raise a 404 since id is not found. The standard implementation
     # get_dataset method returns without error so follow that example here.
     return ref
 
 
-# Not yet supported: TimeSpan is not yet a pydantic model.
-# collections parameter assumes client-side has resolved regexes.
 @external_router.post(
     "/v1/find_dataset/{dataset_type}",
     summary="Retrieve this dataset definition from collection, dataset type, and dataId",
-    response_model=SerializedDatasetRef,
-    response_model_exclude_unset=True,
-    response_model_exclude_defaults=True,
-    response_model_exclude_none=True,
 )
 def find_dataset(
     dataset_type: str,
-    query: FindDatasetModel,
+    query: FindDatasetRequestModel,
     factory: Factory = Depends(factory_dependency),
-) -> SerializedDatasetRef | None:
-    collection_query = query.collections if query.collections else None
-
+) -> FindDatasetResponseModel:
     butler = factory.create_butler()
+    timespan = Timespan.from_simple(query.timespan) if query.timespan is not None else None
     ref = butler.find_dataset(
         dataset_type,
         query.data_id,
-        collections=collection_query,
-        timespan=None,
+        collections=query.collections,
+        timespan=timespan,
         dimension_records=query.dimension_records,
         datastore_records=query.datastore_records,
     )
-    return ref.to_simple() if ref else None
+    serialized_ref = ref.to_simple() if ref else None
+    return FindDatasetResponseModel(dataset_ref=serialized_ref)
 
 
 @external_router.get(
     "/v1/get_file/{dataset_id}",
     summary="Lookup via DatasetId (UUID) the information needed to download and use the files associated"
     " with a dataset.",
 )
```

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/remote_butler/server_models.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,39 +27,49 @@
 
 """Models used for client/server communication."""
 
 __all__ = [
     "CLIENT_REQUEST_ID_HEADER_NAME",
     "CollectionList",
     "DatasetTypeName",
-    "FindDatasetModel",
+    "FindDatasetRequestModel",
+    "FindDatasetResponseModel",
     "GetFileResponseModel",
 ]
 
 from typing import NewType
 
 import pydantic
-from lsst.daf.butler import SerializedDataId, SerializedDatasetRef
+from lsst.daf.butler import SerializedDataId, SerializedDatasetRef, SerializedTimespan
 from lsst.daf.butler.datastores.fileDatastoreClient import FileDatastoreGetPayload
 
 CLIENT_REQUEST_ID_HEADER_NAME = "X-Butler-Client-Request-Id"
 
 CollectionList = NewType("CollectionList", list[str])
+"""A list of search patterns for collection names.  May use glob
+syntax to specify wildcards."""
 DatasetTypeName = NewType("DatasetTypeName", str)
 
 
-class FindDatasetModel(pydantic.BaseModel):
+class FindDatasetRequestModel(pydantic.BaseModel):
     """Request model for find_dataset."""
 
     data_id: SerializedDataId
     collections: CollectionList
+    timespan: SerializedTimespan | None
     dimension_records: bool = False
     datastore_records: bool = False
 
 
+class FindDatasetResponseModel(pydantic.BaseModel):
+    """Response model for find_dataset."""
+
+    dataset_ref: SerializedDatasetRef | None
+
+
 class GetFileByDataIdRequestModel(pydantic.BaseModel):
     """Request model for ``get_file_by_data_id``."""
 
     dataset_type_name: DatasetTypeName
     data_id: SerializedDataId
     collections: CollectionList
```

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/repo_relocation.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/repo_relocation.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/_associate.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/_associate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/_pruneDatasets.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/_pruneDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/butlerImport.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/butlerImport.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/certifyCalibrations.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/certifyCalibrations.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/collectionChain.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/collectionChain.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/configDump.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/configDump.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/configValidate.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/configValidate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/createRepo.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/createRepo.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/exportCalibs.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/exportCalibs.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/ingest_files.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/ingest_files.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/queryCollections.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryCollections.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/queryDataIds.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDataIds.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/queryDatasetTypes.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDatasetTypes.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/queryDatasets.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/queryDimensionRecords.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDimensionRecords.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/register_dataset_type.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/register_dataset_type.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/removeCollections.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/removeCollections.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/removeDatasetType.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/removeDatasetType.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/removeRuns.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/removeRuns.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/retrieveArtifacts.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/retrieveArtifacts.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/script/transferDatasets.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/transferDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/_datasetsHelper.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_datasetsHelper.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/_dummyRegistry.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_dummyRegistry.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/_examplePythonTypes.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_examplePythonTypes.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/_testRepo.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_testRepo.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/butler_query.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/butler_query.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/cliCmdTestBase.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/cliCmdTestBase.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/cliLogTestBase.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/cliLogTestBase.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/deferredFormatter.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/deferredFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/dict_convertible_model.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/dict_convertible_model.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/hybrid_butler.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/hybrid_butler.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,34 +41,38 @@
 from .._file_dataset import FileDataset
 from .._limited_butler import LimitedButler
 from .._query import Query
 from .._storage_class import StorageClass
 from .._timespan import Timespan
 from ..datastore import DatasetRefURIs
 from ..dimensions import DataCoordinate, DataId, DimensionGroup, DimensionRecord, DimensionUniverse
+from ..direct_butler import DirectButler
 from ..registry import CollectionArgType, Registry
 from ..remote_butler import RemoteButler
 from ..transfers import RepoExportContext
+from .hybrid_butler_registry import HybridButlerRegistry
 
 
 class HybridButler(Butler):
     """A `Butler` that delegates methods to internal RemoteButler and
     DirectButler instances.  Intended to allow testing of RemoteButler before
     its implementation is complete, by delegating unsupported methods to
     DirectButler.
     """
 
     _remote_butler: RemoteButler
-    _direct_butler: Butler
+    _direct_butler: DirectButler
+    _registry: Registry
 
-    def __new__(cls, remote_butler: RemoteButler, direct_butler: Butler) -> HybridButler:
+    def __new__(cls, remote_butler: RemoteButler, direct_butler: DirectButler) -> HybridButler:
         self = cast(HybridButler, super().__new__(cls))
         self._remote_butler = remote_butler
         self._direct_butler = direct_butler
         self._datastore = direct_butler._datastore
+        self._registry = HybridButlerRegistry(direct_butler._registry, remote_butler.registry)
         return self
 
     def isWriteable(self) -> bool:
         return self._remote_butler.isWriteable()
 
     def _caching_context(self) -> AbstractContextManager[None]:
         return self._direct_butler._caching_context()
@@ -203,15 +207,15 @@
         self,
         refs: Iterable[DatasetRef],
         destination: ResourcePathExpression,
         transfer: str = "auto",
         preserve_path: bool = True,
         overwrite: bool = False,
     ) -> list[ResourcePath]:
-        return self._direct_butler.retrieveArtifacts(refs, destination, transfer, preserve_path, overwrite)
+        return self._remote_butler.retrieveArtifacts(refs, destination, transfer, preserve_path, overwrite)
 
     def exists(
         self,
         dataset_ref_or_type: DatasetRef | DatasetType | str,
         /,
         data_id: DataId | None = None,
         *,
@@ -313,15 +317,15 @@
 
     @property
     def run(self) -> str | None:
         return self._remote_butler.run
 
     @property
     def registry(self) -> Registry:
-        return self._direct_butler.registry
+        return self._registry
 
     def _query(self) -> AbstractContextManager[Query]:
         return self._direct_butler._query()
 
     def _query_data_ids(
         self,
         dimensions: DimensionGroup | Iterable[str] | str,
```

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/server.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from fastapi.testclient import TestClient
 from lsst.daf.butler import Butler, Config, LabeledButlerFactory
 from lsst.daf.butler.remote_butler import RemoteButler, RemoteButlerFactory
 from lsst.daf.butler.remote_butler.server import create_app
 from lsst.daf.butler.remote_butler.server._dependencies import butler_factory_dependency
 from lsst.resources.s3utils import clean_test_environment_for_s3, getS3Client
 
+from ..direct_butler import DirectButler
 from .hybrid_butler import HybridButler
 from .server_utils import add_auth_header_check_middleware
 
 try:
     # moto v5
     from moto import mock_aws  # type: ignore
 except ImportError:
@@ -99,14 +100,15 @@
 
                 remote_butler = _make_remote_butler(client)
                 remote_butler_without_error_propagation = _make_remote_butler(
                     client_without_error_propagation
                 )
 
                 direct_butler = Butler.from_config(config_file_path, writeable=True)
+                assert isinstance(direct_butler, DirectButler)
                 hybrid_butler = HybridButler(remote_butler, direct_butler)
 
                 yield TestServerInstance(
                     config_file_path=config_file_path,
                     client=client,
                     direct_butler=direct_butler,
                     remote_butler=remote_butler,
```

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/server_utils.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/server_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/testFormatters.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/testFormatters.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/tests/utils.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/time_utils.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/time_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/timespan_database_representation.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/timespan_database_representation.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/transfers/__init__.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/transfers/_context.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/_context.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/transfers/_interfaces.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/_interfaces.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/transfers/_yaml.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/_yaml.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst/daf/butler/utils.py` & `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/python/lsst_daf_butler.egg-info/PKG-INFO` & `lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-daf-butler
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: An abstraction layer for reading and writing astronomical data to datastores.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/daf_butler
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-daf-butler-26.2024.800/python/lsst_daf_butler.egg-info/SOURCES.txt` & `lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 python/lsst/daf/butler/datastores/__init__.py
 python/lsst/daf/butler/datastores/chainedDatastore.py
 python/lsst/daf/butler/datastores/fileDatastore.py
 python/lsst/daf/butler/datastores/fileDatastoreClient.py
 python/lsst/daf/butler/datastores/inMemoryDatastore.py
 python/lsst/daf/butler/datastores/file_datastore/__init__.py
 python/lsst/daf/butler/datastores/file_datastore/get.py
+python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py
 python/lsst/daf/butler/delegates/__init__.py
 python/lsst/daf/butler/delegates/arrowastropy.py
 python/lsst/daf/butler/delegates/arrownumpy.py
 python/lsst/daf/butler/delegates/arrownumpydict.py
 python/lsst/daf/butler/delegates/arrowtable.py
 python/lsst/daf/butler/delegates/dataframe.py
 python/lsst/daf/butler/dimensions/__init__.py
@@ -228,16 +229,18 @@
 python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py
 python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py
 python/lsst/daf/butler/registry/tests/__init__.py
 python/lsst/daf/butler/registry/tests/_database.py
 python/lsst/daf/butler/registry/tests/_registry.py
 python/lsst/daf/butler/remote_butler/__init__.py
 python/lsst/daf/butler/remote_butler/_authentication.py
+python/lsst/daf/butler/remote_butler/_collection_args.py
 python/lsst/daf/butler/remote_butler/_config.py
 python/lsst/daf/butler/remote_butler/_factory.py
+python/lsst/daf/butler/remote_butler/_registry.py
 python/lsst/daf/butler/remote_butler/_remote_butler.py
 python/lsst/daf/butler/remote_butler/server_models.py
 python/lsst/daf/butler/remote_butler/server/__init__.py
 python/lsst/daf/butler/remote_butler/server/_dependencies.py
 python/lsst/daf/butler/remote_butler/server/_exceptions.py
 python/lsst/daf/butler/remote_butler/server/_factory.py
 python/lsst/daf/butler/remote_butler/server/_server.py
@@ -272,14 +275,15 @@
 python/lsst/daf/butler/tests/_testRepo.py
 python/lsst/daf/butler/tests/butler_query.py
 python/lsst/daf/butler/tests/cliCmdTestBase.py
 python/lsst/daf/butler/tests/cliLogTestBase.py
 python/lsst/daf/butler/tests/deferredFormatter.py
 python/lsst/daf/butler/tests/dict_convertible_model.py
 python/lsst/daf/butler/tests/hybrid_butler.py
+python/lsst/daf/butler/tests/hybrid_butler_registry.py
 python/lsst/daf/butler/tests/server.py
 python/lsst/daf/butler/tests/server_utils.py
 python/lsst/daf/butler/tests/testFormatters.py
 python/lsst/daf/butler/tests/utils.py
 python/lsst/daf/butler/transfers/__init__.py
 python/lsst/daf/butler/transfers/_context.py
 python/lsst/daf/butler/transfers/_interfaces.py
```

### Comparing `lsst-daf-butler-26.2024.800/tests/test_astropyTableFormatter.py` & `lsst-daf-butler-26.2024.900/tests/test_astropyTableFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_authentication.py` & `lsst-daf-butler-26.2024.900/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_butler.py` & `lsst-daf-butler-26.2024.900/tests/test_butler.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,14 +383,21 @@
                             )
 
                             if preserve_path:
                                 # No need to run these twice
                                 with self.assertRaises(ValueError):
                                     butler.retrieveArtifacts([ref], destination, transfer="move")
 
+                                with self.assertRaisesRegex(
+                                    ValueError, "^Destination location must refer to a directory"
+                                ):
+                                    butler.retrieveArtifacts(
+                                        [ref], ResourcePath("/some/file.txt", forceDirectory=False)
+                                    )
+
                                 with self.assertRaises(FileExistsError):
                                     butler.retrieveArtifacts([ref], destination)
 
                                 transferred_again = butler.retrieveArtifacts(
                                     [ref], destination, preserve_path=preserve_path, overwrite=True
                                 )
                                 self.assertEqual(set(transferred_again), set(transferred))
```

### Comparing `lsst-daf-butler-26.2024.800/tests/test_butler_factory.py` & `lsst-daf-butler-26.2024.900/tests/test_butler_factory.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_butler_query.py` & `lsst-daf-butler-26.2024.900/tests/test_butler_query.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdAssociate.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdAssociate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdConfigDump.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdConfigDump.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdConfigValidate.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdConfigValidate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdCreate.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdCreate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdImport.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdImport.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdIngestFiles.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdIngestFiles.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdPruneDatasets.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdPruneDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdQueryCollections.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryCollections.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdQueryDataIds.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDataIds.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdQueryDatasetTypes.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDatasetTypes.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdQueryDatasets.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdQueryDimensionRecords.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDimensionRecords.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdRemoveCollections.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdRemoveCollections.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdRemoveRuns.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdRemoveRuns.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliCmdRetrieveArtifacts.py` & `lsst-daf-butler-26.2024.900/tests/test_cliCmdRetrieveArtifacts.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliLog.py` & `lsst-daf-butler-26.2024.900/tests/test_cliLog.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliPluginLoader.py` & `lsst-daf-butler-26.2024.900/tests/test_cliPluginLoader.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliUtilSplitCommas.py` & `lsst-daf-butler-26.2024.900/tests/test_cliUtilSplitCommas.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliUtilSplitKv.py` & `lsst-daf-butler-26.2024.900/tests/test_cliUtilSplitKv.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliUtilToUpper.py` & `lsst-daf-butler-26.2024.900/tests/test_cliUtilToUpper.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_cliUtils.py` & `lsst-daf-butler-26.2024.900/tests/test_cliUtils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_composites.py` & `lsst-daf-butler-26.2024.900/tests/test_composites.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_config.py` & `lsst-daf-butler-26.2024.900/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_connectionString.py` & `lsst-daf-butler-26.2024.900/tests/test_connectionString.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_constraints.py` & `lsst-daf-butler-26.2024.900/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_datasets.py` & `lsst-daf-butler-26.2024.900/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_datastore.py` & `lsst-daf-butler-26.2024.900/tests/test_datastore.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_ddl.py` & `lsst-daf-butler-26.2024.900/tests/test_ddl.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_dimension_record_containers.py` & `lsst-daf-butler-26.2024.900/tests/test_dimension_record_containers.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_dimensions.py` & `lsst-daf-butler-26.2024.900/tests/test_dimensions.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_exprParserLex.py` & `lsst-daf-butler-26.2024.900/tests/test_exprParserLex.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_exprParserYacc.py` & `lsst-daf-butler-26.2024.900/tests/test_exprParserYacc.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_expressions.py` & `lsst-daf-butler-26.2024.900/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_formatter.py` & `lsst-daf-butler-26.2024.900/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_location.py` & `lsst-daf-butler-26.2024.900/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_logFormatter.py` & `lsst-daf-butler-26.2024.900/tests/test_logFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_logging.py` & `lsst-daf-butler-26.2024.900/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_matplotlibFormatter.py` & `lsst-daf-butler-26.2024.900/tests/test_matplotlibFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_nonempty_mapping.py` & `lsst-daf-butler-26.2024.900/tests/test_nonempty_mapping.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_normalFormExpression.py` & `lsst-daf-butler-26.2024.900/tests/test_normalFormExpression.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_obscore.py` & `lsst-daf-butler-26.2024.900/tests/test_obscore.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_packages.py` & `lsst-daf-butler-26.2024.900/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_parquet.py` & `lsst-daf-butler-26.2024.900/tests/test_parquet.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_postgresql.py` & `lsst-daf-butler-26.2024.900/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_progress.py` & `lsst-daf-butler-26.2024.900/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_pydantic_utils.py` & `lsst-daf-butler-26.2024.900/tests/test_pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_quantum.py` & `lsst-daf-butler-26.2024.900/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_quantumBackedButler.py` & `lsst-daf-butler-26.2024.900/tests/test_quantumBackedButler.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_query_relations.py` & `lsst-daf-butler-26.2024.900/tests/test_query_relations.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_server.py` & `lsst-daf-butler-26.2024.900/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_simpleButler.py` & `lsst-daf-butler-26.2024.900/tests/test_simpleButler.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_sqlite.py` & `lsst-daf-butler-26.2024.900/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_storageClass.py` & `lsst-daf-butler-26.2024.900/tests/test_storageClass.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_templates.py` & `lsst-daf-butler-26.2024.900/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_testRepo.py` & `lsst-daf-butler-26.2024.900/tests/test_testRepo.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_thread_utils.py` & `lsst-daf-butler-26.2024.900/tests/test_thread_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_time_utils.py` & `lsst-daf-butler-26.2024.900/tests/test_time_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_timespan.py` & `lsst-daf-butler-26.2024.900/tests/test_timespan.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_utils.py` & `lsst-daf-butler-26.2024.900/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.800/tests/test_versioning.py` & `lsst-daf-butler-26.2024.900/tests/test_versioning.py`

 * *Files identical despite different names*

