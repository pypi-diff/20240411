# Comparing `tmp/lumibot-3.3.5.tar.gz` & `tmp/lumibot-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumibot-3.3.5.tar", last modified: Wed Apr 10 20:58:06 2024, max compression
+gzip compressed data, was "lumibot-3.3.6.tar", last modified: Wed Apr 10 21:18:01 2024, max compression
```

## Comparing `lumibot-3.3.5.tar` & `lumibot-3.3.6.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.296119 lumibot-3.3.5/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.3.5/LICENSE
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-10 20:58:06.296043 lumibot-3.3.5/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.3.5/README.md
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.270434 lumibot-3.3.5/lumibot/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.273005 lumibot-3.3.5/lumibot/backtesting/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/alpaca_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/alpha_vantage_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    31444 2024-04-10 20:12:46.000000 lumibot-3.3.5/lumibot/backtesting/backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/ccxt_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/pandas_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15345 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/polygon_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/yahoo_backtesting.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.275425 lumibot-3.3.5/lumibot/brokers/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/brokers/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/brokers/alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    42451 2024-04-10 02:40:36.000000 lumibot-3.3.5/lumibot/brokers/broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-03-27 23:07:04.000000 lumibot-3.3.5/lumibot/brokers/ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/brokers/interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    27001 2024-04-10 20:52:06.000000 lumibot-3.3.5/lumibot/brokers/tradier.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.278881 lumibot-3.3.5/lumibot/data_sources/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/alpaca_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/alpha_vantage_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/ccxt_backtesting_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/ccxt_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15261 2024-04-03 02:08:33.000000 lumibot-3.3.5/lumibot/data_sources/data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.3.5/lumibot/data_sources/data_source_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/exceptions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/interactive_brokers_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15700 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/pandas_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9535 2024-04-07 08:26:01.000000 lumibot-3.3.5/lumibot/data_sources/tradier_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7022 2024-04-10 20:12:46.000000 lumibot-3.3.5/lumibot/data_sources/yahoo_data.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.281555 lumibot-3.3.5/lumibot/entities/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9174 2024-04-07 08:26:01.000000 lumibot-3.3.5/lumibot/entities/asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/bar.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/bars.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21354 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/dataline.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    28434 2024-04-10 20:12:46.000000 lumibot-3.3.5/lumibot/entities/order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/position.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/trading_fee.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.284073 lumibot-3.3.5/lumibot/example_strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/ccxt_backtesting_example.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/crypto_important_functions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2613 2024-04-10 20:12:46.000000 lumibot-3.3.5/lumibot/example_strategies/options_hold_to_expiry.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/simple_start_single_file.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/stock_bracket.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/stock_buy_and_hold.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/stock_diversified_leverage.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/stock_limit_and_trailing_stops.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/stock_momentum.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/stock_oco.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/strangle.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.285877 lumibot-3.3.5/lumibot/strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    53758 2024-03-31 04:01:24.000000 lumibot-3.3.5/lumibot/strategies/_strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)   149831 2024-04-10 04:58:08.000000 lumibot-3.3.5/lumibot/strategies/strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    39749 2024-04-10 20:12:46.000000 lumibot-3.3.5/lumibot/strategies/strategy_executor.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.289888 lumibot-3.3.5/lumibot/tools/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/black_scholes.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.3.5/lumibot/tools/ccxt_data_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/debugers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/decorators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/helpers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    26195 2024-04-10 20:29:05.000000 lumibot-3.3.5/lumibot/tools/indicators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/lumibot_time.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/pandas.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    19664 2024-04-07 08:25:48.000000 lumibot-3.3.5/lumibot/tools/polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/types.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15620 2024-04-10 20:12:46.000000 lumibot-3.3.5/lumibot/tools/yahoo_helper.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.290401 lumibot-3.3.5/lumibot/traders/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/traders/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7929 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/traders/trader.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.290995 lumibot-3.3.5/lumibot/trading_builtins/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/trading_builtins/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/trading_builtins/custom_stream.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/trading_builtins/safe_list.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.295686 lumibot-3.3.5/lumibot.egg-info/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-10 20:58:06.000000 lumibot-3.3.5/lumibot.egg-info/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3233 2024-04-10 20:58:06.000000 lumibot-3.3.5/lumibot.egg-info/SOURCES.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-04-10 20:58:06.000000 lumibot-3.3.5/lumibot.egg-info/dependency_links.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-04-10 20:58:06.000000 lumibot-3.3.5/lumibot.egg-info/requires.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-04-10 20:58:06.000000 lumibot-3.3.5/lumibot.egg-info/top_level.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.3.5/pyproject.toml
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-04-10 20:58:06.296538 lumibot-3.3.5/setup.cfg
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1865 2024-04-10 20:12:46.000000 lumibot-3.3.5/setup.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.293969 lumibot-3.3.5/tests/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.295486 lumibot-3.3.5/tests/backtest/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/backtest/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11425 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/backtest/test_example_strategies.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/backtest/test_main_pandas_daily.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12830 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/backtest/test_polygon.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/backtest/test_strategy_executor.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1909 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/backtest/test_yahoo.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_alpaca_old.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_ccxt_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      125 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4177 2024-04-10 20:12:46.000000 lumibot-3.3.5/tests/test_order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21416 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_strategy_methods.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    20786 2024-04-10 02:40:36.000000 lumibot-3.3.5/tests/test_tradier.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_tradingfee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.554721 lumibot-3.3.6/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.3.6/LICENSE
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-10 21:18:01.554644 lumibot-3.3.6/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.3.6/README.md
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.530472 lumibot-3.3.6/lumibot/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.532505 lumibot-3.3.6/lumibot/backtesting/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/backtesting/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/backtesting/alpaca_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/backtesting/alpha_vantage_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    31484 2024-04-10 21:16:31.000000 lumibot-3.3.6/lumibot/backtesting/backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/backtesting/ccxt_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/backtesting/pandas_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15345 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/backtesting/polygon_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/backtesting/yahoo_backtesting.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.535060 lumibot-3.3.6/lumibot/brokers/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/brokers/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/brokers/alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    42451 2024-04-10 02:40:36.000000 lumibot-3.3.6/lumibot/brokers/broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-03-27 23:07:04.000000 lumibot-3.3.6/lumibot/brokers/ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/brokers/interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    27001 2024-04-10 20:52:06.000000 lumibot-3.3.6/lumibot/brokers/tradier.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.538316 lumibot-3.3.6/lumibot/data_sources/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/data_sources/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/data_sources/alpaca_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/data_sources/alpha_vantage_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/data_sources/ccxt_backtesting_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/data_sources/ccxt_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15261 2024-04-03 02:08:33.000000 lumibot-3.3.6/lumibot/data_sources/data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.3.6/lumibot/data_sources/data_source_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/data_sources/exceptions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/data_sources/interactive_brokers_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15700 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/data_sources/pandas_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9535 2024-04-07 08:26:01.000000 lumibot-3.3.6/lumibot/data_sources/tradier_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7022 2024-04-10 20:12:46.000000 lumibot-3.3.6/lumibot/data_sources/yahoo_data.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.540938 lumibot-3.3.6/lumibot/entities/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/entities/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9174 2024-04-07 08:26:01.000000 lumibot-3.3.6/lumibot/entities/asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/entities/bar.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/entities/bars.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21354 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/entities/data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/entities/dataline.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    28434 2024-04-10 20:12:46.000000 lumibot-3.3.6/lumibot/entities/order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/entities/position.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/entities/trading_fee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.543255 lumibot-3.3.6/lumibot/example_strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/example_strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/example_strategies/ccxt_backtesting_example.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/example_strategies/crypto_important_functions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2613 2024-04-10 20:12:46.000000 lumibot-3.3.6/lumibot/example_strategies/options_hold_to_expiry.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/example_strategies/simple_start_single_file.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/example_strategies/stock_bracket.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/example_strategies/stock_buy_and_hold.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/example_strategies/stock_diversified_leverage.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/example_strategies/stock_limit_and_trailing_stops.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/example_strategies/stock_momentum.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/example_strategies/stock_oco.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/example_strategies/strangle.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.545104 lumibot-3.3.6/lumibot/strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    53758 2024-03-31 04:01:24.000000 lumibot-3.3.6/lumibot/strategies/_strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)   149831 2024-04-10 04:58:08.000000 lumibot-3.3.6/lumibot/strategies/strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    39749 2024-04-10 20:12:46.000000 lumibot-3.3.6/lumibot/strategies/strategy_executor.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.548822 lumibot-3.3.6/lumibot/tools/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/tools/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/tools/black_scholes.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.3.6/lumibot/tools/ccxt_data_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/tools/debugers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/tools/decorators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/tools/helpers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    26195 2024-04-10 20:29:05.000000 lumibot-3.3.6/lumibot/tools/indicators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/tools/lumibot_time.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/tools/pandas.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    19664 2024-04-07 08:25:48.000000 lumibot-3.3.6/lumibot/tools/polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/tools/types.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15620 2024-04-10 20:12:46.000000 lumibot-3.3.6/lumibot/tools/yahoo_helper.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.549209 lumibot-3.3.6/lumibot/traders/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/traders/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7929 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/traders/trader.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.549755 lumibot-3.3.6/lumibot/trading_builtins/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/trading_builtins/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/trading_builtins/custom_stream.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.3.6/lumibot/trading_builtins/safe_list.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.554266 lumibot-3.3.6/lumibot.egg-info/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-10 21:18:01.000000 lumibot-3.3.6/lumibot.egg-info/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3233 2024-04-10 21:18:01.000000 lumibot-3.3.6/lumibot.egg-info/SOURCES.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-04-10 21:18:01.000000 lumibot-3.3.6/lumibot.egg-info/dependency_links.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-04-10 21:18:01.000000 lumibot-3.3.6/lumibot.egg-info/requires.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-04-10 21:18:01.000000 lumibot-3.3.6/lumibot.egg-info/top_level.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.3.6/pyproject.toml
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-04-10 21:18:01.555157 lumibot-3.3.6/setup.cfg
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1865 2024-04-10 21:17:30.000000 lumibot-3.3.6/setup.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.552588 lumibot-3.3.6/tests/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 21:18:01.554020 lumibot-3.3.6/tests/backtest/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/backtest/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11425 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/backtest/test_example_strategies.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/backtest/test_main_pandas_daily.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12830 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/backtest/test_polygon.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/backtest/test_strategy_executor.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1909 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/backtest/test_yahoo.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/test_alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/test_alpaca_old.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/test_asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/test_backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/test_ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/test_ccxt_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      125 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/test_data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/test_interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4177 2024-04-10 20:12:46.000000 lumibot-3.3.6/tests/test_order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21416 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/test_polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/test_strategy_methods.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    20786 2024-04-10 02:40:36.000000 lumibot-3.3.6/tests/test_tradier.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.3.6/tests/test_tradingfee.py
```

### Comparing `lumibot-3.3.5/LICENSE` & `lumibot-3.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/PKG-INFO` & `lumibot-3.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.3.5
+Version: 3.3.6
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 Requires-Dist: flask-sqlalchemy
 Requires-Dist: flask-marshmallow
 Requires-Dist: flask-security
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: email_validator
 Requires-Dist: bcrypt
 Requires-Dist: pytest
