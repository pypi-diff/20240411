# Comparing `tmp/design.plone.policy-5.0.6.tar.gz` & `tmp/design.plone.policy-5.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.policy-5.0.6.tar", last modified: Tue Aug 29 13:07:15 2023, max compression
+gzip compressed data, was "design.plone.policy-5.0.7.tar", last modified: Wed Dec 13 09:24:47 2023, max compression
```

## Comparing `design.plone.policy-5.0.6.tar` & `design.plone.policy-5.0.7.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.143322 design.plone.policy-5.0.6/
--rw-r--r--   0 roman      (502) staff       (20)     5899 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/CHANGES.rst
--rw-r--r--   0 roman      (502) staff       (20)       73 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/CONTRIBUTORS.rst
--rw-r--r--   0 roman      (502) staff       (20)      585 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/DEVELOP.rst
--rw-r--r--   0 roman      (502) staff       (20)    18092 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/LICENSE.GPL
--rw-r--r--   0 roman      (502) staff       (20)      670 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/LICENSE.rst
--rw-r--r--   0 roman      (502) staff       (20)      139 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/MANIFEST.in
--rw-r--r--   0 roman      (502) staff       (20)    19387 2023-08-29 13:07:15.143614 design.plone.policy-5.0.6/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)     7466 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/README.rst
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.130663 design.plone.policy-5.0.6/docs/
--rw-r--r--   0 roman      (502) staff       (20)     7993 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/docs/conf.py
--rw-r--r--   0 roman      (502) staff       (20)       80 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/docs/index.rst
--rw-r--r--   0 roman      (502) staff       (20)       31 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/requirements.txt
--rw-r--r--   0 roman      (502) staff       (20)      367 2023-08-29 13:07:15.144132 design.plone.policy-5.0.6/setup.cfg
--rw-r--r--   0 roman      (502) staff       (20)     2887 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/setup.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.126098 design.plone.policy-5.0.6/src/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.130899 design.plone.policy-5.0.6/src/design/
--rw-r--r--   0 roman      (502) staff       (20)       80 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.133224 design.plone.policy-5.0.6/src/design/plone/
--rw-r--r--   0 roman      (502) staff       (20)       80 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.136033 design.plone.policy-5.0.6/src/design/plone/policy/
--rw-r--r--   0 roman      (502) staff       (20)      173 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.137031 design.plone.policy-5.0.6/src/design/plone/policy/browser/
--rw-r--r--   0 roman      (502) staff       (20)      119 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/browser/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)    19901 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/browser/config.py
--rw-r--r--   0 roman      (502) staff       (20)      540 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/browser/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     5622 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/browser/trasparenza.py
--rw-r--r--   0 roman      (502) staff       (20)     1623 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      398 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/interfaces.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.138048 design.plone.policy-5.0.6/src/design/plone/policy/locales/
--rw-r--r--   0 roman      (502) staff       (20)      611 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/locales/README.rst
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/locales/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/locales/design.plone.policy.pot
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.126855 design.plone.policy-5.0.6/src/design/plone/policy/locales/en/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.138277 design.plone.policy-5.0.6/src/design/plone/policy/locales/en/LC_MESSAGES/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
--rw-r--r--   0 roman      (502) staff       (20)     1748 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/locales/update.py
--rwxr-xr-x   0 roman      (502) staff       (20)      494 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/locales/update.sh
--rw-r--r--   0 roman      (502) staff       (20)      273 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/permissions.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.127200 design.plone.policy-5.0.6/src/design/plone/policy/profiles/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.139618 design.plone.policy-5.0.6/src/design/plone/policy/profiles/default/
--rw-r--r--   0 roman      (502) staff       (20)      584 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/profiles/default/actions.xml
--rw-r--r--   0 roman      (502) staff       (20)      175 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/profiles/default/browserlayer.xml
--rw-r--r--   0 roman      (502) staff       (20)      122 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/profiles/default/catalog.xml
--rw-r--r--   0 roman      (502) staff       (20)     1027 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/profiles/default/metadata.xml
--rw-r--r--   0 roman      (502) staff       (20)     1742 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/profiles/default/registry.xml
--rw-r--r--   0 roman      (502) staff       (20)      341 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/profiles/default/rolemap.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.140082 design.plone.policy-5.0.6/src/design/plone/policy/profiles/uninstall/
--rw-r--r--   0 roman      (502) staff       (20)      122 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 roman      (502) staff       (20)      268 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/profiles/uninstall/registry.xml
--rw-r--r--   0 roman      (502) staff       (20)      311 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/rejectanonymous.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.140496 design.plone.policy-5.0.6/src/design/plone/policy/restapi/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/restapi/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.141129 design.plone.policy-5.0.6/src/design/plone/policy/restapi/bandi_search_filters/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/restapi/bandi_search_filters/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      534 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      996 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/restapi/bandi_search_filters/get.py
--rw-r--r--   0 roman      (502) staff       (20)      250 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/restapi/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.141762 design.plone.policy-5.0.6/src/design/plone/policy/restapi/search_filters/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/restapi/search_filters/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      519 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/restapi/search_filters/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     3831 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/restapi/search_filters/get.py
--rw-r--r--   0 roman      (502) staff       (20)     2342 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/sensitive.py
--rw-r--r--   0 roman      (502) staff       (20)     3306 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/setuphandlers.py
--rw-r--r--   0 roman      (502) staff       (20)     5214 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/testing.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.143118 design.plone.policy-5.0.6/src/design/plone/policy/tests/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/tests/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     4286 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/tests/test_bandi_search_filters_api.py
--rw-r--r--   0 roman      (502) staff       (20)     4625 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/tests/test_initial_structure.py
--rw-r--r--   0 roman      (502) staff       (20)      795 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/tests/test_registry_entries.py
--rw-r--r--   0 roman      (502) staff       (20)     3864 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/tests/test_search_filters_api.py
--rw-r--r--   0 roman      (502) staff       (20)     3720 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/tests/test_setup.py
--rw-r--r--   0 roman      (502) staff       (20)    15231 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/upgrades.py
--rw-r--r--   0 roman      (502) staff       (20)     5699 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/upgrades.zcml
--rw-r--r--   0 roman      (502) staff       (20)    13481 2023-08-29 13:07:14.000000 design.plone.policy-5.0.6/src/design/plone/policy/utils.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-08-29 13:07:15.132993 design.plone.policy-5.0.6/src/design.plone.policy.egg-info/
--rw-r--r--   0 roman      (502) staff       (20)    19387 2023-08-29 13:07:15.000000 design.plone.policy-5.0.6/src/design.plone.policy.egg-info/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)     2700 2023-08-29 13:07:15.000000 design.plone.policy-5.0.6/src/design.plone.policy.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2023-08-29 13:07:15.000000 design.plone.policy-5.0.6/src/design.plone.policy.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (502) staff       (20)       53 2023-08-29 13:07:15.000000 design.plone.policy-5.0.6/src/design.plone.policy.egg-info/entry_points.txt
--rw-r--r--   0 roman      (502) staff       (20)       20 2023-08-29 13:07:15.000000 design.plone.policy-5.0.6/src/design.plone.policy.egg-info/namespace_packages.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2023-08-29 13:07:15.000000 design.plone.policy-5.0.6/src/design.plone.policy.egg-info/not-zip-safe
--rw-r--r--   0 roman      (502) staff       (20)      504 2023-08-29 13:07:15.000000 design.plone.policy-5.0.6/src/design.plone.policy.egg-info/requires.txt
--rw-r--r--   0 roman      (502) staff       (20)        7 2023-08-29 13:07:15.000000 design.plone.policy-5.0.6/src/design.plone.policy.egg-info/top_level.txt
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.252076 design.plone.policy-5.0.7/
+-rw-r--r--   0 filippocampi   (501) staff       (20)     6119 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/CHANGES.rst
+-rw-r--r--   0 filippocampi   (501) staff       (20)       73 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/CONTRIBUTORS.rst
+-rw-r--r--   0 filippocampi   (501) staff       (20)      585 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/DEVELOP.rst
+-rw-r--r--   0 filippocampi   (501) staff       (20)    18092 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/LICENSE.GPL
+-rw-r--r--   0 filippocampi   (501) staff       (20)      670 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/LICENSE.rst
+-rw-r--r--   0 filippocampi   (501) staff       (20)      139 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/MANIFEST.in
+-rw-r--r--   0 filippocampi   (501) staff       (20)    15669 2023-12-13 09:24:47.251710 design.plone.policy-5.0.7/PKG-INFO
+-rw-r--r--   0 filippocampi   (501) staff       (20)     7466 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/README.rst
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.224052 design.plone.policy-5.0.7/docs/
+-rw-r--r--   0 filippocampi   (501) staff       (20)     7993 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/docs/conf.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)       80 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/docs/index.rst
+-rw-r--r--   0 filippocampi   (501) staff       (20)       31 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/requirements.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      367 2023-12-13 09:24:47.252768 design.plone.policy-5.0.7/setup.cfg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2887 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/setup.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.215997 design.plone.policy-5.0.7/src/
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.224573 design.plone.policy-5.0.7/src/design/
+-rw-r--r--   0 filippocampi   (501) staff       (20)       80 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/__init__.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.228896 design.plone.policy-5.0.7/src/design/plone/
+-rw-r--r--   0 filippocampi   (501) staff       (20)       80 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/__init__.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.234503 design.plone.policy-5.0.7/src/design/plone/policy/
+-rw-r--r--   0 filippocampi   (501) staff       (20)      173 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/__init__.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.236731 design.plone.policy-5.0.7/src/design/plone/policy/browser/
+-rw-r--r--   0 filippocampi   (501) staff       (20)      119 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/browser/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)    19901 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/browser/config.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      540 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/browser/configure.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     5622 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/browser/trasparenza.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1623 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/configure.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      398 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/interfaces.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.238945 design.plone.policy-5.0.7/src/design/plone/policy/locales/
+-rw-r--r--   0 filippocampi   (501) staff       (20)      611 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/locales/README.rst
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/locales/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/locales/design.plone.policy.pot
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.217625 design.plone.policy-5.0.7/src/design/plone/policy/locales/en/
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.239394 design.plone.policy-5.0.7/src/design/plone/policy/locales/en/LC_MESSAGES/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1748 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/locales/update.py
+-rwxr-xr-x   0 filippocampi   (501) staff       (20)      494 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/locales/update.sh
+-rw-r--r--   0 filippocampi   (501) staff       (20)      273 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/permissions.zcml
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.218330 design.plone.policy-5.0.7/src/design/plone/policy/profiles/
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.242159 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/
+-rw-r--r--   0 filippocampi   (501) staff       (20)      584 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/actions.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      175 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/browserlayer.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      122 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/catalog.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1027 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/metadata.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1742 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/registry.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      341 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/rolemap.xml
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.243021 design.plone.policy-5.0.7/src/design/plone/policy/profiles/uninstall/
+-rw-r--r--   0 filippocampi   (501) staff       (20)      122 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      268 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/uninstall/registry.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      311 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/rejectanonymous.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.243786 design.plone.policy-5.0.7/src/design/plone/policy/restapi/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/__init__.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.245049 design.plone.policy-5.0.7/src/design/plone/policy/restapi/bandi_search_filters/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/bandi_search_filters/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      534 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      996 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/bandi_search_filters/get.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      250 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/configure.zcml
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.246507 design.plone.policy-5.0.7/src/design/plone/policy/restapi/search_filters/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/search_filters/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      519 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/search_filters/configure.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3611 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/search_filters/get.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2342 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/sensitive.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3499 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/setuphandlers.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     5214 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/testing.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.249389 design.plone.policy-5.0.7/src/design/plone/policy/tests/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/tests/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     4286 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/tests/test_bandi_search_filters_api.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     4625 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/tests/test_initial_structure.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      795 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/tests/test_registry_entries.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     4993 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/tests/test_search_filters_api.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3720 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/tests/test_setup.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)    15231 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/upgrades.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     6017 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/upgrades.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)    13482 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/utils.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.250017 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/
+-rw-r--r--   0 filippocampi   (501) staff       (20)    15669 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/PKG-INFO
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2700 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/SOURCES.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)        1 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/dependency_links.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)       40 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/entry_points.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)       20 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/namespace_packages.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)        1 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/not-zip-safe
+-rw-r--r--   0 filippocampi   (501) staff       (20)      504 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/requires.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)        7 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/top_level.txt
```

### Comparing `design.plone.policy-5.0.6/CHANGES.rst` & `design.plone.policy-5.0.7/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+5.0.7 (2023-12-13)
+------------------
+
+- Update list of non searchable type in io-Comune
+  [lucabel]
+- Do not return section children in @search-filters endpoint if they are types omitted from search results.
+  [cekk]
+
+
 5.0.6 (2023-08-29)
 ------------------
 
 - Fix to 3001 upgrade step.
   [folix-01]
