# Comparing `tmp/quantrocket-moonshot-2.8.0.1.tar.gz` & `tmp/quantrocket-moonshot-2.9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/tmpsnudz2lp/quantrocket-moonshot-2.8.0.1.tar", last modified: Tue Oct 11 13:07:28 2022, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/tmpj8robro5/quantrocket-moonshot-2.9.0.0.tar", last modified: Tue Apr  4 14:56:09 2023, max compression
```

## Comparing `quantrocket-moonshot-2.8.0.1.tar` & `quantrocket-moonshot-2.9.0.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     9144 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/LICENSE.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/moonshot/
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/moonshot/slippage/
--rw-rw-rw-   0 root         (0) root         (0)     1646 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/slippage/fixed.py
--rw-rw-rw-   0 root         (0) root         (0)     1650 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/slippage/borrowfee.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/slippage/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/slippage/
--rw-rw-rw-   0 root         (0) root         (0)     3738 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/slippage/test_slippage.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/slippage/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)    18288 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/fixtures/test_model.keras.h5
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23705 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_allow_rebalance.py
--rw-rw-rw-   0 root         (0) root         (0)    40889 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_prices.py
--rw-rw-rw-   0 root         (0) root         (0)    15675 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_positions_closed_daily.py
--rw-rw-rw-   0 root         (0) root         (0)    25140 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_orders.py
--rw-rw-rw-   0 root         (0) root         (0)    61696 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_trade_date_validation.py
--rw-rw-rw-   0 root         (0) root         (0)    25756 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_save_custom_dataframe.py
--rw-rw-rw-   0 root         (0) root         (0)    63921 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)   106197 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_commissions.py
--rw-rw-rw-   0 root         (0) root         (0)     4751 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_weight_allocations.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/commission/
--rw-rw-rw-   0 root         (0) root         (0)     7435 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/commission/test_commissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/commission/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    84128 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_limit_position_sizes.py
--rw-rw-rw-   0 root         (0) root         (0)    40893 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_slippage.py
--rw-rw-rw-   0 root         (0) root         (0)    73903 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_backtest.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   116881 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_trade.py
--rw-rw-rw-   0 root         (0) root         (0)    66080 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_benchmark.py
--rw-rw-rw-   0 root         (0) root         (0)    95251 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/tests/test_ml.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/moonshot/mixins/
--rw-rw-rw-   0 root         (0) root         (0)     4366 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/mixins/weight.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/mixins/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/moonshot/strategies/
--rw-rw-rw-   0 root         (0) root         (0)    68542 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/strategies/base.py
--rw-rw-rw-   0 root         (0) root         (0)    20397 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/strategies/ml.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/strategies/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6530 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/cache.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/moonshot/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/moonshot/commission/
--rw-rw-rw-   0 root         (0) root         (0)     5673 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/commission/base.py
--rw-rw-rw-   0 root         (0) root         (0)     9481 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/commission/stk.py
--rw-rw-rw-   0 root         (0) root         (0)     1386 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/commission/fx.py
--rw-rw-rw-   0 root         (0) root         (0)     3553 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/commission/fut.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/commission/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/moonshot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5132 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1175 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/quantrocket_moonshot.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/quantrocket_moonshot.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/quantrocket_moonshot.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/quantrocket_moonshot.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)     1541 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/quantrocket_moonshot.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)      292 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/quantrocket_moonshot.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      194 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    68609 2022-10-11 13:07:09.000000 quantrocket-moonshot-2.8.0.1/versioneer.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2022-10-11 13:07:28.000000 quantrocket-moonshot-2.8.0.1/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     9144 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5132 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/quantrocket_moonshot.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1608 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/quantrocket_moonshot.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/quantrocket_moonshot.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/quantrocket_moonshot.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/quantrocket_moonshot.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/quantrocket_moonshot.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/moonshot/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/moonshot/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/mixins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/mixins/weight.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/py.typed
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/moonshot/commission/
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/commission/fx.py
+-rw-rw-rw-   0 root         (0) root         (0)    10964 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/commission/stk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1808 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/commission/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4049 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/commission/fut.py
+-rw-rw-rw-   0 root         (0) root         (0)     6774 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/commission/base.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/
+-rw-rw-rw-   0 root         (0) root         (0)    66082 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_benchmark.py
+-rw-rw-rw-   0 root         (0) root         (0)   116870 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_trade.py
+-rw-rw-rw-   0 root         (0) root         (0)     4753 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_weight_allocations.py
+-rw-rw-rw-   0 root         (0) root         (0)    84130 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_limit_position_sizes.py
+-rw-rw-rw-   0 root         (0) root         (0)    95253 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_ml.py
+-rw-rw-rw-   0 root         (0) root         (0)    40895 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_slippage.py
+-rw-rw-rw-   0 root         (0) root         (0)    63926 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_cache.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/commission/
+-rw-rw-rw-   0 root         (0) root         (0)     7436 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/commission/test_commissions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/commission/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   106199 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_commissions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15677 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_positions_closed_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)    25141 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_orders.py
+-rw-rw-rw-   0 root         (0) root         (0)    73905 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_backtest.py
+-rw-rw-rw-   0 root         (0) root         (0)    61697 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_trade_date_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23706 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_allow_rebalance.py
+-rw-rw-rw-   0 root         (0) root         (0)    25758 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_save_custom_dataframe.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)    18288 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/fixtures/test_model.keras.h5
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    40891 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_prices.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/slippage/
+-rw-rw-rw-   0 root         (0) root         (0)     3786 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/slippage/test_slippage.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_tests/slippage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/moonshot/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1162 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/moonshot/strategies/
+-rw-rw-rw-   0 root         (0) root         (0)    21742 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/strategies/ml.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/strategies/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    76764 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/strategies/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6531 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/_cache.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 14:56:09.000000 quantrocket-moonshot-2.9.0.0/moonshot/slippage/
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/slippage/fixed.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/slippage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1989 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/slippage/borrowfee.py
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/moonshot/slippage/base.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)    68609 2023-04-04 14:55:50.000000 quantrocket-moonshot-2.9.0.0/versioneer.py
```

### Comparing `quantrocket-moonshot-2.8.0.1/LICENSE.txt` & `quantrocket-moonshot-2.9.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/slippage/fixed.py` & `quantrocket-moonshot-2.9.0.0/moonshot/slippage/fixed.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,57 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-class FixedSlippage(object):
+from .base import Slippage
+import pandas as pd
+
+class FixedSlippage(Slippage):
     """
-    Applies a fixed pct slippage to each trade.
+    Apply a fixed pct slippage to each trade.
 
     This slippage class can be used on strategies indirectly (and more
     easily) by simply specifying SLIPPAGE_BPS on the strategy.
 
     Parameters
     ----------
     ONE_WAY_SLIPPAGE : float
         the slippage to apply to each trade (default 0.0005 = 5 basis points);
         overridden if `one_way_slippage` is passed to __init__
+
+    Notes
+    -----
+    Usage Guide:
+
+    * Moonshot commissions and slippage: https://qrok.it/dl/ms/moonshot-commissions-slippage
     """
     ONE_WAY_SLIPPAGE = 0.0005
 
-    def __init__(self, one_way_slippage=None):
+    def __init__(self, one_way_slippage: float =  None):
         if one_way_slippage is not None:
             self.one_way_slippage = one_way_slippage
         else:
             self.one_way_slippage = self.ONE_WAY_SLIPPAGE
 
-    def get_slippage(self, turnover, *args, **kwargs):
+    def get_slippage(
+        self,
+        turnover: pd.DataFrame,
+        *args,
+        **kwargs
+        ) -> pd.DataFrame:
         """
         Apply the fix pct slippage to each trade.
 
         Parameters
         ----------
         turnover : DataFrame, required
             a DataFrame of turnover
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/slippage/borrowfee.py` & `quantrocket-moonshot-2.9.0.0/moonshot/slippage/borrowfee.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,59 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from .base import Slippage
+import pandas as pd
 from quantrocket.fundamental import get_ibkr_borrow_fees_reindexed_like
 
-class IBKRBorrowFees(object):
+class IBKRBorrowFees(Slippage):
     """
-    Applies borrow fees to each position.
+    Apply borrow fees to each short position.
 