-Requires-Dist: scipy==1.13.0
+Requires-Dist: scipy>=1.13.0
 Requires-Dist: ipython
 Requires-Dist: quantstats-lumi>=0.2.0
 Requires-Dist: python-dotenv
 Requires-Dist: ccxt==4.2.85
 Requires-Dist: termcolor
 Requires-Dist: jsonpickle
 Requires-Dist: apscheduler==3.10.4
```

### Comparing `lumibot-3.3.5/README.md` & `lumibot-3.3.6/README.md`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/__init__.py` & `lumibot-3.3.6/lumibot/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/backtesting/backtesting_broker.py` & `lumibot-3.3.6/lumibot/backtesting/backtesting_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,19 +564,19 @@
                     asset,
                     1,
                     quote=order.quote,
                     timeshift=timeshift,
                 )
 
                 dt = ohlc.df.index[-1]
-                open = ohlc.df.open[-1]
-                high = ohlc.df.high[-1]
-                low = ohlc.df.low[-1]
-                close = ohlc.df.close[-1]
-                volume = ohlc.df.volume[-1]
+                open = ohlc.df['open'].iloc[-1]
+                high = ohlc.df['high'].iloc[-1]
+                low = ohlc.df['low'].iloc[-1]
+                close = ohlc.df['close'].iloc[-1]
+                volume = ohlc.df['volume'].iloc[-1]
 
             # Get the OHLCV data for the asset if we're using the PANDAS data source
             elif self.data_source.SOURCE == "PANDAS":
                 # This is a hack to get around the fact that we need to get the previous day's data to prevent lookahead bias.
                 ohlc = strategy.get_historical_prices(
                     asset,
                     2,
```