```

### Comparing `design.plone.policy-5.0.6/DEVELOP.rst` & `design.plone.policy-5.0.7/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/LICENSE.GPL` & `design.plone.policy-5.0.7/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/LICENSE.rst` & `design.plone.policy-5.0.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/README.rst` & `design.plone.policy-5.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/docs/conf.py` & `design.plone.policy-5.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/setup.py` & `design.plone.policy-5.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.policy",
-    version="5.0.6",
+    version="5.0.7",
     description="Pacchetto per creare un sito Agid su Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/browser/config.py` & `design.plone.policy-5.0.7/src/design/plone/policy/browser/config.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/browser/configure.zcml` & `design.plone.policy-5.0.7/src/design/plone/policy/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/browser/trasparenza.py` & `design.plone.policy-5.0.7/src/design/plone/policy/browser/trasparenza.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/configure.zcml` & `design.plone.policy-5.0.7/src/design/plone/policy/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/locales/README.rst` & `design.plone.policy-5.0.7/src/design/plone/policy/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/locales/update.py` & `design.plone.policy-5.0.7/src/design/plone/policy/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/profiles/default/actions.xml` & `design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/profiles/default/metadata.xml` & `design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/metadata.xml`

 * *Files 8% similar despite different names*

#### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/profiles/default/metadata.xml` & `design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/metadata.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata>
-  <version>3102</version>
+  <version>3103</version>
   <dependencies>
     <dependency>profile-plone.restapi:default</dependency>
     <dependency>profile-design.plone.contenttypes:default</dependency>
     <dependency>profile-redturtle.volto:default</dependency>
     <dependency>profile-collective.volto.dropdownmenu:default</dependency>
     <dependency>profile-collective.volto.socialsettings:default</dependency>
     <dependency>profile-collective.volto.secondarymenu:default</dependency>