-    Parameters
-    ----------
-    TIME : str (HH:MM:SS[ TZ]), optional
-         Query and assess borrow fees as of this time of day. See
-         `quantrocket.fundamental.get_borrow_fees_reindexed_like`
-         for more details.
+    Notes
+    -----
+    Usage Guide:
+
+    * Moonshot borrow fees: https://qrok.it/dl/ms/moonshot-borrow-fees
+
+    Examples
+    --------
+    Use this on your strategy:
+
+    >>>  class MyStrategy(Moonshot):
+    >>>      SLIPPAGE_CLASSES = IBKRBorrowFees
     """
 
-    TIME = None
+    def get_slippage(
+        self,
+        turnover: pd.DataFrame,
+        positions: pd.DataFrame,
+        prices: pd.DataFrame
+        ) -> pd.DataFrame:
+
+        borrow_fees = get_ibkr_borrow_fees_reindexed_like(positions)
+
+        # convert to decimals
+        borrow_fees = borrow_fees / 100
+        # convert to daily rates
+        daily_borrow_fees = borrow_fees / 360 # industry convention is to divide annual fee by 360, not 365
+
+        # account for weekends, which are assessed the borrow fee x 3 days
+        dates = borrow_fees.apply(lambda x: borrow_fees.index)
+        days_held = (dates - dates.shift()).fillna(pd.Timedelta('1d')).apply(lambda x: x.dt.days)
+        daily_borrow_fees *= days_held
 
-    def get_slippage(self, turnover, positions, prices):
+        # by industry convention, collateral amount is 102% of borrow amount
+        assessed_fees = positions.where(positions < 0, 0).abs() * 1.02 * daily_borrow_fees
 
-        borrow_fees = get_ibkr_borrow_fees_reindexed_like(positions, time=self.TIME)
-        borrow_fees = borrow_fees.fillna(0) / 100
-        # Fees are assessed daily but the dataframe is expected to only
-        # includes trading days, thus use 252 instead of 365. In reality the
-        # borrow fee is greater for weekend positions than weekday positions,
-        # but this implementation doesn't model that.
-        daily_borrow_fees = borrow_fees / 252
-        assessed_fees = positions.where(positions < 0, 0).abs() * daily_borrow_fees
         return assessed_fees
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/slippage/test_slippage.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/slippage/test_slippage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import unittest
 from unittest.mock import patch
 import pandas as pd
 from moonshot.slippage import FixedSlippage, IBKRBorrowFees
 from moonshot import Moonshot
 
@@ -49,38 +49,38 @@
             "FI23456": [-0.17, 0.32, 0.23, 0, -0.4, -0.4, -0.4]},
             index=pd.DatetimeIndex(["2018-06-01", "2018-06-02", "2018-06-03",
                                    "2018-06-04", "2018-06-05", "2018-06-08",
                                    "2018-06-09"]))
 
         borrow_fee_rates = pd.DataFrame(
             {"FI12345": [1.75, 1.75, 1.75, 1.85, 1.85, 1.85, 1.2],
-            "FI23456": [8.0, 8.0, 8.23, 8.5, 0, 0, None]},
+            "FI23456": [8.0, 8.0, 8.23, 8.5, 0.25, 0.25, 0.25]},
             index=pd.DatetimeIndex(["2018-06-01", "2018-06-02", "2018-06-03",
                                    "2018-06-04", "2018-06-05", "2018-06-08",
                                    "2018-06-09"]))
 
         mock_get_ibkr_borrow_fees_reindexed_like.return_value = borrow_fee_rates
 
         turnover = prices = None
         fees = IBKRBorrowFees().get_slippage(turnover, positions, prices)
 
-        mock_get_ibkr_borrow_fees_reindexed_like.assert_called_with(positions, time=None)
+        mock_get_ibkr_borrow_fees_reindexed_like.assert_called_with(positions)
 
         fees.index.name = "Date"
         fees.index = fees.index.strftime("%Y-%m-%d")
         fees = fees.to_dict(orient="dict")
 
         self.assertAlmostEqual(fees["FI12345"]["2018-06-01"], 0)
         self.assertAlmostEqual(fees["FI12345"]["2018-06-02"], 0)
-        self.assertAlmostEqual(fees["FI12345"]["2018-06-03"], 0.000013889, 9)
-        self.assertAlmostEqual(fees["FI12345"]["2018-06-04"], 0.000014683, 9)
-        self.assertAlmostEqual(fees["FI12345"]["2018-06-05"], 0.000007341, 9)
+        self.assertAlmostEqual(fees["FI12345"]["2018-06-03"], 0.000009917, 9)
+        self.assertAlmostEqual(fees["FI12345"]["2018-06-04"], 0.000010483, 9)
+        self.assertAlmostEqual(fees["FI12345"]["2018-06-05"], 0.0000052417, 9)
         self.assertAlmostEqual(fees["FI12345"]["2018-06-08"], 0)
-        self.assertAlmostEqual(fees["FI12345"]["2018-06-09"], 0.000011905, 9)
+        self.assertAlmostEqual(fees["FI12345"]["2018-06-09"], 0.0000085, 9)
 
-        self.assertAlmostEqual(fees["FI23456"]["2018-06-01"], 0.000053968, 9)
+        self.assertAlmostEqual(fees["FI23456"]["2018-06-01"], 0.00003853, 8)
         self.assertAlmostEqual(fees["FI23456"]["2018-06-02"], 0)
         self.assertAlmostEqual(fees["FI23456"]["2018-06-03"], 0)
         self.assertAlmostEqual(fees["FI23456"]["2018-06-04"], 0)
-        self.assertAlmostEqual(fees["FI23456"]["2018-06-05"], 0)
-        self.assertAlmostEqual(fees["FI23456"]["2018-06-08"], 0)
-        self.assertAlmostEqual(fees["FI23456"]["2018-06-09"], 0)
+        self.assertAlmostEqual(fees["FI23456"]["2018-06-05"], 0.000002833, 9)
+        self.assertAlmostEqual(fees["FI23456"]["2018-06-08"], 0.0000085) # 3x b/c of weekend
+        self.assertAlmostEqual(fees["FI23456"]["2018-06-09"], 0.000002833, 9)
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/fixtures/test_model.keras.h5` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/fixtures/test_model.keras.h5`

 * *Files identical despite different names*

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_allow_rebalance.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_allow_rebalance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import unittest
 from unittest.mock import patch
 import pandas as pd
 from moonshot import Moonshot
 from moonshot.exceptions import MoonshotParameterError
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_prices.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_prices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import os
 import unittest
 from unittest.mock import patch
 import glob
 import pandas as pd
 from moonshot import Moonshot
 from moonshot.exceptions import MoonshotParameterError
-from moonshot.cache import TMP_DIR
+from moonshot._cache import TMP_DIR
 
 class GetPricesTestCase(unittest.TestCase):
 
     def tearDown(self):
         """
         Remove cached files.
         """
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_positions_closed_daily.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_positions_closed_daily.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import os
 import unittest
 from unittest.mock import patch
 import glob
 import pandas as pd
 from moonshot import Moonshot
-from moonshot.cache import TMP_DIR
+from moonshot._cache import TMP_DIR
 
 class PositionsClosedDailyTestCase(unittest.TestCase):
 
     def tearDown(self):
         """
         Remove cached files.
         """
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_orders.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_orders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import unittest
 from unittest.mock import patch
 import pandas as pd
 from moonshot import Moonshot
 from moonshot.exceptions import MoonshotError, MoonshotParameterError
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_trade_date_validation.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_trade_date_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import unittest
 from unittest.mock import patch
 import pandas as pd
 import datetime
 import pytz
 from moonshot import Moonshot
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_save_custom_dataframe.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_save_custom_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import os
 import unittest
 from unittest.mock import patch
 import glob
 import pandas as pd
 from moonshot import Moonshot
 from moonshot.exceptions import MoonshotParameterError
-from moonshot.cache import TMP_DIR
+from moonshot._cache import TMP_DIR
 
 class SaveCustomDataFrameTestCase(unittest.TestCase):
 
     def tearDown(self):
         """
         Remove cached files.
         """
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_cache.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import os
 import unittest
 from unittest.mock import patch
 import glob
 import pickle
 from pathlib import Path
 import inspect
 import pandas as pd
 import numpy as np
 from moonshot import Moonshot, MoonshotML
-from moonshot.cache import TMP_DIR
+from moonshot._cache import TMP_DIR
 from quantrocket.exceptions import ImproperlyConfigured
 from sklearn.tree import DecisionTreeClassifier
 
 class HistoricalPricesCacheTestCase(unittest.TestCase):
 
     def test_10_complain_if_houston_not_set(self):
         """
@@ -609,15 +609,15 @@
                            # Database was recently modified (in future)
                            {'last_modified': (pd.Timestamp.now() + pd.Timedelta(seconds=60)).isoformat(),
                             'name': 'quantrocket.history.my-db2.sqlite',
                             'path': '/var/lib/quantrocket/quantrocket.history.my-db2.sqlite',
                             'size_in_mb': 2.1},
                            ]}
 
-        with patch("moonshot.cache.list_databases", new=mock_list_databases):
+        with patch("moonshot._cache.list_databases", new=mock_list_databases):
             results = BuyBelow10().backtest(end_date="2018-05-04")
 
         self.assertSetEqual(
             set(results.index.get_level_values("Field")),
             {'Commission',
              'AbsExposure',
              'Signal',
@@ -993,15 +993,15 @@
                             'size_in_mb': 3.1},
                            {'last_modified': "2016-01-01T04:04:00",
                             'name': 'quantrocket.history.my-db2.sqlite',
                             'path': '/var/lib/quantrocket/quantrocket.history.my-db2.sqlite',
                             'size_in_mb': 2.1},
                            ]}
 
-        with patch("moonshot.cache.list_databases", new=mock_list_databases):
+        with patch("moonshot._cache.list_databases", new=mock_list_databases):
             results = BuyBelow10().backtest()
 
         self.assertSetEqual(
             set(results.index.get_level_values("Field")),
             {'Commission',
              'AbsExposure',
              'Signal',
@@ -1102,15 +1102,15 @@
                            # Database was recently modified (in future)
                            {'last_modified': (pd.Timestamp.now() + pd.Timedelta(seconds=60)).isoformat(),
                             'name': 'quantrocket.history.my-db2.sqlite',
                             'path': '/var/lib/quantrocket/quantrocket.history.my-db2.sqlite',
                             'size_in_mb': 2.1},
                            ]}
 
-        with patch("moonshot.cache.list_databases", new=mock_list_databases):
+        with patch("moonshot._cache.list_databases", new=mock_list_databases):
             with self.assertRaises(ImproperlyConfigured) as cm:
 
                 BuyBelow10().backtest()
 
         self.assertIn("HOUSTON_URL is not set", repr(cm.exception))
 
         # Finally, remove cached files
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_commissions.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_commissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import os
 import unittest
 from unittest.mock import patch
 import glob
 import pandas as pd
 from moonshot import Moonshot
-from moonshot.cache import TMP_DIR
+from moonshot._cache import TMP_DIR
 from moonshot.commission import PercentageCommission, FuturesCommission
 from moonshot.exceptions import MoonshotParameterError
 
 class MoonshotCommissionsTestCase(unittest.TestCase):
     """
     Test cases related to applying commissions in a backtest.
     """
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_weight_allocations.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_weight_allocations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import os
 import unittest
 from unittest.mock import patch
 import glob
 import pandas as pd
 from moonshot import Moonshot
