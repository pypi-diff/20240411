# Comparing `tmp/airbyte_source_stripe-5.3.1.tar.gz` & `tmp/airbyte_source_stripe-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_stripe-5.3.1.tar", max compression
+gzip compressed data, was "airbyte_source_stripe-5.3.2.tar", max compression
```

## Comparing `airbyte_source_stripe-5.3.1.tar` & `airbyte_source_stripe-5.3.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     4496 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/README.md
--rw-r--r--   0        0        0      804 2024-04-10 10:37:51.380242 airbyte_source_stripe-5.3.1/pyproject.toml
--rw-r--r--   0        0        0      122 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/__init__.py
--rw-r--r--   0        0        0     6009 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/availability_strategy.py
--rw-r--r--   0        0        0     1595 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/run.py
--rw-r--r--   0        0        0    22080 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/accounts.json
--rw-r--r--   0        0        0     1778 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/application_fees.json
--rw-r--r--   0        0        0      801 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/application_fees_refunds.json
--rw-r--r--   0        0        0     6359 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/authorizations.json
--rw-r--r--   0        0        0      131 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/balance_transactions.json
--rw-r--r--   0        0        0     1032 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/bank_accounts.json
--rw-r--r--   0        0        0      121 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/cardholders.json
--rw-r--r--   0        0        0      115 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/cards.json
--rw-r--r--   0        0        0    27559 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/charges.json
--rw-r--r--   0        0        0    14125 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/checkout_sessions.json
--rw-r--r--   0        0        0     6396 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/checkout_sessions_line_items.json
--rw-r--r--   0        0        0     1157 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/coupons.json
--rw-r--r--   0        0        0     9606 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/credit_notes.json
--rw-r--r--   0        0        0      899 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/customer_balance_transactions.json
--rw-r--r--   0        0        0      119 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/customers.json
--rw-r--r--   0        0        0     4255 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/disputes.json
--rw-r--r--   0        0        0      644 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/early_fraud_warnings.json
--rw-r--r--   0        0        0      897 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/events.json
--rw-r--r--   0        0        0     1043 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/external_account_bank_accounts.json
--rw-r--r--   0        0        0     1654 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/external_account_cards.json
--rw-r--r--   0        0        0      642 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/file_links.json
--rw-r--r--   0        0        0     1904 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/files.json
--rw-r--r--   0        0        0     3890 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/invoice_items.json
--rw-r--r--   0        0        0     5237 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/invoice_line_items.json
--rw-r--r--   0        0        0    13937 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/invoices.json
--rw-r--r--   0        0        0  3248217 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/openapi_spec.json
--rw-r--r--   0        0        0      125 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/payment_intents.json
--rw-r--r--   0        0        0      125 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/payment_methods.json
--rw-r--r--   0        0        0     3038 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/payouts.json
--rw-r--r--   0        0        0    10760 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/persons.json
--rw-r--r--   0        0        0     2099 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/plans.json
--rw-r--r--   0        0        0     1932 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/prices.json
--rw-r--r--   0        0        0     2080 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/products.json
--rw-r--r--   0        0        0     2201 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/promotion_codes.json
--rw-r--r--   0        0        0     1590 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/refunds.json
--rw-r--r--   0        0        0     1710 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/reviews.json
--rw-r--r--   0        0        0    13649 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/setup_attempts.json
--rw-r--r--   0        0        0      123 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/setup_intents.json
--rw-r--r--   0        0        0      392 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/address.json
--rw-r--r--   0        0        0     1486 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/balance_transactions.json
--rw-r--r--   0        0        0     2149 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/card.json
--rw-r--r--   0        0        0     2489 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/cardholder.json
--rw-r--r--   0        0        0    23837 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/customer.json
--rw-r--r--   0        0        0     2206 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/issuing_transaction_purchase_details.json
--rw-r--r--   0        0        0    26783 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/payment_intent.json
--rw-r--r--   0        0        0     6034 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/payment_method.json
--rw-r--r--   0        0        0      163 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/payment_method_configuration_details.json
--rw-r--r--   0        0        0     2109 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/price.json
--rw-r--r--   0        0        0     2024 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/setup_intent.json
--rw-r--r--   0        0        0      510 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/spending_controls.json
--rw-r--r--   0        0        0      940 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/tax_rate.json
--rw-r--r--   0        0        0       78 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/tax_rates.json
--rw-r--r--   0        0        0     1222 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/shipping_rates.json
--rw-r--r--   0        0        0     3769 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/subscription_items.json
--rw-r--r--   0        0        0     5505 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/subscription_schedule.json
--rw-r--r--   0        0        0    10700 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/subscriptions.json
--rw-r--r--   0        0        0     1286 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/top_ups.json
--rw-r--r--   0        0        0     1957 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/transactions.json
--rw-r--r--   0        0        0      809 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/transfer_reversals.json
--rw-r--r--   0        0        0     1999 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/transfers.json
--rw-r--r--   0        0        0      716 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/schemas/usage_records.json
--rw-r--r--   0        0        0    25662 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/source.py
--rw-r--r--   0        0        0     3043 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/spec.yaml
--rw-r--r--   0        0        0     1861 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/stream_helpers.py
--rw-r--r--   0        0        0    37125 2024-04-10 09:24:04.000000 airbyte_source_stripe-5.3.1/source_stripe/streams.py
--rw-r--r--   0        0        0     5264 1970-01-01 00:00:00.000000 airbyte_source_stripe-5.3.1/PKG-INFO
+-rw-r--r--   0        0        0     4496 2024-04-11 12:37:38.523185 airbyte_source_stripe-5.3.2/README.md
+-rw-r--r--   0        0        0      804 2024-04-11 12:40:31.480764 airbyte_source_stripe-5.3.2/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-04-11 12:37:38.523185 airbyte_source_stripe-5.3.2/source_stripe/__init__.py
+-rw-r--r--   0        0        0     6009 2024-04-11 12:37:38.523185 airbyte_source_stripe-5.3.2/source_stripe/availability_strategy.py
+-rw-r--r--   0        0        0     1595 2024-04-11 12:37:38.523185 airbyte_source_stripe-5.3.2/source_stripe/run.py
+-rw-r--r--   0        0        0    22080 2024-04-11 12:37:38.523185 airbyte_source_stripe-5.3.2/source_stripe/schemas/accounts.json
+-rw-r--r--   0        0        0     1778 2024-04-11 12:37:38.523185 airbyte_source_stripe-5.3.2/source_stripe/schemas/application_fees.json
+-rw-r--r--   0        0        0      801 2024-04-11 12:37:38.523185 airbyte_source_stripe-5.3.2/source_stripe/schemas/application_fees_refunds.json
+-rw-r--r--   0        0        0     6359 2024-04-11 12:37:38.523185 airbyte_source_stripe-5.3.2/source_stripe/schemas/authorizations.json
+-rw-r--r--   0        0        0      131 2024-04-11 12:37:38.523185 airbyte_source_stripe-5.3.2/source_stripe/schemas/balance_transactions.json
+-rw-r--r--   0        0        0     1032 2024-04-11 12:37:38.523185 airbyte_source_stripe-5.3.2/source_stripe/schemas/bank_accounts.json
+-rw-r--r--   0        0        0      121 2024-04-11 12:37:38.523185 airbyte_source_stripe-5.3.2/source_stripe/schemas/cardholders.json
+-rw-r--r--   0        0        0      115 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/cards.json
+-rw-r--r--   0        0        0    27559 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/charges.json
+-rw-r--r--   0        0        0    14125 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/checkout_sessions.json
+-rw-r--r--   0        0        0     6396 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/checkout_sessions_line_items.json
+-rw-r--r--   0        0        0     1157 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/coupons.json
+-rw-r--r--   0        0        0     9606 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/credit_notes.json
+-rw-r--r--   0        0        0      899 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/customer_balance_transactions.json
+-rw-r--r--   0        0        0      119 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/customers.json
+-rw-r--r--   0        0        0     4255 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/disputes.json
+-rw-r--r--   0        0        0      644 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/early_fraud_warnings.json
+-rw-r--r--   0        0        0      897 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/events.json
+-rw-r--r--   0        0        0     1043 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/external_account_bank_accounts.json
+-rw-r--r--   0        0        0     1654 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/external_account_cards.json
+-rw-r--r--   0        0        0      642 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/file_links.json
+-rw-r--r--   0        0        0     1904 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/files.json
+-rw-r--r--   0        0        0     3890 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/invoice_items.json
+-rw-r--r--   0        0        0     5237 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/invoice_line_items.json
+-rw-r--r--   0        0        0    13937 2024-04-11 12:37:38.527185 airbyte_source_stripe-5.3.2/source_stripe/schemas/invoices.json
+-rw-r--r--   0        0        0  3248217 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/openapi_spec.json
+-rw-r--r--   0        0        0      125 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/payment_intents.json
+-rw-r--r--   0        0        0      125 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/payment_methods.json
+-rw-r--r--   0        0        0     3038 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/payouts.json
+-rw-r--r--   0        0        0    10760 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/persons.json
+-rw-r--r--   0        0        0     2099 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/plans.json
+-rw-r--r--   0        0        0     1932 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/prices.json
+-rw-r--r--   0        0        0     2080 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/products.json
+-rw-r--r--   0        0        0     2201 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/promotion_codes.json
+-rw-r--r--   0        0        0     1590 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/refunds.json
+-rw-r--r--   0        0        0     1710 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/reviews.json
+-rw-r--r--   0        0        0    13649 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/setup_attempts.json
+-rw-r--r--   0        0        0      123 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/setup_intents.json
+-rw-r--r--   0        0        0      392 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/address.json
+-rw-r--r--   0        0        0     1486 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/balance_transactions.json
+-rw-r--r--   0        0        0     2149 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/card.json
+-rw-r--r--   0        0        0     2489 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/cardholder.json
+-rw-r--r--   0        0        0    23837 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/customer.json
+-rw-r--r--   0        0        0     2206 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/issuing_transaction_purchase_details.json
+-rw-r--r--   0        0        0    26783 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/payment_intent.json
+-rw-r--r--   0        0        0     6034 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/payment_method.json
+-rw-r--r--   0        0        0      163 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/payment_method_configuration_details.json
+-rw-r--r--   0        0        0     2109 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/price.json
+-rw-r--r--   0        0        0     2024 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/setup_intent.json
+-rw-r--r--   0        0        0      510 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/spending_controls.json
+-rw-r--r--   0        0        0      940 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/tax_rate.json
+-rw-r--r--   0        0        0       78 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/tax_rates.json
+-rw-r--r--   0        0        0     1222 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/shipping_rates.json
+-rw-r--r--   0        0        0     3769 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/subscription_items.json
+-rw-r--r--   0        0        0     5505 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/subscription_schedule.json
+-rw-r--r--   0        0        0    10700 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/subscriptions.json
+-rw-r--r--   0        0        0     1286 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/top_ups.json
+-rw-r--r--   0        0        0     1957 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/transactions.json
+-rw-r--r--   0        0        0      809 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/transfer_reversals.json
+-rw-r--r--   0        0        0     1999 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/transfers.json
+-rw-r--r--   0        0        0      716 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/schemas/usage_records.json
+-rw-r--r--   0        0        0    26033 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/source.py
+-rw-r--r--   0        0        0     3043 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/spec.yaml
+-rw-r--r--   0        0        0     1861 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/stream_helpers.py
+-rw-r--r--   0        0        0    37125 2024-04-11 12:37:38.531185 airbyte_source_stripe-5.3.2/source_stripe/streams.py
+-rw-r--r--   0        0        0     5264 1970-01-01 00:00:00.000000 airbyte_source_stripe-5.3.2/PKG-INFO
```

### Comparing `airbyte_source_stripe-5.3.1/README.md` & `airbyte_source_stripe-5.3.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/pyproject.toml` & `airbyte_source_stripe-5.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "5.3.1"
+version = "5.3.2"
 name = "airbyte-source-stripe"
 description = "Source implementation for Stripe."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "Elv2"
 readme = "README.md"
