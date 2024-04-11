# Comparing `tmp/ccxt-4.2.94.tar.gz` & `tmp/ccxt-4.2.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ccxt-4.2.94.tar", last modified: Wed Apr 10 17:06:43 2024, max compression
+gzip compressed data, was "dist/ccxt-4.2.95.tar", last modified: Thu Apr 11 18:17:27 2024, max compression
```

## Comparing `ccxt-4.2.94.tar` & `ccxt-4.2.95.tar`

### file list

```diff
@@ -1,572 +1,572 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.396031 ccxt-4.2.94/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2024-04-10 17:05:38.000000 ccxt-4.2.94/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      101 2024-04-10 16:41:23.000000 ccxt-4.2.94/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)   114404 2024-04-10 17:06:43.400031 ccxt-4.2.94/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2024-04-10 16:41:23.000000 ccxt-4.2.94/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.148028 ccxt-4.2.94/ccxt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15656 2024-04-10 17:05:37.000000 ccxt-4.2.94/ccxt/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.188028 ccxt-4.2.94/ccxt/abstract/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/abstract/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10382 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11394 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4895 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91867 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91867 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    98587 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91867 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15876 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2735 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19194 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    89841 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3443 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14031 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10774 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9379 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27231 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3478 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3978 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      849 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1777 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48599 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14395 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4770 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7162 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34678 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6538 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6842 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8291 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8007 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18475 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7563 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11452 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6915 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      240 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2488 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5877 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3537 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25491 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27937 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24579 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8675 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25902 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3093 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9414 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45891 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2054 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15203 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8073 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5219 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19631 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8029 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10216 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-10 16:43:05.000000 ccxt-4.2.94/ccxt/abstract/zonda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41420 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46908 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151300 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.272029 ccxt-4.2.94/ccxt/async_support/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15409 2024-04-10 17:05:37.000000 ccxt-4.2.94/ccxt/async_support/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41644 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47120 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152088 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.276029 ccxt-4.2.94/ccxt/async_support/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91521 2024-04-10 17:05:37.000000 ccxt-4.2.94/ccxt/async_support/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/base/throttler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.280029 ccxt-4.2.94/ccxt/async_support/base/ws/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/base/ws/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5751 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/base/ws/aiohttp_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8100 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/base/ws/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/base/ws/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/base/ws/fast_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/base/ws/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/base/ws/future.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/base/ws/order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6478 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/base/ws/order_book_side.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1188 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92639 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   599459 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9177 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   182980 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37113 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41949 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48385 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      516 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71968 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   158863 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41694 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   414840 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45564 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   200023 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125968 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68685 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      485 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   136831 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71115 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92342 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102163 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91855 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20460 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    49180 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99698 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36828 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23535 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51678 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36724 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   403379 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70003 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   179388 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87677 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78883 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35719 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   247873 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103489 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46056 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80729 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46987 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    90866 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23615 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   128712 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87181 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151045 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   160915 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   168841 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   114835 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   316838 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      459 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80359 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   153853 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76327 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   420760 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      452 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88457 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92896 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73285 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32284 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52087 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   124519 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   116143 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   215759 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119121 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    96396 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79256 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115876 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45981 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51143 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35425 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   237552 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108892 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64473 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38180 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151629 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   356094 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88409 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54316 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24391 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   219437 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102496 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77756 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76600 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71498 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   123364 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23955 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82082 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   113950 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51493 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101482 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   132574 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53350 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28134 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80866 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/async_support/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.284030 ccxt-4.2.94/ccxt/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/base/decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4099 2024-04-10 16:52:49.000000 ccxt-4.2.94/ccxt/base/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   255276 2024-04-10 17:05:37.000000 ccxt-4.2.94/ccxt/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/base/precise.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7903 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/base/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1174 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92185 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   596881 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9163 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   181968 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36901 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41689 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48131 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      502 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71528 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   158129 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41386 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   413270 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45334 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   199103 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125408 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68281 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      471 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   136173 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70729 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91842 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101831 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91421 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20332 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48788 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99114 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36550 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23341 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51328 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36506 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   401635 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69653 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   178431 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87123 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78377 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35513 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   246603 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103001 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45790 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80409 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46745 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    90432 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23463 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   128158 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86759 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   150437 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   160139 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   167871 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   114203 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   315184 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79846 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152807 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75893 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   418422 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      438 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87957 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92412 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    72809 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32024 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51779 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   123935 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115673 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   214705 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   118519 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95980 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78780 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115164 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45643 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    50829 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35183 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   236392 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108368 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64105 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37860 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151105 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   354633 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87957 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54074 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24203 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   218625 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101948 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77370 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/poloniexfutures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.328030 ccxt-4.2.94/ccxt/pro/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6999 2024-04-10 17:05:37.000000 ccxt-4.2.94/ccxt/pro/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27167 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35432 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   136416 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      976 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2321 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42110 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24826 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42744 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71862 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16799 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62382 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68956 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18724 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      415 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16448 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20886 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56143 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29560 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75022 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    58370 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22578 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25428 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38945 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7789 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45042 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15652 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42643 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22355 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41035 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24527 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52489 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      391 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36641 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56285 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21957 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95779 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23174 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20613 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28282 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11063 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    60657 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63917 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    50705 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46006 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35100 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12348 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42551 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22643 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30385 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68821 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54634 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17877 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    61032 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51236 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41480 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22822 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9654 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30004 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35021 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37022 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/pro/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76208 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/probit.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.328030 ccxt-4.2.94/ccxt/static_dependencies/
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.332030 ccxt-4.2.94/ccxt/static_dependencies/ecdsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ecdsa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ecdsa/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ecdsa/curves.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ecdsa/der.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ecdsa/ecdsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ecdsa/ellipticcurve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ecdsa/keys.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ecdsa/numbertheory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ecdsa/rfc6979.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ecdsa/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.332030 ccxt-4.2.94/ccxt/static_dependencies/ethereum/
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.340030 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      490 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4861 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6871 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/codec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16828 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/decoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20162 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12358 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/grammar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/packed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)    19329 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/registry.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.340030 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5742 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.340030 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      426 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/utils/padding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      436 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/utils/string.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.344030 ccxt-4.2.94/ccxt/static_dependencies/ethereum/account/
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/account/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.344030 ccxt-4.2.94/ccxt/static_dependencies/ethereum/account/encode_typed_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7126 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      982 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10588 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/account/messages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/account/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.348030 ccxt-4.2.94/ccxt/static_dependencies/ethereum/hexbytes/
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/hexbytes/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/hexbytes/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.352030 ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/
--rw-rw-r--   0 travis    (2000) travis    (2000)      913 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      191 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/bls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/discovery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      458 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/enums.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      173 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/ethpm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      546 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/evm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20845 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/networks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.360031 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2162 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2123 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4364 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/address.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/applicators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5498 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/conversions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/currency.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.360031 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/curried/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6398 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      499 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/debug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3997 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/functional.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1826 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4137 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/humanize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5155 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/logging.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      842 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/module_loading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/numeric.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/toolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/types.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.364030 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/typing/
--rw-rw-r--   0 travis    (2000) travis    (2000)      325 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/typing/misc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1757 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/units.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.364030 ccxt-4.2.94/ccxt/static_dependencies/keccak/
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/keccak/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/keccak/keccak.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.364030 ccxt-4.2.94/ccxt/static_dependencies/msgpack/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/msgpack/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/msgpack/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5629 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/msgpack/ext.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33175 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/msgpack/fallback.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.368031 ccxt-4.2.94/ccxt/static_dependencies/parsimonious/
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/parsimonious/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3603 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/parsimonious/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16864 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/parsimonious/expressions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19190 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/parsimonious/grammar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13084 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/parsimonious/nodes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1087 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/parsimonious/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.372031 ccxt-4.2.94/ccxt/static_dependencies/toolz/
--rw-rw-r--   0 travis    (2000) travis    (2000)      374 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/toolz/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20555 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/toolz/_signatures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18447 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/toolz/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      997 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/toolz/compatibility.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.376031 ccxt-4.2.94/ccxt/static_dependencies/toolz/curried/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2226 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/toolz/curried/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      344 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/toolz/curried/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/toolz/curried/operator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8955 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/toolz/dicttoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29821 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/toolz/functoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27612 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/toolz/itertoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1256 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/toolz/recipes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/static_dependencies/toolz/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.376031 ccxt-4.2.94/ccxt/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/test/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.396031 ccxt-4.2.94/ccxt/test/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2024-04-10 16:52:54.000000 ccxt-4.2.94/ccxt/test/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      978 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2931 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_balance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_borrow_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_borrow_rate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/test/base/test_calculate_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2024-04-10 16:52:51.000000 ccxt-4.2.94/ccxt/test/base/test_crypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_currency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2024-04-10 16:52:50.000000 ccxt-4.2.94/ccxt/test/base/test_datetime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/test/base/test_decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/test/base/test_deep_extend.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_deposit_withdrawal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/test/base/test_exchange_datetime_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_funding_rate_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_last_price.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2283 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_ledger_entry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/test/base/test_ledger_item.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_leverage_tier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      869 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_margin_mode.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_margin_modification.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11632 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_market.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22083 2024-04-10 16:52:50.000000 ccxt-4.2.94/ccxt/test/base/test_number.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2036 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_ohlcv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_open_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3964 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_order.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3586 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3884 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_position.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19998 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_shared_methods.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      722 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/test/base/test_throttle.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5810 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_ticker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1066 2024-04-10 16:54:01.000000 ccxt-4.2.94/ccxt/test/base/test_trading_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/test/base/test_transaction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77013 2024-04-10 16:52:54.000000 ccxt-4.2.94/ccxt/test/test_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75994 2024-04-10 16:52:54.000000 ccxt-4.2.94/ccxt/test/test_sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71136 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   123002 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23761 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81600 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   113400 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51191 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   100934 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   131756 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53066 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27952 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80552 2024-04-10 16:41:23.000000 ccxt-4.2.94/ccxt/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-10 17:06:43.148028 ccxt-4.2.94/ccxt.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)   114404 2024-04-10 17:06:42.000000 ccxt-4.2.94/ccxt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    15741 2024-04-10 17:06:43.000000 ccxt-4.2.94/ccxt.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-10 17:06:42.000000 ccxt-4.2.94/ccxt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      218 2024-04-10 17:06:42.000000 ccxt-4.2.94/ccxt.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2024-04-10 17:06:42.000000 ccxt-4.2.94/ccxt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    12515 2024-04-10 17:05:38.000000 ccxt-4.2.94/package.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2024-04-10 17:06:43.400031 ccxt-4.2.94/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3071 2024-04-10 16:41:23.000000 ccxt-4.2.94/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.570912 ccxt-4.2.95/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2024-04-11 18:16:07.000000 ccxt-4.2.95/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      101 2024-04-11 17:44:13.000000 ccxt-4.2.95/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)   114404 2024-04-11 18:17:27.574912 ccxt-4.2.95/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2024-04-11 17:44:13.000000 ccxt-4.2.95/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.210885 ccxt-4.2.95/ccxt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15656 2024-04-11 18:16:06.000000 ccxt-4.2.95/ccxt/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.290891 ccxt-4.2.95/ccxt/abstract/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/abstract/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10382 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11394 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4895 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91867 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91867 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    98587 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91867 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15876 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2735 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19194 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89841 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3443 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14031 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10774 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9379 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27930 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3478 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3978 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      849 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1777 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48599 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14395 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4770 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7162 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34678 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6538 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6842 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8291 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8007 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18475 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7563 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11452 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6915 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      240 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2488 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5877 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3537 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25491 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27937 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24579 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8675 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25902 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3093 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9414 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45891 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2054 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15203 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8073 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5219 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19631 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8029 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10216 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-11 17:46:07.000000 ccxt-4.2.95/ccxt/abstract/zonda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41420 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46908 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151300 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.410900 ccxt-4.2.95/ccxt/async_support/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15409 2024-04-11 18:16:06.000000 ccxt-4.2.95/ccxt/async_support/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41644 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47120 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152088 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.414900 ccxt-4.2.95/ccxt/async_support/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91521 2024-04-11 18:16:06.000000 ccxt-4.2.95/ccxt/async_support/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/base/throttler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.418900 ccxt-4.2.95/ccxt/async_support/base/ws/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/base/ws/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5751 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/base/ws/aiohttp_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8100 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/base/ws/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/base/ws/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/base/ws/fast_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/base/ws/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/base/ws/future.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/base/ws/order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6478 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/base/ws/order_book_side.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1188 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92639 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   599459 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9177 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   182980 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37113 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41949 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48385 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      516 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71968 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   158863 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41694 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   414840 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45564 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   200023 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125968 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68685 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      485 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136831 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71115 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92615 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102163 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91855 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20460 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49180 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99698 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36828 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23535 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51678 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36724 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   403379 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70003 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   179388 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87677 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78883 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35719 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   248412 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103489 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46056 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80729 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46987 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90866 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23615 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   128712 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87181 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151045 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   160915 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   168841 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   114835 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   316838 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      459 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80424 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   153853 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76327 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   421631 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      452 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88457 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92896 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    73285 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32284 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52087 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   124519 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   116143 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   215759 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119121 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    96396 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79256 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115876 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45981 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51143 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35425 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   237552 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108892 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64473 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38180 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151629 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   356098 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88409 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54316 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24391 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   219437 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102496 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77756 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76600 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71498 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   123364 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23955 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82082 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113950 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51493 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101482 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   132574 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53350 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28134 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80866 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/async_support/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.422901 ccxt-4.2.95/ccxt/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/base/decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4107 2024-04-11 18:00:18.000000 ccxt-4.2.95/ccxt/base/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   255276 2024-04-11 18:16:06.000000 ccxt-4.2.95/ccxt/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/base/precise.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7903 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/base/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1174 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92185 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   596881 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9163 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   181968 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36901 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41689 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      478 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48131 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      502 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71528 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   158129 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41386 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   413270 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45334 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   199103 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125408 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68281 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      471 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136173 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70729 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92115 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101831 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91421 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20332 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48788 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99114 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36550 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23341 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51328 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36506 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   401635 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69653 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   178431 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87123 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78377 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35513 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   247142 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103001 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45790 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80409 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46745 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90432 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23463 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   128158 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86759 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   150437 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   160139 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   167871 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   114203 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   315184 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79911 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152807 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75893 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   419293 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      438 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87957 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92412 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    72809 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32024 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51779 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   123935 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115673 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   214705 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   118519 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95980 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78780 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115164 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45643 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50829 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35183 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   236392 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108368 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64105 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37860 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151105 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   354637 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87957 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54074 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24203 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   218625 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101948 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77370 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/poloniexfutures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.478905 ccxt-4.2.95/ccxt/pro/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6999 2024-04-11 18:16:06.000000 ccxt-4.2.95/ccxt/pro/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27167 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35432 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136416 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      976 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2321 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42110 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24826 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42744 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71862 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16799 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62382 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68956 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18724 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      415 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16448 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20886 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56143 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29560 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75022 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58370 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23630 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25428 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38945 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7789 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45042 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15652 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42643 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22355 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41035 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24527 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52489 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      391 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36641 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56285 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21957 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95779 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23174 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20613 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28282 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11063 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60657 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63917 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50705 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46006 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35100 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12348 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42551 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22643 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30385 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68821 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54634 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17877 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    61032 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51236 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41480 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22822 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9654 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30004 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35021 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37022 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/pro/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76208 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/probit.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.478905 ccxt-4.2.95/ccxt/static_dependencies/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       84 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.486905 ccxt-4.2.95/ccxt/static_dependencies/ecdsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ecdsa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ecdsa/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ecdsa/curves.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ecdsa/der.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ecdsa/ecdsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ecdsa/ellipticcurve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ecdsa/keys.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ecdsa/numbertheory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ecdsa/rfc6979.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ecdsa/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.486905 ccxt-4.2.95/ccxt/static_dependencies/ethereum/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.494906 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      276 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      490 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4861 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6871 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/codec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16828 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/decoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20162 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12358 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/grammar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/packed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/py.typed
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19329 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/registry.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.494906 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       65 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5742 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.498906 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      426 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/utils/padding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      436 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/utils/string.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.498906 ccxt-4.2.95/ccxt/static_dependencies/ethereum/account/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/account/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.502906 ccxt-4.2.95/ccxt/static_dependencies/ethereum/account/encode_typed_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7126 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      982 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10588 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/account/messages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/account/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.502906 ccxt-4.2.95/ccxt/static_dependencies/ethereum/hexbytes/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/hexbytes/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/hexbytes/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.510907 ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      913 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      191 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/bls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/discovery.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      117 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      458 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/enums.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      173 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/ethpm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      546 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/evm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20845 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/networks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.522908 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2162 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2123 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4364 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/address.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/applicators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5498 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/conversions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/currency.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.522908 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/curried/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6398 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      499 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/debug.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3997 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      199 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      110 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/functional.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1826 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4137 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/humanize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5155 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/logging.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      842 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/module_loading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/numeric.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/py.typed
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/toolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/types.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.526908 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/typing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      325 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      189 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/typing/misc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1757 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/units.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.526908 ccxt-4.2.95/ccxt/static_dependencies/keccak/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/keccak/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/keccak/keccak.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.530909 ccxt-4.2.95/ccxt/static_dependencies/msgpack/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/msgpack/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/msgpack/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5629 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/msgpack/ext.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33175 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/msgpack/fallback.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.534909 ccxt-4.2.95/ccxt/static_dependencies/parsimonious/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/parsimonious/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3603 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/parsimonious/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16864 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/parsimonious/expressions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19190 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/parsimonious/grammar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13084 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/parsimonious/nodes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1087 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/parsimonious/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.538909 ccxt-4.2.95/ccxt/static_dependencies/toolz/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      374 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/toolz/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20555 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/toolz/_signatures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18447 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/toolz/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      997 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/toolz/compatibility.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.542909 ccxt-4.2.95/ccxt/static_dependencies/toolz/curried/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2226 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/toolz/curried/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      344 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/toolz/curried/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/toolz/curried/operator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8955 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/toolz/dicttoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29821 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/toolz/functoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27612 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/toolz/itertoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1256 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/toolz/recipes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/static_dependencies/toolz/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.542909 ccxt-4.2.95/ccxt/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/test/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.566911 ccxt-4.2.95/ccxt/test/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2024-04-11 18:00:23.000000 ccxt-4.2.95/ccxt/test/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      978 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2931 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_balance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_borrow_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_borrow_rate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/test/base/test_calculate_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2024-04-11 18:00:20.000000 ccxt-4.2.95/ccxt/test/base/test_crypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_currency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2024-04-11 18:00:19.000000 ccxt-4.2.95/ccxt/test/base/test_datetime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/test/base/test_decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/test/base/test_deep_extend.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_deposit_withdrawal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/test/base/test_exchange_datetime_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_funding_rate_history.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_last_price.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2283 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_ledger_entry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/test/base/test_ledger_item.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_leverage_tier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      869 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_margin_mode.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_margin_modification.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11632 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_market.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22083 2024-04-11 18:00:19.000000 ccxt-4.2.95/ccxt/test/base/test_number.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2036 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_ohlcv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_open_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3964 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_order.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3586 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3884 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_position.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19998 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_shared_methods.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      722 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/test/base/test_throttle.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5810 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_ticker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_trade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1066 2024-04-11 18:01:48.000000 ccxt-4.2.95/ccxt/test/base/test_trading_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/test/base/test_transaction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77013 2024-04-11 18:00:23.000000 ccxt-4.2.95/ccxt/test/test_async.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75994 2024-04-11 18:00:23.000000 ccxt-4.2.95/ccxt/test/test_sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71136 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   123002 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23761 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81600 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113400 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51191 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   100934 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   131756 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53066 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27952 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80552 2024-04-11 17:44:13.000000 ccxt-4.2.95/ccxt/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 18:17:27.214885 ccxt-4.2.95/ccxt.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)   114404 2024-04-11 18:17:26.000000 ccxt-4.2.95/ccxt.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15741 2024-04-11 18:17:26.000000 ccxt-4.2.95/ccxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-11 18:17:26.000000 ccxt-4.2.95/ccxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      218 2024-04-11 18:17:26.000000 ccxt-4.2.95/ccxt.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2024-04-11 18:17:26.000000 ccxt-4.2.95/ccxt.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12515 2024-04-11 18:16:07.000000 ccxt-4.2.95/package.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      205 2024-04-11 18:17:27.578912 ccxt-4.2.95/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3071 2024-04-11 17:44:13.000000 ccxt-4.2.95/setup.py
```

### Comparing `ccxt-4.2.94/LICENSE.txt` & `ccxt-4.2.95/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/PKG-INFO` & `ccxt-4.2.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 4.2.94
+Version: 4.2.95
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 100+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
@@ -221,21 +221,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.2.94/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@4.2.94/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.2.95/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@4.2.95/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.2.94/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.2.95/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-4.2.94/README.rst` & `ccxt-4.2.95/README.rst`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/__init__.py` & `ccxt-4.2.95/ccxt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # ----------------------------------------------------------------------------
 
-__version__ = '4.2.94'
+__version__ = '4.2.95'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.base.exchange import Exchange                     # noqa: F401
 from ccxt.base.precise import Precise                       # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
@@ -64,23 +64,23 @@
 from ccxt.base.errors import CancelPending                            # noqa: F401
 from ccxt.base.errors import OrderImmediatelyFillable                 # noqa: F401
 from ccxt.base.errors import OrderNotFillable                         # noqa: F401
 from ccxt.base.errors import DuplicateOrderId                         # noqa: F401
 from ccxt.base.errors import ContractUnavailable                      # noqa: F401
 from ccxt.base.errors import NotSupported                             # noqa: F401
 from ccxt.base.errors import ProxyError                               # noqa: F401
+from ccxt.base.errors import ExchangeClosedByUser                     # noqa: F401
 from ccxt.base.errors import OperationFailed                          # noqa: F401
 from ccxt.base.errors import NetworkError                             # noqa: F401
 from ccxt.base.errors import DDoSProtection                           # noqa: F401
 from ccxt.base.errors import RateLimitExceeded                        # noqa: F401
 from ccxt.base.errors import ExchangeNotAvailable                     # noqa: F401
 from ccxt.base.errors import OnMaintenance                            # noqa: F401
 from ccxt.base.errors import InvalidNonce                             # noqa: F401
 from ccxt.base.errors import RequestTimeout                           # noqa: F401
-from ccxt.base.errors import ExchangeClosedByUser                     # noqa: F401
 from ccxt.base.errors import error_hierarchy                          # noqa: F401
 
 from ccxt.ace import ace                                              # noqa: F401
 from ccxt.alpaca import alpaca                                        # noqa: F401
 from ccxt.ascendex import ascendex                                    # noqa: F401
 from ccxt.bequant import bequant                                      # noqa: F401
 from ccxt.bigone import bigone                                        # noqa: F401
```

### Comparing `ccxt-4.2.94/ccxt/abstract/ace.py` & `ccxt-4.2.95/ccxt/abstract/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/alpaca.py` & `ccxt-4.2.95/ccxt/abstract/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/ascendex.py` & `ccxt-4.2.95/ccxt/abstract/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bequant.py` & `ccxt-4.2.95/ccxt/abstract/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bigone.py` & `ccxt-4.2.95/ccxt/abstract/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/binance.py` & `ccxt-4.2.95/ccxt/abstract/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/binancecoinm.py` & `ccxt-4.2.95/ccxt/abstract/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/binanceus.py` & `ccxt-4.2.95/ccxt/abstract/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/binanceusdm.py` & `ccxt-4.2.95/ccxt/abstract/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bingx.py` & `ccxt-4.2.95/ccxt/abstract/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bit2c.py` & `ccxt-4.2.95/ccxt/abstract/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitbank.py` & `ccxt-4.2.95/ccxt/abstract/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitbay.py` & `ccxt-4.2.95/ccxt/abstract/bitbay.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitbns.py` & `ccxt-4.2.95/ccxt/abstract/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitcoincom.py` & `ccxt-4.2.95/ccxt/abstract/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitfinex.py` & `ccxt-4.2.95/ccxt/abstract/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitfinex2.py` & `ccxt-4.2.95/ccxt/abstract/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitflyer.py` & `ccxt-4.2.95/ccxt/abstract/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitget.py` & `ccxt-4.2.95/ccxt/abstract/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bithumb.py` & `ccxt-4.2.95/ccxt/abstract/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitmart.py` & `ccxt-4.2.95/ccxt/abstract/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitmex.py` & `ccxt-4.2.95/ccxt/abstract/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitopro.py` & `ccxt-4.2.95/ccxt/abstract/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitpanda.py` & `ccxt-4.2.95/ccxt/abstract/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitrue.py` & `ccxt-4.2.95/ccxt/abstract/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitso.py` & `ccxt-4.2.95/ccxt/abstract/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitstamp.py` & `ccxt-4.2.95/ccxt/abstract/bitstamp.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,7 +230,13 @@
     private_post_lmwr_address = privatePostLmwrAddress = Entry('lmwr_address/', 'private', 'POST', {'cost': 1})
     private_post_pepe_withdrawal = privatePostPepeWithdrawal = Entry('pepe_withdrawal/', 'private', 'POST', {'cost': 1})
     private_post_pepe_address = privatePostPepeAddress = Entry('pepe_address/', 'private', 'POST', {'cost': 1})
     private_post_blur_withdrawal = privatePostBlurWithdrawal = Entry('blur_withdrawal/', 'private', 'POST', {'cost': 1})
     private_post_blur_address = privatePostBlurAddress = Entry('blur_address/', 'private', 'POST', {'cost': 1})
     private_post_vext_withdrawal = privatePostVextWithdrawal = Entry('vext_withdrawal/', 'private', 'POST', {'cost': 1})
     private_post_vext_address = privatePostVextAddress = Entry('vext_address/', 'private', 'POST', {'cost': 1})
