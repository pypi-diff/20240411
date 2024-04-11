# Comparing `tmp/hilda-1.4.1.tar.gz` & `tmp/hilda-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilda-1.4.1.tar", last modified: Wed Mar 20 08:20:44 2024, max compression
+gzip compressed data, was "hilda-1.4.2.tar", last modified: Thu Apr 11 11:04:40 2024, max compression
```

## Comparing `hilda-1.4.1.tar` & `hilda-1.4.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.866680 hilda-1.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.850679 hilda-1.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.854679 hilda-1.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-20 08:20:29.000000 hilda-1.4.1/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-20 08:20:29.000000 hilda-1.4.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-20 08:20:29.000000 hilda-1.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-20 08:20:29.000000 hilda-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22398 2024-03-20 08:20:44.866680 hilda-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19741 2024-03-20 08:20:29.000000 hilda-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.854679 hilda-1.4.1/gifs/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-20 08:20:29.000000 hilda-1.4.1/gifs/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-20 08:20:30.000000 hilda-1.4.1/gifs/ui.png
--rw-r--r--   0 runner    (1001) docker     (127)   939935 2024-03-20 08:20:30.000000 hilda-1.4.1/gifs/xpc_print_message.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.858679 hilda-1.4.1/hilda/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-20 08:20:44.000000 hilda-1.4.1/hilda/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)   120119 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/hilda_ascii_art.html
--rw-r--r--   0 runner    (1001) docker     (127)    43340 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/hilda_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/launch_lldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/lldb_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.858679 hilda-1.4.1/hilda/objective_c/
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/objective_c/from_ns_to_json.m
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/objective_c/get_objectivec_class_by_module.m
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/objective_c/get_objectivec_class_description.m
--rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/objective_c/get_objectivec_symbol_data.m
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/objective_c/lsof.m
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/objective_c/to_ns_from_json.m
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.858679 hilda-1.4.1/hilda/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/boringssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/dyld.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/fs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.858679 hilda-1.4.1/hilda/snippets/mach/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/mach/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.862680 hilda-1.4.1/hilda/snippets/macho/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/macho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/macho/all_image_infos.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/macho/apple_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/macho/image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/macho/macho.py
--rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/macho/macho_load_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/remotepairingd.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/syslog.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/snippets/xpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/symbols_jar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.862680 hilda-1.4.1/hilda/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/ui/colors.json
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/ui/ui_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-03-20 08:20:30.000000 hilda-1.4.1/hilda/ui/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.862680 hilda-1.4.1/hilda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22398 2024-03-20 08:20:44.000000 hilda-1.4.1/hilda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-20 08:20:44.000000 hilda-1.4.1/hilda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 08:20:44.000000 hilda-1.4.1/hilda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-20 08:20:44.000000 hilda-1.4.1/hilda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-20 08:20:44.000000 hilda-1.4.1/hilda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 08:20:44.000000 hilda-1.4.1/hilda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-20 08:20:30.000000 hilda-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-20 08:20:30.000000 hilda-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 08:20:44.866680 hilda-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.862680 hilda-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/hilda_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/lldb_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.862680 hilda-1.4.1/tests/test_hilda_client/
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/test_hilda_client/test_from_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/test_hilda_client/test_hilda_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/test_hilda_client/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/test_hilda_client/test_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/test_hilda_client/test_rebind_symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/test_hilda_client/test_registers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.862680 hilda-1.4.1/tests/test_snippets/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/test_snippets/test_xpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:20:44.862680 hilda-1.4.1/tests/test_symbols/
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/test_symbols/test_objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/test_symbols/test_objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/test_symbols/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-20 08:20:30.000000 hilda-1.4.1/tests/test_symbols/test_symbols_jar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.105964 hilda-1.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.089964 hilda-1.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.089964 hilda-1.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-11 11:04:30.000000 hilda-1.4.2/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-11 11:04:30.000000 hilda-1.4.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-11 11:04:30.000000 hilda-1.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-11 11:04:30.000000 hilda-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22398 2024-04-11 11:04:40.105964 hilda-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19741 2024-04-11 11:04:30.000000 hilda-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.093964 hilda-1.4.2/gifs/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 11:04:30.000000 hilda-1.4.2/gifs/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-11 11:04:30.000000 hilda-1.4.2/gifs/ui.png
+-rw-r--r--   0 runner    (1001) docker     (127)   939935 2024-04-11 11:04:30.000000 hilda-1.4.2/gifs/xpc_print_message.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.097964 hilda-1.4.2/hilda/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 11:04:39.000000 hilda-1.4.2/hilda/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120119 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/hilda_ascii_art.html
+-rw-r--r--   0 runner    (1001) docker     (127)    43396 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/hilda_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/launch_lldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/lldb_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.097964 hilda-1.4.2/hilda/objective_c/
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/objective_c/from_ns_to_json.m
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/objective_c/get_objectivec_class_by_module.m
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/objective_c/get_objectivec_class_description.m
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/objective_c/get_objectivec_symbol_data.m
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/objective_c/lsof.m
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/objective_c/to_ns_from_json.m
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.101964 hilda-1.4.2/hilda/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/boringssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/dyld.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/fs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.101964 hilda-1.4.2/hilda/snippets/mach/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/mach/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.101964 hilda-1.4.2/hilda/snippets/macho/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/macho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/macho/all_image_infos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/macho/apple_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/macho/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/macho/macho.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/macho/macho_load_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/remotepairingd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/snippets/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/symbols_jar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.101964 hilda-1.4.2/hilda/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/ui/colors.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/ui/ui_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-04-11 11:04:30.000000 hilda-1.4.2/hilda/ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.105964 hilda-1.4.2/hilda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22398 2024-04-11 11:04:40.000000 hilda-1.4.2/hilda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-11 11:04:40.000000 hilda-1.4.2/hilda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:04:40.000000 hilda-1.4.2/hilda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 11:04:40.000000 hilda-1.4.2/hilda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-11 11:04:40.000000 hilda-1.4.2/hilda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 11:04:40.000000 hilda-1.4.2/hilda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-11 11:04:30.000000 hilda-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-11 11:04:30.000000 hilda-1.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:04:40.105964 hilda-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.101964 hilda-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/hilda_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/lldb_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.105964 hilda-1.4.2/tests/test_hilda_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/test_hilda_client/test_from_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/test_hilda_client/test_hilda_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/test_hilda_client/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/test_hilda_client/test_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/test_hilda_client/test_rebind_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/test_hilda_client/test_registers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.105964 hilda-1.4.2/tests/test_snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/test_snippets/test_xpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:40.105964 hilda-1.4.2/tests/test_symbols/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/test_symbols/test_objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/test_symbols/test_objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/test_symbols/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-11 11:04:30.000000 hilda-1.4.2/tests/test_symbols/test_symbols_jar.py
```

### Comparing `hilda-1.4.1/.github/workflows/python-app.yml` & `hilda-1.4.2/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/.github/workflows/python-publish.yml` & `hilda-1.4.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/.gitignore` & `hilda-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/LICENSE` & `hilda-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/PKG-INFO` & `hilda-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 1.4.1
+Version: 1.4.2
 Summary: LLDB wrapped and empowered by iPython's features
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel cohen <netanelc305@protonmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel cohen <netanelc305@protonmail.com>
 License: Copyright (c) 2012-2023 Doron Zarhi and Metan Perelman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

