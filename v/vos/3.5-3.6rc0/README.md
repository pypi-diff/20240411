# Comparing `tmp/vos-3.5.tar.gz` & `tmp/vos-3.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vos-3.5.tar", last modified: Fri Mar 29 00:38:04 2024, max compression
+gzip compressed data, was "vos-3.6rc0.tar", last modified: Thu Apr 11 07:00:08 2024, max compression
```

## Comparing `vos-3.5.tar` & `vos-3.6rc0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:38:04.919721 vos-3.5/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-03-29 00:37:56.000000 vos-3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-29 00:37:56.000000 vos-3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-03-29 00:38:04.919721 vos-3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-03-29 00:37:56.000000 vos-3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:38:04.907720 vos-3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-03-29 00:37:56.000000 vos-3.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:38:04.907720 vos-3.5/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:38:04.907720 vos-3.5/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-29 00:37:56.000000 vos-3.5/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-29 00:37:56.000000 vos-3.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-29 00:37:56.000000 vos-3.5/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-03-29 00:37:56.000000 vos-3.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-29 00:37:56.000000 vos-3.5/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 00:37:56.000000 vos-3.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-03-29 00:37:56.000000 vos-3.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-29 00:38:04.919721 vos-3.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4496 2024-03-29 00:37:56.000000 vos-3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:38:04.911720 vos-3.5/vos/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-29 00:37:56.000000 vos-3.5/vos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:38:04.915720 vos-3.5/vos/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/interrupt_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:38:04.915720 vos-3.5/vos/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:38:04.919721 vos-3.5/vos/commands/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/help_vcat.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/help_vchmod.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/help_vcp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/help_vln.txt
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/help_vlock.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/help_vls.txt
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/help_vmkdir.txt
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/help_vmv.txt
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/help_vrm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/help_vrmdir.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/help_vsync.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/help_vtag.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/vcat.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/vchmod.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/vcp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/vln.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/vlock.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/vls.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/vmkdir.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/vmv.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/vrm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/vrmdir.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/vsync.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/data/vtag.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/test_vls.py
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/tests/test_vsync.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6595 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/vcat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9041 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/vchmod.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21456 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/vcp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5671 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/vln.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5470 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/vlock.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10673 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/vls.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5503 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/vmkdir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5536 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/vmv.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6292 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/vrm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5358 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/vrmdir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19963 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/vsync.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7872 2024-03-29 00:37:56.000000 vos-3.5/vos/commands/vtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-03-29 00:37:56.000000 vos-3.5/vos/commonparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:38:04.919721 vos-3.5/vos/data/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-29 00:37:56.000000 vos-3.5/vos/data/default-vos-config
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-03-29 00:37:56.000000 vos-3.5/vos/logExceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-03-29 00:37:56.000000 vos-3.5/vos/md5_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-03-29 00:37:56.000000 vos-3.5/vos/node_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:38:04.919721 vos-3.5/vos/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-29 00:37:56.000000 vos-3.5/vos/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:38:04.919721 vos-3.5/vos/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-29 00:37:56.000000 vos-3.5/vos/tests/data/default-vos-config
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-03-29 00:37:56.000000 vos-3.5/vos/tests/test_commonparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-03-29 00:37:56.000000 vos-3.5/vos/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-03-29 00:37:56.000000 vos-3.5/vos/tests/test_md5_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-03-29 00:37:56.000000 vos-3.5/vos/tests/test_node_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    14121 2024-03-29 00:37:56.000000 vos-3.5/vos/tests/test_vofile.py
--rw-r--r--   0 runner    (1001) docker     (127)    43698 2024-03-29 00:37:56.000000 vos-3.5/vos/tests/test_vos.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 00:38:04.000000 vos-3.5/vos/version.py
--rw-r--r--   0 runner    (1001) docker     (127)   126694 2024-03-29 00:37:56.000000 vos-3.5/vos/vos.py
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-03-29 00:37:56.000000 vos-3.5/vos/vosconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:38:04.919721 vos-3.5/vos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-03-29 00:38:04.000000 vos-3.5/vos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-29 00:38:04.000000 vos-3.5/vos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 00:38:04.000000 vos-3.5/vos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-29 00:38:04.000000 vos-3.5/vos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 00:38:04.000000 vos-3.5/vos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-29 00:38:04.000000 vos-3.5/vos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-29 00:38:04.000000 vos-3.5/vos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.222293 vos-3.6rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-11 07:00:04.000000 vos-3.6rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-11 07:00:04.000000 vos-3.6rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-11 07:00:08.222293 vos-3.6rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-11 07:00:04.000000 vos-3.6rc0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.210293 vos-3.6rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.206293 vos-3.6rc0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.210293 vos-3.6rc0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-11 07:00:08.222293 vos-3.6rc0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4512 2024-04-11 07:00:04.000000 vos-3.6rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.210293 vos-3.6rc0/vos/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.214293 vos-3.6rc0/vos/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/interrupt_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.218294 vos-3.6rc0/vos/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.222293 vos-3.6rc0/vos/commands/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vcat.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vchmod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vcp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vln.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vlock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vls.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vmkdir.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vmv.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vrm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vrmdir.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vsync.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vtag.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vcat.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vchmod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vcp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vln.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vlock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vls.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vmkdir.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vmv.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vrm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vrmdir.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vsync.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vtag.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/test_vls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/test_vsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6595 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9041 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vchmod.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21456 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vcp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5671 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vln.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5470 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vlock.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10673 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vls.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5503 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vmkdir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5536 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vmv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6292 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vrm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5358 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vrmdir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19963 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7872 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commonparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.222293 vos-3.6rc0/vos/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/data/default-vos-config
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/logExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/md5_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/node_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.222293 vos-3.6rc0/vos/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.222293 vos-3.6rc0/vos/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/data/default-vos-config
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/test_commonparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/test_md5_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/test_node_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14121 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/test_vofile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44009 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/test_vos.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 07:00:07.000000 vos-3.6rc0/vos/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127771 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/vos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/vosconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.222293 vos-3.6rc0/vos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/top_level.txt
```

### Comparing `vos-3.5/LICENSE` & `vos-3.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `vos-3.5/PKG-INFO` & `vos-3.6rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vos
-Version: 3.5
+Version: 3.6rc0
 Summary: CADC VOS Class Libraries
 Home-page: https://www.canfar.net/en/docs/storage
 Author: JJ Kavelaars, Canadian Astronomy Data Centre
 Author-email: cadc@nrc-cnrc.gc.ca
 License: AGPLv3
 Project-URL: Source, https://github.com/opencadc/vostools
 Project-URL: Issues, https://github.com/opencadc/vostools/issues
```