-from moonshot.cache import TMP_DIR
+from moonshot._cache import TMP_DIR
 
 class WeightAllocationsTestCase(unittest.TestCase):
 
     def test_allocate_equal_weights(self):
         """
         Tests that the allocate_equal_weights returns the expected
         DataFrames.
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/commission/test_commissions.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/commission/test_commissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import unittest
 import pandas as pd
 from moonshot.commission import (
     FuturesCommission, PerShareCommission, NoCommission)
 from moonshot.commission.fx import SpotFXCommission
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_limit_position_sizes.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_limit_position_sizes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import os
 import glob
 import unittest
 from unittest.mock import patch
 import pandas as pd
 import numpy as np
 from moonshot import Moonshot
 from moonshot.exceptions import MoonshotParameterError
-from moonshot.cache import TMP_DIR
+from moonshot._cache import TMP_DIR
 
 class LimitPositionSizesBacktestTestCase(unittest.TestCase):
 
     def tearDown(self):
         """
         Remove cached files.
         """
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_slippage.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_slippage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import os
 import unittest
 from unittest.mock import patch
 import glob
 import pandas as pd
 from moonshot import Moonshot
 from moonshot.slippage import FixedSlippage
-from moonshot.cache import TMP_DIR
+from moonshot._cache import TMP_DIR
 
 class MoonshotSlippageTestCase(unittest.TestCase):
     """
     Test cases related to applying slippage in a backtest.
     """
 
     def tearDown(self):
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_backtest.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_backtest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import os
 import unittest
 from unittest.mock import patch
 import glob
 import pandas as pd
 from moonshot import Moonshot
-from moonshot.cache import TMP_DIR
+from moonshot._cache import TMP_DIR
 
 class BacktestTestCase(unittest.TestCase):
 
     def tearDown(self):
         """
         Remove cached files.
         """
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_trade.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import unittest
 from unittest.mock import patch
 import pandas as pd
 import json
 from moonshot import Moonshot
 from moonshot.exceptions import MoonshotParameterError
@@ -2646,15 +2646,15 @@
                 return signals
 
             def signals_to_target_weights(self, signals, prices):
                 weights = self.allocate_fixed_weights(signals, 0.25)
                 return weights
 
             def order_stubs_to_orders(self, orders, prices):
-                orders["Exchange"] = "GLOBEX"
+                orders["Exchange"] = "CME"
                 orders["OrderType"] = 'MKT'
                 orders["Tif"] = "DAY"
                 return orders
 
         def mock_get_prices(*args, **kwargs):
 
             dt_idx = pd.date_range(end=pd.Timestamp.today(tz="America/Chicago"), periods=3, normalize=True).tz_localize(None)
@@ -2764,37 +2764,37 @@
                 {
                     'Sid': "FI12345",
                     'Account': 'U123',
                     'Action': 'SELL',
                     'OrderRef': 'long-short-10',
                     # 0.5 allocation * 0.25 weight * 85K / multiplier 20 / 10.50
                     'TotalQuantity': 51,
-                    'Exchange': 'GLOBEX',
+                    'Exchange': 'CME',
                     'OrderType': 'MKT',
                     'Tif': 'DAY'
                 },
                 {
                     'Sid': "FI23456",
                     'Account': 'U123',
                     'Action': 'BUY',
                     'OrderRef': 'long-short-10',
                     # 0.5 allocation * 0.25 weight * 85K / multiplier 50 / 10.50
                     'TotalQuantity': 25,
-                    'Exchange': 'GLOBEX',
+                    'Exchange': 'CME',
                     'OrderType': 'MKT',
                     'Tif': 'DAY'
                 },
                 {
                     'Sid': "FI34567",
                     'Account': 'U123',
                     'Action': 'SELL',
                     'OrderRef': 'long-short-10',
                     # 0.5 allocation * 0.25 weight * 85K * magnifier 10 / 11.50
                     'TotalQuantity': 9239,
-                    'Exchange': 'GLOBEX',
+                    'Exchange': 'CME',
                     'OrderType': 'MKT',
                     'Tif': 'DAY'
                 }
             ]
         )
 
     def test_apply_exchange_rates(self):
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_benchmark.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import os
 import unittest
 from unittest.mock import patch
 import glob
 import requests
 import pandas as pd
 from moonshot import Moonshot
 from moonshot.exceptions import MoonshotError, MoonshotParameterError
 from quantrocket.exceptions import NoHistoricalData
-from moonshot.cache import TMP_DIR
+from moonshot._cache import TMP_DIR
 
 class BenchmarkTestCase(unittest.TestCase):
     """
     Test cases for including benchmarks in backtests.
     """
 
     def tearDown(self):
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/tests/test_ml.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_tests/test_ml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To run: python3 -m unittest discover -s tests/ -p test_*.py -t . -v
+# To run: python3 -m unittest discover -s _tests/ -p test_*.py -t . -v
 
 import os
 import unittest
 from unittest.mock import patch
 import glob
 import pickle
 import joblib
 import platform
 import inspect
 import pandas as pd
 import numpy as np
 from moonshot import MoonshotML
-from moonshot.cache import TMP_DIR
+from moonshot._cache import TMP_DIR
 from moonshot.exceptions import MoonshotError
 from sklearn.tree import DecisionTreeClassifier
 
 is_aarch64 = platform.machine() == "aarch64"
 
 class SKLearnMachineLearningTestCase(unittest.TestCase):
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/mixins/weight.py` & `quantrocket-moonshot-2.9.0.0/moonshot/mixins/weight.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,64 +15,82 @@
 import pandas as pd
 import numpy as np
 
 class WeightAllocationMixin(object):
     """
     Mixin class with utilities for turning signals into weights.
     """
-    def allocate_equal_weights(self, signals, cap=1.0):
+    def allocate_equal_weights(
+        self,
+        signals: pd.DataFrame,
+        cap: float = 1.0
+        ) -> pd.DataFrame:
         """
         For multi-security strategies. Given a dataframe of whole number
         signals (-1, 0, 1), reduces the position size so that the absolute
         sum of all weights is never greater than the cap.
         """
         # Count active signals for the day
         signals_count = signals.abs().sum(axis=1)
         # If no signals, divide by 1 to leave the signal as-is (can't divide by 0)
         divisor = np.where(signals_count != 0, signals_count, 1)
         return signals.div(divisor, axis=0) * cap / 1.0
 
-    def allocate_fixed_weights(self, signals, weight):
+    def allocate_fixed_weights(
+        self,
+        signals: pd.DataFrame,
+        weight: float
+        ) -> pd.DataFrame:
         """
         Applies the specified fixed weight to the signals.
         """
         return signals * weight
 
-    def allocate_fixed_weights_capped(self, signals, weight, cap=1.0):
+    def allocate_fixed_weights_capped(
+        self,
+        signals: pd.DataFrame,
+        weight: float,
+        cap: float = 1.0
+        ) -> pd.DataFrame:
         """
         Applies fixed weights, but if the sum of the weights exceeds the cap,
         applies equal weights.
         """
         equal_weighted = self.allocate_equal_weights(signals, cap=cap)
         fixed_weighted = self.allocate_fixed_weights(signals, weight)
         fixed_sum = fixed_weighted.abs().sum(axis=1)
         fixed_sum = pd.DataFrame(dict(
             [(column, fixed_sum.copy()) for column in signals.columns]),
             columns=signals.columns, index=signals.index)
         return pd.DataFrame(
             np.where(fixed_sum > cap, equal_weighted, fixed_weighted),
             index=signals.index, columns=signals.columns)
 
-    def allocate_market_neutral_fixed_weights_capped(self, signals, weight, cap=1.0,
-                                                  neutralize_weights=True):
+    def allocate_market_neutral_fixed_weights_capped(
+        self,
+        signals: pd.DataFrame,
+        weight: float,
+        cap: float = 1.0,
+        neutralize_weights: bool = True
+        ) -> pd.DataFrame:
         """
         Applies fixed capped weights to the long and short side separately to
         ensure the strategy is hedged.
         """
         long_signals = signals.where(signals > 0, 0)
         short_signals = signals.where(signals < 0, 0)
         cap_per_side = cap * 0.5
         long_weights = self.allocate_fixed_weights_capped(long_signals, weight, cap=cap_per_side)
         short_weights = self.allocate_fixed_weights_capped(short_signals, weight, cap=cap_per_side)
         weights = long_weights.where(long_weights > 0, short_weights)
         if neutralize_weights:
             weights = self.neutralize_weights(weights)
         return weights
 
-    def neutralize_weights(self, weights):
+    def neutralize_weights(self, weights: pd.DataFrame) -> pd.DataFrame:
         """
         If the long or short side has a greater total weight than the
         opposite side, proportionately reduces the overweight side.
         """
         long_weights = weights.where(weights > 0, 0)
         short_weights = weights.where(weights < 0, 0)
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/mixins/__init__.py` & `quantrocket-moonshot-2.9.0.0/moonshot/mixins/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .weight import WeightAllocationMixin
+
+__all__ = ["WeightAllocationMixin"]
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/strategies/base.py` & `quantrocket-moonshot-2.9.0.0/moonshot/strategies/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Union, Any
 import io
 import pandas as pd
 import numpy as np
 import time
 import requests
 import json
 import math
-from moonshot.slippage import FixedSlippage
+from moonshot.slippage import Slippage, FixedSlippage
+from moonshot.commission import Commission
 from moonshot.mixins import WeightAllocationMixin
-from moonshot.cache import Cache
+from moonshot._cache import Cache
 from moonshot.exceptions import MoonshotError, MoonshotParameterError
 from quantrocket.price import get_prices
 from quantrocket.master import list_calendar_statuses, download_master_file
 from quantrocket.account import download_account_balances, download_exchange_rates
 from quantrocket.blotter import list_positions, download_order_statuses
 
 class Moonshot(
@@ -51,16 +53,16 @@
         `prices_to_signals` -> `signals_to_target_weights` -> `order_stubs_to_orders`
 
     Parameters
     ----------
     CODE : str, required
         the strategy code
 
-    DB : str, required
-        code of db to pull data from
+    DB : str or list of str, required
+        one or more database codes to pull data from
 
     DB_FIELDS : list of str, optional
         fields to retrieve from db (defaults to ["Open", "Close", "Volume"])
 
     DB_TIMES : list of str (HH:MM:SS), optional
         for intraday databases, only retrieve these times
 
@@ -79,35 +81,36 @@
     EXCLUDE_SIDS : list of str, optional
         exclude these sids from db query
 
     EXCLUDE_UNIVERSES : list of str, optional
         exclude these universes from db query
 
     CONT_FUT : str, optional
-        pass this cont_fut option to db query (default None)
+        pass this cont_fut option to db query (default None). See quantrocket.get_prices
+        for more info.
 
     LOOKBACK_WINDOW : int, optional
         get this many days additional data prior to the backtest start date or
         trade date to account for rolling windows. If set to None (the default),
         will use the largest value of any attributes ending with `*_WINDOW`, or
         252 if no such attributes, and will further pad window based on any
         `*_INTERVAL` attributes, which are interpreted as pandas offset aliases
         (for example `REBALANCE_INTERVAL = 'Q'`). Set to 0 to disable.
 
     NLV : dict, optional
         dict of currency:NLV for each currency represented in the strategy. Can
         alternatively be passed directly to backtest method.
 
-    COMMISSION_CLASS : Class or dict of (sectype,exchange,currency):Class, optional
+    COMMISSION_CLASS : Commission class or dict of (sectype,exchange,currency): Commission class, optional
         the commission class to use. If strategy includes a mix of security types,
         exchanges, or currencies, you can pass a dict mapping tuples of
         (sectype,exchange,currency) to the different commission classes. By default
         no commission is applied.
 
-    SLIPPAGE_CLASSES : iterable of slippage classes, optional
+    SLIPPAGE_CLASSES : iterable of Slippage classes, optional
         one or more slippage classes. By default no slippage is applied.
 
     SLIPPAGE_BPS : float, optional
         amount on one-slippage to apply to each trade in BPS (for example, enter 5 to deduct
         5 BPS)
 
     BENCHMARK : str, optional
@@ -161,67 +164,142 @@
     ACCOUNT_BALANCE_FIELD : str or list of str, optional
         the account field to use for calculating order quantities as a percentage of
         account equity. Applies to trading only, not backtesting. Default is
         NetLiquidation. If a list of fields is provided, the minimum value is used.
         For example, ['NetLiquidation', 'PreviousEquity'] means to use the lesser of
         NetLiquidation or PreviousEquity to determine order quantities.
 
+    Notes
+    -----
+    Usage Guide:
+
+    * Moonshot: https://qrok.it/dl/ms/moonshot
+
     Examples
     --------
     Example of a minimal strategy that runs on a history db called "mexi-stk-1d" and buys when
-    the securities are above their 200-day moving average:
+    the securities are above their 200-day moving average::
+
+        import pandas as pd
 
-    >>> MexicoMovingAverage(Moonshot):
-    >>>
-    >>>     CODE = "mexi-ma"
-    >>>     DB = "mexi-stk-1d"
-    >>>     MAVG_WINDOW = 200
-    >>>
-    >>>     def prices_to_signals(self, prices):
-    >>>         closes = prices.loc["Close"]
-    >>>         mavgs = closes.rolling(self.MAVG_WINDOW).mean()
-    >>>         signals = closes > mavgs.shift()
-    >>>         return signals.astype(int)
+        MexicoMovingAverage(Moonshot):
+
+            CODE = "mexi-ma"
+            DB = "mexi-stk-1d"
+            MAVG_WINDOW = 200
+
+            def prices_to_signals(self, prices: pd.DataFrame):
+                closes = prices.loc["Close"]
+                mavgs = closes.rolling(self.MAVG_WINDOW).mean()
+                signals = closes > mavgs.shift()
+                return signals.astype(int)
     """