### Comparing `hilda-1.4.1/README.md` & `hilda-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/gifs/xpc_print_message.gif` & `hilda-1.4.2/gifs/xpc_print_message.gif`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/exceptions.py` & `hilda-1.4.2/hilda/exceptions.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/hilda_ascii_art.html` & `hilda-1.4.2/hilda/hilda_ascii_art.html`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/hilda_client.py` & `hilda-1.4.2/hilda/hilda_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1026,14 +1026,15 @@
         config = Config()
         config.IPCompleter.use_jedi = True
         config.InteractiveShellApp.exec_lines = [
             """disable_logs()""",
             """IPython.get_ipython().events.register('pre_run_cell', self._ipython_run_cell_hook)""",
             MAGIC_FUNCTIONS,
         ]
+        config.BaseIPythonApplication.profile = 'hilda'
         namespace = globals()
         namespace.update(locals())
         namespace['p'] = self
         if additional_namespace is not None:
             namespace.update(additional_namespace)
 
         IPython.start_ipython(config=config, user_ns=namespace)
```

### Comparing `hilda-1.4.1/hilda/launch_lldb.py` & `hilda-1.4.2/hilda/launch_lldb.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/lldb_entrypoint.py` & `hilda-1.4.2/hilda/lldb_entrypoint.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/objective_c/from_ns_to_json.m` & `hilda-1.4.2/hilda/objective_c/from_ns_to_json.m`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/objective_c/get_objectivec_class_by_module.m` & `hilda-1.4.2/hilda/objective_c/get_objectivec_class_by_module.m`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/objective_c/get_objectivec_class_description.m` & `hilda-1.4.2/hilda/objective_c/get_objectivec_class_description.m`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/objective_c/get_objectivec_symbol_data.m` & `hilda-1.4.2/hilda/objective_c/get_objectivec_symbol_data.m`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/objective_c/lsof.m` & `hilda-1.4.2/hilda/objective_c/lsof.m`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/objective_c/to_ns_from_json.m` & `hilda-1.4.2/hilda/objective_c/to_ns_from_json.m`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/objective_c_class.py` & `hilda-1.4.2/hilda/objective_c_class.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/objective_c_symbol.py` & `hilda-1.4.2/hilda/objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/registers.py` & `hilda-1.4.2/hilda/registers.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/snippets/boringssl.py` & `hilda-1.4.2/hilda/snippets/boringssl.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/snippets/dyld.py` & `hilda-1.4.2/hilda/snippets/dyld.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py` & `hilda-1.4.2/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/snippets/macho/all_image_infos.py` & `hilda-1.4.2/hilda/snippets/macho/all_image_infos.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/snippets/macho/image_info.py` & `hilda-1.4.2/hilda/snippets/macho/image_info.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/snippets/macho/macho.py` & `hilda-1.4.2/hilda/snippets/macho/macho.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/snippets/macho/macho_load_commands.py` & `hilda-1.4.2/hilda/snippets/macho/macho_load_commands.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/snippets/remotepairingd.py` & `hilda-1.4.2/hilda/snippets/remotepairingd.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/snippets/xpc.py` & `hilda-1.4.2/hilda/snippets/xpc.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/symbol.py` & `hilda-1.4.2/hilda/symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/symbols_jar.py` & `hilda-1.4.2/hilda/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/ui/ui_manager.py` & `hilda-1.4.2/hilda/ui/ui_manager.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda/ui/views.py` & `hilda-1.4.2/hilda/ui/views.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/hilda.egg-info/PKG-INFO` & `hilda-1.4.2/hilda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 1.4.1
+Version: 1.4.2
 Summary: LLDB wrapped and empowered by iPython's features
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel cohen <netanelc305@protonmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel cohen <netanelc305@protonmail.com>
 License: Copyright (c) 2012-2023 Doron Zarhi and Metan Perelman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

