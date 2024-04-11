# Comparing `tmp/dissect.hypervisor-3.9.dev1.tar.gz` & `tmp/dissect.hypervisor-3.9.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.hypervisor-3.9.dev1.tar", last modified: Thu Sep 14 08:08:52 2023, max compression
+gzip compressed data, was "dissect.hypervisor-3.9.dev2.tar", last modified: Wed Sep 20 14:53:33 2023, max compression
```

## Comparing `dissect.hypervisor-3.9.dev1.tar` & `dissect.hypervisor-3.9.dev2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.828341 dissect.hypervisor-3.9.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-09-14 08:08:52.828341 dissect.hypervisor-3.9.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.800341 dissect.hypervisor-3.9.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.808341 dissect.hypervisor-3.9.dev1/dissect/hypervisor/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.808341 dissect.hypervisor-3.9.dev1/dissect/hypervisor/backup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/backup/c_vma.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/backup/c_wim.py
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/backup/vma.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/backup/wim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/backup/xva.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.812341 dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/c_hyperv.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/hyperv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/ovf.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/pvs.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/vbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    12500 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/vmx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.812341 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/c_hdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/c_qcow2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/c_vdi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/c_vhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/c_vhdx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/c_vmdk.py
--rw-r--r--   0 runner    (1001) docker     (127)    13091 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/hdd.py
--rw-r--r--   0 runner    (1001) docker     (127)    20218 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/qcow2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/vdi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/vhd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12606 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/vhdx.py
--rw-r--r--   0 runner    (1001) docker     (127)    18069 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/vmdk.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.816341 dissect.hypervisor-3.9.dev1/dissect/hypervisor/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/tools/envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/tools/vma.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.816341 dissect.hypervisor-3.9.dev1/dissect/hypervisor/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10338 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/util/envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/dissect/hypervisor/util/vmtar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.808341 dissect.hypervisor-3.9.dev1/dissect.hypervisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-09-14 08:08:52.000000 dissect.hypervisor-3.9.dev1/dissect.hypervisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2023-09-14 08:08:52.000000 dissect.hypervisor-3.9.dev1/dissect.hypervisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 08:08:52.000000 dissect.hypervisor-3.9.dev1/dissect.hypervisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-09-14 08:08:52.000000 dissect.hypervisor-3.9.dev1/dissect.hypervisor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-09-14 08:08:52.000000 dissect.hypervisor-3.9.dev1/dissect.hypervisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-14 08:08:52.000000 dissect.hypervisor-3.9.dev1/dissect.hypervisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2023-09-14 08:08:40.000000 dissect.hypervisor-3.9.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-14 08:08:52.828341 dissect.hypervisor-3.9.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.816341 dissect.hypervisor-3.9.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.820341 dissect.hypervisor-3.9.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   325934 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/differencing.avhdx.gz
--rwxr-xr-x   0 runner    (1001) docker     (127)   145940 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/dynamic.vhd.gz
--rwxr-xr-x   0 runner    (1001) docker     (127)   184563 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/dynamic.vhdx.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/encrypted.vmx
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/encryption.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.824341 dissect.hypervisor-3.9.dev1/tests/data/expanding.hdd/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/expanding.hdd/DiskDescriptor.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/expanding.hdd/expanding.hdd
--rw-r--r--   0 runner    (1001) docker     (127)   115232 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/expanding.hdd/expanding.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rwxr-xr-x   0 runner    (1001) docker     (127)   151327 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/fixed.vhd.gz
--rwxr-xr-x   0 runner    (1001) docker     (127)   162126 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/fixed.vhdx.gz
--rw-r--r--   0 runner    (1001) docker     (127)   110592 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/local.tgz.ve
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.824341 dissect.hypervisor-3.9.dev1/tests/data/plain.hdd/
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/plain.hdd/DiskDescriptor.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/plain.hdd/plain.hdd
--rw-r--r--   0 runner    (1001) docker     (127)   114982 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/plain.hdd/plain.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (127)    54881 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/sesparse.vmdk.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.824341 dissect.hypervisor-3.9.dev1/tests/data/split.hdd/
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/split.hdd/DiskDescriptor.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/split.hdd/split.hdd
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/split.hdd/split.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/split.hdd/split.hdd.1.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/split.hdd/split.hdd.2.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/split.hdd/split.hdd.3.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/split.hdd/split.hdd.4.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/split.hdd/split.hdd.5.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (127)    45092 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/test.VMRS
--rw-r--r--   0 runner    (1001) docker     (127)    16897 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/test.vgz
--rw-r--r--   0 runner    (1001) docker     (127)    65107 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/test.vma.gz
--rw-r--r--   0 runner    (1001) docker     (127)    81920 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/data/test.vmcx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 08:08:52.824341 dissect.hypervisor-3.9.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/test_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/test_hdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/test_hyperv.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/test_pvs.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/test_vbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/test_vhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/test_vhdx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/test_vma.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/test_vmdk.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/test_vmtar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tests/test_vmx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-09-14 08:08:34.000000 dissect.hypervisor-3.9.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.851342 dissect.hypervisor-3.9.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-09-20 14:53:33.851342 dissect.hypervisor-3.9.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.827341 dissect.hypervisor-3.9.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.831342 dissect.hypervisor-3.9.dev2/dissect/hypervisor/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.835342 dissect.hypervisor-3.9.dev2/dissect/hypervisor/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/backup/c_vma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/backup/c_wim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/backup/vma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/backup/wim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/backup/xva.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.835342 dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/c_hyperv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17692 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/hyperv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/ovf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/vbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/vmx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.839342 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/c_hdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/c_qcow2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/c_vdi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/c_vhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/c_vhdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/c_vmdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13091 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/hdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20218 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/qcow2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/vdi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/vhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/vhdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18069 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/vmdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.839342 dissect.hypervisor-3.9.dev2/dissect/hypervisor/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/tools/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/tools/vma.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.839342 dissect.hypervisor-3.9.dev2/dissect/hypervisor/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/util/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/dissect/hypervisor/util/vmtar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.831342 dissect.hypervisor-3.9.dev2/dissect.hypervisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-09-20 14:53:33.000000 dissect.hypervisor-3.9.dev2/dissect.hypervisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2023-09-20 14:53:33.000000 dissect.hypervisor-3.9.dev2/dissect.hypervisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-20 14:53:33.000000 dissect.hypervisor-3.9.dev2/dissect.hypervisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-09-20 14:53:33.000000 dissect.hypervisor-3.9.dev2/dissect.hypervisor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2023-09-20 14:53:33.000000 dissect.hypervisor-3.9.dev2/dissect.hypervisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-20 14:53:33.000000 dissect.hypervisor-3.9.dev2/dissect.hypervisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2023-09-20 14:53:22.000000 dissect.hypervisor-3.9.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-20 14:53:33.851342 dissect.hypervisor-3.9.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.843342 dissect.hypervisor-3.9.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.847342 dissect.hypervisor-3.9.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   325934 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/differencing.avhdx.gz
+-rwxr-xr-x   0 runner    (1001) docker     (127)   145940 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/dynamic.vhd.gz
+-rwxr-xr-x   0 runner    (1001) docker     (127)   184563 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/dynamic.vhdx.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/encrypted.vmx
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/encryption.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.847342 dissect.hypervisor-3.9.dev2/tests/data/expanding.hdd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/expanding.hdd/DiskDescriptor.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/expanding.hdd/expanding.hdd
+-rw-r--r--   0 runner    (1001) docker     (127)   115232 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/expanding.hdd/expanding.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rwxr-xr-x   0 runner    (1001) docker     (127)   151327 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/fixed.vhd.gz
+-rwxr-xr-x   0 runner    (1001) docker     (127)   162126 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/fixed.vhdx.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   110592 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/local.tgz.ve
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.847342 dissect.hypervisor-3.9.dev2/tests/data/plain.hdd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/plain.hdd/DiskDescriptor.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/plain.hdd/plain.hdd
+-rw-r--r--   0 runner    (1001) docker     (127)   114982 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/plain.hdd/plain.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    54881 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/sesparse.vmdk.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.847342 dissect.hypervisor-3.9.dev2/tests/data/split.hdd/
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/split.hdd/DiskDescriptor.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/split.hdd/split.hdd
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/split.hdd/split.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/split.hdd/split.hdd.1.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/split.hdd/split.hdd.2.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/split.hdd/split.hdd.3.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/split.hdd/split.hdd.4.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/split.hdd/split.hdd.5.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    45092 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/test.VMRS
+-rw-r--r--   0 runner    (1001) docker     (127)    16897 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/test.vgz
+-rw-r--r--   0 runner    (1001) docker     (127)    65107 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/test.vma.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    81920 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/data/test.vmcx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 14:53:33.847342 dissect.hypervisor-3.9.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/test_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/test_hdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/test_hyperv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/test_pvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/test_vbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/test_vhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/test_vhdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/test_vma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/test_vmdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/test_vmtar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tests/test_vmx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-09-20 14:53:14.000000 dissect.hypervisor-3.9.dev2/tox.ini
```

### Comparing `dissect.hypervisor-3.9.dev1/LICENSE` & `dissect.hypervisor-3.9.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/PKG-INFO` & `dissect.hypervisor-3.9.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.hypervisor
-Version: 3.9.dev1
+Version: 3.9.dev2
 Summary: A Dissect module implementing parsers for various hypervisor disk, backup and configuration files
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.hypervisor
 Project-URL: repository, https://github.com/fox-it/dissect.hypervisor
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.hypervisor-3.9.dev1/README.md` & `dissect.hypervisor-3.9.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/backup/c_vma.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/backup/c_vma.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/backup/c_wim.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/backup/c_wim.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/backup/vma.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/backup/vma.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/backup/xva.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/backup/xva.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/c_hyperv.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/c_hyperv.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/hyperv.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/hyperv.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # References:
 # - VmDataStore.dll