-    CODE = None
-    DB = None
-    DB_FIELDS = ["Open", "Close", "Volume"]
-    DB_TIMES = None
-    DB_DATA_FREQUENCY = None
-    SIDS = None
-    UNIVERSES = None
-    EXCLUDE_SIDS = None
-    EXCLUDE_UNIVERSES = None
-    CONT_FUT = None
-    LOOKBACK_WINDOW = None
-    NLV = None
-    COMMISSION_CLASS = None
-    SLIPPAGE_CLASSES = ()
-    SLIPPAGE_BPS = 0
-    BENCHMARK = None
-    BENCHMARK_DB = None
-    BENCHMARK_TIME = None
-    TIMEZONE = None
-    CALENDAR = None
-    POSITIONS_CLOSED_DAILY = False
-    ALLOW_REBALANCE = True
-    CONTRACT_VALUE_REFERENCE_FIELD = None
-    ACCOUNT_BALANCE_FIELD = None
+    CODE: str = None
+    """the strategy code"""
+    DB: Union[str, list[str]] = None
+    """one or more database codes to pull data from"""
+    DB_FIELDS: list[str] = ["Open", "Close", "Volume"]
+    """fields to retrieve from db (defaults to ["Open", "Close", "Volume"])"""
+    DB_TIMES: list[str] = None
+    """for intraday databases, only retrieve these times"""
+    DB_DATA_FREQUENCY: str = None
+    """Only applicable when DB specifies a Zipline bundle. Whether to query minute or
+    daily data.  If omitted, defaults to minute data for minute bundles and to daily
+    data for daily bundles. This parameter only needs to be set to request daily data
+    from a minute bundle. Possible choices: daily, minute (or aliases d, m)."""
+    SIDS: list[str] = None
+    """limit db query to these sids"""
+    UNIVERSES: list[str] = None
+    """limit db query to these universes"""
+    EXCLUDE_SIDS: list[str] = None
+    """exclude these sids from db query"""
+    EXCLUDE_UNIVERSES: list[str] = None
+    """exclude these universes from db query"""
+    CONT_FUT: str = None
+    """pass this cont_fut option to db query (default None). See quantrocket.get_prices
+    for more info."""
+    LOOKBACK_WINDOW: int = None
+    """get this many days additional data prior to the backtest start date or
+    trade date to account for rolling windows. If set to None (the default),
+    will use the largest value of any attributes ending with `*_WINDOW`, or
+    252 if no such attributes, and will further pad window based on any
+    `*_INTERVAL` attributes, which are interpreted as pandas offset aliases
+    (for example `REBALANCE_INTERVAL = 'Q'`). Set to 0 to disable."""
+    NLV: dict[str, float] = None
+    """dict of currency:NLV for each currency represented in the strategy. Can
+    alternatively be passed directly to backtest method."""
+    COMMISSION_CLASS: Union[Commission, dict[tuple[str, str, str], Commission]] = None
+    """Commission class or dict of (sectype,exchange,currency): Commission class, optional
+    the commission class to use. If strategy includes a mix of security types,
+    exchanges, or currencies, you can pass a dict mapping tuples of
+    (sectype,exchange,currency) to the different commission classes. By default
+    no commission is applied."""
+    SLIPPAGE_CLASSES: tuple[Slippage] = ()
+    """one or more slippage classes. By default no slippage is applied."""
+    SLIPPAGE_BPS: float = 0
+    """amount on one-slippage to apply to each trade in BPS (for example, enter 5 to deduct
+    5 BPS)"""
+    BENCHMARK: str = None
+    """the sid of a security in the historical data to use as the benchmark."""
+    BENCHMARK_DB: str = None
+    """the database containing the benchmark, if different from DB. BENCHMARK_DB
+    should contain end-of-day data, not intraday (but can be used with intraday
+    backtests)."""
+    BENCHMARK_TIME: str = None
+    """use prices from this time of day as benchmark prices. Only applicable if
+    benchmark prices originate in DB (not BENCHMARK_DB), DB contains intraday
+    data, and backtest results are daily."""
+    TIMEZONE: str = None
+    """convert timestamps to this timezone (if not provided, will be inferred
+    from securities universe if possible)"""
+    CALENDAR: str = None
+    """use this exchange's trading calendar to determine which date's signals
+    should be used for live trading. If the exchange is currently open,
+    today's signals will be used. If currently closed, the signals corresponding
+    to the last date the exchange was open will be used. If no calendar is specified,
+    today's signals will be used."""
+    POSITIONS_CLOSED_DAILY: bool = False
+    """if True, positions in backtests that fall on adjacent days are assumed to
+    be closed out and reopened each day rather than held continuously; this
+    impacts commission and slippage calculations (default is False, meaning
+    adjacent positions are assumed to be held continuously)"""
+    ALLOW_REBALANCE: Union[bool, float] = True
+    """in live trading, whether to allow rebalancing of existing positions that
+    are already on the correct side. If True (the default), allow rebalancing.
+    If False, no rebalancing. If set to a positive decimal, allow rebalancing
+    only when the existing position differs from the target position by at least
+    this percentage. For example 0.5 means don't rebalance a position unless
+    the position will change by +/-50%."""
+    CONTRACT_VALUE_REFERENCE_FIELD: str = None
+    """the price field to use for determining contract values for the purpose of
+    applying commissions and constraining weights in backtests and calculating
+    order quantities in trading. Defaults to the first available of Close, Open,
+    MinuteCloseClose, SecondCloseClose, LastPriceClose, BidPriceClose, AskPriceClose,
+    TimeSalesLastPriceClose, TimeSalesFilteredLastPriceClose, LastPriceMean,
+    BidPriceMean, AskPriceMean, TimeSalesLastPriceMean, TimeSalesFilteredLastPriceMean,
+    MinuteOpenOpen, SecondOpenOpen, LastPriceOpen, BidPriceOpen, AskPriceOpen,
+    TimeSalesLastPriceOpen, TimeSalesFilteredLastPriceOpen."""
+    ACCOUNT_BALANCE_FIELD: Union[str, list[str]] = None
+    """the account field to use for calculating order quantities as a percentage of
+    account equity. Applies to trading only, not backtesting. Default is
+    NetLiquidation. If a list of fields is provided, the minimum value is used.
+    For example, ['NetLiquidation', 'PreviousEquity'] means to use the lesser of
+    NetLiquidation or PreviousEquity to determine order quantities."""
 
     def __init__(self):
-        self.is_trade = False
-        self.review_date = None # see trade() docstring
-        self.is_backtest = False
+        self.is_trade: bool = False
+        self.review_date: str = None # see trade() docstring
+        self.is_backtest: bool = False
         self._securities_master = None
         self._backtest_results = {}
         self._inferred_timezone = None
         self._signal_date = None # set by _weights_to_today_weights
         self._signal_time = None # set by _weights_to_today_weights
 
-    def prices_to_signals(self, prices):
+    def prices_to_signals(self, prices: pd.DataFrame) -> pd.DataFrame:
         """
         From a DataFrame of prices, return a DataFrame of signals. By convention,
         signals should be 1=long, 0=cash, -1=short.
 
         Must be implemented by strategy subclasses.
 
         Parameters
@@ -231,27 +309,39 @@
             price/market data
 
         Returns
         -------
         DataFrame
             signals
 
+        Notes
+        -----
+        Usage Guide:
+
+        * Moonshot: https://qrok.it/dl/ms/moonshot
+
         Examples
         --------
-        Buy when the close is above yesterday's 50-day moving average:
+        Buy when the close is above yesterday's 50-day moving average::
+
+            import pandas as pd
 
-        >>> def prices_to_signals(self, prices):
-        >>>     closes = prices.loc["Close"]
-        >>>     mavgs = closes.rolling(50).mean()
-        >>>     signals = closes > mavgs.shift()
-        >>>     return signals.astype(int)
+            def prices_to_signals(self, prices: pd.DataFrame):
+                closes = prices.loc["Close"]
+                mavgs = closes.rolling(50).mean()
+                signals = closes > mavgs.shift()
+                return signals.astype(int)
         """
         raise NotImplementedError("strategies must implement prices_to_signals")
 
-    def signals_to_target_weights(self, signals, prices):
+    def signals_to_target_weights(
+        self,
+        signals: pd.DataFrame,
+        prices: pd.DataFrame
+        ) -> pd.DataFrame:
         """
         From a DataFrame of signals, return a DataFrame of target weights.
 
         Whereas signals indicate the direction of the trades, weights
         indicate both the direction and size. For example, -0.5 means a short
         position equal to 50% of the equity allocated to the strategy.
 
@@ -275,26 +365,36 @@
             of price/market data
 
         Returns
         -------
         DataFrame
             weights
 
+        Notes
+        -----
+        Usage Guide:
+
+        * Moonshot: https://qrok.it/dl/ms/moonshot
+
         Examples
         --------
-        The default implementation is shown below:
+        The default implementation is shown below::
 
-        >>> def signals_to_target_weights(self, signals, prices):
-        >>>     weights = self.allocate_equal_weights(signals) # provided by moonshot.mixins.WeightAllocationMixin
-        >>>     return weights
+            def signals_to_target_weights(self, signals: pd.DataFrame, prices: pd.DataFrame):
+                weights = self.allocate_equal_weights(signals) # provided by moonshot.mixins.WeightAllocationMixin
+                return weights
         """
         weights = self.allocate_equal_weights(signals)
         return weights
 
