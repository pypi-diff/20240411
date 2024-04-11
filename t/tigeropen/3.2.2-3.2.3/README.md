# Comparing `tmp/tigeropen-3.2.2.tar.gz` & `tmp/tigeropen-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigeropen-3.2.2.tar", last modified: Tue Apr  9 13:07:53 2024, max compression
+gzip compressed data, was "tigeropen-3.2.3.tar", last modified: Thu Apr 11 02:46:44 2024, max compression
```

## Comparing `tigeropen-3.2.2.tar` & `tigeropen-3.2.3.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.523949 tigeropen-3.2.2/
--rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-3.2.2/MANIFEST.in
--rw-r--r--   0 sukai      (501) staff       (20)     7120 2024-04-09 13:07:53.523661 tigeropen-3.2.2/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-3.2.2/README.md
--rw-r--r--   0 sukai      (501) staff       (20)      137 2024-02-27 08:47:04.000000 tigeropen-3.2.2/requirements.txt
--rw-r--r--   0 sukai      (501) staff       (20)       38 2024-04-09 13:07:53.524017 tigeropen-3.2.2/setup.cfg
--rw-r--r--   0 sukai      (501) staff       (20)     1358 2024-01-19 03:27:35.000000 tigeropen-3.2.2/setup.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.472174 tigeropen-3.2.2/tests/
--rw-r--r--   0 sukai      (501) staff       (20)     2628 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tests/test_client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)     2589 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tests/test_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     2856 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tests/test_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.472872 tigeropen-3.2.2/tigeropen/
--rw-r--r--   0 sukai      (501) staff       (20)       91 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.475213 tigeropen-3.2.2/tigeropen/common/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/common/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.477883 tigeropen-3.2.2/tigeropen/common/consts/
--rw-r--r--   0 sukai      (501) staff       (20)     5171 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/common/consts/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    19289 2024-02-27 08:46:55.000000 tigeropen-3.2.2/tigeropen/common/consts/filter_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)    39797 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/common/consts/fundamental_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-3.2.2/tigeropen/common/consts/params.py
--rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/common/consts/push_destinations.py
--rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/common/consts/push_subscriptions.py
--rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/common/consts/push_types.py
--rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-3.2.2/tigeropen/common/consts/quote_keys.py
--rw-r--r--   0 sukai      (501) staff       (20)     3305 2024-04-09 13:07:50.000000 tigeropen-3.2.2/tigeropen/common/consts/service_types.py
--rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/common/consts/tick_constants.py
--rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/common/exceptions.py
--rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/common/model.py
--rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/common/request.py
--rw-r--r--   0 sukai      (501) staff       (20)      654 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/common/response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.480339 tigeropen-3.2.2/tigeropen/common/util/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/common/util/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/common/util/account_util.py
--rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/common/util/common_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     4032 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/common/util/contract_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     8379 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/common/util/order_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     3124 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/common/util/price_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     2709 2024-02-27 08:47:04.000000 tigeropen-3.2.2/tigeropen/common/util/signature_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/common/util/string_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-3.2.2/tigeropen/common/util/tick_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     1675 2024-02-27 08:47:04.000000 tigeropen-3.2.2/tigeropen/common/util/web_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.482566 tigeropen-3.2.2/tigeropen/examples/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/examples/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/examples/client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)     7026 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/examples/financial_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/examples/nasdaq100.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.483064 tigeropen-3.2.2/tigeropen/examples/option_helpers/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/examples/option_helpers/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/examples/option_helpers/helpers.py
--rw-r--r--   0 sukai      (501) staff       (20)    11453 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/examples/push_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    11030 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/examples/push_client_stomp_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    13724 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/examples/quote_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)     8386 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/examples/trade_client_demo.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.483348 tigeropen-3.2.2/tigeropen/fundamental/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.2/tigeropen/fundamental/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.483579 tigeropen-3.2.2/tigeropen/fundamental/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.2/tigeropen/fundamental/domain/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.484066 tigeropen-3.2.2/tigeropen/fundamental/request/
--rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-3.2.2/tigeropen/fundamental/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     7711 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/fundamental/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.486424 tigeropen-3.2.2/tigeropen/fundamental/response/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.2/tigeropen/fundamental/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-3.2.2/tigeropen/fundamental/response/corporate_dividend_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-3.2.2/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-3.2.2/tigeropen/fundamental/response/corporate_split_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      898 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/fundamental/response/dataframe_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/fundamental/response/financial_daily_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      972 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/fundamental/response/financial_exchange_rate_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/fundamental/response/financial_report_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/fundamental/response/industry_response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.487236 tigeropen-3.2.2/tigeropen/push/
--rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/push/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.489066 tigeropen-3.2.2/tigeropen/push/network/
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/network/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/network/connect.py
--rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/network/exception.py
--rw-r--r--   0 sukai      (501) staff       (20)     7566 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/network/listener.py
--rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/network/protocal.py
--rw-r--r--   0 sukai      (501) staff       (20)    31352 2024-02-27 08:47:04.000000 tigeropen-3.2.2/tigeropen/push/network/transport.py
--rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/network/utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.505413 tigeropen-3.2.2/tigeropen/push/pb/
--rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/AssetData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1572 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/AssetData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1887 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/AssetData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      714 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/push/pb/KlineData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1446 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/push/pb/KlineData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1355 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/push/pb/KlineData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1238 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/OptionTopData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2473 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/OptionTopData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3823 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/OptionTopData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2051 2024-02-28 06:50:45.000000 tigeropen-3.2.2/tigeropen/push/pb/OrderStatusData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2662 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/OrderStatusData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4752 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/OrderStatusData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/OrderTransactionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1729 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/OrderTransactionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2102 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/OrderTransactionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1117 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/PositionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1824 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/PositionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2418 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/PositionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1167 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/PushData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     4348 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/PushData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4193 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/PushData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteBBOData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1702 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteBBOData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteBBOData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteBasicData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3046 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteBasicData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3115 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteBasicData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2303 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3573 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4265 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      433 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteDepthData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1570 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteDepthData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1817 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteDepthData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      657 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/Request.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2495 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/Request_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2572 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/Request_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/Response.proto
--rw-r--r--   0 sukai      (501) staff       (20)     5392 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/Response_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1977 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/Response_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      781 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/push/pb/SocketCommon.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2129 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/push/pb/SocketCommon_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1584 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/push/pb/SocketCommon_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      411 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/StockTopData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1631 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/StockTopData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1720 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/StockTopData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      745 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/TickData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1503 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/TickData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1695 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/TickData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/TradeTickData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1760 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/TradeTickData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2502 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/TradeTickData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)        0 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/readme.md
--rw-r--r--   0 sukai      (501) staff       (20)      661 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/trade_tick.py
--rw-r--r--   0 sukai      (501) staff       (20)     9557 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/util.py
--rw-r--r--   0 sukai      (501) staff       (20)    20015 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/protobuf_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     9966 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    28685 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/stomp_push_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.505765 tigeropen-3.2.2/tigeropen/quote/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/quote/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.508580 tigeropen-3.2.2/tigeropen/quote/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/quote/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/domain/bar.py
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/quote/domain/capital_distribution.py
--rw-r--r--   0 sukai      (501) staff       (20)     9623 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/domain/filter.py
--rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/domain/market_status.py
--rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/domain/quote_brief.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/quote/domain/stock_broker.py
--rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/domain/tick.py
--rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/domain/timeline.py
--rw-r--r--   0 sukai      (501) staff       (20)    84071 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/quote/quote_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.509013 tigeropen-3.2.2/tigeropen/quote/request/
--rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/quote/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    35270 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/quote/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.517684 tigeropen-3.2.2/tigeropen/quote/response/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/quote/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/quote/response/capital_distribution_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/quote/response/capital_flow_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      911 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/fund_contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-3.2.2/tigeropen/quote/response/future_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-3.2.2/tigeropen/quote/response/future_contract_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/future_exchange_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1746 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/future_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/quote/response/future_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-3.2.2/tigeropen/quote/response/future_trading_times_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      706 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/kline_quota_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1805 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/market_scanner_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/market_status_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2515 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/quote/response/option_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-3.2.2/tigeropen/quote/response/option_chains_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1121 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/quote/response/option_expirations_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/option_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/option_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1599 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2469 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_brief_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      983 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_dataframe_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_delay_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_depth_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_grab_permission_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2730 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_hour_trading_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2410 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1152 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/stock_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/quote/response/stock_broker_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4898 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/stock_details_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/stock_short_interest_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/stock_trade_meta_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/symbol_names_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      653 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/symbols_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/quote/response/trading_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      802 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/warrant_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      979 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/warrant_filter_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    11281 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/tiger_open_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    16514 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/tiger_open_config.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.518095 tigeropen-3.2.2/tigeropen/trade/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/trade/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.519748 tigeropen-3.2.2/tigeropen/trade/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/trade/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    11655 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/domain/account.py
--rw-r--r--   0 sukai      (501) staff       (20)     6154 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/domain/contract.py
--rw-r--r--   0 sukai      (501) staff       (20)    11246 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/trade/domain/order.py
--rw-r--r--   0 sukai      (501) staff       (20)     2704 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/domain/position.py
--rw-r--r--   0 sukai      (501) staff       (20)     3242 2024-02-27 08:46:55.000000 tigeropen-3.2.2/tigeropen/trade/domain/prime_account.py
--rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/trade/domain/profile.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.520344 tigeropen-3.2.2/tigeropen/trade/request/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/trade/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    35911 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/trade/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.523251 tigeropen-3.2.2/tigeropen/trade/response/
--rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/trade/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1120 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/account_profile_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      949 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/analytics_asset_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4426 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1608 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/forex_order_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1255 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/order_id_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1278 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/order_preview_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     8507 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/trade/response/orders_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     6199 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/positions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-3.2.2/tigeropen/trade/response/prime_assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2539 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/segment_fund_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1413 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/transactions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    41235 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/trade/trade_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.473840 tigeropen-3.2.2/tigeropen.egg-info/
--rw-r--r--   0 sukai      (501) staff       (20)     7120 2024-04-09 13:07:53.000000 tigeropen-3.2.2/tigeropen.egg-info/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     8155 2024-04-09 13:07:53.000000 tigeropen-3.2.2/tigeropen.egg-info/SOURCES.txt
--rw-r--r--   0 sukai      (501) staff       (20)        1 2024-04-09 13:07:53.000000 tigeropen-3.2.2/tigeropen.egg-info/dependency_links.txt
--rw-r--r--   0 sukai      (501) staff       (20)      138 2024-04-09 13:07:53.000000 tigeropen-3.2.2/tigeropen.egg-info/requires.txt
--rw-r--r--   0 sukai      (501) staff       (20)       10 2024-04-09 13:07:53.000000 tigeropen-3.2.2/tigeropen.egg-info/top_level.txt
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.659628 tigeropen-3.2.3/
+-rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-3.2.3/MANIFEST.in
+-rw-r--r--   0 sukai      (501) staff       (20)     7120 2024-04-11 02:46:44.659339 tigeropen-3.2.3/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-3.2.3/README.md
+-rw-r--r--   0 sukai      (501) staff       (20)      137 2024-02-27 08:47:04.000000 tigeropen-3.2.3/requirements.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       38 2024-04-11 02:46:44.659696 tigeropen-3.2.3/setup.cfg
+-rw-r--r--   0 sukai      (501) staff       (20)     1358 2024-01-19 03:27:35.000000 tigeropen-3.2.3/setup.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.612723 tigeropen-3.2.3/tests/
+-rw-r--r--   0 sukai      (501) staff       (20)     2628 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tests/test_client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2589 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tests/test_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2856 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tests/test_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.613233 tigeropen-3.2.3/tigeropen/
+-rw-r--r--   0 sukai      (501) staff       (20)       91 2024-04-11 02:46:42.000000 tigeropen-3.2.3/tigeropen/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.615618 tigeropen-3.2.3/tigeropen/common/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.3/tigeropen/common/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.618737 tigeropen-3.2.3/tigeropen/common/consts/
+-rw-r--r--   0 sukai      (501) staff       (20)     5171 2024-04-08 07:19:32.000000 tigeropen-3.2.3/tigeropen/common/consts/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    19289 2024-02-27 08:46:55.000000 tigeropen-3.2.3/tigeropen/common/consts/filter_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)    39797 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/common/consts/fundamental_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-3.2.3/tigeropen/common/consts/params.py
+-rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/common/consts/push_destinations.py
+-rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/common/consts/push_subscriptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-3.2.3/tigeropen/common/consts/push_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-3.2.3/tigeropen/common/consts/quote_keys.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3296 2024-04-10 11:04:28.000000 tigeropen-3.2.3/tigeropen/common/consts/service_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/common/consts/tick_constants.py
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-3.2.3/tigeropen/common/exceptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-3.2.3/tigeropen/common/model.py
+-rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/common/request.py
+-rw-r--r--   0 sukai      (501) staff       (20)      654 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/common/response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.621048 tigeropen-3.2.3/tigeropen/common/util/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.3/tigeropen/common/util/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/common/util/account_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/common/util/common_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4032 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/common/util/contract_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8379 2024-04-08 07:19:32.000000 tigeropen-3.2.3/tigeropen/common/util/order_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3124 2024-04-08 07:19:32.000000 tigeropen-3.2.3/tigeropen/common/util/price_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2709 2024-02-27 08:47:04.000000 tigeropen-3.2.3/tigeropen/common/util/signature_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-3.2.3/tigeropen/common/util/string_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-3.2.3/tigeropen/common/util/tick_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1675 2024-02-27 08:47:04.000000 tigeropen-3.2.3/tigeropen/common/util/web_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.623247 tigeropen-3.2.3/tigeropen/examples/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.3/tigeropen/examples/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/examples/client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7026 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/examples/financial_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/examples/nasdaq100.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.623637 tigeropen-3.2.3/tigeropen/examples/option_helpers/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/examples/option_helpers/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/examples/option_helpers/helpers.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11453 2024-03-18 09:47:36.000000 tigeropen-3.2.3/tigeropen/examples/push_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11030 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/examples/push_client_stomp_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13724 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/examples/quote_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8386 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/examples/trade_client_demo.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.623828 tigeropen-3.2.3/tigeropen/fundamental/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.3/tigeropen/fundamental/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.624017 tigeropen-3.2.3/tigeropen/fundamental/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.3/tigeropen/fundamental/domain/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.624345 tigeropen-3.2.3/tigeropen/fundamental/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-3.2.3/tigeropen/fundamental/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7711 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/fundamental/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.626555 tigeropen-3.2.3/tigeropen/fundamental/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.3/tigeropen/fundamental/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-3.2.3/tigeropen/fundamental/response/corporate_dividend_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-3.2.3/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-3.2.3/tigeropen/fundamental/response/corporate_split_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      898 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/fundamental/response/dataframe_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/fundamental/response/financial_daily_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      972 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/fundamental/response/financial_exchange_rate_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/fundamental/response/financial_report_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/fundamental/response/industry_response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.627338 tigeropen-3.2.3/tigeropen/push/
+-rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/push/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.628794 tigeropen-3.2.3/tigeropen/push/network/
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-3.2.3/tigeropen/push/network/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-3.2.3/tigeropen/push/network/connect.py
+-rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-3.2.3/tigeropen/push/network/exception.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7566 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/push/network/listener.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-3.2.3/tigeropen/push/network/protocal.py
+-rw-r--r--   0 sukai      (501) staff       (20)    31352 2024-02-27 08:47:04.000000 tigeropen-3.2.3/tigeropen/push/network/transport.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-3.2.3/tigeropen/push/network/utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.642003 tigeropen-3.2.3/tigeropen/push/pb/
+-rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-3.2.3/tigeropen/push/pb/AssetData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1572 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/AssetData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1887 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/AssetData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      714 2024-03-18 09:47:36.000000 tigeropen-3.2.3/tigeropen/push/pb/KlineData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1446 2024-03-18 09:47:36.000000 tigeropen-3.2.3/tigeropen/push/pb/KlineData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1355 2024-03-18 09:47:36.000000 tigeropen-3.2.3/tigeropen/push/pb/KlineData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1238 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/push/pb/OptionTopData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2473 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/OptionTopData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3823 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/OptionTopData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2051 2024-02-28 06:50:45.000000 tigeropen-3.2.3/tigeropen/push/pb/OrderStatusData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2662 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/OrderStatusData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4752 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/OrderStatusData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-3.2.3/tigeropen/push/pb/OrderTransactionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1729 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/OrderTransactionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2102 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/OrderTransactionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1117 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/push/pb/PositionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1824 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/PositionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2418 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/PositionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1167 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/pb/PushData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     4348 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/pb/PushData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4193 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/pb/PushData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-3.2.3/tigeropen/push/pb/QuoteBBOData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1702 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/QuoteBBOData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/QuoteBBOData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-3.2.3/tigeropen/push/pb/QuoteBasicData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3046 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/QuoteBasicData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3115 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/QuoteBasicData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2303 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/push/pb/QuoteData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3573 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/QuoteData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4265 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/QuoteData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      433 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/push/pb/QuoteDepthData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1570 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/QuoteDepthData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1817 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/QuoteDepthData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      657 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/pb/Request.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2495 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/pb/Request_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2572 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/pb/Request_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-3.2.3/tigeropen/push/pb/Response.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     5392 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/pb/Response_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1977 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/pb/Response_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      781 2024-03-18 09:47:36.000000 tigeropen-3.2.3/tigeropen/push/pb/SocketCommon.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2129 2024-03-18 09:47:36.000000 tigeropen-3.2.3/tigeropen/push/pb/SocketCommon_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1584 2024-03-18 09:47:36.000000 tigeropen-3.2.3/tigeropen/push/pb/SocketCommon_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/push/pb/StockTopData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1631 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/StockTopData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1720 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/StockTopData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      745 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/pb/TickData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1503 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/pb/TickData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1695 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/pb/TickData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-3.2.3/tigeropen/push/pb/TradeTickData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1760 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/TradeTickData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2502 2024-03-06 08:28:03.000000 tigeropen-3.2.3/tigeropen/push/pb/TradeTickData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/push/pb/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-3.2.3/tigeropen/push/pb/readme.md
+-rw-r--r--   0 sukai      (501) staff       (20)      661 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/push/pb/trade_tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9557 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/pb/util.py
+-rw-r--r--   0 sukai      (501) staff       (20)    20015 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/protobuf_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9966 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    28685 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/push/stomp_push_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.642327 tigeropen-3.2.3/tigeropen/quote/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.3/tigeropen/quote/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.644408 tigeropen-3.2.3/tigeropen/quote/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.3/tigeropen/quote/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/quote/domain/bar.py
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-3.2.3/tigeropen/quote/domain/capital_distribution.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9623 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/domain/filter.py
+-rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/quote/domain/market_status.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/quote/domain/quote_brief.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-3.2.3/tigeropen/quote/domain/stock_broker.py
+-rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/quote/domain/tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/quote/domain/timeline.py
+-rw-r--r--   0 sukai      (501) staff       (20)    84071 2024-04-08 07:19:32.000000 tigeropen-3.2.3/tigeropen/quote/quote_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.644748 tigeropen-3.2.3/tigeropen/quote/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/quote/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    35270 2024-04-08 07:19:32.000000 tigeropen-3.2.3/tigeropen/quote/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.653653 tigeropen-3.2.3/tigeropen/quote/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.3/tigeropen/quote/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-3.2.3/tigeropen/quote/response/capital_distribution_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-3.2.3/tigeropen/quote/response/capital_flow_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      911 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/fund_contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-3.2.3/tigeropen/quote/response/future_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-3.2.3/tigeropen/quote/response/future_contract_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/quote/response/future_exchange_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1746 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/future_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/quote/response/future_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-3.2.3/tigeropen/quote/response/future_trading_times_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      706 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/kline_quota_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1805 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/market_scanner_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/quote/response/market_status_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2515 2024-04-08 07:19:32.000000 tigeropen-3.2.3/tigeropen/quote/response/option_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-3.2.3/tigeropen/quote/response/option_chains_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1149 2024-04-11 02:46:42.000000 tigeropen-3.2.3/tigeropen/quote/response/option_expirations_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/quote/response/option_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/quote/response/option_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1599 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2469 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/quote_brief_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      983 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/quote_dataframe_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-3.2.3/tigeropen/quote/response/quote_delay_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/quote/response/quote_depth_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/quote/response/quote_grab_permission_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2730 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/quote_hour_trading_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2410 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-3.2.3/tigeropen/quote/response/quote_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1152 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/stock_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-3.2.3/tigeropen/quote/response/stock_broker_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4898 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/stock_details_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/quote/response/stock_short_interest_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/quote/response/stock_trade_meta_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-3.2.3/tigeropen/quote/response/symbol_names_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      653 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/symbols_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/quote/response/trading_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      802 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/warrant_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      979 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/quote/response/warrant_filter_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11281 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/tiger_open_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    16514 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/tiger_open_config.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.654078 tigeropen-3.2.3/tigeropen/trade/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.3/tigeropen/trade/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.655730 tigeropen-3.2.3/tigeropen/trade/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.3/tigeropen/trade/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11655 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/trade/domain/account.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6154 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/trade/domain/contract.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11246 2024-04-08 07:19:32.000000 tigeropen-3.2.3/tigeropen/trade/domain/order.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2704 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/trade/domain/position.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3242 2024-02-27 08:46:55.000000 tigeropen-3.2.3/tigeropen/trade/domain/prime_account.py
+-rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/trade/domain/profile.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.656336 tigeropen-3.2.3/tigeropen/trade/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.3/tigeropen/trade/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    35911 2024-04-08 07:19:32.000000 tigeropen-3.2.3/tigeropen/trade/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.658929 tigeropen-3.2.3/tigeropen/trade/response/
+-rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-3.2.3/tigeropen/trade/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1120 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/trade/response/account_profile_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      949 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/trade/response/analytics_asset_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4426 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/trade/response/assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1608 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/trade/response/contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/trade/response/forex_order_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1255 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/trade/response/order_id_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1278 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/trade/response/order_preview_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8507 2024-04-08 07:19:32.000000 tigeropen-3.2.3/tigeropen/trade/response/orders_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6199 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/trade/response/positions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-3.2.3/tigeropen/trade/response/prime_assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2539 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/trade/response/segment_fund_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1413 2024-01-19 03:27:35.000000 tigeropen-3.2.3/tigeropen/trade/response/transactions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    41235 2024-04-09 07:24:17.000000 tigeropen-3.2.3/tigeropen/trade/trade_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-11 02:46:44.614342 tigeropen-3.2.3/tigeropen.egg-info/
+-rw-r--r--   0 sukai      (501) staff       (20)     7120 2024-04-11 02:46:44.000000 tigeropen-3.2.3/tigeropen.egg-info/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     8155 2024-04-11 02:46:44.000000 tigeropen-3.2.3/tigeropen.egg-info/SOURCES.txt
+-rw-r--r--   0 sukai      (501) staff       (20)        1 2024-04-11 02:46:44.000000 tigeropen-3.2.3/tigeropen.egg-info/dependency_links.txt
+-rw-r--r--   0 sukai      (501) staff       (20)      138 2024-04-11 02:46:44.000000 tigeropen-3.2.3/tigeropen.egg-info/requires.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       10 2024-04-11 02:46:44.000000 tigeropen-3.2.3/tigeropen.egg-info/top_level.txt
```

### Comparing `tigeropen-3.2.2/PKG-INFO` & `tigeropen-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 3.2.2
+Version: 3.2.3
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-3.2.2/README.md` & `tigeropen-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/setup.py` & `tigeropen-3.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tests/test_client_config.py` & `tigeropen-3.2.3/tests/test_client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tests/test_push_client.py` & `tigeropen-3.2.3/tests/test_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tests/test_utils.py` & `tigeropen-3.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/consts/__init__.py` & `tigeropen-3.2.3/tigeropen/common/consts/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/consts/filter_fields.py` & `tigeropen-3.2.3/tigeropen/common/consts/filter_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/consts/fundamental_fields.py` & `tigeropen-3.2.3/tigeropen/common/consts/fundamental_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/consts/params.py` & `tigeropen-3.2.3/tigeropen/common/consts/params.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/consts/push_types.py` & `tigeropen-3.2.3/tigeropen/common/consts/push_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/consts/quote_keys.py` & `tigeropen-3.2.3/tigeropen/common/consts/quote_keys.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/consts/service_types.py` & `tigeropen-3.2.3/tigeropen/common/consts/service_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 """
 账户/资产
 """
 ACCOUNTS = "accounts"
 ASSETS = "assets"
 PRIME_ASSETS = "prime_assets"
 POSITIONS = "positions"