+from __future__ import annotations
 
 import struct
+from collections.abc import ItemsView, KeysView, ValuesView
+from typing import BinaryIO, Optional, Union
 
 from dissect.util.stream import RangeStream
 
 from dissect.hypervisor.descriptor.c_hyperv import (
     KeyDataFlag,
     KeyDataType,
     ObjectEntryType,
@@ -13,37 +16,37 @@
 )
 from dissect.hypervisor.exceptions import InvalidSignature
 
 
 class HyperVFile:
     """HyperVFile implementation.
 
-    I think, technically, the underlying container is called HyperVStorage, and the HyperVFile adds
-    some features on top of that. We just call it HyperVFile for convenience.
+    I think, technically, the underlying container is called ``HyperVStorage``, and the ``HyperVFile`` adds
+    some features on top of that. We just call it ``HyperVFile`` for convenience.
 
-    A HyperVFile has 2 headers, one at 0x0000 and one at 0x1000. The active header is determined
+    A ``HyperVFile`` has 2 headers, one at ``0x0000`` and one at ``0x1000``. The active header is determined
     by a sequence number.
 
     A replay log is located at an offset specified in the header. This replay log functions as a journal
     for changes made to the file. A file is dirty if it contains outstanding entries in the replay log,
     and replaying the specified log entries is necessary. This is not currently implemented.
 
-    An object table seems to be located at 0x2000, but it's unclear if this is always the case. The offset
+    An object table seems to be located at ``0x2000``, but it's unclear if this is always the case. The offset
     might be related to the header size, log size or data alignment. This will need some more research.
     This table contains entries that describe the various "objects" contained within this file. The available
-    types are listed in the ObjectEntryType enum.
+    types are listed in the ``ObjectEntryType`` enum.
 
-    HyperVFile's have a version number, and it looks like there are some slight differences between
+    ``HyperVFile``'s have a version number, and it looks like there are some slight differences between
     different versions. The key tables are at least stored in a different manner, because there's code
     to handle loading them differently, and also to update them to the new format if an old version is
     encountered. However, I haven't seen any files with older versions yet, so we guard this implementation
-    to only version 0x0400 at this time.
+    to only version ``0x0400`` at this time.
     """
 