### Comparing `lumibot-3.3.5/lumibot/backtesting/polygon_backtesting.py` & `lumibot-3.3.6/lumibot/backtesting/polygon_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/brokers/alpaca.py` & `lumibot-3.3.6/lumibot/brokers/alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/brokers/broker.py` & `lumibot-3.3.6/lumibot/brokers/broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/brokers/ccxt.py` & `lumibot-3.3.6/lumibot/brokers/ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/brokers/interactive_brokers.py` & `lumibot-3.3.6/lumibot/brokers/interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/brokers/tradier.py` & `lumibot-3.3.6/lumibot/brokers/tradier.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/data_sources/alpaca_data.py` & `lumibot-3.3.6/lumibot/data_sources/alpaca_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/data_sources/alpha_vantage_data.py` & `lumibot-3.3.6/lumibot/data_sources/alpha_vantage_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/data_sources/ccxt_backtesting_data.py` & `lumibot-3.3.6/lumibot/data_sources/ccxt_backtesting_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/data_sources/ccxt_data.py` & `lumibot-3.3.6/lumibot/data_sources/ccxt_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/data_sources/data_source.py` & `lumibot-3.3.6/lumibot/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/data_sources/data_source_backtesting.py` & `lumibot-3.3.6/lumibot/data_sources/data_source_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/data_sources/exceptions.py` & `lumibot-3.3.6/lumibot/data_sources/exceptions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/data_sources/interactive_brokers_data.py` & `lumibot-3.3.6/lumibot/data_sources/interactive_brokers_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/data_sources/pandas_data.py` & `lumibot-3.3.6/lumibot/data_sources/pandas_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/data_sources/tradier_data.py` & `lumibot-3.3.6/lumibot/data_sources/tradier_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/data_sources/yahoo_data.py` & `lumibot-3.3.6/lumibot/data_sources/yahoo_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/entities/asset.py` & `lumibot-3.3.6/lumibot/entities/asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/entities/bar.py` & `lumibot-3.3.6/lumibot/entities/bar.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/entities/bars.py` & `lumibot-3.3.6/lumibot/entities/bars.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/entities/data.py` & `lumibot-3.3.6/lumibot/entities/data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/entities/order.py` & `lumibot-3.3.6/lumibot/entities/order.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/entities/position.py` & `lumibot-3.3.6/lumibot/entities/position.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/entities/trading_fee.py` & `lumibot-3.3.6/lumibot/entities/trading_fee.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/example_strategies/ccxt_backtesting_example.py` & `lumibot-3.3.6/lumibot/example_strategies/ccxt_backtesting_example.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/example_strategies/crypto_important_functions.py` & `lumibot-3.3.6/lumibot/example_strategies/crypto_important_functions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/example_strategies/options_hold_to_expiry.py` & `lumibot-3.3.6/lumibot/example_strategies/options_hold_to_expiry.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/example_strategies/simple_start_single_file.py` & `lumibot-3.3.6/lumibot/example_strategies/simple_start_single_file.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/example_strategies/stock_bracket.py` & `lumibot-3.3.6/lumibot/example_strategies/stock_bracket.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/example_strategies/stock_buy_and_hold.py` & `lumibot-3.3.6/lumibot/example_strategies/stock_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/example_strategies/stock_diversified_leverage.py` & `lumibot-3.3.6/lumibot/example_strategies/stock_diversified_leverage.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/example_strategies/stock_limit_and_trailing_stops.py` & `lumibot-3.3.6/lumibot/example_strategies/stock_limit_and_trailing_stops.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/example_strategies/stock_momentum.py` & `lumibot-3.3.6/lumibot/example_strategies/stock_momentum.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/example_strategies/stock_oco.py` & `lumibot-3.3.6/lumibot/example_strategies/stock_oco.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/example_strategies/strangle.py` & `lumibot-3.3.6/lumibot/example_strategies/strangle.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/strategies/_strategy.py` & `lumibot-3.3.6/lumibot/strategies/_strategy.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/strategies/strategy.py` & `lumibot-3.3.6/lumibot/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/strategies/strategy_executor.py` & `lumibot-3.3.6/lumibot/strategies/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/tools/__init__.py` & `lumibot-3.3.6/lumibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/tools/black_scholes.py` & `lumibot-3.3.6/lumibot/tools/black_scholes.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/tools/ccxt_data_store.py` & `lumibot-3.3.6/lumibot/tools/ccxt_data_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/tools/decorators.py` & `lumibot-3.3.6/lumibot/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/tools/helpers.py` & `lumibot-3.3.6/lumibot/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/tools/indicators.py` & `lumibot-3.3.6/lumibot/tools/indicators.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/tools/lumibot_time.py` & `lumibot-3.3.6/lumibot/tools/lumibot_time.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/tools/pandas.py` & `lumibot-3.3.6/lumibot/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/tools/polygon_helper.py` & `lumibot-3.3.6/lumibot/tools/polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/tools/types.py` & `lumibot-3.3.6/lumibot/tools/types.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/tools/yahoo_helper.py` & `lumibot-3.3.6/lumibot/tools/yahoo_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/traders/trader.py` & `lumibot-3.3.6/lumibot/traders/trader.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/trading_builtins/custom_stream.py` & `lumibot-3.3.6/lumibot/trading_builtins/custom_stream.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot/trading_builtins/safe_list.py` & `lumibot-3.3.6/lumibot/trading_builtins/safe_list.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot.egg-info/PKG-INFO` & `lumibot-3.3.6/lumibot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.3.5
+Version: 3.3.6
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 Requires-Dist: flask-sqlalchemy
 Requires-Dist: flask-marshmallow
 Requires-Dist: flask-security
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: email_validator
 Requires-Dist: bcrypt
 Requires-Dist: pytest