-ORDERS = (""
-          "")
+ORDERS = "orders"
 ACTIVE_ORDERS = "active_orders"  # 待成交订单
 INACTIVE_ORDERS = "inactive_orders"  # 已撤销订单
 FILLED_ORDERS = "filled_orders"  # 已成交订单
 ORDER_TRANSACTIONS = "order_transactions"  # 订单成交记录
 ANALYTICS_ASSET = "analytics_asset"
 SEGMENT_FUND_HISTORY = "segment_fund_history"
 SEGMENT_FUND_AVAILABLE = "segment_fund_available"
```

### Comparing `tigeropen-3.2.2/tigeropen/common/consts/tick_constants.py` & `tigeropen-3.2.3/tigeropen/common/consts/tick_constants.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/model.py` & `tigeropen-3.2.3/tigeropen/common/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/request.py` & `tigeropen-3.2.3/tigeropen/common/request.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/response.py` & `tigeropen-3.2.3/tigeropen/common/response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/util/common_utils.py` & `tigeropen-3.2.3/tigeropen/common/util/common_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/util/contract_utils.py` & `tigeropen-3.2.3/tigeropen/common/util/contract_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/util/order_utils.py` & `tigeropen-3.2.3/tigeropen/common/util/order_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/util/price_util.py` & `tigeropen-3.2.3/tigeropen/common/util/price_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/util/signature_utils.py` & `tigeropen-3.2.3/tigeropen/common/util/signature_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/util/string_utils.py` & `tigeropen-3.2.3/tigeropen/common/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/util/tick_util.py` & `tigeropen-3.2.3/tigeropen/common/util/tick_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/common/util/web_utils.py` & `tigeropen-3.2.3/tigeropen/common/util/web_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/examples/client_config.py` & `tigeropen-3.2.3/tigeropen/examples/client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/examples/financial_demo.py` & `tigeropen-3.2.3/tigeropen/examples/financial_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/examples/nasdaq100.py` & `tigeropen-3.2.3/tigeropen/examples/nasdaq100.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/examples/option_helpers/helpers.py` & `tigeropen-3.2.3/tigeropen/examples/option_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/examples/push_client_demo.py` & `tigeropen-3.2.3/tigeropen/examples/push_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/examples/push_client_stomp_demo.py` & `tigeropen-3.2.3/tigeropen/examples/push_client_stomp_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/examples/quote_client_demo.py` & `tigeropen-3.2.3/tigeropen/examples/quote_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/examples/trade_client_demo.py` & `tigeropen-3.2.3/tigeropen/examples/trade_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/fundamental/request/model.py` & `tigeropen-3.2.3/tigeropen/fundamental/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/fundamental/response/corporate_dividend_response.py` & `tigeropen-3.2.3/tigeropen/fundamental/response/corporate_dividend_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/fundamental/response/corporate_earnings_calendar_response.py` & `tigeropen-3.2.3/tigeropen/fundamental/response/corporate_earnings_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/fundamental/response/corporate_split_response.py` & `tigeropen-3.2.3/tigeropen/fundamental/response/corporate_split_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/fundamental/response/dataframe_response.py` & `tigeropen-3.2.3/tigeropen/fundamental/response/dataframe_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/fundamental/response/financial_daily_response.py` & `tigeropen-3.2.3/tigeropen/fundamental/response/financial_daily_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/fundamental/response/financial_exchange_rate_response.py` & `tigeropen-3.2.3/tigeropen/fundamental/response/financial_exchange_rate_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/fundamental/response/financial_report_response.py` & `tigeropen-3.2.3/tigeropen/fundamental/response/financial_report_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/fundamental/response/industry_response.py` & `tigeropen-3.2.3/tigeropen/fundamental/response/industry_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/__init__.py` & `tigeropen-3.2.3/tigeropen/push/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/network/connect.py` & `tigeropen-3.2.3/tigeropen/push/network/connect.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/network/exception.py` & `tigeropen-3.2.3/tigeropen/push/network/exception.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/network/listener.py` & `tigeropen-3.2.3/tigeropen/push/network/listener.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/network/protocal.py` & `tigeropen-3.2.3/tigeropen/push/network/protocal.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/network/transport.py` & `tigeropen-3.2.3/tigeropen/push/network/transport.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/network/utils.py` & `tigeropen-3.2.3/tigeropen/push/network/utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/AssetData.proto` & `tigeropen-3.2.3/tigeropen/push/pb/AssetData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/AssetData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/AssetData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/AssetData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/AssetData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/KlineData.proto` & `tigeropen-3.2.3/tigeropen/push/pb/KlineData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/KlineData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/KlineData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/KlineData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/KlineData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/OptionTopData.proto` & `tigeropen-3.2.3/tigeropen/push/pb/OptionTopData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/OptionTopData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/OptionTopData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/OptionTopData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/OptionTopData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/OrderStatusData.proto` & `tigeropen-3.2.3/tigeropen/push/pb/OrderStatusData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/OrderStatusData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/OrderStatusData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/OrderStatusData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/OrderStatusData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/OrderTransactionData.proto` & `tigeropen-3.2.3/tigeropen/push/pb/OrderTransactionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/OrderTransactionData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/OrderTransactionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/OrderTransactionData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/OrderTransactionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/PositionData.proto` & `tigeropen-3.2.3/tigeropen/push/pb/PositionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/PositionData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/PositionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/PositionData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/PositionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/PushData.proto` & `tigeropen-3.2.3/tigeropen/push/pb/PushData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/PushData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/PushData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/PushData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/PushData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/QuoteBBOData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/QuoteBBOData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/QuoteBBOData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/QuoteBBOData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/QuoteBasicData.proto` & `tigeropen-3.2.3/tigeropen/push/pb/QuoteBasicData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/QuoteBasicData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/QuoteBasicData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/QuoteBasicData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/QuoteBasicData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/QuoteData.proto` & `tigeropen-3.2.3/tigeropen/push/pb/QuoteData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/QuoteData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/QuoteData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/QuoteData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/QuoteData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/QuoteDepthData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/QuoteDepthData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/QuoteDepthData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/QuoteDepthData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/Request.proto` & `tigeropen-3.2.3/tigeropen/push/pb/Request.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/Request_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/Request_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/Request_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/Request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/Response_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/Response_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/Response_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/Response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/SocketCommon.proto` & `tigeropen-3.2.3/tigeropen/push/pb/SocketCommon.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/SocketCommon_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/SocketCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/SocketCommon_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/SocketCommon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/StockTopData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/StockTopData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/StockTopData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/StockTopData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/TickData.proto` & `tigeropen-3.2.3/tigeropen/push/pb/TickData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/TickData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/TickData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/TickData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/TickData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/TradeTickData.proto` & `tigeropen-3.2.3/tigeropen/push/pb/TradeTickData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/TradeTickData_pb2.py` & `tigeropen-3.2.3/tigeropen/push/pb/TradeTickData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/TradeTickData_pb2.pyi` & `tigeropen-3.2.3/tigeropen/push/pb/TradeTickData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/trade_tick.py` & `tigeropen-3.2.3/tigeropen/push/pb/trade_tick.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/pb/util.py` & `tigeropen-3.2.3/tigeropen/push/pb/util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/protobuf_push_client.py` & `tigeropen-3.2.3/tigeropen/push/protobuf_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/push_client.py` & `tigeropen-3.2.3/tigeropen/push/push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/push/stomp_push_client.py` & `tigeropen-3.2.3/tigeropen/push/stomp_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/domain/filter.py` & `tigeropen-3.2.3/tigeropen/quote/domain/filter.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/domain/quote_brief.py` & `tigeropen-3.2.3/tigeropen/quote/domain/quote_brief.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/domain/stock_broker.py` & `tigeropen-3.2.3/tigeropen/quote/domain/stock_broker.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/quote_client.py` & `tigeropen-3.2.3/tigeropen/quote/quote_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/request/model.py` & `tigeropen-3.2.3/tigeropen/quote/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/capital_distribution_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/capital_distribution_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/capital_flow_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/capital_flow_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/fund_contracts_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/fund_contracts_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/future_briefs_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/future_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/future_contract_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/future_contract_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/future_exchange_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/future_exchange_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/future_quote_bar_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/future_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/future_quote_ticks_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/future_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/future_trading_times_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/future_trading_times_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/kline_quota_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/kline_quota_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/market_scanner_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/market_scanner_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/market_status_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/market_status_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/option_briefs_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/option_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/option_chains_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/option_chains_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/option_expirations_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/option_expirations_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,10 +23,12 @@
             self.expirations = pd.DataFrame()
             for item in self.data:
                 symbol = item.get('symbol')
                 dates = item.get('dates')
                 item.pop('count', None)
 
                 if symbol and dates:
-                    self.expirations = pd.concat([self.expirations, pd.DataFrame(item)]).rename(
-                        columns={'dates': 'date', 'timestamps': 'timestamp',
-                                 'periodTags': 'period_tag'})
+                    self.expirations = pd.concat([self.expirations, pd.DataFrame(item)])
+
+            self.expirations.rename(
+                columns={'dates': 'date', 'timestamps': 'timestamp',
+                         'periodTags': 'period_tag'}, inplace=True)
```

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/option_quote_bar_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/option_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/option_quote_ticks_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/option_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/quote_bar_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/quote_brief_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/quote_brief_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/quote_dataframe_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/quote_dataframe_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/quote_delay_briefs_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/quote_delay_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/quote_depth_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/quote_depth_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/quote_grab_permission_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/quote_grab_permission_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/quote_hour_trading_timeline_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/quote_hour_trading_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/quote_ticks_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/quote_timeline_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/quote_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/stock_briefs_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/stock_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/stock_broker_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/stock_broker_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/stock_details_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/stock_details_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/stock_short_interest_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/stock_short_interest_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/stock_trade_meta_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/stock_trade_meta_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/symbol_names_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/symbol_names_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/symbols_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/symbols_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/trading_calendar_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/trading_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/warrant_briefs_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/warrant_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/quote/response/warrant_filter_response.py` & `tigeropen-3.2.3/tigeropen/quote/response/warrant_filter_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/tiger_open_client.py` & `tigeropen-3.2.3/tigeropen/tiger_open_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/tiger_open_config.py` & `tigeropen-3.2.3/tigeropen/tiger_open_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/domain/account.py` & `tigeropen-3.2.3/tigeropen/trade/domain/account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/domain/contract.py` & `tigeropen-3.2.3/tigeropen/trade/domain/contract.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/domain/order.py` & `tigeropen-3.2.3/tigeropen/trade/domain/order.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/domain/position.py` & `tigeropen-3.2.3/tigeropen/trade/domain/position.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/domain/prime_account.py` & `tigeropen-3.2.3/tigeropen/trade/domain/prime_account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/request/model.py` & `tigeropen-3.2.3/tigeropen/trade/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/response/__init__.py` & `tigeropen-3.2.3/tigeropen/trade/response/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/response/account_profile_response.py` & `tigeropen-3.2.3/tigeropen/trade/response/account_profile_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/response/analytics_asset_response.py` & `tigeropen-3.2.3/tigeropen/trade/response/analytics_asset_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/response/assets_response.py` & `tigeropen-3.2.3/tigeropen/trade/response/assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/response/contracts_response.py` & `tigeropen-3.2.3/tigeropen/trade/response/contracts_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/response/forex_order_response.py` & `tigeropen-3.2.3/tigeropen/trade/response/forex_order_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/response/order_id_response.py` & `tigeropen-3.2.3/tigeropen/trade/response/order_id_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/response/order_preview_response.py` & `tigeropen-3.2.3/tigeropen/trade/response/order_preview_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/response/orders_response.py` & `tigeropen-3.2.3/tigeropen/trade/response/orders_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/response/positions_response.py` & `tigeropen-3.2.3/tigeropen/trade/response/positions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/response/prime_assets_response.py` & `tigeropen-3.2.3/tigeropen/trade/response/prime_assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/response/segment_fund_response.py` & `tigeropen-3.2.3/tigeropen/trade/response/segment_fund_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/response/transactions_response.py` & `tigeropen-3.2.3/tigeropen/trade/response/transactions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen/trade/trade_client.py` & `tigeropen-3.2.3/tigeropen/trade/trade_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.2/tigeropen.egg-info/PKG-INFO` & `tigeropen-3.2.3/tigeropen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 3.2.2
+Version: 3.2.3
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-3.2.2/tigeropen.egg-info/SOURCES.txt` & `tigeropen-3.2.3/tigeropen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