-    def __init__(self, fh):
+    def __init__(self, fh: BinaryIO):
         self.fh = fh
 
         self.fh.seek(c_hyperv.FIRST_HEADER_OFFSET)
         header1 = c_hyperv.HyperVStorageHeader(self.fh)
         self.fh.seek(c_hyperv.SECOND_HEADER_OFFSET)
         header2 = c_hyperv.HyperVStorageHeader(self.fh)
 
@@ -55,16 +58,16 @@
 
         if self.header.version != 0x400:
             # Need test files to know how the keys are stored.
             raise NotImplementedError(f"Unsupported version: 0x{self.header.version:x}")
 
         self.replay_logs = [HyperVStorageReplayLog(self, self.header.replay_log_offset)]
         self.object_tables = [HyperVStorageObjectTable(self, c_hyperv.OBJECT_TABLE_OFFSET)]
-        self.key_tables = {}
-        self.file_objects = {}
+        self.key_tables: dict[int, list[HyperVStorageKeyTable]] = {}
+        self.file_objects: dict[int, HyperVStorageFileObject] = {}
 
         for object_table in self.object_tables:
             for entry in object_table.entries:
                 if entry.allocated == 0:
                     continue
 
                 if entry.type == ObjectEntryType.ObjectTable:
@@ -99,52 +102,52 @@
 
                 parent = entry.parent
                 if parent:
                     parent.children[entry.key] = entry
                 else:
                     self.root[entry.key] = entry
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> HyperVStorageKeyTableEntry:
         return self.root[key]
 
