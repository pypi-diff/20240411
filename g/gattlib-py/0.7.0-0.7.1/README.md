# Comparing `tmp/gattlib-py-0.7.0.tar.gz` & `tmp/gattlib-py-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gattlib-py-0.7.0.tar", last modified: Wed Apr 10 22:47:16 2024, max compression
+gzip compressed data, was "gattlib-py-0.7.1.tar", last modified: Thu Apr 11 20:39:07 2024, max compression
```

## Comparing `gattlib-py-0.7.0.tar` & `gattlib-py-0.7.1.tar`

### file list

```diff
@@ -1,20 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:47:16.328952 gattlib-py-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 22:47:16.328952 gattlib-py-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-10 22:29:34.000000 gattlib-py-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:47:16.324952 gattlib-py-0.7.0/gattlib/
--rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-04-10 22:29:34.000000 gattlib-py-0.7.0/gattlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 22:47:16.000000 gattlib-py-0.7.0/gattlib/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-10 22:29:34.000000 gattlib-py-0.7.0/gattlib/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-04-10 22:29:34.000000 gattlib-py-0.7.0/gattlib/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-10 22:29:34.000000 gattlib-py-0.7.0/gattlib/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-10 22:29:34.000000 gattlib-py-0.7.0/gattlib/gatt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-10 22:29:34.000000 gattlib-py-0.7.0/gattlib/mainloop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-10 22:29:34.000000 gattlib-py-0.7.0/gattlib/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:47:16.328952 gattlib-py-0.7.0/gattlib_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 22:47:16.000000 gattlib-py-0.7.0/gattlib_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-10 22:47:16.000000 gattlib-py-0.7.0/gattlib_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 22:47:16.000000 gattlib-py-0.7.0/gattlib_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-10 22:47:16.000000 gattlib-py-0.7.0/gattlib_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 22:47:16.000000 gattlib-py-0.7.0/gattlib_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 22:47:16.328952 gattlib-py-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-04-10 22:29:34.000000 gattlib-py-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.211399 gattlib-py-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/CrossCompilation.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-11 20:39:07.211399 gattlib-py-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.187399 gattlib-py-0.7.1/bluez/
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.183399 gattlib-py-0.7.1/bluez/bluez4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.191399 gattlib-py-0.7.1/bluez/bluez4/attrib/
+-rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/attrib/att.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/attrib/att.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14820 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/attrib/gatt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/attrib/gatt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/attrib/gattrib.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/attrib/gattrib.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.191399 gattlib-py-0.7.1/bluez/bluez4/btio/
+-rw-r--r--   0 runner    (1001) docker     (127)    29676 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/btio/btio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/btio/btio.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.191399 gattlib-py-0.7.1/bluez/bluez4/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    10884 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/bluetooth.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/bluetooth.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61436 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/hci.c
+-rw-r--r--   0 runner    (1001) docker     (127)    61945 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/hci.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/hci_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/l2cap.h
+-rw-r--r--   0 runner    (1001) docker     (127)   113715 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/sdp.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17273 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/sdp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21697 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/sdp_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/uuid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/uuid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.191399 gattlib-py-0.7.1/bluez/bluez4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/src/log.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/src/log.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.187399 gattlib-py-0.7.1/bluez/bluez5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.191399 gattlib-py-0.7.1/bluez/bluez5/attrib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/att-database.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/att.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/att.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/gatt-service.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27805 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/gatt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/gatt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/gattrib.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/gattrib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/gatttool.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.191399 gattlib-py-0.7.1/bluez/bluez5/btio/
+-rw-r--r--   0 runner    (1001) docker     (127)    37670 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/btio/btio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/btio/btio.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.195399 gattlib-py-0.7.1/bluez/bluez5/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/a2mp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/amp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49250 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/bluetooth.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/bluetooth.h
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/bluez.pc
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/bluez.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/bnep.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/cmtp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    65395 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/hci.c
+-rw-r--r--   0 runner    (1001) docker     (127)    63804 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/hci.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/hci_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/hidp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/l2cap.h
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/libbluetooth-internal.la
+-rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/mgmt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/rfcomm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/sco.h
+-rw-r--r--   0 runner    (1001) docker     (127)   115468 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/sdp.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18250 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/sdp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21725 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/sdp_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/uuid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/uuid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.195399 gattlib-py-0.7.1/bluez/bluez5/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)    78785 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/monitor/bt.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.187399 gattlib-py-0.7.1/bluez/bluez5/profiles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.195399 gattlib-py-0.7.1/bluez/bluez5/profiles/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/profiles/input/uhid_copy.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.195399 gattlib-py-0.7.1/bluez/bluez5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/eir.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/log.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/log.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.203399 gattlib-py-0.7.1/bluez/bluez5/src/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/ad.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/ad.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/att-types.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33357 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/att.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/att.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/btsnoop.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/btsnoop.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15523 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/crypto.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/crypto.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/ecc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/ecc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    73336 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-client.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-client.h
+-rw-r--r--   0 runner    (1001) docker     (127)    39496 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-db.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-db.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-helpers.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37513 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-server.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-server.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/hci-crypto.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/hci-crypto.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10786 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/hci.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/hci.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29458 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/hfp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/hfp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/io-glib.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/io.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/mainloop.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/mainloop.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/mgmt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/mgmt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/pcap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/pcap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/queue.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/ringbuf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/ringbuf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16939 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/tester.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/tester.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/timeout-glib.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/timeout-mainloop.c
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/timeout.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/tty.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/uhid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/uhid.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/util.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/gattlib.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/gattlib_adapter.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16490 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/gattlib_connect.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/gattlib_discover.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/gattlib_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/gattlib_read_write.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.203399 gattlib-py-0.7.1/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_callback_connected_device.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_callback_disconnected_device.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_callback_discovered_device.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_callback_notification_device.c
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_callback_python.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_common_adapter.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_device_state_management.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_eddystone.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.187399 gattlib-py-0.7.1/common/logging_backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.203399 gattlib-py-0.7.1/common/logging_backend/printf/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/logging_backend/printf/gattlib_logging.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.203399 gattlib-py-0.7.1/common/logging_backend/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/logging_backend/python/gattlib_logging.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.203399 gattlib-py-0.7.1/common/logging_backend/syslog/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/logging_backend/syslog/gattlib_logging.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.203399 gattlib-py-0.7.1/common/mainloop/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/mainloop/gattlib_glib_mainloop.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.207399 gattlib-py-0.7.1/dbus/
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.187399 gattlib-py-0.7.1/dbus/bluez5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.207399 gattlib-py-0.7.1/dbus/bluez5/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/bluez5/lib/uuid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/bluez5/lib/uuid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.207399 gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.Adapter1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.Device1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.GattCharacteristic1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.GattDescriptor1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.GattService1.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.207399 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.Adapter1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.Battery1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.Device1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.GattCharacteristic1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.GattDescriptor1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.GattService1.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.207399 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.Adapter1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.Battery1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.Device1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.GattCharacteristic1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.GattDescriptor1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.GattService1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    38771 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib.c
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)    25348 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib_adapter.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib_advertisement.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib_backend.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib_char.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib_notification.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib_stream.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.211399 gattlib-py-0.7.1/gattlib/
+-rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 20:39:07.000000 gattlib-py-0.7.1/gattlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/gatt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/mainloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.211399 gattlib-py-0.7.1/gattlib_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-11 20:39:07.000000 gattlib-py-0.7.1/gattlib_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-11 20:39:07.000000 gattlib-py-0.7.1/gattlib_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:39:07.000000 gattlib-py-0.7.1/gattlib_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-11 20:39:07.000000 gattlib-py-0.7.1/gattlib_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 20:39:07.000000 gattlib-py-0.7.1/gattlib_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.211399 gattlib-py-0.7.1/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    30854 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/include/gattlib.h
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 20:39:07.211399 gattlib-py-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/setup.py
```

### Comparing `gattlib-py-0.7.0/PKG-INFO` & `gattlib-py-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattlib-py
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python wrapper for gattlib library
 Home-page: https://github.com/labapart/gattlib/gattlib-py
 Author: Olivier Martin
 Author-email: olivier@labapart.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gattlib-py-0.7.0/gattlib/__init__.py` & `gattlib-py-0.7.1/gattlib/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,14 +99,24 @@
 #     size_t   data_length;
 # } gattlib_advertisement_data_t;
 class GattlibAdvertisementData(Structure):
     _fields_ = [("uuid", GattlibUuid),
                 ("data", c_void_p),
                 ("data_length", c_size_t)]
 