-    def target_weights_to_positions(self, weights, prices):
+    def target_weights_to_positions(
+        self,
+        weights: pd.DataFrame,
+        prices: pd.DataFrame
+        ) -> pd.DataFrame:
         """
         From a DataFrame of target weights, return a DataFrame of simulated
         positions.
 
         The positions should shift the weights based on when the weights
         would be filled in live trading.
 
@@ -312,27 +412,37 @@
             price/market data
 
         Returns
         -------
         DataFrame
             positions
 
+        Notes
+        -----
+        Usage Guide:
+
+        * Moonshot: https://qrok.it/dl/ms/moonshot
+
         Examples
         --------
         The default implemention is shown below (enter position in the period after
-        signal generation/weight allocation):
+        signal generation/weight allocation)::
 
-        >>> def target_weights_to_positions(self, weights, prices):
-        >>>     positions = weights.shift()
-        >>>     return positions
+            def target_weights_to_positions(self, weights: pd.DataFrame, prices: pd.DataFrame):
+                positions = weights.shift()
+                return positions
         """
         positions = weights.shift()
         return positions
 
-    def positions_to_gross_returns(self, positions, prices):
+    def positions_to_gross_returns(
+        self,
+        positions: pd.DataFrame,
+        prices: pd.DataFrame
+        ) -> pd.DataFrame:
         """
         From a DataFrame of positions, return a DataFrame of returns before
         commissions and slippage.
 
         By default, assumes entry on the close on the period the position is
         taken and calculates the return through the following period's close.
         Intended to be overridden by strategy subclasses.
@@ -347,28 +457,38 @@
             price/market data
 
         Returns
         -------
         DataFrame
             gross returns
 
+        Notes
+        -----
+        Usage Guide:
+
+        * Moonshot: https://qrok.it/dl/ms/moonshot
+
         Examples
         --------
-        The default implementation is shown below:
+        The default implementation is shown below::
 
-        >>> def positions_to_gross_returns(self, positions, prices):
-        >>>     closes = prices.loc["Close"]
-        >>>     gross_returns = closes.pct_change() * positions.shift()
-        >>>     return gross_returns
+            def positions_to_gross_returns(self, positions: pd.DataFrame, prices: pd.DataFrame):
+                closes = prices.loc["Close"]
+                gross_returns = closes.pct_change() * positions.shift()
+                return gross_returns
         """
         closes = prices.loc["Close"]
         gross_returns = closes.pct_change() * positions.shift()
         return gross_returns
 
-    def order_stubs_to_orders(self, orders, prices):
+    def order_stubs_to_orders(
+        self,
+        orders: pd.DataFrame,
+        prices: pd.DataFrame
+        ) -> pd.DataFrame:
         """
         From a DataFrame of order stubs, creates a DataFrame of fully
         specified orders.
 
         Parameters
         ----------
         orders : DataFrame
@@ -381,48 +501,58 @@
 
         Returns
         -------
         DataFrame
             a DataFrame of fully specified orders, with (at minimum) columns
             Exchange, Tif, OrderType added
 
+        Notes
+        -----
+        Usage Guide:
+
+        * Moonshot live trading: https://qrok.it/dl/ms/moonshot-trade
+
         Examples
         --------
         The orders DataFrame provided to this method resembles the following:
 
         >>> print(orders)
               Sid  Account Action     OrderRef  TotalQuantity
         0   12345   U12345   SELL  my-strategy            100
         1   12345   U55555   SELL  my-strategy             50
         2   23456   U12345    BUY  my-strategy            100
         3   23456   U55555    BUY  my-strategy             50
         4   34567   U12345    BUY  my-strategy            200
         5   34567   U55555    BUY  my-strategy            100
 
         The default implemention creates MKT DAY orders and is
-        shown below:
+        shown below::
 
-        >>> def order_stubs_to_orders(self, orders, prices):
-        >>>     orders["OrderType"] = "MKT"
-        >>>     orders["Tif"] = "DAY"
-        >>>     return orders
-
-        Set a limit price equal to the prior closing price:
-
-        >>> closes = prices.loc["Close"]
-        >>> prior_closes = closes.shift()
-        >>> prior_closes = self.reindex_like_orders(prior_closes, orders)
-        >>> orders["OrderType"] = "LMT"
-        >>> orders["LmtPrice"] = prior_closes
+            def order_stubs_to_orders(self, orders: pd.DataFrame, prices: pd.DataFrame):
+                orders["OrderType"] = "MKT"
+                orders["Tif"] = "DAY"
+                return orders
+
+        Set a limit price equal to the prior closing price::
+
+            closes = prices.loc["Close"]
+            prior_closes = closes.shift()
+            prior_closes = self.reindex_like_orders(prior_closes, orders)
+            orders["OrderType"] = "LMT"
+            orders["LmtPrice"] = prior_closes
         """
         orders["OrderType"] = "MKT"
         orders["Tif"] = "DAY"
         return orders
 