-    def keys(self):
+    def keys(self) -> KeysView[str]:
         return self.root.keys()
 
-    def items(self):
+    def items(self) -> ItemsView[str, HyperVStorageKeyTableEntry]:
         return self.root.items()
 
-    def values(self):
+    def values(self) -> ValuesView[HyperVStorageKeyTableEntry]:
         return self.root.values()
 
-    def as_dict(self):
+    def as_dict(self) -> dict:
         obj = {}
 
         for key, entry in self.root.items():
             obj[key] = entry.as_dict()
 
         return obj
 
     @property
-    def version(self):
+    def version(self) -> int:
         return self.header.version
 
-    def _align(self, offset):
+    def _align(self, offset: int) -> int:
         remainder = offset % self.header.alignment
         if remainder == 0:
             return offset
         return offset + self.header.alignment - remainder
 
 
 class HyperVStorageReplayLog:
     """The replay log tracks changes in the file.
 
-    Old changes are actually still resident in the log, but not counted in the num_entries field.
+    Old changes are actually still resident in the log, but not counted in the ``num_entries`` field.
     """
 
-    def __init__(self, hyperv_file, offset):
+    def __init__(self, hyperv_file: HyperVFile, offset: int):
         self.file = hyperv_file
         self.offset = offset
 
         self.file.fh.seek(offset)
         self.header = c_hyperv.HyperVStorageReplayLog(self.file.fh)
 
         if self.header.signature != c_hyperv.SIGNATURE_REPLAY_LOG_HEADER:
@@ -156,15 +159,15 @@
 class HyperVStorageObjectTable:
     """The object table tracks all "objects".
 
     Objects are specific blocks in the file that have been designated a specific type.
     For example, the object table can list one or more key tables.
     """
 
-    def __init__(self, hyperv_file, offset):
+    def __init__(self, hyperv_file: HyperVFile, offset: int):
         self.file = hyperv_file
         self.offset = offset
 
         self.file.fh.seek(offset)
         self.header = c_hyperv.HyperVStorageObjectTable(self.file.fh)
 
         if self.header.signature != c_hyperv.SIGNATURE_OBJECT_TABLE_HEADER:
@@ -175,175 +178,176 @@
 
 class HyperVStorageKeyTable:
     """The key table stores key value pairs and their relation to parent keys.
 
     A table has a specific table index and one or more key entries.
     """
 
