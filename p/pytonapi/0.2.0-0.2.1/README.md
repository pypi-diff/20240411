# Comparing `tmp/pytonapi-0.2.0.tar.gz` & `tmp/pytonapi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytonapi-0.2.0.tar", last modified: Mon Feb 26 22:03:26 2024, max compression
+gzip compressed data, was "pytonapi-0.2.1.tar", last modified: Thu Apr 11 12:57:07 2024, max compression
```

## Comparing `pytonapi-0.2.0.tar` & `pytonapi-0.2.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-02-26 22:03:26.244554 pytonapi-0.2.0/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2024-01-22 06:18:08.000000 pytonapi-0.2.0/LICENSE
--rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-02-26 22:03:26.244554 pytonapi-0.2.0/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     4653 2024-02-17 08:30:09.000000 pytonapi-0.2.0/README.md
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-02-26 22:03:26.224553 pytonapi-0.2.0/pytonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)      129 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/__init__.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-02-26 22:03:26.224553 pytonapi-0.2.0/pytonapi/async_tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     3349 2024-02-26 21:48:42.000000 pytonapi-0.2.0/pytonapi/async_tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     9652 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-02-26 22:03:26.232553 pytonapi-0.2.0/pytonapi/async_tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)      967 2024-02-26 21:46:16.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    14416 2024-02-26 21:47:00.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     9152 2024-02-26 21:58:25.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1655 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4671 2024-02-22 20:46:27.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/emulate.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1347 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/events.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4176 2024-02-26 21:51:20.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/inscriptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1770 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     8021 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/liteserver.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4509 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1791 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/rates.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2399 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/sse.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2455 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/staking.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      476 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/storage.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      895 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      768 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2343 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/wallet.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2349 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/async_tonapi/methods/websocket.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2174 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/exceptions.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-02-26 22:03:26.236553 pytonapi-0.2.0/pytonapi/schema/
--rw-rw-r--   0 ness      (1000) ness      (1000)      678 2024-02-26 21:51:20.000000 pytonapi-0.2.0/pytonapi/schema/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      874 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/schema/_address.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      896 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/schema/_balance.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1787 2024-02-22 20:50:18.000000 pytonapi-0.2.0/pytonapi/schema/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7591 2024-02-22 20:46:27.000000 pytonapi-0.2.0/pytonapi/schema/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      575 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/schema/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      500 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/schema/domains.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6158 2024-02-26 21:07:34.000000 pytonapi-0.2.0/pytonapi/schema/events.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      245 2024-02-26 21:54:06.000000 pytonapi-0.2.0/pytonapi/schema/inscriptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1460 2024-02-22 20:53:09.000000 pytonapi-0.2.0/pytonapi/schema/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1856 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/schema/liteserver.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1164 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/schema/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      369 2024-02-22 20:53:09.000000 pytonapi-0.2.0/pytonapi/schema/rates.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1152 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/schema/staking.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      364 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/schema/storage.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      169 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/schema/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3133 2024-02-22 20:40:44.000000 pytonapi-0.2.0/pytonapi/schema/traces.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-02-26 22:03:26.236553 pytonapi-0.2.0/pytonapi/tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     3028 2024-02-26 21:45:12.000000 pytonapi-0.2.0/pytonapi/tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     8088 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-02-26 22:03:26.244554 pytonapi-0.2.0/pytonapi/tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)      905 2024-02-26 21:45:12.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    14172 2024-02-22 20:57:14.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     8771 2024-02-26 22:03:08.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1592 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4595 2024-02-22 20:46:27.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/emulate.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1310 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/events.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4112 2024-02-26 21:51:20.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/inscriptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1725 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7825 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/liteserver.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4324 2024-02-26 22:00:27.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1680 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/rates.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2313 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/sse.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2325 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/staking.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      448 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/storage.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      855 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      731 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2279 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/tonapi/methods/wallet.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3256 2024-01-22 06:18:08.000000 pytonapi-0.2.0/pytonapi/utils.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-02-26 22:03:26.244554 pytonapi-0.2.0/pytonapi.egg-info/
--rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-02-26 22:03:26.000000 pytonapi-0.2.0/pytonapi.egg-info/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     2165 2024-02-26 22:03:26.000000 pytonapi-0.2.0/pytonapi.egg-info/SOURCES.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-02-26 22:03:26.000000 pytonapi-0.2.0/pytonapi.egg-info/dependency_links.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       45 2024-02-26 22:03:26.000000 pytonapi-0.2.0/pytonapi.egg-info/requires.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        9 2024-02-26 22:03:26.000000 pytonapi-0.2.0/pytonapi.egg-info/top_level.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-02-26 22:03:26.244554 pytonapi-0.2.0/setup.cfg
--rw-rw-r--   0 ness      (1000) ness      (1000)      970 2024-02-26 21:49:40.000000 pytonapi-0.2.0/setup.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-11 12:57:07.921260 pytonapi-0.2.1/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2024-04-04 18:07:04.000000 pytonapi-0.2.1/LICENSE
+-rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-04-11 12:57:07.921260 pytonapi-0.2.1/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4653 2024-04-04 18:07:04.000000 pytonapi-0.2.1/README.md
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-11 12:57:07.913260 pytonapi-0.2.1/pytonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      129 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/__init__.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-11 12:57:07.913260 pytonapi-0.2.1/pytonapi/async_tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3349 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     9652 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-11 12:57:07.917260 pytonapi-0.2.1/pytonapi/async_tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      967 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    14416 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     9152 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1655 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4671 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/emulate.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1347 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/events.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4176 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/inscriptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2633 2024-04-11 12:27:47.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     8021 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/liteserver.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4509 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1791 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2399 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/sse.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2455 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/staking.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      476 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/storage.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      895 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      768 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2343 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/wallet.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2349 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/async_tonapi/methods/websocket.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2174 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/exceptions.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-11 12:57:07.917260 pytonapi-0.2.1/pytonapi/schema/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      678 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      874 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/_address.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      896 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/_balance.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1787 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7591 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      575 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      500 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/domains.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6158 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/events.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      245 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/inscriptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1460 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1856 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/liteserver.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1164 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      369 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1152 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/staking.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      364 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/storage.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      169 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3133 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/schema/traces.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-11 12:57:07.917260 pytonapi-0.2.1/pytonapi/tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3028 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     8088 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-11 12:57:07.921260 pytonapi-0.2.1/pytonapi/tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      905 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    14172 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     8771 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1592 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4595 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/emulate.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1310 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/events.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4112 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/inscriptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2568 2024-04-11 12:29:15.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7825 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/liteserver.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4324 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1680 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2313 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/sse.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2325 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/staking.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      448 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/storage.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      855 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      731 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2279 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/tonapi/methods/wallet.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3256 2024-04-04 18:07:04.000000 pytonapi-0.2.1/pytonapi/utils.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-11 12:57:07.913260 pytonapi-0.2.1/pytonapi.egg-info/
+-rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-04-11 12:57:07.000000 pytonapi-0.2.1/pytonapi.egg-info/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2165 2024-04-11 12:57:07.000000 pytonapi-0.2.1/pytonapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-04-11 12:57:07.000000 pytonapi-0.2.1/pytonapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       45 2024-04-11 12:57:07.000000 pytonapi-0.2.1/pytonapi.egg-info/requires.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        9 2024-04-11 12:57:07.000000 pytonapi-0.2.1/pytonapi.egg-info/top_level.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-04-11 12:57:07.921260 pytonapi-0.2.1/setup.cfg
+-rw-rw-r--   0 ness      (1000) ness      (1000)      970 2024-04-11 12:44:16.000000 pytonapi-0.2.1/setup.py
```

### Comparing `pytonapi-0.2.0/LICENSE` & `pytonapi-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/PKG-INFO` & `pytonapi-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Provide access to indexed TON blockchain.
 Home-page: https://github.com/tonkeeper/pytonapi/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pytonapi-0.2.0/README.md` & `pytonapi-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/__init__.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/client.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/client.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/__init__.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/accounts.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/blockchain.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/dns.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/emulate.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/emulate.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/events.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/events.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/inscriptions.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/inscriptions.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/jettons.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/jettons.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,84 @@