### Comparing `hilda-1.4.1/hilda.egg-info/SOURCES.txt` & `hilda-1.4.2/hilda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/pyproject.toml` & `hilda-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/tests/lldb_entrypoint.py` & `hilda-1.4.2/tests/lldb_entrypoint.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/tests/test_hilda_client/test_from_ns.py` & `hilda-1.4.2/tests/test_hilda_client/test_from_ns.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/tests/test_hilda_client/test_hilda_client.py` & `hilda-1.4.2/tests/test_hilda_client/test_hilda_client.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/tests/test_hilda_client/test_monitor.py` & `hilda-1.4.2/tests/test_hilda_client/test_monitor.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/tests/test_hilda_client/test_ns.py` & `hilda-1.4.2/tests/test_hilda_client/test_ns.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/tests/test_hilda_client/test_registers.py` & `hilda-1.4.2/tests/test_hilda_client/test_registers.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/tests/test_snippets/test_xpc.py` & `hilda-1.4.2/tests/test_snippets/test_xpc.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/tests/test_symbols/test_objective_c_class.py` & `hilda-1.4.2/tests/test_symbols/test_objective_c_class.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/tests/test_symbols/test_objective_c_symbol.py` & `hilda-1.4.2/tests/test_symbols/test_objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/tests/test_symbols/test_symbol.py` & `hilda-1.4.2/tests/test_symbols/test_symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.1/tests/test_symbols/test_symbols_jar.py` & `hilda-1.4.2/tests/test_symbols/test_symbols_jar.py`

 * *Files identical despite different names*