-    def __init__(self, hyperv_file, offset, size):
+    def __init__(self, hyperv_file: HyperVFile, offset: int, size: int):
         self.file = hyperv_file
         self.offset = offset
         self.size = size
 
         fh = self.file.fh
         fh.seek(offset)
         self.raw = memoryview(fh.read(size))
 
         self.header = c_hyperv.HyperVStorageKeyTable(self.raw)
 
         if self.header.signature != c_hyperv.SIGNATURE_KEY_TABLE_HEADER:
             raise InvalidSignature(f"Invalid key table signature: 0x{self.header.signature:x}")
 
-        self.entries = []
-        self._lookup = {}
+        self.entries: list[HyperVStorageKeyTableEntry] = []
+        self._lookup: dict[int, HyperVStorageKeyTableEntry] = {}
 
         entry_offset = len(c_hyperv.HyperVStorageKeyTable)
         while entry_offset < size:
             entry = HyperVStorageKeyTableEntry(self, entry_offset)
             if entry.size == 0:
                 break
 
             self.entries.append(entry)
             self._lookup[entry_offset] = entry
 
             entry_offset = entry_offset + entry.size
 
     @property
-    def index(self):
+    def index(self) -> int:
         """Return the table index."""
         return self.header.index
 
     @property
-    def sequence_number(self):
+    def sequence_number(self) -> int:
         """Return the table sequence number."""
         return self.header.sequence_number
 
 
 class HyperVStorageKeyTableEntry:
     """Entry in a key table.
 
     The first 16 bytes are a combined flag and type field. The high 8 bits are flags, the low 8 bits are type.
 
-    Only one flag is currently known, which we've called FileObjectPointer. It's the lowest bit of the flag bits.
+    Only one flag is currently known, which we've called ``FileObjectPointer``. It's the lowest bit of the flag bits.
     If this flag is set, it means the value of this entry is located in a file object. File objects pointers are
-    12 bytes and consist of a uint32 size and a uint64 offset value. The offset is the absolute offset into the
+    12 bytes and consist of a ``uint32`` size and a ``uint64`` offset value. The offset is the absolute offset into the
     file. This method is similar to how parent keys are referenced.
 
-    Values are stored in a file object if their size >= 0x800. As only strings and "arrays" are of variable size,
+    Values are stored in a file object if their size >= ``0x800``. As only strings and "arrays" are of variable size,
     these are the only data types that can be stored in file objects.
 
     Data type summary:
 
-    - KeyDataType.Free:
+    - ``KeyDataType.Free``:
         - Allocated but free.
 
-    - KeyDataType.Unknown:
+    - ``KeyDataType.Unknown``:
         - Unknown entry type. Anything greater than 9 and exactly 2 is unknown.
 
-    - KeyDataType.Int:
+    - ``KeyDataType.Int``:
         - Signed 64 bit integer.
 
-    - KeyDataType.UInt:
+    - ``KeyDataType.UInt``:
         - Unsigned 64 bit integer.
 
-    - KeyDataType.Double:
+    - ``KeyDataType.Double``:
         - 64 bit double.
 
-    - KeyDataType.String:
+    - ``KeyDataType.String``:
         - UTF-16-LE encoded string
 
-    - KeyDataType.Array:
+    - ``KeyDataType.Array``:
         - Bytes?
 
-    - KeyDataType.Bool:
+    - ``KeyDataType.Bool``:
         - Boolean encoded as 32 bit integer.
 
-    - KeyDataType.Node:
+    - ``KeyDataType.Node``:
         - Tree nodes. Value size is coded as 8, but actual size is 12.
         - First 8 bytes are unknown, but latter 4 bytes is the insertion sequence number.
     """
 
-    def __init__(self, table, offset):
+    def __init__(self, table: HyperVStorageKeyTable, offset: int):
         self.table = table
         self.offset = offset
         self.header = c_hyperv.HyperVStorageKeyTableEntryHeader(table.raw[offset:])
-        self.children = {}
+        self.children: dict[str, HyperVStorageKeyTableEntry] = {}
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> HyperVStorageKeyTableEntry:
         return self.children[key]
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<HyperVStorageKeyTableEntry type={self.type} size={self.size}>"
 
     @property