-Requires-Dist: scipy==1.13.0
+Requires-Dist: scipy>=1.13.0
 Requires-Dist: ipython
 Requires-Dist: quantstats-lumi>=0.2.0
 Requires-Dist: python-dotenv
 Requires-Dist: ccxt==4.2.85
 Requires-Dist: termcolor
 Requires-Dist: jsonpickle
 Requires-Dist: apscheduler==3.10.4
```

### Comparing `lumibot-3.3.5/lumibot.egg-info/SOURCES.txt` & `lumibot-3.3.6/lumibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/lumibot.egg-info/requires.txt` & `lumibot-3.3.6/lumibot.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 flask-sqlalchemy
 flask-marshmallow
 flask-security
 marshmallow-sqlalchemy
 email_validator
 bcrypt
 pytest
-scipy==1.13.0
+scipy>=1.13.0
 ipython
 quantstats-lumi>=0.2.0
 python-dotenv
 ccxt==4.2.85
 termcolor
 jsonpickle
 apscheduler==3.10.4
```

### Comparing `lumibot-3.3.5/pyproject.toml` & `lumibot-3.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/setup.cfg` & `lumibot-3.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/setup.py` & `lumibot-3.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lumibot",
-    version="3.3.5",
+    version="3.3.6",
     author="Robert Grzesik",
     author_email="rob@lumiwealth.com",
     description="Backtesting and Trading Library, Made by Lumiwealth",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Lumiwealth/lumibot",
     packages=setuptools.find_packages(),
