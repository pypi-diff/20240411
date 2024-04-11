# Comparing `tmp/airbyte_source_quickbooks-3.0.2.tar.gz` & `tmp/airbyte_source_quickbooks-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_quickbooks-3.0.2.tar", max compression
+gzip compressed data, was "airbyte_source_quickbooks-3.0.3.tar", max compression
```

## Comparing `airbyte_source_quickbooks-3.0.2.tar` & `airbyte_source_quickbooks-3.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     4059 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/README.md
--rw-r--r--   0        0        0      809 2024-02-21 17:36:36.626464 airbyte_source_quickbooks-3.0.2/pyproject.toml
--rw-r--r--   0        0        0      211 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/__init__.py
--rw-r--r--   0        0        0     3406 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/components.py
--rw-r--r--   0        0        0     8847 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/manifest.yaml
--rw-r--r--   0        0        0      242 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/run.py
--rw-r--r--   0        0        0     1711 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/accounts.json
--rw-r--r--   0        0        0     3325 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/bill_payments.json
--rw-r--r--   0        0        0     5216 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/bills.json
--rw-r--r--   0        0        0     2556 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/budgets.json
--rw-r--r--   0        0        0     1105 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/classes.json
--rw-r--r--   0        0        0     5800 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/credit_memos.json
--rw-r--r--   0        0        0     4833 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/customers.json
--rw-r--r--   0        0        0     1110 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/departments.json
--rw-r--r--   0        0        0     3852 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/deposits.json
--rw-r--r--   0        0        0     2165 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/employees.json
--rw-r--r--   0        0        0     7073 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/estimates.json
--rw-r--r--   0        0        0     9527 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/invoices.json
--rw-r--r--   0        0        0     2135 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/items.json
--rw-r--r--   0        0        0     4325 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/journal_entries.json
--rw-r--r--   0        0        0      867 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/payment_methods.json
--rw-r--r--   0        0        0     4442 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/payments.json
--rw-r--r--   0        0        0     6937 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/purchase_orders.json
--rw-r--r--   0        0        0     6198 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/purchases.json
--rw-r--r--   0        0        0     5123 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/refund_receipts.json
--rw-r--r--   0        0        0     6847 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/sales_receipts.json
--rw-r--r--   0        0        0      974 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/tax_agencies.json
--rw-r--r--   0        0        0     1945 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/tax_codes.json
--rw-r--r--   0        0        0     2213 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/tax_rates.json
--rw-r--r--   0        0        0     1253 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/terms.json
--rw-r--r--   0        0        0     1865 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/time_activities.json
--rw-r--r--   0        0        0     1581 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/transfers.json
--rw-r--r--   0        0        0     3795 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/vendor_credits.json
--rw-r--r--   0        0        0     3243 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/vendors.json
--rw-r--r--   0        0        0      479 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/source.py
--rw-r--r--   0        0        0     3392 2024-02-21 16:55:49.000000 airbyte_source_quickbooks-3.0.2/source_quickbooks/spec.json
--rw-r--r--   0        0        0     4841 1970-01-01 00:00:00.000000 airbyte_source_quickbooks-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4059 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/README.md
+-rw-r--r--   0        0        0      809 2024-04-11 14:26:26.281180 airbyte_source_quickbooks-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0      211 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/__init__.py
+-rw-r--r--   0        0        0     3406 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/components.py
+-rw-r--r--   0        0        0     8879 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/manifest.yaml
+-rw-r--r--   0        0        0      242 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/run.py
+-rw-r--r--   0        0        0     1711 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/accounts.json
+-rw-r--r--   0        0        0     3325 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/bill_payments.json
+-rw-r--r--   0        0        0     5593 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/bills.json
+-rw-r--r--   0        0        0     2556 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/budgets.json
+-rw-r--r--   0        0        0     1105 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/classes.json
+-rw-r--r--   0        0        0     5800 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/credit_memos.json
+-rw-r--r--   0        0        0     4833 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/customers.json
+-rw-r--r--   0        0        0     1110 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/departments.json
+-rw-r--r--   0        0        0     4319 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/deposits.json
+-rw-r--r--   0        0        0     2165 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/employees.json
+-rw-r--r--   0        0        0     7073 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/estimates.json
+-rw-r--r--   0        0        0     9527 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/invoices.json
+-rw-r--r--   0        0        0     2135 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/items.json
+-rw-r--r--   0        0        0     5356 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/journal_entries.json
+-rw-r--r--   0        0        0      867 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/payment_methods.json
+-rw-r--r--   0        0        0     4442 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/payments.json
+-rw-r--r--   0        0        0     6937 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/purchase_orders.json
+-rw-r--r--   0        0        0     6575 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/purchases.json
+-rw-r--r--   0        0        0     5123 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/refund_receipts.json
+-rw-r--r--   0        0        0     6847 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/sales_receipts.json
+-rw-r--r--   0        0        0      974 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/tax_agencies.json
+-rw-r--r--   0        0        0     1945 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/tax_codes.json
+-rw-r--r--   0        0        0     2213 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/tax_rates.json
+-rw-r--r--   0        0        0     1253 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/terms.json
+-rw-r--r--   0        0        0     1865 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/time_activities.json
+-rw-r--r--   0        0        0     1581 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/transfers.json
+-rw-r--r--   0        0        0     3795 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/vendor_credits.json
+-rw-r--r--   0        0        0     3243 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/vendors.json
+-rw-r--r--   0        0        0      479 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/source.py
+-rw-r--r--   0        0        0     3392 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/spec.json
+-rw-r--r--   0        0        0     4841 1970-01-01 00:00:00.000000 airbyte_source_quickbooks-3.0.3/PKG-INFO
```

### Comparing `airbyte_source_quickbooks-3.0.2/README.md` & `airbyte_source_quickbooks-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/pyproject.toml` & `airbyte_source_quickbooks-3.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "3.0.2"
+version = "3.0.3"
 name = "airbyte-source-quickbooks"
 description = "Source implementation for quickbooks."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/components.py` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/manifest.yaml` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/manifest.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
       "User-Agent": "airbyte-connector"
     authenticator:
       type: OAuthAuthenticator
       token_refresh_endpoint: "https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer"
       client_id: "{{ config['credentials']['client_id'] }}"
       client_secret: "{{ config['credentials']['client_secret'] }}"
       refresh_token: "{{ config['credentials']['refresh_token'] }}"