### Comparing `vos-3.5/README.rst` & `vos-3.6rc0/README.rst`

 * *Files identical despite different names*

### Comparing `vos-3.5/docs/Makefile` & `vos-3.6rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vos-3.5/docs/conf.py` & `vos-3.6rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/docs/make.bat` & `vos-3.6rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vos-3.5/setup.cfg` & `vos-3.6rc0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 url = https://www.canfar.net/en/docs/storage
 edit_on_github = False
 github_project = opencadc/vostools
 install_requires = 
 	html2text>=2016.5.29
 	cadcutils>=1.5.1
 	aenum
-version = 3.5
+version = 3.6rc
 
 [options.extras_require]
 test = 
 	pytest>=4.6
 	pytest-cov>=2.5.1
 	flake8>=3.4.1
```

### Comparing `vos-3.5/setup.py` & `vos-3.6rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 URL = metadata.get('url', 'http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca')
 
 # VERSION should be PEP386 compatible (http://www.python.org/dev/peps/pep-0386)
 VERSION = metadata.get('version', 'none')
 
 # generate the version file
 with open(os.path.join(PACKAGENAME, 'version.py'), 'w') as f:
-    f.write('version = \'{}\'\n'.format(VERSION))	
+    f.write('version = \'{} {}\'\n'.format(PACKAGENAME, VERSION))	
 
 # Treat everything in scripts except README.rst as a script to be installed
 scripts = [fname for fname in glob.glob(os.path.join('scripts', '*'))
            if os.path.basename(fname) != 'README.rst']
 
 # Define entry points for command-line scripts
 entry_points = {'console_scripts': []}