+# typedef struct {
+# 	uint16_t manufacturer_id;
+# 	uint8_t* data;
+# 	size_t data_size;
+# } gattlib_manufacturer_data_t;
+class GattlibManufacturerData(Structure):
+    _fields_ = [("manufacturer_id", c_ushort),
+                ("data", c_void_p),
+                ("data_size", c_size_t)]
+
 
 # int gattlib_adapter_open(const char* adapter_name, gattlib_adapter_t** adapter);
 gattlib_adapter_open = gattlib.gattlib_adapter_open
 gattlib_adapter_open.argtypes = [c_char_p, POINTER(c_void_p)]
 
 # const char *gattlib_adapter_get_name(gattlib_adapter_t* adapter)
 gattlib_adapter_get_name = gattlib.gattlib_adapter_get_name
@@ -208,21 +218,21 @@
 gattlib_get_rssi_from_mac = gattlib.gattlib_get_rssi_from_mac
 gattlib_get_rssi_from_mac.argtypes = [c_void_p, c_char_p, POINTER(c_int16)]
 
 # int gattlib_get_advertisement_data(gattlib_connection_t *connection,
 # 		 gattlib_advertisement_data_t **advertisement_data, size_t *advertisement_data_count,
 # 		 gattlib_manufacturer_data_t** manufacturer_data, size_t* manufacturer_data_count)
 gattlib_get_advertisement_data = gattlib.gattlib_get_advertisement_data
