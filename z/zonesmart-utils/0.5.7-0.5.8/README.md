# Comparing `tmp/zonesmart-utils-0.5.7.tar.gz` & `tmp/zonesmart-utils-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zonesmart-utils-0.5.7.tar", last modified: Wed Apr 10 13:44:09 2024, max compression
+gzip compressed data, was "zonesmart-utils-0.5.8.tar", last modified: Wed Apr 10 18:25:04 2024, max compression
```

## Comparing `zonesmart-utils-0.5.7.tar` & `zonesmart-utils-0.5.8.tar`

### file list

```diff
@@ -1,344 +1,345 @@
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.458038 zonesmart-utils-0.5.7/
--rw-rw-r--   0 kamil     (1000) kamil     (1000)      110 2024-04-10 13:44:09.458038 zonesmart-utils-0.5.7/PKG-INFO
--rw-r--r--   0 kamil     (1000) kamil     (1000)        9 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/README.md
--rw-r--r--   0 kamil     (1000) kamil     (1000)      368 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/pyproject.toml
--rw-r--r--   0 kamil     (1000) kamil     (1000)      209 2024-04-10 13:44:09.458038 zonesmart-utils-0.5.7/setup.cfg
--rw-r--r--   0 kamil     (1000) kamil     (1000)      529 2024-04-10 13:43:48.000000 zonesmart-utils-0.5.7/setup.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.426038 zonesmart-utils-0.5.7/zonesmart_utils.egg-info/
--rw-rw-r--   0 kamil     (1000) kamil     (1000)      110 2024-04-10 13:44:09.000000 zonesmart-utils-0.5.7/zonesmart_utils.egg-info/PKG-INFO
--rw-rw-r--   0 kamil     (1000) kamil     (1000)    10772 2024-04-10 13:44:09.000000 zonesmart-utils-0.5.7/zonesmart_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 kamil     (1000) kamil     (1000)        1 2024-04-10 13:44:09.000000 zonesmart-utils-0.5.7/zonesmart_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 kamil     (1000) kamil     (1000)      388 2024-04-10 13:44:09.000000 zonesmart-utils-0.5.7/zonesmart_utils.egg-info/requires.txt
--rw-rw-r--   0 kamil     (1000) kamil     (1000)        9 2024-04-10 13:44:09.000000 zonesmart-utils-0.5.7/zonesmart_utils.egg-info/top_level.txt
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.430038 zonesmart-utils-0.5.7/zs_utils/
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/__init__.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.430038 zonesmart-utils-0.5.7/zs_utils/api/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/__init__.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.430038 zonesmart-utils-0.5.7/zs_utils/api/aliexpress/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2193 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress/base_api.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.430038 zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/
--rw-r--r--   0 kamil     (1000) kamil     (1000)      209 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      609 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/category.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1352 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/dropshipping.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      360 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/freight_template.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      995 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/logistics.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      162 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/merchant.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1071 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/order.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     4000 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/product.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      223 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/service_template.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.434038 zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      503 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/base_api.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.434038 zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/core/
--rw-r--r--   0 kamil     (1000) kamil     (1000)      112 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/core/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1098 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/core/category.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1038 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/core/chat.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1720 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/core/order.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2966 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/core/product.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2918 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/core/shipment.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.434038 zonesmart-utils-0.5.7/zs_utils/api/amocrm/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-11-17 10:34:16.000000 zonesmart-utils-0.5.7/zs_utils/api/amocrm/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     5219 2023-11-17 10:34:16.000000 zonesmart-utils-0.5.7/zs_utils/api/amocrm/actions.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      124 2023-11-17 10:34:16.000000 zonesmart-utils-0.5.7/zs_utils/api/amocrm/apps.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     3497 2023-11-17 10:34:16.000000 zonesmart-utils-0.5.7/zs_utils/api/amocrm/base_action.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      423 2023-11-17 10:34:16.000000 zonesmart-utils-0.5.7/zs_utils/api/amocrm/base_api.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1978 2023-11-17 10:34:16.000000 zonesmart-utils-0.5.7/zs_utils/api/amocrm/core.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.434038 zonesmart-utils-0.5.7/zs_utils/api/amocrm/migrations/
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1771 2023-11-17 10:34:16.000000 zonesmart-utils-0.5.7/zs_utils/api/amocrm/migrations/0001_initial.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-11-17 10:34:16.000000 zonesmart-utils-0.5.7/zs_utils/api/amocrm/migrations/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1681 2023-11-17 10:34:16.000000 zonesmart-utils-0.5.7/zs_utils/api/amocrm/models.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     4718 2023-11-17 10:34:16.000000 zonesmart-utils-0.5.7/zs_utils/api/amocrm/services.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.434038 zonesmart-utils-0.5.7/zs_utils/api/apiship/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/apiship/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      548 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/apiship/base_api.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.434038 zonesmart-utils-0.5.7/zs_utils/api/apiship/core/
--rw-r--r--   0 kamil     (1000) kamil     (1000)      154 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/apiship/core/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      356 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/apiship/core/account.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1323 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/apiship/core/connection.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      354 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/apiship/core/label.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      354 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/apiship/core/lists.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1803 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/apiship/core/order.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      515 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/apiship/core/rate.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1511 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/apiship/core/status.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      120 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/apps.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)    20998 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/base_action.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     5542 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/base_api.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      980 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/constants.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.434038 zonesmart-utils-0.5.7/zs_utils/api/ebay/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       24 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/__init__.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.434038 zonesmart-utils-0.5.7/zs_utils/api/ebay/base_api/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       50 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/base_api/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     3190 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/base_api/new_api.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2824 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/base_api/trading_api.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.434038 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/
--rw-r--r--   0 kamil     (1000) kamil     (1000)      118 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/__init__.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.438038 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/commerce/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       71 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/commerce/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      701 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/commerce/catalog.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)      368 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/commerce/identity.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2946 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/commerce/taxonomy.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      664 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/developer.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1368 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/post_order.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.438038 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)      126 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/__init__.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.438038 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/account/
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)      113 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/account/__init__.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)      275 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/account/base.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1978 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/account/fulfillment_policy.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1858 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/account/payment_policy.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1828 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/account/return_policy.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.438038 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/fulfillment/
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)       88 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/fulfillment/__init__.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     4167 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/fulfillment/order.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     3281 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/fulfillment/payment_dispute.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1085 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/fulfillment/shipping_fulfillment.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.438038 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/inventory/
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)      114 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/inventory/__init__.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     3082 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/inventory/item.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1707 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/inventory/item_group.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)      299 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/inventory/listing.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     2284 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/inventory/location.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     2644 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/inventory/offer.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1232 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/metadata.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      641 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/negotiation.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.438038 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/
--rw-r--r--   0 kamil     (1000) kamil     (1000)      260 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2952 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/best_offer.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2081 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/billing.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1185 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/category.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      738 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/details.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      505 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/feedback.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      836 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/image.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      334 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/limits.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1823 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/listing.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     7317 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/messages.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     5466 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/notifications.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      426 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/store.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.438038 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/__init__.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.442038 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)      241 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      736 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/aspect_enums.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1389 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/common_enums.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     2791 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/listing_enums.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1060 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/message_enums.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1571 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/notification_enums.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     3189 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/order_enums.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1745 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/policy_enums.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     5709 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/shipping_carriers_enum.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.442038 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/marketplace/
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)      109 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/marketplace/__init__.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)      990 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/marketplace/marketplace_to_currency.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1429 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/marketplace/marketplace_to_host.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     2627 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/marketplace/marketplace_to_lang.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      538 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/data/marketplace/marketplace_to_site.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.442038 zonesmart-utils-0.5.7/zs_utils/api/ebay/mip/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/mip/__init__.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     4809 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/mip/sftp_get.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     2153 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/mip/sftp_put.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.442038 zonesmart-utils-0.5.7/zs_utils/api/ebay/oauth/
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/oauth/__init__.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1535 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/oauth/model.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     3163 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/oauth/oauth_client.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.442038 zonesmart-utils-0.5.7/zs_utils/api/ebay/utils/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       28 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/utils/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      873 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ebay/utils/custom_quote.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.442038 zonesmart-utils-0.5.7/zs_utils/api/etsy/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1174 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/base_api.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.442038 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/
--rw-r--r--   0 kamil     (1000) kamil     (1000)      259 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/__init__.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.442038 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/account/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       68 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/account/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1070 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/account/shop.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      795 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/account/shop_section.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      271 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/account/user.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      395 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/carrier.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      718 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/category.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.442038 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/listing/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       44 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/listing/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2270 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/listing/image.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     7978 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/listing/listing.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1466 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/receipt.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2168 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/shipping_profile.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2233 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/shipping_profile_destination.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1927 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/shipping_profile_upgrade.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      713 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/etsy/core/transaction.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.442038 zonesmart-utils-0.5.7/zs_utils/api/fedex/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/fedex/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      519 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/fedex/base_api.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.442038 zonesmart-utils-0.5.7/zs_utils/api/fedex/core/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       90 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/fedex/core/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1566 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/fedex/core/pickup.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      337 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/fedex/core/rate.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      692 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/fedex/core/shipment.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      256 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/fedex/core/tracking.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      724 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/filters.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.442038 zonesmart-utils-0.5.7/zs_utils/api/insales/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/insales/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      549 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/insales/base_api.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.446038 zonesmart-utils-0.5.7/zs_utils/api/insales/core/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       90 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/insales/core/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      215 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/insales/core/category.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      541 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/insales/core/order.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      467 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/insales/core/policy.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      555 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/insales/core/product.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.446038 zonesmart-utils-0.5.7/zs_utils/api/kokoc_crm/
--rw-rw-r--   0 kamil     (1000) kamil     (1000)        0 2023-09-12 18:56:10.000000 zonesmart-utils-0.5.7/zs_utils/api/kokoc_crm/__init__.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1589 2024-02-22 16:18:00.000000 zonesmart-utils-0.5.7/zs_utils/api/kokoc_crm/constants.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     7658 2024-03-22 07:13:16.000000 zonesmart-utils-0.5.7/zs_utils/api/kokoc_crm/services.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.446038 zonesmart-utils-0.5.7/zs_utils/api/migrations/
--rw-r--r--   0 kamil     (1000) kamil     (1000)     4222 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/migrations/0001_initial.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/migrations/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2219 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/models.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.446038 zonesmart-utils-0.5.7/zs_utils/api/ozon/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ozon/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1002 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ozon/base_api.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.446038 zonesmart-utils-0.5.7/zs_utils/api/ozon/core/
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)      157 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ozon/core/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      593 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ozon/core/act.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)      954 2024-03-20 11:57:21.000000 zonesmart-utils-0.5.7/zs_utils/api/ozon/core/category.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1532 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ozon/core/chat.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     2832 2024-03-20 11:57:21.000000 zonesmart-utils-0.5.7/zs_utils/api/ozon/core/listing.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      238 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ozon/core/report.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     3197 2024-02-22 16:09:57.000000 zonesmart-utils-0.5.7/zs_utils/api/ozon/core/shipment.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      301 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/ozon/core/warehouse.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      956 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/serializers.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     3801 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/services.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.450038 zonesmart-utils-0.5.7/zs_utils/api/shipstation/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shipstation/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      444 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shipstation/base_api.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.450038 zonesmart-utils-0.5.7/zs_utils/api/shipstation/core/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       67 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shipstation/core/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      328 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shipstation/core/carrier.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      559 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shipstation/core/rate.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      938 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shipstation/core/shipment.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.450038 zonesmart-utils-0.5.7/zs_utils/api/shopify/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      734 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/base_api.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.450038 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/
--rw-r--r--   0 kamil     (1000) kamil     (1000)      114 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/__init__.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.450038 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/account/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       44 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/account/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      527 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/account/location.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      364 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/account/shop.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.450038 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/listing/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       92 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/listing/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1957 2023-11-17 10:22:48.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/listing/image.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      903 2023-11-17 10:22:48.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/listing/inventory.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2938 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/listing/product.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1680 2023-11-17 10:22:48.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/listing/variant.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2918 2023-11-17 10:22:48.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/order.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1872 2023-11-17 10:22:48.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/shipment.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1410 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/shopify/core/webhook.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.450038 zonesmart-utils-0.5.7/zs_utils/api/utils/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       31 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/utils/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      683 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/utils/response_keeper.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      468 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/views.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.450038 zonesmart-utils-0.5.7/zs_utils/api/wildberries/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/wildberries/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      971 2023-09-14 11:58:33.000000 zonesmart-utils-0.5.7/zs_utils/api/wildberries/base_api.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.454038 zonesmart-utils-0.5.7/zs_utils/api/wildberries/core/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       93 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/wildberries/core/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1815 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/wildberries/core/category.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2843 2024-04-10 13:41:30.000000 zonesmart-utils-0.5.7/zs_utils/api/wildberries/core/listing.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     4213 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/wildberries/core/order.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1143 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/wildberries/core/warehouse.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.454038 zonesmart-utils-0.5.7/zs_utils/api/yandex_market/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yandex_market/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      813 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yandex_market/base_api.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.454038 zonesmart-utils-0.5.7/zs_utils/api/yandex_market/core/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       64 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yandex_market/core/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      340 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yandex_market/core/listing.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     4417 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yandex_market/core/order.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     3269 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yandex_market/core/shop.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.454038 zonesmart-utils-0.5.7/zs_utils/api/yookassa/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yookassa/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     3054 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yookassa/base_action.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     5654 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yookassa/constants.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.454038 zonesmart-utils-0.5.7/zs_utils/api/yookassa/core/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       87 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yookassa/core/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     3009 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yookassa/core/payment_create.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      590 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yookassa/core/payment_get.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2233 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yookassa/core/payment_refund.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     7230 2023-11-17 10:25:58.000000 zonesmart-utils-0.5.7/zs_utils/api/yookassa/services.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2436 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/api/yookassa/views.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      662 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/captcha.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     8147 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/compare_data.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     3615 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/currency_converter.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.454038 zonesmart-utils-0.5.7/zs_utils/data/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/data/__init__.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.454038 zonesmart-utils-0.5.7/zs_utils/data/enums/
--rw-r--r--   0 kamil     (1000) kamil     (1000)      137 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/data/enums/__init__.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)    14709 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/data/enums/country.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)    14881 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/data/enums/currency.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      739 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/data/enums/files.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     7295 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/data/enums/language.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      839 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/data/enums/unit.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1682 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/data/enums/usa_state.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     3070 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/dict_converter.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     6562 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/exceptions.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1398 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/file_io.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      866 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/function_timeout.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      732 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/get_file_extension.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      331 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/html_utils.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2802 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/import_utils.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1889 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/inspect_func.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     4053 2024-03-22 07:15:22.000000 zonesmart-utils-0.5.7/zs_utils/json_utils.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      652 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/permissions.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      968 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/s3_storage_backend.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2401 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/time_utils.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2285 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/transliterate.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.454038 zonesmart-utils-0.5.7/zs_utils/unit_converter/
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)       47 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/unit_converter/__init__.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1531 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/unit_converter/converter.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     3855 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/unit_converter/data.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)      615 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/unit_converter/exceptions.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1984 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/unit_converter/parser.py
--rwxr-xr-x   0 kamil     (1000) kamil     (1000)     6952 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/unit_converter/units.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.458038 zonesmart-utils-0.5.7/zs_utils/user/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/user/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      114 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/user/apps.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.458038 zonesmart-utils-0.5.7/zs_utils/user/migrations/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/user/migrations/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2469 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/user/models.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      626 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/user/utils.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.458038 zonesmart-utils-0.5.7/zs_utils/views/
--rw-r--r--   0 kamil     (1000) kamil     (1000)       42 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/views/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     6117 2023-12-15 10:00:15.000000 zonesmart-utils-0.5.7/zs_utils/views/core.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     7394 2023-09-08 13:42:12.000000 zonesmart-utils-0.5.7/zs_utils/views/mixins.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.458038 zonesmart-utils-0.5.7/zs_utils/websocket/
--rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/websocket/__init__.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     7453 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/websocket/consumer.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1919 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/websocket/middleware.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     2419 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/websocket/services.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      667 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/websocket/tasks.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     4325 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.7/zs_utils/xml_parser.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.458038 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/
--rw-rw-r--   0 kamil     (1000) kamil     (1000)       65 2023-12-29 09:36:21.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/__init__.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)      277 2023-11-17 10:49:05.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/exceptions.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.458038 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1064 2023-11-17 10:49:05.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/__init__.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     4895 2023-11-17 15:38:02.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/abstract.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     2101 2023-11-17 15:38:02.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/age.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)      982 2023-11-17 10:49:05.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/category.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1583 2023-11-17 15:38:02.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/condition.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     2214 2023-11-17 15:38:02.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/currency.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1352 2023-11-17 10:49:05.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/dimensions.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1229 2023-11-17 10:49:05.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/feed.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 13:44:09.458038 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/fields/
--rw-rw-r--   0 kamil     (1000) kamil     (1000)      103 2023-11-17 10:49:05.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/fields/__init__.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1318 2023-11-17 15:38:02.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/fields/enable_auto_discounts.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)      600 2023-11-17 10:49:05.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/fields/options.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)      251 2023-11-17 10:49:05.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/fields/outlets.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)      310 2023-11-17 10:49:05.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/fields/year.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1427 2023-11-17 15:38:02.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/gift.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)    30099 2023-11-17 15:38:02.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/offers.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1084 2023-11-17 10:49:05.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/option.py
--rw-r--r--   0 kamil     (1000) kamil     (1000)     1051 2023-11-17 10:49:05.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/outlet.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1231 2023-11-17 15:38:02.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/parameter.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1592 2023-11-17 10:49:05.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/price.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     5740 2023-11-17 15:38:02.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/promo.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     8300 2023-11-17 15:38:02.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/shop.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1321 2023-11-17 15:38:02.000000 zonesmart-utils-0.5.7/zs_utils/yandex_market_language/yml.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.972758 zonesmart-utils-0.5.8/
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      110 2024-04-10 18:25:04.972758 zonesmart-utils-0.5.8/PKG-INFO
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        9 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.8/README.md
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      368 2023-08-21 11:30:30.000000 zonesmart-utils-0.5.8/pyproject.toml
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      209 2024-04-10 18:25:04.972758 zonesmart-utils-0.5.8/setup.cfg
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      529 2024-04-10 18:24:23.000000 zonesmart-utils-0.5.8/setup.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.944758 zonesmart-utils-0.5.8/zonesmart_utils.egg-info/
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      110 2024-04-10 18:25:04.000000 zonesmart-utils-0.5.8/zonesmart_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)    10811 2024-04-10 18:25:04.000000 zonesmart-utils-0.5.8/zonesmart_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)        1 2024-04-10 18:25:04.000000 zonesmart-utils-0.5.8/zonesmart_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      388 2024-04-10 18:25:04.000000 zonesmart-utils-0.5.8/zonesmart_utils.egg-info/requires.txt
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)        9 2024-04-10 18:25:04.000000 zonesmart-utils-0.5.8/zonesmart_utils.egg-info/top_level.txt
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.948758 zonesmart-utils-0.5.8/zs_utils/
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/__init__.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.948758 zonesmart-utils-0.5.8/zs_utils/api/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/__init__.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.948758 zonesmart-utils-0.5.8/zs_utils/api/aliexpress/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2193 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress/base_api.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.948758 zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      209 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      609 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/category.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1352 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/dropshipping.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      360 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/freight_template.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      995 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/logistics.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      162 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/merchant.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1071 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/order.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     4000 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/product.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      223 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/service_template.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.948758 zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      503 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/base_api.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.952758 zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/core/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      112 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/core/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1098 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/core/category.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1038 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/core/chat.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1720 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/core/order.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2966 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/core/product.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2918 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/core/shipment.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.952758 zonesmart-utils-0.5.8/zs_utils/api/amocrm/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/amocrm/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     5219 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/amocrm/actions.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      124 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/amocrm/apps.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     3497 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/amocrm/base_action.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      423 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/amocrm/base_api.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1978 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/amocrm/core.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.952758 zonesmart-utils-0.5.8/zs_utils/api/amocrm/migrations/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1771 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/amocrm/migrations/0001_initial.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/amocrm/migrations/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1681 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/amocrm/models.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     4718 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/amocrm/services.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.952758 zonesmart-utils-0.5.8/zs_utils/api/apiship/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/apiship/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      548 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/apiship/base_api.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.952758 zonesmart-utils-0.5.8/zs_utils/api/apiship/core/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      154 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/apiship/core/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      356 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/apiship/core/account.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1323 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/apiship/core/connection.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      354 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/apiship/core/label.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      354 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/apiship/core/lists.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1803 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/apiship/core/order.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      515 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/apiship/core/rate.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1511 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/apiship/core/status.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      120 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/apps.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)    21005 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/base_action.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     5542 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/base_api.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      980 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/constants.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.952758 zonesmart-utils-0.5.8/zs_utils/api/ebay/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       24 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/__init__.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.952758 zonesmart-utils-0.5.8/zs_utils/api/ebay/base_api/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       50 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/base_api/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     3190 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/base_api/new_api.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2824 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/base_api/trading_api.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.952758 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      118 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/__init__.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.952758 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/commerce/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       71 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/commerce/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      701 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/commerce/catalog.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)      368 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/commerce/identity.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2946 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/commerce/taxonomy.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      664 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/developer.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1368 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/post_order.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.952758 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)      126 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/__init__.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.956758 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/account/
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)      113 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/account/__init__.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)      275 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/account/base.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1978 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/account/fulfillment_policy.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1858 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/account/payment_policy.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1828 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/account/return_policy.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.956758 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/fulfillment/
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)       88 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/fulfillment/__init__.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     4167 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/fulfillment/order.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     3281 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/fulfillment/payment_dispute.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1085 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/fulfillment/shipping_fulfillment.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.956758 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/inventory/
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)      114 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/inventory/__init__.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     3082 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/inventory/item.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1707 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/inventory/item_group.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)      299 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/inventory/listing.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     2284 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/inventory/location.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     2644 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/inventory/offer.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1232 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/metadata.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      641 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/negotiation.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.956758 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      260 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2952 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/best_offer.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2081 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/billing.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1185 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/category.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      738 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/details.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      505 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/feedback.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      836 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/image.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      334 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/limits.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1823 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/listing.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     7317 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/messages.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     5466 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/notifications.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      426 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/store.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.956758 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/__init__.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.956758 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)      241 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      736 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/aspect_enums.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1389 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/common_enums.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     2791 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/listing_enums.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1060 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/message_enums.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1571 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/notification_enums.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     3189 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/order_enums.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1745 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/policy_enums.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     5709 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/shipping_carriers_enum.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.956758 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/marketplace/
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)      109 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/marketplace/__init__.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)      990 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/marketplace/marketplace_to_currency.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1429 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/marketplace/marketplace_to_host.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     2627 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/marketplace/marketplace_to_lang.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      538 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/data/marketplace/marketplace_to_site.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.960758 zonesmart-utils-0.5.8/zs_utils/api/ebay/mip/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/mip/__init__.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     4809 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/mip/sftp_get.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     2153 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/mip/sftp_put.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.960758 zonesmart-utils-0.5.8/zs_utils/api/ebay/oauth/
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/oauth/__init__.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1535 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/oauth/model.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     3163 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/oauth/oauth_client.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.960758 zonesmart-utils-0.5.8/zs_utils/api/ebay/utils/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       28 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/utils/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      873 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ebay/utils/custom_quote.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.960758 zonesmart-utils-0.5.8/zs_utils/api/etsy/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1174 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/base_api.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.960758 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      259 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/__init__.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.960758 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/account/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       68 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/account/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1070 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/account/shop.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      795 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/account/shop_section.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      271 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/account/user.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      395 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/carrier.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      718 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/category.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.960758 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/listing/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       44 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/listing/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2270 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/listing/image.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     7978 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/listing/listing.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1466 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/receipt.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2168 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/shipping_profile.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2233 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/shipping_profile_destination.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1927 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/shipping_profile_upgrade.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      713 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/etsy/core/transaction.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.960758 zonesmart-utils-0.5.8/zs_utils/api/fedex/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/fedex/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      519 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/fedex/base_api.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.960758 zonesmart-utils-0.5.8/zs_utils/api/fedex/core/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       90 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/fedex/core/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1566 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/fedex/core/pickup.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      337 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/fedex/core/rate.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      692 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/fedex/core/shipment.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      256 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/fedex/core/tracking.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      724 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/filters.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.960758 zonesmart-utils-0.5.8/zs_utils/api/insales/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/insales/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      549 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/insales/base_api.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.960758 zonesmart-utils-0.5.8/zs_utils/api/insales/core/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       90 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/insales/core/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      215 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/insales/core/category.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      541 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/insales/core/order.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      467 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/insales/core/policy.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      555 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/insales/core/product.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.960758 zonesmart-utils-0.5.8/zs_utils/api/kokoc_crm/
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/kokoc_crm/__init__.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     1589 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/kokoc_crm/constants.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     7658 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/kokoc_crm/services.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.964758 zonesmart-utils-0.5.8/zs_utils/api/migrations/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     4222 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/migrations/0001_initial.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/migrations/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2219 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/models.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.964758 zonesmart-utils-0.5.8/zs_utils/api/ozon/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ozon/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1002 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ozon/base_api.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.964758 zonesmart-utils-0.5.8/zs_utils/api/ozon/core/
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)      157 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ozon/core/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      593 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ozon/core/act.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      954 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ozon/core/category.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1532 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ozon/core/chat.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     2832 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ozon/core/listing.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      238 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ozon/core/report.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     3197 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ozon/core/shipment.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      301 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/ozon/core/warehouse.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      956 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/serializers.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     3801 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/services.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.964758 zonesmart-utils-0.5.8/zs_utils/api/shipstation/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shipstation/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      444 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shipstation/base_api.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.964758 zonesmart-utils-0.5.8/zs_utils/api/shipstation/core/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       67 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shipstation/core/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      328 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shipstation/core/carrier.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      559 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shipstation/core/rate.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      938 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shipstation/core/shipment.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.964758 zonesmart-utils-0.5.8/zs_utils/api/shopify/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      734 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/base_api.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.964758 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      114 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/__init__.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.964758 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/account/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       44 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/account/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      527 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/account/location.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      364 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/account/shop.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.964758 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/listing/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       92 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/listing/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1957 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/listing/image.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      903 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/listing/inventory.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2938 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/listing/product.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1680 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/listing/variant.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2918 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/order.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1872 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/shipment.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1410 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/shopify/core/webhook.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.964758 zonesmart-utils-0.5.8/zs_utils/api/utils/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       31 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/utils/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      683 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/utils/response_keeper.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      468 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/views.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.964758 zonesmart-utils-0.5.8/zs_utils/api/wildberries/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/wildberries/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      971 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/wildberries/base_api.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.968758 zonesmart-utils-0.5.8/zs_utils/api/wildberries/core/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      114 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/wildberries/core/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1815 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/wildberries/core/category.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2260 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/wildberries/core/listing.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     4213 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/wildberries/core/order.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      762 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/wildberries/core/price.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1143 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/wildberries/core/warehouse.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.968758 zonesmart-utils-0.5.8/zs_utils/api/yandex_market/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yandex_market/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      813 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yandex_market/base_api.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.968758 zonesmart-utils-0.5.8/zs_utils/api/yandex_market/core/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       64 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yandex_market/core/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      340 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yandex_market/core/listing.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     4417 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yandex_market/core/order.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     3269 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yandex_market/core/shop.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.968758 zonesmart-utils-0.5.8/zs_utils/api/yookassa/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yookassa/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     3054 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yookassa/base_action.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     5654 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yookassa/constants.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.968758 zonesmart-utils-0.5.8/zs_utils/api/yookassa/core/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       87 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yookassa/core/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     3009 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yookassa/core/payment_create.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      590 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yookassa/core/payment_get.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2233 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yookassa/core/payment_refund.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     7230 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yookassa/services.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2436 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/api/yookassa/views.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      662 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/captcha.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     8147 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/compare_data.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     3615 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/currency_converter.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.968758 zonesmart-utils-0.5.8/zs_utils/data/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/data/__init__.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.968758 zonesmart-utils-0.5.8/zs_utils/data/enums/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      137 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/data/enums/__init__.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)    14709 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/data/enums/country.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)    14881 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/data/enums/currency.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      739 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/data/enums/files.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     7295 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/data/enums/language.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      839 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/data/enums/unit.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1682 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/data/enums/usa_state.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     3070 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/dict_converter.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     6666 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/exceptions.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1398 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/file_io.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      866 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/function_timeout.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      732 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/get_file_extension.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      331 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/html_utils.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2802 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/import_utils.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1889 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/inspect_func.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     4053 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/json_utils.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      652 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/permissions.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      968 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/s3_storage_backend.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2401 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/time_utils.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2285 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/transliterate.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.968758 zonesmart-utils-0.5.8/zs_utils/unit_converter/
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)       47 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/unit_converter/__init__.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1531 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/unit_converter/converter.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     3855 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/unit_converter/data.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)      615 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/unit_converter/exceptions.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     1984 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/unit_converter/parser.py
+-rwxr-xr-x   0 kamil     (1000) kamil     (1000)     6952 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/unit_converter/units.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.968758 zonesmart-utils-0.5.8/zs_utils/user/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/user/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      114 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/user/apps.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.968758 zonesmart-utils-0.5.8/zs_utils/user/migrations/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/user/migrations/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2469 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/user/models.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      626 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/user/utils.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.968758 zonesmart-utils-0.5.8/zs_utils/views/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)       42 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/views/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     6117 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/views/core.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     7394 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/views/mixins.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.972758 zonesmart-utils-0.5.8/zs_utils/websocket/
+-rw-r--r--   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/websocket/__init__.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     7453 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/websocket/consumer.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1919 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/websocket/middleware.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     2419 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/websocket/services.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      667 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/websocket/tasks.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     4325 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/xml_parser.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.972758 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)       65 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/__init__.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      277 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/exceptions.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.972758 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     1064 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/__init__.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     4895 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/abstract.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     2101 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/age.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      982 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/category.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     1583 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/condition.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     2214 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/currency.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     1352 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/dimensions.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     1229 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/feed.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2024-04-10 18:25:04.972758 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/fields/
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      103 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/fields/__init__.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     1318 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/fields/enable_auto_discounts.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      600 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/fields/options.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)      251 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/fields/outlets.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      310 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/fields/year.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     1427 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/gift.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)    30099 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/offers.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     1084 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/option.py
+-rw-r--r--   0 kamil     (1000) kamil     (1000)     1051 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/outlet.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     1231 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/parameter.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     1592 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/price.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     5740 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/promo.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     8300 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/shop.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     1321 2024-04-10 18:23:47.000000 zonesmart-utils-0.5.8/zs_utils/yandex_market_language/yml.py
```

### Comparing `zonesmart-utils-0.5.7/setup.py` & `zonesmart-utils-0.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,13 +9,13 @@
             if line:
                 reqs.append(line)
     return reqs
 
 
 setup(
     name="zonesmart-utils",
-    version="0.5.7",
+    version="0.5.8",
     author="Zonesmart",
     author_email="kamil@zonesmart.ru",
     packages=find_packages(include=["zs_utils", "zs_utils.*"]),
     install_requires=parse_requirements(),
 )