```

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/profiles/default/registry.xml` & `design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml` & `design.plone.policy-5.0.7/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/restapi/bandi_search_filters/get.py` & `design.plone.policy-5.0.7/src/design/plone/policy/restapi/bandi_search_filters/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/restapi/search_filters/configure.zcml` & `design.plone.policy-5.0.7/src/design/plone/policy/restapi/search_filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/restapi/search_filters/get.py` & `design.plone.policy-5.0.7/src/design/plone/policy/restapi/search_filters/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from AccessControl.unauthorized import Unauthorized
 from design.plone.contenttypes.controlpanels.settings import IDesignPloneSettings
 from plone import api
 from plone.registry.interfaces import IRegistry
 from plone.restapi.interfaces import ISerializeToJsonSummary
 from plone.restapi.services import Service
 from Products.CMFPlone.interfaces import ISearchSchema
+from Products.CMFCore.utils import getToolByName
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.i18n import translate
 from zope.interface import implementer
 from zope.publisher.interfaces import IPublishTraverse
 
 import json
@@ -34,54 +35,53 @@
             for t in ptool.getUserFriendlyTypes()
             if t not in types_not_searched
         ]
         return sorted(types, key=lambda k: k["label"])
 
     def reply(self):
         settings = api.portal.get_registry_record(
-            "search_sections",
-            interface=IDesignPloneSettings,
+            "search_sections", interface=IDesignPloneSettings, default="[]"
         )
+        utils = getToolByName(self.context, "plone_utils")
+
         sections = []
-        if settings:
-            settings = json.loads(settings)
-            for setting in settings:
-                items = []
-                for section_settings in setting.get("items") or []:
-                    for uid in section_settings.get("linkUrl") or []:
-                        try:
-                            section = api.content.get(UID=uid)
-                        except Unauthorized:
-                            # private folder
-                            continue
-                        if section:
-                            item_infos = getMultiAdapter(
-                                (section, self.request),
-                                ISerializeToJsonSummary,
-                            )()
-                            children = section.listFolderContents()
-                            if children:
-                                item_infos["items"] = []
-                                for children in section.listFolderContents():
-                                    item_infos["items"].append(
-                                        getMultiAdapter(
-                                            (children, self.request),
-                                            ISerializeToJsonSummary,
-                                        )()
-                                    )
-                            if section_settings.get("title", ""):
-                                item_infos["title"] = section_settings["title"]
-                            items.append(item_infos)
-                if items:
-                    sections.append(
-                        {
-                            "rootPath": setting.get("rootPath", ""),
-                            "items": items,
-                        }
+        for setting in json.loads(settings or "[]"):
+            items = []
+            for section_settings in setting.get("items") or []:
+                for uid in section_settings.get("linkUrl") or []:
+                    try:
+                        section = api.content.get(UID=uid)
+                    except Unauthorized:
+                        # private folder
+                        continue
+                    if not section:
+                        continue
+                    item_infos = getMultiAdapter(
+                        (section, self.request),
+                        ISerializeToJsonSummary,
+                    )()
+                    children = section.listFolderContents(
+                        contentFilter={"portal_type": utils.getUserFriendlyTypes()}
                     )
+                    item_infos["items"] = [
+                        getMultiAdapter(
+                            (x, self.request),
+                            ISerializeToJsonSummary,
+                        )()
+                        for x in children
+                    ]
+                    item_infos["title"] = section_settings.get("title", "")
+                    items.append(item_infos)
+            if items:
+                sections.append(
+                    {
+                        "rootPath": setting.get("rootPath", ""),
+                        "items": items,
+                    }
+                )
         topics = [
             getMultiAdapter(
                 (brain, self.request),
                 ISerializeToJsonSummary,
             )()
             for brain in api.content.find(
                 portal_type="Pagina Argomento",
```

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/sensitive.py` & `design.plone.policy-5.0.7/src/design/plone/policy/sensitive.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/setuphandlers.py` & `design.plone.policy-5.0.7/src/design/plone/policy/setuphandlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,27 +58,35 @@
     disable_searchable_types()
     set_default_subsite_colors()
     create_footer()
     create_menu()
     create_secondary_menu()
 
 