-    def reindex_like_orders(self, df, orders):
+    def reindex_like_orders(
+        self,
+        df: pd.DataFrame,
+        orders: pd.DataFrame
+        ) -> 'pd.Series[Any]':
         """
         Reindexes a DataFrame (having Sids as columns and dates as index)
         to match the shape of the orders DataFrame.
 
         Parameters
         ----------
         df : DataFrame, required
@@ -433,29 +563,35 @@
             an orders DataFrame with a Sid column
 
         Returns
         -------
         Series
             a Series with an index matching orders
 
+        Notes
+        -----
+        Usage Guide:
+
+        * Moonshot live trading: https://qrok.it/dl/ms/moonshot-trade
+
         Examples
         --------
         Calculate prior closes (assuming daily bars) and reindex like
-        orders:
+        orders::
 
-        >>> closes = prices.loc["Close"]
-        >>> prior_closes = closes.shift()
-        >>> prior_closes = self.reindex_like_orders(prior_closes, orders)
+            closes = prices.loc["Close"]
+            prior_closes = closes.shift()
+            prior_closes = self.reindex_like_orders(prior_closes, orders)
 
         Calculate prior closes (assuming 30-min bars) and reindex like
-        orders:
+        orders::
 
-        >>> session_closes = prices.loc["Close"].xs("15:30:00", level="Time")
-        >>> prior_closes = session_closes.shift()
-        >>> prior_closes = self.reindex_like_orders(prior_closes, orders)
+            session_closes = prices.loc["Close"].xs("15:30:00", level="Time")
+            prior_closes = session_closes.shift()
+            prior_closes = self.reindex_like_orders(prior_closes, orders)
 
         """
         df = df.loc[self._signal_date]
         if "Time" in df.index.names:
             if not self._signal_time:
                 raise MoonshotError(
                     "cannot reindex DataFrame like orders because DataFrame contains "
@@ -464,15 +600,15 @@
             df = df.loc[self._signal_time]
 
         df.name = "_MoonshotOther"
         df = orders.join(df, on="Sid")._MoonshotOther
         df.name = None
         return df
 
-    def orders_to_child_orders(self, orders):
+    def orders_to_child_orders(self, orders: pd.DataFrame) -> pd.DataFrame:
         """
         From a DataFrame of orders, returns a DataFrame of child orders
         (bracket orders) to be submitted if the parent orders fill.
 
         An OrderId column will be added to the orders DataFrame, and child
         orders will be linked to it via a ParentId column. The Action
         (BUY/SELL) will be reversed on the child orders but otherwise the
@@ -484,14 +620,20 @@
             an orders DataFrame
 
         Returns
         -------
         DataFrame
             a DataFrame of child orders
 
+        Notes
+        -----
+        Usage Guide:
+
+        * Moonshot live trading: https://qrok.it/dl/ms/moonshot-trade
+
         Examples
         --------
         >>> orders.head()
               Sid   Action  TotalQuantity Exchange OrderType  Tif
         0   12345      BUY            200    SMART       MKT  Day
         1   23456      BUY            400    SMART       MKT  Day
         >>> child_orders = self.orders_to_child_orders(orders)
@@ -825,15 +967,18 @@
 
         # Convert quantities back to weights
         target_trade_values_in_trade_currency = quantities * contract_values
         weights = target_trade_values_in_trade_currency / nlvs_in_trade_currency
 
         return weights
 
-    def limit_position_sizes(self, prices):
+    def limit_position_sizes(
+        self,
+        prices: pd.DataFrame
+        ) -> tuple[pd.DataFrame, pd.DataFrame]:
         """
         This method should return a tuple of DataFrames::
 
             return max_quantities_for_longs, max_quantities_for_shorts
 
         where the DataFrames define the maximum number of shares/contracts
         that can be held long and short, respectively. Maximum limits might
@@ -875,26 +1020,32 @@
             price/market data
 
         Returns
         -------
         tuple of (DataFrame, DataFrame)
             max quantities for long, max quantities for shorts
 
+        Notes
+        -----
+        Usage Guide:
+
+        * Position size constraints: https://qrok.it/dl/ms/moonshot-limit-positions
+
         Examples
         --------
-        Limit quantities to 1% of 15-day average daily volume:
+        Limit quantities to 1% of 15-day average daily volume::
 
-        >>> def limit_position_sizes(self, prices):
-        >>>     # assumes end-of-day bars, for intraday bars, use `.xs` to
-        >>>     # select a time of day
-        >>>     volumes = prices.loc["Volume"]
-        >>>     mean_volumes = volumes.rolling(15).mean()
-        >>>     max_shares = (mean_volumes * 0.01).round()
-        >>>     max_quantities_for_longs = max_quantities_for_shorts = max_shares
-        >>>     return max_quantities_for_longs, max_quantities_for_shorts
+            def limit_position_sizes(self, prices):
+                # assumes end-of-day bars, for intraday bars, use `.xs` to
+                # select a time of day
+                volumes = prices.loc["Volume"]
+                mean_volumes = volumes.rolling(15).mean()
+                max_shares = (mean_volumes * 0.01).round()
+                max_quantities_for_longs = max_quantities_for_shorts = max_shares
+                return max_quantities_for_longs, max_quantities_for_shorts
         """
         max_quantities_for_longs = None
         max_quantities_for_shorts = None
         return max_quantities_for_longs, max_quantities_for_shorts
 
     @classmethod
     def _get_lookback_window(cls):
@@ -1025,18 +1176,47 @@
         else:
             buffer = 10
 
         start_date = pd.Timestamp(start_date) - pd.Timedelta(
             days=math.ceil(lookback_window*days_per_year/trading_days_per_year) + buffer)
         return start_date.date().isoformat()
 
-    def get_prices(self, start_date, end_date=None, nlv=None, no_cache=False):
+    def get_prices(
+        self,
+        start_date: str = None,
+        end_date: str = None,
+        nlv: dict[str, float] = None,
+        no_cache: bool = False
+        ) -> pd.DataFrame:
         """
-        Downloads prices from a history db and/or real-time aggregate db.
-        Downloads security details from the master db.
+        Download prices from a history db and/or real-time aggregate db.
+
+        Parameters
+        ----------
+        start_date : str (YYYY-MM-DD), optional
+            download prices on or after this date (default is to include all
+            history in db)
+
+        end_date : str (YYYY-MM-DD), optional
+            download prices on or before this date (default is to include all
+            history in db)
+
+        nlv : dict
+            dict of currency:nlv. Should contain a currency:nlv pair for
+            each currency represented in the strategy
+
+        no_cache : bool
+            don't use cached files even if available. Using cached files speeds
+            up backtests but may be undesirable if underlying data has changed.
+            See http://qrok.it/h/mcache to learn more about caching in Moonshot.
+
+        Returns
+        -------
+        DataFrame
+            multiindex (Field, Date) or (Field, Date, Time) DataFrame of prices
         """
         if start_date:
             start_date = self._get_start_date_with_lookback(start_date)
 
         codes = self.DB
         if not isinstance(codes, (list, tuple)):
             codes = [self.DB]
@@ -1106,16 +1286,23 @@
         Converts a prices DataFrame to a DataFrame of signals. This private
         method, which simply calls the user-modified public method
         `prices_to_signals`, exists for the benefit of the MoonshotML
         subclass, which overrides it.
         """
         return self.prices_to_signals(prices)
 
-    def backtest(self, start_date=None, end_date=None, nlv=None, allocation=1.0,
-                 label_sids=False, no_cache=False):
+    def backtest(
+        self,
+        start_date: str = None,
+        end_date: str = None,
+        nlv: dict[str, float] = None,
+        allocation: float = 1.0,
+        label_sids: bool = False,
+        no_cache: bool = False
+        ) -> pd.DataFrame:
         """
         Backtest a strategy and return a DataFrame of results.
 
         Parameters
         ----------
         start_date : str (YYYY-MM-DD), optional
             the backtest start date (default is to include all history in db)
@@ -1308,15 +1495,19 @@
                 benchmark = benchmark.xs(self.BENCHMARK_TIME, level="Time")
             except KeyError:
                 raise MoonshotError("BENCHMARK_TIME {0} is not in {1} data".format(
                     self.BENCHMARK_TIME, benchmark_db))
 
         return pd.DataFrame(benchmark)
 
-    def save_to_results(self, name, df):
+    def save_to_results(
+        self,
+        name: str,
+        df: pd.DataFrame
+        ) -> None:
         """
         Saves the DataFrame to the backtest results output.
 
         DataFrame should have a Date or (Date, Time) index with
         Sids as columns.
 
         Parameters
@@ -1327,21 +1518,27 @@
         df : DataFrame, required
             the DataFrame to save
 
         Returns
         -------
         None
 
+        Notes
+        -----
+        Usage Guide:
+
+        * Save custom DataFrames to backtest results: https://qrok.it/dl/ms/moonshot-save
+
         Examples
         --------
-        Save moving averages of closing prices to results:
+        Save moving averages of closing prices to results::
 
-        >>> closes = prices.loc["Close"]
-        >>> mavgs = closes.rolling(50).mean()
-        >>> self.save_to_results("MAvg", mavgs)
+            closes = prices.loc["Close"]
+            mavgs = closes.rolling(50).mean()
+            self.save_to_results("MAvg", mavgs)
         """
 
         # No-op if trading
         if self.is_trade:
             return
 
         reserved_names = [
@@ -1368,15 +1565,19 @@
                     name, ",".join([str(level_name) for level_name in index_levels])))
 
         if not hasattr(df.index.get_level_values("Date"), "date"):
             raise MoonshotParameterError("custom DataFrame '{0}' must have a DatetimeIndex to concat properly".format(name))
 
         self._backtest_results[name] = df
 
-    def trade(self, allocations, review_date=None):
+    def trade(
+        self,
+        allocations: dict[str, float],
+        review_date: str = None
+        ) -> pd.DataFrame:
         """
         Run the strategy and create orders.
 
         Parameters
         ----------
         allocations : dict, required
             dict of account:allocation to strategy (expressed as a percentage of NLV)
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/strategies/ml.py` & `quantrocket-moonshot-2.9.0.0/moonshot/strategies/ml.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pickle
+from typing import Union, Any
 try:
     import joblib
 except ImportError:
     pass
 import pandas as pd
 import numpy as np
 from moonshot.strategies.base import Moonshot
 from moonshot.exceptions import MoonshotError, MoonshotParameterError
-from moonshot.cache import Cache
+from moonshot._cache import Cache
 
 class MoonshotML(Moonshot):
     """
     Base class for Moonshot machine learning strategies.
 
     To create a strategy, subclass this class. Implement your trading logic in the class
     methods, and store your strategy parameters as class attributes.
@@ -161,40 +162,51 @@
     ACCOUNT_BALANCE_FIELD : str or list of str, optional
         the account field to use for calculating order quantities as a percentage of
         account equity. Applies to trading only, not backtesting. Default is
         NetLiquidation. If a list of fields is provided, the minimum value is used.
         For example, ['NetLiquidation', 'PreviousEquity'] means to use the lesser of
         NetLiquidation or PreviousEquity to determine order quantities.
 
+    Notes
+    -----
+    Usage Guide:
+
+    * MoonshotML: https://qrok.it/dl/ms/moonshot-ml
+
     Examples
     --------
     Example of a minimal strategy that runs on a history db called "usa-stk-1d", trains
     the model using the 1-day and 2-day returns, and buys when the machine learning
-    model predicts a positive 1-day forward return:
+    model predicts a positive 1-day forward return::
+
+        import pandas as pd
+
+        class DemoMLStrategy(MoonshotML):
 
-    >>> class DemoMLStrategy(MoonshotML):
-    >>>
-    >>>     CODE = "demo-ml"
-    >>>     DB = "usa-stk-1d"
-    >>>     MODEL = "my_ml_model.pkl"
-    >>>
-    >>>     def prices_to_features(self, prices):
-    >>>         closes = prices.loc["Close"]
-    >>>         features = {}
-    >>>         features["returns_1d"]= closes.pct_change()
-    >>>         features["returns_2d"] = (closes - closes.shift(2)) / closes.shift(2)
-    >>>         targets = closes.pct_change().shift(-1)
-    >>>         return features, targets
-    >>>
-    >>>     def predictions_to_signals(self, predictions, prices):
-    >>>         signals = predictions > 0
-    >>>         return signals.astype(int)
+            CODE = "demo-ml"
+            DB = "usa-stk-1d"
+            MODEL = "my_ml_model.pkl"
+
+            def prices_to_features(self, prices: pd.DataFrame):
+                closes = prices.loc["Close"]
+                features = {}
+                features["returns_1d"]= closes.pct_change()
+                features["returns_2d"] = (closes - closes.shift(2)) / closes.shift(2)
+                targets = closes.pct_change().shift(-1)
+                return features, targets
+
+            def predictions_to_signals(self, predictions: pd.DataFrame, prices: pd.DataFrame):
+                signals = predictions > 0
+                return signals.astype(int)
     """
 
-    MODEL = None
+    MODEL: str = None
+    """path of machine learning model to load (for scikit-learn models, a joblib or
+    pickle file); alternatively model can be passed as a parameter to backtest
+    method, in which case the MODEL parameter is ignored"""
 
     def __init__(self, *args, **kwargs):
         super(MoonshotML, self).__init__(*args, **kwargs)
         self.model = None
 
     def _load_model(self):
         """
@@ -208,15 +220,23 @@
         elif "keras.h5" in self.MODEL:
             from keras.models import load_model
             self.model = load_model(self.MODEL)
         else:
             with open(self.MODEL, "rb") as f:
                 self.model = pickle.load(f)
 
-    def prices_to_features(self, prices):
+    def prices_to_features(
+        self,
+        prices: pd.DataFrame
+        ) -> tuple[
+            Union[
+                list[Union[pd.DataFrame, 'pd.Series[float]']],
+                dict[str, Union[pd.DataFrame, 'pd.Series[float]']]
+            ],
+            Union[pd.DataFrame, 'pd.Series[float]']]:
         """
         From a DataFrame of prices, return a tuple of features and targets to be
         provided to the machine learning model.
 
         The returned features can be a list or dict of DataFrames, where each
         DataFrame is a feature and should have the same shape, with a Date or
         (Date, Time) index and sids as columns. (Moonshot will convert the
@@ -238,89 +258,113 @@
         ----------
         prices : DataFrame, required
             multiindex (Field, Date) or (Field, Date, Time) DataFrame of
             price/market data
 
         Returns
         -------
-        dict or list of DataFrames or Series
-            features
+        tuple of (dict or list of DataFrames or Series, and DataFrame or Series)
+            features and targets
+
+        Notes
+        -----
+        Usage Guide:
+
+        * MoonshotML: https://qrok.it/dl/ms/moonshot-ml
 
         Examples
         --------
-        Predict next-day returns based on 1-day and 2-day returns:
+        Predict next-day returns based on 1-day and 2-day returns::
 
-        >>> def prices_to_features(self, prices):
-        >>>     closes = prices.loc["Close"]
-        >>>     features = {}
-        >>>     features["returns_1d"]= closes.pct_change()
-        >>>     features["returns_2d"] = (closes - closes.shift(2)) / closes.shift(2)
-        >>>     targets = closes.pct_change().shift(-1)
-        >>>     return features, targets
+            def prices_to_features(self, prices: pd.DataFrame):
+                closes = prices.loc["Close"]
+                features = {}
+                features["returns_1d"]= closes.pct_change()
+                features["returns_2d"] = (closes - closes.shift(2)) / closes.shift(2)
+                targets = closes.pct_change().shift(-1)
+                return features, targets
 
         Predict next-day returns for a single security in the prices
-        DataFrame using another security's returns:
+        DataFrame using another security's returns::
 
-        >>> def prices_to_features(self, prices):
-        >>>     closes = prices.loc["Close"]
-        >>>     closes_to_predict = closes[12345]
-        >>>     closes_to_predict_with = closes[23456]
-        >>>     features = {}
-        >>>     features["returns_1d"]= closes_to_predict_with.pct_change()
-        >>>     features["returns_2d"] = (closes_to_predict_with - closes_to_predict_with.shift(2)) / closes_to_predict_with.shift(2)
-        >>>     targets = closes_to_predict.pct_change().shift(-1)
-        >>>     return features, targets
+            def prices_to_features(self, prices: pd.DataFrame):
+                closes = prices.loc["Close"]
+                closes_to_predict = closes[12345]
+                closes_to_predict_with = closes[23456]
+                features = {}
+                features["returns_1d"]= closes_to_predict_with.pct_change()
+                features["returns_2d"] = (closes_to_predict_with - closes_to_predict_with.shift(2)) / closes_to_predict_with.shift(2)
+                targets = closes_to_predict.pct_change().shift(-1)
+                return features, targets
         """
         raise NotImplementedError("strategies must implement prices_to_features")
 
-    def predictions_to_signals(self, predictions, prices):
+    def predictions_to_signals(
+        self,
+        predictions: Union[pd.DataFrame, 'pd.Series[float]'],
+        prices: pd.DataFrame
+        ) -> pd.DataFrame:
         """
         From a DataFrame of predictions produced by a machine learning model,
         return a DataFrame of signals. By convention, signals should be
         1=long, 0=cash, -1=short.
 
         The index of predictions will match the index of the features
         DataFrames or Series returned in prices_to_features.
 
         Must be implemented by strategy subclasses.
 
         Parameters
         ----------
-        predictions : DataFrame, required
+        predictions : DataFrame or Series, required
             DataFrame of machine learning predictions
 
         prices : DataFrame, required
             multiindex (Field, Date) or (Field, Date, Time) DataFrame of
             price/market data
 
         Returns
         -------
         DataFrame
             signals
 
+        Notes
+        -----
+        Usage Guide:
+
+        * MoonshotML: https://qrok.it/dl/ms/moonshot-ml
+
         Examples
         --------
-        Buy when prediction (a DataFrame) is above zero.
+        Buy when prediction (a DataFrame) is above zero::
 
-        >>> def predictions_to_signals(self, predictions, prices):
-        >>>     signals = predictions > 0
-        >>>     return signals.astype(int)
-
-        Buy a single security when the predictions (a Series) is above zero.
-
-        >>> def predictions_to_signals(self, predictions, prices):
-        >>>     closes = prices.loc["Close"]
-        >>>     signals = pd.DataFrame(False, index=closes.index, columns=closes.columns)
-        >>>     signals.loc[:, 12345] = predictions > 0
-        >>>     return signals.astype(int)
+            def predictions_to_signals(self, predictions: pd.DataFrame, prices: pd.DataFrame):
+                signals = predictions > 0
+                return signals.astype(int)
+
+        Buy a single security when the predictions (a Series) is above zero::
+
+            def predictions_to_signals(self, predictions: pd.Series, prices: pd.DataFrame):
+                closes = prices.loc["Close"]
+                signals = pd.DataFrame(False, index=closes.index, columns=closes.columns)
+                signals.loc[:, 12345] = predictions > 0
+                return signals.astype(int)
         """
         raise NotImplementedError("strategies must implement predictions_to_signals")
 
-    def backtest(self, model=None, start_date=None, end_date=None, nlv=None,
-                allocation=1.0, label_sids=False, no_cache=False):
+    def backtest(
+        self,
+        model: Any = None,
+        start_date: str = None,
+        end_date: str = None,
+        nlv: dict[str, float] = None,
+        allocation: float = 1.0,
+        label_sids: bool = False,
+        no_cache: bool = False
+        ) -> pd.DataFrame:
         """
         Backtest a strategy and return a DataFrame of results.
 
         Parameters
         ----------
         model : object, optional
             machine learning model to use for predictions; if not specified,
@@ -468,15 +512,19 @@
         if unstack_predictions_series:
             predictions = predictions.unstack(level="Sid")
 
         # predictions to signals
         signals = self.predictions_to_signals(predictions, prices)
         return signals
 
-    def trade(self, allocations, review_date=None):
+    def trade(
+        self,
+        allocations: dict[str, float],
+        review_date: str = None
+        ) -> pd.DataFrame:
         """
         Run the strategy and create orders.
 
         Parameters
         ----------
         allocations : dict, required
             dict of account:allocation to strategy (expressed as a percentage of NLV)
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/strategies/__init__.py` & `quantrocket-moonshot-2.9.0.0/moonshot/strategies/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/cache.py` & `quantrocket-moonshot-2.9.0.0/moonshot/_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -31,15 +31,15 @@
 
     Examples
     --------
     Set and get a DataFrame from the cache based on the prices index and columns,
     in backtests only, and don't use the cache if the file containing the strategy
     code was modified more recently than the DataFrame was cached.
 
-    >>> from moonshot.cache import Cache
+    >>> from moonshot._cache import Cache
     >>>
     >>> class MyStrategy(Moonshot):
     >>>
     >>>     def prices_to_signals(self, prices):
     >>>
     >>>         my_dataframe = None
     >>>
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/commission/base.py` & `quantrocket-moonshot-2.9.0.0/moonshot/commission/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import pandas as pd
 
-class BaseCommission(object):
+class Commission(object):
     """
     Base class for all commission classes.
     """
-    MIN_COMMISSION = 0
+    MIN_COMMISSION: float = 0
+    """the minimum commission charged by the broker. Only enforced if NLVs are passed
+    by the backtest"""
 
     @classmethod
-    def get_commissions(cls, contract_values, turnover, nlvs=None):
+    def get_commissions(
+        cls,
+        contract_values: pd.DataFrame,
+        turnover: pd.DataFrame,
+        nlvs: pd.DataFrame = None
+        ) -> pd.DataFrame:
         """
         Returns a DataFrame of commissions.
 
 
         Parameters
         ----------
         contract_values : DataFrame, required
@@ -53,15 +61,15 @@
         """
         # Express the min commission as a percentage of NLV
         min_commissions = cls.MIN_COMMISSION / nlvs
         must_pay_min_commissions = (commissions > 0) & (commissions < min_commissions)
         commissions = commissions.where(must_pay_min_commissions == False, min_commissions)
         return commissions
 
-class PercentageCommission(BaseCommission):
+class PercentageCommission(Commission):
     """
     Base class for commissions which are a fixed percentage of the trade
     value. These commissions consist of a broker commission percentage rate
     (which might vary based on monthly trade volume) plus a fixed exchange
     fee percentage rate.
 
     This class can't be used directly but should be subclassed with the
@@ -95,22 +103,34 @@
     >>>     EXCHANGE_FEE_RATE = 0.000004
     >>>     MIN_COMMISSION = 80.00 # JPY
     >>>
     >>>  # then, use this on your strategy:
     >>>  class MyJapanStrategy(Moonshot):
     >>>      COMMISSION_CLASS = JapanStockCommission
     """
-    BROKER_COMMISSION_RATE = 0
-    BROKER_COMMISSION_RATE_TIER_2 = None
-    TIER_2_RATIO = None
-    EXCHANGE_FEE_RATE = 0
-    MIN_COMMISSION = 0
+    BROKER_COMMISSION_RATE: float = 0
+    """the commission rate (as a percentage of trade value) charged by the broker"""
+    BROKER_COMMISSION_RATE_TIER_2: float = None
+    """the commission rate (as a percentage of trade value) charged by the broker
+    at monthly volume tier 2"""
+    TIER_2_RATIO: float = None
+    """the ratio of monthly trades at volume tier 2 (default 0)"""
+    EXCHANGE_FEE_RATE: float = 0
+    """the exchange fee as a percentage of trade value"""
+    MIN_COMMISSION: float = 0
+    """the minimum commission charged by the broker. Only enforced if NLVs are passed
+    by the backtest."""
 
     @classmethod
-    def get_commissions(cls, contract_values, turnover, nlvs=None):
+    def get_commissions(
+        cls,
+        contract_values: pd.DataFrame,
+        turnover: pd.DataFrame,
+        nlvs: pd.DataFrame = None
+        ) -> pd.DataFrame:
         """
         Returns a DataFrame of commissions.
 
 
         Parameters
         ----------
         contract_values : DataFrame, required
@@ -147,11 +167,17 @@
         exchange_commissions = turnover * cls.EXCHANGE_FEE_RATE
 
         commissions = broker_commissions + exchange_commissions
 
         return commissions
 
 class NoCommission(PercentageCommission):
+    """
+    Commission class for strategies that don't pay commissions.
+    """
 
-    BROKER_COMMISSION_RATE = 0
-    EXCHANGE_FEE_RATE = 0
-    MIN_COMMISSION = 0
+    BROKER_COMMISSION_RATE: float = 0
+    """the commission rate (as a percentage of trade value) charged by the broker"""
+    EXCHANGE_FEE_RATE: float = 0
+    """the exchange fee as a percentage of trade value"""
+    MIN_COMMISSION: float = 0
+    """the minimum commission charged by the broker."""
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/commission/fx.py` & `quantrocket-moonshot-2.9.0.0/moonshot/commission/fx.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,25 +14,38 @@
 
 from moonshot.commission.base import PercentageCommission
 
 class SpotFXCommission(PercentageCommission):
     """
     Commission class for spot FX. This class can be used as-is.
 
-    NOTE: min commissions are not modeled for spot FX. This is because min
+    Notes
+    -----
+    Min commissions are not modeled for spot FX. This is because min
     commissions for spot FX are in USD ($2), regardless of the quote
     currency. The Moonshot class passes NLVs in the quote currency (the
     Currency field). To accurately model min commissions, these NLVs would need
     to be converted to USD.
 
+    Usage Guide:
+
+    * Moonshot commissions and slippage: https://qrok.it/dl/ms/moonshot-commissions-slippage
+
     Examples
     --------
     Use this on your strategy:
 
     >>>  class MyFXStrategy(Moonshot):
     >>>      COMMISSION_CLASS = SpotFXCommission
 
     """
 
-    BROKER_COMMISSION_RATE = 0.00002 # 0.2 bps
-    EXCHANGE_FEE_RATE = 0
-    MIN_COMMISSION = 0 # see NOTE in docstring
+    BROKER_COMMISSION_RATE: float = 0.00002 # 0.2 bps
+    """the commission rate (as a percentage of trade value) charged by the broker"""
+    EXCHANGE_FEE_RATE: float = 0
+    """the exchange fee as a percentage of trade value"""
+    MIN_COMMISSION: float = 0
+    """NOTE: min commissions are not modeled for spot FX. This is because min
+    commissions for spot FX are in USD ($2), regardless of the quote
+    currency. The Moonshot class passes NLVs in the quote currency (the
+    Currency field). To accurately model min commissions, these NLVs would need
+    to be converted to USD."""
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/commission/fut.py` & `quantrocket-moonshot-2.9.0.0/moonshot/commission/fut.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from moonshot.commission.base import BaseCommission, PercentageCommission
+from typing import Any
+import pandas as pd
+from moonshot.commission.base import Commission, PercentageCommission
 
-class FuturesCommission(BaseCommission):
+class FuturesCommission(Commission):
     """
     Base class for futures commissions.
 
     Parameters
     ----------
     BROKER_COMMISSION_PER_CONTRACT : float
         the commission per contract
@@ -26,80 +28,95 @@
     EXCHANGE_FEE_PER_CONTRACT : float
         the exchange and regulatory fees per contract
 
     CARRYING_FEE_PER_CONTRACT : float
         the overnight carrying fee per contract (depends on equity in excess of
         margin requirement)
 
+    Notes
+    -----
+    Usage Guide:
+
+    * Moonshot commissions and slippage: https://qrok.it/dl/ms/moonshot-commissions-slippage
+
     Examples
     --------
-    Example subclass for Globex E-Mini commissions:
+    Example subclass for CME E-Mini commissions:
 
-    >>> class GlobexEquityEMiniFixedCommission(FuturesCommission):
+    >>> class CMEEquityEMiniFixedCommission(FuturesCommission):
     >>>     BROKER_COMMISSION_PER_CONTRACT = 0.85
     >>>     EXCHANGE_FEE_PER_CONTRACT = 1.18
     >>>     CARRYING_FEE_PER_CONTRACT = 0 # Depends on equity in excess of margin requirement
     >>>
     >>>  # then, use this on your strategy:
     >>>  class MyEminiStrategy(Moonshot):
-    >>>      COMMISSION_CLASS = GlobexEquityEMiniFixedCommission
+    >>>      COMMISSION_CLASS = CMEEquityEMiniFixedCommission
     """
-    BROKER_COMMISSION_PER_CONTRACT = 0
-    EXCHANGE_FEE_PER_CONTRACT = 0
-    CARRYING_FEE_PER_CONTRACT = 0 # Depends on equity in excess of margin requirement
+    BROKER_COMMISSION_PER_CONTRACT: float = 0
+    """the commission per contract"""
+    EXCHANGE_FEE_PER_CONTRACT: float = 0
+    """the exchange and regulatory fees per contract"""
+    CARRYING_FEE_PER_CONTRACT: float = 0
+    """the overnight carrying fee per contract (depends on equity in excess of
+    margin requirement)"""
 
     @classmethod
-    def get_commissions(cls, contract_values, turnover, **kwargs):
+    def get_commissions(
+        cls,
+        contract_values: pd.DataFrame,
+        turnover: pd.DataFrame,
+        **kwargs: Any
+        ) -> pd.DataFrame:
         """
         Return a DataFrame of commissions as percentages of account equity.
         """
         cost_per_contract = cls.BROKER_COMMISSION_PER_CONTRACT + cls.EXCHANGE_FEE_PER_CONTRACT + cls.CARRYING_FEE_PER_CONTRACT
 
         # Express the commission as a percent of contract value
         commission_rates = float(cost_per_contract)/contract_values
 
         # Multipy the commission rates by the turnover
         commissions = commission_rates * turnover
 
         return commissions
 
-class DemoGlobexEquityEMiniFixedCommission(FuturesCommission):
+class DemoCMEEquityEMiniFixedCommission(FuturesCommission):
     """
-    Fixed commission for Globex Equity E-Minis.
+    Fixed commission for CME Equity E-Minis.
     """
-    BROKER_COMMISSION_PER_CONTRACT = 0.85
-    EXCHANGE_FEE_PER_CONTRACT = 1.18
-    CARRYING_FEE_PER_CONTRACT = 0
+    BROKER_COMMISSION_PER_CONTRACT: float = 0.85
+    EXCHANGE_FEE_PER_CONTRACT: float = 1.18
+    CARRYING_FEE_PER_CONTRACT: float = 0
 
 class DemoCanadaCADFuturesTieredCommission(FuturesCommission):
     """
     Tiered/Cost-Plus commission for Canada futures denominated in CAD, for US
     customers.
     """
 
-    BROKER_COMMISSION_PER_CONTRACT = 0.85
-    EXCHANGE_FEE_PER_CONTRACT = (
+    BROKER_COMMISSION_PER_CONTRACT: float = 0.85
+    EXCHANGE_FEE_PER_CONTRACT: float = (
         1.12   # exchange fee
         + 0.03 # regulatory fee
         + 0.01 # NFA assessment fee
     )
-    CARRYING_FEE_PER_CONTRACT = 0
+    CARRYING_FEE_PER_CONTRACT: float = 0
 
 class DemoKoreaFuturesCommission(PercentageCommission):
     """
     Fixed rate commission for Korea futures excluding stock futures.
     """
     # 0.4 bps fixed rate, excludes stock futures and KWY futures (US dollar)
 
-    BROKER_COMMISSION_RATE = 0.00004
-    EXCHANGE_FEE_RATE = 0
-    MIN_COMMISSION = 0
+    BROKER_COMMISSION_RATE: float = 0.00004
+    EXCHANGE_FEE_RATE: float = 0
+    MIN_COMMISSION: float = 0
 
 class DemoKoreaStockFuturesCommission(PercentageCommission):
     """
     Fixed rate commission for Korea stock futures.
     """
     # 4 bps fixed rate for stock futures
 
-    BROKER_COMMISSION_RATE = 0.0004
-    EXCHANGE_FEE_RATE = 0
-    MIN_COMMISSION = 0
+    BROKER_COMMISSION_RATE: float = 0.0004
+    EXCHANGE_FEE_RATE: float = 0
+    MIN_COMMISSION: float = 0
```

### Comparing `quantrocket-moonshot-2.8.0.1/moonshot/exceptions.py` & `quantrocket-moonshot-2.9.0.0/moonshot/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 QuantRocket LLC - All Rights Reserved
+# Copyright 2017-2023 QuantRocket LLC - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quantrocket-moonshot-2.8.0.1/README.md` & `quantrocket-moonshot-2.9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `quantrocket-moonshot-2.8.0.1/setup.py` & `quantrocket-moonshot-2.9.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 QuantRocket - All Rights Reserved
+# Copyright 2017-2023 QuantRocket - All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,19 +15,22 @@
 from setuptools import setup, find_packages
 import versioneer
 
 setup(name='quantrocket-moonshot',
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description='Moonshot',
-    long_description='Vectorized backtester and trading engine',
+    long_description='Vectorized backtesting and trading engine',
     url='https://www.quantrocket.com',
     author='QuantRocket LLC',
     author_email='support@quantrocket.com',
     license='Apache-2.0',
     packages=find_packages(),
-    package_data={"moonshot.tests.fixtures": ['*.h5']},
+    package_data={
+        "moonshot._tests.fixtures": ['*.h5'],
+        "moonshot": ["py.typed"],
+    },
     install_requires=[
         "quantrocket-client",
         "pandas"
     ]
 )
```

### Comparing `quantrocket-moonshot-2.8.0.1/quantrocket_moonshot.egg-info/SOURCES.txt` & `quantrocket-moonshot-2.9.0.0/quantrocket_moonshot.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 moonshot/__init__.py
+moonshot/_cache.py
 moonshot/_version.py
-moonshot/cache.py
 moonshot/exceptions.py
+moonshot/py.typed
+moonshot/_tests/__init__.py
+moonshot/_tests/test_allow_rebalance.py
+moonshot/_tests/test_backtest.py
+moonshot/_tests/test_benchmark.py
+moonshot/_tests/test_cache.py
+moonshot/_tests/test_commissions.py
+moonshot/_tests/test_limit_position_sizes.py
+moonshot/_tests/test_ml.py
+moonshot/_tests/test_orders.py
+moonshot/_tests/test_positions_closed_daily.py
+moonshot/_tests/test_prices.py
+moonshot/_tests/test_save_custom_dataframe.py
+moonshot/_tests/test_slippage.py
+moonshot/_tests/test_trade.py
+moonshot/_tests/test_trade_date_validation.py
+moonshot/_tests/test_weight_allocations.py
+moonshot/_tests/commission/__init__.py
+moonshot/_tests/commission/test_commissions.py
+moonshot/_tests/fixtures/__init__.py
+moonshot/_tests/fixtures/test_model.keras.h5
+moonshot/_tests/slippage/__init__.py
+moonshot/_tests/slippage/test_slippage.py
 moonshot/commission/__init__.py
 moonshot/commission/base.py
 moonshot/commission/fut.py
 moonshot/commission/fx.py
 moonshot/commission/stk.py
 moonshot/mixins/__init__.py
 moonshot/mixins/weight.py
 moonshot/slippage/__init__.py
+moonshot/slippage/base.py
 moonshot/slippage/borrowfee.py
 moonshot/slippage/fixed.py
 moonshot/strategies/__init__.py
 moonshot/strategies/base.py
 moonshot/strategies/ml.py
-moonshot/tests/__init__.py
-moonshot/tests/test_allow_rebalance.py
-moonshot/tests/test_backtest.py
-moonshot/tests/test_benchmark.py
-moonshot/tests/test_cache.py
-moonshot/tests/test_commissions.py
-moonshot/tests/test_limit_position_sizes.py
-moonshot/tests/test_ml.py
-moonshot/tests/test_orders.py
-moonshot/tests/test_positions_closed_daily.py
-moonshot/tests/test_prices.py
-moonshot/tests/test_save_custom_dataframe.py
-moonshot/tests/test_slippage.py
-moonshot/tests/test_trade.py
-moonshot/tests/test_trade_date_validation.py
-moonshot/tests/test_weight_allocations.py
-moonshot/tests/commission/__init__.py
-moonshot/tests/commission/test_commissions.py
-moonshot/tests/fixtures/__init__.py
-moonshot/tests/fixtures/test_model.keras.h5
-moonshot/tests/slippage/__init__.py
-moonshot/tests/slippage/test_slippage.py
 quantrocket_moonshot.egg-info/PKG-INFO
 quantrocket_moonshot.egg-info/SOURCES.txt
 quantrocket_moonshot.egg-info/dependency_links.txt
 quantrocket_moonshot.egg-info/requires.txt
 quantrocket_moonshot.egg-info/top_level.txt
```

### Comparing `quantrocket-moonshot-2.8.0.1/versioneer.py` & `quantrocket-moonshot-2.9.0.0/versioneer.py`

 * *Files identical despite different names*