-gattlib_get_advertisement_data.argtypes = [c_void_p, POINTER(POINTER(GattlibAdvertisementData)), POINTER(c_size_t), POINTER(c_uint16), POINTER(c_void_p), POINTER(c_size_t)]
+gattlib_get_advertisement_data.argtypes = [c_void_p, POINTER(POINTER(GattlibAdvertisementData)), POINTER(c_size_t), POINTER(POINTER(GattlibManufacturerData)), POINTER(c_size_t)]
 
 # int gattlib_get_advertisement_data_from_mac(gattlib_adapter_t* adapter, const char *mac_address,
 #        gattlib_advertisement_data_t **advertisement_data, size_t *advertisement_data_length,
 #        gattlib_manufacturer_data_t** manufacturer_data, size_t* manufacturer_data_count)
 gattlib_get_advertisement_data_from_mac = gattlib.gattlib_get_advertisement_data_from_mac
-gattlib_get_advertisement_data_from_mac.argtypes = [c_void_p, c_char_p, POINTER(POINTER(GattlibAdvertisementData)), POINTER(c_size_t), POINTER(c_uint16), POINTER(c_void_p), POINTER(c_size_t)]
+gattlib_get_advertisement_data_from_mac.argtypes = [c_void_p, c_char_p, POINTER(POINTER(GattlibAdvertisementData)), POINTER(c_size_t), POINTER(POINTER(GattlibManufacturerData)), POINTER(c_size_t)]
 
 # int gattlib_mainloop_python(PyObject *handler, PyObject *user_data)
 gattlib_mainloop = gattlib.gattlib_mainloop_python
 gattlib_mainloop.argtypes = [py_object, py_object]
 
 # void gattlib_free_mem(void *ptr])
 gattlib_free_mem = gattlib.gattlib_free_mem
```

### Comparing `gattlib-py-0.7.0/gattlib/adapter.py` & `gattlib-py-0.7.1/gattlib/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 
 import threading
 from uuid import UUID
 
 from gattlib import *
 from .device import Device
-from .exception import handle_return, AdapterNotOpened
+from .exception import handle_return
 from .uuid import gattlib_uuid_to_int
 
 GATTLIB_DISCOVER_FILTER_USE_UUID = (1 << 0)
 GATTLIB_DISCOVER_FILTER_USE_RSSI = (1 << 1)
 GATTLIB_DISCOVER_FILTER_NOTIFY_CHANGE = (1 << 2)
 
 GATTLIB_EDDYSTONE_TYPE_UID = (1 << 0)
@@ -234,45 +234,49 @@
 
     def gattlib_get_advertisement_data_from_mac(self, mac_address):
         if isinstance(mac_address, str):
             mac_address = mac_address.encode("utf-8")
 
         _advertisement_data = POINTER(GattlibAdvertisementData)()
         _advertisement_data_count = c_size_t(0)