-def disable_searchable_types():
+def disable_searchable_types(context=None):
     # remove some types from search enabled ones
+
+    # This is the list updated at 2023/12/01 with all types that
+    # could not be searchable in io-Comune
+
     registry = getUtility(IRegistry)
     settings = registry.forInterface(ISearchSchema, prefix="plone")
     remove_types = [
         "Folder",
         "Bando Folder Deepening",
         "Link",
         "Collection",
         "Discussion Item",
         "Dataset",
         "Documento Personale",
+        "File",
+        "Image",
+        "Incarico",
         "Messaggio",
+        "Modulo",
         "Pratica",
         "RicevutaPagamento",
     ]
     types = set(settings.types_not_searched)
     types.update(remove_types)
     settings.types_not_searched = tuple(types)
```

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/testing.py` & `design.plone.policy-5.0.7/src/design/plone/policy/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/tests/test_bandi_search_filters_api.py` & `design.plone.policy-5.0.7/src/design/plone/policy/tests/test_bandi_search_filters_api.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/tests/test_initial_structure.py` & `design.plone.policy-5.0.7/src/design/plone/policy/tests/test_initial_structure.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/tests/test_registry_entries.py` & `design.plone.policy-5.0.7/src/design/plone/policy/tests/test_registry_entries.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/tests/test_search_filters_api.py` & `design.plone.policy-5.0.7/src/design/plone/policy/tests/test_search_filters_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -93,7 +93,36 @@
         commit()
 
         response = self.api_session.get("/@search-filters").json()
 
         self.assertIn("portal_types", response)
         types = [x["id"] for x in response["portal_types"]]
         self.assertNotIn("Document", types)
+
+    def test_endpoint_do_not_return_contents_that_are_not_searchable(self):
+        api.content.create(
+            container=self.portal["amministrazione"],
+            type="UnitaOrganizzativa",
+            title="UO Foo",
+            id="uo-foo",
+        )
+        commit()
+
+        response = self.api_session.get("/@search-filters").json()
+        amministrazione = response["sections"][0]["items"][0]
+
+        self.assertEqual("Amministrazione", amministrazione["title"])
+        self.assertEqual(8, len(amministrazione["items"]))
+        self.assertEqual("UO Foo", amministrazione["items"][-1]["title"])
+
+        registry = getUtility(IRegistry)
+        settings = registry.forInterface(ISearchSchema, prefix="plone")
+        settings.types_not_searched = tuple(
+            list(settings.types_not_searched) + ["UnitaOrganizzativa"]
+        )
+        commit()
+
+        response = self.api_session.get("/@search-filters").json()
+        amministrazione = response["sections"][0]["items"][0]
+
+        self.assertEqual("Amministrazione", amministrazione["title"])
+        self.assertEqual(7, len(amministrazione["items"]))
```

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/tests/test_setup.py` & `design.plone.policy-5.0.7/src/design/plone/policy/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/upgrades.py` & `design.plone.policy-5.0.7/src/design/plone/policy/upgrades.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/upgrades.zcml` & `design.plone.policy-5.0.7/src/design/plone/policy/upgrades.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -197,8 +197,18 @@
       destination="3102"
       >
     <genericsetup:upgradeStep
         title="Set plone.base.plone.base.interfaces.syndication.ISiteSyndicationSettings.show_author_info to False"
         handler=".upgrades.update_registry"
         />
   </genericsetup:upgradeSteps>
+  <genericsetup:upgradeSteps
+      profile="design.plone.policy:default"
+      source="3102"
+      destination="3103"
+      >
+    <genericsetup:upgradeStep
+        title="Update not searchable types in io-Comune site"
+        handler=".setuphandlers.disable_searchable_types"
+        />
+  </genericsetup:upgradeSteps>
 </configure>
```

### Comparing `design.plone.policy-5.0.6/src/design/plone/policy/utils.py` & `design.plone.policy-5.0.7/src/design/plone/policy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     {
         "title": "Informativa privacy",
         "type": "Document",
         "data-element": "privacy-policy-link",
     },
     {"title": "Note legali", "type": "Document"},
     {
-        "title": "Dichiarazione di accessiblità",
+        "title": "Dichiarazione di accessibilità",
         "type": "Link",
         "data-element": "accessibility-link",
     },
 ]
 
 
 def folderSubstructureGenerator(title, types=[]):
```

### Comparing `design.plone.policy-5.0.6/src/design.plone.policy.egg-info/SOURCES.txt` & `design.plone.policy-5.0.7/src/design.plone.policy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