@@ -31,15 +31,15 @@
         "flask-sqlalchemy",
         "flask-marshmallow",
         "flask-security",
         "marshmallow-sqlalchemy",
         "email_validator",
         "bcrypt",
         "pytest",
-        "scipy==1.13.0",  # Newer versions of scipy are currently causing issues
+        "scipy>=1.13.0",  # Newer versions of scipy are currently causing issues
         "ipython",  # required for quantstats, but not in their dependency list for some reason
         "quantstats-lumi>=0.2.0",
         "python-dotenv",  # Secret Storage
         "ccxt==4.2.85",
         "termcolor",
         "jsonpickle",
         "apscheduler==3.10.4",
```

### Comparing `lumibot-3.3.5/tests/backtest/test_example_strategies.py` & `lumibot-3.3.6/tests/backtest/test_example_strategies.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/backtest/test_main_pandas_daily.py` & `lumibot-3.3.6/tests/backtest/test_main_pandas_daily.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/backtest/test_polygon.py` & `lumibot-3.3.6/tests/backtest/test_polygon.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/backtest/test_strategy_executor.py` & `lumibot-3.3.6/tests/backtest/test_strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/backtest/test_yahoo.py` & `lumibot-3.3.6/tests/backtest/test_yahoo.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/test_alpaca.py` & `lumibot-3.3.6/tests/test_alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/test_alpaca_old.py` & `lumibot-3.3.6/tests/test_alpaca_old.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/test_asset.py` & `lumibot-3.3.6/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/test_backtesting_broker.py` & `lumibot-3.3.6/tests/test_backtesting_broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/test_ccxt.py` & `lumibot-3.3.6/tests/test_ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/test_ccxt_store.py` & `lumibot-3.3.6/tests/test_ccxt_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/test_interactive_brokers.py` & `lumibot-3.3.6/tests/test_interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/test_order.py` & `lumibot-3.3.6/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/test_polygon_helper.py` & `lumibot-3.3.6/tests/test_polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/test_strategy_methods.py` & `lumibot-3.3.6/tests/test_strategy_methods.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.5/tests/test_tradier.py` & `lumibot-3.3.6/tests/test_tradier.py`

 * *Files identical despite different names*