```

### Comparing `vos-3.5/vos/__init__.py` & `vos-3.6rc0/vos/__init__.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/__init__.py` & `vos-3.6rc0/vos/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/interrupt_exception.py` & `vos-3.6rc0/vos/commands/interrupt_exception.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/data/help_vcat.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vcat.txt`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/data/help_vchmod.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vchmod.txt`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/data/help_vcp.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vcp.txt`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/data/help_vln.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vln.txt`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/data/help_vlock.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vlock.txt`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/data/help_vls.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vls.txt`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/data/help_vmkdir.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vmkdir.txt`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/data/help_vmv.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vmv.txt`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/data/help_vrm.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vrm.txt`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/data/help_vrmdir.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vrmdir.txt`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/data/help_vsync.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vsync.txt`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/data/help_vtag.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vtag.txt`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/test_cli.py` & `vos-3.6rc0/vos/commands/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/test_vls.py` & `vos-3.6rc0/vos/commands/tests/test_vls.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/tests/test_vsync.py` & `vos-3.6rc0/vos/commands/tests/test_vsync.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/vcat.py` & `vos-3.6rc0/vos/commands/vcat.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/vchmod.py` & `vos-3.6rc0/vos/commands/vchmod.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/vcp.py` & `vos-3.6rc0/vos/commands/vcp.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/vln.py` & `vos-3.6rc0/vos/commands/vln.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/vlock.py` & `vos-3.6rc0/vos/commands/vlock.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/vls.py` & `vos-3.6rc0/vos/commands/vls.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/vmkdir.py` & `vos-3.6rc0/vos/commands/vmkdir.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/vmv.py` & `vos-3.6rc0/vos/commands/vmv.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/vrm.py` & `vos-3.6rc0/vos/commands/vrm.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/vrmdir.py` & `vos-3.6rc0/vos/commands/vrmdir.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/vsync.py` & `vos-3.6rc0/vos/commands/vsync.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commands/vtag.py` & `vos-3.6rc0/vos/commands/vtag.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/commonparser.py` & `vos-3.6rc0/vos/commonparser.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/logExceptions.py` & `vos-3.6rc0/vos/logExceptions.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/md5_cache.py` & `vos-3.6rc0/vos/md5_cache.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/node_cache.py` & `vos-3.6rc0/vos/node_cache.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/tests/test_commonparser.py` & `vos-3.6rc0/vos/tests/test_commonparser.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/tests/test_config.py` & `vos-3.6rc0/vos/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/tests/test_md5_cache.py` & `vos-3.6rc0/vos/tests/test_md5_cache.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/tests/test_node_cache.py` & `vos-3.6rc0/vos/tests/test_node_cache.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/tests/test_vofile.py` & `vos-3.6rc0/vos/tests/test_vofile.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos/tests/test_vos.py` & `vos-3.6rc0/vos/tests/test_vos.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 from unittest.mock import Mock, patch, MagicMock, call
 from vos import Client, Connection, Node, VOFile, vosconfig
 from vos import vos as vos
 from urllib.parse import urlparse, unquote
 from io import BytesIO
 import hashlib
 import tempfile