-        _manufacturer_id = c_uint16(0)
-        _manufacturer_data = c_void_p(None)
+        _manufacturer_data = POINTER(GattlibManufacturerData)()
         _manufacturer_data_len = c_size_t(0)
 
         ret = gattlib_get_advertisement_data_from_mac(self._adapter, mac_address,
                                                       byref(_advertisement_data), byref(_advertisement_data_count),
-                                                      byref(_manufacturer_id),
                                                       byref(_manufacturer_data), byref(_manufacturer_data_len))
         handle_return(ret)
 
         advertisement_data = {}
-        manufacturer_data = None
+        manufacturer_data = {}
 
         for i in range(0, _advertisement_data_count.value):
             service_data = _advertisement_data[i]
             uuid = gattlib_uuid_to_int(service_data.uuid)
 
             pointer_type = POINTER(c_byte * service_data.data_length)
             c_bytearray = cast(service_data.data, pointer_type)
 
             data = bytearray(service_data.data_length)
             for i in range(service_data.data_length):
                 data[i] = c_bytearray.contents[i] & 0xFF
 
             advertisement_data[uuid] = data
 
-        if _manufacturer_data_len.value > 0:
-            pointer_type = POINTER(c_byte * _manufacturer_data_len.value)
-            c_bytearray = cast(_manufacturer_data, pointer_type)
+        for i in range(0, _manufacturer_data_len.value):
+            _manufacturer_data = _manufacturer_data[i]
 
-            manufacturer_data = bytearray(_manufacturer_data_len.value)
-            for i in range(_manufacturer_data_len.value):
-                manufacturer_data[i] = c_bytearray.contents[i] & 0xFF
+            pointer_type = POINTER(c_byte * _manufacturer_data.data_size.value)
+            c_bytearray = cast(_manufacturer_data.data, pointer_type)
+
+            data = bytearray(_manufacturer_data.data_size.value)
+            for j in range(_manufacturer_data.data_size.value):
+                data[j] = c_bytearray.contents[j] & 0xFF
+
+            manufacturer_data[_manufacturer_data.manufacturer_id] = data
+
+            gattlib_free_mem(_manufacturer_data.data)
 
         gattlib_free_mem(_advertisement_data)
         gattlib_free_mem(_manufacturer_data)
 
-        return advertisement_data, _manufacturer_id.value, manufacturer_data
+        return advertisement_data, manufacturer_data
```

### Comparing `gattlib-py-0.7.0/gattlib/device.py` & `gattlib-py-0.7.1/gattlib/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,59 +178,62 @@
             self._characteristics[characteristic.short_uuid] = characteristic
 
             logger.debug("Characteristic UUID:0x%x" % characteristic.short_uuid)
 
     def get_advertisement_data(self):
         _advertisement_data = POINTER(GattlibAdvertisementData)()
         _advertisement_data_count = c_size_t(0)
-        _manufacturer_id = c_uint16(0)
-        _manufacturer_data = c_void_p(None)
+        _manufacturer_data = POINTER(GattlibManufacturerData)()
         _manufacturer_data_len = c_size_t(0)
 
         if self._connection is None:
             ret = gattlib_get_advertisement_data_from_mac(self._adapter._adapter, self._addr,
                                                           byref(_advertisement_data), byref(_advertisement_data_count),
-                                                          byref(_manufacturer_id),
                                                           byref(_manufacturer_data), byref(_manufacturer_data_len))
         else:
             ret = gattlib_get_advertisement_data(self._connection,
                                                  byref(_advertisement_data), byref(_advertisement_data_count),
-                                                 byref(_manufacturer_id),
                                                  byref(_manufacturer_data), byref(_manufacturer_data_len))
 
         handle_return(ret)
 
         advertisement_data = {}
-        manufacturer_data = None
+        manufacturer_data = {}
 
         for i in range(0, _advertisement_data_count.value):
             service_data = _advertisement_data[i]
             uuid = gattlib_uuid_to_int(service_data.uuid)
 
             pointer_type = POINTER(c_byte * service_data.data_length)
             c_bytearray = cast(service_data.data, pointer_type)
 
             data = bytearray(service_data.data_length)
             for i in range(service_data.data_length):
                 data[i] = c_bytearray.contents[i] & 0xFF
 
             advertisement_data[uuid] = data
 
