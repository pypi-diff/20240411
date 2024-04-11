# Comparing `tmp/pybit-5.6.2.tar.gz` & `tmp/pybit-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybit-5.6.2.tar", last modified: Fri Oct 27 14:21:51 2023, max compression
+gzip compressed data, was "pybit-5.7.0.tar", last modified: Thu Apr 11 17:56:43 2024, max compression
```

## Comparing `pybit-5.6.2.tar` & `pybit-5.7.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-10-27 14:21:51.476743 pybit-5.6.2/
--rw-r--r--   0 uk09002ml   (502) staff       (20)    23997 2023-10-27 14:20:09.000000 pybit-5.6.2/CHANGELOG.md
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1217 2022-05-19 15:36:12.000000 pybit-5.6.2/LICENSE
--rw-r--r--   0 uk09002ml   (502) staff       (20)       83 2021-06-17 15:56:06.000000 pybit-5.6.2/MANIFEST.in
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8093 2023-10-27 14:21:51.477109 pybit-5.6.2/PKG-INFO
--rw-r--r--   0 uk09002ml   (502) staff       (20)     6585 2023-05-19 19:10:45.000000 pybit-5.6.2/README.md
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-10-27 14:21:51.423956 pybit-5.6.2/examples/
--rw-r--r--   0 uk09002ml   (502) staff       (20)     6148 2023-04-18 11:36:33.000000 pybit-5.6.2/examples/.DS_Store
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1143 2023-04-06 11:15:33.000000 pybit-5.6.2/examples/direct_session.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1605 2023-04-26 18:06:01.000000 pybit-5.6.2/examples/http_example_explanatory.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      315 2023-09-18 12:30:54.000000 pybit-5.6.2/examples/http_example_quickstart.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      802 2023-09-25 15:49:57.000000 pybit-5.6.2/examples/http_example_rsa_authentication.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1707 2023-09-25 14:41:53.000000 pybit-5.6.2/examples/my_rsa_private_key.pem
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1861 2023-04-06 11:15:33.000000 pybit-5.6.2/examples/websocket_example_explanatory.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      258 2023-09-18 12:30:54.000000 pybit-5.6.2/examples/websocket_example_quickstart.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      913 2023-09-25 15:49:57.000000 pybit-5.6.2/examples/websocket_example_rsa_authentication.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     2256 2023-04-06 11:15:33.000000 pybit-5.6.2/examples/wrapper_class.py
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-10-27 14:21:51.463002 pybit-5.6.2/pybit/
--rw-r--r--   0 uk09002ml   (502) staff       (20)       18 2023-10-27 14:20:09.000000 pybit-5.6.2/pybit/__init__.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1964 2023-04-06 11:15:33.000000 pybit-5.6.2/pybit/_helpers.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    13824 2023-10-27 14:19:53.000000 pybit-5.6.2/pybit/_http_manager.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     7471 2023-04-26 18:06:01.000000 pybit-5.6.2/pybit/_v5_account.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    15024 2023-10-09 12:35:41.000000 pybit-5.6.2/pybit/_v5_asset.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      530 2023-09-25 15:24:34.000000 pybit-5.6.2/pybit/_v5_broker.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     9442 2023-10-09 12:35:41.000000 pybit-5.6.2/pybit/_v5_market.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      560 2023-09-25 15:24:34.000000 pybit-5.6.2/pybit/_v5_misc.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8543 2023-04-06 11:15:33.000000 pybit-5.6.2/pybit/_v5_position.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     4204 2023-09-25 15:24:34.000000 pybit-5.6.2/pybit/_v5_pre_upgrade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     2826 2023-04-06 11:15:33.000000 pybit-5.6.2/pybit/_v5_spot_leverage_token.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     7479 2023-10-09 12:35:41.000000 pybit-5.6.2/pybit/_v5_spot_margin_trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8521 2023-04-26 18:06:01.000000 pybit-5.6.2/pybit/_v5_trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     6529 2023-10-09 12:35:41.000000 pybit-5.6.2/pybit/_v5_user.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    15447 2023-10-27 14:19:53.000000 pybit-5.6.2/pybit/_websocket_stream.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      694 2023-04-06 11:15:33.000000 pybit-5.6.2/pybit/account.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1860 2023-04-26 18:06:01.000000 pybit-5.6.2/pybit/asset.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      160 2023-09-25 15:24:34.000000 pybit-5.6.2/pybit/broker.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1773 2023-05-19 19:00:49.000000 pybit-5.6.2/pybit/exceptions.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1364 2023-09-25 15:49:57.000000 pybit-5.6.2/pybit/helpers.py
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-10-27 14:21:51.476072 pybit-5.6.2/pybit/legacy/
--rw-r--r--   0 uk09002ml   (502) staff       (20)        0 2023-04-18 15:54:54.000000 pybit-5.6.2/pybit/legacy/__init__.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1966 2023-04-06 11:15:33.000000 pybit-5.6.2/pybit/legacy/_helpers.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    32447 2023-10-18 17:16:19.000000 pybit-5.6.2/pybit/legacy/_http_manager.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    18474 2023-04-06 11:15:33.000000 pybit-5.6.2/pybit/legacy/_websocket_stream.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     9678 2023-04-06 11:15:33.000000 pybit-5.6.2/pybit/legacy/copy_trading.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1302 2023-04-06 11:15:33.000000 pybit-5.6.2/pybit/legacy/exceptions.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    13589 2023-04-06 11:15:33.000000 pybit-5.6.2/pybit/legacy/usdc_options.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    14531 2023-04-06 11:15:33.000000 pybit-5.6.2/pybit/legacy/usdc_perpetual.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      950 2023-10-09 12:35:41.000000 pybit-5.6.2/pybit/market.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      153 2023-09-25 15:24:34.000000 pybit-5.6.2/pybit/misc.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      607 2023-04-06 11:15:33.000000 pybit-5.6.2/pybit/position.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      571 2023-09-25 15:24:34.000000 pybit-5.6.2/pybit/pre_upgrade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      406 2023-04-06 11:15:33.000000 pybit-5.6.2/pybit/spot_leverage_token.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1107 2023-10-09 12:35:41.000000 pybit-5.6.2/pybit/spot_margin_trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      600 2023-04-06 11:15:33.000000 pybit-5.6.2/pybit/trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     9049 2023-09-25 15:24:34.000000 pybit-5.6.2/pybit/unified_trading.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      672 2023-09-25 15:24:34.000000 pybit-5.6.2/pybit/user.py
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-10-27 14:21:51.466861 pybit-5.6.2/pybit.egg-info/
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8093 2023-10-27 14:21:51.000000 pybit-5.6.2/pybit.egg-info/PKG-INFO
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1412 2023-10-27 14:21:51.000000 pybit-5.6.2/pybit.egg-info/SOURCES.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2023-10-27 14:21:51.000000 pybit-5.6.2/pybit.egg-info/dependency_links.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2021-07-09 21:25:55.000000 pybit-5.6.2/pybit.egg-info/not-zip-safe
--rw-r--r--   0 uk09002ml   (502) staff       (20)       50 2023-10-27 14:21:51.000000 pybit-5.6.2/pybit.egg-info/requires.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)        6 2023-10-27 14:21:51.000000 pybit-5.6.2/pybit.egg-info/top_level.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)      131 2023-10-27 14:21:51.478133 pybit-5.6.2/setup.cfg
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1109 2023-10-27 14:20:09.000000 pybit-5.6.2/setup.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2024-04-11 17:56:43.441646 pybit-5.7.0/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    24495 2024-04-11 17:56:31.000000 pybit-5.7.0/CHANGELOG.md
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1217 2022-05-19 15:36:12.000000 pybit-5.7.0/LICENSE
+-rw-r--r--   0 uk09002ml   (502) staff       (20)       83 2021-06-17 15:56:06.000000 pybit-5.7.0/MANIFEST.in
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8093 2024-04-11 17:56:43.443046 pybit-5.7.0/PKG-INFO
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     6585 2023-05-19 19:10:45.000000 pybit-5.7.0/README.md
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2024-04-11 17:56:43.259665 pybit-5.7.0/examples/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     6148 2023-04-18 11:36:33.000000 pybit-5.7.0/examples/.DS_Store
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1143 2023-04-06 11:15:33.000000 pybit-5.7.0/examples/direct_session.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1605 2023-04-26 18:06:01.000000 pybit-5.7.0/examples/http_example_explanatory.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      315 2024-01-30 14:08:35.000000 pybit-5.7.0/examples/http_example_quickstart.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      791 2024-04-11 13:58:34.000000 pybit-5.7.0/examples/http_example_rsa_authentication.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1861 2023-04-06 11:15:33.000000 pybit-5.7.0/examples/websocket_example_explanatory.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      258 2024-01-30 14:56:26.000000 pybit-5.7.0/examples/websocket_example_quickstart.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      903 2024-04-11 13:58:34.000000 pybit-5.7.0/examples/websocket_example_rsa_authentication.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     2256 2023-04-06 11:15:33.000000 pybit-5.7.0/examples/wrapper_class.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2024-04-11 17:56:43.400294 pybit-5.7.0/pybit/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)       18 2024-04-11 17:56:31.000000 pybit-5.7.0/pybit/__init__.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1964 2023-04-06 11:15:33.000000 pybit-5.7.0/pybit/_helpers.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    14233 2024-04-11 13:58:34.000000 pybit-5.7.0/pybit/_http_manager.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     9348 2024-04-11 17:25:30.000000 pybit-5.7.0/pybit/_v5_account.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    15024 2024-04-11 13:58:34.000000 pybit-5.7.0/pybit/_v5_asset.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      530 2023-09-25 15:24:34.000000 pybit-5.7.0/pybit/_v5_broker.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     2932 2024-04-11 13:58:34.000000 pybit-5.7.0/pybit/_v5_institutional_loan.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     9442 2024-04-11 13:58:34.000000 pybit-5.7.0/pybit/_v5_market.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1129 2024-04-11 13:58:34.000000 pybit-5.7.0/pybit/_v5_misc.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8543 2024-04-10 10:35:17.000000 pybit-5.7.0/pybit/_v5_position.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     4204 2023-09-25 15:24:34.000000 pybit-5.7.0/pybit/_v5_pre_upgrade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     2826 2023-04-06 11:15:33.000000 pybit-5.7.0/pybit/_v5_spot_leverage_token.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     7479 2024-04-11 13:58:34.000000 pybit-5.7.0/pybit/_v5_spot_margin_trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8521 2023-04-26 18:06:01.000000 pybit-5.7.0/pybit/_v5_trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     6529 2024-04-11 13:58:34.000000 pybit-5.7.0/pybit/_v5_user.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    16125 2024-04-11 17:34:34.000000 pybit-5.7.0/pybit/_websocket_stream.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      882 2024-04-11 17:25:30.000000 pybit-5.7.0/pybit/account.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1860 2023-04-26 18:06:01.000000 pybit-5.7.0/pybit/asset.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      160 2023-09-25 15:24:34.000000 pybit-5.7.0/pybit/broker.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1773 2023-05-19 19:00:49.000000 pybit-5.7.0/pybit/exceptions.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1364 2023-09-25 15:49:57.000000 pybit-5.7.0/pybit/helpers.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      435 2024-04-11 13:58:34.000000 pybit-5.7.0/pybit/institutional_loan.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2024-04-11 17:56:43.439453 pybit-5.7.0/pybit/legacy/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        0 2023-04-18 15:54:54.000000 pybit-5.7.0/pybit/legacy/__init__.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1966 2023-04-06 11:15:33.000000 pybit-5.7.0/pybit/legacy/_helpers.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    32447 2024-04-11 13:58:34.000000 pybit-5.7.0/pybit/legacy/_http_manager.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    18474 2023-04-06 11:15:33.000000 pybit-5.7.0/pybit/legacy/_websocket_stream.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     9678 2023-04-06 11:15:33.000000 pybit-5.7.0/pybit/legacy/copy_trading.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1302 2023-04-06 11:15:33.000000 pybit-5.7.0/pybit/legacy/exceptions.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    13589 2023-04-06 11:15:33.000000 pybit-5.7.0/pybit/legacy/usdc_options.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    14531 2023-04-06 11:15:33.000000 pybit-5.7.0/pybit/legacy/usdc_perpetual.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      950 2024-04-11 13:58:34.000000 pybit-5.7.0/pybit/market.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      217 2024-04-11 13:58:34.000000 pybit-5.7.0/pybit/misc.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      607 2024-04-10 10:35:17.000000 pybit-5.7.0/pybit/position.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      571 2023-09-25 15:24:34.000000 pybit-5.7.0/pybit/pre_upgrade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      406 2023-04-06 11:15:33.000000 pybit-5.7.0/pybit/spot_leverage_token.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1107 2024-04-11 13:58:34.000000 pybit-5.7.0/pybit/spot_margin_trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      600 2023-04-06 11:15:33.000000 pybit-5.7.0/pybit/trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     9134 2024-04-11 13:58:34.000000 pybit-5.7.0/pybit/unified_trading.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      672 2024-04-10 10:35:17.000000 pybit-5.7.0/pybit/user.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2024-04-11 17:56:43.418475 pybit-5.7.0/pybit.egg-info/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8093 2024-04-11 17:56:43.000000 pybit-5.7.0/pybit.egg-info/PKG-INFO
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1440 2024-04-11 17:56:43.000000 pybit-5.7.0/pybit.egg-info/SOURCES.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2024-04-11 17:56:43.000000 pybit-5.7.0/pybit.egg-info/dependency_links.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2021-07-09 21:25:55.000000 pybit-5.7.0/pybit.egg-info/not-zip-safe
+-rw-r--r--   0 uk09002ml   (502) staff       (20)       37 2024-04-11 17:56:43.000000 pybit-5.7.0/pybit.egg-info/requires.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        6 2024-04-11 17:56:43.000000 pybit-5.7.0/pybit.egg-info/top_level.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      131 2024-04-11 17:56:43.445958 pybit-5.7.0/setup.cfg
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1085 2024-04-11 17:56:31.000000 pybit-5.7.0/setup.py
```

### Comparing `pybit-5.6.2/CHANGELOG.md` & `pybit-5.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,24 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
-## [5.6.2] - 2023-10-27
+## [5.7.0] - 2024-04-11
+### Added
+- [Demo Trading](https://bybit-exchange.github.io/docs/v5/demo) support 
+- Add methods for the [Institutional Loan](https://bybit-exchange.github.io/docs/v5/otc/margin-product-info) endpoints
+- Add [Account](https://bybit-exchange.github.io/docs/v5/account/wallet-balance) methods `repay_liability()`, `set_collateral_coin()`, `batch_set_collateral_coin()`
+- `tld` arg for users in The Netherlands and Hong Kong for `HTTP` sessions
+
 ### Fixed
-- `ModuleNotFoundError: No module named 'Crypto'`
+- Options WebSocket failing to maintain connection (https://github.com/bybit-exchange/pybit/issues/164)
+
 
 ## [5.6.1] - 2023-10-09
 ### Changed
 - Improved the IP rate limit error message to indicate that an HTTP status code 403 may also mean that the IP address was identified as being from the USA – all requests from USA IPs are [banned](https://t.me/BybitAPI/180420) by Bybit.
 
 
 ## [5.6.0] - 2023-09-28
```

### Comparing `pybit-5.6.2/LICENSE` & `pybit-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/PKG-INFO` & `pybit-5.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybit
-Version: 5.6.2
+Version: 5.7.0
 Summary: Python3 Bybit HTTP/WebSocket API Connector
 Home-page: https://github.com/bybit-exchange/pybit
 Author: Dexter Dickinson
 Author-email: dexter.dickinson@bybit.com
 License: MIT License
 Description: # pybit
         <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
```

### Comparing `pybit-5.6.2/README.md` & `pybit-5.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/examples/.DS_Store` & `pybit-5.7.0/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/examples/direct_session.py` & `pybit-5.7.0/examples/direct_session.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/examples/http_example_explanatory.py` & `pybit-5.7.0/examples/http_example_explanatory.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/examples/http_example_rsa_authentication.py` & `pybit-5.7.0/examples/http_example_rsa_authentication.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Learn about RSA authentication here:
 https://www.bybit.com/en-US/help-center/bybitHC_Article?id=000001923&language=en_US
 """
 from pybit.unified_trading import HTTP
 
 # The API key is given to you by Bybit's API management page after inputting
 # your RSA public key.
-api_key = "ZzM49jZjnY6CQla21b"
+api_key = "xxxxxxx"
 # The API secret is your RSA generated private key. It begins with the line:
 # -----BEGIN PRIVATE KEY-----
 with open("my_rsa_private_key.pem", "r") as private_key_file:
     api_secret = private_key_file.read()
 
 session = HTTP(
     testnet=True,
```

### Comparing `pybit-5.6.2/examples/websocket_example_explanatory.py` & `pybit-5.7.0/examples/websocket_example_explanatory.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/examples/websocket_example_rsa_authentication.py` & `pybit-5.7.0/examples/websocket_example_rsa_authentication.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 https://www.bybit.com/en-US/help-center/bybitHC_Article?id=000001923&language=en_US
 """
 from pybit.unified_trading import WebSocket
 from time import sleep
 
 # The API key is given to you by Bybit's API management page after inputting
 # your RSA public key.
-api_key = "ZzM49jZjnY6CQla21b"
+api_key = "xxxxxxxx"
 # The API secret is your RSA generated private key. It begins with the line:
 # -----BEGIN PRIVATE KEY-----
 with open("my_rsa_private_key.pem", "r") as private_key_file:
     api_secret = private_key_file.read()
 
 ws = WebSocket(
     testnet=True,
```

### Comparing `pybit-5.6.2/examples/wrapper_class.py` & `pybit-5.7.0/examples/wrapper_class.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/_helpers.py` & `pybit-5.7.0/pybit/_helpers.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/_http_manager.py` & `pybit-5.7.0/pybit/_http_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,24 @@
 
 # Requests will use simplejson if available.
 try:
     from simplejson.errors import JSONDecodeError
 except ImportError:
     from json.decoder import JSONDecodeError
 
-HTTP_URL = "https://{SUBDOMAIN}.{DOMAIN}.com"
+HTTP_URL = "https://{SUBDOMAIN}.{DOMAIN}.{TLD}"
 SUBDOMAIN_TESTNET = "api-testnet"
 SUBDOMAIN_MAINNET = "api"
+DEMO_SUBDOMAIN_TESTNET = "api-demo-testnet"
+DEMO_SUBDOMAIN_MAINNET = "api-demo"
 DOMAIN_MAIN = "bybit"
 DOMAIN_ALT = "bytick"
+TLD_MAIN = "com"
+TLD_NL = "nl"
+TLD_HK = "com.hk"
 
 
 def generate_signature(use_rsa_authentication, secret, param_str):
     def generate_hmac():
         hash = hmac.new(
             bytes(secret, "utf-8"),
             param_str.encode("utf-8"),
@@ -53,14 +58,16 @@
         return generate_rsa()
 
 
 @dataclass
 class _V5HTTPManager:
     testnet: bool = field(default=False)
     domain: str = field(default=DOMAIN_MAIN)
+    tld: str = field(default=TLD_MAIN)
+    demo: bool = field(default=False)
     rsa_authentication: str = field(default=False)
     api_key: str = field(default=None)
     api_secret: str = field(default=None)
     logging_level: logging = field(default=logging.INFO)
     log_requests: bool = field(default=False)
     timeout: int = field(default=10)
     recv_window: bool = field(default=5000)
@@ -78,15 +85,20 @@
     referral_id: bool = field(default=None)
     record_request_time: bool = field(default=False)
     return_response_headers: bool = field(default=False)
 
     def __post_init__(self):
         subdomain = SUBDOMAIN_TESTNET if self.testnet else SUBDOMAIN_MAINNET
         domain = DOMAIN_MAIN if not self.domain else self.domain
-        url = HTTP_URL.format(SUBDOMAIN=subdomain, DOMAIN=domain)
+        if self.demo:
+            if self.testnet:
+                subdomain = DEMO_SUBDOMAIN_TESTNET
+            else:
+                subdomain = DEMO_SUBDOMAIN_MAINNET
+        url = HTTP_URL.format(SUBDOMAIN=subdomain, DOMAIN=domain, TLD=self.tld)
         self.endpoint = url
 
         if not self.ignore_codes:
             self.ignore_codes = set()
         if not self.retry_codes:
             self.retry_codes = {10002, 10006, 30034, 30035, 130035, 130150}
         self.logger = logging.getLogger(__name__)
@@ -233,26 +245,14 @@
                     "X-BAPI-SIGN-TYPE": "2",
                     "X-BAPI-TIMESTAMP": str(timestamp),
                     "X-BAPI-RECV-WINDOW": str(recv_window),
                 }
             else:
                 headers = {}
 
-            # Log the request.
-            if self.log_requests:
-                if req_params:
-                    self.logger.debug(
-                        f"Request -> {method} {path}. Body: {req_params}. "
-                        f"Headers: {headers}"
-                    )
-                else:
-                    self.logger.debug(
-                        f"Request -> {method} {path}. Headers: {headers}"
-                    )
-
             if method == "GET":
                 if req_params:
                     r = self.client.prepare_request(
                         requests.Request(
                             method, path + f"?{req_params}", headers=headers
                         )
                     )
@@ -262,14 +262,26 @@
                     )
             else:
                 r = self.client.prepare_request(
                     requests.Request(
                         method, path, data=req_params, headers=headers
                     )
                 )
+            
+            # Log the request.
+            if self.log_requests:
+                if req_params:
+                    self.logger.debug(
+                        f"Request -> {method} {path}. Body: {req_params}. "
+                        f"Headers: {r.headers}"
+                    )
+                else:
+                    self.logger.debug(
+                        f"Request -> {method} {path}. Headers: {r.headers}"
+                    )
 
             # Attempt the request.
             try:
                 s = self.client.send(r, timeout=self.timeout)
 
             # If requests fires an error, retry.
             except (
```

### Comparing `pybit-5.6.2/pybit/_v5_account.py` & `pybit-5.7.0/pybit/_v5_position.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,224 +1,248 @@
 from ._http_manager import _V5HTTPManager
-from .account import Account
+from .position import Position
 
 
-class AccountHTTP(_V5HTTPManager):
-    def get_wallet_balance(self, **kwargs):
-        """Obtain wallet balance, query asset information of each currency, and account risk rate information under unified margin mode.
-        By default, currency information with assets or liabilities of 0 is not returned.
+class PositionHTTP(_V5HTTPManager):
+    def get_positions(self, **kwargs):
+        """Query real-time position data, such as position size, cumulative realizedPNL.
 
         Required args:
-            accountType (string): Account type
-                Unified account: UNIFIED
-                Normal account: CONTRACT
+            category (string): Product type
+                Unified account: linear, option
+                Normal account: linear, inverse.
+
+                Please note that category is not involved with business logic
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/account/wallet-balance
+            https://bybit-exchange.github.io/docs/v5/position
         """
         return self._submit_request(
             method="GET",
-            path=f"{self.endpoint}{Account.GET_WALLET_BALANCE}",
+            path=f"{self.endpoint}{Position.GET_POSITIONS}",
             query=kwargs,
             auth=True,
         )
 
-    def upgrade_to_unified_trading_account(self, **kwargs):
-        """Upgrade Unified Account
+    def set_leverage(self, **kwargs):
+        """Set the leverage
+
+        Required args:
+            category (string): Product type
+                Unified account: linear
+                Normal account: linear, inverse.
+
+                Please note that category is not involved with business logic
+            symbol (string): Symbol name
+            buyLeverage (string): [0, max leverage of corresponding risk limit].
+                Note: Under one-way mode, buyLeverage must be the same as sellLeverage
+            sellLeverage (string): [0, max leverage of corresponding risk limit].
+                Note: Under one-way mode, buyLeverage must be the same as sellLeverage
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/account/upgrade-unified-account
+            https://bybit-exchange.github.io/docs/v5/position/leverage
         """
         return self._submit_request(
             method="POST",
-            path=f"{self.endpoint}{Account.UPGRADE_TO_UNIFIED_ACCOUNT}",
+            path=f"{self.endpoint}{Position.SET_LEVERAGE}",
             query=kwargs,
             auth=True,
         )
 
-    def get_borrow_history(self, **kwargs):
-        """Get interest records, sorted in reverse order of creation time.
-
-        Returns:
-            Request results as dictionary.
+    def switch_margin_mode(self, **kwargs):
+        """Select cross margin mode or isolated margin mode
 
-        Additional information:
-            https://bybit-exchange.github.io/docs/v5/account/borrow-history
-        """
-        return self._submit_request(
-            method="GET",
-            path=f"{self.endpoint}{Account.GET_BORROW_HISTORY}",
-            query=kwargs,
-            auth=True,
-        )
+        Required args:
+            category (string): Product type. linear,inverse
 
-    def get_collateral_info(self, **kwargs):
-        """Get the collateral information of the current unified margin account, including loan interest rate, loanable amount, collateral conversion rate, whether it can be mortgaged as margin, etc.
+                Please note that category is not involved with business logicUnified account is not applicable
+            symbol (string): Symbol name
+            tradeMode (integer): 0: cross margin. 1: isolated margin
+            buyLeverage (string): The value must be equal to sellLeverage value
+            sellLeverage (string): The value must be equal to buyLeverage value
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/account/collateral-info
+            https://bybit-exchange.github.io/docs/v5/position/cross-isolate
         """
         return self._submit_request(
-            method="GET",
-            path=f"{self.endpoint}{Account.GET_COLLATERAL_INFO}",
+            method="POST",
+            path=f"{self.endpoint}{Position.SWITCH_MARGIN_MODE}",
             query=kwargs,
             auth=True,
         )
 
-    def get_coin_greeks(self, **kwargs):
-        """Get current account Greeks information
-
-        Returns:
-            Request results as dictionary.
+    def set_tp_sl_mode(self, **kwargs):
+        """Set TP/SL mode to Full or Partial
 
-        Additional information:
-            https://bybit-exchange.github.io/docs/v5/account/coin-greeks
-        """
-        return self._submit_request(
-            method="GET",
-            path=f"{self.endpoint}{Account.GET_COIN_GREEKS}",
-            query=kwargs,
-            auth=True,
-        )
+        Required args:
+            category (string): Product type
+                Unified account: linear
+                Normal account: linear, inverse.
 
-    def get_fee_rates(self, **kwargs):
-        """Get the trading fee rate of derivatives.
+                Please note that category is not involved with business logic
+            symbol (string): Symbol name
+            tpSlMode (string): TP/SL mode. Full,Partial
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/account/fee-rate
+            https://bybit-exchange.github.io/docs/v5/position/tpsl-mode
         """
         return self._submit_request(
-            method="GET",
-            path=f"{self.endpoint}{Account.GET_FEE_RATE}",
+            method="POST",
+            path=f"{self.endpoint}{Position.SET_TP_SL_MODE}",
             query=kwargs,
             auth=True,
         )
 
-    def get_account_info(self, **kwargs):
-        """Query the margin mode configuration of the account.
+    def switch_position_mode(self, **kwargs):
+        """
+        It supports to switch the position mode for USDT perpetual and Inverse futures.
+        If you are in one-way Mode, you can only open one position on Buy or Sell side.
+        If you are in hedge mode, you can open both Buy and Sell side positions simultaneously.
+
+        Required args:
+            category (string): Product type. linear,inverse
+
+                Please note that category is not involved with business logicUnified account is not applicable
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/account/account-info
+            https://bybit-exchange.github.io/docs/v5/position/position-mode
         """
         return self._submit_request(
-            method="GET",
-            path=f"{self.endpoint}{Account.GET_ACCOUNT_INFO}",
+            method="POST",
+            path=f"{self.endpoint}{Position.SWITCH_POSITION_MODE}",
             query=kwargs,
             auth=True,
         )
 
-    def get_transaction_log(self, **kwargs):
-        """Query transaction logs in Unified account.
+    def set_risk_limit(self, **kwargs):
+        """
+        The risk limit will limit the maximum position value you can hold under different margin requirements.
+        If you want to hold a bigger position size, you need more margin. This interface can set the risk limit of a single position.
+        If the order exceeds the current risk limit when placing an order, it will be rejected. Click here to learn more about risk limit.
+
+        Required args:
+            category (string): Product type
+                Unified account: linear
+                Normal account: linear, inverse.
+
+                Please note that category is not involved with business logic
+            symbol (string): Symbol name
+            riskId (integer): Risk limit ID
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/account/transaction-log
+            https://bybit-exchange.github.io/docs/v5/position/set-risk-limit
         """
         return self._submit_request(
-            method="GET",
-            path=f"{self.endpoint}{Account.GET_TRANSACTION_LOG}",
+            method="POST",
+            path=f"{self.endpoint}{Position.SET_RISK_LIMIT}",
             query=kwargs,
             auth=True,
         )
 
-    def set_margin_mode(self, **kwargs):
-        """Default is regular margin mode. This mode is valid for USDT Perp, USDC Perp and USDC Option.
+    def set_trading_stop(self, **kwargs):
+        """Set the take profit, stop loss or trailing stop for the position.
 
         Required args:
-            setMarginMode (string): REGULAR_MARGIN, PORTFOLIO_MARGIN
+            category (string): Product type
+                Unified account: linear
+                Normal account: linear, inverse.
+
+                Please note that category is not involved with business logic
+            symbol (string): Symbol name
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/account/set-margin-mode
+            https://bybit-exchange.github.io/docs/v5/position/trading-stop
         """
         return self._submit_request(
             method="POST",
-            path=f"{self.endpoint}{Account.SET_MARGIN_MODE}",
+            path=f"{self.endpoint}{Position.SET_TRADING_STOP}",
             query=kwargs,
             auth=True,
         )
 
-    def set_mmp(self, **kwargs):
-        """
-        Market Maker Protection (MMP) is an automated mechanism designed to protect market makers (MM) against liquidity risks
-        and over-exposure in the market. It prevents simultaneous trade executions on quotes provided by the MM within a short time span.
-        The MM can automatically pull their quotes if the number of contracts traded for an underlying asset exceeds the configured
-        threshold within a certain time frame. Once MMP is triggered, any pre-existing MMP orders will be automatically canceled,
-        and new orders tagged as MMP will be rejected for a specific duration — known as the frozen period — so that MM can
-        reassess the market and modify the quotes.
+    def set_auto_add_margin(self, **kwargs):
+        """Turn on/off auto-add-margin for isolated margin position
 
         Required args:
-            baseCoin (strin): Base coin
-            window (string): Time window (ms)
-            frozenPeriod (string): Frozen period (ms). "0" means the trade will remain frozen until manually reset
-            qtyLimit (string): Trade qty limit (positive and up to 2 decimal places)
-            deltaLimit (string): Delta limit (positive and up to 2 decimal places)
+            category (string): Product type. linear
+            symbol (string): Symbol name
+            autoAddMargin (integer): Turn on/off. 0: off. 1: on
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/account/set-mmp
+            https://bybit-exchange.github.io/docs/v5/position/add-margin
         """
         return self._submit_request(
             method="POST",
-            path=f"{self.endpoint}{Account.SET_MMP}",
+            path=f"{self.endpoint}{Position.SET_AUTO_ADD_MARGIN}",
             query=kwargs,
             auth=True,
         )
 
-    def reset_mmp(self, **kwargs):
-        """Once the mmp triggered, you can unfreeze the account by this endpoint
+    def get_executions(self, **kwargs):
+        """Query users' execution records, sorted by execTime in descending order
 
         Required args:
-            baseCoin (string): Base coin
+            category (string):
+                Product type Unified account: spot, linear, option
+                Normal account: linear, inverse.
+
+                Please note that category is not involved with business logic
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/account/reset-mmp
+            https://bybit-exchange.github.io/docs/v5/position/execution
         """
         return self._submit_request(
-            method="POST",
-            path=f"{self.endpoint}{Account.RESET_MMP}",
+            method="GET",
+            path=f"{self.endpoint}{Position.GET_EXECUTIONS}",
             query=kwargs,
             auth=True,
         )
 
-    def get_mmp_state(self, **kwargs):
-        """Get MMP state
+    def get_closed_pnl(self, **kwargs):
+        """Query user's closed profit and loss records. The results are sorted by createdTime in descending order.
 
         Required args:
-            baseCoin (string): Base coin
+            category (string):
+                Product type Unified account: linear
+                Normal account: linear, inverse.
+
+                Please note that category is not involved with business logic
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/account/get-mmp-state
+            https://bybit-exchange.github.io/docs/v5/position/close-pnl
         """
         return self._submit_request(
             method="GET",
-            path=f"{self.endpoint}{Account.GET_MMP_STATE}",
+            path=f"{self.endpoint}{Position.GET_CLOSED_PNL}",
             query=kwargs,
             auth=True,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pybit-5.6.2/pybit/_v5_asset.py` & `pybit-5.7.0/pybit/_v5_asset.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/_v5_broker.py` & `pybit-5.7.0/pybit/_v5_broker.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/_v5_market.py` & `pybit-5.7.0/pybit/_v5_market.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/_v5_position.py` & `pybit-5.7.0/pybit/_v5_trade.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,248 +1,244 @@
 from ._http_manager import _V5HTTPManager
-from .position import Position
+from .trade import Trade
 
 
-class PositionHTTP(_V5HTTPManager):
-    def get_positions(self, **kwargs):
-        """Query real-time position data, such as position size, cumulative realizedPNL.
+class TradeHTTP(_V5HTTPManager):
+    def place_order(self, **kwargs):
+        """This method supports to create the order for spot, spot margin, linear perpetual, inverse futures and options.
 
         Required args:
-            category (string): Product type
-                Unified account: linear, option
-                Normal account: linear, inverse.
-
-                Please note that category is not involved with business logic
-
+            category (string): Product type Unified account: spot, linear, optionNormal account: linear, inverse. Please note that category is not involved with business logic
+            symbol (string): Symbol name
+            side (string): Buy, Sell
+            orderType (string): Market, Limit
+            qty (string): Order quantity
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/position
+            https://bybit-exchange.github.io/docs/v5/order/create-order
         """
         return self._submit_request(
-            method="GET",
-            path=f"{self.endpoint}{Position.GET_POSITIONS}",
+            method="POST",
+            path=f"{self.endpoint}{Trade.PLACE_ORDER}",
             query=kwargs,
             auth=True,
         )
 
-    def set_leverage(self, **kwargs):
-        """Set the leverage
+    def amend_order(self, **kwargs):
+        """Unified account covers: Linear contract / Options
+        Normal account covers: USDT perpetual / Inverse perpetual / Inverse futures
 
         Required args:
-            category (string): Product type
-                Unified account: linear
-                Normal account: linear, inverse.
-
-                Please note that category is not involved with business logic
+            category (string): Product type Unified account: spot, linear, optionNormal account: linear, inverse. Please note that category is not involved with business logic
             symbol (string): Symbol name
-            buyLeverage (string): [0, max leverage of corresponding risk limit].
-                Note: Under one-way mode, buyLeverage must be the same as sellLeverage
-            sellLeverage (string): [0, max leverage of corresponding risk limit].
-                Note: Under one-way mode, buyLeverage must be the same as sellLeverage
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/position/leverage
+            https://bybit-exchange.github.io/docs/v5/order/amend-order
         """
         return self._submit_request(
             method="POST",
-            path=f"{self.endpoint}{Position.SET_LEVERAGE}",
+            path=f"{self.endpoint}{Trade.AMEND_ORDER}",
             query=kwargs,
             auth=True,
         )
 
-    def switch_margin_mode(self, **kwargs):
-        """Select cross margin mode or isolated margin mode
+    def cancel_order(self, **kwargs):
+        """Unified account covers: Spot / Linear contract / Options
+        Normal account covers: USDT perpetual / Inverse perpetual / Inverse futures
 
         Required args:
-            category (string): Product type. linear,inverse
-
-                Please note that category is not involved with business logicUnified account is not applicable
+            category (string): Product type Unified account: spot, linear, optionNormal account: linear, inverse. Please note that category is not involved with business logic
             symbol (string): Symbol name
-            tradeMode (integer): 0: cross margin. 1: isolated margin
-            buyLeverage (string): The value must be equal to sellLeverage value
-            sellLeverage (string): The value must be equal to buyLeverage value
+            orderId (string): Order ID. Either orderId or orderLinkId is required
+            orderLinkId (string): User customised order ID. Either orderId or orderLinkId is required
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/position/cross-isolate
+            https://bybit-exchange.github.io/docs/v5/order/cancel-order
         """
         return self._submit_request(
             method="POST",
-            path=f"{self.endpoint}{Position.SWITCH_MARGIN_MODE}",
+            path=f"{self.endpoint}{Trade.CANCEL_ORDER}",
             query=kwargs,
             auth=True,
         )
 
-    def set_tp_sl_mode(self, **kwargs):
-        """Set TP/SL mode to Full or Partial
+    def get_open_orders(self, **kwargs):
+        """Query unfilled or partially filled orders in real-time. To query older order records, please use the order history interface.
 
         Required args:
-            category (string): Product type
-                Unified account: linear
-                Normal account: linear, inverse.
-
-                Please note that category is not involved with business logic
-            symbol (string): Symbol name
-            tpSlMode (string): TP/SL mode. Full,Partial
+            category (string): Product type Unified account: spot, linear, optionNormal account: linear, inverse. Please note that category is not involved with business logic
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/position/tpsl-mode
+            https://bybit-exchange.github.io/docs/v5/order/open-order
         """
         return self._submit_request(
-            method="POST",
-            path=f"{self.endpoint}{Position.SET_TP_SL_MODE}",
+            method="GET",
+            path=f"{self.endpoint}{Trade.GET_OPEN_ORDERS}",
             query=kwargs,
             auth=True,
         )
 
-    def switch_position_mode(self, **kwargs):
-        """
-        It supports to switch the position mode for USDT perpetual and Inverse futures.
-        If you are in one-way Mode, you can only open one position on Buy or Sell side.
-        If you are in hedge mode, you can open both Buy and Sell side positions simultaneously.
+    def cancel_all_orders(self, **kwargs):
+        """Cancel all open orders
 
         Required args:
-            category (string): Product type. linear,inverse
+            category (string): Product type
+                Unified account: spot, linear, option
+                Normal account: linear, inverse.
 
-                Please note that category is not involved with business logicUnified account is not applicable
+                Please note that category is not involved with business logic. If cancel all by baseCoin, it will cancel all linear & inverse orders
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/position/position-mode
+            https://bybit-exchange.github.io/docs/v5/order/cancel-all
         """
         return self._submit_request(
             method="POST",
-            path=f"{self.endpoint}{Position.SWITCH_POSITION_MODE}",
+            path=f"{self.endpoint}{Trade.CANCEL_ALL_ORDERS}",
             query=kwargs,
             auth=True,
         )
 
-    def set_risk_limit(self, **kwargs):
-        """
-        The risk limit will limit the maximum position value you can hold under different margin requirements.
-        If you want to hold a bigger position size, you need more margin. This interface can set the risk limit of a single position.
-        If the order exceeds the current risk limit when placing an order, it will be rejected. Click here to learn more about risk limit.
+    def get_order_history(self, **kwargs):
+        """Query order history. As order creation/cancellation is asynchronous, the data returned from this endpoint may delay.
+        If you want to get real-time order information, you could query this endpoint or rely on the websocket stream (recommended).
 
         Required args:
             category (string): Product type
-                Unified account: linear
+                Unified account: spot, linear, option
                 Normal account: linear, inverse.
 
                 Please note that category is not involved with business logic
-            symbol (string): Symbol name
-            riskId (integer): Risk limit ID
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/position/set-risk-limit
+            https://bybit-exchange.github.io/docs/v5/order/order-list
         """
         return self._submit_request(
-            method="POST",
-            path=f"{self.endpoint}{Position.SET_RISK_LIMIT}",
+            method="GET",
+            path=f"{self.endpoint}{Trade.GET_ORDER_HISTORY}",
             query=kwargs,
             auth=True,
         )
 
-    def set_trading_stop(self, **kwargs):
-        """Set the take profit, stop loss or trailing stop for the position.
+    def place_batch_order(self, **kwargs):
+        """Covers: Option (Unified Account)
 
         Required args:
-            category (string): Product type
-                Unified account: linear
-                Normal account: linear, inverse.
-
-                Please note that category is not involved with business logic
-            symbol (string): Symbol name
+            category (string): Product type. option
+            request (array): Object
+            > symbol (string): Symbol name
+            > side (string): Buy, Sell
+            > orderType (string): Market, Limit
+            > qty (string): Order quantity
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/position/trading-stop
+            https://bybit-exchange.github.io/docs/v5/order/batch-place
         """
         return self._submit_request(
             method="POST",
-            path=f"{self.endpoint}{Position.SET_TRADING_STOP}",
+            path=f"{self.endpoint}{Trade.BATCH_PLACE_ORDER}",
             query=kwargs,
             auth=True,
         )
 
-    def set_auto_add_margin(self, **kwargs):
-        """Turn on/off auto-add-margin for isolated margin position
+    def amend_batch_order(self, **kwargs):
+        """Covers: Option (Unified Account)
 
         Required args:
-            category (string): Product type. linear
-            symbol (string): Symbol name
-            autoAddMargin (integer): Turn on/off. 0: off. 1: on
+            category (string): Product type. option
+            request (array): Object
+            > symbol (string): Symbol name
+            > orderId (string): Order ID. Either orderId or orderLinkId is required
+            > orderLinkId (string): User customised order ID. Either orderId or orderLinkId is required
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/position/add-margin
+            https://bybit-exchange.github.io/docs/v5/order/batch-amend
         """
         return self._submit_request(
             method="POST",
-            path=f"{self.endpoint}{Position.SET_AUTO_ADD_MARGIN}",
+            path=f"{self.endpoint}{Trade.BATCH_AMEND_ORDER}",
             query=kwargs,
             auth=True,
         )
 
-    def get_executions(self, **kwargs):
-        """Query users' execution records, sorted by execTime in descending order
+    def cancel_batch_order(self, **kwargs):
+        """This endpoint allows you to cancel more than one open order in a single request.
 
         Required args:
-            category (string):
-                Product type Unified account: spot, linear, option
-                Normal account: linear, inverse.
+            category (string): Product type. option
+            request (array): Object
+            > symbol (string): Symbol name
 
-                Please note that category is not involved with business logic
+        Returns:
+            Request results as dictionary.
+
+        Additional information:
+            https://bybit-exchange.github.io/docs/v5/order/batch-cancel
+        """
+        return self._submit_request(
+            method="POST",
+            path=f"{self.endpoint}{Trade.BATCH_CANCEL_ORDER}",
+            query=kwargs,
+            auth=True,
+        )
+
+    def get_borrow_quota(self, **kwargs):
+        """Query the qty and amount of borrowable coins in spot account.
+
+        Required args:
+            category (string): Product type. spot
+            symbol (string): Symbol name
+            side (string): Transaction side. Buy,Sell
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/position/execution
+            https://bybit-exchange.github.io/docs/v5/order/spot-borrow-quota
         """
         return self._submit_request(
             method="GET",
-            path=f"{self.endpoint}{Position.GET_EXECUTIONS}",
+            path=f"{self.endpoint}{Trade.GET_BORROW_QUOTA}",
             query=kwargs,
             auth=True,
         )
 
-    def get_closed_pnl(self, **kwargs):
-        """Query user's closed profit and loss records. The results are sorted by createdTime in descending order.
+    def set_dcp(self, **kwargs):
+        """Covers: Option (Unified Account)
 
         Required args:
-            category (string):
-                Product type Unified account: linear
-                Normal account: linear, inverse.
-
-                Please note that category is not involved with business logic
+            timeWindow (integer): Disconnection timing window time. [10, 300], unit: second
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/position/close-pnl
+            https://bybit-exchange.github.io/docs/v5/order/dcp
         """
         return self._submit_request(
-            method="GET",
-            path=f"{self.endpoint}{Position.GET_CLOSED_PNL}",
+            method="POST",
+            path=f"{self.endpoint}{Trade.SET_DCP}",
             query=kwargs,
             auth=True,
         )
```

### Comparing `pybit-5.6.2/pybit/_v5_pre_upgrade.py` & `pybit-5.7.0/pybit/_v5_pre_upgrade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/_v5_spot_leverage_token.py` & `pybit-5.7.0/pybit/_v5_spot_leverage_token.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/_v5_spot_margin_trade.py` & `pybit-5.7.0/pybit/_v5_spot_margin_trade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/_v5_user.py` & `pybit-5.7.0/pybit/_v5_user.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/_websocket_stream.py` & `pybit-5.7.0/pybit/_websocket_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,39 +10,42 @@
 
 
 logger = logging.getLogger(__name__)
 
 
 SUBDOMAIN_TESTNET = "stream-testnet"
 SUBDOMAIN_MAINNET = "stream"
+DEMO_SUBDOMAIN_TESTNET = "stream-demo-testnet"
+DEMO_SUBDOMAIN_MAINNET = "stream-demo"
 DOMAIN_MAIN = "bybit"
 DOMAIN_ALT = "bytick"
 
 
 class _WebSocketManager:
     def __init__(
         self,
         callback_function,
         ws_name,
         testnet,
         domain="",
+        demo=False,
         rsa_authentication=False,
         api_key=None,
         api_secret=None,
         ping_interval=20,
         ping_timeout=10,
         retries=10,
         restart_on_error=True,
         trace_logging=False,
-        private_auth_expire=1
+        private_auth_expire=1,
     ):
         self.testnet = testnet
         self.domain = domain
         self.rsa_authentication = rsa_authentication
-
+        self.demo = demo
         # Set API keys.
         self.api_key = api_key
         self.api_secret = api_secret
 
         self.callback = callback_function
         self.ws_name = ws_name
         if api_key:
@@ -119,14 +122,19 @@
                 self.ws.send(subscription_message)
 
         self.attempting_connection = True
 
         # Set endpoint.
         subdomain = SUBDOMAIN_TESTNET if self.testnet else SUBDOMAIN_MAINNET
         domain = DOMAIN_MAIN if not self.domain else self.domain
+        if self.demo:
+            if self.testnet:
+                subdomain = DEMO_SUBDOMAIN_TESTNET
+            else:
+                subdomain = DEMO_SUBDOMAIN_MAINNET
         url = url.format(SUBDOMAIN=subdomain, DOMAIN=domain)
         self.endpoint = url
 
         # Attempt to connect for X seconds.
         retries = self.retries
         if retries == 0:
             infinitely_reconnect = True
@@ -175,14 +183,15 @@
         logger.info(f"WebSocket {self.ws_name} connected")
 
         # If given an api_key, authenticate.
         if self.api_key and self.api_secret:
             self._auth()
 
         resubscribe_to_topics()
+        self._send_initial_ping()
 
         self.attempting_connection = False
 
     def _auth(self):
         """
         Prepares authentication signature per Bybit API specifications.
         """
@@ -244,14 +253,21 @@
         a normal OPCODE_TEXT message and not an OPCODE_PING.
         """
         self._send_custom_ping()
 
     def _send_custom_ping(self):
         self.ws.send(self.custom_ping_message)
 
+    def _send_initial_ping(self):
+        """https://github.com/bybit-exchange/pybit/issues/164"""
+        timer = threading.Timer(
+            self.ping_interval, self._send_custom_ping
+        )
+        timer.start()
+
     @staticmethod
     def _is_custom_pong(message):
         """
         Referring to OPCODE_TEXT pongs from Bybit, not OPCODE_PONG.
         """
         if message.get("ret_msg") == "pong" or message.get("op") == "pong":
             return True
@@ -348,14 +364,16 @@
         # Record the initial snapshot.
         if "snapshot" in message["type"]:
             self.data[topic] = message["data"]
             return
 
         # Make updates according to delta response.
         book_sides = {"b": message["data"]["b"], "a": message["data"]["a"]}
+        self.data[topic]["u"]=message["data"]["u"]
+        self.data[topic]["seq"]=message["data"]["seq"]
 
         for side, entries in book_sides.items():
             for entry in entries:
                 # Delete.
                 if float(entry[1]) == 0:
                     index = _helpers.find_index(
                         self.data[topic][side], entry, 0
@@ -401,15 +419,15 @@
         if message.get("success") is True:
             logger.debug(f"Authorization for {self.ws_name} successful.")
             self.auth = True
         # If we get unsuccessful auth, notify user.
         elif message.get("success") is False or message.get("type") == "error":
             raise Exception(
                 f"Authorization for {self.ws_name} failed. Please check your "
-                f"API keys and restart. Raw error: {message}"
+                f"API keys and resync your system time. Raw error: {message}"
             )
 
     def _process_subscription_message(self, message):
         if message.get("req_id"):
             sub = self.subscriptions[message["req_id"]]
         else:
             # if req_id is not supported, guess that the last subscription
```

### Comparing `pybit-5.6.2/pybit/account.py` & `pybit-5.7.0/pybit/account.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from enum import Enum
 
 
 class Account(str, Enum):
     GET_WALLET_BALANCE = "/v5/account/wallet-balance"
     UPGRADE_TO_UNIFIED_ACCOUNT = "/v5/account/upgrade-to-uta"
     GET_BORROW_HISTORY = "/v5/account/borrow-history"
+    REPAY_LIABILITY = "/v5/account/quick-repayment"
     GET_COLLATERAL_INFO = "/v5/account/collateral-info"
+    SET_COLLATERAL_COIN = "/v5/account/set-collateral-switch"
+    BATCH_SET_COLLATERAL_COIN = "/v5/account/set-collateral-switch-batch"
     GET_COIN_GREEKS = "/v5/asset/coin-greeks"
     GET_FEE_RATE = "/v5/account/fee-rate"
     GET_ACCOUNT_INFO = "/v5/account/info"
     GET_TRANSACTION_LOG = "/v5/account/transaction-log"
     SET_MARGIN_MODE = "/v5/account/set-margin-mode"
     SET_MMP = "/v5/account/mmp-modify"
     RESET_MMP = "/v5/account/mmp-reset"
```

### Comparing `pybit-5.6.2/pybit/asset.py` & `pybit-5.7.0/pybit/asset.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/exceptions.py` & `pybit-5.7.0/pybit/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/helpers.py` & `pybit-5.7.0/pybit/helpers.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/legacy/_helpers.py` & `pybit-5.7.0/pybit/legacy/_helpers.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/legacy/_http_manager.py` & `pybit-5.7.0/pybit/legacy/_http_manager.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/legacy/_websocket_stream.py` & `pybit-5.7.0/pybit/legacy/_websocket_stream.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/legacy/copy_trading.py` & `pybit-5.7.0/pybit/legacy/copy_trading.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/legacy/exceptions.py` & `pybit-5.7.0/pybit/legacy/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/legacy/usdc_options.py` & `pybit-5.7.0/pybit/legacy/usdc_options.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/legacy/usdc_perpetual.py` & `pybit-5.7.0/pybit/legacy/usdc_perpetual.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/market.py` & `pybit-5.7.0/pybit/market.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/position.py` & `pybit-5.7.0/pybit/position.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/pre_upgrade.py` & `pybit-5.7.0/pybit/pre_upgrade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/spot_margin_trade.py` & `pybit-5.7.0/pybit/spot_margin_trade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/trade.py` & `pybit-5.7.0/pybit/trade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit/unified_trading.py` & `pybit-5.7.0/pybit/unified_trading.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ._v5_asset import AssetHTTP
 from ._v5_position import PositionHTTP
 from ._v5_pre_upgrade import PreUpgradeHTTP
 from ._v5_spot_leverage_token import SpotLeverageHTTP
 from ._v5_spot_margin_trade import SpotMarginTradeHTTP
 from ._v5_user import UserHTTP
 from ._v5_broker import BrokerHTTP
+from ._v5_institutional_loan import InstitutionalLoanHTTP
 from ._websocket_stream import _V5WebSocketManager
 
 
 WSS_NAME = "Unified V5"
 PRIVATE_WSS = "wss://{SUBDOMAIN}.{DOMAIN}.com/v5/private"
 PUBLIC_WSS = "wss://{SUBDOMAIN}.{DOMAIN}.com/v5/public/{CHANNEL_TYPE}"
 AVAILABLE_CHANNEL_TYPES = [
@@ -39,14 +40,15 @@
     AssetHTTP,
     PositionHTTP,
     PreUpgradeHTTP,
     SpotLeverageHTTP,
     SpotMarginTradeHTTP,
     UserHTTP,
     BrokerHTTP,
+    InstitutionalLoanHTTP,
 ):
     def __init__(self, **args):
         super().__init__(**args)
 
 
 class WebSocket(_V5WebSocketManager):
     def _validate_public_topic(self):
```

### Comparing `pybit-5.6.2/pybit/user.py` & `pybit-5.7.0/pybit/user.py`

 * *Files identical despite different names*

### Comparing `pybit-5.6.2/pybit.egg-info/PKG-INFO` & `pybit-5.7.0/pybit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybit
-Version: 5.6.2
+Version: 5.7.0
 Summary: Python3 Bybit HTTP/WebSocket API Connector
 Home-page: https://github.com/bybit-exchange/pybit
 Author: Dexter Dickinson
 Author-email: dexter.dickinson@bybit.com
 License: MIT License
 Description: # pybit
         <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
```

### Comparing `pybit-5.6.2/pybit.egg-info/SOURCES.txt` & `pybit-5.7.0/pybit.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,39 +5,40 @@
 setup.cfg
 setup.py
 examples/.DS_Store
 examples/direct_session.py
 examples/http_example_explanatory.py
 examples/http_example_quickstart.py
 examples/http_example_rsa_authentication.py
-examples/my_rsa_private_key.pem
 examples/websocket_example_explanatory.py
 examples/websocket_example_quickstart.py
 examples/websocket_example_rsa_authentication.py
 examples/wrapper_class.py
 pybit/__init__.py
 pybit/_helpers.py
 pybit/_http_manager.py
 pybit/_v5_account.py
 pybit/_v5_asset.py
 pybit/_v5_broker.py
+pybit/_v5_institutional_loan.py
 pybit/_v5_market.py
 pybit/_v5_misc.py
 pybit/_v5_position.py
 pybit/_v5_pre_upgrade.py
 pybit/_v5_spot_leverage_token.py
 pybit/_v5_spot_margin_trade.py
 pybit/_v5_trade.py
 pybit/_v5_user.py
 pybit/_websocket_stream.py
 pybit/account.py
 pybit/asset.py
 pybit/broker.py
 pybit/exceptions.py
 pybit/helpers.py
+pybit/institutional_loan.py
 pybit/market.py
 pybit/misc.py
 pybit/position.py
 pybit/pre_upgrade.py
 pybit/spot_leverage_token.py
 pybit/spot_margin_trade.py
 pybit/trade.py
```

### Comparing `pybit-5.6.2/setup.py` & `pybit-5.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pybit',
-    version='5.6.2',
+    version='5.7.0',
     description='Python3 Bybit HTTP/WebSocket API Connector', 
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bybit-exchange/pybit",
     license="MIT License",
     author="Dexter Dickinson",
     author_email="dexter.dickinson@bybit.com",
@@ -27,10 +27,9 @@
     keywords="bybit api connector",
     packages=["pybit", "pybit.legacy"],
     python_requires=">=3.6",
     install_requires=[
         "requests",
         "websocket-client",
         "websockets",
-        "pycryptodome",
     ],
 )
```