-from pytonapi.async_tonapi.client import AsyncTonapiClient
+from typing import List
+
 from pytonapi.schema.events import Event
-from pytonapi.schema.jettons import JettonInfo, JettonHolders, Jettons
+from pytonapi.tonapi.client import TonapiClient
+
+from pytonapi.schema.jettons import JettonInfo, JettonHolders, Jettons, JettonHolder
 
 
-class JettonsMethod(AsyncTonapiClient):
+class JettonsMethod(TonapiClient):
 
-    async def get_info(self, account_id: str) -> JettonInfo:
+    def get_info(self, account_id: str) -> JettonInfo:
         """
         Get jetton metadata by jetton master address.
 
-        :param account_id: Account ID
-        :return: JettonInfo
+        :param account_id: account ID
+        :return: :class:`JettonInfo`
         """
         method = f"v2/jettons/{account_id}"
-        response = await self._get(method=method)
+        response = self._get(method=method)
 
         return JettonInfo(**response)
 
-    async def get_holders(self, account_id: str) -> JettonHolders:
+    def get_holders(self, account_id: str, limit: int = 1000, offset: int = 0) -> JettonHolders:
         """
         Get jetton's holders.
 
         :param account_id: Account ID
+        :param limit: Default value - 1000
+        :param offset: Default value - 0
         :return: JettonHolders
         """
         method = f"v2/jettons/{account_id}/holders"