-        if _manufacturer_data_len.value > 0:
-            pointer_type = POINTER(c_byte * _manufacturer_data_len.value)
-            c_bytearray = cast(_manufacturer_data, pointer_type)
-
-            manufacturer_data = bytearray(_manufacturer_data_len.value)
-            for i in range(_manufacturer_data_len.value):
-                manufacturer_data[i] = c_bytearray.contents[i] & 0xFF
+        for i in range(0, _manufacturer_data_len.value):
+            _manufacturer_data = _manufacturer_data[i]
+
+            pointer_type = POINTER(c_byte * _manufacturer_data.data_size.value)
+            c_bytearray = cast(_manufacturer_data.data, pointer_type)
+
+            data = bytearray(_manufacturer_data.data_size.value)
+            for j in range(_manufacturer_data.data_size.value):
+                data[j] = c_bytearray.contents[j] & 0xFF
+
+            manufacturer_data[_manufacturer_data.manufacturer_id] = data
+
+            gattlib_free_mem(_manufacturer_data.data)
 
         gattlib_free_mem(_advertisement_data)
         gattlib_free_mem(_manufacturer_data)
 
-        return advertisement_data, _manufacturer_id.value, manufacturer_data
+        return advertisement_data, manufacturer_data
 
     @property
     def services(self):
         if not hasattr(self, '_services'):
             logger.warning("Start GATT discovery implicitly")
             self.discover()
```

### Comparing `gattlib-py-0.7.0/gattlib/exception.py` & `gattlib-py-0.7.1/gattlib/exception.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.0/gattlib/gatt.py` & `gattlib-py-0.7.1/gattlib/gatt.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.0/gattlib/mainloop.py` & `gattlib-py-0.7.1/gattlib/mainloop.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.0/gattlib/uuid.py` & `gattlib-py-0.7.1/gattlib/uuid.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.0/gattlib_py.egg-info/PKG-INFO` & `gattlib-py-0.7.1/gattlib_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattlib-py
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python wrapper for gattlib library
 Home-page: https://github.com/labapart/gattlib/gattlib-py
 Author: Olivier Martin
 Author-email: olivier@labapart.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gattlib-py-0.7.0/setup.py` & `gattlib-py-0.7.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,31 +10,47 @@
 import sys
 from pathlib import Path
 
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext
 import subprocess
 
+SETUP_DIR = os.path.dirname(os.path.realpath(__file__))
+
 # Name of the directory containing the python sources
 python_module_name = "gattlib"
 # Specified where the CMakeLists.txt is located
 native_source_dir = os.environ.get("NATIVE_SOURCE_DIR", ".")
 
 # Retrieve version from GIT
 git_version_command = subprocess.Popen(['git', 'describe', '--abbrev=7', '--dirty', '--always', '--tags'],
                                        stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 stdout, stderr = git_version_command.communicate()
-git_version = stdout.decode('utf-8').strip()
+if git_version_command.returncode == 0:
+    git_version = stdout.decode('utf-8').strip()
+else:
+    git_version = None
 
 #
 # Create '_version.py'
 #
 package_version = os.environ.get('GATTLIB_PY_VERSION', git_version)
-with open(os.path.join("gattlib", "_version.py"), "w") as f:
-    f.write(f"__version__ = \"{package_version}\"\n")
+
+GATTLIB_VERSION_FILE = os.path.join(SETUP_DIR, "gattlib", "_version.py")
+
+# Case we are building from source package
+if package_version is None:
+    with open(GATTLIB_VERSION_FILE, "r") as f:
+        gattlib_version_statement = f.read()
+        res = re.search(r'__version__ = "(.*)"', gattlib_version_statement)
+        package_version = res.group(1)
+
+if package_version:
+    with open(GATTLIB_VERSION_FILE, "w") as f:
+        f.write(f"__version__ = \"{package_version}\"\n")
 
 
 class CMakeExtension(Extension):
     """Custom extension class that allows to specify the root folder of the CMake project."""
     def __init__(self, name, sourcedir='.', **kwa):
         Extension.__init__(self, name, sources=[], **kwa)
         self.sourcedir = os.path.abspath(sourcedir)
@@ -159,15 +175,15 @@
 setup(
     name='gattlib-py',
     version=package_version,
     author="Olivier Martin",
     author_email="olivier@labapart.com",
     description="Python wrapper for gattlib library",
     url="https://github.com/labapart/gattlib/gattlib-py",
-    long_description=open('README.md').read(),
+    long_description=open(os.path.join(SETUP_DIR, 'README.md')).read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'setuptools',
         'PyGObject>=3.44.0'
     ],
     ext_modules=[CMakeExtension(python_module_name, sourcedir=native_source_dir)],
```