+      refresh_token_updater: {}
   retriever:
     type: SimpleRetriever
     record_selector:
       $ref: "#/definitions/selector"
     paginator:
       type: DefaultPaginator
       pagination_strategy:
```

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/accounts.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/bill_payments.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/bill_payments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/bills.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/bills.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999990699404763%*

 * *Differences: {"'properties'": "{'Line': {'items': {'properties': {'AccountBasedExpenseLineDetail': "*

 * *                 "{'properties': {'ClassRef': OrderedDict([('additionalProperties', True), "*

 * *                 "('properties', OrderedDict([('name', OrderedDict([('type', ['null', "*

 * *                 "'string'])])), ('value', OrderedDict([('type', ['null', 'string'])]))])), "*

 * *                 "('type', ['null', 'object'])])}}}}}}"}*

```diff
@@ -119,14 +119,35 @@
                             },
                             "BillableStatus": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
                             },
+                            "ClassRef": {
+                                "additionalProperties": true,
+                                "properties": {
+                                    "name": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    },
+                                    "value": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    }
+                                },
+                                "type": [
+                                    "null",
+                                    "object"
+                                ]
+                            },
                             "CustomerRef": {
                                 "properties": {
                                     "name": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
```

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/budgets.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/budgets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/classes.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/classes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/credit_memos.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/credit_memos.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/customers.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/departments.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/departments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/deposits.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/deposits.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999891493055556%*

 * *Differences: {"'properties'": "{'Line': {'items': {'properties': {'DepositLineDetail': {'properties': "*

 * *                 "{'Entity': OrderedDict([('properties', OrderedDict([('name', "*

 * *                 "OrderedDict([('type', ['null', 'string'])])), ('value', OrderedDict([('type', "*

 * *                 "['null', 'string'])])), ('type', OrderedDict([('type', ['null', "*

 * *                 "'string'])]))])), ('type', ['null', 'object'])])}, 'additionalProperties': "*

 * *                 'True}}}}}'}*

```diff
@@ -119,14 +119,15 @@
                     "Amount": {
                         "type": [
                             "null",
                             "number"
                         ]
                     },
                     "DepositLineDetail": {
+                        "additionalProperties": true,
                         "properties": {
                             "AccountRef": {
                                 "properties": {
                                     "name": {
                                         "type": [
                                             "null",
                                             "string"
@@ -146,14 +147,40 @@
                             },
                             "CheckNum": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
                             },
+                            "Entity": {
+                                "properties": {
+                                    "name": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    },
+                                    "type": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    },
+                                    "value": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    }
+                                },
+                                "type": [
+                                    "null",
+                                    "object"
+                                ]
+                            },
                             "PaymentMethodRef": {
                                 "properties": {
                                     "value": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
```

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/employees.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/employees.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/estimates.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/estimates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/invoices.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/invoices.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/items.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/journal_entries.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/journal_entries.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999956597222223%*

 * *Differences: {"'properties'": "{'Line': {'items': {'properties': {'JournalEntryLineDetail': {'properties': "*

 * *                 "{'ClassRef': OrderedDict([('additionalProperties', True), ('properties', "*

 * *                 "OrderedDict([('name', OrderedDict([('type', ['null', 'string'])])), ('value', "*

 * *                 "OrderedDict([('type', ['null', 'string'])]))])), ('type', ['null', 'object'])]), "*

 * *                 "'Entity': OrderedDict([('additionalProperties', True), ('properties', "*

 * *                 "OrderedDict([('T […]*

```diff
@@ -90,14 +90,70 @@
                                     }
                                 },
                                 "type": [
                                     "null",
                                     "object"
                                 ]
                             },
+                            "ClassRef": {
+                                "additionalProperties": true,
+                                "properties": {
+                                    "name": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    },
+                                    "value": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    }
+                                },
+                                "type": [
+                                    "null",
+                                    "object"
+                                ]
+                            },
+                            "Entity": {
+                                "additionalProperties": true,
+                                "properties": {
+                                    "EntityRef": {
+                                        "properties": {
+                                            "name": {
+                                                "type": [
+                                                    "null",
+                                                    "string"
+                                                ]
+                                            },
+                                            "value": {
+                                                "type": [
+                                                    "null",
+                                                    "string"
+                                                ]
+                                            }
+                                        },
+                                        "type": [
+                                            "null",
+                                            "object"
+                                        ]
+                                    },
+                                    "Type": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    }
+                                },
+                                "type": [
+                                    "null",
+                                    "object"
+                                ]
+                            },
                             "PostingType": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
                             }
                         },