-    def parent(self):
+    def parent(self) -> Optional[HyperVStorageKeyTableEntry]:
         """Return the entry parent, if there is any.
 
-        Requires that all key tables are loaded."""
+        Requires that all key tables are loaded.
+        """
         if not self.header.parent_table_idx:
             return None
 
         return self.table.file.key_tables[self.header.parent_table_idx][0]._lookup[self.header.parent_offset]
 
     @property
-    def flags(self):
+    def flags(self) -> int:
         """Return the entry flags."""
         return (self.header.type & 0xFF00) >> 8
 
     @property
-    def type(self):
+    def type(self) -> KeyDataType:
         """Return the entry type."""
         return KeyDataType(self.header.type & 0xFF)
 
     @property
-    def size(self):
+    def size(self) -> int:
         """Return the entry size."""
         return self.header.size
 
     @property
-    def is_file_object_pointer(self):
+    def is_file_object_pointer(self) -> bool:
         """Return whether the value is a file object pointer."""
         return bool(KeyDataFlag(self.flags) & KeyDataFlag.FileObjectPointer)
 
     @property
-    def file_object_pointer(self):
+    def file_object_pointer(self) -> tuple[int, int]:
         """Return the file object pointer information."""
         if not self.is_file_object_pointer:
             raise TypeError(f"KeyTableEntry is not a file object pointer: {self}")
 
         data = self.raw[self.header.data_offset :]
         size, offset = struct.unpack("<IQ", data[:12])
         # We swap the values since that is a bit more logical
         return offset, size
 
     @property
-    def raw(self):
+    def raw(self) -> memoryview:
         """Returns the raw data for this entry."""
         data_offset = self.offset + len(c_hyperv.HyperVStorageKeyTableEntryHeader)
         return self.table.raw[data_offset : self.offset + self.size]
 
     @property
-    def data(self):
+    def data(self) -> memoryview:
         """Returns the data portion for this entry."""
         if self.is_file_object_pointer:
             _, size = self.file_object_pointer
             file_object = self.get_file_object()
             # This memoryview has no purpose, only do it so the return value type is consistent
             return memoryview(file_object.read(size))
         else:
             return self.raw[self.header.data_offset :]
 
     @property
-    def key(self):
+    def key(self) -> str:
         """Returns the key name for this entry."""
         # Subtract 1 for the terminating null byte
         return self.raw.tobytes()[: self.header.data_offset - 1].decode("utf-8")
 
     @property
-    def value(self):
+    def value(self) -> Union[int, bytes, str]:
         """Return a Python native value for this entry."""
         data = self.data
 
         if self.type == KeyDataType.Int:
             return struct.unpack("<q", data[:8])[0]
 
         if self.type == KeyDataType.UInt:
@@ -362,30 +366,30 @@
                 return data.decode("utf-16-le")
             return data
 
         if self.type == KeyDataType.Bool:
             return struct.unpack("<I", data[:4])[0] != 0
 
     @property
-    def data_size(self):
+    def data_size(self) -> int:
         """Return the total amount of data bytes, including the key name.
 
         Reference:
-        - HyperVStorageKeyTableEntry::GetDataSizeInBytes
+            - ``HyperVStorageKeyTableEntry::GetDataSizeInBytes``
         """
         if self.type == KeyDataType.Node:
             return self.header.data_offset + 12
         return self.header.data_offset + self.value_size
 
     @property
-    def value_size(self):
+    def value_size(self) -> int:
         """Return the amount of bytes a value occupies.
 
         Reference:
-        - HyperVStorageKeyTableEntry::GetValueSizeInBytes
+            - ``HyperVStorageKeyTableEntry::GetValueSizeInBytes``
         """
         if self.type == KeyDataType.Free:
             return self.header.size - len(c_hyperv.HyperVStorageKeyTableEntryHeader)
 
         if self.is_file_object_pointer:
             return 12
 
@@ -404,39 +408,39 @@
             return 8
 
         if self.type == KeyDataType.Bool:
             return 4
 
         raise TypeError(f"Unknown data type: {self.type}")
 
-    def keys(self):
+    def keys(self) -> KeysView[int]:
         return self.children.keys()
 
-    def items(self):
+    def items(self) -> ItemsView[int, HyperVStorageKeyTableEntry]:
         return self.children.items()
 
-    def values(self):
+    def values(self) -> ValuesView[HyperVStorageKeyTableEntry]:
         return self.children.values()
 
-    def as_dict(self):
+    def as_dict(self) -> dict:
         if self.type != KeyDataType.Node:
             raise TypeError(f"KeyTableEntry can't be dumped as dictionary: {self.type}")
 
         obj = {}
         for key, child in self.children.items():
             if child.type == KeyDataType.Node:
                 value = child.as_dict()
             else:
                 value = child.value
 
             obj[key] = value
 
         return obj
 
-    def get_file_object(self):
+    def get_file_object(self) -> HyperVStorageFileObject:
         if not self.is_file_object_pointer:
             raise TypeError(f"Entry is not a file object pointer: {self}")
 
         offset, size = self.file_object_pointer
         file_object = self.table.file.file_objects.get(offset)
         if not file_object:
             raise ValueError(f"Unknown file object: 0x{offset:x} (0x{size:x})")
@@ -445,30 +449,30 @@
 
 
 class HyperVStorageFileObject:
     """File object from the object table.
 
     File objects are referenced by their absolute offset in the file. The object table also stores
     a size, but this size will always be aligned with the data alignment of the Hyper-V file.