-        response = await self._get(method=method)
+        params = {"limit": limit, "offset": offset}
+        response = self._get(method=method, params=params)
 
         return JettonHolders(**response)
 
-    async def get_all_jettons(self, limit: int = 100, offset: int = 0) -> Jettons:
+    def get_all_holders(self, account_id: str) -> JettonHolders:
+        """
+        Get all jetton's holders.
+
+        :param account_id: Account ID
+        :return: :class:`JettonHolders`
+        """
+        jetton_holders: List[JettonHolder] = []
+        offset, limit = 0, 1000
+
+        while True:
+            result = self.get_holders(
+                account_id=account_id, limit=limit, offset=offset,
+            )
+            jetton_holders += result.addresses
+            offset += limit
+
+            if len(result.addresses) != limit:
+                break
+
+        return JettonHolders(addresses=jetton_holders)
+
+    def get_all_jettons(self, limit: int = 100, offset: int = 0) -> Jettons:
         """
         Get a list of all indexed jetton masters in the blockchain.
 
         :param limit: Default value - 100
         :param offset: Default value - 0
         :return: :class:`Jettons`
         """
-        method = "v2/jettons"
+        method = f"v2/jettons"
         params = {"limit": limit, "offset": offset}
-        response = await self._get(method=method, params=params)
+        response = self._get(method=method, params=params)
 
         return Jettons(**response)
 
-    async def get_jetton_transfer_event(self, event_id: str) -> Event:
+    def get_jetton_transfer_event(self, event_id: str) -> Event:
         """
         Get only jetton transfers in the event.
 
         :param event_id: event ID or transaction hash in hex (without 0x) or base64url format
         :return: :class:`Event`
         """
         method = f"v2/events/{event_id}/jettons"
-        response = await self._get(method=method)
+        response = self._get(method=method)
 
         return Event(**response)
```

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/liteserver.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/liteserver.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/nft.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/rates.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/rates.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/sse.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/sse.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/staking.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/staking.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/tonconnect.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/tonconnect.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/traces.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/wallet.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/wallet.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/async_tonapi/methods/websocket.py` & `pytonapi-0.2.1/pytonapi/async_tonapi/methods/websocket.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/exceptions.py` & `pytonapi-0.2.1/pytonapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/schema/__init__.py` & `pytonapi-0.2.1/pytonapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/schema/_address.py` & `pytonapi-0.2.1/pytonapi/schema/_address.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/schema/_balance.py` & `pytonapi-0.2.1/pytonapi/schema/_balance.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/schema/accounts.py` & `pytonapi-0.2.1/pytonapi/schema/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/schema/blockchain.py` & `pytonapi-0.2.1/pytonapi/schema/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/schema/dns.py` & `pytonapi-0.2.1/pytonapi/schema/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/schema/events.py` & `pytonapi-0.2.1/pytonapi/schema/events.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/schema/jettons.py` & `pytonapi-0.2.1/pytonapi/schema/jettons.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/schema/liteserver.py` & `pytonapi-0.2.1/pytonapi/schema/liteserver.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/schema/nft.py` & `pytonapi-0.2.1/pytonapi/schema/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/schema/staking.py` & `pytonapi-0.2.1/pytonapi/schema/staking.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/schema/traces.py` & `pytonapi-0.2.1/pytonapi/schema/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/__init__.py` & `pytonapi-0.2.1/pytonapi/tonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/client.py` & `pytonapi-0.2.1/pytonapi/tonapi/client.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/__init__.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/accounts.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/blockchain.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/dns.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/emulate.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/emulate.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/events.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/events.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/inscriptions.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/inscriptions.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/liteserver.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/liteserver.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/nft.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/rates.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/rates.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/sse.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/sse.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/staking.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/staking.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/tonconnect.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/tonconnect.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/traces.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/tonapi/methods/wallet.py` & `pytonapi-0.2.1/pytonapi/tonapi/methods/wallet.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi/utils.py` & `pytonapi-0.2.1/pytonapi/utils.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/pytonapi.egg-info/PKG-INFO` & `pytonapi-0.2.1/pytonapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Provide access to indexed TON blockchain.
 Home-page: https://github.com/tonkeeper/pytonapi/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pytonapi-0.2.0/pytonapi.egg-info/SOURCES.txt` & `pytonapi-0.2.1/pytonapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.0/setup.py` & `pytonapi-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytonapi",
-    version="0.2.0",
+    version="0.2.1",
     author="nessshon",
     description="Provide access to indexed TON blockchain.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tonkeeper/pytonapi/",
     packages=setuptools.find_packages(exclude=["examples", "tests"]),
     install_requires=[
```