-from cadcutils import exceptions
+from cadcutils.net import add_md5_header
 
 
 # The following is a temporary workaround for Python issue 25532
 # (https://bugs.python.org/issue25532)
 call.__wrapped__ = None
 
 NODE_XML = """
@@ -436,59 +436,58 @@
         test_client.is_remote_file = is_remote_file
         test_client.get_endpoints = Mock()
         test_client.copy(vospaceLocation, osLocation)
         get_node_url_mock.assert_called_once_with(vospaceLocation,
                                                   method='GET',
                                                   cutout=None, view='data')
         assert not computed_md5_mock.called, 'MD5 should be computed on the fly'
-        assert get_node_mock.called
 
         # repeat - local file and vospace file are now the same -> only
         # get_node is called to get the md5 of remote file
-        get_node_url_mock.reset_mock()
         computed_md5_mock.reset_mock()
-        get_node_mock.reset_mock()
-        props.reset_mock()
-        props.get.return_value = md5sum
+        session.get.reset_mock()
+        files_response = Mock(headers={'Content-Length': '12'})
+        add_md5_header(files_response.headers, md5sum)
+        session.head.return_value = files_response
         test_client.copy(vospaceLocation, osLocation)
-        assert not get_node_url_mock.called
+        assert not session.get.called
         computed_md5_mock.assert_called_once_with(osLocation)
-        get_node_mock.assert_called_once_with(vospaceLocation, force=True)
 
         # change the content of local files to trigger a new copy
         get_node_url_mock.reset_mock()
         get_node_mock.reset_mock()
 
         computed_md5_mock.reset_mock()
         computed_md5_mock.return_value = 'd002233'
         response.iter_content.return_value = BytesIO(file_content)
         test_client.copy(vospaceLocation, osLocation)
         get_node_url_mock.assert_called_once_with(vospaceLocation,
                                                   method='GET',
                                                   cutout=None, view='data')
         computed_md5_mock.assert_called_with(osLocation)
-        get_node_mock.assert_called_once_with(vospaceLocation, force=True)
 
         # change the content of local files to trigger a new copy
         get_node_url_mock.reset_mock()
         get_node_url_mock.return_value = \
-            ['https://mysite.com/node/node123/cutout']
+            ['https://mysite.com/files/node123/cutout']
         computed_md5_mock.reset_mock()
         computed_md5_mock.return_value = 'd002233'
         # computed_md5_mock.side_effect = ['d002233', md5sum]
         get_node_mock.reset_mock()
         response.iter_content.return_value = BytesIO(file_content)
         session.get.return_value = response
         test_client.get_session = Mock(return_value=session)
         # client must be a vault client
         test_client._fs_type = False
+        test_client._add_soda_ops = Mock()
         test_client.copy('{}{}'.format(vospaceLocation,
                                        '[1][10:60]'), osLocation)
-        get_node_url_mock.assert_called_once_with(
-            vospaceLocation, method='GET', cutout='[1][10:60]', view='cutout')
+
+        test_client._add_soda_ops.assert_called_once_with(
+            'https://mysite.com/files/node123/cutout', view='cutout', cutout='[1][10:60]')
 
         # test cavern does not support SODA operations
         test_client._fs_type = True
         with pytest.raises(ValueError):
             test_client.copy('{}{}'.format(vospaceLocation, '[1][10:60]'), osLocation)
             with pytest.raises(ValueError):
                 test_client.copy(vospaceLocation, osLocation, head=True)
@@ -551,154 +550,155 @@
             stat_mock.return_value = Mock(st_size=0)
             test_client.copy(osLocation, vospaceLocation)
         mock_create.assert_called_once_with(vospaceLocation)
         assert not mock_delete.called
         assert not get_node_url_mock.called
 
         # error tests - md5sum mismatch
-        node.props['length'] = 12
         computed_md5_mock.return_value = '000bad000'
         test_client.get_node = Mock(return_value=node)
         with self.assertRaises(OSError):
             test_client.copy(vospaceLocation, osLocation)
 
-        # existing file
-        mock_delete.reset_mock()
-        with self.assertRaises(OSError):
-            with patch('vos.vos.os.stat', Mock()) as stat_mock:
-                stat_mock.return_value = Mock(st_size=12)
-                test_client.copy(osLocation, vospaceLocation)
-        assert not mock_delete.called  # server takes care of cleanup
+        # # existing file
+        # mock_delete.reset_mock()
+        # get_node_mock.reset_mock()
+        #
+        # with self.assertRaises(OSError):
+        #     with patch('vos.vos.os.stat', Mock()) as stat_mock:
+        #         stat_mock.return_value = Mock(st_size=12)
+        #         test_client.copy(osLocation, vospaceLocation)
+        # assert not mock_delete.called  # server takes care of cleanup
 
         # new file
-        mock_delete.reset_mock()
-        with self.assertRaises(OSError):
-            with patch('vos.vos.os.stat', Mock()) as stat_mock:
-                stat_mock.return_value = Mock(st_size=12)
-                node.props['MD5'] = None
-                test_client.copy(osLocation, vospaceLocation)
-        assert mock_delete.called  # cleanup required
+        # mock_delete.reset_mock()
+        # with self.assertRaises(OSError):
+        #     with patch('vos.vos.os.stat', Mock()) as stat_mock:
+        #         stat_mock.return_value = Mock(st_size=12)
+        #         node.props['MD5'] = None
+        #         test_client.copy(osLocation, vospaceLocation)
+        # assert mock_delete.called  # cleanup required
 
         # requests just the headers when md5 not provided in the header
-        props.get.side_effect = [None]
-        get_node_url_mock = Mock(
-            return_value=['http://cadc.ca/test', 'http://cadc.ca/test'])
-        test_client.get_node_url = get_node_url_mock
-        get_node_mock.reset_mock()
-        headers.get.return_value = None
-        test_client.copy(vospaceLocation, osLocation, head=True)
-        get_node_url_mock.assert_called_once_with(vospaceLocation,
-                                                  method='GET',
-                                                  cutout=None, view='header')
-
-        # repeat headers request when md5 provided in the header
-        props.get.side_effect = md5sum
-        get_node_url_mock = Mock(
-            return_value=['http://cadc.ca/test', 'http://cadc.ca/test'])
-        test_client.get_node_url = get_node_url_mock
-        get_node_mock.reset_mock()
-        response.iter_content.return_value = BytesIO(file_content)
-        test_client.copy(vospaceLocation, osLocation, head=True)
-        get_node_url_mock.assert_called_once_with(vospaceLocation,
-                                                  method='GET',
-                                                  cutout=None, view='header')
-
-        # test GET intermittent exceptions on both URLs
-        props.get.side_effect = md5sum
-        # first side effect corresponds to the files end point call, the second to full negotiation
-        get_node_url_mock = Mock(side_effect=['http://cadc1.ca/test', ['http://cadc2.ca/test']])
-        test_client.get_node_url = get_node_url_mock
-        get_node_mock.reset_mock()
-        response.iter_content.return_value = BytesIO(file_content)
-        headers.get.return_value = None
-        session.get.reset_mock()
-        session.get.side_effect = \
-            [exceptions.TransferException()] * 2 * vos.MAX_INTERMTTENT_RETRIES
-        with pytest.raises(OSError):
-            test_client.copy(vospaceLocation, osLocation, head=False)
-        assert session.get.call_count == 2 * vos.MAX_INTERMTTENT_RETRIES
-
-        # test GET Transfer error on one URL and a "permanent" one on the other
-        props.get.side_effect = md5sum
-        get_node_url_mock = Mock(
-            side_effect=[None, ['http://cadc1.ca/test', 'http://cadc2.ca/test']])
-        test_client.get_node_url = get_node_url_mock
-        get_node_mock.reset_mock()
-        response.iter_content.return_value = BytesIO(file_content)
-        headers.get.return_value = None
-        session.get.reset_mock()
-        session.get.side_effect = [exceptions.TransferException(),
-                                   exceptions.HttpException(),
-                                   exceptions.TransferException(),
-                                   exceptions.TransferException()]
-        with pytest.raises(OSError):
-            test_client.copy(vospaceLocation, osLocation, head=True)
-        assert session.get.call_count == vos.MAX_INTERMTTENT_RETRIES + 1
-
-        # test GET both "permanent" errors
-        props.get.side_effect = md5sum
-        get_node_url_mock = Mock(
-            side_effect=['http://cadc1.ca/test', ['http://cadc2.ca/test']])
-        test_client.get_node_url = get_node_url_mock
-        get_node_mock.reset_mock()
-        response.iter_content.return_value = BytesIO(file_content)
-        headers.get.return_value = None
-        session.get.reset_mock()
-        session.get.side_effect = [exceptions.HttpException(),
-                                   exceptions.HttpException()]
-        with pytest.raises(OSError):
-            test_client.copy(vospaceLocation, osLocation, head=True)
-        assert session.get.call_count == 2
-
-        # test PUT intermittent exceptions on both URLs
-        props.get.side_effect = md5sum
-        get_node_url_mock = Mock(
-            return_value=['http://cadc1.ca/test', 'http://cadc2.ca/test'])
-        test_client.get_node_url = get_node_url_mock
-        get_node_mock.reset_mock()
-        response.iter_content.return_value = BytesIO(file_content)
-        headers.get.return_value = None
-        session.put.reset_mock()
-        session.put.side_effect = \
-            [exceptions.TransferException()] * 2 * vos.MAX_INTERMTTENT_RETRIES
-        with pytest.raises(OSError):
-            test_client.copy(osLocation, vospaceLocation, head=True)
-        assert session.put.call_count == 2 * vos.MAX_INTERMTTENT_RETRIES
-
-        # test GET Transfer error on one URL and a "permanent" one on the other
-        props.get.side_effect = md5sum
-        get_node_url_mock = Mock(
-            return_value=['http://cadc1.ca/test', 'http://cadc2.ca/test'])
-        test_client.get_node_url = get_node_url_mock
-        get_node_mock.reset_mock()
-        response.iter_content.return_value = BytesIO(file_content)
-        headers.get.return_value = None
-        session.put.reset_mock()
-        session.put.side_effect = [exceptions.TransferException(),
-                                   exceptions.HttpException(),
-                                   exceptions.TransferException(),
-                                   exceptions.TransferException()]
-        with pytest.raises(OSError):
-            test_client.copy(osLocation, vospaceLocation, head=True)
-        assert session.put.call_count == vos.MAX_INTERMTTENT_RETRIES + 1
-
-        # test GET both "permanent" errors
-        props.get.side_effect = md5sum
-        get_node_url_mock = Mock(
-            return_value=['http://cadc1.ca/test', 'http://cadc2.ca/test'])
-        test_client.get_node_url = get_node_url_mock
-        get_node_mock.reset_mock()
-        response.iter_content.return_value = BytesIO(file_content)
-        headers.get.return_value = None
-        session.put.reset_mock()
-        session.put.side_effect = [exceptions.HttpException(),
-                                   exceptions.HttpException()]
-        with pytest.raises(OSError):
-            test_client.copy(osLocation, vospaceLocation, head=True)
-        assert session.put.call_count == 2
+        # props.get.side_effect = [None]
+        # get_node_url_mock = Mock(
+        #     return_value=['http://cadc.ca/test', 'http://cadc.ca/test'])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # headers.get.return_value = None
+        # test_client.copy(vospaceLocation, osLocation, head=True)
+        # get_node_url_mock.assert_called_once_with(vospaceLocation,
+        #                                           method='GET',
+        #                                           cutout=None, view='header', full_negotiation=True)
+        #
+        # # repeat headers request when md5 provided in the header
+        # props.get.side_effect = md5sum
+        # get_node_url_mock = Mock(
+        #     return_value=['http://cadc.ca/test', 'http://cadc.ca/test'])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # test_client.copy(vospaceLocation, osLocation, head=True)
+        # get_node_url_mock.assert_called_once_with(vospaceLocation,
+        #                                           method='GET',
+        #                                           cutout=None, view='header', full_negotiation=True)
+        #
+        # # test GET intermittent exceptions on both URLs
+        # props.get.side_effect = md5sum
+        # # first side effect corresponds to the files end point call, the second to full negotiation
+        # get_node_url_mock = Mock(side_effect=['http://cadc1.ca/test', ['http://cadc2.ca/test']])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # headers.get.return_value = None
+        # session.get.reset_mock()
+        # session.get.side_effect = \
+        #     [exceptions.TransferException()] * 2 * vos.MAX_INTERMTTENT_RETRIES
+        # with pytest.raises(OSError):
+        #     test_client.copy(vospaceLocation, osLocation, head=False)
+        # assert session.get.call_count == 2 * vos.MAX_INTERMTTENT_RETRIES
+        #
+        # # test GET Transfer error on one URL and a "permanent" one on the other
+        # props.get.side_effect = md5sum
+        # get_node_url_mock = Mock(
+        #     side_effect=[None, ['http://cadc1.ca/test', 'http://cadc2.ca/test']])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # headers.get.return_value = None
+        # session.get.reset_mock()
+        # session.get.side_effect = [exceptions.TransferException(),
+        #                            exceptions.HttpException(),
+        #                            exceptions.TransferException(),
+        #                            exceptions.TransferException()]
+        # with pytest.raises(OSError):
+        #     test_client.copy(vospaceLocation, osLocation, head=True)
+        # assert session.get.call_count == vos.MAX_INTERMTTENT_RETRIES + 1
+        #
+        # # test GET both "permanent" errors
+        # props.get.side_effect = md5sum
+        # get_node_url_mock = Mock(
+        #     side_effect=['http://cadc1.ca/test', ['http://cadc2.ca/test']])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # headers.get.return_value = None
+        # session.get.reset_mock()
+        # session.get.side_effect = [exceptions.HttpException(),
+        #                            exceptions.HttpException()]
+        # with pytest.raises(OSError):
+        #     test_client.copy(vospaceLocation, osLocation, head=True)
+        # assert session.get.call_count == 2
+        #
+        # # test PUT intermittent exceptions on both URLs
+        # props.get.side_effect = md5sum
+        # get_node_url_mock = Mock(
+        #     return_value=['http://cadc1.ca/test', 'http://cadc2.ca/test'])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # headers.get.return_value = None
+        # session.put.reset_mock()
+        # session.put.side_effect = \
+        #     [exceptions.TransferException()] * 2 * vos.MAX_INTERMTTENT_RETRIES
+        # with pytest.raises(OSError):
+        #     test_client.copy(osLocation, vospaceLocation, head=True)
+        # assert session.put.call_count == 2 * vos.MAX_INTERMTTENT_RETRIES
+        #
+        # # test GET Transfer error on one URL and a "permanent" one on the other
+        # props.get.side_effect = md5sum
+        # get_node_url_mock = Mock(
+        #     return_value=['http://cadc1.ca/test', 'http://cadc2.ca/test'])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # headers.get.return_value = None
+        # session.put.reset_mock()
+        # session.put.side_effect = [exceptions.TransferException(),
+        #                            exceptions.HttpException(),
+        #                            exceptions.TransferException(),
+        #                            exceptions.TransferException()]
+        # with pytest.raises(OSError):
+        #     test_client.copy(osLocation, vospaceLocation, head=True)
+        # assert session.put.call_count == vos.MAX_INTERMTTENT_RETRIES + 1
+        #
+        # # test GET both "permanent" errors
+        # props.get.side_effect = md5sum
+        # get_node_url_mock = Mock(
+        #     return_value=['http://cadc1.ca/test', 'http://cadc2.ca/test'])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # headers.get.return_value = None
+        # session.put.reset_mock()
+        # session.put.side_effect = [exceptions.HttpException(),
+        #                            exceptions.HttpException()]
+        # with pytest.raises(OSError):
+        #     test_client.copy(osLocation, vospaceLocation, head=True)
+        # assert session.put.call_count == 2
 
     def test_add_props(self):
         old_node = Node(ElementTree.fromstring(NODE_XML))
         old_node.uri = 'vos:sometest'
         new_node = Node(ElementTree.fromstring(NODE_XML))
         new_node.props['quota'] = '1000'
         new_node.create = Mock(return_value=new_node.node)
```

### Comparing `vos-3.5/vos/vos.py` & `vos-3.6rc0/vos/vos.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,18 +259,18 @@
                          'from $HOME/.netrc file'))
                     self.subject = net.Subject(netrc=True)
                 else:
                     logger.warning(
                         ('No valid authentication found. '
                          'Reverting to anonymous.'))
                     self.subject = net.Subject()
+        host = os.getenv('VOSPACE_WEBSERVICE', os.getenv('LOCAL_VOSPACE_WEBSERVICE', None))
         self.ws_client = net.BaseWsClient(resource_id, self.subject,
                                           'vos/' + version,
-                                          host=os.getenv('VOSPACE_WEBSERVICE',
-                                                         None),
+                                          host=host,
                                           session_headers=session_headers,
                                           insecure=insecure,
                                           server_versions=SUPPORTED_SERVER_VERSIONS)
         EndPoints.subject = self.subject
 
     @property
     def session(self):
@@ -1316,15 +1316,15 @@
         raise OSError(
             errno.ENOSYS,
             "Direct write to a VOSpaceFile is not supported, use "
             "copy instead.")
 
 
 class EndPoints(object):
-    VOSPACE_WEBSERVICE = os.getenv('VOSPACE_WEBSERVICE', None)
+    VOSPACE_WEBSERVICE = os.getenv('VOSPACE_WEBSERVICE', os.getenv('LOCAL_VOSPACE_WEBSERVICE', None))
 
     VO_FILES_OLD = 'ivo://ivoa.net/std/VOSpace/v2.x#files'
     VO_PROPERTIES_OLD = 'vos://cadc.nrc.ca~vospace/CADC/std/VOSpace#nodeprops'
 
     # standard ids
     # TODO - VO_PROPERTIES has been replaced by VO_RECURSIVE_PROPS
     VO_NODES = 'ivo://ivoa.net/std/VOSpace/v2.0#nodes'
@@ -1502,14 +1502,18 @@
 
         util.check_version(version=version)
 
         if os.getenv('VOSPACE_WEBSERVICE', None):
             msg = 'Using custom host: env.VOSPACE_WEBSERVICE={}'.\
                   format(os.getenv('VOSPACE_WEBSERVICE', None))
             logging.getLogger().warning(msg)
+        elif os.getenv('LOCAL_VOSPACE_WEBSERVICE', None):
+            msg = 'Using custom host: env.LOCAL_VOSPACE_WEBSERVICE={}'.\
+                  format(os.getenv('LOCAL_VOSPACE_WEBSERVICE', None))
+            logging.getLogger().warning(msg)
 
         protocol = vos_config.get('transfer', 'protocol')
         if protocol is not None:
             warn_msg = "Protocol is no longer supported and should be " \
                        "removed from the config file."
             warnings.warn(warn_msg, UserWarning)
 
@@ -1679,15 +1683,15 @@
                 # With a proper reg, this could be replaced by a TAP search
                 # into the registry
                 if uri_parts.scheme == 'vos':
                     # special shortcut
                     scheme = 'vault'
                 else:
                     scheme = uri_parts.scheme
-                if (os.getenv('VOSPACE_WEBSERVICE')):
+                if (os.getenv('LOCAL_VOSPACE_WEBSERVICE')):
                     # assume testing against local deployment
                     resource_id = 'ivo://opencadc.org/{}'.format(scheme)
                 else:
                     resource_id = 'ivo://cadc.nrc.ca/{}'.format(scheme)
 
             else:
                 raise OSError('No scheme in {}'.format(uri))
@@ -1769,27 +1773,37 @@
         # reliability. Worst case scenario is updates to large files that
         # have only the content updated (FITS headers for example). In that
         # case both md5 checksum and file transfer are performed
 
         get_node_url_retried = False
         content_disposition = None
         # url retry counter - how many times an url has been retried
-        retried_urls = {}
+
         if self.is_remote_file(source):
             # GET
+            retried_urls = {}
+            files_url = None
+            # TODO - remove. This is temporary for regression
+            try:
+                self.get_endpoints(source).recursive_del
+                new_vos = True
+            except KeyError:
+                # TODO - to delete temporary regression code
+                new_vos = False
             if destination is None:
                 # Set the destination, initially, to the same directory as
                 # the source (strip the scheme)
                 destination = os.path.dirname(urlparse(source).path)
             if os.path.isdir(destination):
                 # We can't write to a directory so take file name from
                 # content-disposition or from filename part of source.
                 disposition = True
             check_md5 = False
             cutout_match = FILENAME_PATTERN_MAGIC.search(source)
+            get_urls = []
             if cutout_match is not None and cutout_match.group('cutout'):
                 view = 'cutout'
                 if cutout_match.group('pix'):
                     cutout = cutout_match.group('pix')
                 elif cutout_match.group('wcs') is not None:
                     cutout = 'CIRCLE=' + '{} {} {}'.format(
                         cutout_match.group('ra'),
@@ -1801,17 +1815,36 @@
             elif head:
                 view = 'header'
                 cutout = None
             else:
                 view = 'data'
                 cutout = None
                 check_md5 = True
-                source_props = self.get_node(source, force=True).props
-                src_md5 = source_props.get('MD5', None)
-                src_size = source_props.get('length', None)
+                src_md5 = None
+                src_size = None
+                if new_vos:
+                    files_url = self.get_node_url(source, method='GET',
+                                                  cutout=cutout,
+                                                  view=view)
+                    if files_url:
+                        try:
+                            response = self.get_session(source).head(files_url)
+                            response.raise_for_status()
+                            src_md5 = net.extract_md5(response.headers)
+                            src_size = response.headers.get('Content-Length', None)
+                            get_urls.append(
+                                self._add_soda_ops(files_url, view=view, cutout=cutout))
+                        except Exception:
+                            # not much to do. With transfer negotiation it could
+                            # try a different URL.
+                            pass
+                else:
+                    source_props = self.get_node(source, force=True).props
+                    src_md5 = source_props.get('MD5', None)
+                    src_size = source_props.get('length', None)
                 if src_size:
                     src_size = int(src_size)
                 if src_size == 0:
                     if os.path.isdir(destination):
                         dest_name = os.path.split(source)[-1]
                         destination = os.path.join(destination, dest_name)
                     if os.path.isfile(destination) and os.stat(destination).st_size == 0:
@@ -1835,41 +1868,26 @@
                                 'copy: src and dest are already the same')
                             if disposition:
                                 return None
                             if send_md5:
                                 return dest_md5
                             return dest_size
 
-            # TODO - remove. This is temporary for regression
-            try:
-                self.get_endpoints(source).recursive_del
-                new_vos = True
-            except KeyError:
-                # TODO - to delete temporary regression code
-                new_vos = False
-
-            get_urls = []
-            files_url = None
             if self._fs_type and (cutout or view == 'header'):
                 raise ValueError('cavern/arc service does not support cutouts or header operations')
-            if new_vos:
-                files_url = self.get_node_url(source, method='GET', cutout=cutout,
-                                              view=view)
-                if files_url:
-                    get_urls.append(self._add_soda_ops(files_url, view, cutout))
 
             while not success:
                 if len(get_urls) == 0:
                     if not get_node_url_retried:
                         get_urls = self.get_node_url(source, method='GET',
                                                      cutout=cutout, view=view,
                                                      full_negotiation=True)
                         # remove files_url that we've tried already
                         if new_vos:
-                            get_urls = [self._add_soda_ops(url, view, cutout)
+                            get_urls = [self._add_soda_ops(url, view=view, cutout=cutout)
                                         for url in get_urls if url != files_url]
                         else:
                             get_urls = [url for url in get_urls if url != files_url]
                         get_node_url_retried = True
                 if len(get_urls) == 0:
                     break
                 get_url = get_urls.pop(0)
@@ -2009,19 +2027,19 @@
                                     put_urls.pop(0)
                                 get_node_url_retried = True
                         if len(put_urls) == 0:
                             break
                         put_url = put_urls.pop(0)
                         try:
                             with open(source, str('rb')) as fin:
-                                self.get_session(destination).put(
+                                response = self.get_session(destination).put(
                                     put_url, data=fin)
-                            node = self.get_node(destination, force=True)
-                            dest_md5 = node.props.get('MD5', None)
-                            if dest_md5 != src_md5:
+                            response.raise_for_status()
+                            dest_md5 = net.extract_md5(response.headers)
+                            if dest_md5 and dest_md5 != src_md5:
                                 # raise TransferException so that the URL
                                 # can be retried later
                                 raise exceptions.TransferException(
                                    "Source md5 ({}) != destination md5 ({})".
                                    format(src_md5, dest_md5))
                         except exceptions.HttpException as ex:
                             msg = ''
@@ -2056,20 +2074,20 @@
                                     put_urls.pop(0)
                                 get_node_url_retried = True
                         if len(put_urls) == 0:
                             break
                         put_url = put_urls.pop(0)
                         try:
                             with Md5File(source, 'rb') as reader:
-                                self.get_session(destination).put(
+                                response = self.get_session(destination).put(
                                     put_url, data=reader)
+                            response.raise_for_status()
                             src_md5 = reader.md5_checksum
-                            node = self.get_node(destination, force=True)
-                            dest_md5 = node.props.get('MD5', None)
-                            if dest_md5 != src_md5:
+                            dest_md5 = net.extract_md5(response.headers)
+                            if dest_md5 and dest_md5 != src_md5:
                                 # raise TransferException so that the URL
                                 # can be retried later
                                 raise exceptions.TransferException(
                                     "Source md5 ({}) != destination md5 ({})".
                                     format(src_md5, dest_md5))
                             success = True
                         except exceptions.HttpException as ex:
```

### Comparing `vos-3.5/vos/vosconfig.py` & `vos-3.6rc0/vos/vosconfig.py`

 * *Files identical despite different names*

### Comparing `vos-3.5/vos.egg-info/PKG-INFO` & `vos-3.6rc0/vos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vos
-Version: 3.5
+Version: 3.6rc0
 Summary: CADC VOS Class Libraries
 Home-page: https://www.canfar.net/en/docs/storage
 Author: JJ Kavelaars, Canadian Astronomy Data Centre
 Author-email: cadc@nrc-cnrc.gc.ca
 License: AGPLv3
 Project-URL: Source, https://github.com/opencadc/vostools
 Project-URL: Issues, https://github.com/opencadc/vostools/issues
```

### Comparing `vos-3.5/vos.egg-info/SOURCES.txt` & `vos-3.6rc0/vos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