```

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/availability_strategy.py` & `airbyte_source_stripe-5.3.2/source_stripe/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/run.py` & `airbyte_source_stripe-5.3.2/source_stripe/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/accounts.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/application_fees.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/application_fees.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/application_fees_refunds.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/application_fees_refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/authorizations.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/authorizations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/bank_accounts.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/bank_accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/charges.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/charges.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/checkout_sessions.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/checkout_sessions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/checkout_sessions_line_items.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/checkout_sessions_line_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/coupons.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/coupons.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/credit_notes.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/credit_notes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/customer_balance_transactions.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/customer_balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/disputes.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/disputes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/early_fraud_warnings.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/early_fraud_warnings.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/events.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/external_account_bank_accounts.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/external_account_bank_accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/external_account_cards.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/external_account_cards.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/file_links.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/file_links.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/files.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/files.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/invoice_items.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/invoice_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/invoice_line_items.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/invoice_line_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/invoices.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/invoices.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/openapi_spec.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/openapi_spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/payouts.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/payouts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/persons.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/persons.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/plans.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/plans.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/prices.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/prices.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/products.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/promotion_codes.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/promotion_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/refunds.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/reviews.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/reviews.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/setup_attempts.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/setup_attempts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/balance_transactions.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/card.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/card.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/cardholder.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/cardholder.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/customer.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/customer.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/issuing_transaction_purchase_details.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/issuing_transaction_purchase_details.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/payment_intent.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/payment_intent.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/payment_method.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/payment_method.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/price.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/price.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/setup_intent.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/setup_intent.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/shared/tax_rate.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/shared/tax_rate.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/shipping_rates.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/shipping_rates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/subscription_items.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/subscription_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/subscription_schedule.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/subscription_schedule.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/subscriptions.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/subscriptions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/top_ups.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/top_ups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/transactions.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/transfer_reversals.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/transfer_reversals.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/transfers.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/transfers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/schemas/usage_records.json` & `airbyte_source_stripe-5.3.2/source_stripe/schemas/usage_records.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/source.py` & `airbyte_source_stripe-5.3.2/source_stripe/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import logging
 import os
-from datetime import timedelta
+from datetime import datetime, timedelta, timezone
 from typing import Any, List, Mapping, MutableMapping, Optional, Tuple
 
 import pendulum
 import stripe
 from airbyte_cdk import AirbyteLogger
 from airbyte_cdk.entrypoint import logger as entrypoint_logger
 from airbyte_cdk.models import ConfiguredAirbyteCatalog, FailureType
@@ -516,17 +516,27 @@
                 parent=subscription_items,
                 primary_key=None,
                 **args,
             ),
         ]
 
         state_manager = ConnectorStateManager(stream_instance_map={s.name: s for s in streams}, state=self._state)
-        return [self._to_concurrent(stream, self._start_date_to_timestamp(config), state_manager) for stream in streams]
+        return [
+            self._to_concurrent(
+                stream,
+                datetime.fromtimestamp(self._start_date_to_timestamp(config), timezone.utc),
+                timedelta(days=config["slice_range"]),
+                state_manager,
+            )
+            for stream in streams
+        ]
 
-    def _to_concurrent(self, stream: Stream, fallback_start, state_manager: ConnectorStateManager) -> Stream:
+    def _to_concurrent(
+        self, stream: Stream, fallback_start: datetime, slice_range: timedelta, state_manager: ConnectorStateManager
+    ) -> Stream:
         if stream.name in self._streams_configured_as_full_refresh:
             return StreamFacade.create_from_stream(
                 stream,
                 self,
                 entrypoint_logger,
                 self._create_empty_state(),
                 FinalStateCursor(stream_name=stream.name, stream_namespace=stream.namespace, message_repository=self.message_repository),
@@ -543,14 +553,17 @@
                 state_manager.get_stream_state(stream.name, stream.namespace),
                 self.message_repository,
                 state_manager,
                 converter,
                 cursor_field,
                 slice_boundary_fields,
                 fallback_start,
+                converter.get_end_provider(),
+                timedelta(seconds=0),
+                slice_range,
             )
             return StreamFacade.create_from_stream(stream, self, entrypoint_logger, state, cursor)
 
         return stream
 
     def _create_empty_state(self) -> MutableMapping[str, Any]:
         return {}
```

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/spec.yaml` & `airbyte_source_stripe-5.3.2/source_stripe/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/stream_helpers.py` & `airbyte_source_stripe-5.3.2/source_stripe/stream_helpers.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/source_stripe/streams.py` & `airbyte_source_stripe-5.3.2/source_stripe/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.1/PKG-INFO` & `airbyte_source_stripe-5.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-stripe
-Version: 5.3.1
+Version: 5.3.2
 Summary: Source implementation for Stripe.
 Home-page: https://airbyte.com
 License: Elv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

