# Comparing `tmp/getnet-python-3.4.tar.gz` & `tmp/getnet-python-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getnet-python-3.4.tar", last modified: Mon Feb 12 13:53:08 2024, max compression
+gzip compressed data, was "getnet-python-3.5.tar", last modified: Thu Apr 11 17:05:32 2024, max compression
```

## Comparing `getnet-python-3.4.tar` & `getnet-python-3.5.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.394808 getnet-python-3.4/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1069 2024-02-12 13:30:16.000000 getnet-python-3.4/LICENSE
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     5180 2024-02-12 13:53:08.398808 getnet-python-3.4/PKG-INFO
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     4645 2024-02-12 13:30:16.000000 getnet-python-3.4/README.md
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.350808 getnet-python-3.4/getnet/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      530 2024-02-12 13:40:25.000000 getnet-python-3.4/getnet/__init__.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.350808 getnet-python-3.4/getnet/application/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       32 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/application/__init__.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.358808 getnet-python-3.4/getnet/application/dtos/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       37 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/application/dtos/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      272 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/application/dtos/authentication.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      473 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/application/dtos/card_bin.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      115 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/application/dtos/card_token.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      206 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/application/dtos/card_verification.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      541 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/application/dtos/customer.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      288 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/application/dtos/pix.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.358808 getnet-python-3.4/getnet/domain/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       27 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/__init__.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.358808 getnet-python-3.4/getnet/domain/authentication/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       43 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/authentication/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1998 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/authentication/authentication.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.362808 getnet-python-3.4/getnet/domain/card_bin/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       60 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/card_bin/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      709 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/card_bin/card_bin.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.366808 getnet-python-3.4/getnet/domain/cards/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       83 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/cards/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     3725 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/cards/card.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1966 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/cards/card_response.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     2653 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/cards/service.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      178 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/cards/status.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.370808 getnet-python-3.4/getnet/domain/customers/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       68 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/customers/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      679 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/customers/address.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1783 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/customers/customer.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      240 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/customers/customer_response.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     2573 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/customers/service.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.370808 getnet-python-3.4/getnet/domain/device/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       48 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/device/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      622 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/device/device.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.374808 getnet-python-3.4/getnet/domain/payments/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      103 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/__init__.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.382808 getnet-python-3.4/getnet/domain/payments/credit/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       60 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/credit/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      431 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/credit/card.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1998 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/credit/credit.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1579 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/credit/credit_adjust.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1298 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/credit/credit_cancel.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1230 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/credit/credit_capture.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     2017 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/credit/credit_response.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     3170 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/credit/service.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      733 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/customer.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      801 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/order.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      972 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/payment_response.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.382808 getnet-python-3.4/getnet/domain/payments/pix/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       50 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/pix/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      473 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/payments/pix/pix.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1264 2024-02-12 13:41:52.000000 getnet-python-3.4/getnet/domain/payments/pix/pix_response.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1021 2024-02-12 12:45:36.000000 getnet-python-3.4/getnet/domain/payments/pix/service.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.386808 getnet-python-3.4/getnet/domain/services/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       63 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/services/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1270 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/services/service.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.386808 getnet-python-3.4/getnet/domain/token/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       78 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/token/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1200 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/token/card_number.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      502 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/token/card_token.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1088 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/token/service.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.386808 getnet-python-3.4/getnet/domain/usecases/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       36 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/usecases/__init__.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.390808 getnet-python-3.4/getnet/domain/usecases/client/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       31 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/usecases/client/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     7701 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/usecases/client/get_client.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.390808 getnet-python-3.4/getnet/domain/usecases/environment/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       41 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/usecases/environment/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      436 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/usecases/environment/get_environment.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.390808 getnet-python-3.4/getnet/domain/usecases/errors/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      112 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/usecases/errors/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      801 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/usecases/errors/business_error.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      411 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/usecases/errors/generic_errors.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      294 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/usecases/errors/request_error.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.390808 getnet-python-3.4/getnet/domain/verification/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      122 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/verification/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1205 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/verification/card_verification.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      303 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/verification/card_verified.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1194 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/domain/verification/service.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1855 2023-12-14 14:35:58.000000 getnet-python-3.4/getnet/utils.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.390808 getnet-python-3.4/getnet_python.egg-info/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     5180 2024-02-12 13:53:08.000000 getnet-python-3.4/getnet_python.egg-info/PKG-INFO
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     3542 2024-02-12 13:53:08.000000 getnet-python-3.4/getnet_python.egg-info/SOURCES.txt
--rw-rw-r--   0 fabio     (1000) fabio     (1000)        1 2024-02-12 13:53:08.000000 getnet-python-3.4/getnet_python.egg-info/dependency_links.txt
--rw-rw-r--   0 fabio     (1000) fabio     (1000)        1 2024-02-12 13:43:06.000000 getnet-python-3.4/getnet_python.egg-info/not-zip-safe
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       64 2024-02-12 13:53:08.000000 getnet-python-3.4/getnet_python.egg-info/requires.txt
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       13 2024-02-12 13:53:08.000000 getnet-python-3.4/getnet_python.egg-info/top_level.txt
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      102 2024-02-12 13:53:08.398808 getnet-python-3.4/setup.cfg
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1191 2024-02-12 13:30:16.000000 getnet-python-3.4/setup.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.390808 getnet-python-3.4/tests/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/__init__.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.390808 getnet-python-3.4/tests/getnet/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/__init__.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.390808 getnet-python-3.4/tests/getnet/services/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/__init__.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.394808 getnet-python-3.4/tests/getnet/services/cards/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/cards/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1172 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/cards/conftest.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1416 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/cards/test_card.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      494 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/cards/test_card_response.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     2468 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/cards/test_integration.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1573 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/cards/test_service.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      436 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/conftest.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.394808 getnet-python-3.4/tests/getnet/services/customers/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/customers/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1010 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/customers/conftest.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      549 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/customers/test_customer.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     2098 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/customers/test_integration.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     1571 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/customers/test_service.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.394808 getnet-python-3.4/tests/getnet/services/token/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/token/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      525 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/token/test_card_number.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      388 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/token/test_integration.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      592 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/token/test_service.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:53:08.394808 getnet-python-3.4/tests/getnet/services/utils/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/utils/__init__.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      510 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/services/utils/test_device.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     2702 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/test_client.py
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      296 2024-02-12 13:30:16.000000 getnet-python-3.4/tests/getnet/test_environment.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.780239 getnet-python-3.5/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1069 2024-02-12 13:30:16.000000 getnet-python-3.5/LICENSE
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     5180 2024-04-11 17:05:32.780239 getnet-python-3.5/PKG-INFO
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     4645 2024-02-12 13:30:16.000000 getnet-python-3.5/README.md
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.772240 getnet-python-3.5/getnet/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      623 2024-04-11 17:01:23.000000 getnet-python-3.5/getnet/__init__.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.772240 getnet-python-3.5/getnet/application/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       32 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/application/__init__.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.772240 getnet-python-3.5/getnet/application/dtos/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       37 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/application/dtos/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      272 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/application/dtos/authentication.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      473 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/application/dtos/card_bin.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      115 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/application/dtos/card_token.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      206 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/application/dtos/card_verification.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      541 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/application/dtos/customer.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      288 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/application/dtos/pix.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.772240 getnet-python-3.5/getnet/domain/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       27 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/__init__.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.772240 getnet-python-3.5/getnet/domain/authentication/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       43 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/authentication/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1998 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/authentication/authentication.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.772240 getnet-python-3.5/getnet/domain/card_bin/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       60 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/card_bin/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      709 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/card_bin/card_bin.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.772240 getnet-python-3.5/getnet/domain/cards/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       83 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/cards/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     3725 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/cards/card.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1966 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/cards/card_response.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     2653 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/cards/service.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      178 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/cards/status.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.772240 getnet-python-3.5/getnet/domain/customers/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       68 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/customers/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      679 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/customers/address.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1783 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/customers/customer.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      240 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/customers/customer_response.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     2573 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/customers/service.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.776239 getnet-python-3.5/getnet/domain/device/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       48 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/device/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      622 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/device/device.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.776239 getnet-python-3.5/getnet/domain/payments/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      103 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/payments/__init__.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.776239 getnet-python-3.5/getnet/domain/payments/credit/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       60 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/payments/credit/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      431 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/payments/credit/card.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1998 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/payments/credit/credit.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1579 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/payments/credit/credit_adjust.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1298 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/payments/credit/credit_cancel.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1230 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/payments/credit/credit_capture.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     2017 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/payments/credit/credit_response.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     3170 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/payments/credit/service.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      733 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/payments/customer.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      801 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/payments/order.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      972 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/payments/payment_response.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.776239 getnet-python-3.5/getnet/domain/payments/pix/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       50 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/payments/pix/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      473 2024-04-11 16:41:18.000000 getnet-python-3.5/getnet/domain/payments/pix/pix.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1270 2024-04-11 17:01:13.000000 getnet-python-3.5/getnet/domain/payments/pix/pix_response.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1021 2024-04-11 17:01:32.000000 getnet-python-3.5/getnet/domain/payments/pix/service.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.776239 getnet-python-3.5/getnet/domain/services/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       63 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/services/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1270 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/services/service.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.776239 getnet-python-3.5/getnet/domain/token/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       78 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/token/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1200 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/token/card_number.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      502 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/token/card_token.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1088 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/token/service.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.776239 getnet-python-3.5/getnet/domain/usecases/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       36 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/usecases/__init__.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.776239 getnet-python-3.5/getnet/domain/usecases/client/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       31 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/usecases/client/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     7701 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/usecases/client/get_client.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.776239 getnet-python-3.5/getnet/domain/usecases/environment/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       41 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/usecases/environment/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      436 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/usecases/environment/get_environment.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.776239 getnet-python-3.5/getnet/domain/usecases/errors/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      112 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/usecases/errors/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      801 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/usecases/errors/business_error.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      411 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/usecases/errors/generic_errors.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      294 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/usecases/errors/request_error.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.776239 getnet-python-3.5/getnet/domain/verification/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      122 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/verification/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1205 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/verification/card_verification.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      303 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/verification/card_verified.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1194 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/domain/verification/service.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1855 2023-12-14 14:35:58.000000 getnet-python-3.5/getnet/utils.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.780239 getnet-python-3.5/getnet_python.egg-info/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     5180 2024-04-11 17:05:32.000000 getnet-python-3.5/getnet_python.egg-info/PKG-INFO
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     3542 2024-04-11 17:05:32.000000 getnet-python-3.5/getnet_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)        1 2024-04-11 17:05:32.000000 getnet-python-3.5/getnet_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)        1 2024-04-11 17:02:20.000000 getnet-python-3.5/getnet_python.egg-info/not-zip-safe
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       64 2024-04-11 17:05:32.000000 getnet-python-3.5/getnet_python.egg-info/requires.txt
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       13 2024-04-11 17:05:32.000000 getnet-python-3.5/getnet_python.egg-info/top_level.txt
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      102 2024-04-11 17:05:32.784239 getnet-python-3.5/setup.cfg
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1191 2024-02-12 13:30:16.000000 getnet-python-3.5/setup.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.780239 getnet-python-3.5/tests/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/__init__.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.780239 getnet-python-3.5/tests/getnet/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/__init__.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.780239 getnet-python-3.5/tests/getnet/services/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/__init__.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.780239 getnet-python-3.5/tests/getnet/services/cards/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/cards/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1172 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/cards/conftest.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1416 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/cards/test_card.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      494 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/cards/test_card_response.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     2468 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/cards/test_integration.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1573 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/cards/test_service.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      436 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/conftest.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.780239 getnet-python-3.5/tests/getnet/services/customers/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/customers/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1010 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/customers/conftest.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      549 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/customers/test_customer.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     2098 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/customers/test_integration.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     1571 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/customers/test_service.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.780239 getnet-python-3.5/tests/getnet/services/token/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/token/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      525 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/token/test_card_number.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      388 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/token/test_integration.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      592 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/token/test_service.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2024-04-11 17:05:32.780239 getnet-python-3.5/tests/getnet/services/utils/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)        0 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/utils/__init__.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      510 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/services/utils/test_device.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     2702 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/test_client.py
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      296 2024-02-12 13:30:16.000000 getnet-python-3.5/tests/getnet/test_environment.py
```

### Comparing `getnet-python-3.4/LICENSE` & `getnet-python-3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/PKG-INFO` & `getnet-python-3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getnet-python
-Version: 3.4
+Version: 3.5
 Summary: A Getnet SDK
 Home-page: https://github.com/FVitor7/getnet-python
 Author: Fabio Vitor
 Author-email: fabvitor2010@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `getnet-python-3.4/README.md` & `getnet-python-3.5/README.md`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/__init__.py` & `getnet-python-3.5/getnet/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 This package implements an API client to Santander Getnet.
 """
 import logging
 
 from .domain.usecases.client import Client
 from .domain.usecases.environment import Environment
-
-__version__ = "3.4"
+from .domain.usecases.errors import NotFound, ServerError, ServiceUnavailable, GatewayTimeout
+__version__ = "3.5"
 
 import requests
 
 if requests.__version__ < "2.0.0":
     msg = (
         "You are using requests version %s, which is older than "
         "getnet-py expects, please upgrade to 2.0.0 or later."
```

### Comparing `getnet-python-3.4/getnet/application/dtos/customer.py` & `getnet-python-3.5/getnet/application/dtos/customer.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/authentication/authentication.py` & `getnet-python-3.5/getnet/domain/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/card_bin/card_bin.py` & `getnet-python-3.5/getnet/domain/card_bin/card_bin.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/cards/card.py` & `getnet-python-3.5/getnet/domain/cards/card.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/cards/card_response.py` & `getnet-python-3.5/getnet/domain/cards/card_response.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/cards/service.py` & `getnet-python-3.5/getnet/domain/cards/service.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/customers/address.py` & `getnet-python-3.5/getnet/domain/customers/address.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/customers/customer.py` & `getnet-python-3.5/getnet/domain/customers/customer.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/customers/service.py` & `getnet-python-3.5/getnet/domain/customers/service.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/device/device.py` & `getnet-python-3.5/getnet/domain/device/device.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/payments/credit/credit.py` & `getnet-python-3.5/getnet/domain/payments/credit/credit.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/payments/credit/credit_adjust.py` & `getnet-python-3.5/getnet/domain/payments/credit/credit_adjust.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/payments/credit/credit_cancel.py` & `getnet-python-3.5/getnet/domain/payments/credit/credit_cancel.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/payments/credit/credit_capture.py` & `getnet-python-3.5/getnet/domain/payments/credit/credit_capture.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/payments/credit/credit_response.py` & `getnet-python-3.5/getnet/domain/payments/credit/credit_response.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/payments/credit/service.py` & `getnet-python-3.5/getnet/domain/payments/credit/service.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/payments/customer.py` & `getnet-python-3.5/getnet/domain/payments/customer.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/payments/order.py` & `getnet-python-3.5/getnet/domain/payments/order.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/payments/payment_response.py` & `getnet-python-3.5/getnet/domain/payments/payment_response.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/payments/pix/pix_response.py` & `getnet-python-3.5/getnet/domain/payments/pix/pix_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Union
-
 from getnet.domain.payments.pix.pix import Pix
 from getnet.domain.payments.payment_response import PaymentResponse
 from getnet.application.dtos.pix import AdditionalData
 
 
 class PixResponse(Pix):
     description: str
@@ -44,11 +42,12 @@
         **kwargs,
 
     ):
         self.description = description
         self.payment_id = payment_id
         self.status = status
         additional_data = kwargs.get("additional_data", {})
-        self.additional_data = AdditionalData(**additional_data)
+        if additional_data:
+            self.additional_data = AdditionalData(**additional_data)
 
     def _as_dict(self):
         return self.__dict__.copy()
```

### Comparing `getnet-python-3.4/getnet/domain/payments/pix/service.py` & `getnet-python-3.5/getnet/domain/payments/pix/service.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/services/service.py` & `getnet-python-3.5/getnet/domain/services/service.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/token/card_number.py` & `getnet-python-3.5/getnet/domain/token/card_number.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/token/service.py` & `getnet-python-3.5/getnet/domain/token/service.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/usecases/client/get_client.py` & `getnet-python-3.5/getnet/domain/usecases/client/get_client.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/usecases/errors/business_error.py` & `getnet-python-3.5/getnet/domain/usecases/errors/business_error.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/verification/card_verification.py` & `getnet-python-3.5/getnet/domain/verification/card_verification.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/domain/verification/service.py` & `getnet-python-3.5/getnet/domain/verification/service.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet/utils.py` & `getnet-python-3.5/getnet/utils.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/getnet_python.egg-info/PKG-INFO` & `getnet-python-3.5/getnet_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getnet-python
-Version: 3.4
+Version: 3.5
 Summary: A Getnet SDK
 Home-page: https://github.com/FVitor7/getnet-python
 Author: Fabio Vitor
 Author-email: fabvitor2010@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `getnet-python-3.4/getnet_python.egg-info/SOURCES.txt` & `getnet-python-3.5/getnet_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/setup.py` & `getnet-python-3.5/setup.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/tests/getnet/services/cards/conftest.py` & `getnet-python-3.5/tests/getnet/services/cards/conftest.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/tests/getnet/services/cards/test_card.py` & `getnet-python-3.5/tests/getnet/services/cards/test_card.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/tests/getnet/services/cards/test_integration.py` & `getnet-python-3.5/tests/getnet/services/cards/test_integration.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/tests/getnet/services/cards/test_service.py` & `getnet-python-3.5/tests/getnet/services/cards/test_service.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/tests/getnet/services/customers/conftest.py` & `getnet-python-3.5/tests/getnet/services/customers/conftest.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/tests/getnet/services/customers/test_customer.py` & `getnet-python-3.5/tests/getnet/services/customers/test_customer.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/tests/getnet/services/customers/test_integration.py` & `getnet-python-3.5/tests/getnet/services/customers/test_integration.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/tests/getnet/services/customers/test_service.py` & `getnet-python-3.5/tests/getnet/services/customers/test_service.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/tests/getnet/services/token/test_card_number.py` & `getnet-python-3.5/tests/getnet/services/token/test_card_number.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/tests/getnet/services/token/test_service.py` & `getnet-python-3.5/tests/getnet/services/token/test_service.py`

 * *Files identical despite different names*

### Comparing `getnet-python-3.4/tests/getnet/test_client.py` & `getnet-python-3.5/tests/getnet/test_client.py`

 * *Files identical despite different names*