+    private_post_cspr_withdrawal = privatePostCsprWithdrawal = Entry('cspr_withdrawal/', 'private', 'POST', {'cost': 1})
+    private_post_cspr_address = privatePostCsprAddress = Entry('cspr_address/', 'private', 'POST', {'cost': 1})
+    private_post_vchf_withdrawal = privatePostVchfWithdrawal = Entry('vchf_withdrawal/', 'private', 'POST', {'cost': 1})
+    private_post_vchf_address = privatePostVchfAddress = Entry('vchf_address/', 'private', 'POST', {'cost': 1})
+    private_post_veur_withdrawal = privatePostVeurWithdrawal = Entry('veur_withdrawal/', 'private', 'POST', {'cost': 1})
+    private_post_veur_address = privatePostVeurAddress = Entry('veur_address/', 'private', 'POST', {'cost': 1})
```

### Comparing `ccxt-4.2.94/ccxt/abstract/bitteam.py` & `ccxt-4.2.95/ccxt/abstract/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bitvavo.py` & `ccxt-4.2.95/ccxt/abstract/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bl3p.py` & `ccxt-4.2.95/ccxt/abstract/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/blockchaincom.py` & `ccxt-4.2.95/ccxt/abstract/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/blofin.py` & `ccxt-4.2.95/ccxt/abstract/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/btcalpha.py` & `ccxt-4.2.95/ccxt/abstract/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/btcbox.py` & `ccxt-4.2.95/ccxt/abstract/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/btcmarkets.py` & `ccxt-4.2.95/ccxt/abstract/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/btcturk.py` & `ccxt-4.2.95/ccxt/abstract/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/bybit.py` & `ccxt-4.2.95/ccxt/abstract/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/cex.py` & `ccxt-4.2.95/ccxt/abstract/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/coinbase.py` & `ccxt-4.2.95/ccxt/abstract/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/coinbaseinternational.py` & `ccxt-4.2.95/ccxt/abstract/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/coinbasepro.py` & `ccxt-4.2.95/ccxt/abstract/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/coincheck.py` & `ccxt-4.2.95/ccxt/abstract/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/coinex.py` & `ccxt-4.2.95/ccxt/abstract/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/coinlist.py` & `ccxt-4.2.95/ccxt/abstract/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/coinmate.py` & `ccxt-4.2.95/ccxt/abstract/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/coinmetro.py` & `ccxt-4.2.95/ccxt/abstract/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/coinone.py` & `ccxt-4.2.95/ccxt/abstract/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/coinsph.py` & `ccxt-4.2.95/ccxt/abstract/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/coinspot.py` & `ccxt-4.2.95/ccxt/abstract/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/cryptocom.py` & `ccxt-4.2.95/ccxt/abstract/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/currencycom.py` & `ccxt-4.2.95/ccxt/abstract/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/delta.py` & `ccxt-4.2.95/ccxt/abstract/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/deribit.py` & `ccxt-4.2.95/ccxt/abstract/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/digifinex.py` & `ccxt-4.2.95/ccxt/abstract/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/exmo.py` & `ccxt-4.2.95/ccxt/abstract/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/fmfwio.py` & `ccxt-4.2.95/ccxt/abstract/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/gate.py` & `ccxt-4.2.95/ccxt/abstract/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/gateio.py` & `ccxt-4.2.95/ccxt/abstract/gateio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/gemini.py` & `ccxt-4.2.95/ccxt/abstract/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/hitbtc.py` & `ccxt-4.2.95/ccxt/abstract/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/hitbtc3.py` & `ccxt-4.2.95/ccxt/abstract/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/hollaex.py` & `ccxt-4.2.95/ccxt/abstract/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/htx.py` & `ccxt-4.2.95/ccxt/abstract/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/huobi.py` & `ccxt-4.2.95/ccxt/abstract/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/huobijp.py` & `ccxt-4.2.95/ccxt/abstract/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/idex.py` & `ccxt-4.2.95/ccxt/abstract/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/independentreserve.py` & `ccxt-4.2.95/ccxt/abstract/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/indodax.py` & `ccxt-4.2.95/ccxt/abstract/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/kraken.py` & `ccxt-4.2.95/ccxt/abstract/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/krakenfutures.py` & `ccxt-4.2.95/ccxt/abstract/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/kucoin.py` & `ccxt-4.2.95/ccxt/abstract/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/kucoinfutures.py` & `ccxt-4.2.95/ccxt/abstract/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/kuna.py` & `ccxt-4.2.95/ccxt/abstract/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/latoken.py` & `ccxt-4.2.95/ccxt/abstract/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/lbank.py` & `ccxt-4.2.95/ccxt/abstract/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/luno.py` & `ccxt-4.2.95/ccxt/abstract/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/lykke.py` & `ccxt-4.2.95/ccxt/abstract/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/mercado.py` & `ccxt-4.2.95/ccxt/abstract/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/mexc.py` & `ccxt-4.2.95/ccxt/abstract/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/ndax.py` & `ccxt-4.2.95/ccxt/abstract/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/novadax.py` & `ccxt-4.2.95/ccxt/abstract/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/oceanex.py` & `ccxt-4.2.95/ccxt/abstract/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/okcoin.py` & `ccxt-4.2.95/ccxt/abstract/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/okx.py` & `ccxt-4.2.95/ccxt/abstract/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/onetrading.py` & `ccxt-4.2.95/ccxt/abstract/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/p2b.py` & `ccxt-4.2.95/ccxt/abstract/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/paymium.py` & `ccxt-4.2.95/ccxt/abstract/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/phemex.py` & `ccxt-4.2.95/ccxt/abstract/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/poloniex.py` & `ccxt-4.2.95/ccxt/abstract/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/poloniexfutures.py` & `ccxt-4.2.95/ccxt/abstract/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/probit.py` & `ccxt-4.2.95/ccxt/abstract/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/timex.py` & `ccxt-4.2.95/ccxt/abstract/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/tokocrypto.py` & `ccxt-4.2.95/ccxt/abstract/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/tradeogre.py` & `ccxt-4.2.95/ccxt/abstract/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/upbit.py` & `ccxt-4.2.95/ccxt/abstract/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/wavesexchange.py` & `ccxt-4.2.95/ccxt/abstract/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/wazirx.py` & `ccxt-4.2.95/ccxt/abstract/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/whitebit.py` & `ccxt-4.2.95/ccxt/abstract/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/woo.py` & `ccxt-4.2.95/ccxt/abstract/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/yobit.py` & `ccxt-4.2.95/ccxt/abstract/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/zaif.py` & `ccxt-4.2.95/ccxt/abstract/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/abstract/zonda.py` & `ccxt-4.2.95/ccxt/abstract/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/ace.py` & `ccxt-4.2.95/ccxt/ace.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.ace import ImplicitAPI
 from ccxt.base.types import Balances, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class ace(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/alpaca.py` & `ccxt-4.2.95/ccxt/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/ascendex.py` & `ccxt-4.2.95/ccxt/ascendex.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,35 +35,35 @@
 00000220: 6e73 6163 7469 6f6e 2c20 5472 616e 7366  nsaction, Transf
 00000230: 6572 456e 7472 790a 6672 6f6d 2074 7970  erEntry.from typ
 00000240: 696e 6720 696d 706f 7274 204c 6973 740a  ing import List.
 00000250: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
 00000260: 7272 6f72 7320 696d 706f 7274 2045 7863  rrors import Exc
 00000270: 6861 6e67 6545 7272 6f72 0a66 726f 6d20  hangeError.from 
 00000280: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-00000290: 2069 6d70 6f72 7420 5065 726d 6973 7369   import Permissi
-000002a0: 6f6e 4465 6e69 6564 0a66 726f 6d20 6363  onDenied.from cc
-000002b0: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
-000002c0: 6d70 6f72 7420 4172 6775 6d65 6e74 7352  mport ArgumentsR
-000002d0: 6571 7569 7265 640a 6672 6f6d 2063 6378  equired.from ccx
-000002e0: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
-000002f0: 706f 7274 2042 6164 5265 7175 6573 740a  port BadRequest.
-00000300: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-00000310: 7272 6f72 7320 696d 706f 7274 2042 6164  rrors import Bad
-00000320: 5379 6d62 6f6c 0a66 726f 6d20 6363 7874  Symbol.from ccxt
-00000330: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000340: 6f72 7420 496e 7375 6666 6963 6965 6e74  ort Insufficient
-00000350: 4675 6e64 730a 6672 6f6d 2063 6378 742e  Funds.from ccxt.
-00000360: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-00000370: 7274 2049 6e76 616c 6964 4f72 6465 720a  rt InvalidOrder.
-00000380: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-00000390: 7272 6f72 7320 696d 706f 7274 204e 6f74  rrors import Not
-000003a0: 5375 7070 6f72 7465 640a 6672 6f6d 2063  Supported.from c
-000003b0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-000003c0: 696d 706f 7274 2041 7574 6865 6e74 6963  import Authentic
-000003d0: 6174 696f 6e45 7272 6f72 0a66 726f 6d20  ationError.from 
+00000290: 2069 6d70 6f72 7420 4175 7468 656e 7469   import Authenti
+000002a0: 6361 7469 6f6e 4572 726f 720a 6672 6f6d  cationError.from
+000002b0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+000002c0: 7320 696d 706f 7274 2050 6572 6d69 7373  s import Permiss
+000002d0: 696f 6e44 656e 6965 640a 6672 6f6d 2063  ionDenied.from c
+000002e0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+000002f0: 696d 706f 7274 2041 7267 756d 656e 7473  import Arguments
+00000300: 5265 7175 6972 6564 0a66 726f 6d20 6363  Required.from cc
+00000310: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
+00000320: 6d70 6f72 7420 4261 6452 6571 7565 7374  mport BadRequest
+00000330: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
+00000340: 6572 726f 7273 2069 6d70 6f72 7420 4261  errors import Ba
+00000350: 6453 796d 626f 6c0a 6672 6f6d 2063 6378  dSymbol.from ccx
+00000360: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+00000370: 706f 7274 2049 6e73 7566 6669 6369 656e  port Insufficien
+00000380: 7446 756e 6473 0a66 726f 6d20 6363 7874  tFunds.from ccxt
+00000390: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+000003a0: 6f72 7420 496e 7661 6c69 644f 7264 6572  ort InvalidOrder
+000003b0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
+000003c0: 6572 726f 7273 2069 6d70 6f72 7420 4e6f  errors import No
+000003d0: 7453 7570 706f 7274 6564 0a66 726f 6d20  tSupported.from 
 000003e0: 6363 7874 2e62 6173 652e 6465 6369 6d61  ccxt.base.decima
 000003f0: 6c5f 746f 5f70 7265 6369 7369 6f6e 2069  l_to_precision i
 00000400: 6d70 6f72 7420 5449 434b 5f53 495a 450a  mport TICK_SIZE.
 00000410: 6672 6f6d 2063 6378 742e 6261 7365 2e70  from ccxt.base.p
 00000420: 7265 6369 7365 2069 6d70 6f72 7420 5072  recise import Pr
 00000430: 6563 6973 650a 0a0a 636c 6173 7320 6173  ecise...class as
 00000440: 6365 6e64 6578 2845 7863 6861 6e67 652c  cendex(Exchange,
```

### Comparing `ccxt-4.2.94/ccxt/async_support/__init__.py` & `ccxt-4.2.95/ccxt/async_support/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.2.94'
+__version__ = '4.2.95'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange                   # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
 from ccxt.base.decimal_to_precision import TRUNCATE              # noqa: F401
@@ -43,23 +43,23 @@
 from ccxt.base.errors import CancelPending                            # noqa: F401
 from ccxt.base.errors import OrderImmediatelyFillable                 # noqa: F401
 from ccxt.base.errors import OrderNotFillable                         # noqa: F401
 from ccxt.base.errors import DuplicateOrderId                         # noqa: F401
 from ccxt.base.errors import ContractUnavailable                      # noqa: F401
 from ccxt.base.errors import NotSupported                             # noqa: F401
 from ccxt.base.errors import ProxyError                               # noqa: F401
+from ccxt.base.errors import ExchangeClosedByUser                     # noqa: F401
 from ccxt.base.errors import OperationFailed                          # noqa: F401
 from ccxt.base.errors import NetworkError                             # noqa: F401
 from ccxt.base.errors import DDoSProtection                           # noqa: F401
 from ccxt.base.errors import RateLimitExceeded                        # noqa: F401
 from ccxt.base.errors import ExchangeNotAvailable                     # noqa: F401
 from ccxt.base.errors import OnMaintenance                            # noqa: F401
 from ccxt.base.errors import InvalidNonce                             # noqa: F401
 from ccxt.base.errors import RequestTimeout                           # noqa: F401
-from ccxt.base.errors import ExchangeClosedByUser                     # noqa: F401
 from ccxt.base.errors import error_hierarchy                          # noqa: F401
 
 
 from ccxt.async_support.ace import ace                                          # noqa: F401
 from ccxt.async_support.alpaca import alpaca                                    # noqa: F401
 from ccxt.async_support.ascendex import ascendex                                # noqa: F401
 from ccxt.async_support.bequant import bequant                                  # noqa: F401
```

### Comparing `ccxt-4.2.94/ccxt/async_support/ace.py` & `ccxt-4.2.95/ccxt/async_support/ace.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.ace import ImplicitAPI
 from ccxt.base.types import Balances, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class ace(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/alpaca.py` & `ccxt-4.2.95/ccxt/async_support/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/ascendex.py` & `ccxt-4.2.95/ccxt/async_support/ascendex.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,35 +36,35 @@
 00000230: 6163 7469 6f6e 2c20 5472 616e 7366 6572  action, Transfer
 00000240: 456e 7472 790a 6672 6f6d 2074 7970 696e  Entry.from typin
 00000250: 6720 696d 706f 7274 204c 6973 740a 6672  g import List.fr
 00000260: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
 00000270: 6f72 7320 696d 706f 7274 2045 7863 6861  ors import Excha
 00000280: 6e67 6545 7272 6f72 0a66 726f 6d20 6363  ngeError.from cc
 00000290: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
-000002a0: 6d70 6f72 7420 5065 726d 6973 7369 6f6e  mport Permission
-000002b0: 4465 6e69 6564 0a66 726f 6d20 6363 7874  Denied.from ccxt
-000002c0: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-000002d0: 6f72 7420 4172 6775 6d65 6e74 7352 6571  ort ArgumentsReq
-000002e0: 7569 7265 640a 6672 6f6d 2063 6378 742e  uired.from ccxt.
-000002f0: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-00000300: 7274 2042 6164 5265 7175 6573 740a 6672  rt BadRequest.fr
-00000310: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-00000320: 6f72 7320 696d 706f 7274 2042 6164 5379  ors import BadSy
-00000330: 6d62 6f6c 0a66 726f 6d20 6363 7874 2e62  mbol.from ccxt.b
-00000340: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
-00000350: 7420 496e 7375 6666 6963 6965 6e74 4675  t InsufficientFu
-00000360: 6e64 730a 6672 6f6d 2063 6378 742e 6261  nds.from ccxt.ba
-00000370: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000380: 2049 6e76 616c 6964 4f72 6465 720a 6672   InvalidOrder.fr
-00000390: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-000003a0: 6f72 7320 696d 706f 7274 204e 6f74 5375  ors import NotSu
-000003b0: 7070 6f72 7465 640a 6672 6f6d 2063 6378  pported.from ccx
-000003c0: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
-000003d0: 706f 7274 2041 7574 6865 6e74 6963 6174  port Authenticat
-000003e0: 696f 6e45 7272 6f72 0a66 726f 6d20 6363  ionError.from cc
+000002a0: 6d70 6f72 7420 4175 7468 656e 7469 6361  mport Authentica
+000002b0: 7469 6f6e 4572 726f 720a 6672 6f6d 2063  tionError.from c
+000002c0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+000002d0: 696d 706f 7274 2050 6572 6d69 7373 696f  import Permissio
+000002e0: 6e44 656e 6965 640a 6672 6f6d 2063 6378  nDenied.from ccx
+000002f0: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+00000300: 706f 7274 2041 7267 756d 656e 7473 5265  port ArgumentsRe
+00000310: 7175 6972 6564 0a66 726f 6d20 6363 7874  quired.from ccxt
+00000320: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+00000330: 6f72 7420 4261 6452 6571 7565 7374 0a66  ort BadRequest.f
+00000340: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+00000350: 726f 7273 2069 6d70 6f72 7420 4261 6453  rors import BadS
+00000360: 796d 626f 6c0a 6672 6f6d 2063 6378 742e  ymbol.from ccxt.
+00000370: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
+00000380: 7274 2049 6e73 7566 6669 6369 656e 7446  rt InsufficientF
+00000390: 756e 6473 0a66 726f 6d20 6363 7874 2e62  unds.from ccxt.b
+000003a0: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+000003b0: 7420 496e 7661 6c69 644f 7264 6572 0a66  t InvalidOrder.f
+000003c0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+000003d0: 726f 7273 2069 6d70 6f72 7420 4e6f 7453  rors import NotS
+000003e0: 7570 706f 7274 6564 0a66 726f 6d20 6363  upported.from cc
 000003f0: 7874 2e62 6173 652e 6465 6369 6d61 6c5f  xt.base.decimal_
 00000400: 746f 5f70 7265 6369 7369 6f6e 2069 6d70  to_precision imp
 00000410: 6f72 7420 5449 434b 5f53 495a 450a 6672  ort TICK_SIZE.fr
 00000420: 6f6d 2063 6378 742e 6261 7365 2e70 7265  om ccxt.base.pre
 00000430: 6369 7365 2069 6d70 6f72 7420 5072 6563  cise import Prec
 00000440: 6973 650a 0a0a 636c 6173 7320 6173 6365  ise...class asce
 00000450: 6e64 6578 2845 7863 6861 6e67 652c 2049  ndex(Exchange, I
```

### Comparing `ccxt-4.2.94/ccxt/async_support/base/exchange.py` & `ccxt-4.2.95/ccxt/async_support/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.2.94'
+__version__ = '4.2.95'
 
 # -----------------------------------------------------------------------------
 
 import asyncio
 import concurrent.futures
 import socket
 import certifi
```

### Comparing `ccxt-4.2.94/ccxt/async_support/base/throttler.py` & `ccxt-4.2.95/ccxt/async_support/base/throttler.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/base/ws/__init__.py` & `ccxt-4.2.95/ccxt/async_support/base/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/base/ws/aiohttp_client.py` & `ccxt-4.2.95/ccxt/async_support/base/ws/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/base/ws/cache.py` & `ccxt-4.2.95/ccxt/async_support/base/ws/cache.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/base/ws/client.py` & `ccxt-4.2.95/ccxt/async_support/base/ws/client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/base/ws/fast_client.py` & `ccxt-4.2.95/ccxt/async_support/base/ws/fast_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/base/ws/functions.py` & `ccxt-4.2.95/ccxt/async_support/base/ws/functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/base/ws/future.py` & `ccxt-4.2.95/ccxt/async_support/base/ws/future.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/base/ws/order_book.py` & `ccxt-4.2.95/ccxt/async_support/base/ws/order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/base/ws/order_book_side.py` & `ccxt-4.2.95/ccxt/async_support/base/ws/order_book_side.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/bequant.py` & `ccxt-4.2.95/ccxt/async_support/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/bigone.py` & `ccxt-4.2.95/ccxt/async_support/bigone.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bigone import ImplicitAPI
 import asyncio
 from ccxt.base.types import Balances, Bool, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bigone(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/binance.py` & `ccxt-4.2.95/ccxt/async_support/binance.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,72 +40,72 @@
 00000270: 2c20 5472 616e 7361 6374 696f 6e2c 2054  , Transaction, T
 00000280: 7261 6e73 6665 7245 6e74 7279 0a66 726f  ransferEntry.fro
 00000290: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
 000002a0: 4c69 7374 0a66 726f 6d20 6363 7874 2e62  List.from ccxt.b
 000002b0: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
 000002c0: 7420 4578 6368 616e 6765 4572 726f 720a  t ExchangeError.
 000002d0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-000002e0: 7272 6f72 7320 696d 706f 7274 2050 6572  rrors import Per
-000002f0: 6d69 7373 696f 6e44 656e 6965 640a 6672  missionDenied.fr
-00000300: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-00000310: 6f72 7320 696d 706f 7274 2041 6363 6f75  ors import Accou
-00000320: 6e74 5375 7370 656e 6465 640a 6672 6f6d  ntSuspended.from
-00000330: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-00000340: 7320 696d 706f 7274 2041 7267 756d 656e  s import Argumen
-00000350: 7473 5265 7175 6972 6564 0a66 726f 6d20  tsRequired.from 
-00000360: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-00000370: 2069 6d70 6f72 7420 4261 6452 6571 7565   import BadReque
-00000380: 7374 0a66 726f 6d20 6363 7874 2e62 6173  st.from ccxt.bas
-00000390: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
-000003a0: 4261 6453 796d 626f 6c0a 6672 6f6d 2063  BadSymbol.from c
-000003b0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-000003c0: 696d 706f 7274 204d 6172 6769 6e4d 6f64  import MarginMod
-000003d0: 6541 6c72 6561 6479 5365 740a 6672 6f6d  eAlreadySet.from
-000003e0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-000003f0: 7320 696d 706f 7274 2042 6164 5265 7370  s import BadResp
-00000400: 6f6e 7365 0a66 726f 6d20 6363 7874 2e62  onse.from ccxt.b
-00000410: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
-00000420: 7420 496e 7375 6666 6963 6965 6e74 4675  t InsufficientFu
-00000430: 6e64 730a 6672 6f6d 2063 6378 742e 6261  nds.from ccxt.ba
-00000440: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000450: 2049 6e76 616c 6964 4f72 6465 720a 6672   InvalidOrder.fr
-00000460: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-00000470: 6f72 7320 696d 706f 7274 204f 7264 6572  ors import Order
-00000480: 4e6f 7446 6f75 6e64 0a66 726f 6d20 6363  NotFound.from cc
-00000490: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
-000004a0: 6d70 6f72 7420 4f72 6465 7249 6d6d 6564  mport OrderImmed
-000004b0: 6961 7465 6c79 4669 6c6c 6162 6c65 0a66  iatelyFillable.f
-000004c0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-000004d0: 726f 7273 2069 6d70 6f72 7420 4f72 6465  rors import Orde
-000004e0: 724e 6f74 4669 6c6c 6162 6c65 0a66 726f  rNotFillable.fro
-000004f0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-00000500: 7273 2069 6d70 6f72 7420 4e6f 7453 7570  rs import NotSup
-00000510: 706f 7274 6564 0a66 726f 6d20 6363 7874  ported.from ccxt
-00000520: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000530: 6f72 7420 4444 6f53 5072 6f74 6563 7469  ort DDoSProtecti
-00000540: 6f6e 0a66 726f 6d20 6363 7874 2e62 6173  on.from ccxt.bas
-00000550: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
-00000560: 5261 7465 4c69 6d69 7445 7863 6565 6465  RateLimitExceede
-00000570: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
-00000580: 2e65 7272 6f72 7320 696d 706f 7274 204f  .errors import O
-00000590: 6e4d 6169 6e74 656e 616e 6365 0a66 726f  nMaintenance.fro
-000005a0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-000005b0: 7273 2069 6d70 6f72 7420 496e 7661 6c69  rs import Invali
-000005c0: 644e 6f6e 6365 0a66 726f 6d20 6363 7874  dNonce.from ccxt
-000005d0: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-000005e0: 6f72 7420 5265 7175 6573 7454 696d 656f  ort RequestTimeo
-000005f0: 7574 0a66 726f 6d20 6363 7874 2e62 6173  ut.from ccxt.bas
-00000600: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
-00000610: 4175 7468 656e 7469 6361 7469 6f6e 4572  AuthenticationEr
-00000620: 726f 720a 6672 6f6d 2063 6378 742e 6261  ror.from ccxt.ba
-00000630: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000640: 204f 7065 7261 7469 6f6e 5265 6a65 6374   OperationReject
-00000650: 6564 0a66 726f 6d20 6363 7874 2e62 6173  ed.from ccxt.bas
-00000660: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
-00000670: 4f70 6572 6174 696f 6e46 6169 6c65 640a  OperationFailed.
+000002e0: 7272 6f72 7320 696d 706f 7274 2041 7574  rrors import Aut
+000002f0: 6865 6e74 6963 6174 696f 6e45 7272 6f72  henticationError
+00000300: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
+00000310: 6572 726f 7273 2069 6d70 6f72 7420 5065  errors import Pe
+00000320: 726d 6973 7369 6f6e 4465 6e69 6564 0a66  rmissionDenied.f
+00000330: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+00000340: 726f 7273 2069 6d70 6f72 7420 4163 636f  rors import Acco
+00000350: 756e 7453 7573 7065 6e64 6564 0a66 726f  untSuspended.fro
+00000360: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+00000370: 7273 2069 6d70 6f72 7420 4172 6775 6d65  rs import Argume
+00000380: 6e74 7352 6571 7569 7265 640a 6672 6f6d  ntsRequired.from
+00000390: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+000003a0: 7320 696d 706f 7274 2042 6164 5265 7175  s import BadRequ
+000003b0: 6573 740a 6672 6f6d 2063 6378 742e 6261  est.from ccxt.ba
+000003c0: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
+000003d0: 2042 6164 5379 6d62 6f6c 0a66 726f 6d20   BadSymbol.from 
+000003e0: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
+000003f0: 2069 6d70 6f72 7420 4f70 6572 6174 696f   import Operatio
+00000400: 6e52 656a 6563 7465 640a 6672 6f6d 2063  nRejected.from c
+00000410: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+00000420: 696d 706f 7274 204d 6172 6769 6e4d 6f64  import MarginMod
+00000430: 6541 6c72 6561 6479 5365 740a 6672 6f6d  eAlreadySet.from
+00000440: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+00000450: 7320 696d 706f 7274 2042 6164 5265 7370  s import BadResp
+00000460: 6f6e 7365 0a66 726f 6d20 6363 7874 2e62  onse.from ccxt.b
+00000470: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+00000480: 7420 496e 7375 6666 6963 6965 6e74 4675  t InsufficientFu
+00000490: 6e64 730a 6672 6f6d 2063 6378 742e 6261  nds.from ccxt.ba
+000004a0: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
+000004b0: 2049 6e76 616c 6964 4f72 6465 720a 6672   InvalidOrder.fr
+000004c0: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+000004d0: 6f72 7320 696d 706f 7274 204f 7264 6572  ors import Order
+000004e0: 4e6f 7446 6f75 6e64 0a66 726f 6d20 6363  NotFound.from cc
+000004f0: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
+00000500: 6d70 6f72 7420 4f72 6465 7249 6d6d 6564  mport OrderImmed
+00000510: 6961 7465 6c79 4669 6c6c 6162 6c65 0a66  iatelyFillable.f
+00000520: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+00000530: 726f 7273 2069 6d70 6f72 7420 4f72 6465  rors import Orde
+00000540: 724e 6f74 4669 6c6c 6162 6c65 0a66 726f  rNotFillable.fro
+00000550: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+00000560: 7273 2069 6d70 6f72 7420 4e6f 7453 7570  rs import NotSup
+00000570: 706f 7274 6564 0a66 726f 6d20 6363 7874  ported.from ccxt
+00000580: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+00000590: 6f72 7420 4f70 6572 6174 696f 6e46 6169  ort OperationFai
+000005a0: 6c65 640a 6672 6f6d 2063 6378 742e 6261  led.from ccxt.ba
+000005b0: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
+000005c0: 2044 446f 5350 726f 7465 6374 696f 6e0a   DDoSProtection.
+000005d0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+000005e0: 7272 6f72 7320 696d 706f 7274 2052 6174  rrors import Rat
+000005f0: 654c 696d 6974 4578 6365 6564 6564 0a66  eLimitExceeded.f
+00000600: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+00000610: 726f 7273 2069 6d70 6f72 7420 4f6e 4d61  rors import OnMa
+00000620: 696e 7465 6e61 6e63 650a 6672 6f6d 2063  intenance.from c
+00000630: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+00000640: 696d 706f 7274 2049 6e76 616c 6964 4e6f  import InvalidNo
+00000650: 6e63 650a 6672 6f6d 2063 6378 742e 6261  nce.from ccxt.ba
+00000660: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
+00000670: 2052 6571 7565 7374 5469 6d65 6f75 740a   RequestTimeout.
 00000680: 6672 6f6d 2063 6378 742e 6261 7365 2e64  from ccxt.base.d
 00000690: 6563 696d 616c 5f74 6f5f 7072 6563 6973  ecimal_to_precis
 000006a0: 696f 6e20 696d 706f 7274 2054 5255 4e43  ion import TRUNC
 000006b0: 4154 450a 6672 6f6d 2063 6378 742e 6261  ATE.from ccxt.ba
 000006c0: 7365 2e64 6563 696d 616c 5f74 6f5f 7072  se.decimal_to_pr
 000006d0: 6563 6973 696f 6e20 696d 706f 7274 2044  ecision import D
 000006e0: 4543 494d 414c 5f50 4c41 4345 530a 6672  ECIMAL_PLACES.fr
```

### Comparing `ccxt-4.2.94/ccxt/async_support/binancecoinm.py` & `ccxt-4.2.95/ccxt/async_support/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/binanceus.py` & `ccxt-4.2.95/ccxt/async_support/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/binanceusdm.py` & `ccxt-4.2.95/ccxt/async_support/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/bingx.py` & `ccxt-4.2.95/ccxt/async_support/bingx.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from ccxt.abstract.bingx import ImplicitAPI
 import asyncio
 import hashlib
 import numbers
 from ccxt.base.types import Balances, Currencies, Currency, Int, Leverage, MarginMode, MarginModification, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Position, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.precise import Precise
 
 
 class bingx(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bit2c.py` & `ccxt-4.2.95/ccxt/async_support/bit2c.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bit2c import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Ticker, Trade, TradingFees
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bit2c(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bitbank.py` & `ccxt-4.2.95/ccxt/async_support/bitbank.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bitbank import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Ticker, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class bitbank(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(bitbank, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bitbns.py` & `ccxt-4.2.95/ccxt/async_support/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/bitcoincom.py` & `ccxt-4.2.95/ccxt/async_support/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/bitfinex.py` & `ccxt-4.2.95/ccxt/async_support/bitfinex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bitfinex import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import ROUND
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.decimal_to_precision import SIGNIFICANT_DIGITS
 from ccxt.base.precise import Precise
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bitfinex2.py` & `ccxt-4.2.95/ccxt/async_support/bitfinex2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bitfinex2 import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, MarginModification, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import ROUND
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.decimal_to_precision import SIGNIFICANT_DIGITS
 from ccxt.base.precise import Precise
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bitflyer.py` & `ccxt-4.2.95/ccxt/async_support/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/bitget.py` & `ccxt-4.2.95/ccxt/async_support/bitget.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ccxt.abstract.bitget import ImplicitAPI
 import asyncio
 import hashlib
 import json
 from ccxt.base.types import Balances, Conversion, Currencies, Currency, FundingHistory, Int, Liquidation, Leverage, MarginMode, MarginModification, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Position, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
@@ -24,15 +25,14 @@
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitget(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bithumb.py` & `ccxt-4.2.95/ccxt/async_support/bithumb.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bithumb import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, MarketInterface, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.decimal_to_precision import SIGNIFICANT_DIGITS
 from ccxt.base.precise import Precise
 
 
 class bithumb(Exchange, ImplicitAPI):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bitmart.py` & `ccxt-4.2.95/ccxt/async_support/bitmart.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bitmart import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
@@ -20,15 +21,14 @@
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitmart(Exchange, ImplicitAPI):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bitmex.py` & `ccxt-4.2.95/ccxt/async_support/bitmex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bitmex import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Leverage, Leverages, Market, MarketType, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitmex(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bitopro.py` & `ccxt-4.2.95/ccxt/async_support/bitopro.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bitopro import ImplicitAPI
 import hashlib
 import math
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitopro(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bitrue.py` & `ccxt-4.2.95/ccxt/async_support/bitrue.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ccxt.abstract.bitrue import ImplicitAPI
 import asyncio
 import hashlib
 import json
 from ccxt.base.types import Balances, Currencies, Currency, Int, MarginModification, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
@@ -22,15 +23,14 @@
 from ccxt.base.errors import OrderImmediatelyFillable
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitrue(Exchange, ImplicitAPI):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bitso.py` & `ccxt-4.2.95/ccxt/async_support/bitso.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bitso import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitso(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bitstamp.py` & `ccxt-4.2.95/ccxt/async_support/bitstamp.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bitstamp import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitstamp(Exchange, ImplicitAPI):
 
     def describe(self):
@@ -366,14 +366,20 @@
                         'lmwr_address/': 1,
                         'pepe_withdrawal/': 1,
                         'pepe_address/': 1,
                         'blur_withdrawal/': 1,
                         'blur_address/': 1,
                         'vext_withdrawal/': 1,
                         'vext_address/': 1,
+                        'cspr_withdrawal/': 1,
+                        'cspr_address/': 1,
+                        'vchf_withdrawal/': 1,
+                        'vchf_address/': 1,
+                        'veur_withdrawal/': 1,
+                        'veur_address/': 1,
                     },
                 },
             },
             'fees': {
                 'trading': {
                     'tierBased': True,
                     'percentage': True,
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bitteam.py` & `ccxt-4.2.95/ccxt/async_support/bitteam.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bitteam import ImplicitAPI
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.precise import Precise
 
 
 class bitteam(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bitvavo.py` & `ccxt-4.2.95/ccxt/async_support/bitvavo.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bitvavo import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import ROUND
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.decimal_to_precision import SIGNIFICANT_DIGITS
 from ccxt.base.precise import Precise
```

### Comparing `ccxt-4.2.94/ccxt/async_support/bl3p.py` & `ccxt-4.2.95/ccxt/async_support/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/blockchaincom.py` & `ccxt-4.2.95/ccxt/async_support/blockchaincom.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.blockchaincom import ImplicitAPI
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import OrderNotFound
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class blockchaincom(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/blofin.py` & `ccxt-4.2.95/ccxt/async_support/blofin.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.blofin import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Leverage, Leverages, MarginMode, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Position, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class blofin(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/btcalpha.py` & `ccxt-4.2.95/ccxt/async_support/btcalpha.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.btcalpha import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, IndexType, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import DDoSProtection
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class btcalpha(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/btcbox.py` & `ccxt-4.2.95/ccxt/async_support/btcbox.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.btcbox import ImplicitAPI
 import hashlib
 import json
 from ccxt.base.types import Balances, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Ticker, Trade
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class btcbox(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/btcmarkets.py` & `ccxt-4.2.95/ccxt/async_support/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/btcturk.py` & `ccxt-4.2.95/ccxt/async_support/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/bybit.py` & `ccxt-4.2.95/ccxt/async_support/bybit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.bybit import ImplicitAPI
 import asyncio
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Greeks, Int, Leverage, Market, MarketInterface, Num, Option, OptionChain, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
+from ccxt.base.errors import NoChange
 from ccxt.base.errors import MarginModeAlreadySet
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import InvalidNonce
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
-from ccxt.base.errors import NoChange
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bybit(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/cex.py` & `ccxt-4.2.95/ccxt/async_support/cex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.cex import ImplicitAPI
 import hashlib
 import json
 from ccxt.base.types import Balances, Currencies, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import NullResponse
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class cex(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/coinbase.py` & `ccxt-4.2.95/ccxt/async_support/coinbase.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.coinbase import ImplicitAPI
 import asyncio
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinbase(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/coinbaseinternational.py` & `ccxt-4.2.95/ccxt/async_support/coinbaseinternational.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.coinbaseinternational import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Order, OrderSide, OrderType, Position, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
 from typing import Any
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import DuplicateOrderId
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinbaseinternational(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/coinbasepro.py` & `ccxt-4.2.95/ccxt/async_support/coinbasepro.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.coinbasepro import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinbasepro(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/coincheck.py` & `ccxt-4.2.95/ccxt/async_support/coincheck.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.coincheck import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Ticker, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
-from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import BadSymbol
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class coincheck(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(coincheck, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/async_support/coinex.py` & `ccxt-4.2.95/ccxt/async_support/coinex.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.coinex import ImplicitAPI
 import asyncio
 from ccxt.base.types import Balances, Currencies, Currency, Int, Leverage, Leverages, MarginModification, Market, Num, Order, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinex(Exchange, ImplicitAPI):
 
     def describe(self):
@@ -1072,83 +1072,89 @@
         #
         data = self.safe_dict(response, 'data', {})
         return self.safe_integer(data, 'timestamp')
 
     async def fetch_order_book(self, symbol: str, limit: Int = 20, params={}):
         """
         fetches information on open orders with bid(buy) and ask(sell) prices, volumes and other data
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot001_market004_market_depth
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http010_market_depth
+        :see: https://docs.coinex.com/api/v2/spot/market/http/list-market-depth
+        :see: https://docs.coinex.com/api/v2/futures/market/http/list-market-depth
         :param str symbol: unified symbol of the market to fetch the order book for
         :param int [limit]: the maximum amount of order book entries to return
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: A dictionary of `order book structures <https://docs.ccxt.com/#/?id=order-book-structure>` indexed by market symbols
         """
         await self.load_markets()
         market = self.market(symbol)
         if limit is None:
             limit = 20  # default
         request = {
-            'market': self.market_id(symbol),
-            'merge': '0',
-            'limit': str(limit),
+            'market': market['id'],
+            'limit': limit,
+            'interval': '0',
         }
         response = None
         if market['swap']:
-            response = await self.v1PerpetualPublicGetMarketDepth(self.extend(request, params))
+            response = await self.v2PublicGetFuturesDepth(self.extend(request, params))
+            #
+            #     {
+            #         "code": 0,
+            #         "data": {
+            #             "depth": {
+            #                 "asks": [
+            #                     ["70851.94", "0.2119"],
+            #                     ["70851.95", "0.0004"],
+            #                     ["70851.96", "0.0004"]
+            #                 ],
+            #                 "bids": [
+            #                     ["70851.93", "1.0314"],
+            #                     ["70850.93", "0.0021"],
+            #                     ["70850.42", "0.0306"]
+            #                 ],
+            #                 "checksum": 2956436260,
+            #                 "last": "70851.94",
+            #                 "updated_at": 1712824003252
+            #             },
+            #             "is_full": True,
+            #             "market": "BTCUSDT"
+            #         },
+            #         "message": "OK"
+            #     }
+            #
         else:
-            response = await self.v1PublicGetMarketDepth(self.extend(request, params))
-        #
-        # Spot
-        #
-        #     {
-        #         "code": 0,
-        #         "data": {
-        #             "asks": [
-        #                 ["41056.33", "0.31727613"],
-        #                 ["41056.34", "1.05657294"],
-        #                 ["41056.35", "0.02346648"]
-        #             ],
-        #             "bids": [
-        #                 ["41050.61", "0.40618608"],
-        #                 ["41046.98", "0.13800000"],
-        #                 ["41046.56", "0.22579234"]
-        #             ],
-        #             "last": "41050.61",
-        #             "time": 1650573220346
-        #         },
-        #         "message": "OK"
-        #     }
-        #
-        # Swap
-        #
-        #     {
-        #         "code": 0,
-        #         "data": {
-        #             "asks": [
-        #                 ["40620.90", "0.0384"],
-        #                 ["40625.50", "0.0219"],
-        #                 ["40625.90", "0.3506"]
-        #             ],
-        #             "bids": [
-        #                 ["40620.89", "19.6861"],
-        #                 ["40620.80", "0.0012"],
-        #                 ["40619.87", "0.0365"]
-        #             ],
-        #             "last": "40620.89",
-        #             "time": 1650587672406,
-        #             "sign_price": "40619.32",
-        #             "index_price": "40609.93"
-        #         },
-        #         "message": "OK"
-        #     }
-        #
-        result = self.safe_value(response, 'data', {})
-        timestamp = self.safe_integer(result, 'time')
-        return self.parse_order_book(result, symbol, timestamp)
+            response = await self.v2PublicGetSpotDepth(self.extend(request, params))
+            #
+            #     {
+            #         "code": 0,
+            #         "data": {
+            #             "depth": {
+            #                 "asks": [
+            #                     ["70875.31", "0.28670282"],
+            #                     ["70875.32", "0.31008114"],
+            #                     ["70875.42", "0.05876653"]
+            #                 ],
+            #                 "bids": [
+            #                     ["70855.3", "0.00632222"],
+            #                     ["70855.29", "0.36216834"],
+            #                     ["70855.17", "0.10166802"]
+            #                 ],
+            #                 "checksum": 2313816665,
+            #                 "last": "70857.19",
+            #                 "updated_at": 1712823790987
+            #             },
+            #             "is_full": True,
+            #             "market": "BTCUSDT"
+            #         },
+            #         "message": "OK"
+            #     }
+            #
+        data = self.safe_dict(response, 'data', {})
+        depth = self.safe_dict(data, 'depth', {})
+        timestamp = self.safe_integer(depth, 'updated_at')
+        return self.parse_order_book(depth, symbol, timestamp)
 
     def parse_trade(self, trade, market: Market = None) -> Trade:
         #
         # Spot and Swap fetchTrades(public)
         #
         #      {
         #          "id":  2611511379,
```

### Comparing `ccxt-4.2.94/ccxt/async_support/coinlist.py` & `ccxt-4.2.95/ccxt/async_support/coinlist.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.coinlist import ImplicitAPI
 import hashlib
 import math
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinlist(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/coinmate.py` & `ccxt-4.2.95/ccxt/async_support/coinmate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.coinmate import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import RateLimitExceeded
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinmate(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/coinmetro.py` & `ccxt-4.2.95/ccxt/async_support/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/coinone.py` & `ccxt-4.2.95/ccxt/async_support/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/coinsph.py` & `ccxt-4.2.95/ccxt/async_support/coinsph.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.coinsph import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import BadResponse
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import OrderImmediatelyFillable
 from ccxt.base.errors import DuplicateOrderId
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinsph(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/coinspot.py` & `ccxt-4.2.95/ccxt/async_support/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/cryptocom.py` & `ccxt-4.2.95/ccxt/async_support/cryptocom.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.cryptocom import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currency, Int, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountNotEnabled
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class cryptocom(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/currencycom.py` & `ccxt-4.2.95/ccxt/async_support/currencycom.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.currencycom import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Leverage, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class currencycom(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/delta.py` & `ccxt-4.2.95/ccxt/async_support/delta.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.delta import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Greeks, Int, Leverage, MarginMode, MarginModification, Market, MarketInterface, Num, Option, Order, OrderBook, OrderSide, OrderType, Position, Str, Strings, Ticker, Tickers, Trade
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class delta(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/deribit.py` & `ccxt-4.2.95/ccxt/async_support/deribit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.deribit import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, Greeks, Int, Market, MarketInterface, Num, Option, OptionChain, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class deribit(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/digifinex.py` & `ccxt-4.2.95/ccxt/async_support/digifinex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ccxt.abstract.digifinex import ImplicitAPI
 import asyncio
 import hashlib
 import json
 from ccxt.base.types import Balances, Currencies, Currency, Int, MarginModification, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import BadResponse
 from ccxt.base.errors import InsufficientFunds
@@ -22,15 +23,14 @@
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class digifinex(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/exmo.py` & `ccxt-4.2.95/ccxt/async_support/exmo.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.exmo import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, MarginModification, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class exmo(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/flowbtc.py` & `ccxt-4.2.95/ccxt/async_support/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/fmfwio.py` & `ccxt-4.2.95/ccxt/async_support/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/gate.py` & `ccxt-4.2.95/ccxt/async_support/gate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.gate import ImplicitAPI
 import asyncio
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, FundingHistory, Greeks, Int, Leverage, Leverages, MarginModification, Market, MarketInterface, Num, Option, OptionChain, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountNotEnabled
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import BadResponse
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import OrderImmediatelyFillable
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class gate(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/gemini.py` & `ccxt-4.2.95/ccxt/async_support/gemini.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.gemini import ImplicitAPI
 import asyncio
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class gemini(Exchange, ImplicitAPI):
 
     def describe(self):
@@ -662,15 +662,16 @@
             marketIdUpper = marketId.upper()
             isPerp = (marketIdUpper.find('PERP') >= 0)
             marketIdWithoutPerp = marketIdUpper.replace('PERP', '')
             quoteQurrencies = self.handle_option('fetchMarketsFromAPI', 'quoteCurrencies', [])
             for i in range(0, len(quoteQurrencies)):
                 quoteCurrency = quoteQurrencies[i]
                 if marketIdWithoutPerp.endswith(quoteCurrency):
-                    baseId = marketIdWithoutPerp.replace(quoteCurrency, '')
+                    quoteLength = self.parse_to_int(-1 * len(quoteCurrency))
+                    baseId = marketIdWithoutPerp[0:quoteLength]
                     quoteId = quoteCurrency
                     if isPerp:
                         settleId = quoteCurrency  # always same
                     break
         base = self.safe_currency_code(baseId)
         quote = self.safe_currency_code(quoteId)
         settle = self.safe_currency_code(settleId)
```

### Comparing `ccxt-4.2.94/ccxt/async_support/hitbtc.py` & `ccxt-4.2.95/ccxt/async_support/hitbtc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.hitbtc import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Leverage, MarginMode, MarginModes, MarginModification, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class hitbtc(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/hollaex.py` & `ccxt-4.2.95/ccxt/async_support/hollaex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.hollaex import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import OrderImmediatelyFillable
 from ccxt.base.errors import NetworkError
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class hollaex(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/htx.py` & `ccxt-4.2.95/ccxt/async_support/htx.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.htx import ImplicitAPI
 import asyncio
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountNotEnabled
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
-from ccxt.base.errors import NetworkError
+from ccxt.base.errors import OperationFailed
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class htx(Exchange, ImplicitAPI):
 
@@ -955,22 +955,16 @@
                 },
             },
             'precisionMode': TICK_SIZE,
             'options': {
                 'fetchMarkets': {
                     'types': {
                         'spot': True,
-                        'future': {
-                            'linear': True,
-                            'inverse': True,
-                        },
-                        'swap': {
-                            'linear': True,
-                            'inverse': True,
-                        },
+                        'linear': True,
+                        'inverse': True,
                     },
                 },
                 'fetchOHLCV': {
                     'useHistoricalEndpointForSpot': True,
                 },
                 'withdraw': {
                     'includeFee': False,
@@ -1606,60 +1600,49 @@
 
     async def fetch_markets(self, params={}) -> List[Market]:
         """
         retrieves data on all markets for huobi
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: an array of objects representing market data
         """
-        options = self.safe_value(self.options, 'fetchMarkets', {})
-        types = self.safe_value(options, 'types', {})
+        types = None
+        types, params = self.handle_option_and_params(params, 'fetchMarkets', 'types', {})
         allMarkets = []
         promises = []
         keys = list(types.keys())
         for i in range(0, len(keys)):
-            type = keys[i]
-            value = self.safe_value(types, type)
-            if value is True:
-                promises.append(self.fetch_markets_by_type_and_sub_type(type, None, params))
-            elif value:
-                subKeys = list(value.keys())
-                for j in range(0, len(subKeys)):
-                    subType = subKeys[j]
-                    subValue = self.safe_value(value, subType)
-                    if subValue:
-                        promises.append(self.fetch_markets_by_type_and_sub_type(type, subType, params))
+            key = keys[i]
+            if self.safe_bool(types, key):
+                if key == 'spot':
+                    promises.append(self.fetch_markets_by_type_and_sub_type('spot', None, params))
+                elif key == 'linear':
+                    promises.append(self.fetch_markets_by_type_and_sub_type(None, 'linear', params))
+                elif key == 'inverse':
+                    promises.append(self.fetch_markets_by_type_and_sub_type('swap', 'inverse', params))
+                    promises.append(self.fetch_markets_by_type_and_sub_type('future', 'inverse', params))
         promises = await asyncio.gather(*promises)
         for i in range(0, len(promises)):
             allMarkets = self.array_concat(allMarkets, promises[i])
         return allMarkets
 
     async def fetch_markets_by_type_and_sub_type(self, type, subType, params={}):
-        query = self.omit(params, ['type', 'subType'])
-        spot = (type == 'spot')
-        contract = (type != 'spot')
-        future = (type == 'future')
-        swap = (type == 'swap')
-        linear = None
-        inverse = None
+        isSpot = (type == 'spot')
         request = {}
         response = None
-        if contract:
-            linear = (subType == 'linear')
-            inverse = (subType == 'inverse')
-            if linear:
-                if future:
-                    request['business_type'] = 'futures'
-                response = await self.contractPublicGetLinearSwapApiV1SwapContractInfo(self.extend(request, query))
-            elif inverse:
-                if future:
-                    response = await self.contractPublicGetApiV1ContractContractInfo(self.extend(request, query))
-                elif swap:
-                    response = await self.contractPublicGetSwapApiV1SwapContractInfo(self.extend(request, query))
+        if not isSpot:
+            if subType == 'linear':
+                request['business_type'] = 'all'  # override default to fetch all linear markets
+                response = await self.contractPublicGetLinearSwapApiV1SwapContractInfo(self.extend(request, params))
+            elif subType == 'inverse':
+                if type == 'future':
+                    response = await self.contractPublicGetApiV1ContractContractInfo(self.extend(request, params))
+                elif type == 'swap':
+                    response = await self.contractPublicGetSwapApiV1SwapContractInfo(self.extend(request, params))
         else:
-            response = await self.spotPublicGetV1CommonSymbols(self.extend(request, query))
+            response = await self.spotPublicGetV1CommonSymbols(self.extend(request, params))
         #
         # spot
         #
         #     {
         #         "status":"ok",
         #         "data":[
         #             {
@@ -1690,110 +1673,109 @@
         #                 "init-nav":10.000000000000000000,
         #                 "api-trading":"enabled",
         #                 "tags":"etp,nav,holdinglimit"
         #             },
         #         ]
         #     }
         #
-        # inverse future
+        # inverse(swap & future)
         #
         #     {
         #         "status":"ok",
         #         "data":[
         #             {
         #                 "symbol":"BTC",
-        #                 "contract_code":"BTC211126",
-        #                 "contract_type":"self_week",
-        #                 "contract_size":100.000000000000000000,
-        #                 "price_tick":0.010000000000000000,
-        #                 "delivery_date":"20211126",
-        #                 "delivery_time":"1637913600000",
+        #                 "contract_code":"BTC211126",  #/ BTC-USD in swap
+        #                 "contract_type":"self_week",  # only in future
+        #                 "contract_size":100,
+        #                 "price_tick":0.1,
+        #                 "delivery_date":"20211126",  # only in future
+        #                 "delivery_time":"1637913600000",  # empty in swap
         #                 "create_date":"20211112",
         #                 "contract_status":1,
-        #                 "settlement_time":"1637481600000"
+        #                 "settlement_time":"1637481600000"  # only in future
+        #                 "settlement_date":"16xxxxxxxxxxx"  # only in swap
         #             },
+        #           ...
         #         ],
         #         "ts":1637474595140
         #     }
         #
-        # linear futures
+        # linear(swap & future)
         #
         #     {
         #         "status":"ok",
         #         "data":[
         #             {
         #                 "symbol":"BTC",
-        #                 "contract_code":"BTC-USDT-211231",
-        #                 "contract_size":0.001000000000000000,
-        #                 "price_tick":0.100000000000000000,
-        #                 "delivery_date":"20211231",
-        #                 "delivery_time":"1640937600000",
+        #                 "contract_code":"BTC-USDT-211231",  # or "BTC-USDT" in swap
+        #                 "contract_size":0.001,
+        #                 "price_tick":0.1,
+        #                 "delivery_date":"20211231",  # empty in swap
+        #                 "delivery_time":"1640937600000",  # empty in swap
         #                 "create_date":"20211228",
         #                 "contract_status":1,
         #                 "settlement_date":"1640764800000",
-        #                 "support_margin_mode":"cross",
-        #                 "business_type":"futures",
+        #                 "support_margin_mode":"cross",  # "all" or "cross"
+        #                 "business_type":"futures",  # "swap" or "futures"
         #                 "pair":"BTC-USDT",
-        #                 "contract_type":"self_week"  # next_week, quarter
-        #             },
+        #                 "contract_type":"self_week",  # "swap", "self_week", "next_week", "quarter"
+        #                 "trade_partition":"USDT",
+        #             }
         #         ],
         #         "ts":1640736207263
         #     }
         #
-        # swaps
-        #
-        #     {
-        #         "status":"ok",
-        #         "data":[
-        #             {
-        #                 "symbol":"BTC",
-        #                 "contract_code":"BTC-USDT",
-        #                 "contract_size":0.001000000000000000,
-        #                 "price_tick":0.100000000000000000,
-        #                 "delivery_time":"",
-        #                 "create_date":"20201021",
-        #                 "contract_status":1,
-        #                 "settlement_date":"1637481600000",
-        #                 "support_margin_mode":"all",  # isolated
-        #             },
-        #         ],
-        #         "ts":1637474774467
-        #     }
-        #
-        markets = self.safe_value(response, 'data', [])
+        markets = self.safe_list(response, 'data', [])
         numMarkets = len(markets)
         if numMarkets < 1:
-            raise NetworkError(self.id + ' fetchMarkets() returned an empty response: ' + self.json(markets))
+            raise OperationFailed(self.id + ' fetchMarkets() returned an empty response: ' + self.json(response))
         result = []
         for i in range(0, len(markets)):
             market = markets[i]
             baseId = None
             quoteId = None
             settleId = None
             id = None
             lowercaseId = None
+            contract = ('contract_code' in market)
+            spot = not contract
+            swap = False
+            future = False
+            linear = None
+            inverse = None
+            # check if parsed market is contract
             if contract:
                 id = self.safe_string(market, 'contract_code')
                 lowercaseId = id.lower()
+                delivery_date = self.safe_string(market, 'delivery_date')
+                business_type = self.safe_string(market, 'business_type')
+                future = delivery_date is not None
+                swap = not future
+                linear = business_type is not None
+                inverse = not linear
                 if swap:
+                    type = 'swap'
                     parts = id.split('-')
                     baseId = self.safe_string_lower(market, 'symbol')
                     quoteId = self.safe_string_lower(parts, 1)
                     settleId = baseId if inverse else quoteId
                 elif future:
+                    type = 'future'
                     baseId = self.safe_string_lower(market, 'symbol')
                     if inverse:
                         quoteId = 'USD'
                         settleId = baseId
                     else:
                         pair = self.safe_string(market, 'pair')
                         parts = pair.split('-')
                         quoteId = self.safe_string_lower(parts, 1)
                         settleId = quoteId
             else:
+                type = 'spot'
                 baseId = self.safe_string(market, 'base-currency')
                 quoteId = self.safe_string(market, 'quote-currency')
                 id = baseId + quoteId
                 lowercaseId = id.lower()
             base = self.safe_currency_code(baseId)
             quote = self.safe_currency_code(quoteId)
             settle = self.safe_currency_code(settleId)
@@ -1908,14 +1890,48 @@
                     },
                 },
                 'created': created,
                 'info': market,
             })
         return result
 
+    def try_get_symbol_from_future_markets(self, symbolOrMarketId: str):
+        if symbolOrMarketId in self.markets:
+            return symbolOrMarketId
+        # only on "future" market type(inverse & linear), market-id differs between "fetchMarkets" and "fetchTicker"
+        # so we have to create a mapping
+        # - market-id from fetchMarkts:    `BTC-USDT-240419`(linear future) or `BTC240412`(inverse future)
+        # - market-id from fetchTciker[s]: `BTC-USDT-CW`     (linear future) or `BTC_CW`    (inverse future)
+        if not ('futureMarketIdsForSymbols' in self.options):
+            self.options['futureMarketIdsForSymbols'] = {}
+        futureMarketIdsForSymbols = self.safe_dict(self.options, 'futureMarketIdsForSymbols', {})
+        if symbolOrMarketId in futureMarketIdsForSymbols:
+            return futureMarketIdsForSymbols[symbolOrMarketId]
+        futureMarkets = self.filter_by(self.markets, 'future', True)
+        futuresCharsMaps = {
+            'this_week': 'CW',
+            'next_week': 'NW',
+            'quarter': 'CQ',
+            'next_quarter': 'NQ',
+        }
+        for i in range(0, len(futureMarkets)):
+            market = futureMarkets[i]
+            info = self.safe_value(market, 'info', {})
+            contractType = self.safe_string(info, 'contract_type')
+            contractSuffix = futuresCharsMaps[contractType]
+            # see comment on formats a bit above
+            constructedId = market['base'] + '-' + market['quote'] + '-' + contractSuffix if market['linear'] else market['base'] + '_' + contractSuffix
+            if constructedId == symbolOrMarketId:
+                symbol = market['symbol']
+                self.options['futureMarketIdsForSymbols'][symbolOrMarketId] = symbol
+                return symbol
+        # if not found, just save it to avoid unnecessary future iterations
+        self.options['futureMarketIdsForSymbols'][symbolOrMarketId] = symbolOrMarketId
+        return symbolOrMarketId
+
     def parse_ticker(self, ticker, market: Market = None) -> Ticker:
         #
         # fetchTicker
         #
         #     {
         #         "amount": 26228.672978342216,
         #         "open": 9078.95,
@@ -1956,14 +1972,15 @@
         #         "bidSize": 1.685945,
         #         "quoteTime": 1671941599612,
         #         "symbol": "btcusdt"
         #     }
         #
         marketId = self.safe_string_2(ticker, 'symbol', 'contract_code')
         symbol = self.safe_symbol(marketId, market)
+        symbol = self.try_get_symbol_from_future_markets(symbol)
         timestamp = self.safe_integer_2(ticker, 'ts', 'quoteTime')
         bid = None
         bidVolume = None
         ask = None
         askVolume = None
         if 'bid' in ticker:
             if isinstance(ticker['bid'], list):
@@ -2083,45 +2100,55 @@
     async def fetch_tickers(self, symbols: Strings = None, params={}) -> Tickers:
         """
         fetches price tickers for multiple markets, statistical information calculated over the past 24 hours for each market
         :see: https://huobiapi.github.io/docs/spot/v1/en/#get-latest-tickers-for-all-pairs
         :see: https://huobiapi.github.io/docs/usdt_swap/v1/en/#general-get-a-batch-of-market-data-overview
         :see: https://huobiapi.github.io/docs/dm/v1/en/#get-a-batch-of-market-data-overview
         :see: https://huobiapi.github.io/docs/coin_margined_swap/v1/en/#get-a-batch-of-market-data-overview-v2
-        :param str[]|None symbols: unified symbols of the markets to fetch the ticker for, all market tickers are returned if not assigned
+        :param str[] [symbols]: unified symbols of the markets to fetch the ticker for, all market tickers are returned if not assigned
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a dictionary of `ticker structures <https://docs.ccxt.com/#/?id=ticker-structure>`
         """
         await self.load_markets()
         symbols = self.market_symbols(symbols)
         first = self.safe_string(symbols, 0)
         market = None
         if first is not None:
             market = self.market(first)
+        isSubTypeRequested = ('subType' in params) or ('business_type' in params)
         type = None
         subType = None
         type, params = self.handle_market_type_and_params('fetchTickers', market, params)
         subType, params = self.handle_sub_type_and_params('fetchTickers', market, params)
         request = {}
+        isSpot = (type == 'spot')
         future = (type == 'future')
         swap = (type == 'swap')
         linear = (subType == 'linear')
         inverse = (subType == 'inverse')
-        params = self.omit(params, ['type', 'subType'])
         response = None
-        if future or swap:
+        if not isSpot or isSubTypeRequested:
             if linear:
+                # independently of type, supports calling all linear symbols i.e. fetchTickers(None, {subType:'linear'})
                 if future:
                     request['business_type'] = 'futures'
+                elif swap:
+                    request['business_type'] = 'swap'
+                else:
+                    request['business_type'] = 'all'
                 response = await self.contractPublicGetLinearSwapExMarketDetailBatchMerged(self.extend(request, params))
             elif inverse:
                 if future:
                     response = await self.contractPublicGetMarketDetailBatchMerged(self.extend(request, params))
                 elif swap:
                     response = await self.contractPublicGetSwapExMarketDetailBatchMerged(self.extend(request, params))
+                else:
+                    raise NotSupported(self.id + ' fetchTickers() you have to set params["type"] to either "swap" or "future" for inverse contracts')
+            else:
+                raise NotSupported(self.id + ' fetchTickers() you have to set params["subType"] to either "linear" or "inverse" for contracts')
         else:
             response = await self.spotPublicGetMarketTickers(self.extend(request, params))
         #
         # spot
         #
         #     {
         #         "data":[
@@ -2166,51 +2193,25 @@
         #                 "business_type":"futures",  # only in linear futures
         #                 "contract_code":"BTC-USDT-CW",  # only in linear futures, instead of 'symbol'
         #             }
         #         ],
         #         "ts":1637504679376
         #     }
         #
-        tickers = self.safe_value_2(response, 'data', 'ticks', [])
-        timestamp = self.safe_integer(response, 'ts')
-        result = {}
-        for i in range(0, len(tickers)):
-            ticker = self.parse_ticker(tickers[i])
-            # the market ids for linear futures are non-standard and differ from all the other endpoints
-            # we are doing a linear-matching here
-            if future and linear:
-                for j in range(0, len(self.symbols)):
-                    symbolInner = self.symbols[j]
-                    marketInner = self.market(symbolInner)
-                    contractType = self.safe_string(marketInner['info'], 'contract_type')
-                    if (contractType == 'this_week') and (ticker['symbol'] == (marketInner['baseId'] + '-' + marketInner['quoteId'] + '-CW')):
-                        ticker['symbol'] = marketInner['symbol']
-                        break
-                    elif (contractType == 'next_week') and (ticker['symbol'] == (marketInner['baseId'] + '-' + marketInner['quoteId'] + '-NW')):
-                        ticker['symbol'] = marketInner['symbol']
-                        break
-                    elif (contractType == 'this_quarter') and (ticker['symbol'] == (marketInner['baseId'] + '-' + marketInner['quoteId'] + '-CQ')):
-                        ticker['symbol'] = marketInner['symbol']
-                        break
-                    elif (contractType == 'next_quarter') and (ticker['symbol'] == (marketInner['baseId'] + '-' + marketInner['quoteId'] + '-NQ')):
-                        ticker['symbol'] = marketInner['symbol']
-                        break
-            symbol = ticker['symbol']
-            ticker['timestamp'] = timestamp
-            ticker['datetime'] = self.iso8601(timestamp)
-            result[symbol] = ticker
-        return self.filter_by_array_tickers(result, 'symbol', symbols)
+        rawTickers = self.safe_list_2(response, 'data', 'ticks', [])
+        tickers = self.parse_tickers(rawTickers, symbols, params)
+        return self.filter_by_array_tickers(tickers, 'symbol', symbols)
 
     async def fetch_last_prices(self, symbols: Strings = None, params={}):
         """
         fetches the last price for multiple markets
         :see: https://www.htx.com/en-us/opend/newApiPages/?id=8cb81024-77b5-11ed-9966-0242ac110003 linear swap & linear future
         :see: https://www.htx.com/en-us/opend/newApiPages/?id=28c2e8fc-77ae-11ed-9966-0242ac110003 inverse future
         :see: https://www.htx.com/en-us/opend/newApiPages/?id=5d517ef5-77b6-11ed-9966-0242ac110003 inverse swap
-        :param str[]|None symbols: unified symbols of the markets to fetch the last prices
+        :param str[] [symbols]: unified symbols of the markets to fetch the last prices
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a dictionary of lastprices structures
         """
         await self.load_markets()
         symbols = self.market_symbols(symbols)
         market = self.get_market_from_symbols(symbols)
         type = None
```

### Comparing `ccxt-4.2.94/ccxt/async_support/huobijp.py` & `ccxt-4.2.95/ccxt/async_support/huobijp.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.huobijp import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class huobijp(Exchange, ImplicitAPI):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/hyperliquid.py` & `ccxt-4.2.95/ccxt/async_support/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/idex.py` & `ccxt-4.2.95/ccxt/async_support/idex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.idex import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import ROUND
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.decimal_to_precision import PAD_WITH_ZERO
 from ccxt.base.precise import Precise
```

### Comparing `ccxt-4.2.94/ccxt/async_support/independentreserve.py` & `ccxt-4.2.95/ccxt/async_support/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/indodax.py` & `ccxt-4.2.95/ccxt/async_support/indodax.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.indodax import ImplicitAPI
 import hashlib
 import math
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class indodax(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(indodax, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/async_support/kraken.py` & `ccxt-4.2.95/ccxt/async_support/kraken.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,61 +31,61 @@
 000001e0: 652c 2054 7261 6e73 6163 7469 6f6e 2c20  e, Transaction, 
 000001f0: 5472 616e 7366 6572 456e 7472 790a 6672  TransferEntry.fr
 00000200: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
 00000210: 204c 6973 740a 6672 6f6d 2063 6378 742e   List.from ccxt.
 00000220: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
 00000230: 7274 2045 7863 6861 6e67 6545 7272 6f72  rt ExchangeError
 00000240: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-00000250: 6572 726f 7273 2069 6d70 6f72 7420 5065  errors import Pe
-00000260: 726d 6973 7369 6f6e 4465 6e69 6564 0a66  rmissionDenied.f
-00000270: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-00000280: 726f 7273 2069 6d70 6f72 7420 4163 636f  rors import Acco
-00000290: 756e 7453 7573 7065 6e64 6564 0a66 726f  untSuspended.fro
-000002a0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-000002b0: 7273 2069 6d70 6f72 7420 4172 6775 6d65  rs import Argume
-000002c0: 6e74 7352 6571 7569 7265 640a 6672 6f6d  ntsRequired.from
-000002d0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-000002e0: 7320 696d 706f 7274 2042 6164 5265 7175  s import BadRequ
-000002f0: 6573 740a 6672 6f6d 2063 6378 742e 6261  est.from ccxt.ba
-00000300: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000310: 2042 6164 5379 6d62 6f6c 0a66 726f 6d20   BadSymbol.from 
-00000320: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-00000330: 2069 6d70 6f72 7420 496e 7375 6666 6963   import Insuffic
-00000340: 6965 6e74 4675 6e64 730a 6672 6f6d 2063  ientFunds.from c
-00000350: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-00000360: 696d 706f 7274 2049 6e76 616c 6964 4164  import InvalidAd
-00000370: 6472 6573 730a 6672 6f6d 2063 6378 742e  dress.from ccxt.
-00000380: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-00000390: 7274 2049 6e76 616c 6964 4f72 6465 720a  rt InvalidOrder.
-000003a0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-000003b0: 7272 6f72 7320 696d 706f 7274 204f 7264  rrors import Ord
-000003c0: 6572 4e6f 7446 6f75 6e64 0a66 726f 6d20  erNotFound.from 
-000003d0: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-000003e0: 2069 6d70 6f72 7420 4361 6e63 656c 5065   import CancelPe
-000003f0: 6e64 696e 670a 6672 6f6d 2063 6378 742e  nding.from ccxt.
-00000400: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-00000410: 7274 204e 6f74 5375 7070 6f72 7465 640a  rt NotSupported.
-00000420: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-00000430: 7272 6f72 7320 696d 706f 7274 2044 446f  rrors import DDo
-00000440: 5350 726f 7465 6374 696f 6e0a 6672 6f6d  SProtection.from
-00000450: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-00000460: 7320 696d 706f 7274 2052 6174 654c 696d  s import RateLim
-00000470: 6974 4578 6365 6564 6564 0a66 726f 6d20  itExceeded.from 
-00000480: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-00000490: 2069 6d70 6f72 7420 4578 6368 616e 6765   import Exchange
-000004a0: 4e6f 7441 7661 696c 6162 6c65 0a66 726f  NotAvailable.fro
-000004b0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-000004c0: 7273 2069 6d70 6f72 7420 4f6e 4d61 696e  rs import OnMain
-000004d0: 7465 6e61 6e63 650a 6672 6f6d 2063 6378  tenance.from ccx
-000004e0: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
-000004f0: 706f 7274 2049 6e76 616c 6964 4e6f 6e63  port InvalidNonc
-00000500: 650a 6672 6f6d 2063 6378 742e 6261 7365  e.from ccxt.base
-00000510: 2e65 7272 6f72 7320 696d 706f 7274 2041  .errors import A
-00000520: 7574 6865 6e74 6963 6174 696f 6e45 7272  uthenticationErr
-00000530: 6f72 0a66 726f 6d20 6363 7874 2e62 6173  or.from ccxt.bas
+00000250: 6572 726f 7273 2069 6d70 6f72 7420 4175  errors import Au
+00000260: 7468 656e 7469 6361 7469 6f6e 4572 726f  thenticationErro
+00000270: 720a 6672 6f6d 2063 6378 742e 6261 7365  r.from ccxt.base
+00000280: 2e65 7272 6f72 7320 696d 706f 7274 2050  .errors import P
+00000290: 6572 6d69 7373 696f 6e44 656e 6965 640a  ermissionDenied.
+000002a0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+000002b0: 7272 6f72 7320 696d 706f 7274 2041 6363  rrors import Acc
+000002c0: 6f75 6e74 5375 7370 656e 6465 640a 6672  ountSuspended.fr
+000002d0: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+000002e0: 6f72 7320 696d 706f 7274 2041 7267 756d  ors import Argum
+000002f0: 656e 7473 5265 7175 6972 6564 0a66 726f  entsRequired.fro
+00000300: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+00000310: 7273 2069 6d70 6f72 7420 4261 6452 6571  rs import BadReq
+00000320: 7565 7374 0a66 726f 6d20 6363 7874 2e62  uest.from ccxt.b
+00000330: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+00000340: 7420 4261 6453 796d 626f 6c0a 6672 6f6d  t BadSymbol.from
+00000350: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+00000360: 7320 696d 706f 7274 2049 6e73 7566 6669  s import Insuffi
+00000370: 6369 656e 7446 756e 6473 0a66 726f 6d20  cientFunds.from 
+00000380: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
+00000390: 2069 6d70 6f72 7420 496e 7661 6c69 6441   import InvalidA
+000003a0: 6464 7265 7373 0a66 726f 6d20 6363 7874  ddress.from ccxt
+000003b0: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+000003c0: 6f72 7420 496e 7661 6c69 644f 7264 6572  ort InvalidOrder
+000003d0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
+000003e0: 6572 726f 7273 2069 6d70 6f72 7420 4f72  errors import Or
+000003f0: 6465 724e 6f74 466f 756e 640a 6672 6f6d  derNotFound.from
+00000400: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+00000410: 7320 696d 706f 7274 2043 616e 6365 6c50  s import CancelP
+00000420: 656e 6469 6e67 0a66 726f 6d20 6363 7874  ending.from ccxt
+00000430: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+00000440: 6f72 7420 4e6f 7453 7570 706f 7274 6564  ort NotSupported
+00000450: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
+00000460: 6572 726f 7273 2069 6d70 6f72 7420 4444  errors import DD
+00000470: 6f53 5072 6f74 6563 7469 6f6e 0a66 726f  oSProtection.fro
+00000480: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+00000490: 7273 2069 6d70 6f72 7420 5261 7465 4c69  rs import RateLi
+000004a0: 6d69 7445 7863 6565 6465 640a 6672 6f6d  mitExceeded.from
+000004b0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+000004c0: 7320 696d 706f 7274 2045 7863 6861 6e67  s import Exchang
+000004d0: 654e 6f74 4176 6169 6c61 626c 650a 6672  eNotAvailable.fr
+000004e0: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+000004f0: 6f72 7320 696d 706f 7274 204f 6e4d 6169  ors import OnMai
+00000500: 6e74 656e 616e 6365 0a66 726f 6d20 6363  ntenance.from cc
+00000510: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
+00000520: 6d70 6f72 7420 496e 7661 6c69 644e 6f6e  mport InvalidNon
+00000530: 6365 0a66 726f 6d20 6363 7874 2e62 6173  ce.from ccxt.bas
 00000540: 652e 6465 6369 6d61 6c5f 746f 5f70 7265  e.decimal_to_pre
 00000550: 6369 7369 6f6e 2069 6d70 6f72 7420 5452  cision import TR
 00000560: 554e 4341 5445 0a66 726f 6d20 6363 7874  UNCATE.from ccxt
 00000570: 2e62 6173 652e 6465 6369 6d61 6c5f 746f  .base.decimal_to
 00000580: 5f70 7265 6369 7369 6f6e 2069 6d70 6f72  _precision impor
 00000590: 7420 5449 434b 5f53 495a 450a 6672 6f6d  t TICK_SIZE.from
 000005a0: 2063 6378 742e 6261 7365 2e70 7265 6369   ccxt.base.preci
```

### Comparing `ccxt-4.2.94/ccxt/async_support/krakenfutures.py` & `ccxt-4.2.95/ccxt/async_support/krakenfutures.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.krakenfutures import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Leverage, Leverages, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import OrderImmediatelyFillable
 from ccxt.base.errors import OrderNotFillable
 from ccxt.base.errors import DuplicateOrderId
+from ccxt.base.errors import ContractUnavailable
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
-from ccxt.base.errors import ContractUnavailable
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class krakenfutures(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/kucoin.py` & `ccxt-4.2.95/ccxt/async_support/kucoin.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 import asyncio
 import hashlib
 import math
 import json
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class kucoin(Exchange, ImplicitAPI):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/kucoinfutures.py` & `ccxt-4.2.95/ccxt/async_support/kucoinfutures.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.async_support.kucoin import kucoin
 from ccxt.abstract.kucoinfutures import ImplicitAPI
 from ccxt.base.types import Balances, Currency, Int, MarginModification, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class kucoinfutures(kucoin, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/kuna.py` & `ccxt-4.2.95/ccxt/async_support/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/latoken.py` & `ccxt-4.2.95/ccxt/async_support/latoken.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.latoken import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class latoken(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(latoken, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/async_support/lbank.py` & `ccxt-4.2.95/ccxt/async_support/lbank.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,46 +31,46 @@
 000001e0: 6746 6565 732c 2054 7261 6e73 6163 7469  gFees, Transacti
 000001f0: 6f6e 0a66 726f 6d20 7479 7069 6e67 2069  on.from typing i
 00000200: 6d70 6f72 7420 4c69 7374 0a66 726f 6d20  mport List.from 
 00000210: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
 00000220: 2069 6d70 6f72 7420 4578 6368 616e 6765   import Exchange
 00000230: 4572 726f 720a 6672 6f6d 2063 6378 742e  Error.from ccxt.
 00000240: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-00000250: 7274 2050 6572 6d69 7373 696f 6e44 656e  rt PermissionDen
-00000260: 6965 640a 6672 6f6d 2063 6378 742e 6261  ied.from ccxt.ba
-00000270: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000280: 2041 7267 756d 656e 7473 5265 7175 6972   ArgumentsRequir
-00000290: 6564 0a66 726f 6d20 6363 7874 2e62 6173  ed.from ccxt.bas
-000002a0: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
-000002b0: 4261 6452 6571 7565 7374 0a66 726f 6d20  BadRequest.from 
-000002c0: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-000002d0: 2069 6d70 6f72 7420 4261 6453 796d 626f   import BadSymbo
-000002e0: 6c0a 6672 6f6d 2063 6378 742e 6261 7365  l.from ccxt.base
-000002f0: 2e65 7272 6f72 7320 696d 706f 7274 2049  .errors import I
-00000300: 6e73 7566 6669 6369 656e 7446 756e 6473  nsufficientFunds
-00000310: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-00000320: 6572 726f 7273 2069 6d70 6f72 7420 496e  errors import In
-00000330: 7661 6c69 6441 6464 7265 7373 0a66 726f  validAddress.fro
-00000340: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-00000350: 7273 2069 6d70 6f72 7420 496e 7661 6c69  rs import Invali
-00000360: 644f 7264 6572 0a66 726f 6d20 6363 7874  dOrder.from ccxt
-00000370: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000380: 6f72 7420 4475 706c 6963 6174 654f 7264  ort DuplicateOrd
-00000390: 6572 4964 0a66 726f 6d20 6363 7874 2e62  erId.from ccxt.b
-000003a0: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
-000003b0: 7420 4e6f 7453 7570 706f 7274 6564 0a66  t NotSupported.f
-000003c0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-000003d0: 726f 7273 2069 6d70 6f72 7420 5261 7465  rors import Rate
-000003e0: 4c69 6d69 7445 7863 6565 6465 640a 6672  LimitExceeded.fr
-000003f0: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-00000400: 6f72 7320 696d 706f 7274 2049 6e76 616c  ors import Inval
-00000410: 6964 4e6f 6e63 650a 6672 6f6d 2063 6378  idNonce.from ccx
-00000420: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
-00000430: 706f 7274 2041 7574 6865 6e74 6963 6174  port Authenticat
-00000440: 696f 6e45 7272 6f72 0a66 726f 6d20 6363  ionError.from cc
+00000250: 7274 2041 7574 6865 6e74 6963 6174 696f  rt Authenticatio
+00000260: 6e45 7272 6f72 0a66 726f 6d20 6363 7874  nError.from ccxt
+00000270: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+00000280: 6f72 7420 5065 726d 6973 7369 6f6e 4465  ort PermissionDe
+00000290: 6e69 6564 0a66 726f 6d20 6363 7874 2e62  nied.from ccxt.b
+000002a0: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+000002b0: 7420 4172 6775 6d65 6e74 7352 6571 7569  t ArgumentsRequi
+000002c0: 7265 640a 6672 6f6d 2063 6378 742e 6261  red.from ccxt.ba
+000002d0: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
+000002e0: 2042 6164 5265 7175 6573 740a 6672 6f6d   BadRequest.from
+000002f0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+00000300: 7320 696d 706f 7274 2042 6164 5379 6d62  s import BadSymb
+00000310: 6f6c 0a66 726f 6d20 6363 7874 2e62 6173  ol.from ccxt.bas
+00000320: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+00000330: 496e 7375 6666 6963 6965 6e74 4675 6e64  InsufficientFund
+00000340: 730a 6672 6f6d 2063 6378 742e 6261 7365  s.from ccxt.base
+00000350: 2e65 7272 6f72 7320 696d 706f 7274 2049  .errors import I
+00000360: 6e76 616c 6964 4164 6472 6573 730a 6672  nvalidAddress.fr
+00000370: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+00000380: 6f72 7320 696d 706f 7274 2049 6e76 616c  ors import Inval
+00000390: 6964 4f72 6465 720a 6672 6f6d 2063 6378  idOrder.from ccx
+000003a0: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+000003b0: 706f 7274 2044 7570 6c69 6361 7465 4f72  port DuplicateOr
+000003c0: 6465 7249 640a 6672 6f6d 2063 6378 742e  derId.from ccxt.
+000003d0: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
+000003e0: 7274 204e 6f74 5375 7070 6f72 7465 640a  rt NotSupported.
+000003f0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+00000400: 7272 6f72 7320 696d 706f 7274 2052 6174  rrors import Rat
+00000410: 654c 696d 6974 4578 6365 6564 6564 0a66  eLimitExceeded.f
+00000420: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+00000430: 726f 7273 2069 6d70 6f72 7420 496e 7661  rors import Inva
+00000440: 6c69 644e 6f6e 6365 0a66 726f 6d20 6363  lidNonce.from cc
 00000450: 7874 2e62 6173 652e 6465 6369 6d61 6c5f  xt.base.decimal_
 00000460: 746f 5f70 7265 6369 7369 6f6e 2069 6d70  to_precision imp
 00000470: 6f72 7420 5449 434b 5f53 495a 450a 6672  ort TICK_SIZE.fr
 00000480: 6f6d 2063 6378 742e 6261 7365 2e70 7265  om ccxt.base.pre
 00000490: 6369 7365 2069 6d70 6f72 7420 5072 6563  cise import Prec
 000004a0: 6973 650a 0a0a 636c 6173 7320 6c62 616e  ise...class lban
 000004b0: 6b28 4578 6368 616e 6765 2c20 496d 706c  k(Exchange, Impl
```

### Comparing `ccxt-4.2.94/ccxt/async_support/luno.py` & `ccxt-4.2.95/ccxt/async_support/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/lykke.py` & `ccxt-4.2.95/ccxt/async_support/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/mercado.py` & `ccxt-4.2.95/ccxt/async_support/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/mexc.py` & `ccxt-4.2.95/ccxt/async_support/mexc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.mexc import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, IndexType, Int, Leverage, MarginModification, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class mexc(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/ndax.py` & `ccxt-4.2.95/ccxt/async_support/ndax.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.ndax import ImplicitAPI
 import hashlib
 import json
 from ccxt.base.types import Account, Balances, Currencies, Currency, IndexType, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Ticker, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import OrderNotFound
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class ndax(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/novadax.py` & `ccxt-4.2.95/ccxt/async_support/novadax.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.novadax import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountNotEnabled
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import CancelPending
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class novadax(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/oceanex.py` & `ccxt-4.2.95/ccxt/async_support/oceanex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.oceanex import ImplicitAPI
 from ccxt.base.types import Balances, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class oceanex(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(oceanex, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/async_support/okcoin.py` & `ccxt-4.2.95/ccxt/async_support/okcoin.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,66 +29,66 @@
 000001c0: 652c 2054 7261 6e73 6163 7469 6f6e 2c20  e, Transaction, 
 000001d0: 5472 616e 7366 6572 456e 7472 790a 6672  TransferEntry.fr
 000001e0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
 000001f0: 204c 6973 740a 6672 6f6d 2063 6378 742e   List.from ccxt.
 00000200: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
 00000210: 7274 2045 7863 6861 6e67 6545 7272 6f72  rt ExchangeError
 00000220: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-00000230: 6572 726f 7273 2069 6d70 6f72 7420 5065  errors import Pe
-00000240: 726d 6973 7369 6f6e 4465 6e69 6564 0a66  rmissionDenied.f
-00000250: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-00000260: 726f 7273 2069 6d70 6f72 7420 4163 636f  rors import Acco
-00000270: 756e 744e 6f74 456e 6162 6c65 640a 6672  untNotEnabled.fr
-00000280: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-00000290: 6f72 7320 696d 706f 7274 2041 6363 6f75  ors import Accou
-000002a0: 6e74 5375 7370 656e 6465 640a 6672 6f6d  ntSuspended.from
-000002b0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-000002c0: 7320 696d 706f 7274 2041 7267 756d 656e  s import Argumen
-000002d0: 7473 5265 7175 6972 6564 0a66 726f 6d20  tsRequired.from 
-000002e0: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-000002f0: 2069 6d70 6f72 7420 4261 6452 6571 7565   import BadReque
-00000300: 7374 0a66 726f 6d20 6363 7874 2e62 6173  st.from ccxt.bas
-00000310: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
-00000320: 4261 6453 796d 626f 6c0a 6672 6f6d 2063  BadSymbol.from c
-00000330: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-00000340: 696d 706f 7274 2049 6e73 7566 6669 6369  import Insuffici
-00000350: 656e 7446 756e 6473 0a66 726f 6d20 6363  entFunds.from cc
-00000360: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
-00000370: 6d70 6f72 7420 496e 7661 6c69 6441 6464  mport InvalidAdd
-00000380: 7265 7373 0a66 726f 6d20 6363 7874 2e62  ress.from ccxt.b
-00000390: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
-000003a0: 7420 496e 7661 6c69 644f 7264 6572 0a66  t InvalidOrder.f
-000003b0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-000003c0: 726f 7273 2069 6d70 6f72 7420 4f72 6465  rors import Orde
-000003d0: 724e 6f74 466f 756e 640a 6672 6f6d 2063  rNotFound.from c
-000003e0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-000003f0: 696d 706f 7274 2043 616e 6365 6c50 656e  import CancelPen
-00000400: 6469 6e67 0a66 726f 6d20 6363 7874 2e62  ding.from ccxt.b
-00000410: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
-00000420: 7420 4e6f 7453 7570 706f 7274 6564 0a66  t NotSupported.f
-00000430: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-00000440: 726f 7273 2069 6d70 6f72 7420 4e65 7477  rors import Netw
-00000450: 6f72 6b45 7272 6f72 0a66 726f 6d20 6363  orkError.from cc
-00000460: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
-00000470: 6d70 6f72 7420 5261 7465 4c69 6d69 7445  mport RateLimitE
-00000480: 7863 6565 6465 640a 6672 6f6d 2063 6378  xceeded.from ccx
-00000490: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
-000004a0: 706f 7274 2045 7863 6861 6e67 654e 6f74  port ExchangeNot
-000004b0: 4176 6169 6c61 626c 650a 6672 6f6d 2063  Available.from c
-000004c0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-000004d0: 696d 706f 7274 204f 6e4d 6169 6e74 656e  import OnMainten
-000004e0: 616e 6365 0a66 726f 6d20 6363 7874 2e62  ance.from ccxt.b
-000004f0: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
-00000500: 7420 496e 7661 6c69 644e 6f6e 6365 0a66  t InvalidNonce.f
-00000510: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-00000520: 726f 7273 2069 6d70 6f72 7420 5265 7175  rors import Requ
-00000530: 6573 7454 696d 656f 7574 0a66 726f 6d20  estTimeout.from 
-00000540: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-00000550: 2069 6d70 6f72 7420 4175 7468 656e 7469   import Authenti
-00000560: 6361 7469 6f6e 4572 726f 720a 6672 6f6d  cationError.from
+00000230: 6572 726f 7273 2069 6d70 6f72 7420 4175  errors import Au
+00000240: 7468 656e 7469 6361 7469 6f6e 4572 726f  thenticationErro
+00000250: 720a 6672 6f6d 2063 6378 742e 6261 7365  r.from ccxt.base
+00000260: 2e65 7272 6f72 7320 696d 706f 7274 2050  .errors import P
+00000270: 6572 6d69 7373 696f 6e44 656e 6965 640a  ermissionDenied.
+00000280: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+00000290: 7272 6f72 7320 696d 706f 7274 2041 6363  rrors import Acc
+000002a0: 6f75 6e74 4e6f 7445 6e61 626c 6564 0a66  ountNotEnabled.f
+000002b0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+000002c0: 726f 7273 2069 6d70 6f72 7420 4163 636f  rors import Acco
+000002d0: 756e 7453 7573 7065 6e64 6564 0a66 726f  untSuspended.fro
+000002e0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+000002f0: 7273 2069 6d70 6f72 7420 4172 6775 6d65  rs import Argume
+00000300: 6e74 7352 6571 7569 7265 640a 6672 6f6d  ntsRequired.from
+00000310: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+00000320: 7320 696d 706f 7274 2042 6164 5265 7175  s import BadRequ
+00000330: 6573 740a 6672 6f6d 2063 6378 742e 6261  est.from ccxt.ba
+00000340: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
+00000350: 2042 6164 5379 6d62 6f6c 0a66 726f 6d20   BadSymbol.from 
+00000360: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
+00000370: 2069 6d70 6f72 7420 496e 7375 6666 6963   import Insuffic
+00000380: 6965 6e74 4675 6e64 730a 6672 6f6d 2063  ientFunds.from c
+00000390: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+000003a0: 696d 706f 7274 2049 6e76 616c 6964 4164  import InvalidAd
+000003b0: 6472 6573 730a 6672 6f6d 2063 6378 742e  dress.from ccxt.
+000003c0: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
+000003d0: 7274 2049 6e76 616c 6964 4f72 6465 720a  rt InvalidOrder.
+000003e0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+000003f0: 7272 6f72 7320 696d 706f 7274 204f 7264  rrors import Ord
+00000400: 6572 4e6f 7446 6f75 6e64 0a66 726f 6d20  erNotFound.from 
+00000410: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
+00000420: 2069 6d70 6f72 7420 4361 6e63 656c 5065   import CancelPe
+00000430: 6e64 696e 670a 6672 6f6d 2063 6378 742e  nding.from ccxt.
+00000440: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
+00000450: 7274 204e 6f74 5375 7070 6f72 7465 640a  rt NotSupported.
+00000460: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+00000470: 7272 6f72 7320 696d 706f 7274 204e 6574  rrors import Net
+00000480: 776f 726b 4572 726f 720a 6672 6f6d 2063  workError.from c
+00000490: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+000004a0: 696d 706f 7274 2052 6174 654c 696d 6974  import RateLimit
+000004b0: 4578 6365 6564 6564 0a66 726f 6d20 6363  Exceeded.from cc
+000004c0: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
+000004d0: 6d70 6f72 7420 4578 6368 616e 6765 4e6f  mport ExchangeNo
+000004e0: 7441 7661 696c 6162 6c65 0a66 726f 6d20  tAvailable.from 
+000004f0: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
+00000500: 2069 6d70 6f72 7420 4f6e 4d61 696e 7465   import OnMainte
+00000510: 6e61 6e63 650a 6672 6f6d 2063 6378 742e  nance.from ccxt.
+00000520: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
+00000530: 7274 2049 6e76 616c 6964 4e6f 6e63 650a  rt InvalidNonce.
+00000540: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+00000550: 7272 6f72 7320 696d 706f 7274 2052 6571  rrors import Req
+00000560: 7565 7374 5469 6d65 6f75 740a 6672 6f6d  uestTimeout.from
 00000570: 2063 6378 742e 6261 7365 2e64 6563 696d   ccxt.base.decim
 00000580: 616c 5f74 6f5f 7072 6563 6973 696f 6e20  al_to_precision 
 00000590: 696d 706f 7274 2054 4943 4b5f 5349 5a45  import TICK_SIZE
 000005a0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
 000005b0: 7072 6563 6973 6520 696d 706f 7274 2050  precise import P
 000005c0: 7265 6369 7365 0a0a 0a63 6c61 7373 206f  recise...class o
 000005d0: 6b63 6f69 6e28 4578 6368 616e 6765 2c20  kcoin(Exchange,
```

### Comparing `ccxt-4.2.94/ccxt/async_support/okx.py` & `ccxt-4.2.95/ccxt/async_support/okx.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.okx import ImplicitAPI
 import asyncio
 import hashlib
 from ccxt.base.types import Account, Balances, Conversion, Currencies, Currency, Greeks, Int, Leverage, MarginModification, Market, MarketInterface, Num, Option, OptionChain, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountNotEnabled
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import CancelPending
+from ccxt.base.errors import ContractUnavailable
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
-from ccxt.base.errors import ContractUnavailable
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class okx(Exchange, ImplicitAPI):
 
     def describe(self):
@@ -1135,15 +1135,15 @@
         params = self.omit(params, 'instType')
         type = self.safe_string(params, 'type')
         if (type is None) and (instType is not None):
             params['type'] = instType
         return super(okx, self).handle_market_type_and_params(methodName, market, params)
 
     def convert_to_instrument_type(self, type):
-        exchangeTypes = self.safe_value(self.options, 'exchangeType', {})
+        exchangeTypes = self.safe_dict(self.options, 'exchangeType', {})
         return self.safe_string(exchangeTypes, type, type)
 
     def create_expired_option_market(self, symbol: str):
         # support expired option contracts
         quote = 'USD'
         optionParts = symbol.split('-')
         symbolBase = symbol.split('/')
@@ -2769,15 +2769,15 @@
         for i in range(0, len(orders)):
             rawOrder = orders[i]
             marketId = self.safe_string(rawOrder, 'symbol')
             type = self.safe_string(rawOrder, 'type')
             side = self.safe_string(rawOrder, 'side')
             amount = self.safe_value(rawOrder, 'amount')
             price = self.safe_value(rawOrder, 'price')
-            orderParams = self.safe_value(rawOrder, 'params', {})
+            orderParams = self.safe_dict(rawOrder, 'params', {})
             extendedParams = self.extend(orderParams, params)  # the request does not accept extra params since it's a list, so we're extending each order with the common params
             orderRequest = self.create_order_request(marketId, type, side, amount, price, extendedParams)
             ordersRequests.append(orderRequest)
         response = await self.privatePostTradeBatchOrders(ordersRequests)
         # {
         #     "code": "0",
         #     "data": [
@@ -2931,16 +2931,16 @@
         #                 "sCode": "0",
         #                 "sMsg": ""
         #            }
         #        ],
         #        "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data', [])
-        first = self.safe_value(data, 0)
+        data = self.safe_list(response, 'data', [])
+        first = self.safe_dict(data, 0, {})
         order = self.parse_order(first, market)
         order['type'] = type
         order['side'] = side
         return order
 
     async def cancel_order(self, id: str, symbol: Str = None, params={}):
         """
@@ -4037,15 +4037,15 @@
         :returns dict: a `ledger structure <https://docs.ccxt.com/#/?id=ledger-structure>`
         """
         await self.load_markets()
         paginate = False
         paginate, params = self.handle_option_and_params(params, 'fetchLedger', 'paginate')
         if paginate:
             return await self.fetch_paginated_call_dynamic('fetchLedger', code, since, limit, params)
-        options = self.safe_value(self.options, 'fetchLedger', {})
+        options = self.safe_dict(self.options, 'fetchLedger', {})
         method = self.safe_string(options, 'method')
         method = self.safe_string(params, 'method', method)
         params = self.omit(params, 'method')
         request = {
             # 'instType': None,  # 'SPOT', 'MARGIN', 'SWAP', 'FUTURES", 'OPTION'
             # 'ccy': None,  # currency['id'],
             # 'mgnMode': None,  # 'isolated', 'cross'
@@ -4352,15 +4352,15 @@
         #             # {"ccy":"usdt-erc20","to":"6","addr":"0x696abb81974a8793352cbd33aadcf78eda3cfdfa","selected":true},
         #             # {"ccy":"usdt-trc20","to":"6","addr":"TRrd5SiSZrfQVRKm4e9SRSbn2LNTYqCjqx","selected":true},
         #             # {"ccy":"usdt_okexchain","to":"6","addr":"0x696abb81974a8793352cbd33aadcf78eda3cfdfa","selected":true},
         #             # {"ccy":"usdt_kip20","to":"6","addr":"0x696abb81974a8793352cbd33aadcf78eda3cfdfa","selected":true},
         #         ]
         #     }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         filtered = self.filter_by(data, 'selected', True)
         parsed = self.parse_deposit_addresses(filtered, [currency['code']], False)
         return self.index_by(parsed, 'network')
 
     async def fetch_deposit_address(self, code: str, params={}):
         """
         fetch the deposit address for a currency associated with self account
@@ -4415,23 +4415,23 @@
             'ccy': currency['id'],
             'toAddr': address,
             'dest': '4',  # 2 = OKCoin International, 3 = OKX 4 = others
             'amt': self.number_to_string(amount),
         }
         network = self.safe_string(params, 'network')  # self line allows the user to specify either ERC20 or ETH
         if network is not None:
-            networks = self.safe_value(self.options, 'networks', {})
+            networks = self.safe_dict(self.options, 'networks', {})
             network = self.safe_string(networks, network.upper(), network)  # handle ETH>ERC20 alias
             request['chain'] = currency['id'] + '-' + network
             params = self.omit(params, 'network')
         fee = self.safe_string(params, 'fee')
         if fee is None:
             currencies = await self.fetch_currencies()
             self.currencies = self.deep_extend(self.currencies, currencies)
-            targetNetwork = self.safe_value(currency['networks'], self.network_id_to_code(network), {})
+            targetNetwork = self.safe_dict(currency['networks'], self.network_id_to_code(network), {})
             fee = self.safe_string(targetNetwork, 'fee')
             if fee is None:
                 raise ArgumentsRequired(self.id + ' withdraw() requires a "fee" string parameter, network transaction fee must be ≥ 0. Withdrawals to OKCoin or OKX are fee-free, please set "0". Withdrawing to external digital asset address requires network transaction fee.')
         request['fee'] = self.number_to_string(fee)  # withdrawals to OKCoin or OKX are fee-free, please set 0
         query = self.omit(params, ['fee'])
         response = await self.privatePostAssetWithdrawal(self.extend(request, query))
         #
@@ -4443,15 +4443,15 @@
         #                 "amt": "0.1",
         #                 "wdId": "67485",
         #                 "ccy": "BTC"
         #             }
         #         ]
         #     }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         transaction = self.safe_dict(data, 0)
         return self.parse_transaction(transaction, currency)
 
     async def fetch_deposits(self, code: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Transaction]:
         """
         fetch all deposits made to an account
         :see: https://www.okx.com/docs-v5/en/#rest-api-funding-get-deposit-history
@@ -4650,15 +4650,15 @@
         #                "ts": "1641376485000",
         #                "wdId": "25147041"
         #            }
         #        ],
         #        "msg": ''
         #    }
         #
-        data = self.safe_value(response, 'data')
+        data = self.safe_list(response, 'data', [])
         withdrawal = self.safe_dict(data, 0, {})
         return self.parse_transaction(withdrawal)
 
     def parse_transaction_status(self, status):
         #
         # deposit statuses
         #
@@ -4922,16 +4922,16 @@
         #                 "uplRatio": "-0.0025490556801078",
         #                 "vegaBS": "",
         #                 "vegaPA": ""
         #             }
         #         ]
         #     }
         #
-        data = self.safe_value(response, 'data', [])
-        position = self.safe_value(data, 0)
+        data = self.safe_list(response, 'data', [])
+        position = self.safe_dict(data, 0)
         if position is None:
             return None
         return self.parse_position(position, market)
 
     async def fetch_positions(self, symbols: Strings = None, params={}):
         """
         :see: https://www.okx.com/docs-v5/en/#rest-api-account-get-positions
@@ -4953,15 +4953,15 @@
             for i in range(0, len(symbols)):
                 entry = symbols[i]
                 market = self.market(entry)
                 marketIds.append(market['id'])
             marketIdsLength = len(marketIds)
             if marketIdsLength > 0:
                 request['instId'] = ','.join(marketIds)
-        fetchPositionsOptions = self.safe_value(self.options, 'fetchPositions', {})
+        fetchPositionsOptions = self.safe_dict(self.options, 'fetchPositions', {})
         method = self.safe_string(fetchPositionsOptions, 'method', 'privateGetAccountPositions')
         response = None
         if method == 'privateGetAccountPositionsHistory':
             response = await self.privateGetAccountPositionsHistory(self.extend(request, params))
         else:
             response = await self.privateGetAccountPositions(self.extend(request, params))
         #
@@ -5006,15 +5006,15 @@
         #                 "uplRatio": "-0.0025490556801078",
         #                 "vegaBS": "",
         #                 "vegaPA": ""
         #             }
         #         ]
         #     }
         #
-        positions = self.safe_value(response, 'data', [])
+        positions = self.safe_list(response, 'data', [])
         result = []
         for i in range(0, len(positions)):
             result.append(self.parse_position(positions[i]))
         return self.filter_by_array_positions(result, 'symbol', symbols, False)
 
     async def fetch_positions_for_symbol(self, symbol: str, params={}):
         """
@@ -5194,15 +5194,15 @@
         :param str fromAccount: account to transfer from
         :param str toAccount: account to transfer to
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `transfer structure <https://docs.ccxt.com/#/?id=transfer-structure>`
         """
         await self.load_markets()
         currency = self.currency(code)
-        accountsByType = self.safe_value(self.options, 'accountsByType', {})
+        accountsByType = self.safe_dict(self.options, 'accountsByType', {})
         fromId = self.safe_string(accountsByType, fromAccount, fromAccount)
         toId = self.safe_string(accountsByType, toAccount, toAccount)
         request = {
             'ccy': currency['id'],
             'amt': self.currency_to_precision(code, amount),
             'type': '0',  # 0 = transfer within account by default, 1 = master account to sub-account, 2 = sub-account to master account, 3 = sub-account to master account(Only applicable to APIKey from sub-account), 4 = sub-account to sub-account
             'from': fromId,  # remitting account, 6: Funding account, 18: Trading account
@@ -5234,15 +5234,15 @@
         #                 "from": "6",
         #                 "amt": "0.1",
         #                 "to": "18"
         #             }
         #         ]
         #     }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         rawTransfer = self.safe_dict(data, 0, {})
         return self.parse_transfer(rawTransfer, currency)
 
     def parse_transfer(self, transfer, currency: Currency = None):
         #
         # transfer
         #
@@ -5297,15 +5297,15 @@
         #
         id = self.safe_string_2(transfer, 'transId', 'billId')
         currencyId = self.safe_string(transfer, 'ccy')
         code = self.safe_currency_code(currencyId, currency)
         amount = self.safe_number(transfer, 'amt')
         fromAccountId = self.safe_string(transfer, 'from')
         toAccountId = self.safe_string(transfer, 'to')
-        accountsById = self.safe_value(self.options, 'accountsById', {})
+        accountsById = self.safe_dict(self.options, 'accountsById', {})
         timestamp = self.safe_integer(transfer, 'ts')
         balanceChange = self.safe_string(transfer, 'sz')
         if balanceChange is not None:
             amount = self.parse_number(Precise.string_abs(balanceChange))
         return {
             'info': transfer,
             'id': id,
@@ -5347,15 +5347,15 @@
         #                 "transId": "464424732",
         #                 "type": "0"
         #             }
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         transfer = self.safe_dict(data, 0)
         return self.parse_transfer(transfer)
 
     async def fetch_transfers(self, code: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         fetch a history of internal transfers made on an account
         :see: https://www.okx.com/docs-v5/en/#trading-account-rest-api-get-bills-details-last-3-months
@@ -5532,16 +5532,16 @@
         #                "nextFundingRate": "0.00017",
         #                "nextFundingTime": "1634284800000"
         #            }
         #        ],
         #        "msg": ""
         #    }
         #
-        data = self.safe_value(response, 'data', [])
-        entry = self.safe_value(data, 0, {})
+        data = self.safe_list(response, 'data', [])
+        entry = self.safe_dict(data, 0, {})
         return self.parse_funding_rate(entry, market)
 
     async def fetch_funding_history(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         fetch the history of funding payments paid and received on self account
         :see: https://www.okx.com/docs-v5/en/#trading-account-rest-api-get-bills-details-last-3-months
         :param str symbol: unified market symbol
@@ -5665,15 +5665,15 @@
         #        "subType": "174",
         #        "sz": "9",
         #        "to": "",
         #        "ts": "1636387215588",
         #        "type": "8"
         #    }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         result = []
         for i in range(0, len(data)):
             entry = data[i]
             timestamp = self.safe_integer(entry, 'ts')
             instId = self.safe_string(entry, 'instId')
             marketInner = self.safe_market(instId)
             currencyId = self.safe_string(entry, 'ccy')
@@ -5836,15 +5836,15 @@
         #                "ccy": "BTC",
         #                "interestRate": "0.00000833"
         #            }
         #            ...
         #        ],
         #    }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         rates = []
         for i in range(0, len(data)):
             rates.append(self.parse_borrow_rate(data[i]))
         return rates
 
     async def fetch_cross_borrow_rate(self, code: str, params={}):
         """
@@ -5869,16 +5869,16 @@
         #                "interestRate": "0.00002065"
         #             }
         #             ...
         #        ],
         #        "msg": ""
         #    }
         #
-        data = self.safe_value(response, 'data')
-        rate = self.safe_value(data, 0)
+        data = self.safe_list(response, 'data', [])
+        rate = self.safe_dict(data, 0, {})
         return self.parse_borrow_rate(rate)
 
     def parse_borrow_rate(self, info, currency: Currency = None):
         #
         #    {
         #        "amt": "992.10341195",
         #        "ccy": "BTC",
@@ -5965,15 +5965,15 @@
         #                 "rate": "0.01",
         #                 "ts": "1643954400000"
         #             },
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data')
+        data = self.safe_list(response, 'data', [])
         return self.parse_borrow_rate_histories(data, codes, since, limit)
 
     async def fetch_borrow_rate_history(self, code: str, since: Int = None, limit: Int = None, params={}):
         """
         retrieves a history of a currencies borrow interest rate at specific time slots
         :see: https://www.okx.com/docs-v5/en/#financial-product-savings-get-public-borrow-history-public
         :param str code: unified currency code
@@ -6005,15 +6005,15 @@
         #                 "rate": "0.01",
         #                 "ts": "1643954400000"
         #             },
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data')
+        data = self.safe_list(response, 'data', [])
         return self.parse_borrow_rate_history(data, code, since, limit)
 
     async def modify_margin_helper(self, symbol: str, amount, type, params={}) -> MarginModification:
         await self.load_markets()
         market = self.market(symbol)
         posSide = self.safe_string(params, 'posSide', 'net')
         params = self.omit(params, ['posSide'])
@@ -6185,15 +6185,15 @@
         #                "tier": "1",
         #                "uly": ""
         #            },
         #            ...
         #        ]
         #    }
         #
-        data = self.safe_value(response, 'data')
+        data = self.safe_list(response, 'data', [])
         return self.parse_market_leverage_tiers(data, market)
 
     def parse_market_leverage_tiers(self, info, market: Market = None):
         """
          * @ignore
         :param dict info: Exchange response for 1 market
         :param dict market: CCXT market
@@ -6278,15 +6278,15 @@
         #                "type": "1"
         #            },
         #            ...
         #        ],
         #        "msg": ""
         #    }
         #
-        data = self.safe_value(response, 'data')
+        data = self.safe_list(response, 'data', [])
         interest = self.parse_borrow_interests(data)
         return self.filter_by_currency_since_limit(interest, code, since, limit)
 
     def parse_borrow_interest(self, info, market: Market = None):
         instId = self.safe_string(info, 'instId')
         if instId is not None:
             market = self.safe_market(instId, market)
@@ -6331,16 +6331,16 @@
         #                 "side": "borrow",
         #                 "state": "1"
         #             }
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data', [])
-        loan = self.safe_value(data, 0)
+        data = self.safe_list(response, 'data', [])
+        loan = self.safe_dict(data, 0, {})
         return self.parse_margin_loan(loan, currency)
 
     async def repay_cross_margin(self, code: str, amount, params={}):
         """
         repay borrowed margin and interest
         :see: https://www.okx.com/docs-v5/en/#trading-account-rest-api-vip-loans-borrow-and-repay
         :param str code: unified currency code of the currency to repay
@@ -6373,16 +6373,16 @@
         #                 "side": "repay",
         #                 "state": "1"
         #             }
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data', [])
-        loan = self.safe_value(data, 0)
+        data = self.safe_list(response, 'data', [])
+        loan = self.safe_dict(data, 0, {})
         return self.parse_margin_loan(loan, currency)
 
     def parse_margin_loan(self, info, currency: Currency = None):
         #
         #     {
         #         "amt": "102",
         #         "availLoan": "97",
@@ -6451,16 +6451,16 @@
         :param str timeframe: "5m", "1h", or "1d" for option only "1d" or "8h"
         :param int [since]: The time in ms of the earliest record to retrieve unix timestamp
         :param int [limit]: Not used by okx, but parsed internally by CCXT
         :param dict [params]: Exchange specific parameters
         :param int [params.until]: The time in ms of the latest record to retrieve unix timestamp
         :returns: An array of `open interest structures <https://docs.ccxt.com/#/?id=open-interest-structure>`
         """
-        options = self.safe_value(self.options, 'fetchOpenInterestHistory', {})
-        timeframes = self.safe_value(options, 'timeframes', {})
+        options = self.safe_dict(self.options, 'fetchOpenInterestHistory', {})
+        timeframes = self.safe_dict(options, 'timeframes', {})
         timeframe = self.safe_string(timeframes, timeframe, timeframe)
         if timeframe != '5m' and timeframe != '1H' and timeframe != '1D':
             raise BadRequest(self.id + ' fetchOpenInterestHistory cannot only use the 5m, 1h, and 1d timeframe')
         await self.load_markets()
         # handle unified currency code or symbol
         currencyId = None
         market = None
@@ -6717,15 +6717,15 @@
         #                 ],
         #                 "ts":"1684656000000"
         #             }
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         settlements = self.parse_settlements(data, market)
         sorted = self.sort_by(settlements, 'timestamp')
         return self.filter_by_symbol_since_limit(sorted, market['symbol'], since, limit)
 
     def parse_settlement(self, settlement, market):
         #
         #     {
@@ -6756,15 +6756,15 @@
         #         "ts":"1684656000000"
         #     }
         #
         result = []
         for i in range(0, len(settlements)):
             entry = settlements[i]
             timestamp = self.safe_integer(entry, 'ts')
-            details = self.safe_value(entry, 'details', [])
+            details = self.safe_list(entry, 'details', [])
             for j in range(0, len(details)):
                 settlement = self.parse_settlement(details[j], market)
                 result.append(self.extend(settlement, {
                     'timestamp': timestamp,
                     'datetime': self.iso8601(timestamp),
                 }))
         return result
@@ -6796,15 +6796,15 @@
         #                 "BTC-USD",
         #                 "ETH-USD"
         #             ]
         #         ],
         #         "msg": ""
         #     }
         #
-        underlyings = self.safe_value(response, 'data', [])
+        underlyings = self.safe_list(response, 'data', [])
         return underlyings[0]
 
     async def fetch_greeks(self, symbol: str, params={}) -> Greeks:
         """
         fetches an option contracts greeks, financial metrics used to measure the factors that affect the price of an options contract
         :see: https://www.okx.com/docs-v5/en/#public-data-rest-api-get-option-market-data
         :param str symbol: unified symbol of the market to fetch greeks for
@@ -6846,15 +6846,15 @@
         #                 "vegaBS": "74.44022302387287",
         #                 "volLv": "0.5948549730405797"
         #             },
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         for i in range(0, len(data)):
             entry = data[i]
             entryMarketId = self.safe_string(entry, 'instId')
             if entryMarketId == marketId:
                 return self.parse_greeks(entry, market)
         return None
 
@@ -6959,15 +6959,15 @@
         #            }
         #        ],
         #        "inTime": "1701877077101064",
         #        "msg": "All operations failed",
         #        "outTime": "1701877077102579"
         #    }
         #
-        data = self.safe_value(response, 'data')
+        data = self.safe_list(response, 'data', [])
         order = self.safe_dict(data, 0)
         return self.parse_order(order, market)
 
     async def fetch_option(self, symbol: str, params={}) -> Option:
         """
         fetches option data that is commonly found in an option chain
         :see: https://www.okx.com/docs-v5/en/#order-book-trading-market-data-get-ticker
@@ -7268,15 +7268,15 @@
         #        "data": [],
         #        "msg": "Incorrect trade password"
         #    }
         #
         code = self.safe_string(response, 'code')
         if (code != '0') and (code != '2'):  # 2 means that bulk operation partially succeeded
             feedback = self.id + ' ' + body
-            data = self.safe_value(response, 'data', [])
+            data = self.safe_list(response, 'data', [])
             for i in range(0, len(data)):
                 error = data[i]
                 errorCode = self.safe_string(error, 'sCode')
                 message = self.safe_string(error, 'sMsg')
                 self.throw_exactly_matched_exception(self.exceptions['exact'], errorCode, feedback)
                 self.throw_broadly_matched_exception(self.exceptions['broad'], message, feedback)
             self.throw_exactly_matched_exception(self.exceptions['exact'], code, feedback)
```

### Comparing `ccxt-4.2.94/ccxt/async_support/onetrading.py` & `ccxt-4.2.95/ccxt/async_support/onetrading.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.onetrading import ImplicitAPI
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class onetrading(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/p2b.py` & `ccxt-4.2.95/ccxt/async_support/p2b.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.p2b import ImplicitAPI
 import hashlib
 from ccxt.base.types import Int, Market, Num, Order, OrderSide, OrderType, Str, Strings, Ticker, Tickers
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class p2b(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(p2b, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/async_support/paymium.py` & `ccxt-4.2.95/ccxt/async_support/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/phemex.py` & `ccxt-4.2.95/ccxt/async_support/phemex.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,51 +32,51 @@
 000001f0: 6e2c 2054 7261 6e73 6665 7245 6e74 7279  n, TransferEntry
 00000200: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
 00000210: 6f72 7420 4c69 7374 0a66 726f 6d20 6363  ort List.from cc
 00000220: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
 00000230: 6d70 6f72 7420 4578 6368 616e 6765 4572  mport ExchangeEr
 00000240: 726f 720a 6672 6f6d 2063 6378 742e 6261  ror.from ccxt.ba
 00000250: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000260: 2050 6572 6d69 7373 696f 6e44 656e 6965   PermissionDenie
-00000270: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
-00000280: 2e65 7272 6f72 7320 696d 706f 7274 2041  .errors import A
-00000290: 6363 6f75 6e74 5375 7370 656e 6465 640a  ccountSuspended.
-000002a0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-000002b0: 7272 6f72 7320 696d 706f 7274 2041 7267  rrors import Arg
-000002c0: 756d 656e 7473 5265 7175 6972 6564 0a66  umentsRequired.f
-000002d0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-000002e0: 726f 7273 2069 6d70 6f72 7420 4261 6452  rors import BadR
-000002f0: 6571 7565 7374 0a66 726f 6d20 6363 7874  equest.from ccxt
-00000300: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000310: 6f72 7420 4261 6453 796d 626f 6c0a 6672  ort BadSymbol.fr
-00000320: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-00000330: 6f72 7320 696d 706f 7274 2049 6e73 7566  ors import Insuf
-00000340: 6669 6369 656e 7446 756e 6473 0a66 726f  ficientFunds.fro
-00000350: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-00000360: 7273 2069 6d70 6f72 7420 496e 7661 6c69  rs import Invali
-00000370: 644f 7264 6572 0a66 726f 6d20 6363 7874  dOrder.from ccxt
-00000380: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000390: 6f72 7420 4f72 6465 724e 6f74 466f 756e  ort OrderNotFoun
-000003a0: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
-000003b0: 2e65 7272 6f72 7320 696d 706f 7274 2043  .errors import C
-000003c0: 616e 6365 6c50 656e 6469 6e67 0a66 726f  ancelPending.fro
-000003d0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-000003e0: 7273 2069 6d70 6f72 7420 4475 706c 6963  rs import Duplic
-000003f0: 6174 654f 7264 6572 4964 0a66 726f 6d20  ateOrderId.from 
-00000400: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-00000410: 2069 6d70 6f72 7420 4e6f 7453 7570 706f   import NotSuppo
-00000420: 7274 6564 0a66 726f 6d20 6363 7874 2e62  rted.from ccxt.b
-00000430: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
-00000440: 7420 4444 6f53 5072 6f74 6563 7469 6f6e  t DDoSProtection
-00000450: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-00000460: 6572 726f 7273 2069 6d70 6f72 7420 5261  errors import Ra
-00000470: 7465 4c69 6d69 7445 7863 6565 6465 640a  teLimitExceeded.
-00000480: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-00000490: 7272 6f72 7320 696d 706f 7274 2041 7574  rrors import Aut
-000004a0: 6865 6e74 6963 6174 696f 6e45 7272 6f72  henticationError
+00000260: 2041 7574 6865 6e74 6963 6174 696f 6e45   AuthenticationE
+00000270: 7272 6f72 0a66 726f 6d20 6363 7874 2e62  rror.from ccxt.b
+00000280: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+00000290: 7420 5065 726d 6973 7369 6f6e 4465 6e69  t PermissionDeni
+000002a0: 6564 0a66 726f 6d20 6363 7874 2e62 6173  ed.from ccxt.bas
+000002b0: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+000002c0: 4163 636f 756e 7453 7573 7065 6e64 6564  AccountSuspended
+000002d0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
+000002e0: 6572 726f 7273 2069 6d70 6f72 7420 4172  errors import Ar
+000002f0: 6775 6d65 6e74 7352 6571 7569 7265 640a  gumentsRequired.
+00000300: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+00000310: 7272 6f72 7320 696d 706f 7274 2042 6164  rrors import Bad
+00000320: 5265 7175 6573 740a 6672 6f6d 2063 6378  Request.from ccx
+00000330: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+00000340: 706f 7274 2042 6164 5379 6d62 6f6c 0a66  port BadSymbol.f
+00000350: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+00000360: 726f 7273 2069 6d70 6f72 7420 496e 7375  rors import Insu
+00000370: 6666 6963 6965 6e74 4675 6e64 730a 6672  fficientFunds.fr
+00000380: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+00000390: 6f72 7320 696d 706f 7274 2049 6e76 616c  ors import Inval
+000003a0: 6964 4f72 6465 720a 6672 6f6d 2063 6378  idOrder.from ccx
+000003b0: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+000003c0: 706f 7274 204f 7264 6572 4e6f 7446 6f75  port OrderNotFou
+000003d0: 6e64 0a66 726f 6d20 6363 7874 2e62 6173  nd.from ccxt.bas
+000003e0: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+000003f0: 4361 6e63 656c 5065 6e64 696e 670a 6672  CancelPending.fr
+00000400: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+00000410: 6f72 7320 696d 706f 7274 2044 7570 6c69  ors import Dupli
+00000420: 6361 7465 4f72 6465 7249 640a 6672 6f6d  cateOrderId.from
+00000430: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+00000440: 7320 696d 706f 7274 204e 6f74 5375 7070  s import NotSupp
+00000450: 6f72 7465 640a 6672 6f6d 2063 6378 742e  orted.from ccxt.
+00000460: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
+00000470: 7274 2044 446f 5350 726f 7465 6374 696f  rt DDoSProtectio
+00000480: 6e0a 6672 6f6d 2063 6378 742e 6261 7365  n.from ccxt.base
+00000490: 2e65 7272 6f72 7320 696d 706f 7274 2052  .errors import R
+000004a0: 6174 654c 696d 6974 4578 6365 6564 6564  ateLimitExceeded
 000004b0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
 000004c0: 6465 6369 6d61 6c5f 746f 5f70 7265 6369  decimal_to_preci
 000004d0: 7369 6f6e 2069 6d70 6f72 7420 5449 434b  sion import TICK
 000004e0: 5f53 495a 450a 6672 6f6d 2063 6378 742e  _SIZE.from ccxt.
 000004f0: 6261 7365 2e70 7265 6369 7365 2069 6d70  base.precise imp
 00000500: 6f72 7420 5072 6563 6973 650a 0a0a 636c  ort Precise...cl
 00000510: 6173 7320 7068 656d 6578 2845 7863 6861  ass phemex(Excha
```

### Comparing `ccxt-4.2.94/ccxt/async_support/poloniex.py` & `ccxt-4.2.95/ccxt/async_support/poloniex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.poloniex import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class poloniex(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/poloniexfutures.py` & `ccxt-4.2.95/ccxt/async_support/poloniexfutures.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.poloniexfutures import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class poloniexfutures(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/probit.py` & `ccxt-4.2.95/ccxt/async_support/probit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.probit import ImplicitAPI
 import math
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import BadResponse
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class probit(Exchange, ImplicitAPI):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/timex.py` & `ccxt-4.2.95/ccxt/async_support/timex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.timex import ImplicitAPI
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class timex(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/tokocrypto.py` & `ccxt-4.2.95/ccxt/async_support/tokocrypto.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,69 +29,69 @@
 000001c0: 5472 6164 652c 2054 7261 6e73 6163 7469  Trade, Transacti
 000001d0: 6f6e 0a66 726f 6d20 7479 7069 6e67 2069  on.from typing i
 000001e0: 6d70 6f72 7420 4c69 7374 0a66 726f 6d20  mport List.from 
 000001f0: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
 00000200: 2069 6d70 6f72 7420 4578 6368 616e 6765   import Exchange
 00000210: 4572 726f 720a 6672 6f6d 2063 6378 742e  Error.from ccxt.
 00000220: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-00000230: 7274 2050 6572 6d69 7373 696f 6e44 656e  rt PermissionDen
-00000240: 6965 640a 6672 6f6d 2063 6378 742e 6261  ied.from ccxt.ba
-00000250: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000260: 2041 6363 6f75 6e74 5375 7370 656e 6465   AccountSuspende
-00000270: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
-00000280: 2e65 7272 6f72 7320 696d 706f 7274 2041  .errors import A
-00000290: 7267 756d 656e 7473 5265 7175 6972 6564  rgumentsRequired
-000002a0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-000002b0: 6572 726f 7273 2069 6d70 6f72 7420 4261  errors import Ba
-000002c0: 6452 6571 7565 7374 0a66 726f 6d20 6363  dRequest.from cc
-000002d0: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
-000002e0: 6d70 6f72 7420 4261 6453 796d 626f 6c0a  mport BadSymbol.
-000002f0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-00000300: 7272 6f72 7320 696d 706f 7274 204d 6172  rrors import Mar
-00000310: 6769 6e4d 6f64 6541 6c72 6561 6479 5365  ginModeAlreadySe
-00000320: 740a 6672 6f6d 2063 6378 742e 6261 7365  t.from ccxt.base
-00000330: 2e65 7272 6f72 7320 696d 706f 7274 2042  .errors import B
-00000340: 6164 5265 7370 6f6e 7365 0a66 726f 6d20  adResponse.from 
-00000350: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-00000360: 2069 6d70 6f72 7420 496e 7375 6666 6963   import Insuffic
-00000370: 6965 6e74 4675 6e64 730a 6672 6f6d 2063  ientFunds.from c
-00000380: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-00000390: 696d 706f 7274 2049 6e76 616c 6964 4f72  import InvalidOr
-000003a0: 6465 720a 6672 6f6d 2063 6378 742e 6261  der.from ccxt.ba
-000003b0: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-000003c0: 204f 7264 6572 4e6f 7446 6f75 6e64 0a66   OrderNotFound.f
-000003d0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-000003e0: 726f 7273 2069 6d70 6f72 7420 4f72 6465  rors import Orde
-000003f0: 7249 6d6d 6564 6961 7465 6c79 4669 6c6c  rImmediatelyFill
-00000400: 6162 6c65 0a66 726f 6d20 6363 7874 2e62  able.from ccxt.b
-00000410: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
-00000420: 7420 4f72 6465 724e 6f74 4669 6c6c 6162  t OrderNotFillab
-00000430: 6c65 0a66 726f 6d20 6363 7874 2e62 6173  le.from ccxt.bas
-00000440: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
-00000450: 4e6f 7453 7570 706f 7274 6564 0a66 726f  NotSupported.fro
-00000460: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-00000470: 7273 2069 6d70 6f72 7420 4444 6f53 5072  rs import DDoSPr
-00000480: 6f74 6563 7469 6f6e 0a66 726f 6d20 6363  otection.from cc
-00000490: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
-000004a0: 6d70 6f72 7420 5261 7465 4c69 6d69 7445  mport RateLimitE
-000004b0: 7863 6565 6465 640a 6672 6f6d 2063 6378  xceeded.from ccx
-000004c0: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
-000004d0: 706f 7274 2045 7863 6861 6e67 654e 6f74  port ExchangeNot
-000004e0: 4176 6169 6c61 626c 650a 6672 6f6d 2063  Available.from c
-000004f0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-00000500: 696d 706f 7274 204f 6e4d 6169 6e74 656e  import OnMainten
-00000510: 616e 6365 0a66 726f 6d20 6363 7874 2e62  ance.from ccxt.b
-00000520: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
-00000530: 7420 496e 7661 6c69 644e 6f6e 6365 0a66  t InvalidNonce.f
-00000540: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-00000550: 726f 7273 2069 6d70 6f72 7420 5265 7175  rors import Requ
-00000560: 6573 7454 696d 656f 7574 0a66 726f 6d20  estTimeout.from 
-00000570: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-00000580: 2069 6d70 6f72 7420 4175 7468 656e 7469   import Authenti
-00000590: 6361 7469 6f6e 4572 726f 720a 6672 6f6d  cationError.from
+00000230: 7274 2041 7574 6865 6e74 6963 6174 696f  rt Authenticatio
+00000240: 6e45 7272 6f72 0a66 726f 6d20 6363 7874  nError.from ccxt
+00000250: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+00000260: 6f72 7420 5065 726d 6973 7369 6f6e 4465  ort PermissionDe
+00000270: 6e69 6564 0a66 726f 6d20 6363 7874 2e62  nied.from ccxt.b
+00000280: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+00000290: 7420 4163 636f 756e 7453 7573 7065 6e64  t AccountSuspend
+000002a0: 6564 0a66 726f 6d20 6363 7874 2e62 6173  ed.from ccxt.bas
+000002b0: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+000002c0: 4172 6775 6d65 6e74 7352 6571 7569 7265  ArgumentsRequire
+000002d0: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
+000002e0: 2e65 7272 6f72 7320 696d 706f 7274 2042  .errors import B
+000002f0: 6164 5265 7175 6573 740a 6672 6f6d 2063  adRequest.from c
+00000300: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+00000310: 696d 706f 7274 2042 6164 5379 6d62 6f6c  import BadSymbol
+00000320: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
+00000330: 6572 726f 7273 2069 6d70 6f72 7420 4d61  errors import Ma
+00000340: 7267 696e 4d6f 6465 416c 7265 6164 7953  rginModeAlreadyS
+00000350: 6574 0a66 726f 6d20 6363 7874 2e62 6173  et.from ccxt.bas
+00000360: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+00000370: 4261 6452 6573 706f 6e73 650a 6672 6f6d  BadResponse.from
+00000380: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+00000390: 7320 696d 706f 7274 2049 6e73 7566 6669  s import Insuffi
+000003a0: 6369 656e 7446 756e 6473 0a66 726f 6d20  cientFunds.from 
+000003b0: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
+000003c0: 2069 6d70 6f72 7420 496e 7661 6c69 644f   import InvalidO
+000003d0: 7264 6572 0a66 726f 6d20 6363 7874 2e62  rder.from ccxt.b
+000003e0: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+000003f0: 7420 4f72 6465 724e 6f74 466f 756e 640a  t OrderNotFound.
+00000400: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+00000410: 7272 6f72 7320 696d 706f 7274 204f 7264  rrors import Ord
+00000420: 6572 496d 6d65 6469 6174 656c 7946 696c  erImmediatelyFil
+00000430: 6c61 626c 650a 6672 6f6d 2063 6378 742e  lable.from ccxt.
+00000440: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
+00000450: 7274 204f 7264 6572 4e6f 7446 696c 6c61  rt OrderNotFilla
+00000460: 626c 650a 6672 6f6d 2063 6378 742e 6261  ble.from ccxt.ba
+00000470: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
+00000480: 204e 6f74 5375 7070 6f72 7465 640a 6672   NotSupported.fr
+00000490: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+000004a0: 6f72 7320 696d 706f 7274 2044 446f 5350  ors import DDoSP
+000004b0: 726f 7465 6374 696f 6e0a 6672 6f6d 2063  rotection.from c
+000004c0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+000004d0: 696d 706f 7274 2052 6174 654c 696d 6974  import RateLimit
+000004e0: 4578 6365 6564 6564 0a66 726f 6d20 6363  Exceeded.from cc
+000004f0: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
+00000500: 6d70 6f72 7420 4578 6368 616e 6765 4e6f  mport ExchangeNo
+00000510: 7441 7661 696c 6162 6c65 0a66 726f 6d20  tAvailable.from 
+00000520: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
+00000530: 2069 6d70 6f72 7420 4f6e 4d61 696e 7465   import OnMainte
+00000540: 6e61 6e63 650a 6672 6f6d 2063 6378 742e  nance.from ccxt.
+00000550: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
+00000560: 7274 2049 6e76 616c 6964 4e6f 6e63 650a  rt InvalidNonce.
+00000570: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+00000580: 7272 6f72 7320 696d 706f 7274 2052 6571  rrors import Req
+00000590: 7565 7374 5469 6d65 6f75 740a 6672 6f6d  uestTimeout.from
 000005a0: 2063 6378 742e 6261 7365 2e64 6563 696d   ccxt.base.decim
 000005b0: 616c 5f74 6f5f 7072 6563 6973 696f 6e20  al_to_precision 
 000005c0: 696d 706f 7274 2054 5255 4e43 4154 450a  import TRUNCATE.
 000005d0: 6672 6f6d 2063 6378 742e 6261 7365 2e64  from ccxt.base.d
 000005e0: 6563 696d 616c 5f74 6f5f 7072 6563 6973  ecimal_to_precis
 000005f0: 696f 6e20 696d 706f 7274 2044 4543 494d  ion import DECIM
 00000600: 414c 5f50 4c41 4345 530a 6672 6f6d 2063  AL_PLACES.from c
```

### Comparing `ccxt-4.2.94/ccxt/async_support/tradeogre.py` & `ccxt-4.2.95/ccxt/async_support/tradeogre.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.tradeogre import ImplicitAPI
 from ccxt.base.types import IndexType, Int, Market, Num, Order, OrderSide, OrderType, Str, Ticker
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class tradeogre(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(tradeogre, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/async_support/upbit.py` & `ccxt-4.2.95/ccxt/async_support/upbit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.upbit import ImplicitAPI
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
+from ccxt.base.errors import AddressPending
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
-from ccxt.base.errors import AuthenticationError
-from ccxt.base.errors import AddressPending
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class upbit(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/wavesexchange.py` & `ccxt-4.2.95/ccxt/async_support/wavesexchange.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from ccxt.abstract.wavesexchange import ImplicitAPI
 import asyncio
 import json
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from typing import Any
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import DuplicateOrderId
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.precise import Precise
 
 
 class wavesexchange(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/wazirx.py` & `ccxt-4.2.95/ccxt/async_support/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/whitebit.py` & `ccxt-4.2.95/ccxt/async_support/whitebit.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,44 +31,44 @@
 000001e0: 6573 2c20 5472 616e 7361 6374 696f 6e2c  es, Transaction,
 000001f0: 2054 7261 6e73 6665 7245 6e74 7279 0a66   TransferEntry.f
 00000200: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 00000210: 7420 4c69 7374 0a66 726f 6d20 6363 7874  t List.from ccxt
 00000220: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
 00000230: 6f72 7420 4578 6368 616e 6765 4572 726f  ort ExchangeErro
 00000240: 720a 6672 6f6d 2063 6378 742e 6261 7365  r.from ccxt.base
-00000250: 2e65 7272 6f72 7320 696d 706f 7274 2050  .errors import P
-00000260: 6572 6d69 7373 696f 6e44 656e 6965 640a  ermissionDenied.
-00000270: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-00000280: 7272 6f72 7320 696d 706f 7274 2041 7267  rrors import Arg
-00000290: 756d 656e 7473 5265 7175 6972 6564 0a66  umentsRequired.f
-000002a0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-000002b0: 726f 7273 2069 6d70 6f72 7420 4261 6452  rors import BadR
-000002c0: 6571 7565 7374 0a66 726f 6d20 6363 7874  equest.from ccxt
-000002d0: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-000002e0: 6f72 7420 4261 6453 796d 626f 6c0a 6672  ort BadSymbol.fr
-000002f0: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-00000300: 6f72 7320 696d 706f 7274 2049 6e73 7566  ors import Insuf
-00000310: 6669 6369 656e 7446 756e 6473 0a66 726f  ficientFunds.fro
-00000320: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-00000330: 7273 2069 6d70 6f72 7420 496e 7661 6c69  rs import Invali
-00000340: 644f 7264 6572 0a66 726f 6d20 6363 7874  dOrder.from ccxt
-00000350: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000360: 6f72 7420 4f72 6465 724e 6f74 466f 756e  ort OrderNotFoun
-00000370: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
-00000380: 2e65 7272 6f72 7320 696d 706f 7274 204e  .errors import N
-00000390: 6f74 5375 7070 6f72 7465 640a 6672 6f6d  otSupported.from
-000003a0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-000003b0: 7320 696d 706f 7274 2044 446f 5350 726f  s import DDoSPro
-000003c0: 7465 6374 696f 6e0a 6672 6f6d 2063 6378  tection.from ccx
-000003d0: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
-000003e0: 706f 7274 2045 7863 6861 6e67 654e 6f74  port ExchangeNot
-000003f0: 4176 6169 6c61 626c 650a 6672 6f6d 2063  Available.from c
-00000400: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-00000410: 696d 706f 7274 2041 7574 6865 6e74 6963  import Authentic
-00000420: 6174 696f 6e45 7272 6f72 0a66 726f 6d20  ationError.from 
+00000250: 2e65 7272 6f72 7320 696d 706f 7274 2041  .errors import A
+00000260: 7574 6865 6e74 6963 6174 696f 6e45 7272  uthenticationErr
+00000270: 6f72 0a66 726f 6d20 6363 7874 2e62 6173  or.from ccxt.bas
+00000280: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+00000290: 5065 726d 6973 7369 6f6e 4465 6e69 6564  PermissionDenied
+000002a0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
+000002b0: 6572 726f 7273 2069 6d70 6f72 7420 4172  errors import Ar
+000002c0: 6775 6d65 6e74 7352 6571 7569 7265 640a  gumentsRequired.
+000002d0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+000002e0: 7272 6f72 7320 696d 706f 7274 2042 6164  rrors import Bad
+000002f0: 5265 7175 6573 740a 6672 6f6d 2063 6378  Request.from ccx
+00000300: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+00000310: 706f 7274 2042 6164 5379 6d62 6f6c 0a66  port BadSymbol.f
+00000320: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+00000330: 726f 7273 2069 6d70 6f72 7420 496e 7375  rors import Insu
+00000340: 6666 6963 6965 6e74 4675 6e64 730a 6672  fficientFunds.fr
+00000350: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+00000360: 6f72 7320 696d 706f 7274 2049 6e76 616c  ors import Inval
+00000370: 6964 4f72 6465 720a 6672 6f6d 2063 6378  idOrder.from ccx
+00000380: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+00000390: 706f 7274 204f 7264 6572 4e6f 7446 6f75  port OrderNotFou
+000003a0: 6e64 0a66 726f 6d20 6363 7874 2e62 6173  nd.from ccxt.bas
+000003b0: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+000003c0: 4e6f 7453 7570 706f 7274 6564 0a66 726f  NotSupported.fro
+000003d0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+000003e0: 7273 2069 6d70 6f72 7420 4444 6f53 5072  rs import DDoSPr
+000003f0: 6f74 6563 7469 6f6e 0a66 726f 6d20 6363  otection.from cc
+00000400: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
+00000410: 6d70 6f72 7420 4578 6368 616e 6765 4e6f  mport ExchangeNo
+00000420: 7441 7661 696c 6162 6c65 0a66 726f 6d20  tAvailable.from 
 00000430: 6363 7874 2e62 6173 652e 6465 6369 6d61  ccxt.base.decima
 00000440: 6c5f 746f 5f70 7265 6369 7369 6f6e 2069  l_to_precision i
 00000450: 6d70 6f72 7420 5449 434b 5f53 495a 450a  mport TICK_SIZE.
 00000460: 6672 6f6d 2063 6378 742e 6261 7365 2e70  from ccxt.base.p
 00000470: 7265 6369 7365 2069 6d70 6f72 7420 5072  recise import Pr
 00000480: 6563 6973 650a 0a0a 636c 6173 7320 7768  ecise...class wh
 00000490: 6974 6562 6974 2845 7863 6861 6e67 652c  itebit(Exchange,
```

### Comparing `ccxt-4.2.94/ccxt/async_support/woo.py` & `ccxt-4.2.95/ccxt/async_support/woo.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.woo import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Bool, Conversion, Currencies, Currency, Int, Leverage, Market, MarketType, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class woo(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/yobit.py` & `ccxt-4.2.95/ccxt/async_support/yobit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.yobit import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class yobit(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/async_support/zaif.py` & `ccxt-4.2.95/ccxt/async_support/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/async_support/zonda.py` & `ccxt-4.2.95/ccxt/async_support/zonda.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.zonda import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import OrderImmediatelyFillable
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class zonda(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/base/__init__.py` & `ccxt-4.2.95/ccxt/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/base/decimal_to_precision.py` & `ccxt-4.2.95/ccxt/base/decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/base/errors.py` & `ccxt-4.2.95/ccxt/base/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,27 +30,27 @@
                 'OrderImmediatelyFillable': {},
                 'OrderNotFillable': {},
                 'DuplicateOrderId': {},
                 'ContractUnavailable': {},
             },
             'NotSupported': {},
             'ProxyError': {},
+            'ExchangeClosedByUser': {},
         },
         'OperationFailed': {
             'NetworkError': {
                 'DDoSProtection': {},
                 'RateLimitExceeded': {},
                 'ExchangeNotAvailable': {
                     'OnMaintenance': {},
                 },
                 'InvalidNonce': {},
                 'RequestTimeout': {},
             },
         },
-        'ExchangeClosedByUser': {},
     },
 }
 
 
 class BaseError(Exception):
     pass
 
@@ -155,14 +155,18 @@
     pass
 
 
 class ProxyError(ExchangeError):
     pass
 
 
+class ExchangeClosedByUser(ExchangeError):
+    pass
+
+
 class OperationFailed(BaseError):
     pass
 
 
 class NetworkError(OperationFailed):
     pass
 
@@ -187,18 +191,14 @@
     pass
 
 
 class RequestTimeout(NetworkError):
     pass
 
 
-class ExchangeClosedByUser(BaseError):
-    pass
-
-
 __all__ = [
     'error_hierarchy',
     'BaseError',
     'ExchangeError',
     'AuthenticationError',
     'PermissionDenied',
     'AccountNotEnabled',
@@ -220,17 +220,17 @@
     'CancelPending',
     'OrderImmediatelyFillable',
     'OrderNotFillable',
     'DuplicateOrderId',
     'ContractUnavailable',
     'NotSupported',
     'ProxyError',
+    'ExchangeClosedByUser',
     'OperationFailed',
     'NetworkError',
     'DDoSProtection',
     'RateLimitExceeded',
     'ExchangeNotAvailable',
     'OnMaintenance',
     'InvalidNonce',
-    'RequestTimeout',
-    'ExchangeClosedByUser'
+    'RequestTimeout'
 ]
```

### Comparing `ccxt-4.2.94/ccxt/base/exchange.py` & `ccxt-4.2.95/ccxt/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Base exchange class"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.2.94'
+__version__ = '4.2.95'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.base.errors import ExchangeError
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import AuthenticationError
```

### Comparing `ccxt-4.2.94/ccxt/base/precise.py` & `ccxt-4.2.95/ccxt/base/precise.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/base/types.py` & `ccxt-4.2.95/ccxt/base/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/bequant.py` & `ccxt-4.2.95/ccxt/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/bigone.py` & `ccxt-4.2.95/ccxt/bigone.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bigone import ImplicitAPI
 from ccxt.base.types import Balances, Bool, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bigone(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/binance.py` & `ccxt-4.2.95/ccxt/binance.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,72 +39,72 @@
 00000260: 2c20 5472 616e 7366 6572 456e 7472 790a  , TransferEntry.
 00000270: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
 00000280: 7274 204c 6973 740a 6672 6f6d 2063 6378  rt List.from ccx
 00000290: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
 000002a0: 706f 7274 2045 7863 6861 6e67 6545 7272  port ExchangeErr
 000002b0: 6f72 0a66 726f 6d20 6363 7874 2e62 6173  or.from ccxt.bas
 000002c0: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
-000002d0: 5065 726d 6973 7369 6f6e 4465 6e69 6564  PermissionDenied
-000002e0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-000002f0: 6572 726f 7273 2069 6d70 6f72 7420 4163  errors import Ac
-00000300: 636f 756e 7453 7573 7065 6e64 6564 0a66  countSuspended.f
-00000310: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-00000320: 726f 7273 2069 6d70 6f72 7420 4172 6775  rors import Argu
-00000330: 6d65 6e74 7352 6571 7569 7265 640a 6672  mentsRequired.fr
-00000340: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-00000350: 6f72 7320 696d 706f 7274 2042 6164 5265  ors import BadRe
-00000360: 7175 6573 740a 6672 6f6d 2063 6378 742e  quest.from ccxt.
-00000370: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-00000380: 7274 2042 6164 5379 6d62 6f6c 0a66 726f  rt BadSymbol.fro
-00000390: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-000003a0: 7273 2069 6d70 6f72 7420 4d61 7267 696e  rs import Margin
-000003b0: 4d6f 6465 416c 7265 6164 7953 6574 0a66  ModeAlreadySet.f
-000003c0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-000003d0: 726f 7273 2069 6d70 6f72 7420 4261 6452  rors import BadR
-000003e0: 6573 706f 6e73 650a 6672 6f6d 2063 6378  esponse.from ccx
-000003f0: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
-00000400: 706f 7274 2049 6e73 7566 6669 6369 656e  port Insufficien
-00000410: 7446 756e 6473 0a66 726f 6d20 6363 7874  tFunds.from ccxt
-00000420: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000430: 6f72 7420 496e 7661 6c69 644f 7264 6572  ort InvalidOrder
-00000440: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-00000450: 6572 726f 7273 2069 6d70 6f72 7420 4f72  errors import Or
-00000460: 6465 724e 6f74 466f 756e 640a 6672 6f6d  derNotFound.from
-00000470: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-00000480: 7320 696d 706f 7274 204f 7264 6572 496d  s import OrderIm
-00000490: 6d65 6469 6174 656c 7946 696c 6c61 626c  mediatelyFillabl
-000004a0: 650a 6672 6f6d 2063 6378 742e 6261 7365  e.from ccxt.base
-000004b0: 2e65 7272 6f72 7320 696d 706f 7274 204f  .errors import O
-000004c0: 7264 6572 4e6f 7446 696c 6c61 626c 650a  rderNotFillable.
-000004d0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-000004e0: 7272 6f72 7320 696d 706f 7274 204e 6f74  rrors import Not
-000004f0: 5375 7070 6f72 7465 640a 6672 6f6d 2063  Supported.from c
-00000500: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-00000510: 696d 706f 7274 2044 446f 5350 726f 7465  import DDoSProte
-00000520: 6374 696f 6e0a 6672 6f6d 2063 6378 742e  ction.from ccxt.
-00000530: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-00000540: 7274 2052 6174 654c 696d 6974 4578 6365  rt RateLimitExce
-00000550: 6564 6564 0a66 726f 6d20 6363 7874 2e62  eded.from ccxt.b
-00000560: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
-00000570: 7420 4f6e 4d61 696e 7465 6e61 6e63 650a  t OnMaintenance.
-00000580: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-00000590: 7272 6f72 7320 696d 706f 7274 2049 6e76  rrors import Inv
-000005a0: 616c 6964 4e6f 6e63 650a 6672 6f6d 2063  alidNonce.from c
-000005b0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-000005c0: 696d 706f 7274 2052 6571 7565 7374 5469  import RequestTi
-000005d0: 6d65 6f75 740a 6672 6f6d 2063 6378 742e  meout.from ccxt.
-000005e0: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-000005f0: 7274 2041 7574 6865 6e74 6963 6174 696f  rt Authenticatio
-00000600: 6e45 7272 6f72 0a66 726f 6d20 6363 7874  nError.from ccxt
-00000610: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000620: 6f72 7420 4f70 6572 6174 696f 6e52 656a  ort OperationRej
-00000630: 6563 7465 640a 6672 6f6d 2063 6378 742e  ected.from ccxt.
-00000640: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-00000650: 7274 204f 7065 7261 7469 6f6e 4661 696c  rt OperationFail
-00000660: 6564 0a66 726f 6d20 6363 7874 2e62 6173  ed.from ccxt.bas
+000002d0: 4175 7468 656e 7469 6361 7469 6f6e 4572  AuthenticationEr
+000002e0: 726f 720a 6672 6f6d 2063 6378 742e 6261  ror.from ccxt.ba
+000002f0: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
+00000300: 2050 6572 6d69 7373 696f 6e44 656e 6965   PermissionDenie
+00000310: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
+00000320: 2e65 7272 6f72 7320 696d 706f 7274 2041  .errors import A
+00000330: 6363 6f75 6e74 5375 7370 656e 6465 640a  ccountSuspended.
+00000340: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+00000350: 7272 6f72 7320 696d 706f 7274 2041 7267  rrors import Arg
+00000360: 756d 656e 7473 5265 7175 6972 6564 0a66  umentsRequired.f
+00000370: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+00000380: 726f 7273 2069 6d70 6f72 7420 4261 6452  rors import BadR
+00000390: 6571 7565 7374 0a66 726f 6d20 6363 7874  equest.from ccxt
+000003a0: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+000003b0: 6f72 7420 4261 6453 796d 626f 6c0a 6672  ort BadSymbol.fr
+000003c0: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+000003d0: 6f72 7320 696d 706f 7274 204f 7065 7261  ors import Opera
+000003e0: 7469 6f6e 5265 6a65 6374 6564 0a66 726f  tionRejected.fro
+000003f0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+00000400: 7273 2069 6d70 6f72 7420 4d61 7267 696e  rs import Margin
+00000410: 4d6f 6465 416c 7265 6164 7953 6574 0a66  ModeAlreadySet.f
+00000420: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+00000430: 726f 7273 2069 6d70 6f72 7420 4261 6452  rors import BadR
+00000440: 6573 706f 6e73 650a 6672 6f6d 2063 6378  esponse.from ccx
+00000450: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+00000460: 706f 7274 2049 6e73 7566 6669 6369 656e  port Insufficien
+00000470: 7446 756e 6473 0a66 726f 6d20 6363 7874  tFunds.from ccxt
+00000480: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+00000490: 6f72 7420 496e 7661 6c69 644f 7264 6572  ort InvalidOrder
+000004a0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
+000004b0: 6572 726f 7273 2069 6d70 6f72 7420 4f72  errors import Or
+000004c0: 6465 724e 6f74 466f 756e 640a 6672 6f6d  derNotFound.from
+000004d0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+000004e0: 7320 696d 706f 7274 204f 7264 6572 496d  s import OrderIm
+000004f0: 6d65 6469 6174 656c 7946 696c 6c61 626c  mediatelyFillabl
+00000500: 650a 6672 6f6d 2063 6378 742e 6261 7365  e.from ccxt.base
+00000510: 2e65 7272 6f72 7320 696d 706f 7274 204f  .errors import O
+00000520: 7264 6572 4e6f 7446 696c 6c61 626c 650a  rderNotFillable.
+00000530: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+00000540: 7272 6f72 7320 696d 706f 7274 204e 6f74  rrors import Not
+00000550: 5375 7070 6f72 7465 640a 6672 6f6d 2063  Supported.from c
+00000560: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+00000570: 696d 706f 7274 204f 7065 7261 7469 6f6e  import Operation
+00000580: 4661 696c 6564 0a66 726f 6d20 6363 7874  Failed.from ccxt
+00000590: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+000005a0: 6f72 7420 4444 6f53 5072 6f74 6563 7469  ort DDoSProtecti
+000005b0: 6f6e 0a66 726f 6d20 6363 7874 2e62 6173  on.from ccxt.bas
+000005c0: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+000005d0: 5261 7465 4c69 6d69 7445 7863 6565 6465  RateLimitExceede
+000005e0: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
+000005f0: 2e65 7272 6f72 7320 696d 706f 7274 204f  .errors import O
+00000600: 6e4d 6169 6e74 656e 616e 6365 0a66 726f  nMaintenance.fro
+00000610: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+00000620: 7273 2069 6d70 6f72 7420 496e 7661 6c69  rs import Invali
+00000630: 644e 6f6e 6365 0a66 726f 6d20 6363 7874  dNonce.from ccxt
+00000640: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+00000650: 6f72 7420 5265 7175 6573 7454 696d 656f  ort RequestTimeo
+00000660: 7574 0a66 726f 6d20 6363 7874 2e62 6173  ut.from ccxt.bas
 00000670: 652e 6465 6369 6d61 6c5f 746f 5f70 7265  e.decimal_to_pre
 00000680: 6369 7369 6f6e 2069 6d70 6f72 7420 5452  cision import TR
 00000690: 554e 4341 5445 0a66 726f 6d20 6363 7874  UNCATE.from ccxt
 000006a0: 2e62 6173 652e 6465 6369 6d61 6c5f 746f  .base.decimal_to
 000006b0: 5f70 7265 6369 7369 6f6e 2069 6d70 6f72  _precision impor
 000006c0: 7420 4445 4349 4d41 4c5f 504c 4143 4553  t DECIMAL_PLACES
 000006d0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
```

### Comparing `ccxt-4.2.94/ccxt/binancecoinm.py` & `ccxt-4.2.95/ccxt/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/binanceus.py` & `ccxt-4.2.95/ccxt/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/binanceusdm.py` & `ccxt-4.2.95/ccxt/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/bingx.py` & `ccxt-4.2.95/ccxt/bingx.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bingx import ImplicitAPI
 import hashlib
 import numbers
 from ccxt.base.types import Balances, Currencies, Currency, Int, Leverage, MarginMode, MarginModification, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Position, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.precise import Precise
 
 
 class bingx(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/bit2c.py` & `ccxt-4.2.95/ccxt/bit2c.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bit2c import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Ticker, Trade, TradingFees
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bit2c(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/bitbank.py` & `ccxt-4.2.95/ccxt/bitbank.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bitbank import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Ticker, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class bitbank(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(bitbank, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/bitbns.py` & `ccxt-4.2.95/ccxt/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/bitfinex.py` & `ccxt-4.2.95/ccxt/bitfinex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bitfinex import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import ROUND
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.decimal_to_precision import SIGNIFICANT_DIGITS
 from ccxt.base.precise import Precise
```

### Comparing `ccxt-4.2.94/ccxt/bitfinex2.py` & `ccxt-4.2.95/ccxt/bitfinex2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bitfinex2 import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, MarginModification, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import ROUND
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.decimal_to_precision import SIGNIFICANT_DIGITS
 from ccxt.base.precise import Precise
```

### Comparing `ccxt-4.2.94/ccxt/bitflyer.py` & `ccxt-4.2.95/ccxt/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/bitget.py` & `ccxt-4.2.95/ccxt/bitget.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bitget import ImplicitAPI
 import hashlib
 import json
 from ccxt.base.types import Balances, Conversion, Currencies, Currency, FundingHistory, Int, Liquidation, Leverage, MarginMode, MarginModification, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Position, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
@@ -23,15 +24,14 @@
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitget(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/bithumb.py` & `ccxt-4.2.95/ccxt/bithumb.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bithumb import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, MarketInterface, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.decimal_to_precision import SIGNIFICANT_DIGITS
 from ccxt.base.precise import Precise
 
 
 class bithumb(Exchange, ImplicitAPI):
```

### Comparing `ccxt-4.2.94/ccxt/bitmart.py` & `ccxt-4.2.95/ccxt/bitmart.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bitmart import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
@@ -20,15 +21,14 @@
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitmart(Exchange, ImplicitAPI):
```

### Comparing `ccxt-4.2.94/ccxt/bitmex.py` & `ccxt-4.2.95/ccxt/bitmex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bitmex import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Leverage, Leverages, Market, MarketType, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitmex(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/bitopro.py` & `ccxt-4.2.95/ccxt/bitopro.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bitopro import ImplicitAPI
 import hashlib
 import math
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitopro(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/bitrue.py` & `ccxt-4.2.95/ccxt/bitrue.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bitrue import ImplicitAPI
 import hashlib
 import json
 from ccxt.base.types import Balances, Currencies, Currency, Int, MarginModification, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
@@ -21,15 +22,14 @@
 from ccxt.base.errors import OrderImmediatelyFillable
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitrue(Exchange, ImplicitAPI):
```

### Comparing `ccxt-4.2.94/ccxt/bitso.py` & `ccxt-4.2.95/ccxt/bitso.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bitso import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitso(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/bitstamp.py` & `ccxt-4.2.95/ccxt/bitstamp.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bitstamp import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bitstamp(Exchange, ImplicitAPI):
 
     def describe(self):
@@ -366,14 +366,20 @@
                         'lmwr_address/': 1,
                         'pepe_withdrawal/': 1,
                         'pepe_address/': 1,
                         'blur_withdrawal/': 1,
                         'blur_address/': 1,
                         'vext_withdrawal/': 1,
                         'vext_address/': 1,
+                        'cspr_withdrawal/': 1,
+                        'cspr_address/': 1,
+                        'vchf_withdrawal/': 1,
+                        'vchf_address/': 1,
+                        'veur_withdrawal/': 1,
+                        'veur_address/': 1,
                     },
                 },
             },
             'fees': {
                 'trading': {
                     'tierBased': True,
                     'percentage': True,
```

### Comparing `ccxt-4.2.94/ccxt/bitteam.py` & `ccxt-4.2.95/ccxt/bitteam.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bitteam import ImplicitAPI
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.precise import Precise
 
 
 class bitteam(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/bitvavo.py` & `ccxt-4.2.95/ccxt/bitvavo.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bitvavo import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import ROUND
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.decimal_to_precision import SIGNIFICANT_DIGITS
 from ccxt.base.precise import Precise
```

### Comparing `ccxt-4.2.94/ccxt/bl3p.py` & `ccxt-4.2.95/ccxt/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/blockchaincom.py` & `ccxt-4.2.95/ccxt/blockchaincom.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.blockchaincom import ImplicitAPI
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import OrderNotFound
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class blockchaincom(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/blofin.py` & `ccxt-4.2.95/ccxt/blofin.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.blofin import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Leverage, Leverages, MarginMode, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Position, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class blofin(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/btcalpha.py` & `ccxt-4.2.95/ccxt/btcalpha.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.btcalpha import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, IndexType, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import DDoSProtection
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class btcalpha(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/btcbox.py` & `ccxt-4.2.95/ccxt/btcbox.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.btcbox import ImplicitAPI
 import hashlib
 import json
 from ccxt.base.types import Balances, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Ticker, Trade
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class btcbox(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/btcmarkets.py` & `ccxt-4.2.95/ccxt/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/btcturk.py` & `ccxt-4.2.95/ccxt/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/bybit.py` & `ccxt-4.2.95/ccxt/bybit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.bybit import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Greeks, Int, Leverage, Market, MarketInterface, Num, Option, OptionChain, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
+from ccxt.base.errors import NoChange
 from ccxt.base.errors import MarginModeAlreadySet
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import InvalidNonce
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
-from ccxt.base.errors import NoChange
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class bybit(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/cex.py` & `ccxt-4.2.95/ccxt/cex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.cex import ImplicitAPI
 import hashlib
 import json
 from ccxt.base.types import Balances, Currencies, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import NullResponse
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class cex(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/coinbase.py` & `ccxt-4.2.95/ccxt/coinbase.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.coinbase import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinbase(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/coinbaseinternational.py` & `ccxt-4.2.95/ccxt/coinbaseinternational.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.coinbaseinternational import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Order, OrderSide, OrderType, Position, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
 from typing import Any
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import DuplicateOrderId
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinbaseinternational(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/coinbasepro.py` & `ccxt-4.2.95/ccxt/coinbasepro.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.coinbasepro import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinbasepro(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/coincheck.py` & `ccxt-4.2.95/ccxt/coincheck.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.coincheck import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Ticker, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
-from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import BadSymbol
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class coincheck(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(coincheck, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/coinex.py` & `ccxt-4.2.95/ccxt/coinex.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.coinex import ImplicitAPI
 from ccxt.base.types import Balances, Currencies, Currency, Int, Leverage, Leverages, MarginModification, Market, Num, Order, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinex(Exchange, ImplicitAPI):
 
     def describe(self):
@@ -1071,83 +1071,89 @@
         #
         data = self.safe_dict(response, 'data', {})
         return self.safe_integer(data, 'timestamp')
 
     def fetch_order_book(self, symbol: str, limit: Int = 20, params={}):
         """
         fetches information on open orders with bid(buy) and ask(sell) prices, volumes and other data
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot001_market004_market_depth
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http010_market_depth
+        :see: https://docs.coinex.com/api/v2/spot/market/http/list-market-depth
+        :see: https://docs.coinex.com/api/v2/futures/market/http/list-market-depth
         :param str symbol: unified symbol of the market to fetch the order book for
         :param int [limit]: the maximum amount of order book entries to return
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: A dictionary of `order book structures <https://docs.ccxt.com/#/?id=order-book-structure>` indexed by market symbols
         """
         self.load_markets()
         market = self.market(symbol)
         if limit is None:
             limit = 20  # default
         request = {
-            'market': self.market_id(symbol),
-            'merge': '0',
-            'limit': str(limit),
+            'market': market['id'],
+            'limit': limit,
+            'interval': '0',
         }
         response = None
         if market['swap']:
-            response = self.v1PerpetualPublicGetMarketDepth(self.extend(request, params))
+            response = self.v2PublicGetFuturesDepth(self.extend(request, params))
+            #
+            #     {
+            #         "code": 0,
+            #         "data": {
+            #             "depth": {
+            #                 "asks": [
+            #                     ["70851.94", "0.2119"],
+            #                     ["70851.95", "0.0004"],
+            #                     ["70851.96", "0.0004"]
+            #                 ],
+            #                 "bids": [
+            #                     ["70851.93", "1.0314"],
+            #                     ["70850.93", "0.0021"],
+            #                     ["70850.42", "0.0306"]
+            #                 ],
+            #                 "checksum": 2956436260,
+            #                 "last": "70851.94",
+            #                 "updated_at": 1712824003252
+            #             },
+            #             "is_full": True,
+            #             "market": "BTCUSDT"
+            #         },
+            #         "message": "OK"
+            #     }
+            #
         else:
-            response = self.v1PublicGetMarketDepth(self.extend(request, params))
-        #
-        # Spot
-        #
-        #     {
-        #         "code": 0,
-        #         "data": {
-        #             "asks": [
-        #                 ["41056.33", "0.31727613"],
-        #                 ["41056.34", "1.05657294"],
-        #                 ["41056.35", "0.02346648"]
-        #             ],
-        #             "bids": [
-        #                 ["41050.61", "0.40618608"],
-        #                 ["41046.98", "0.13800000"],
-        #                 ["41046.56", "0.22579234"]
-        #             ],
-        #             "last": "41050.61",
-        #             "time": 1650573220346
-        #         },
-        #         "message": "OK"
-        #     }
-        #
-        # Swap
-        #
-        #     {
-        #         "code": 0,
-        #         "data": {
-        #             "asks": [
-        #                 ["40620.90", "0.0384"],
-        #                 ["40625.50", "0.0219"],
-        #                 ["40625.90", "0.3506"]
-        #             ],
-        #             "bids": [
-        #                 ["40620.89", "19.6861"],
-        #                 ["40620.80", "0.0012"],
-        #                 ["40619.87", "0.0365"]
-        #             ],
-        #             "last": "40620.89",
-        #             "time": 1650587672406,
-        #             "sign_price": "40619.32",
-        #             "index_price": "40609.93"
-        #         },
-        #         "message": "OK"
-        #     }
-        #
-        result = self.safe_value(response, 'data', {})
-        timestamp = self.safe_integer(result, 'time')
-        return self.parse_order_book(result, symbol, timestamp)
+            response = self.v2PublicGetSpotDepth(self.extend(request, params))
+            #
+            #     {
+            #         "code": 0,
+            #         "data": {
+            #             "depth": {
+            #                 "asks": [
+            #                     ["70875.31", "0.28670282"],
+            #                     ["70875.32", "0.31008114"],
+            #                     ["70875.42", "0.05876653"]
+            #                 ],
+            #                 "bids": [
+            #                     ["70855.3", "0.00632222"],
+            #                     ["70855.29", "0.36216834"],
+            #                     ["70855.17", "0.10166802"]
+            #                 ],
+            #                 "checksum": 2313816665,
+            #                 "last": "70857.19",
+            #                 "updated_at": 1712823790987
+            #             },
+            #             "is_full": True,
+            #             "market": "BTCUSDT"
+            #         },
+            #         "message": "OK"
+            #     }
+            #
+        data = self.safe_dict(response, 'data', {})
+        depth = self.safe_dict(data, 'depth', {})
+        timestamp = self.safe_integer(depth, 'updated_at')
+        return self.parse_order_book(depth, symbol, timestamp)
 
     def parse_trade(self, trade, market: Market = None) -> Trade:
         #
         # Spot and Swap fetchTrades(public)
         #
         #      {
         #          "id":  2611511379,
```

### Comparing `ccxt-4.2.94/ccxt/coinlist.py` & `ccxt-4.2.95/ccxt/coinlist.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.coinlist import ImplicitAPI
 import hashlib
 import math
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinlist(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/coinmate.py` & `ccxt-4.2.95/ccxt/coinmate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.coinmate import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import RateLimitExceeded
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinmate(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/coinmetro.py` & `ccxt-4.2.95/ccxt/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/coinone.py` & `ccxt-4.2.95/ccxt/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/coinsph.py` & `ccxt-4.2.95/ccxt/coinsph.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.coinsph import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import BadResponse
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import OrderImmediatelyFillable
 from ccxt.base.errors import DuplicateOrderId
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class coinsph(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/coinspot.py` & `ccxt-4.2.95/ccxt/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/cryptocom.py` & `ccxt-4.2.95/ccxt/cryptocom.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.cryptocom import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currency, Int, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountNotEnabled
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class cryptocom(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/currencycom.py` & `ccxt-4.2.95/ccxt/currencycom.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.currencycom import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Leverage, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class currencycom(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/delta.py` & `ccxt-4.2.95/ccxt/delta.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.delta import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Greeks, Int, Leverage, MarginMode, MarginModification, Market, MarketInterface, Num, Option, Order, OrderBook, OrderSide, OrderType, Position, Str, Strings, Ticker, Tickers, Trade
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class delta(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/deribit.py` & `ccxt-4.2.95/ccxt/deribit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.deribit import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, Greeks, Int, Market, MarketInterface, Num, Option, OptionChain, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class deribit(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/digifinex.py` & `ccxt-4.2.95/ccxt/digifinex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.digifinex import ImplicitAPI
 import hashlib
 import json
 from ccxt.base.types import Balances, Currencies, Currency, Int, MarginModification, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import BadResponse
 from ccxt.base.errors import InsufficientFunds
@@ -21,15 +22,14 @@
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class digifinex(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/exmo.py` & `ccxt-4.2.95/ccxt/exmo.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.exmo import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, MarginModification, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class exmo(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/flowbtc.py` & `ccxt-4.2.95/ccxt/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/fmfwio.py` & `ccxt-4.2.95/ccxt/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/gate.py` & `ccxt-4.2.95/ccxt/gate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.gate import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, FundingHistory, Greeks, Int, Leverage, Leverages, MarginModification, Market, MarketInterface, Num, Option, OptionChain, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountNotEnabled
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import BadResponse
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import OrderImmediatelyFillable
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class gate(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/gemini.py` & `ccxt-4.2.95/ccxt/gemini.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.gemini import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class gemini(Exchange, ImplicitAPI):
 
     def describe(self):
@@ -661,15 +661,16 @@
             marketIdUpper = marketId.upper()
             isPerp = (marketIdUpper.find('PERP') >= 0)
             marketIdWithoutPerp = marketIdUpper.replace('PERP', '')
             quoteQurrencies = self.handle_option('fetchMarketsFromAPI', 'quoteCurrencies', [])
             for i in range(0, len(quoteQurrencies)):
                 quoteCurrency = quoteQurrencies[i]
                 if marketIdWithoutPerp.endswith(quoteCurrency):
-                    baseId = marketIdWithoutPerp.replace(quoteCurrency, '')
+                    quoteLength = self.parse_to_int(-1 * len(quoteCurrency))
+                    baseId = marketIdWithoutPerp[0:quoteLength]
                     quoteId = quoteCurrency
                     if isPerp:
                         settleId = quoteCurrency  # always same
                     break
         base = self.safe_currency_code(baseId)
         quote = self.safe_currency_code(quoteId)
         settle = self.safe_currency_code(settleId)
```

### Comparing `ccxt-4.2.94/ccxt/hitbtc.py` & `ccxt-4.2.95/ccxt/hitbtc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.hitbtc import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Leverage, MarginMode, MarginModes, MarginModification, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class hitbtc(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/hollaex.py` & `ccxt-4.2.95/ccxt/hollaex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.hollaex import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import OrderImmediatelyFillable
 from ccxt.base.errors import NetworkError
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class hollaex(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/htx.py` & `ccxt-4.2.95/ccxt/htx.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.htx import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountNotEnabled
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
-from ccxt.base.errors import NetworkError
+from ccxt.base.errors import OperationFailed
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class htx(Exchange, ImplicitAPI):
 
@@ -954,22 +954,16 @@
                 },
             },
             'precisionMode': TICK_SIZE,
             'options': {
                 'fetchMarkets': {
                     'types': {
                         'spot': True,
-                        'future': {
-                            'linear': True,
-                            'inverse': True,
-                        },
-                        'swap': {
-                            'linear': True,
-                            'inverse': True,
-                        },
+                        'linear': True,
+                        'inverse': True,
                     },
                 },
                 'fetchOHLCV': {
                     'useHistoricalEndpointForSpot': True,
                 },
                 'withdraw': {
                     'includeFee': False,
@@ -1605,60 +1599,49 @@
 
     def fetch_markets(self, params={}) -> List[Market]:
         """
         retrieves data on all markets for huobi
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: an array of objects representing market data
         """
-        options = self.safe_value(self.options, 'fetchMarkets', {})
-        types = self.safe_value(options, 'types', {})
+        types = None
+        types, params = self.handle_option_and_params(params, 'fetchMarkets', 'types', {})
         allMarkets = []
         promises = []
         keys = list(types.keys())
         for i in range(0, len(keys)):
-            type = keys[i]
-            value = self.safe_value(types, type)
-            if value is True:
-                promises.append(self.fetch_markets_by_type_and_sub_type(type, None, params))
-            elif value:
-                subKeys = list(value.keys())
-                for j in range(0, len(subKeys)):
-                    subType = subKeys[j]
-                    subValue = self.safe_value(value, subType)
-                    if subValue:
-                        promises.append(self.fetch_markets_by_type_and_sub_type(type, subType, params))
+            key = keys[i]
+            if self.safe_bool(types, key):
+                if key == 'spot':
+                    promises.append(self.fetch_markets_by_type_and_sub_type('spot', None, params))
+                elif key == 'linear':
+                    promises.append(self.fetch_markets_by_type_and_sub_type(None, 'linear', params))
+                elif key == 'inverse':
+                    promises.append(self.fetch_markets_by_type_and_sub_type('swap', 'inverse', params))
+                    promises.append(self.fetch_markets_by_type_and_sub_type('future', 'inverse', params))
         promises = promises
         for i in range(0, len(promises)):
             allMarkets = self.array_concat(allMarkets, promises[i])
         return allMarkets
 
     def fetch_markets_by_type_and_sub_type(self, type, subType, params={}):
-        query = self.omit(params, ['type', 'subType'])
-        spot = (type == 'spot')
-        contract = (type != 'spot')
-        future = (type == 'future')
-        swap = (type == 'swap')
-        linear = None
-        inverse = None
+        isSpot = (type == 'spot')
         request = {}
         response = None
-        if contract:
-            linear = (subType == 'linear')
-            inverse = (subType == 'inverse')
-            if linear:
-                if future:
-                    request['business_type'] = 'futures'
-                response = self.contractPublicGetLinearSwapApiV1SwapContractInfo(self.extend(request, query))
-            elif inverse:
-                if future:
-                    response = self.contractPublicGetApiV1ContractContractInfo(self.extend(request, query))
-                elif swap:
-                    response = self.contractPublicGetSwapApiV1SwapContractInfo(self.extend(request, query))
+        if not isSpot:
+            if subType == 'linear':
+                request['business_type'] = 'all'  # override default to fetch all linear markets
+                response = self.contractPublicGetLinearSwapApiV1SwapContractInfo(self.extend(request, params))
+            elif subType == 'inverse':
+                if type == 'future':
+                    response = self.contractPublicGetApiV1ContractContractInfo(self.extend(request, params))
+                elif type == 'swap':
+                    response = self.contractPublicGetSwapApiV1SwapContractInfo(self.extend(request, params))
         else:
-            response = self.spotPublicGetV1CommonSymbols(self.extend(request, query))
+            response = self.spotPublicGetV1CommonSymbols(self.extend(request, params))
         #
         # spot
         #
         #     {
         #         "status":"ok",
         #         "data":[
         #             {
@@ -1689,110 +1672,109 @@
         #                 "init-nav":10.000000000000000000,
         #                 "api-trading":"enabled",
         #                 "tags":"etp,nav,holdinglimit"
         #             },
         #         ]
         #     }
         #
-        # inverse future
+        # inverse(swap & future)
         #
         #     {
         #         "status":"ok",
         #         "data":[
         #             {
         #                 "symbol":"BTC",
-        #                 "contract_code":"BTC211126",
-        #                 "contract_type":"self_week",
-        #                 "contract_size":100.000000000000000000,
-        #                 "price_tick":0.010000000000000000,
-        #                 "delivery_date":"20211126",
-        #                 "delivery_time":"1637913600000",
+        #                 "contract_code":"BTC211126",  #/ BTC-USD in swap
+        #                 "contract_type":"self_week",  # only in future
+        #                 "contract_size":100,
+        #                 "price_tick":0.1,
+        #                 "delivery_date":"20211126",  # only in future
+        #                 "delivery_time":"1637913600000",  # empty in swap
         #                 "create_date":"20211112",
         #                 "contract_status":1,
-        #                 "settlement_time":"1637481600000"
+        #                 "settlement_time":"1637481600000"  # only in future
+        #                 "settlement_date":"16xxxxxxxxxxx"  # only in swap
         #             },
+        #           ...
         #         ],
         #         "ts":1637474595140
         #     }
         #
-        # linear futures
+        # linear(swap & future)
         #
         #     {
         #         "status":"ok",
         #         "data":[
         #             {
         #                 "symbol":"BTC",
-        #                 "contract_code":"BTC-USDT-211231",
-        #                 "contract_size":0.001000000000000000,
-        #                 "price_tick":0.100000000000000000,
-        #                 "delivery_date":"20211231",
-        #                 "delivery_time":"1640937600000",
+        #                 "contract_code":"BTC-USDT-211231",  # or "BTC-USDT" in swap
+        #                 "contract_size":0.001,
+        #                 "price_tick":0.1,
+        #                 "delivery_date":"20211231",  # empty in swap
+        #                 "delivery_time":"1640937600000",  # empty in swap
         #                 "create_date":"20211228",
         #                 "contract_status":1,
         #                 "settlement_date":"1640764800000",
-        #                 "support_margin_mode":"cross",
-        #                 "business_type":"futures",
+        #                 "support_margin_mode":"cross",  # "all" or "cross"
+        #                 "business_type":"futures",  # "swap" or "futures"
         #                 "pair":"BTC-USDT",
-        #                 "contract_type":"self_week"  # next_week, quarter
-        #             },
+        #                 "contract_type":"self_week",  # "swap", "self_week", "next_week", "quarter"
+        #                 "trade_partition":"USDT",
+        #             }
         #         ],
         #         "ts":1640736207263
         #     }
         #
-        # swaps
-        #
-        #     {
-        #         "status":"ok",
-        #         "data":[
-        #             {
-        #                 "symbol":"BTC",
-        #                 "contract_code":"BTC-USDT",
-        #                 "contract_size":0.001000000000000000,
-        #                 "price_tick":0.100000000000000000,
-        #                 "delivery_time":"",
-        #                 "create_date":"20201021",
-        #                 "contract_status":1,
-        #                 "settlement_date":"1637481600000",
-        #                 "support_margin_mode":"all",  # isolated
-        #             },
-        #         ],
-        #         "ts":1637474774467
-        #     }
-        #
-        markets = self.safe_value(response, 'data', [])
+        markets = self.safe_list(response, 'data', [])
         numMarkets = len(markets)
         if numMarkets < 1:
-            raise NetworkError(self.id + ' fetchMarkets() returned an empty response: ' + self.json(markets))
+            raise OperationFailed(self.id + ' fetchMarkets() returned an empty response: ' + self.json(response))
         result = []
         for i in range(0, len(markets)):
             market = markets[i]
             baseId = None
             quoteId = None
             settleId = None
             id = None
             lowercaseId = None
+            contract = ('contract_code' in market)
+            spot = not contract
+            swap = False
+            future = False
+            linear = None
+            inverse = None
+            # check if parsed market is contract
             if contract:
                 id = self.safe_string(market, 'contract_code')
                 lowercaseId = id.lower()
+                delivery_date = self.safe_string(market, 'delivery_date')
+                business_type = self.safe_string(market, 'business_type')
+                future = delivery_date is not None
+                swap = not future
+                linear = business_type is not None
+                inverse = not linear
                 if swap:
+                    type = 'swap'
                     parts = id.split('-')
                     baseId = self.safe_string_lower(market, 'symbol')
                     quoteId = self.safe_string_lower(parts, 1)
                     settleId = baseId if inverse else quoteId
                 elif future:
+                    type = 'future'
                     baseId = self.safe_string_lower(market, 'symbol')
                     if inverse:
                         quoteId = 'USD'
                         settleId = baseId
                     else:
                         pair = self.safe_string(market, 'pair')
                         parts = pair.split('-')
                         quoteId = self.safe_string_lower(parts, 1)
                         settleId = quoteId
             else:
+                type = 'spot'
                 baseId = self.safe_string(market, 'base-currency')
                 quoteId = self.safe_string(market, 'quote-currency')
                 id = baseId + quoteId
                 lowercaseId = id.lower()
             base = self.safe_currency_code(baseId)
             quote = self.safe_currency_code(quoteId)
             settle = self.safe_currency_code(settleId)
@@ -1907,14 +1889,48 @@
                     },
                 },
                 'created': created,
                 'info': market,
             })
         return result
 
+    def try_get_symbol_from_future_markets(self, symbolOrMarketId: str):
+        if symbolOrMarketId in self.markets:
+            return symbolOrMarketId
+        # only on "future" market type(inverse & linear), market-id differs between "fetchMarkets" and "fetchTicker"
+        # so we have to create a mapping
+        # - market-id from fetchMarkts:    `BTC-USDT-240419`(linear future) or `BTC240412`(inverse future)
+        # - market-id from fetchTciker[s]: `BTC-USDT-CW`     (linear future) or `BTC_CW`    (inverse future)
+        if not ('futureMarketIdsForSymbols' in self.options):
+            self.options['futureMarketIdsForSymbols'] = {}
+        futureMarketIdsForSymbols = self.safe_dict(self.options, 'futureMarketIdsForSymbols', {})
+        if symbolOrMarketId in futureMarketIdsForSymbols:
+            return futureMarketIdsForSymbols[symbolOrMarketId]
+        futureMarkets = self.filter_by(self.markets, 'future', True)
+        futuresCharsMaps = {
+            'this_week': 'CW',
+            'next_week': 'NW',
+            'quarter': 'CQ',
+            'next_quarter': 'NQ',
+        }
+        for i in range(0, len(futureMarkets)):
+            market = futureMarkets[i]
+            info = self.safe_value(market, 'info', {})
+            contractType = self.safe_string(info, 'contract_type')
+            contractSuffix = futuresCharsMaps[contractType]
+            # see comment on formats a bit above
+            constructedId = market['base'] + '-' + market['quote'] + '-' + contractSuffix if market['linear'] else market['base'] + '_' + contractSuffix
+            if constructedId == symbolOrMarketId:
+                symbol = market['symbol']
+                self.options['futureMarketIdsForSymbols'][symbolOrMarketId] = symbol
+                return symbol
+        # if not found, just save it to avoid unnecessary future iterations
+        self.options['futureMarketIdsForSymbols'][symbolOrMarketId] = symbolOrMarketId
+        return symbolOrMarketId
+
     def parse_ticker(self, ticker, market: Market = None) -> Ticker:
         #
         # fetchTicker
         #
         #     {
         #         "amount": 26228.672978342216,
         #         "open": 9078.95,
@@ -1955,14 +1971,15 @@
         #         "bidSize": 1.685945,
         #         "quoteTime": 1671941599612,
         #         "symbol": "btcusdt"
         #     }
         #
         marketId = self.safe_string_2(ticker, 'symbol', 'contract_code')
         symbol = self.safe_symbol(marketId, market)
+        symbol = self.try_get_symbol_from_future_markets(symbol)
         timestamp = self.safe_integer_2(ticker, 'ts', 'quoteTime')
         bid = None
         bidVolume = None
         ask = None
         askVolume = None
         if 'bid' in ticker:
             if isinstance(ticker['bid'], list):
@@ -2082,45 +2099,55 @@
     def fetch_tickers(self, symbols: Strings = None, params={}) -> Tickers:
         """
         fetches price tickers for multiple markets, statistical information calculated over the past 24 hours for each market
         :see: https://huobiapi.github.io/docs/spot/v1/en/#get-latest-tickers-for-all-pairs
         :see: https://huobiapi.github.io/docs/usdt_swap/v1/en/#general-get-a-batch-of-market-data-overview
         :see: https://huobiapi.github.io/docs/dm/v1/en/#get-a-batch-of-market-data-overview
         :see: https://huobiapi.github.io/docs/coin_margined_swap/v1/en/#get-a-batch-of-market-data-overview-v2
-        :param str[]|None symbols: unified symbols of the markets to fetch the ticker for, all market tickers are returned if not assigned
+        :param str[] [symbols]: unified symbols of the markets to fetch the ticker for, all market tickers are returned if not assigned
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a dictionary of `ticker structures <https://docs.ccxt.com/#/?id=ticker-structure>`
         """
         self.load_markets()
         symbols = self.market_symbols(symbols)
         first = self.safe_string(symbols, 0)
         market = None
         if first is not None:
             market = self.market(first)
+        isSubTypeRequested = ('subType' in params) or ('business_type' in params)
         type = None
         subType = None
         type, params = self.handle_market_type_and_params('fetchTickers', market, params)
         subType, params = self.handle_sub_type_and_params('fetchTickers', market, params)
         request = {}
+        isSpot = (type == 'spot')
         future = (type == 'future')
         swap = (type == 'swap')
         linear = (subType == 'linear')
         inverse = (subType == 'inverse')
-        params = self.omit(params, ['type', 'subType'])
         response = None
-        if future or swap:
+        if not isSpot or isSubTypeRequested:
             if linear:
+                # independently of type, supports calling all linear symbols i.e. fetchTickers(None, {subType:'linear'})
                 if future:
                     request['business_type'] = 'futures'
+                elif swap:
+                    request['business_type'] = 'swap'
+                else:
+                    request['business_type'] = 'all'
                 response = self.contractPublicGetLinearSwapExMarketDetailBatchMerged(self.extend(request, params))
             elif inverse:
                 if future:
                     response = self.contractPublicGetMarketDetailBatchMerged(self.extend(request, params))
                 elif swap:
                     response = self.contractPublicGetSwapExMarketDetailBatchMerged(self.extend(request, params))
+                else:
+                    raise NotSupported(self.id + ' fetchTickers() you have to set params["type"] to either "swap" or "future" for inverse contracts')
+            else:
+                raise NotSupported(self.id + ' fetchTickers() you have to set params["subType"] to either "linear" or "inverse" for contracts')
         else:
             response = self.spotPublicGetMarketTickers(self.extend(request, params))
         #
         # spot
         #
         #     {
         #         "data":[
@@ -2165,51 +2192,25 @@
         #                 "business_type":"futures",  # only in linear futures
         #                 "contract_code":"BTC-USDT-CW",  # only in linear futures, instead of 'symbol'
         #             }
         #         ],
         #         "ts":1637504679376
         #     }
         #
-        tickers = self.safe_value_2(response, 'data', 'ticks', [])
-        timestamp = self.safe_integer(response, 'ts')
-        result = {}
-        for i in range(0, len(tickers)):
-            ticker = self.parse_ticker(tickers[i])
-            # the market ids for linear futures are non-standard and differ from all the other endpoints
-            # we are doing a linear-matching here
-            if future and linear:
-                for j in range(0, len(self.symbols)):
-                    symbolInner = self.symbols[j]
-                    marketInner = self.market(symbolInner)
-                    contractType = self.safe_string(marketInner['info'], 'contract_type')
-                    if (contractType == 'this_week') and (ticker['symbol'] == (marketInner['baseId'] + '-' + marketInner['quoteId'] + '-CW')):
-                        ticker['symbol'] = marketInner['symbol']
-                        break
-                    elif (contractType == 'next_week') and (ticker['symbol'] == (marketInner['baseId'] + '-' + marketInner['quoteId'] + '-NW')):
-                        ticker['symbol'] = marketInner['symbol']
-                        break
-                    elif (contractType == 'this_quarter') and (ticker['symbol'] == (marketInner['baseId'] + '-' + marketInner['quoteId'] + '-CQ')):
-                        ticker['symbol'] = marketInner['symbol']
-                        break
-                    elif (contractType == 'next_quarter') and (ticker['symbol'] == (marketInner['baseId'] + '-' + marketInner['quoteId'] + '-NQ')):
-                        ticker['symbol'] = marketInner['symbol']
-                        break
-            symbol = ticker['symbol']
-            ticker['timestamp'] = timestamp
-            ticker['datetime'] = self.iso8601(timestamp)
-            result[symbol] = ticker
-        return self.filter_by_array_tickers(result, 'symbol', symbols)
+        rawTickers = self.safe_list_2(response, 'data', 'ticks', [])
+        tickers = self.parse_tickers(rawTickers, symbols, params)
+        return self.filter_by_array_tickers(tickers, 'symbol', symbols)
 
     def fetch_last_prices(self, symbols: Strings = None, params={}):
         """
         fetches the last price for multiple markets
         :see: https://www.htx.com/en-us/opend/newApiPages/?id=8cb81024-77b5-11ed-9966-0242ac110003 linear swap & linear future
         :see: https://www.htx.com/en-us/opend/newApiPages/?id=28c2e8fc-77ae-11ed-9966-0242ac110003 inverse future
         :see: https://www.htx.com/en-us/opend/newApiPages/?id=5d517ef5-77b6-11ed-9966-0242ac110003 inverse swap
-        :param str[]|None symbols: unified symbols of the markets to fetch the last prices
+        :param str[] [symbols]: unified symbols of the markets to fetch the last prices
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a dictionary of lastprices structures
         """
         self.load_markets()
         symbols = self.market_symbols(symbols)
         market = self.get_market_from_symbols(symbols)
         type = None
```

### Comparing `ccxt-4.2.94/ccxt/huobijp.py` & `ccxt-4.2.95/ccxt/huobijp.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.huobijp import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class huobijp(Exchange, ImplicitAPI):
```

### Comparing `ccxt-4.2.94/ccxt/hyperliquid.py` & `ccxt-4.2.95/ccxt/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/idex.py` & `ccxt-4.2.95/ccxt/idex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.idex import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import ROUND
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.decimal_to_precision import PAD_WITH_ZERO
 from ccxt.base.precise import Precise
```

### Comparing `ccxt-4.2.94/ccxt/independentreserve.py` & `ccxt-4.2.95/ccxt/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/indodax.py` & `ccxt-4.2.95/ccxt/indodax.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.indodax import ImplicitAPI
 import hashlib
 import math
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class indodax(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(indodax, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/kraken.py` & `ccxt-4.2.95/ccxt/kraken.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,60 +31,60 @@
 000001e0: 2c20 5472 616e 7366 6572 456e 7472 790a  , TransferEntry.
 000001f0: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
 00000200: 7274 204c 6973 740a 6672 6f6d 2063 6378  rt List.from ccx
 00000210: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
 00000220: 706f 7274 2045 7863 6861 6e67 6545 7272  port ExchangeErr
 00000230: 6f72 0a66 726f 6d20 6363 7874 2e62 6173  or.from ccxt.bas
 00000240: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
-00000250: 5065 726d 6973 7369 6f6e 4465 6e69 6564  PermissionDenied
-00000260: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-00000270: 6572 726f 7273 2069 6d70 6f72 7420 4163  errors import Ac
-00000280: 636f 756e 7453 7573 7065 6e64 6564 0a66  countSuspended.f
-00000290: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-000002a0: 726f 7273 2069 6d70 6f72 7420 4172 6775  rors import Argu
-000002b0: 6d65 6e74 7352 6571 7569 7265 640a 6672  mentsRequired.fr
-000002c0: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-000002d0: 6f72 7320 696d 706f 7274 2042 6164 5265  ors import BadRe
-000002e0: 7175 6573 740a 6672 6f6d 2063 6378 742e  quest.from ccxt.
-000002f0: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-00000300: 7274 2042 6164 5379 6d62 6f6c 0a66 726f  rt BadSymbol.fro
-00000310: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-00000320: 7273 2069 6d70 6f72 7420 496e 7375 6666  rs import Insuff
-00000330: 6963 6965 6e74 4675 6e64 730a 6672 6f6d  icientFunds.from
-00000340: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-00000350: 7320 696d 706f 7274 2049 6e76 616c 6964  s import Invalid
-00000360: 4164 6472 6573 730a 6672 6f6d 2063 6378  Address.from ccx
-00000370: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
-00000380: 706f 7274 2049 6e76 616c 6964 4f72 6465  port InvalidOrde
-00000390: 720a 6672 6f6d 2063 6378 742e 6261 7365  r.from ccxt.base
-000003a0: 2e65 7272 6f72 7320 696d 706f 7274 204f  .errors import O
-000003b0: 7264 6572 4e6f 7446 6f75 6e64 0a66 726f  rderNotFound.fro
-000003c0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-000003d0: 7273 2069 6d70 6f72 7420 4361 6e63 656c  rs import Cancel
-000003e0: 5065 6e64 696e 670a 6672 6f6d 2063 6378  Pending.from ccx
-000003f0: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
-00000400: 706f 7274 204e 6f74 5375 7070 6f72 7465  port NotSupporte
-00000410: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
-00000420: 2e65 7272 6f72 7320 696d 706f 7274 2044  .errors import D
-00000430: 446f 5350 726f 7465 6374 696f 6e0a 6672  DoSProtection.fr
-00000440: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-00000450: 6f72 7320 696d 706f 7274 2052 6174 654c  ors import RateL
-00000460: 696d 6974 4578 6365 6564 6564 0a66 726f  imitExceeded.fro
-00000470: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-00000480: 7273 2069 6d70 6f72 7420 4578 6368 616e  rs import Exchan
-00000490: 6765 4e6f 7441 7661 696c 6162 6c65 0a66  geNotAvailable.f
-000004a0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-000004b0: 726f 7273 2069 6d70 6f72 7420 4f6e 4d61  rors import OnMa
-000004c0: 696e 7465 6e61 6e63 650a 6672 6f6d 2063  intenance.from c
-000004d0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-000004e0: 696d 706f 7274 2049 6e76 616c 6964 4e6f  import InvalidNo
-000004f0: 6e63 650a 6672 6f6d 2063 6378 742e 6261  nce.from ccxt.ba
-00000500: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000510: 2041 7574 6865 6e74 6963 6174 696f 6e45   AuthenticationE
-00000520: 7272 6f72 0a66 726f 6d20 6363 7874 2e62  rror.from ccxt.b
+00000250: 4175 7468 656e 7469 6361 7469 6f6e 4572  AuthenticationEr
+00000260: 726f 720a 6672 6f6d 2063 6378 742e 6261  ror.from ccxt.ba
+00000270: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
+00000280: 2050 6572 6d69 7373 696f 6e44 656e 6965   PermissionDenie
+00000290: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
+000002a0: 2e65 7272 6f72 7320 696d 706f 7274 2041  .errors import A
+000002b0: 6363 6f75 6e74 5375 7370 656e 6465 640a  ccountSuspended.
+000002c0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+000002d0: 7272 6f72 7320 696d 706f 7274 2041 7267  rrors import Arg
+000002e0: 756d 656e 7473 5265 7175 6972 6564 0a66  umentsRequired.f
+000002f0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+00000300: 726f 7273 2069 6d70 6f72 7420 4261 6452  rors import BadR
+00000310: 6571 7565 7374 0a66 726f 6d20 6363 7874  equest.from ccxt
+00000320: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+00000330: 6f72 7420 4261 6453 796d 626f 6c0a 6672  ort BadSymbol.fr
+00000340: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+00000350: 6f72 7320 696d 706f 7274 2049 6e73 7566  ors import Insuf
+00000360: 6669 6369 656e 7446 756e 6473 0a66 726f  ficientFunds.fro
+00000370: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+00000380: 7273 2069 6d70 6f72 7420 496e 7661 6c69  rs import Invali
+00000390: 6441 6464 7265 7373 0a66 726f 6d20 6363  dAddress.from cc
+000003a0: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
+000003b0: 6d70 6f72 7420 496e 7661 6c69 644f 7264  mport InvalidOrd
+000003c0: 6572 0a66 726f 6d20 6363 7874 2e62 6173  er.from ccxt.bas
+000003d0: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+000003e0: 4f72 6465 724e 6f74 466f 756e 640a 6672  OrderNotFound.fr
+000003f0: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+00000400: 6f72 7320 696d 706f 7274 2043 616e 6365  ors import Cance
+00000410: 6c50 656e 6469 6e67 0a66 726f 6d20 6363  lPending.from cc
+00000420: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
+00000430: 6d70 6f72 7420 4e6f 7453 7570 706f 7274  mport NotSupport
+00000440: 6564 0a66 726f 6d20 6363 7874 2e62 6173  ed.from ccxt.bas
+00000450: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+00000460: 4444 6f53 5072 6f74 6563 7469 6f6e 0a66  DDoSProtection.f
+00000470: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+00000480: 726f 7273 2069 6d70 6f72 7420 5261 7465  rors import Rate
+00000490: 4c69 6d69 7445 7863 6565 6465 640a 6672  LimitExceeded.fr
+000004a0: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+000004b0: 6f72 7320 696d 706f 7274 2045 7863 6861  ors import Excha
+000004c0: 6e67 654e 6f74 4176 6169 6c61 626c 650a  ngeNotAvailable.
+000004d0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+000004e0: 7272 6f72 7320 696d 706f 7274 204f 6e4d  rrors import OnM
+000004f0: 6169 6e74 656e 616e 6365 0a66 726f 6d20  aintenance.from 
+00000500: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
+00000510: 2069 6d70 6f72 7420 496e 7661 6c69 644e   import InvalidN
+00000520: 6f6e 6365 0a66 726f 6d20 6363 7874 2e62  once.from ccxt.b
 00000530: 6173 652e 6465 6369 6d61 6c5f 746f 5f70  ase.decimal_to_p
 00000540: 7265 6369 7369 6f6e 2069 6d70 6f72 7420  recision import 
 00000550: 5452 554e 4341 5445 0a66 726f 6d20 6363  TRUNCATE.from cc
 00000560: 7874 2e62 6173 652e 6465 6369 6d61 6c5f  xt.base.decimal_
 00000570: 746f 5f70 7265 6369 7369 6f6e 2069 6d70  to_precision imp
 00000580: 6f72 7420 5449 434b 5f53 495a 450a 6672  ort TICK_SIZE.fr
 00000590: 6f6d 2063 6378 742e 6261 7365 2e70 7265  om ccxt.base.pre
```

### Comparing `ccxt-4.2.94/ccxt/krakenfutures.py` & `ccxt-4.2.95/ccxt/krakenfutures.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.krakenfutures import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Leverage, Leverages, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import OrderImmediatelyFillable
 from ccxt.base.errors import OrderNotFillable
 from ccxt.base.errors import DuplicateOrderId
+from ccxt.base.errors import ContractUnavailable
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
-from ccxt.base.errors import ContractUnavailable
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class krakenfutures(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/kucoin.py` & `ccxt-4.2.95/ccxt/kucoin.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 from ccxt.abstract.kucoin import ImplicitAPI
 import hashlib
 import math
 import json
 from ccxt.base.types import Account, Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class kucoin(Exchange, ImplicitAPI):
```

### Comparing `ccxt-4.2.94/ccxt/kucoinfutures.py` & `ccxt-4.2.95/ccxt/kucoinfutures.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.kucoin import kucoin
 from ccxt.abstract.kucoinfutures import ImplicitAPI
 from ccxt.base.types import Balances, Currency, Int, MarginModification, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class kucoinfutures(kucoin, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/kuna.py` & `ccxt-4.2.95/ccxt/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/latoken.py` & `ccxt-4.2.95/ccxt/latoken.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.latoken import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class latoken(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(latoken, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/lbank.py` & `ccxt-4.2.95/ccxt/lbank.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,46 +29,46 @@
 000001c0: 6469 6e67 4665 6573 2c20 5472 616e 7361  dingFees, Transa
 000001d0: 6374 696f 6e0a 6672 6f6d 2074 7970 696e  ction.from typin
 000001e0: 6720 696d 706f 7274 204c 6973 740a 6672  g import List.fr
 000001f0: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
 00000200: 6f72 7320 696d 706f 7274 2045 7863 6861  ors import Excha
 00000210: 6e67 6545 7272 6f72 0a66 726f 6d20 6363  ngeError.from cc
 00000220: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
-00000230: 6d70 6f72 7420 5065 726d 6973 7369 6f6e  mport Permission
-00000240: 4465 6e69 6564 0a66 726f 6d20 6363 7874  Denied.from ccxt
-00000250: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000260: 6f72 7420 4172 6775 6d65 6e74 7352 6571  ort ArgumentsReq
-00000270: 7569 7265 640a 6672 6f6d 2063 6378 742e  uired.from ccxt.
-00000280: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-00000290: 7274 2042 6164 5265 7175 6573 740a 6672  rt BadRequest.fr
-000002a0: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-000002b0: 6f72 7320 696d 706f 7274 2042 6164 5379  ors import BadSy
-000002c0: 6d62 6f6c 0a66 726f 6d20 6363 7874 2e62  mbol.from ccxt.b
-000002d0: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
-000002e0: 7420 496e 7375 6666 6963 6965 6e74 4675  t InsufficientFu
-000002f0: 6e64 730a 6672 6f6d 2063 6378 742e 6261  nds.from ccxt.ba
-00000300: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000310: 2049 6e76 616c 6964 4164 6472 6573 730a   InvalidAddress.
-00000320: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-00000330: 7272 6f72 7320 696d 706f 7274 2049 6e76  rrors import Inv
-00000340: 616c 6964 4f72 6465 720a 6672 6f6d 2063  alidOrder.from c
-00000350: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-00000360: 696d 706f 7274 2044 7570 6c69 6361 7465  import Duplicate
-00000370: 4f72 6465 7249 640a 6672 6f6d 2063 6378  OrderId.from ccx
-00000380: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
-00000390: 706f 7274 204e 6f74 5375 7070 6f72 7465  port NotSupporte
-000003a0: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
-000003b0: 2e65 7272 6f72 7320 696d 706f 7274 2052  .errors import R
-000003c0: 6174 654c 696d 6974 4578 6365 6564 6564  ateLimitExceeded
-000003d0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-000003e0: 6572 726f 7273 2069 6d70 6f72 7420 496e  errors import In
-000003f0: 7661 6c69 644e 6f6e 6365 0a66 726f 6d20  validNonce.from 
-00000400: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-00000410: 2069 6d70 6f72 7420 4175 7468 656e 7469   import Authenti
-00000420: 6361 7469 6f6e 4572 726f 720a 6672 6f6d  cationError.from
+00000230: 6d70 6f72 7420 4175 7468 656e 7469 6361  mport Authentica
+00000240: 7469 6f6e 4572 726f 720a 6672 6f6d 2063  tionError.from c
+00000250: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+00000260: 696d 706f 7274 2050 6572 6d69 7373 696f  import Permissio
+00000270: 6e44 656e 6965 640a 6672 6f6d 2063 6378  nDenied.from ccx
+00000280: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+00000290: 706f 7274 2041 7267 756d 656e 7473 5265  port ArgumentsRe
+000002a0: 7175 6972 6564 0a66 726f 6d20 6363 7874  quired.from ccxt
+000002b0: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+000002c0: 6f72 7420 4261 6452 6571 7565 7374 0a66  ort BadRequest.f
+000002d0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+000002e0: 726f 7273 2069 6d70 6f72 7420 4261 6453  rors import BadS
+000002f0: 796d 626f 6c0a 6672 6f6d 2063 6378 742e  ymbol.from ccxt.
+00000300: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
+00000310: 7274 2049 6e73 7566 6669 6369 656e 7446  rt InsufficientF
+00000320: 756e 6473 0a66 726f 6d20 6363 7874 2e62  unds.from ccxt.b
+00000330: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+00000340: 7420 496e 7661 6c69 6441 6464 7265 7373  t InvalidAddress
+00000350: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
+00000360: 6572 726f 7273 2069 6d70 6f72 7420 496e  errors import In
+00000370: 7661 6c69 644f 7264 6572 0a66 726f 6d20  validOrder.from 
+00000380: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
+00000390: 2069 6d70 6f72 7420 4475 706c 6963 6174   import Duplicat
+000003a0: 654f 7264 6572 4964 0a66 726f 6d20 6363  eOrderId.from cc
+000003b0: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
+000003c0: 6d70 6f72 7420 4e6f 7453 7570 706f 7274  mport NotSupport
+000003d0: 6564 0a66 726f 6d20 6363 7874 2e62 6173  ed.from ccxt.bas
+000003e0: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+000003f0: 5261 7465 4c69 6d69 7445 7863 6565 6465  RateLimitExceede
+00000400: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
+00000410: 2e65 7272 6f72 7320 696d 706f 7274 2049  .errors import I
+00000420: 6e76 616c 6964 4e6f 6e63 650a 6672 6f6d  nvalidNonce.from
 00000430: 2063 6378 742e 6261 7365 2e64 6563 696d   ccxt.base.decim
 00000440: 616c 5f74 6f5f 7072 6563 6973 696f 6e20  al_to_precision 
 00000450: 696d 706f 7274 2054 4943 4b5f 5349 5a45  import TICK_SIZE
 00000460: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
 00000470: 7072 6563 6973 6520 696d 706f 7274 2050  precise import P
 00000480: 7265 6369 7365 0a0a 0a63 6c61 7373 206c  recise...class l
 00000490: 6261 6e6b 2845 7863 6861 6e67 652c 2049  bank(Exchange, I
```

### Comparing `ccxt-4.2.94/ccxt/luno.py` & `ccxt-4.2.95/ccxt/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/lykke.py` & `ccxt-4.2.95/ccxt/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/mercado.py` & `ccxt-4.2.95/ccxt/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/mexc.py` & `ccxt-4.2.95/ccxt/mexc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.mexc import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currencies, Currency, IndexType, Int, Leverage, MarginModification, Market, Num, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class mexc(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/ndax.py` & `ccxt-4.2.95/ccxt/ndax.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.ndax import ImplicitAPI
 import hashlib
 import json
 from ccxt.base.types import Account, Balances, Currencies, Currency, IndexType, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Ticker, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import OrderNotFound
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class ndax(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/novadax.py` & `ccxt-4.2.95/ccxt/novadax.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.novadax import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountNotEnabled
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import CancelPending
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class novadax(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/oceanex.py` & `ccxt-4.2.95/ccxt/oceanex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.oceanex import ImplicitAPI
 from ccxt.base.types import Balances, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class oceanex(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(oceanex, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/okcoin.py` & `ccxt-4.2.95/ccxt/okcoin.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,65 +29,65 @@
 000001c0: 2c20 5472 616e 7366 6572 456e 7472 790a  , TransferEntry.
 000001d0: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
 000001e0: 7274 204c 6973 740a 6672 6f6d 2063 6378  rt List.from ccx
 000001f0: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
 00000200: 706f 7274 2045 7863 6861 6e67 6545 7272  port ExchangeErr
 00000210: 6f72 0a66 726f 6d20 6363 7874 2e62 6173  or.from ccxt.bas
 00000220: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
-00000230: 5065 726d 6973 7369 6f6e 4465 6e69 6564  PermissionDenied
-00000240: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-00000250: 6572 726f 7273 2069 6d70 6f72 7420 4163  errors import Ac
-00000260: 636f 756e 744e 6f74 456e 6162 6c65 640a  countNotEnabled.
-00000270: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-00000280: 7272 6f72 7320 696d 706f 7274 2041 6363  rrors import Acc
-00000290: 6f75 6e74 5375 7370 656e 6465 640a 6672  ountSuspended.fr
-000002a0: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-000002b0: 6f72 7320 696d 706f 7274 2041 7267 756d  ors import Argum
-000002c0: 656e 7473 5265 7175 6972 6564 0a66 726f  entsRequired.fro
-000002d0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-000002e0: 7273 2069 6d70 6f72 7420 4261 6452 6571  rs import BadReq
-000002f0: 7565 7374 0a66 726f 6d20 6363 7874 2e62  uest.from ccxt.b
-00000300: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
-00000310: 7420 4261 6453 796d 626f 6c0a 6672 6f6d  t BadSymbol.from
-00000320: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-00000330: 7320 696d 706f 7274 2049 6e73 7566 6669  s import Insuffi
-00000340: 6369 656e 7446 756e 6473 0a66 726f 6d20  cientFunds.from 
-00000350: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-00000360: 2069 6d70 6f72 7420 496e 7661 6c69 6441   import InvalidA
-00000370: 6464 7265 7373 0a66 726f 6d20 6363 7874  ddress.from ccxt
-00000380: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000390: 6f72 7420 496e 7661 6c69 644f 7264 6572  ort InvalidOrder
-000003a0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-000003b0: 6572 726f 7273 2069 6d70 6f72 7420 4f72  errors import Or
-000003c0: 6465 724e 6f74 466f 756e 640a 6672 6f6d  derNotFound.from
-000003d0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-000003e0: 7320 696d 706f 7274 2043 616e 6365 6c50  s import CancelP
-000003f0: 656e 6469 6e67 0a66 726f 6d20 6363 7874  ending.from ccxt
-00000400: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000410: 6f72 7420 4e6f 7453 7570 706f 7274 6564  ort NotSupported
-00000420: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-00000430: 6572 726f 7273 2069 6d70 6f72 7420 4e65  errors import Ne
-00000440: 7477 6f72 6b45 7272 6f72 0a66 726f 6d20  tworkError.from 
-00000450: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-00000460: 2069 6d70 6f72 7420 5261 7465 4c69 6d69   import RateLimi
-00000470: 7445 7863 6565 6465 640a 6672 6f6d 2063  tExceeded.from c
-00000480: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-00000490: 696d 706f 7274 2045 7863 6861 6e67 654e  import ExchangeN
-000004a0: 6f74 4176 6169 6c61 626c 650a 6672 6f6d  otAvailable.from
-000004b0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-000004c0: 7320 696d 706f 7274 204f 6e4d 6169 6e74  s import OnMaint
-000004d0: 656e 616e 6365 0a66 726f 6d20 6363 7874  enance.from ccxt
-000004e0: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-000004f0: 6f72 7420 496e 7661 6c69 644e 6f6e 6365  ort InvalidNonce
-00000500: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-00000510: 6572 726f 7273 2069 6d70 6f72 7420 5265  errors import Re
-00000520: 7175 6573 7454 696d 656f 7574 0a66 726f  questTimeout.fro
-00000530: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-00000540: 7273 2069 6d70 6f72 7420 4175 7468 656e  rs import Authen
-00000550: 7469 6361 7469 6f6e 4572 726f 720a 6672  ticationError.fr
+00000230: 4175 7468 656e 7469 6361 7469 6f6e 4572  AuthenticationEr
+00000240: 726f 720a 6672 6f6d 2063 6378 742e 6261  ror.from ccxt.ba
+00000250: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
+00000260: 2050 6572 6d69 7373 696f 6e44 656e 6965   PermissionDenie
+00000270: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
+00000280: 2e65 7272 6f72 7320 696d 706f 7274 2041  .errors import A
+00000290: 6363 6f75 6e74 4e6f 7445 6e61 626c 6564  ccountNotEnabled
+000002a0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
+000002b0: 6572 726f 7273 2069 6d70 6f72 7420 4163  errors import Ac
+000002c0: 636f 756e 7453 7573 7065 6e64 6564 0a66  countSuspended.f
+000002d0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+000002e0: 726f 7273 2069 6d70 6f72 7420 4172 6775  rors import Argu
+000002f0: 6d65 6e74 7352 6571 7569 7265 640a 6672  mentsRequired.fr
+00000300: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+00000310: 6f72 7320 696d 706f 7274 2042 6164 5265  ors import BadRe
+00000320: 7175 6573 740a 6672 6f6d 2063 6378 742e  quest.from ccxt.
+00000330: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
+00000340: 7274 2042 6164 5379 6d62 6f6c 0a66 726f  rt BadSymbol.fro
+00000350: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+00000360: 7273 2069 6d70 6f72 7420 496e 7375 6666  rs import Insuff
+00000370: 6963 6965 6e74 4675 6e64 730a 6672 6f6d  icientFunds.from
+00000380: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+00000390: 7320 696d 706f 7274 2049 6e76 616c 6964  s import Invalid
+000003a0: 4164 6472 6573 730a 6672 6f6d 2063 6378  Address.from ccx
+000003b0: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+000003c0: 706f 7274 2049 6e76 616c 6964 4f72 6465  port InvalidOrde
+000003d0: 720a 6672 6f6d 2063 6378 742e 6261 7365  r.from ccxt.base
+000003e0: 2e65 7272 6f72 7320 696d 706f 7274 204f  .errors import O
+000003f0: 7264 6572 4e6f 7446 6f75 6e64 0a66 726f  rderNotFound.fro
+00000400: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+00000410: 7273 2069 6d70 6f72 7420 4361 6e63 656c  rs import Cancel
+00000420: 5065 6e64 696e 670a 6672 6f6d 2063 6378  Pending.from ccx
+00000430: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+00000440: 706f 7274 204e 6f74 5375 7070 6f72 7465  port NotSupporte
+00000450: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
+00000460: 2e65 7272 6f72 7320 696d 706f 7274 204e  .errors import N
+00000470: 6574 776f 726b 4572 726f 720a 6672 6f6d  etworkError.from
+00000480: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+00000490: 7320 696d 706f 7274 2052 6174 654c 696d  s import RateLim
+000004a0: 6974 4578 6365 6564 6564 0a66 726f 6d20  itExceeded.from 
+000004b0: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
+000004c0: 2069 6d70 6f72 7420 4578 6368 616e 6765   import Exchange
+000004d0: 4e6f 7441 7661 696c 6162 6c65 0a66 726f  NotAvailable.fro
+000004e0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+000004f0: 7273 2069 6d70 6f72 7420 4f6e 4d61 696e  rs import OnMain
+00000500: 7465 6e61 6e63 650a 6672 6f6d 2063 6378  tenance.from ccx
+00000510: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+00000520: 706f 7274 2049 6e76 616c 6964 4e6f 6e63  port InvalidNonc
+00000530: 650a 6672 6f6d 2063 6378 742e 6261 7365  e.from ccxt.base
+00000540: 2e65 7272 6f72 7320 696d 706f 7274 2052  .errors import R
+00000550: 6571 7565 7374 5469 6d65 6f75 740a 6672  equestTimeout.fr
 00000560: 6f6d 2063 6378 742e 6261 7365 2e64 6563  om ccxt.base.dec
 00000570: 696d 616c 5f74 6f5f 7072 6563 6973 696f  imal_to_precisio
 00000580: 6e20 696d 706f 7274 2054 4943 4b5f 5349  n import TICK_SI
 00000590: 5a45 0a66 726f 6d20 6363 7874 2e62 6173  ZE.from ccxt.bas
 000005a0: 652e 7072 6563 6973 6520 696d 706f 7274  e.precise import
 000005b0: 2050 7265 6369 7365 0a0a 0a63 6c61 7373   Precise...class
 000005c0: 206f 6b63 6f69 6e28 4578 6368 616e 6765   okcoin(Exchange
```

### Comparing `ccxt-4.2.94/ccxt/okx.py` & `ccxt-4.2.95/ccxt/okx.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.okx import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Conversion, Currencies, Currency, Greeks, Int, Leverage, MarginModification, Market, MarketInterface, Num, Option, OptionChain, Order, OrderBook, OrderRequest, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountNotEnabled
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import CancelPending
+from ccxt.base.errors import ContractUnavailable
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
-from ccxt.base.errors import ContractUnavailable
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class okx(Exchange, ImplicitAPI):
 
     def describe(self):
@@ -1134,15 +1134,15 @@
         params = self.omit(params, 'instType')
         type = self.safe_string(params, 'type')
         if (type is None) and (instType is not None):
             params['type'] = instType
         return super(okx, self).handle_market_type_and_params(methodName, market, params)
 
     def convert_to_instrument_type(self, type):
-        exchangeTypes = self.safe_value(self.options, 'exchangeType', {})
+        exchangeTypes = self.safe_dict(self.options, 'exchangeType', {})
         return self.safe_string(exchangeTypes, type, type)
 
     def create_expired_option_market(self, symbol: str):
         # support expired option contracts
         quote = 'USD'
         optionParts = symbol.split('-')
         symbolBase = symbol.split('/')
@@ -2768,15 +2768,15 @@
         for i in range(0, len(orders)):
             rawOrder = orders[i]
             marketId = self.safe_string(rawOrder, 'symbol')
             type = self.safe_string(rawOrder, 'type')
             side = self.safe_string(rawOrder, 'side')
             amount = self.safe_value(rawOrder, 'amount')
             price = self.safe_value(rawOrder, 'price')
-            orderParams = self.safe_value(rawOrder, 'params', {})
+            orderParams = self.safe_dict(rawOrder, 'params', {})
             extendedParams = self.extend(orderParams, params)  # the request does not accept extra params since it's a list, so we're extending each order with the common params
             orderRequest = self.create_order_request(marketId, type, side, amount, price, extendedParams)
             ordersRequests.append(orderRequest)
         response = self.privatePostTradeBatchOrders(ordersRequests)
         # {
         #     "code": "0",
         #     "data": [
@@ -2930,16 +2930,16 @@
         #                 "sCode": "0",
         #                 "sMsg": ""
         #            }
         #        ],
         #        "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data', [])
-        first = self.safe_value(data, 0)
+        data = self.safe_list(response, 'data', [])
+        first = self.safe_dict(data, 0, {})
         order = self.parse_order(first, market)
         order['type'] = type
         order['side'] = side
         return order
 
     def cancel_order(self, id: str, symbol: Str = None, params={}):
         """
@@ -4036,15 +4036,15 @@
         :returns dict: a `ledger structure <https://docs.ccxt.com/#/?id=ledger-structure>`
         """
         self.load_markets()
         paginate = False
         paginate, params = self.handle_option_and_params(params, 'fetchLedger', 'paginate')
         if paginate:
             return self.fetch_paginated_call_dynamic('fetchLedger', code, since, limit, params)
-        options = self.safe_value(self.options, 'fetchLedger', {})
+        options = self.safe_dict(self.options, 'fetchLedger', {})
         method = self.safe_string(options, 'method')
         method = self.safe_string(params, 'method', method)
         params = self.omit(params, 'method')
         request = {
             # 'instType': None,  # 'SPOT', 'MARGIN', 'SWAP', 'FUTURES", 'OPTION'
             # 'ccy': None,  # currency['id'],
             # 'mgnMode': None,  # 'isolated', 'cross'
@@ -4351,15 +4351,15 @@
         #             # {"ccy":"usdt-erc20","to":"6","addr":"0x696abb81974a8793352cbd33aadcf78eda3cfdfa","selected":true},
         #             # {"ccy":"usdt-trc20","to":"6","addr":"TRrd5SiSZrfQVRKm4e9SRSbn2LNTYqCjqx","selected":true},
         #             # {"ccy":"usdt_okexchain","to":"6","addr":"0x696abb81974a8793352cbd33aadcf78eda3cfdfa","selected":true},
         #             # {"ccy":"usdt_kip20","to":"6","addr":"0x696abb81974a8793352cbd33aadcf78eda3cfdfa","selected":true},
         #         ]
         #     }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         filtered = self.filter_by(data, 'selected', True)
         parsed = self.parse_deposit_addresses(filtered, [currency['code']], False)
         return self.index_by(parsed, 'network')
 
     def fetch_deposit_address(self, code: str, params={}):
         """
         fetch the deposit address for a currency associated with self account
@@ -4414,23 +4414,23 @@
             'ccy': currency['id'],
             'toAddr': address,
             'dest': '4',  # 2 = OKCoin International, 3 = OKX 4 = others
             'amt': self.number_to_string(amount),
         }
         network = self.safe_string(params, 'network')  # self line allows the user to specify either ERC20 or ETH
         if network is not None:
-            networks = self.safe_value(self.options, 'networks', {})
+            networks = self.safe_dict(self.options, 'networks', {})
             network = self.safe_string(networks, network.upper(), network)  # handle ETH>ERC20 alias
             request['chain'] = currency['id'] + '-' + network
             params = self.omit(params, 'network')
         fee = self.safe_string(params, 'fee')
         if fee is None:
             currencies = self.fetch_currencies()
             self.currencies = self.deep_extend(self.currencies, currencies)
-            targetNetwork = self.safe_value(currency['networks'], self.network_id_to_code(network), {})
+            targetNetwork = self.safe_dict(currency['networks'], self.network_id_to_code(network), {})
             fee = self.safe_string(targetNetwork, 'fee')
             if fee is None:
                 raise ArgumentsRequired(self.id + ' withdraw() requires a "fee" string parameter, network transaction fee must be ≥ 0. Withdrawals to OKCoin or OKX are fee-free, please set "0". Withdrawing to external digital asset address requires network transaction fee.')
         request['fee'] = self.number_to_string(fee)  # withdrawals to OKCoin or OKX are fee-free, please set 0
         query = self.omit(params, ['fee'])
         response = self.privatePostAssetWithdrawal(self.extend(request, query))
         #
@@ -4442,15 +4442,15 @@
         #                 "amt": "0.1",
         #                 "wdId": "67485",
         #                 "ccy": "BTC"
         #             }
         #         ]
         #     }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         transaction = self.safe_dict(data, 0)
         return self.parse_transaction(transaction, currency)
 
     def fetch_deposits(self, code: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Transaction]:
         """
         fetch all deposits made to an account
         :see: https://www.okx.com/docs-v5/en/#rest-api-funding-get-deposit-history
@@ -4649,15 +4649,15 @@
         #                "ts": "1641376485000",
         #                "wdId": "25147041"
         #            }
         #        ],
         #        "msg": ''
         #    }
         #
-        data = self.safe_value(response, 'data')
+        data = self.safe_list(response, 'data', [])
         withdrawal = self.safe_dict(data, 0, {})
         return self.parse_transaction(withdrawal)
 
     def parse_transaction_status(self, status):
         #
         # deposit statuses
         #
@@ -4921,16 +4921,16 @@
         #                 "uplRatio": "-0.0025490556801078",
         #                 "vegaBS": "",
         #                 "vegaPA": ""
         #             }
         #         ]
         #     }
         #
-        data = self.safe_value(response, 'data', [])
-        position = self.safe_value(data, 0)
+        data = self.safe_list(response, 'data', [])
+        position = self.safe_dict(data, 0)
         if position is None:
             return None
         return self.parse_position(position, market)
 
     def fetch_positions(self, symbols: Strings = None, params={}):
         """
         :see: https://www.okx.com/docs-v5/en/#rest-api-account-get-positions
@@ -4952,15 +4952,15 @@
             for i in range(0, len(symbols)):
                 entry = symbols[i]
                 market = self.market(entry)
                 marketIds.append(market['id'])
             marketIdsLength = len(marketIds)
             if marketIdsLength > 0:
                 request['instId'] = ','.join(marketIds)
-        fetchPositionsOptions = self.safe_value(self.options, 'fetchPositions', {})
+        fetchPositionsOptions = self.safe_dict(self.options, 'fetchPositions', {})
         method = self.safe_string(fetchPositionsOptions, 'method', 'privateGetAccountPositions')
         response = None
         if method == 'privateGetAccountPositionsHistory':
             response = self.privateGetAccountPositionsHistory(self.extend(request, params))
         else:
             response = self.privateGetAccountPositions(self.extend(request, params))
         #
@@ -5005,15 +5005,15 @@
         #                 "uplRatio": "-0.0025490556801078",
         #                 "vegaBS": "",
         #                 "vegaPA": ""
         #             }
         #         ]
         #     }
         #
-        positions = self.safe_value(response, 'data', [])
+        positions = self.safe_list(response, 'data', [])
         result = []
         for i in range(0, len(positions)):
             result.append(self.parse_position(positions[i]))
         return self.filter_by_array_positions(result, 'symbol', symbols, False)
 
     def fetch_positions_for_symbol(self, symbol: str, params={}):
         """
@@ -5193,15 +5193,15 @@
         :param str fromAccount: account to transfer from
         :param str toAccount: account to transfer to
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `transfer structure <https://docs.ccxt.com/#/?id=transfer-structure>`
         """
         self.load_markets()
         currency = self.currency(code)
-        accountsByType = self.safe_value(self.options, 'accountsByType', {})
+        accountsByType = self.safe_dict(self.options, 'accountsByType', {})
         fromId = self.safe_string(accountsByType, fromAccount, fromAccount)
         toId = self.safe_string(accountsByType, toAccount, toAccount)
         request = {
             'ccy': currency['id'],
             'amt': self.currency_to_precision(code, amount),
             'type': '0',  # 0 = transfer within account by default, 1 = master account to sub-account, 2 = sub-account to master account, 3 = sub-account to master account(Only applicable to APIKey from sub-account), 4 = sub-account to sub-account
             'from': fromId,  # remitting account, 6: Funding account, 18: Trading account
@@ -5233,15 +5233,15 @@
         #                 "from": "6",
         #                 "amt": "0.1",
         #                 "to": "18"
         #             }
         #         ]
         #     }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         rawTransfer = self.safe_dict(data, 0, {})
         return self.parse_transfer(rawTransfer, currency)
 
     def parse_transfer(self, transfer, currency: Currency = None):
         #
         # transfer
         #
@@ -5296,15 +5296,15 @@
         #
         id = self.safe_string_2(transfer, 'transId', 'billId')
         currencyId = self.safe_string(transfer, 'ccy')
         code = self.safe_currency_code(currencyId, currency)
         amount = self.safe_number(transfer, 'amt')
         fromAccountId = self.safe_string(transfer, 'from')
         toAccountId = self.safe_string(transfer, 'to')
-        accountsById = self.safe_value(self.options, 'accountsById', {})
+        accountsById = self.safe_dict(self.options, 'accountsById', {})
         timestamp = self.safe_integer(transfer, 'ts')
         balanceChange = self.safe_string(transfer, 'sz')
         if balanceChange is not None:
             amount = self.parse_number(Precise.string_abs(balanceChange))
         return {
             'info': transfer,
             'id': id,
@@ -5346,15 +5346,15 @@
         #                 "transId": "464424732",
         #                 "type": "0"
         #             }
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         transfer = self.safe_dict(data, 0)
         return self.parse_transfer(transfer)
 
     def fetch_transfers(self, code: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         fetch a history of internal transfers made on an account
         :see: https://www.okx.com/docs-v5/en/#trading-account-rest-api-get-bills-details-last-3-months
@@ -5531,16 +5531,16 @@
         #                "nextFundingRate": "0.00017",
         #                "nextFundingTime": "1634284800000"
         #            }
         #        ],
         #        "msg": ""
         #    }
         #
-        data = self.safe_value(response, 'data', [])
-        entry = self.safe_value(data, 0, {})
+        data = self.safe_list(response, 'data', [])
+        entry = self.safe_dict(data, 0, {})
         return self.parse_funding_rate(entry, market)
 
     def fetch_funding_history(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         fetch the history of funding payments paid and received on self account
         :see: https://www.okx.com/docs-v5/en/#trading-account-rest-api-get-bills-details-last-3-months
         :param str symbol: unified market symbol
@@ -5664,15 +5664,15 @@
         #        "subType": "174",
         #        "sz": "9",
         #        "to": "",
         #        "ts": "1636387215588",
         #        "type": "8"
         #    }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         result = []
         for i in range(0, len(data)):
             entry = data[i]
             timestamp = self.safe_integer(entry, 'ts')
             instId = self.safe_string(entry, 'instId')
             marketInner = self.safe_market(instId)
             currencyId = self.safe_string(entry, 'ccy')
@@ -5835,15 +5835,15 @@
         #                "ccy": "BTC",
         #                "interestRate": "0.00000833"
         #            }
         #            ...
         #        ],
         #    }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         rates = []
         for i in range(0, len(data)):
             rates.append(self.parse_borrow_rate(data[i]))
         return rates
 
     def fetch_cross_borrow_rate(self, code: str, params={}):
         """
@@ -5868,16 +5868,16 @@
         #                "interestRate": "0.00002065"
         #             }
         #             ...
         #        ],
         #        "msg": ""
         #    }
         #
-        data = self.safe_value(response, 'data')
-        rate = self.safe_value(data, 0)
+        data = self.safe_list(response, 'data', [])
+        rate = self.safe_dict(data, 0, {})
         return self.parse_borrow_rate(rate)
 
     def parse_borrow_rate(self, info, currency: Currency = None):
         #
         #    {
         #        "amt": "992.10341195",
         #        "ccy": "BTC",
@@ -5964,15 +5964,15 @@
         #                 "rate": "0.01",
         #                 "ts": "1643954400000"
         #             },
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data')
+        data = self.safe_list(response, 'data', [])
         return self.parse_borrow_rate_histories(data, codes, since, limit)
 
     def fetch_borrow_rate_history(self, code: str, since: Int = None, limit: Int = None, params={}):
         """
         retrieves a history of a currencies borrow interest rate at specific time slots
         :see: https://www.okx.com/docs-v5/en/#financial-product-savings-get-public-borrow-history-public
         :param str code: unified currency code
@@ -6004,15 +6004,15 @@
         #                 "rate": "0.01",
         #                 "ts": "1643954400000"
         #             },
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data')
+        data = self.safe_list(response, 'data', [])
         return self.parse_borrow_rate_history(data, code, since, limit)
 
     def modify_margin_helper(self, symbol: str, amount, type, params={}) -> MarginModification:
         self.load_markets()
         market = self.market(symbol)
         posSide = self.safe_string(params, 'posSide', 'net')
         params = self.omit(params, ['posSide'])
@@ -6184,15 +6184,15 @@
         #                "tier": "1",
         #                "uly": ""
         #            },
         #            ...
         #        ]
         #    }
         #
-        data = self.safe_value(response, 'data')
+        data = self.safe_list(response, 'data', [])
         return self.parse_market_leverage_tiers(data, market)
 
     def parse_market_leverage_tiers(self, info, market: Market = None):
         """
          * @ignore
         :param dict info: Exchange response for 1 market
         :param dict market: CCXT market
@@ -6277,15 +6277,15 @@
         #                "type": "1"
         #            },
         #            ...
         #        ],
         #        "msg": ""
         #    }
         #
-        data = self.safe_value(response, 'data')
+        data = self.safe_list(response, 'data', [])
         interest = self.parse_borrow_interests(data)
         return self.filter_by_currency_since_limit(interest, code, since, limit)
 
     def parse_borrow_interest(self, info, market: Market = None):
         instId = self.safe_string(info, 'instId')
         if instId is not None:
             market = self.safe_market(instId, market)
@@ -6330,16 +6330,16 @@
         #                 "side": "borrow",
         #                 "state": "1"
         #             }
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data', [])
-        loan = self.safe_value(data, 0)
+        data = self.safe_list(response, 'data', [])
+        loan = self.safe_dict(data, 0, {})
         return self.parse_margin_loan(loan, currency)
 
     def repay_cross_margin(self, code: str, amount, params={}):
         """
         repay borrowed margin and interest
         :see: https://www.okx.com/docs-v5/en/#trading-account-rest-api-vip-loans-borrow-and-repay
         :param str code: unified currency code of the currency to repay
@@ -6372,16 +6372,16 @@
         #                 "side": "repay",
         #                 "state": "1"
         #             }
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data', [])
-        loan = self.safe_value(data, 0)
+        data = self.safe_list(response, 'data', [])
+        loan = self.safe_dict(data, 0, {})
         return self.parse_margin_loan(loan, currency)
 
     def parse_margin_loan(self, info, currency: Currency = None):
         #
         #     {
         #         "amt": "102",
         #         "availLoan": "97",
@@ -6450,16 +6450,16 @@
         :param str timeframe: "5m", "1h", or "1d" for option only "1d" or "8h"
         :param int [since]: The time in ms of the earliest record to retrieve unix timestamp
         :param int [limit]: Not used by okx, but parsed internally by CCXT
         :param dict [params]: Exchange specific parameters
         :param int [params.until]: The time in ms of the latest record to retrieve unix timestamp
         :returns: An array of `open interest structures <https://docs.ccxt.com/#/?id=open-interest-structure>`
         """
-        options = self.safe_value(self.options, 'fetchOpenInterestHistory', {})
-        timeframes = self.safe_value(options, 'timeframes', {})
+        options = self.safe_dict(self.options, 'fetchOpenInterestHistory', {})
+        timeframes = self.safe_dict(options, 'timeframes', {})
         timeframe = self.safe_string(timeframes, timeframe, timeframe)
         if timeframe != '5m' and timeframe != '1H' and timeframe != '1D':
             raise BadRequest(self.id + ' fetchOpenInterestHistory cannot only use the 5m, 1h, and 1d timeframe')
         self.load_markets()
         # handle unified currency code or symbol
         currencyId = None
         market = None
@@ -6716,15 +6716,15 @@
         #                 ],
         #                 "ts":"1684656000000"
         #             }
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         settlements = self.parse_settlements(data, market)
         sorted = self.sort_by(settlements, 'timestamp')
         return self.filter_by_symbol_since_limit(sorted, market['symbol'], since, limit)
 
     def parse_settlement(self, settlement, market):
         #
         #     {
@@ -6755,15 +6755,15 @@
         #         "ts":"1684656000000"
         #     }
         #
         result = []
         for i in range(0, len(settlements)):
             entry = settlements[i]
             timestamp = self.safe_integer(entry, 'ts')
-            details = self.safe_value(entry, 'details', [])
+            details = self.safe_list(entry, 'details', [])
             for j in range(0, len(details)):
                 settlement = self.parse_settlement(details[j], market)
                 result.append(self.extend(settlement, {
                     'timestamp': timestamp,
                     'datetime': self.iso8601(timestamp),
                 }))
         return result
@@ -6795,15 +6795,15 @@
         #                 "BTC-USD",
         #                 "ETH-USD"
         #             ]
         #         ],
         #         "msg": ""
         #     }
         #
-        underlyings = self.safe_value(response, 'data', [])
+        underlyings = self.safe_list(response, 'data', [])
         return underlyings[0]
 
     def fetch_greeks(self, symbol: str, params={}) -> Greeks:
         """
         fetches an option contracts greeks, financial metrics used to measure the factors that affect the price of an options contract
         :see: https://www.okx.com/docs-v5/en/#public-data-rest-api-get-option-market-data
         :param str symbol: unified symbol of the market to fetch greeks for
@@ -6845,15 +6845,15 @@
         #                 "vegaBS": "74.44022302387287",
         #                 "volLv": "0.5948549730405797"
         #             },
         #         ],
         #         "msg": ""
         #     }
         #
-        data = self.safe_value(response, 'data', [])
+        data = self.safe_list(response, 'data', [])
         for i in range(0, len(data)):
             entry = data[i]
             entryMarketId = self.safe_string(entry, 'instId')
             if entryMarketId == marketId:
                 return self.parse_greeks(entry, market)
         return None
 
@@ -6958,15 +6958,15 @@
         #            }
         #        ],
         #        "inTime": "1701877077101064",
         #        "msg": "All operations failed",
         #        "outTime": "1701877077102579"
         #    }
         #
-        data = self.safe_value(response, 'data')
+        data = self.safe_list(response, 'data', [])
         order = self.safe_dict(data, 0)
         return self.parse_order(order, market)
 
     def fetch_option(self, symbol: str, params={}) -> Option:
         """
         fetches option data that is commonly found in an option chain
         :see: https://www.okx.com/docs-v5/en/#order-book-trading-market-data-get-ticker
@@ -7267,15 +7267,15 @@
         #        "data": [],
         #        "msg": "Incorrect trade password"
         #    }
         #
         code = self.safe_string(response, 'code')
         if (code != '0') and (code != '2'):  # 2 means that bulk operation partially succeeded
             feedback = self.id + ' ' + body
-            data = self.safe_value(response, 'data', [])
+            data = self.safe_list(response, 'data', [])
             for i in range(0, len(data)):
                 error = data[i]
                 errorCode = self.safe_string(error, 'sCode')
                 message = self.safe_string(error, 'sMsg')
                 self.throw_exactly_matched_exception(self.exceptions['exact'], errorCode, feedback)
                 self.throw_broadly_matched_exception(self.exceptions['broad'], message, feedback)
             self.throw_exactly_matched_exception(self.exceptions['exact'], code, feedback)
```

### Comparing `ccxt-4.2.94/ccxt/onetrading.py` & `ccxt-4.2.95/ccxt/onetrading.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.onetrading import ImplicitAPI
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class onetrading(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/p2b.py` & `ccxt-4.2.95/ccxt/p2b.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.p2b import ImplicitAPI
 import hashlib
 from ccxt.base.types import Int, Market, Num, Order, OrderSide, OrderType, Str, Strings, Ticker, Tickers
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class p2b(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(p2b, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/paymium.py` & `ccxt-4.2.95/ccxt/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/phemex.py` & `ccxt-4.2.95/ccxt/phemex.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,52 +31,52 @@
 000001e0: 696f 6e2c 2054 7261 6e73 6665 7245 6e74  ion, TransferEnt
 000001f0: 7279 0a66 726f 6d20 7479 7069 6e67 2069  ry.from typing i
 00000200: 6d70 6f72 7420 4c69 7374 0a66 726f 6d20  mport List.from 
 00000210: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
 00000220: 2069 6d70 6f72 7420 4578 6368 616e 6765   import Exchange
 00000230: 4572 726f 720a 6672 6f6d 2063 6378 742e  Error.from ccxt.
 00000240: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-00000250: 7274 2050 6572 6d69 7373 696f 6e44 656e  rt PermissionDen
-00000260: 6965 640a 6672 6f6d 2063 6378 742e 6261  ied.from ccxt.ba
-00000270: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000280: 2041 6363 6f75 6e74 5375 7370 656e 6465   AccountSuspende
-00000290: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
-000002a0: 2e65 7272 6f72 7320 696d 706f 7274 2041  .errors import A
-000002b0: 7267 756d 656e 7473 5265 7175 6972 6564  rgumentsRequired
-000002c0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-000002d0: 6572 726f 7273 2069 6d70 6f72 7420 4261  errors import Ba
-000002e0: 6452 6571 7565 7374 0a66 726f 6d20 6363  dRequest.from cc
-000002f0: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
-00000300: 6d70 6f72 7420 4261 6453 796d 626f 6c0a  mport BadSymbol.
-00000310: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-00000320: 7272 6f72 7320 696d 706f 7274 2049 6e73  rrors import Ins
-00000330: 7566 6669 6369 656e 7446 756e 6473 0a66  ufficientFunds.f
-00000340: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-00000350: 726f 7273 2069 6d70 6f72 7420 496e 7661  rors import Inva
-00000360: 6c69 644f 7264 6572 0a66 726f 6d20 6363  lidOrder.from cc
-00000370: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
-00000380: 6d70 6f72 7420 4f72 6465 724e 6f74 466f  mport OrderNotFo
-00000390: 756e 640a 6672 6f6d 2063 6378 742e 6261  und.from ccxt.ba
-000003a0: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-000003b0: 2043 616e 6365 6c50 656e 6469 6e67 0a66   CancelPending.f
-000003c0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-000003d0: 726f 7273 2069 6d70 6f72 7420 4475 706c  rors import Dupl
-000003e0: 6963 6174 654f 7264 6572 4964 0a66 726f  icateOrderId.fro
-000003f0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-00000400: 7273 2069 6d70 6f72 7420 4e6f 7453 7570  rs import NotSup
-00000410: 706f 7274 6564 0a66 726f 6d20 6363 7874  ported.from ccxt
-00000420: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000430: 6f72 7420 4444 6f53 5072 6f74 6563 7469  ort DDoSProtecti
-00000440: 6f6e 0a66 726f 6d20 6363 7874 2e62 6173  on.from ccxt.bas
-00000450: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
-00000460: 5261 7465 4c69 6d69 7445 7863 6565 6465  RateLimitExceede
-00000470: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
-00000480: 2e65 7272 6f72 7320 696d 706f 7274 2041  .errors import A
-00000490: 7574 6865 6e74 6963 6174 696f 6e45 7272  uthenticationErr
-000004a0: 6f72 0a66 726f 6d20 6363 7874 2e62 6173  or.from ccxt.bas
+00000250: 7274 2041 7574 6865 6e74 6963 6174 696f  rt Authenticatio
+00000260: 6e45 7272 6f72 0a66 726f 6d20 6363 7874  nError.from ccxt
+00000270: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+00000280: 6f72 7420 5065 726d 6973 7369 6f6e 4465  ort PermissionDe
+00000290: 6e69 6564 0a66 726f 6d20 6363 7874 2e62  nied.from ccxt.b
+000002a0: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+000002b0: 7420 4163 636f 756e 7453 7573 7065 6e64  t AccountSuspend
+000002c0: 6564 0a66 726f 6d20 6363 7874 2e62 6173  ed.from ccxt.bas
+000002d0: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+000002e0: 4172 6775 6d65 6e74 7352 6571 7569 7265  ArgumentsRequire
+000002f0: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
+00000300: 2e65 7272 6f72 7320 696d 706f 7274 2042  .errors import B
+00000310: 6164 5265 7175 6573 740a 6672 6f6d 2063  adRequest.from c
+00000320: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+00000330: 696d 706f 7274 2042 6164 5379 6d62 6f6c  import BadSymbol
+00000340: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
+00000350: 6572 726f 7273 2069 6d70 6f72 7420 496e  errors import In
+00000360: 7375 6666 6963 6965 6e74 4675 6e64 730a  sufficientFunds.
+00000370: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+00000380: 7272 6f72 7320 696d 706f 7274 2049 6e76  rrors import Inv
+00000390: 616c 6964 4f72 6465 720a 6672 6f6d 2063  alidOrder.from c
+000003a0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+000003b0: 696d 706f 7274 204f 7264 6572 4e6f 7446  import OrderNotF
+000003c0: 6f75 6e64 0a66 726f 6d20 6363 7874 2e62  ound.from ccxt.b
+000003d0: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+000003e0: 7420 4361 6e63 656c 5065 6e64 696e 670a  t CancelPending.
+000003f0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+00000400: 7272 6f72 7320 696d 706f 7274 2044 7570  rrors import Dup
+00000410: 6c69 6361 7465 4f72 6465 7249 640a 6672  licateOrderId.fr
+00000420: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+00000430: 6f72 7320 696d 706f 7274 204e 6f74 5375  ors import NotSu
+00000440: 7070 6f72 7465 640a 6672 6f6d 2063 6378  pported.from ccx
+00000450: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+00000460: 706f 7274 2044 446f 5350 726f 7465 6374  port DDoSProtect
+00000470: 696f 6e0a 6672 6f6d 2063 6378 742e 6261  ion.from ccxt.ba
+00000480: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
+00000490: 2052 6174 654c 696d 6974 4578 6365 6564   RateLimitExceed
+000004a0: 6564 0a66 726f 6d20 6363 7874 2e62 6173  ed.from ccxt.bas
 000004b0: 652e 6465 6369 6d61 6c5f 746f 5f70 7265  e.decimal_to_pre
 000004c0: 6369 7369 6f6e 2069 6d70 6f72 7420 5449  cision import TI
 000004d0: 434b 5f53 495a 450a 6672 6f6d 2063 6378  CK_SIZE.from ccx
 000004e0: 742e 6261 7365 2e70 7265 6369 7365 2069  t.base.precise i
 000004f0: 6d70 6f72 7420 5072 6563 6973 650a 0a0a  mport Precise...
 00000500: 636c 6173 7320 7068 656d 6578 2845 7863  class phemex(Exc
 00000510: 6861 6e67 652c 2049 6d70 6c69 6369 7441  hange, ImplicitA
```

### Comparing `ccxt-4.2.94/ccxt/poloniex.py` & `ccxt-4.2.95/ccxt/poloniex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.poloniex import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class poloniex(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/poloniexfutures.py` & `ccxt-4.2.95/ccxt/poloniexfutures.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.poloniexfutures import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class poloniexfutures(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/pro/__init__.py` & `ccxt-4.2.95/ccxt/pro/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # ----------------------------------------------------------------------------
 
-__version__ = '4.2.94'
+__version__ = '4.2.95'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange  # noqa: F401
 
 # CCXT Pro exchanges (now this is mainly used for importing exchanges in WS tests)
```

### Comparing `ccxt-4.2.94/ccxt/pro/alpaca.py` & `ccxt-4.2.95/ccxt/pro/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/ascendex.py` & `ccxt-4.2.95/ccxt/pro/ascendex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheByTimestamp
 import hashlib
 from ccxt.base.types import Balances, Int, Order, OrderBook, Str, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
-from ccxt.base.errors import NetworkError
 from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import NetworkError
 
 
 class ascendex(ccxt.async_support.ascendex):
 
     def describe(self):
         return self.deep_extend(super(ascendex, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/bequant.py` & `ccxt-4.2.95/ccxt/pro/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/binance.py` & `ccxt-4.2.95/ccxt/pro/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/binancecoinm.py` & `ccxt-4.2.95/ccxt/pro/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/binanceus.py` & `ccxt-4.2.95/ccxt/pro/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/binanceusdm.py` & `ccxt-4.2.95/ccxt/pro/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/bingx.py` & `ccxt-4.2.95/ccxt/pro/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/bitcoincom.py` & `ccxt-4.2.95/ccxt/pro/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/bitfinex.py` & `ccxt-4.2.95/ccxt/pro/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/bitfinex2.py` & `ccxt-4.2.95/ccxt/pro/bitfinex2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheByTimestamp
 import hashlib
 from ccxt.base.types import Balances, Int, Order, OrderBook, Str, Ticker, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
-from ccxt.base.errors import InvalidNonce
 from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import InvalidNonce
 from ccxt.base.precise import Precise
 
 
 class bitfinex2(ccxt.async_support.bitfinex2):
 
     def describe(self):
         return self.deep_extend(super(bitfinex2, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/pro/bitget.py` & `ccxt-4.2.95/ccxt/pro/bitget.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheBySymbolBySide, ArrayCacheByTimestamp
 import hashlib
 from ccxt.base.types import Balances, Int, Order, OrderBook, Position, Str, Strings, Ticker, Tickers, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.precise import Precise
 
 
 class bitget(ccxt.async_support.bitget):
 
     def describe(self):
         return self.deep_extend(super(bitget, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/pro/bithumb.py` & `ccxt-4.2.95/ccxt/pro/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/bitmart.py` & `ccxt-4.2.95/ccxt/pro/bitmart.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheBySymbolBySide, ArrayCacheByTimestamp
 from ccxt.async_support.base.ws.order_book_side import Asks, Bids
 import hashlib
 from ccxt.base.types import Balances, Int, Market, Order, OrderBook, Position, Str, Strings, Ticker, Tickers, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import NotSupported
-from ccxt.base.errors import AuthenticationError
 
 
 class bitmart(ccxt.async_support.bitmart):
 
     def describe(self):
         return self.deep_extend(super(bitmart, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/bitmex.py` & `ccxt-4.2.95/ccxt/pro/bitmex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheBySymbolBySide, ArrayCacheByTimestamp
 import hashlib
 from ccxt.base.types import Balances, Int, Order, OrderBook, Position, Str, Strings, Ticker, Tickers, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
-from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import RateLimitExceeded
 
 
 class bitmex(ccxt.async_support.bitmex):
 
     def describe(self):
         return self.deep_extend(super(bitmex, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/bitopro.py` & `ccxt-4.2.95/ccxt/pro/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/bitrue.py` & `ccxt-4.2.95/ccxt/pro/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/bitstamp.py` & `ccxt-4.2.95/ccxt/pro/bitstamp.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById
 from ccxt.base.types import Int, Order, OrderBook, Str, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
-from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import ArgumentsRequired
 
 
 class bitstamp(ccxt.async_support.bitstamp):
 
     def describe(self):
         return self.deep_extend(super(bitstamp, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/bitvavo.py` & `ccxt-4.2.95/ccxt/pro/bitvavo.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheByTimestamp
 import hashlib
 from ccxt.base.types import Balances, Int, Num, Order, OrderBook, OrderSide, OrderType, Str, Ticker, Trade, TradingFees
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
-from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import ArgumentsRequired
 
 
 class bitvavo(ccxt.async_support.bitvavo):
 
     def describe(self):
         return self.deep_extend(super(bitvavo, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/blockchaincom.py` & `ccxt-4.2.95/ccxt/pro/blockchaincom.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheByTimestamp
 from ccxt.base.types import Balances, Int, Order, OrderBook, Str, Ticker, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
-from ccxt.base.errors import NotSupported
 from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import NotSupported
 
 
 class blockchaincom(ccxt.async_support.blockchaincom):
 
     def describe(self):
         return self.deep_extend(super(blockchaincom, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/bybit.py` & `ccxt-4.2.95/ccxt/pro/bybit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheBySymbolBySide, ArrayCacheByTimestamp
 import asyncio
 import hashlib
 from ccxt.base.types import Balances, Int, Order, OrderBook, Position, Str, Strings, Ticker, Tickers, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
-from ccxt.base.errors import AuthenticationError
 
 
 class bybit(ccxt.async_support.bybit):
 
     def describe(self):
         return self.deep_extend(super(bybit, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/cex.py` & `ccxt-4.2.95/ccxt/pro/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/coinbase.py` & `ccxt-4.2.95/ccxt/pro/coinbase.py`

 * *Files 13% similar despite different names*

```diff
@@ -178,23 +178,27 @@
                 result = self.parse_ws_ticker(ticker)
                 symbol = result['symbol']
                 self.tickers[symbol] = result
                 wsMarketId = self.safe_string(ticker, 'product_id')
                 messageHash = channel + '::' + wsMarketId
                 newTickers.append(result)
                 client.resolve(result, messageHash)
+                if messageHash.endswith('USD'):
+                    client.resolve(result, messageHash + 'C')  # sometimes we subscribe to BTC/USDC and coinbase returns BTC/USD
         messageHashes = self.find_message_hashes(client, 'ticker_batch::')
         for i in range(0, len(messageHashes)):
             messageHash = messageHashes[i]
             parts = messageHash.split('::')
             symbolsString = parts[1]
             symbols = symbolsString.split(',')
             tickers = self.filter_by_array(newTickers, 'symbol', symbols)
             if not self.is_empty(tickers):
                 client.resolve(tickers, messageHash)
+                if messageHash.endswith('USD'):
+                    client.resolve(tickers, messageHash + 'C')  # sometimes we subscribe to BTC/USDC and coinbase returns BTC/USD
         return message
 
     def parse_ws_ticker(self, ticker, market=None):
         #
         #     {
         #         "type": "ticker",
         #         "product_id": "DOGE-USD",
@@ -323,14 +327,16 @@
         for i in range(0, len(events)):
             currentEvent = events[i]
             currentTrades = self.safe_value(currentEvent, 'trades')
             for j in range(0, len(currentTrades)):
                 item = currentTrades[i]
                 tradesArray.append(self.parse_trade(item))
         client.resolve(tradesArray, messageHash)
+        if marketId.endswith('USD'):
+            client.resolve(tradesArray, messageHash + 'C')  # sometimes we subscribe to BTC/USDC and coinbase returns BTC/USD
         return message
 
     def handle_order(self, client, message):
         #
         #    {
         #        "channel": "user",
         #        "client_id": "",
@@ -374,14 +380,16 @@
                 if not (marketId in marketIds):
                     marketIds.append(marketId)
                 cachedOrders.append(parsed)
         for i in range(0, len(marketIds)):
             marketId = marketIds[i]
             messageHash = 'user::' + marketId
             client.resolve(self.orders, messageHash)
+            if messageHash.endswith('USD'):
+                client.resolve(self.orders, messageHash + 'C')  # sometimes we subscribe to BTC/USDC and coinbase returns BTC/USD
         client.resolve(self.orders, 'user')
         return message
 
     def parse_ws_order(self, order, market=None):
         #
         #    {
         #        "order_id": "XXX",
@@ -484,21 +492,25 @@
                 self.orderbooks[symbol] = self.order_book({}, limit)
                 orderbook = self.orderbooks[symbol]
                 self.handle_order_book_helper(orderbook, updates)
                 orderbook['timestamp'] = None
                 orderbook['datetime'] = None
                 orderbook['symbol'] = symbol
                 client.resolve(orderbook, messageHash)
+                if messageHash.endswith('USD'):
+                    client.resolve(orderbook, messageHash + 'C')  # sometimes we subscribe to BTC/USDC and coinbase returns BTC/USD
             elif type == 'update':
                 orderbook = self.orderbooks[symbol]
                 self.handle_order_book_helper(orderbook, updates)
                 orderbook['datetime'] = datetime
                 orderbook['timestamp'] = self.parse8601(datetime)
                 orderbook['symbol'] = symbol
                 client.resolve(orderbook, messageHash)
+                if messageHash.endswith('USD'):
+                    client.resolve(orderbook, messageHash + 'C')  # sometimes we subscribe to BTC/USDC and coinbase returns BTC/USD
         return message
 
     def handle_subscription_status(self, client, message):
         #
         #     {
         #         "type": "subscriptions",
         #         "channels": [
```

### Comparing `ccxt-4.2.94/ccxt/pro/coinbaseinternational.py` & `ccxt-4.2.95/ccxt/pro/coinbaseinternational.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache
 import hashlib
 from ccxt.base.types import Int, Market, OrderBook, Strings, Ticker, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
-from ccxt.base.errors import NotSupported
 from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import NotSupported
 
 
 class coinbaseinternational(ccxt.async_support.coinbaseinternational):
 
     def describe(self):
         return self.deep_extend(super(coinbaseinternational, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/coinbasepro.py` & `ccxt-4.2.95/ccxt/pro/coinbasepro.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById
 import hashlib
 from ccxt.base.types import Int, Order, OrderBook, Str, Strings, Ticker, Tickers, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
-from ccxt.base.errors import AuthenticationError
 
 
 class coinbasepro(ccxt.async_support.coinbasepro):
 
     def describe(self):
         return self.deep_extend(super(coinbasepro, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/coincheck.py` & `ccxt-4.2.95/ccxt/pro/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/coinex.py` & `ccxt-4.2.95/ccxt/pro/coinex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheByTimestamp
 from ccxt.base.types import Balances, Int, Order, OrderBook, Str, Strings, Ticker, Tickers, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import RequestTimeout
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.precise import Precise
 
 
 class coinex(ccxt.async_support.coinex):
 
     def describe(self):
         return self.deep_extend(super(coinex, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/pro/coinone.py` & `ccxt-4.2.95/ccxt/pro/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/cryptocom.py` & `ccxt-4.2.95/ccxt/pro/cryptocom.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheBySymbolBySide, ArrayCacheByTimestamp
 import hashlib
 from ccxt.base.types import Balances, Int, Num, Order, OrderBook, OrderSide, OrderType, Position, Str, Strings, Ticker, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 
 
 class cryptocom(ccxt.async_support.cryptocom):
 
     def describe(self):
         return self.deep_extend(super(cryptocom, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/currencycom.py` & `ccxt-4.2.95/ccxt/pro/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/deribit.py` & `ccxt-4.2.95/ccxt/pro/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/exmo.py` & `ccxt-4.2.95/ccxt/pro/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/gate.py` & `ccxt-4.2.95/ccxt/pro/gate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheBySymbolBySide, ArrayCacheByTimestamp
 import hashlib
 from ccxt.base.types import Balances, Int, Order, OrderBook, Position, Str, Strings, Ticker, Tickers, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 
 
 class gate(ccxt.async_support.gate):
 
     def describe(self):
         return self.deep_extend(super(gate, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/gemini.py` & `ccxt-4.2.95/ccxt/pro/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/hitbtc.py` & `ccxt-4.2.95/ccxt/pro/hitbtc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheByTimestamp
 import hashlib
 from ccxt.base.types import Balances, Int, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
-from ccxt.base.errors import NotSupported
 from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import NotSupported
 
 
 class hitbtc(ccxt.async_support.hitbtc):
 
     def describe(self):
         return self.deep_extend(super(hitbtc, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/hollaex.py` & `ccxt-4.2.95/ccxt/pro/hollaex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById
 import hashlib
 from ccxt.base.types import Balances, Int, Order, OrderBook, Str, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
-from ccxt.base.errors import AuthenticationError
 
 
 class hollaex(ccxt.async_support.hollaex):
 
     def describe(self):
         return self.deep_extend(super(hollaex, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/htx.py` & `ccxt-4.2.95/ccxt/pro/htx.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheBySymbolBySide, ArrayCacheByTimestamp
 import hashlib
 from ccxt.base.types import Balances, Int, Order, OrderBook, Position, Str, Strings, Ticker, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 
 
 class htx(ccxt.async_support.htx):
 
     def describe(self):
         return self.deep_extend(super(htx, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/huobijp.py` & `ccxt-4.2.95/ccxt/pro/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/hyperliquid.py` & `ccxt-4.2.95/ccxt/pro/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/idex.py` & `ccxt-4.2.95/ccxt/pro/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/independentreserve.py` & `ccxt-4.2.95/ccxt/pro/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/kraken.py` & `ccxt-4.2.95/ccxt/pro/kraken.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheByTimestamp
 from ccxt.base.types import Int, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.precise import Precise
 
 
 class kraken(ccxt.async_support.kraken):
 
     def describe(self):
         return self.deep_extend(super(kraken, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/pro/krakenfutures.py` & `ccxt-4.2.95/ccxt/pro/krakenfutures.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById
 import hashlib
 from ccxt.base.types import Balances, Int, Order, OrderBook, Position, Str, Strings, Ticker, Tickers, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
-from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.precise import Precise
 
 
 class krakenfutures(ccxt.async_support.krakenfutures):
 
     def describe(self):
         return self.deep_extend(super(krakenfutures, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/pro/kucoin.py` & `ccxt-4.2.95/ccxt/pro/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/kucoinfutures.py` & `ccxt-4.2.95/ccxt/pro/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/lbank.py` & `ccxt-4.2.95/ccxt/pro/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/luno.py` & `ccxt-4.2.95/ccxt/pro/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/mexc.py` & `ccxt-4.2.95/ccxt/pro/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/ndax.py` & `ccxt-4.2.95/ccxt/pro/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/okcoin.py` & `ccxt-4.2.95/ccxt/pro/okcoin.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheByTimestamp
 import hashlib
 from ccxt.base.types import Balances, Int, Order, OrderBook, Str, Ticker, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
-from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import ArgumentsRequired
 
 
 class okcoin(ccxt.async_support.okcoin):
 
     def describe(self):
         return self.deep_extend(super(okcoin, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/okx.py` & `ccxt-4.2.95/ccxt/pro/okx.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheBySymbolBySide, ArrayCacheByTimestamp
 import hashlib
 from ccxt.base.types import Balances, Int, Num, Order, OrderBook, OrderSide, OrderType, Position, Str, Strings, Ticker, Tickers, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 
 
 class okx(ccxt.async_support.okx):
 
     def describe(self):
         return self.deep_extend(super(okx, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/onetrading.py` & `ccxt-4.2.95/ccxt/pro/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/p2b.py` & `ccxt-4.2.95/ccxt/pro/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/phemex.py` & `ccxt-4.2.95/ccxt/pro/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/poloniex.py` & `ccxt-4.2.95/ccxt/pro/poloniex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheByTimestamp
 import hashlib
 from ccxt.base.types import Balances, Int, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InvalidOrder
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.precise import Precise
 
 
 class poloniex(ccxt.async_support.poloniex):
 
     def describe(self):
         return self.deep_extend(super(poloniex, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/pro/poloniexfutures.py` & `ccxt-4.2.95/ccxt/pro/poloniexfutures.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById
 from ccxt.base.types import Balances, Int, Order, OrderBook, Str, Ticker, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
 from ccxt.base.errors import ExchangeError
-from ccxt.base.errors import BadRequest
 from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import BadRequest
 
 
 class poloniexfutures(ccxt.async_support.poloniexfutures):
 
     def describe(self):
         return self.deep_extend(super(poloniexfutures, self).describe(), {
             'has': {
```

### Comparing `ccxt-4.2.94/ccxt/pro/probit.py` & `ccxt-4.2.95/ccxt/pro/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/upbit.py` & `ccxt-4.2.95/ccxt/pro/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/wazirx.py` & `ccxt-4.2.95/ccxt/pro/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/pro/whitebit.py` & `ccxt-4.2.95/ccxt/pro/whitebit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 import ccxt.async_support
 from ccxt.async_support.base.ws.cache import ArrayCache, ArrayCacheBySymbolById, ArrayCacheByTimestamp
 from ccxt.base.types import Balances, Int, Order, OrderBook, Str, Ticker, Trade
 from ccxt.async_support.base.ws.client import Client
 from typing import List
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.precise import Precise
 
 
 class whitebit(ccxt.async_support.whitebit):
 
     def describe(self):
         return self.deep_extend(super(whitebit, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/pro/woo.py` & `ccxt-4.2.95/ccxt/pro/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/probit.py` & `ccxt-4.2.95/ccxt/probit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.probit import ImplicitAPI
 import math
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import BadResponse
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidAddress
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TRUNCATE
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class probit(Exchange, ImplicitAPI):
```

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ecdsa/__init__.py` & `ccxt-4.2.95/ccxt/static_dependencies/ecdsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ecdsa/_version.py` & `ccxt-4.2.95/ccxt/static_dependencies/ecdsa/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ecdsa/curves.py` & `ccxt-4.2.95/ccxt/static_dependencies/ecdsa/curves.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ecdsa/der.py` & `ccxt-4.2.95/ccxt/static_dependencies/ecdsa/der.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ecdsa/ecdsa.py` & `ccxt-4.2.95/ccxt/static_dependencies/ecdsa/ecdsa.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ecdsa/ellipticcurve.py` & `ccxt-4.2.95/ccxt/static_dependencies/ecdsa/ellipticcurve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ecdsa/keys.py` & `ccxt-4.2.95/ccxt/static_dependencies/ecdsa/keys.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ecdsa/numbertheory.py` & `ccxt-4.2.95/ccxt/static_dependencies/ecdsa/numbertheory.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ecdsa/rfc6979.py` & `ccxt-4.2.95/ccxt/static_dependencies/ecdsa/rfc6979.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ecdsa/util.py` & `ccxt-4.2.95/ccxt/static_dependencies/ecdsa/util.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/base.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/base.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/codec.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/codec.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/decoding.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/decoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/encoding.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/encoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/exceptions.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/grammar.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/registry.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/registry.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/abi/utils/numeric.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/abi/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/account/messages.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/account/messages.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/hexbytes/_utils.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/hexbytes/_utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/hexbytes/main.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/hexbytes/main.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/__init__.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/evm.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/evm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/typing/networks.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/typing/networks.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/__init__.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/abi.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/abi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/address.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/address.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/applicators.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/applicators.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/conversions.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/currency.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/curried/__init__.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/decorators.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/functional.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/functional.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/hexadecimal.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/humanize.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/logging.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/module_loading.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/numeric.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/toolz.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/toolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/types.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/ethereum/utils/units.py` & `ccxt-4.2.95/ccxt/static_dependencies/ethereum/utils/units.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/keccak/keccak.py` & `ccxt-4.2.95/ccxt/static_dependencies/keccak/keccak.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/msgpack/__init__.py` & `ccxt-4.2.95/ccxt/static_dependencies/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/msgpack/exceptions.py` & `ccxt-4.2.95/ccxt/static_dependencies/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/msgpack/ext.py` & `ccxt-4.2.95/ccxt/static_dependencies/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/msgpack/fallback.py` & `ccxt-4.2.95/ccxt/static_dependencies/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/parsimonious/exceptions.py` & `ccxt-4.2.95/ccxt/static_dependencies/parsimonious/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/parsimonious/expressions.py` & `ccxt-4.2.95/ccxt/static_dependencies/parsimonious/expressions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/parsimonious/grammar.py` & `ccxt-4.2.95/ccxt/static_dependencies/parsimonious/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/parsimonious/nodes.py` & `ccxt-4.2.95/ccxt/static_dependencies/parsimonious/nodes.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/parsimonious/utils.py` & `ccxt-4.2.95/ccxt/static_dependencies/parsimonious/utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/toolz/_signatures.py` & `ccxt-4.2.95/ccxt/static_dependencies/toolz/_signatures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/toolz/_version.py` & `ccxt-4.2.95/ccxt/static_dependencies/toolz/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/toolz/compatibility.py` & `ccxt-4.2.95/ccxt/static_dependencies/toolz/compatibility.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/toolz/curried/__init__.py` & `ccxt-4.2.95/ccxt/static_dependencies/toolz/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/toolz/curried/operator.py` & `ccxt-4.2.95/ccxt/static_dependencies/toolz/curried/operator.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/toolz/dicttoolz.py` & `ccxt-4.2.95/ccxt/static_dependencies/toolz/dicttoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/toolz/functoolz.py` & `ccxt-4.2.95/ccxt/static_dependencies/toolz/functoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/toolz/itertoolz.py` & `ccxt-4.2.95/ccxt/static_dependencies/toolz/itertoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/static_dependencies/toolz/recipes.py` & `ccxt-4.2.95/ccxt/static_dependencies/toolz/recipes.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/__init__.py` & `ccxt-4.2.95/ccxt/test/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_account.py` & `ccxt-4.2.95/ccxt/test/base/test_account.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_balance.py` & `ccxt-4.2.95/ccxt/test/base/test_balance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_borrow_interest.py` & `ccxt-4.2.95/ccxt/test/base/test_borrow_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_borrow_rate.py` & `ccxt-4.2.95/ccxt/test/base/test_borrow_rate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_calculate_fee.py` & `ccxt-4.2.95/ccxt/test/base/test_calculate_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_crypto.py` & `ccxt-4.2.95/ccxt/test/base/test_crypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_currency.py` & `ccxt-4.2.95/ccxt/test/base/test_currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_datetime.py` & `ccxt-4.2.95/ccxt/test/base/test_datetime.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_decimal_to_precision.py` & `ccxt-4.2.95/ccxt/test/base/test_decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_deep_extend.py` & `ccxt-4.2.95/ccxt/test/base/test_deep_extend.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_deposit_withdrawal.py` & `ccxt-4.2.95/ccxt/test/base/test_deposit_withdrawal.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_exchange_datetime_functions.py` & `ccxt-4.2.95/ccxt/test/base/test_exchange_datetime_functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_funding_rate_history.py` & `ccxt-4.2.95/ccxt/test/base/test_funding_rate_history.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_last_price.py` & `ccxt-4.2.95/ccxt/test/base/test_last_price.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_ledger_entry.py` & `ccxt-4.2.95/ccxt/test/base/test_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_ledger_item.py` & `ccxt-4.2.95/ccxt/test/base/test_ledger_item.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_leverage_tier.py` & `ccxt-4.2.95/ccxt/test/base/test_leverage_tier.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_margin_mode.py` & `ccxt-4.2.95/ccxt/test/base/test_margin_mode.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_margin_modification.py` & `ccxt-4.2.95/ccxt/test/base/test_margin_modification.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_market.py` & `ccxt-4.2.95/ccxt/test/base/test_market.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_number.py` & `ccxt-4.2.95/ccxt/test/base/test_number.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_ohlcv.py` & `ccxt-4.2.95/ccxt/test/base/test_ohlcv.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_open_interest.py` & `ccxt-4.2.95/ccxt/test/base/test_open_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_order.py` & `ccxt-4.2.95/ccxt/test/base/test_order.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_order_book.py` & `ccxt-4.2.95/ccxt/test/base/test_order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_position.py` & `ccxt-4.2.95/ccxt/test/base/test_position.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_shared_methods.py` & `ccxt-4.2.95/ccxt/test/base/test_shared_methods.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_status.py` & `ccxt-4.2.95/ccxt/test/base/test_status.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_throttle.py` & `ccxt-4.2.95/ccxt/test/base/test_throttle.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_ticker.py` & `ccxt-4.2.95/ccxt/test/base/test_ticker.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_trade.py` & `ccxt-4.2.95/ccxt/test/base/test_trade.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_trading_fee.py` & `ccxt-4.2.95/ccxt/test/base/test_trading_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/base/test_transaction.py` & `ccxt-4.2.95/ccxt/test/base/test_transaction.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/test_async.py` & `ccxt-4.2.95/ccxt/test/test_async.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/test/test_sync.py` & `ccxt-4.2.95/ccxt/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/timex.py` & `ccxt-4.2.95/ccxt/timex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.timex import ImplicitAPI
 from ccxt.base.types import Balances, Currencies, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class timex(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/tokocrypto.py` & `ccxt-4.2.95/ccxt/tokocrypto.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,69 +28,69 @@
 000001b0: 2c20 5472 6164 652c 2054 7261 6e73 6163  , Trade, Transac
 000001c0: 7469 6f6e 0a66 726f 6d20 7479 7069 6e67  tion.from typing
 000001d0: 2069 6d70 6f72 7420 4c69 7374 0a66 726f   import List.fro
 000001e0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
 000001f0: 7273 2069 6d70 6f72 7420 4578 6368 616e  rs import Exchan
 00000200: 6765 4572 726f 720a 6672 6f6d 2063 6378  geError.from ccx
 00000210: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
-00000220: 706f 7274 2050 6572 6d69 7373 696f 6e44  port PermissionD
-00000230: 656e 6965 640a 6672 6f6d 2063 6378 742e  enied.from ccxt.
-00000240: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-00000250: 7274 2041 6363 6f75 6e74 5375 7370 656e  rt AccountSuspen
-00000260: 6465 640a 6672 6f6d 2063 6378 742e 6261  ded.from ccxt.ba
-00000270: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000280: 2041 7267 756d 656e 7473 5265 7175 6972   ArgumentsRequir
-00000290: 6564 0a66 726f 6d20 6363 7874 2e62 6173  ed.from ccxt.bas
-000002a0: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
-000002b0: 4261 6452 6571 7565 7374 0a66 726f 6d20  BadRequest.from 
-000002c0: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-000002d0: 2069 6d70 6f72 7420 4261 6453 796d 626f   import BadSymbo
-000002e0: 6c0a 6672 6f6d 2063 6378 742e 6261 7365  l.from ccxt.base
-000002f0: 2e65 7272 6f72 7320 696d 706f 7274 204d  .errors import M
-00000300: 6172 6769 6e4d 6f64 6541 6c72 6561 6479  arginModeAlready
-00000310: 5365 740a 6672 6f6d 2063 6378 742e 6261  Set.from ccxt.ba
-00000320: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000330: 2042 6164 5265 7370 6f6e 7365 0a66 726f   BadResponse.fro
-00000340: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-00000350: 7273 2069 6d70 6f72 7420 496e 7375 6666  rs import Insuff
-00000360: 6963 6965 6e74 4675 6e64 730a 6672 6f6d  icientFunds.from
-00000370: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-00000380: 7320 696d 706f 7274 2049 6e76 616c 6964  s import Invalid
-00000390: 4f72 6465 720a 6672 6f6d 2063 6378 742e  Order.from ccxt.
-000003a0: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
-000003b0: 7274 204f 7264 6572 4e6f 7446 6f75 6e64  rt OrderNotFound
-000003c0: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-000003d0: 6572 726f 7273 2069 6d70 6f72 7420 4f72  errors import Or
-000003e0: 6465 7249 6d6d 6564 6961 7465 6c79 4669  derImmediatelyFi
-000003f0: 6c6c 6162 6c65 0a66 726f 6d20 6363 7874  llable.from ccxt
-00000400: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000410: 6f72 7420 4f72 6465 724e 6f74 4669 6c6c  ort OrderNotFill
-00000420: 6162 6c65 0a66 726f 6d20 6363 7874 2e62  able.from ccxt.b
-00000430: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
-00000440: 7420 4e6f 7453 7570 706f 7274 6564 0a66  t NotSupported.f
-00000450: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-00000460: 726f 7273 2069 6d70 6f72 7420 4444 6f53  rors import DDoS
-00000470: 5072 6f74 6563 7469 6f6e 0a66 726f 6d20  Protection.from 
-00000480: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
-00000490: 2069 6d70 6f72 7420 5261 7465 4c69 6d69   import RateLimi
-000004a0: 7445 7863 6565 6465 640a 6672 6f6d 2063  tExceeded.from c
-000004b0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-000004c0: 696d 706f 7274 2045 7863 6861 6e67 654e  import ExchangeN
-000004d0: 6f74 4176 6169 6c61 626c 650a 6672 6f6d  otAvailable.from
-000004e0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-000004f0: 7320 696d 706f 7274 204f 6e4d 6169 6e74  s import OnMaint
-00000500: 656e 616e 6365 0a66 726f 6d20 6363 7874  enance.from ccxt
-00000510: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
-00000520: 6f72 7420 496e 7661 6c69 644e 6f6e 6365  ort InvalidNonce
-00000530: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-00000540: 6572 726f 7273 2069 6d70 6f72 7420 5265  errors import Re
-00000550: 7175 6573 7454 696d 656f 7574 0a66 726f  questTimeout.fro
-00000560: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
-00000570: 7273 2069 6d70 6f72 7420 4175 7468 656e  rs import Authen
-00000580: 7469 6361 7469 6f6e 4572 726f 720a 6672  ticationError.fr
+00000220: 706f 7274 2041 7574 6865 6e74 6963 6174  port Authenticat
+00000230: 696f 6e45 7272 6f72 0a66 726f 6d20 6363  ionError.from cc
+00000240: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
+00000250: 6d70 6f72 7420 5065 726d 6973 7369 6f6e  mport Permission
+00000260: 4465 6e69 6564 0a66 726f 6d20 6363 7874  Denied.from ccxt
+00000270: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+00000280: 6f72 7420 4163 636f 756e 7453 7573 7065  ort AccountSuspe
+00000290: 6e64 6564 0a66 726f 6d20 6363 7874 2e62  nded.from ccxt.b
+000002a0: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+000002b0: 7420 4172 6775 6d65 6e74 7352 6571 7569  t ArgumentsRequi
+000002c0: 7265 640a 6672 6f6d 2063 6378 742e 6261  red.from ccxt.ba
+000002d0: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
+000002e0: 2042 6164 5265 7175 6573 740a 6672 6f6d   BadRequest.from
+000002f0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+00000300: 7320 696d 706f 7274 2042 6164 5379 6d62  s import BadSymb
+00000310: 6f6c 0a66 726f 6d20 6363 7874 2e62 6173  ol.from ccxt.bas
+00000320: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+00000330: 4d61 7267 696e 4d6f 6465 416c 7265 6164  MarginModeAlread
+00000340: 7953 6574 0a66 726f 6d20 6363 7874 2e62  ySet.from ccxt.b
+00000350: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+00000360: 7420 4261 6452 6573 706f 6e73 650a 6672  t BadResponse.fr
+00000370: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
+00000380: 6f72 7320 696d 706f 7274 2049 6e73 7566  ors import Insuf
+00000390: 6669 6369 656e 7446 756e 6473 0a66 726f  ficientFunds.fro
+000003a0: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+000003b0: 7273 2069 6d70 6f72 7420 496e 7661 6c69  rs import Invali
+000003c0: 644f 7264 6572 0a66 726f 6d20 6363 7874  dOrder.from ccxt
+000003d0: 2e62 6173 652e 6572 726f 7273 2069 6d70  .base.errors imp
+000003e0: 6f72 7420 4f72 6465 724e 6f74 466f 756e  ort OrderNotFoun
+000003f0: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
+00000400: 2e65 7272 6f72 7320 696d 706f 7274 204f  .errors import O
+00000410: 7264 6572 496d 6d65 6469 6174 656c 7946  rderImmediatelyF
+00000420: 696c 6c61 626c 650a 6672 6f6d 2063 6378  illable.from ccx
+00000430: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+00000440: 706f 7274 204f 7264 6572 4e6f 7446 696c  port OrderNotFil
+00000450: 6c61 626c 650a 6672 6f6d 2063 6378 742e  lable.from ccxt.
+00000460: 6261 7365 2e65 7272 6f72 7320 696d 706f  base.errors impo
+00000470: 7274 204e 6f74 5375 7070 6f72 7465 640a  rt NotSupported.
+00000480: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+00000490: 7272 6f72 7320 696d 706f 7274 2044 446f  rrors import DDo
+000004a0: 5350 726f 7465 6374 696f 6e0a 6672 6f6d  SProtection.from
+000004b0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
+000004c0: 7320 696d 706f 7274 2052 6174 654c 696d  s import RateLim
+000004d0: 6974 4578 6365 6564 6564 0a66 726f 6d20  itExceeded.from 
+000004e0: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
+000004f0: 2069 6d70 6f72 7420 4578 6368 616e 6765   import Exchange
+00000500: 4e6f 7441 7661 696c 6162 6c65 0a66 726f  NotAvailable.fro
+00000510: 6d20 6363 7874 2e62 6173 652e 6572 726f  m ccxt.base.erro
+00000520: 7273 2069 6d70 6f72 7420 4f6e 4d61 696e  rs import OnMain
+00000530: 7465 6e61 6e63 650a 6672 6f6d 2063 6378  tenance.from ccx
+00000540: 742e 6261 7365 2e65 7272 6f72 7320 696d  t.base.errors im
+00000550: 706f 7274 2049 6e76 616c 6964 4e6f 6e63  port InvalidNonc
+00000560: 650a 6672 6f6d 2063 6378 742e 6261 7365  e.from ccxt.base
+00000570: 2e65 7272 6f72 7320 696d 706f 7274 2052  .errors import R
+00000580: 6571 7565 7374 5469 6d65 6f75 740a 6672  equestTimeout.fr
 00000590: 6f6d 2063 6378 742e 6261 7365 2e64 6563  om ccxt.base.dec
 000005a0: 696d 616c 5f74 6f5f 7072 6563 6973 696f  imal_to_precisio
 000005b0: 6e20 696d 706f 7274 2054 5255 4e43 4154  n import TRUNCAT
 000005c0: 450a 6672 6f6d 2063 6378 742e 6261 7365  E.from ccxt.base
 000005d0: 2e64 6563 696d 616c 5f74 6f5f 7072 6563  .decimal_to_prec
 000005e0: 6973 696f 6e20 696d 706f 7274 2044 4543  ision import DEC
 000005f0: 494d 414c 5f50 4c41 4345 530a 6672 6f6d  IMAL_PLACES.from
```

### Comparing `ccxt-4.2.94/ccxt/tradeogre.py` & `ccxt-4.2.95/ccxt/tradeogre.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.tradeogre import ImplicitAPI
 from ccxt.base.types import IndexType, Int, Market, Num, Order, OrderSide, OrderType, Str, Ticker
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 
 
 class tradeogre(Exchange, ImplicitAPI):
 
     def describe(self):
         return self.deep_extend(super(tradeogre, self).describe(), {
```

### Comparing `ccxt-4.2.94/ccxt/upbit.py` & `ccxt-4.2.95/ccxt/upbit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.upbit import ImplicitAPI
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, Transaction
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InsufficientFunds
+from ccxt.base.errors import AddressPending
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
-from ccxt.base.errors import AuthenticationError
-from ccxt.base.errors import AddressPending
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class upbit(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/wavesexchange.py` & `ccxt-4.2.95/ccxt/wavesexchange.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.wavesexchange import ImplicitAPI
 import json
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction
 from typing import List
 from typing import Any
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import DuplicateOrderId
 from ccxt.base.errors import ExchangeNotAvailable
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import DECIMAL_PLACES
 from ccxt.base.precise import Precise
 
 
 class wavesexchange(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/wazirx.py` & `ccxt-4.2.95/ccxt/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/whitebit.py` & `ccxt-4.2.95/ccxt/whitebit.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,43 +31,43 @@
 000001e0: 6e2c 2054 7261 6e73 6665 7245 6e74 7279  n, TransferEntry
 000001f0: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
 00000200: 6f72 7420 4c69 7374 0a66 726f 6d20 6363  ort List.from cc
 00000210: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
 00000220: 6d70 6f72 7420 4578 6368 616e 6765 4572  mport ExchangeEr
 00000230: 726f 720a 6672 6f6d 2063 6378 742e 6261  ror.from ccxt.ba
 00000240: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000250: 2050 6572 6d69 7373 696f 6e44 656e 6965   PermissionDenie
-00000260: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
-00000270: 2e65 7272 6f72 7320 696d 706f 7274 2041  .errors import A
-00000280: 7267 756d 656e 7473 5265 7175 6972 6564  rgumentsRequired
-00000290: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
-000002a0: 6572 726f 7273 2069 6d70 6f72 7420 4261  errors import Ba
-000002b0: 6452 6571 7565 7374 0a66 726f 6d20 6363  dRequest.from cc
-000002c0: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
-000002d0: 6d70 6f72 7420 4261 6453 796d 626f 6c0a  mport BadSymbol.
-000002e0: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
-000002f0: 7272 6f72 7320 696d 706f 7274 2049 6e73  rrors import Ins
-00000300: 7566 6669 6369 656e 7446 756e 6473 0a66  ufficientFunds.f
-00000310: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
-00000320: 726f 7273 2069 6d70 6f72 7420 496e 7661  rors import Inva
-00000330: 6c69 644f 7264 6572 0a66 726f 6d20 6363  lidOrder.from cc
-00000340: 7874 2e62 6173 652e 6572 726f 7273 2069  xt.base.errors i
-00000350: 6d70 6f72 7420 4f72 6465 724e 6f74 466f  mport OrderNotFo
-00000360: 756e 640a 6672 6f6d 2063 6378 742e 6261  und.from ccxt.ba
-00000370: 7365 2e65 7272 6f72 7320 696d 706f 7274  se.errors import
-00000380: 204e 6f74 5375 7070 6f72 7465 640a 6672   NotSupported.fr
-00000390: 6f6d 2063 6378 742e 6261 7365 2e65 7272  om ccxt.base.err
-000003a0: 6f72 7320 696d 706f 7274 2044 446f 5350  ors import DDoSP
-000003b0: 726f 7465 6374 696f 6e0a 6672 6f6d 2063  rotection.from c
-000003c0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
-000003d0: 696d 706f 7274 2045 7863 6861 6e67 654e  import ExchangeN
-000003e0: 6f74 4176 6169 6c61 626c 650a 6672 6f6d  otAvailable.from
-000003f0: 2063 6378 742e 6261 7365 2e65 7272 6f72   ccxt.base.error
-00000400: 7320 696d 706f 7274 2041 7574 6865 6e74  s import Authent
-00000410: 6963 6174 696f 6e45 7272 6f72 0a66 726f  icationError.fro
+00000250: 2041 7574 6865 6e74 6963 6174 696f 6e45   AuthenticationE
+00000260: 7272 6f72 0a66 726f 6d20 6363 7874 2e62  rror.from ccxt.b
+00000270: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+00000280: 7420 5065 726d 6973 7369 6f6e 4465 6e69  t PermissionDeni
+00000290: 6564 0a66 726f 6d20 6363 7874 2e62 6173  ed.from ccxt.bas
+000002a0: 652e 6572 726f 7273 2069 6d70 6f72 7420  e.errors import 
+000002b0: 4172 6775 6d65 6e74 7352 6571 7569 7265  ArgumentsRequire
+000002c0: 640a 6672 6f6d 2063 6378 742e 6261 7365  d.from ccxt.base
+000002d0: 2e65 7272 6f72 7320 696d 706f 7274 2042  .errors import B
+000002e0: 6164 5265 7175 6573 740a 6672 6f6d 2063  adRequest.from c
+000002f0: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+00000300: 696d 706f 7274 2042 6164 5379 6d62 6f6c  import BadSymbol
+00000310: 0a66 726f 6d20 6363 7874 2e62 6173 652e  .from ccxt.base.
+00000320: 6572 726f 7273 2069 6d70 6f72 7420 496e  errors import In
+00000330: 7375 6666 6963 6965 6e74 4675 6e64 730a  sufficientFunds.
+00000340: 6672 6f6d 2063 6378 742e 6261 7365 2e65  from ccxt.base.e
+00000350: 7272 6f72 7320 696d 706f 7274 2049 6e76  rrors import Inv
+00000360: 616c 6964 4f72 6465 720a 6672 6f6d 2063  alidOrder.from c
+00000370: 6378 742e 6261 7365 2e65 7272 6f72 7320  cxt.base.errors 
+00000380: 696d 706f 7274 204f 7264 6572 4e6f 7446  import OrderNotF
+00000390: 6f75 6e64 0a66 726f 6d20 6363 7874 2e62  ound.from ccxt.b
+000003a0: 6173 652e 6572 726f 7273 2069 6d70 6f72  ase.errors impor
+000003b0: 7420 4e6f 7453 7570 706f 7274 6564 0a66  t NotSupported.f
+000003c0: 726f 6d20 6363 7874 2e62 6173 652e 6572  rom ccxt.base.er
+000003d0: 726f 7273 2069 6d70 6f72 7420 4444 6f53  rors import DDoS
+000003e0: 5072 6f74 6563 7469 6f6e 0a66 726f 6d20  Protection.from 
+000003f0: 6363 7874 2e62 6173 652e 6572 726f 7273  ccxt.base.errors
+00000400: 2069 6d70 6f72 7420 4578 6368 616e 6765   import Exchange
+00000410: 4e6f 7441 7661 696c 6162 6c65 0a66 726f  NotAvailable.fro
 00000420: 6d20 6363 7874 2e62 6173 652e 6465 6369  m ccxt.base.deci
 00000430: 6d61 6c5f 746f 5f70 7265 6369 7369 6f6e  mal_to_precision
 00000440: 2069 6d70 6f72 7420 5449 434b 5f53 495a   import TICK_SIZ
 00000450: 450a 6672 6f6d 2063 6378 742e 6261 7365  E.from ccxt.base
 00000460: 2e70 7265 6369 7365 2069 6d70 6f72 7420  .precise import 
 00000470: 5072 6563 6973 650a 0a0a 636c 6173 7320  Precise...class 
 00000480: 7768 6974 6562 6974 2845 7863 6861 6e67  whitebit(Exchang
```

### Comparing `ccxt-4.2.94/ccxt/woo.py` & `ccxt-4.2.95/ccxt/woo.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.woo import ImplicitAPI
 import hashlib
 from ccxt.base.types import Account, Balances, Bool, Conversion, Currencies, Currency, Int, Leverage, Market, MarketType, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Trade, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import OnMaintenance
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class woo(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/yobit.py` & `ccxt-4.2.95/ccxt/yobit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.yobit import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, TradingFees
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import DDoSProtection
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import ExchangeNotAvailable
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class yobit(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt/zaif.py` & `ccxt-4.2.95/ccxt/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/ccxt/zonda.py` & `ccxt-4.2.95/ccxt/zonda.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.zonda import ImplicitAPI
 import hashlib
 from ccxt.base.types import Balances, Currency, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
 from ccxt.base.errors import InvalidOrder
 from ccxt.base.errors import OrderNotFound
 from ccxt.base.errors import OrderImmediatelyFillable
 from ccxt.base.errors import RateLimitExceeded
 from ccxt.base.errors import OnMaintenance
 from ccxt.base.errors import InvalidNonce
-from ccxt.base.errors import AuthenticationError
 from ccxt.base.decimal_to_precision import TICK_SIZE
 from ccxt.base.precise import Precise
 
 
 class zonda(Exchange, ImplicitAPI):
 
     def describe(self):
```

### Comparing `ccxt-4.2.94/ccxt.egg-info/PKG-INFO` & `ccxt-4.2.95/ccxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 4.2.94
+Version: 4.2.95
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 100+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
@@ -221,21 +221,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.2.94/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@4.2.94/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.2.95/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@4.2.95/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.2.94/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.2.95/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-4.2.94/ccxt.egg-info/SOURCES.txt` & `ccxt-4.2.95/ccxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.94/package.json` & `ccxt-4.2.95/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'4.2.95'"}*

```diff
@@ -265,9 +265,9 @@
         "update-links": "node build/update-links",
         "validate-types": "node --loader ts-node/esm build/validate-types.ts",
         "vss": "node build/vss"
     },
     "type": "module",
     "types": "./js/ccxt.d.ts",
     "unpkg": "dist/ccxt.browser.js",
-    "version": "4.2.94"
+    "version": "4.2.95"
 }
```

### Comparing `ccxt-4.2.94/setup.py` & `ccxt-4.2.95/setup.py`

 * *Files identical despite different names*