```

### Comparing `zonesmart-utils-0.5.7/zonesmart_utils.egg-info/SOURCES.txt` & `zonesmart-utils-0.5.8/zonesmart_utils.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,15 @@
 zs_utils/api/utils/response_keeper.py
 zs_utils/api/wildberries/__init__.py
 zs_utils/api/wildberries/base_api.py
 zs_utils/api/wildberries/core/__init__.py
 zs_utils/api/wildberries/core/category.py
 zs_utils/api/wildberries/core/listing.py
 zs_utils/api/wildberries/core/order.py
+zs_utils/api/wildberries/core/price.py
 zs_utils/api/wildberries/core/warehouse.py
 zs_utils/api/yandex_market/__init__.py
 zs_utils/api/yandex_market/base_api.py
 zs_utils/api/yandex_market/core/__init__.py
 zs_utils/api/yandex_market/core/listing.py
 zs_utils/api/yandex_market/core/order.py
 zs_utils/api/yandex_market/core/shop.py
```

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/aliexpress/base_api.py` & `zonesmart-utils-0.5.8/zs_utils/api/aliexpress/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/category.py` & `zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/category.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/dropshipping.py` & `zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/dropshipping.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/logistics.py` & `zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/logistics.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/order.py` & `zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/aliexpress/core/product.py` & `zonesmart-utils-0.5.8/zs_utils/api/aliexpress/core/product.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/core/category.py` & `zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/core/category.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/core/chat.py` & `zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/core/chat.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/core/order.py` & `zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/core/product.py` & `zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/core/product.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/aliexpress_russia/core/shipment.py` & `zonesmart-utils-0.5.8/zs_utils/api/aliexpress_russia/core/shipment.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/amocrm/actions.py` & `zonesmart-utils-0.5.8/zs_utils/api/amocrm/actions.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/amocrm/base_action.py` & `zonesmart-utils-0.5.8/zs_utils/api/amocrm/base_action.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/amocrm/core.py` & `zonesmart-utils-0.5.8/zs_utils/api/amocrm/core.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/amocrm/migrations/0001_initial.py` & `zonesmart-utils-0.5.8/zs_utils/api/amocrm/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/amocrm/models.py` & `zonesmart-utils-0.5.8/zs_utils/api/amocrm/models.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/amocrm/services.py` & `zonesmart-utils-0.5.8/zs_utils/api/amocrm/services.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/apiship/base_api.py` & `zonesmart-utils-0.5.8/zs_utils/api/apiship/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/apiship/core/connection.py` & `zonesmart-utils-0.5.8/zs_utils/api/apiship/core/connection.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/apiship/core/order.py` & `zonesmart-utils-0.5.8/zs_utils/api/apiship/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/apiship/core/rate.py` & `zonesmart-utils-0.5.8/zs_utils/api/apiship/core/rate.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/apiship/core/status.py` & `zonesmart-utils-0.5.8/zs_utils/api/apiship/core/status.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/base_action.py` & `zonesmart-utils-0.5.8/zs_utils/api/base_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,15 +509,15 @@
         if self.instance:
             self.instance.incr_request_counter()
 
     def response_is_success(
         self,
         results: dict,
         response: requests.Response,
-        exception: CustomException = None,
+        exception: CustomException | None = None,
     ) -> bool:
         """
         Проверка, что запрос успешный
         """
         if exception is not None:
             return False
         if response is not None:
```

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/base_api.py` & `zonesmart-utils-0.5.8/zs_utils/api/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/constants.py` & `zonesmart-utils-0.5.8/zs_utils/api/constants.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/base_api/new_api.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/base_api/new_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/base_api/trading_api.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/base_api/trading_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/commerce/catalog.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/commerce/catalog.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/commerce/taxonomy.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/commerce/taxonomy.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/developer.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/developer.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/post_order.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/post_order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/account/fulfillment_policy.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/account/fulfillment_policy.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/account/payment_policy.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/account/payment_policy.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/account/return_policy.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/account/return_policy.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/fulfillment/order.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/fulfillment/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/fulfillment/payment_dispute.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/fulfillment/payment_dispute.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/fulfillment/shipping_fulfillment.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/fulfillment/shipping_fulfillment.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/inventory/item.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/inventory/item.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/inventory/item_group.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/inventory/item_group.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/inventory/location.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/inventory/location.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/inventory/offer.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/inventory/offer.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/metadata.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/metadata.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/sell/negotiation.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/sell/negotiation.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/best_offer.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/best_offer.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/billing.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/billing.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/category.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/category.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/details.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/details.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/image.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/image.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/listing.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/listing.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/messages.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/messages.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/core/trading/notifications.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/core/trading/notifications.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/aspect_enums.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/aspect_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/common_enums.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/common_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/listing_enums.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/listing_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/message_enums.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/message_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/notification_enums.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/notification_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/order_enums.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/order_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/policy_enums.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/policy_enums.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/data/enums/shipping_carriers_enum.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/data/enums/shipping_carriers_enum.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/data/marketplace/marketplace_to_currency.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/data/marketplace/marketplace_to_currency.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/data/marketplace/marketplace_to_host.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/data/marketplace/marketplace_to_host.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/data/marketplace/marketplace_to_lang.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/data/marketplace/marketplace_to_lang.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/data/marketplace/marketplace_to_site.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/data/marketplace/marketplace_to_site.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/mip/sftp_get.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/mip/sftp_get.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/mip/sftp_put.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/mip/sftp_put.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/oauth/model.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/oauth/model.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/oauth/oauth_client.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/oauth/oauth_client.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ebay/utils/custom_quote.py` & `zonesmart-utils-0.5.8/zs_utils/api/ebay/utils/custom_quote.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/etsy/base_api.py` & `zonesmart-utils-0.5.8/zs_utils/api/etsy/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/etsy/core/account/shop.py` & `zonesmart-utils-0.5.8/zs_utils/api/etsy/core/account/shop.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/etsy/core/account/shop_section.py` & `zonesmart-utils-0.5.8/zs_utils/api/etsy/core/account/shop_section.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/etsy/core/category.py` & `zonesmart-utils-0.5.8/zs_utils/api/etsy/core/category.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/etsy/core/listing/image.py` & `zonesmart-utils-0.5.8/zs_utils/api/etsy/core/listing/image.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/etsy/core/listing/listing.py` & `zonesmart-utils-0.5.8/zs_utils/api/etsy/core/listing/listing.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/etsy/core/receipt.py` & `zonesmart-utils-0.5.8/zs_utils/api/etsy/core/receipt.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/etsy/core/shipping_profile.py` & `zonesmart-utils-0.5.8/zs_utils/api/etsy/core/shipping_profile.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/etsy/core/shipping_profile_destination.py` & `zonesmart-utils-0.5.8/zs_utils/api/etsy/core/shipping_profile_destination.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/etsy/core/shipping_profile_upgrade.py` & `zonesmart-utils-0.5.8/zs_utils/api/etsy/core/shipping_profile_upgrade.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/etsy/core/transaction.py` & `zonesmart-utils-0.5.8/zs_utils/api/etsy/core/transaction.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/fedex/base_api.py` & `zonesmart-utils-0.5.8/zs_utils/api/fedex/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/fedex/core/pickup.py` & `zonesmart-utils-0.5.8/zs_utils/api/fedex/core/pickup.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/fedex/core/shipment.py` & `zonesmart-utils-0.5.8/zs_utils/api/fedex/core/shipment.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/filters.py` & `zonesmart-utils-0.5.8/zs_utils/api/filters.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/insales/base_api.py` & `zonesmart-utils-0.5.8/zs_utils/api/insales/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/insales/core/order.py` & `zonesmart-utils-0.5.8/zs_utils/api/insales/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/insales/core/product.py` & `zonesmart-utils-0.5.8/zs_utils/api/insales/core/product.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/kokoc_crm/constants.py` & `zonesmart-utils-0.5.8/zs_utils/api/kokoc_crm/constants.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/kokoc_crm/services.py` & `zonesmart-utils-0.5.8/zs_utils/api/kokoc_crm/services.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/migrations/0001_initial.py` & `zonesmart-utils-0.5.8/zs_utils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/models.py` & `zonesmart-utils-0.5.8/zs_utils/api/models.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ozon/base_api.py` & `zonesmart-utils-0.5.8/zs_utils/api/ozon/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ozon/core/act.py` & `zonesmart-utils-0.5.8/zs_utils/api/ozon/core/act.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ozon/core/category.py` & `zonesmart-utils-0.5.8/zs_utils/api/ozon/core/category.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ozon/core/chat.py` & `zonesmart-utils-0.5.8/zs_utils/api/ozon/core/chat.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ozon/core/listing.py` & `zonesmart-utils-0.5.8/zs_utils/api/ozon/core/listing.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/ozon/core/shipment.py` & `zonesmart-utils-0.5.8/zs_utils/api/ozon/core/shipment.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/serializers.py` & `zonesmart-utils-0.5.8/zs_utils/api/serializers.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/services.py` & `zonesmart-utils-0.5.8/zs_utils/api/services.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/shipstation/core/rate.py` & `zonesmart-utils-0.5.8/zs_utils/api/shipstation/core/rate.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/shipstation/core/shipment.py` & `zonesmart-utils-0.5.8/zs_utils/api/shipstation/core/shipment.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/shopify/base_api.py` & `zonesmart-utils-0.5.8/zs_utils/api/shopify/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/shopify/core/account/location.py` & `zonesmart-utils-0.5.8/zs_utils/api/shopify/core/account/location.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/shopify/core/listing/image.py` & `zonesmart-utils-0.5.8/zs_utils/api/shopify/core/listing/image.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/shopify/core/listing/inventory.py` & `zonesmart-utils-0.5.8/zs_utils/api/shopify/core/listing/inventory.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/shopify/core/listing/product.py` & `zonesmart-utils-0.5.8/zs_utils/api/shopify/core/listing/product.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/shopify/core/listing/variant.py` & `zonesmart-utils-0.5.8/zs_utils/api/shopify/core/listing/variant.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/shopify/core/order.py` & `zonesmart-utils-0.5.8/zs_utils/api/shopify/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/shopify/core/shipment.py` & `zonesmart-utils-0.5.8/zs_utils/api/shopify/core/shipment.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/shopify/core/webhook.py` & `zonesmart-utils-0.5.8/zs_utils/api/shopify/core/webhook.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/utils/response_keeper.py` & `zonesmart-utils-0.5.8/zs_utils/api/utils/response_keeper.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/wildberries/base_api.py` & `zonesmart-utils-0.5.8/zs_utils/api/wildberries/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/wildberries/core/category.py` & `zonesmart-utils-0.5.8/zs_utils/api/wildberries/core/category.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/wildberries/core/listing.py` & `zonesmart-utils-0.5.8/zs_utils/api/wildberries/core/listing.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,35 +17,14 @@
     """
 
     http_method = "POST"
     resource_method = "content/v1/cards/filter"
     required_params = ["vendorCodes"]
 
 
-class GetWildberriesPrices(WildberriesAPI):
-    """
-    https://openapi.wb.ru/prices/api/ru/#tag/Spiski-tovarov/paths/~1api~1v2~1list~1goods~1filter/get
-    """
-
-    http_method = "GET"
-    resource_method = "api/v2/list/goods/filter"
-    required_params = ["limit"]
-    allowed_params = ["offset", "filterNmID"]
-
-
-class UpdateWildberriesPrices(WildberriesAPI):
-    """
-    https://openapi.wb.ru/prices/api/ru/#tag/Ustanovka-cen-i-skidok/paths/~1api~1v2~1upload~1task/post
-    """
-
-    http_method = "POST"
-    resource_method = "api/v2/upload/task"
-    required_params = ["data"]
-
-
 class CreateWildberriesBarcodes(WildberriesAPI):
     """
     https://openapi.wb.ru/#tag/Kontent-Prosmotr/paths/~1content~1v1~1barcodes/post
     """
 
     http_method = "POST"
     resource_method = "content/v1/barcodes"
```

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/wildberries/core/order.py` & `zonesmart-utils-0.5.8/zs_utils/api/wildberries/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/wildberries/core/warehouse.py` & `zonesmart-utils-0.5.8/zs_utils/api/wildberries/core/warehouse.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/yandex_market/base_api.py` & `zonesmart-utils-0.5.8/zs_utils/api/yandex_market/base_api.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/yandex_market/core/order.py` & `zonesmart-utils-0.5.8/zs_utils/api/yandex_market/core/order.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/yandex_market/core/shop.py` & `zonesmart-utils-0.5.8/zs_utils/api/yandex_market/core/shop.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/yookassa/base_action.py` & `zonesmart-utils-0.5.8/zs_utils/api/yookassa/base_action.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/yookassa/constants.py` & `zonesmart-utils-0.5.8/zs_utils/api/yookassa/constants.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/yookassa/core/payment_create.py` & `zonesmart-utils-0.5.8/zs_utils/api/yookassa/core/payment_create.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/yookassa/core/payment_get.py` & `zonesmart-utils-0.5.8/zs_utils/api/yookassa/core/payment_get.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/yookassa/core/payment_refund.py` & `zonesmart-utils-0.5.8/zs_utils/api/yookassa/core/payment_refund.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/yookassa/services.py` & `zonesmart-utils-0.5.8/zs_utils/api/yookassa/services.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/api/yookassa/views.py` & `zonesmart-utils-0.5.8/zs_utils/api/yookassa/views.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/captcha.py` & `zonesmart-utils-0.5.8/zs_utils/captcha.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/compare_data.py` & `zonesmart-utils-0.5.8/zs_utils/compare_data.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/currency_converter.py` & `zonesmart-utils-0.5.8/zs_utils/currency_converter.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/data/enums/country.py` & `zonesmart-utils-0.5.8/zs_utils/data/enums/country.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/data/enums/currency.py` & `zonesmart-utils-0.5.8/zs_utils/data/enums/currency.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/data/enums/files.py` & `zonesmart-utils-0.5.8/zs_utils/data/enums/files.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/data/enums/language.py` & `zonesmart-utils-0.5.8/zs_utils/data/enums/language.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/data/enums/unit.py` & `zonesmart-utils-0.5.8/zs_utils/data/enums/unit.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/data/enums/usa_state.py` & `zonesmart-utils-0.5.8/zs_utils/data/enums/usa_state.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/dict_converter.py` & `zonesmart-utils-0.5.8/zs_utils/dict_converter.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/exceptions.py` & `zonesmart-utils-0.5.8/zs_utils/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,17 @@
             message += str(self.message)
         elif self.messages:
             message += "; ".join(self.messages)
 
         if self.message_dict:
             message += "\n" + pretty_json(data=self.message_dict)
 
+        if (not message) and (self.response_code):
+            message = f"Code: {self.response_code}"
+
         return message
 
     def __repr__(self) -> str:
         val = ""
         if self.messages:
             val = f"messages={self.messages}"
         elif self.message:
```

### Comparing `zonesmart-utils-0.5.7/zs_utils/file_io.py` & `zonesmart-utils-0.5.8/zs_utils/file_io.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/function_timeout.py` & `zonesmart-utils-0.5.8/zs_utils/function_timeout.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/get_file_extension.py` & `zonesmart-utils-0.5.8/zs_utils/get_file_extension.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/import_utils.py` & `zonesmart-utils-0.5.8/zs_utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/inspect_func.py` & `zonesmart-utils-0.5.8/zs_utils/inspect_func.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/json_utils.py` & `zonesmart-utils-0.5.8/zs_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/permissions.py` & `zonesmart-utils-0.5.8/zs_utils/permissions.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/s3_storage_backend.py` & `zonesmart-utils-0.5.8/zs_utils/s3_storage_backend.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/time_utils.py` & `zonesmart-utils-0.5.8/zs_utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/transliterate.py` & `zonesmart-utils-0.5.8/zs_utils/transliterate.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/unit_converter/converter.py` & `zonesmart-utils-0.5.8/zs_utils/unit_converter/converter.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/unit_converter/data.py` & `zonesmart-utils-0.5.8/zs_utils/unit_converter/data.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/unit_converter/exceptions.py` & `zonesmart-utils-0.5.8/zs_utils/unit_converter/exceptions.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/unit_converter/parser.py` & `zonesmart-utils-0.5.8/zs_utils/unit_converter/parser.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/unit_converter/units.py` & `zonesmart-utils-0.5.8/zs_utils/unit_converter/units.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/user/models.py` & `zonesmart-utils-0.5.8/zs_utils/user/models.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/user/utils.py` & `zonesmart-utils-0.5.8/zs_utils/user/utils.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/views/core.py` & `zonesmart-utils-0.5.8/zs_utils/views/core.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/views/mixins.py` & `zonesmart-utils-0.5.8/zs_utils/views/mixins.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/websocket/consumer.py` & `zonesmart-utils-0.5.8/zs_utils/websocket/consumer.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/websocket/middleware.py` & `zonesmart-utils-0.5.8/zs_utils/websocket/middleware.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/websocket/services.py` & `zonesmart-utils-0.5.8/zs_utils/websocket/services.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/websocket/tasks.py` & `zonesmart-utils-0.5.8/zs_utils/websocket/tasks.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/xml_parser.py` & `zonesmart-utils-0.5.8/zs_utils/xml_parser.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/__init__.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/abstract.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/abstract.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/age.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/age.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/category.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/category.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/condition.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/condition.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/currency.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/currency.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/dimensions.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/dimensions.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/feed.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/feed.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/fields/enable_auto_discounts.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/fields/enable_auto_discounts.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/fields/options.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/fields/options.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/gift.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/gift.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/offers.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/offers.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/option.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/option.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/outlet.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/outlet.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/parameter.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/parameter.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/price.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/price.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/promo.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/promo.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/models/shop.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/models/shop.py`

 * *Files identical despite different names*

### Comparing `zonesmart-utils-0.5.7/zs_utils/yandex_market_language/yml.py` & `zonesmart-utils-0.5.8/zs_utils/yandex_market_language/yml.py`

 * *Files identical despite different names*