```

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/payment_methods.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/payment_methods.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/payments.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/payments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/purchase_orders.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/purchase_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/purchases.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/purchases.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999989149305556%*

 * *Differences: {"'properties'": "{'Line': {'items': {'properties': {'AccountBasedExpenseLineDetail': "*

 * *                 "{'properties': {'ClassRef': OrderedDict([('additionalProperties', True), "*

 * *                 "('properties', OrderedDict([('name', OrderedDict([('type', ['null', "*

 * *                 "'string'])])), ('value', OrderedDict([('type', ['null', 'string'])]))])), "*

 * *                 "('type', ['null', 'object'])])}}}}}}"}*

```diff
@@ -118,14 +118,35 @@
                             },
                             "BillableStatus": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
                             },
+                            "ClassRef": {
+                                "additionalProperties": true,
+                                "properties": {
+                                    "name": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    },
+                                    "value": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    }
+                                },
+                                "type": [
+                                    "null",
+                                    "object"
+                                ]
+                            },
                             "CustomerRef": {
                                 "properties": {
                                     "name": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
```

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/refund_receipts.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/refund_receipts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/sales_receipts.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/sales_receipts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/tax_agencies.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/tax_agencies.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/tax_codes.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/tax_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/tax_rates.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/tax_rates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/terms.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/terms.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/time_activities.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/time_activities.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/transfers.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/transfers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/vendor_credits.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/vendor_credits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/schemas/vendors.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/vendors.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/source_quickbooks/spec.json` & `airbyte_source_quickbooks-3.0.3/source_quickbooks/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.2/PKG-INFO` & `airbyte_source_quickbooks-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-quickbooks
-Version: 3.0.2
+Version: 3.0.3
 Summary: Source implementation for quickbooks.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