-    The actual size of the data stored is located in the data portion of the HyperVStorageKeyTableEntry
+    The actual size of the data stored is located in the data portion of the ``HyperVStorageKeyTableEntry``
     that references that file object.
     """
 
-    def __init__(self, hyperv_file, offset, size):
+    def __init__(self, hyperv_file: HyperVFile, offset: int, size: int):
         self.file = hyperv_file
         self.offset = offset
         self.size = size
 
-    def read(self, n=-1):
+    def read(self, n: int = -1) -> bytes:
         if n is not None and n < -1:
             raise ValueError("invalid number of bytes to read")
 
         if n == -1:
             read_length = self.size
         else:
             read_length = min(n, self.size)
 
         self.file.fh.seek(self.offset)
         return self.file.fh.read(read_length)
 
-    def open(self, size=None):
+    def open(self, size: Optional[int] = None) -> BinaryIO:
         return RangeStream(self.file.fh, self.offset, size or self.size)
```

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/ovf.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/ovf.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/pvs.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/pvs.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/vbox.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/vbox.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/descriptor/vmx.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/descriptor/vmx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/c_hdd.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/c_hdd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/c_qcow2.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/c_qcow2.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/c_vdi.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/c_vdi.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/c_vhd.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/c_vhd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/c_vhdx.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/c_vhdx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/c_vmdk.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/c_vmdk.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/hdd.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/hdd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/qcow2.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/qcow2.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/vdi.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/vdi.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/vhd.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/vhd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/vhdx.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/vhdx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/disk/vmdk.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/disk/vmdk.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/tools/envelope.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/tools/envelope.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/tools/vma.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/tools/vma.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/util/envelope.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/util/envelope.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect/hypervisor/util/vmtar.py` & `dissect.hypervisor-3.9.dev2/dissect/hypervisor/util/vmtar.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/dissect.hypervisor.egg-info/PKG-INFO` & `dissect.hypervisor-3.9.dev2/dissect.hypervisor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.hypervisor
-Version: 3.9.dev1
+Version: 3.9.dev2
 Summary: A Dissect module implementing parsers for various hypervisor disk, backup and configuration files
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.hypervisor
 Project-URL: repository, https://github.com/fox-it/dissect.hypervisor
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.hypervisor-3.9.dev1/dissect.hypervisor.egg-info/SOURCES.txt` & `dissect.hypervisor-3.9.dev2/dissect.hypervisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/pyproject.toml` & `dissect.hypervisor-3.9.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/conftest.py` & `dissect.hypervisor-3.9.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/differencing.avhdx.gz` & `dissect.hypervisor-3.9.dev2/tests/data/differencing.avhdx.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/dynamic.vhd.gz` & `dissect.hypervisor-3.9.dev2/tests/data/dynamic.vhd.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/dynamic.vhdx.gz` & `dissect.hypervisor-3.9.dev2/tests/data/dynamic.vhdx.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/encrypted.vmx` & `dissect.hypervisor-3.9.dev2/tests/data/encrypted.vmx`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/expanding.hdd/DiskDescriptor.xml` & `dissect.hypervisor-3.9.dev2/tests/data/expanding.hdd/DiskDescriptor.xml`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/expanding.hdd/expanding.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.9.dev2/tests/data/expanding.hdd/expanding.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/fixed.vhd.gz` & `dissect.hypervisor-3.9.dev2/tests/data/fixed.vhd.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/fixed.vhdx.gz` & `dissect.hypervisor-3.9.dev2/tests/data/fixed.vhdx.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/local.tgz.ve` & `dissect.hypervisor-3.9.dev2/tests/data/local.tgz.ve`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/plain.hdd/DiskDescriptor.xml` & `dissect.hypervisor-3.9.dev2/tests/data/plain.hdd/DiskDescriptor.xml`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/plain.hdd/plain.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.9.dev2/tests/data/plain.hdd/plain.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/sesparse.vmdk.gz` & `dissect.hypervisor-3.9.dev2/tests/data/sesparse.vmdk.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/split.hdd/DiskDescriptor.xml` & `dissect.hypervisor-3.9.dev2/tests/data/split.hdd/DiskDescriptor.xml`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/split.hdd/split.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.9.dev2/tests/data/split.hdd/split.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/split.hdd/split.hdd.1.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.9.dev2/tests/data/split.hdd/split.hdd.1.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/split.hdd/split.hdd.2.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.9.dev2/tests/data/split.hdd/split.hdd.2.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/split.hdd/split.hdd.3.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.9.dev2/tests/data/split.hdd/split.hdd.3.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/split.hdd/split.hdd.4.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.9.dev2/tests/data/split.hdd/split.hdd.4.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/split.hdd/split.hdd.5.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.9.dev2/tests/data/split.hdd/split.hdd.5.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/test.VMRS` & `dissect.hypervisor-3.9.dev2/tests/data/test.VMRS`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/test.vgz` & `dissect.hypervisor-3.9.dev2/tests/data/test.vgz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/test.vma.gz` & `dissect.hypervisor-3.9.dev2/tests/data/test.vma.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/data/test.vmcx` & `dissect.hypervisor-3.9.dev2/tests/data/test.vmcx`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/docs/Makefile` & `dissect.hypervisor-3.9.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/docs/conf.py` & `dissect.hypervisor-3.9.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/test_envelope.py` & `dissect.hypervisor-3.9.dev2/tests/test_envelope.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/test_hdd.py` & `dissect.hypervisor-3.9.dev2/tests/test_hdd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/test_hyperv.py` & `dissect.hypervisor-3.9.dev2/tests/test_hyperv.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/test_pvs.py` & `dissect.hypervisor-3.9.dev2/tests/test_pvs.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/test_vbox.py` & `dissect.hypervisor-3.9.dev2/tests/test_vbox.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/test_vhd.py` & `dissect.hypervisor-3.9.dev2/tests/test_vhd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/test_vhdx.py` & `dissect.hypervisor-3.9.dev2/tests/test_vhdx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/test_vma.py` & `dissect.hypervisor-3.9.dev2/tests/test_vma.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/test_vmdk.py` & `dissect.hypervisor-3.9.dev2/tests/test_vmdk.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/test_vmtar.py` & `dissect.hypervisor-3.9.dev2/tests/test_vmtar.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tests/test_vmx.py` & `dissect.hypervisor-3.9.dev2/tests/test_vmx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.9.dev1/tox.ini` & `dissect.hypervisor-3.9.dev2/tox.ini`

 * *Files identical despite different names*

