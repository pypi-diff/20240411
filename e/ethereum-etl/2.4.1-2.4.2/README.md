# Comparing `tmp/ethereum-etl-2.4.1.tar.gz` & `tmp/ethereum-etl-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ethereum-etl-2.4.1.tar", last modified: Wed Apr  3 04:44:03 2024, max compression
+gzip compressed data, was "dist/ethereum-etl-2.4.2.tar", last modified: Thu Apr 11 12:43:30 2024, max compression
```

## Comparing `ethereum-etl-2.4.1.tar` & `ethereum-etl-2.4.2.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/blockchainetl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/atomic_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/csv_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/blockchainetl/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/base_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/composite_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/console_item_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/composite_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/int_to_decimal_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/int_to_string_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/list_field_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/simple_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/unix_timestamp_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/gcs_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/google_pubsub_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/in_memory_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/kafka_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/kinesis_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/multi_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/postgres_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/logging_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/blockchainetl/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/streaming/postgres_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/streaming/streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/streaming/streamer_adapter_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/streaming/streaming_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/atomic_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_blocks_and_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_geth_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_origin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_receipts_and_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_token_transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/extract_contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/extract_csv_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/extract_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/extract_geth_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/extract_token_transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/extract_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/filter_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/get_block_range_for_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/get_block_range_for_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/get_keccak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/csv_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/domain/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/geth_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/origin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/receipt_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/token_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/enumeration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/enumeration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/enumeration/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/erc20_abi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/executors/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/executors/batch_work_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/executors/bounded_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/executors/fail_safe_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/exporters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/ipfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/ipfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/ipfs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/ipfs/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_all_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_blocks_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_origin_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_receipts_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_traces_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/blocks_and_transactions_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/contracts_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/geth_traces_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/origin_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/receipts_and_logs_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/token_transfers_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/tokens_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/traces_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/extract_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/extract_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/extract_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/extract_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/json_rpc_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11649 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mainnet_daofork_state_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)   673817 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mainnet_genesis_alloc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/mappers/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/block_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/contract_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/geth_trace_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/origin_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/receipt_log_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/receipt_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/token_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/token_transfer_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/trace_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/transaction_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/misc/retriable_value_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/progress_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/providers/auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/providers/ipc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/providers/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/service/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/eth_contract_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/eth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/eth_special_trace_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/eth_token_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/graph_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/origin_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/token_transfer_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/trace_id_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/trace_status_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/eth_item_id_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/eth_item_timestamp_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/eth_streamer_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/item_exporter_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/postgres_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/thread_local_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/web3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/tests/ethereumetl/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/mock_batch_web3_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/mock_ipfs_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/mock_web3_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_blocks_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_origin_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_receipts_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_extract_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_extract_token_transfers_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/tests/ethereumetl/service/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70321 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/service/test_eth_contract_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/service/test_eth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/service/test_token_transfer_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/test_progress_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/blockchainetl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/atomic_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/csv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/blockchainetl/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/base_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/composite_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/console_item_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/composite_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/int_to_decimal_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/int_to_string_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/list_field_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/simple_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/unix_timestamp_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/gcs_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/google_pubsub_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/in_memory_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/kafka_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/kinesis_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/multi_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/jobs/exporters/postgres_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/blockchainetl/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/streaming/postgres_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/streaming/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/streaming/streamer_adapter_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/blockchainetl/streaming/streaming_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereum_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereum_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereum_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereum_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereum_etl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereum_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereum_etl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereumetl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/atomic_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereumetl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/export_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/export_blocks_and_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/export_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/export_geth_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/export_origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/export_receipts_and_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/export_token_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/export_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/export_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/extract_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/extract_csv_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/extract_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/extract_geth_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/extract_token_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/extract_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/filter_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/get_block_range_for_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/get_block_range_for_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/get_keccak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/cli/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/csv_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereumetl/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/domain/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/domain/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/domain/geth_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/domain/origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/domain/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/domain/receipt_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/domain/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/domain/token_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/domain/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/domain/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereumetl/enumeration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/enumeration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/enumeration/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/erc20_abi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereumetl/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/executors/batch_work_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/executors/bounded_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/executors/fail_safe_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/exporters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereumetl/ipfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/ipfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/ipfs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/ipfs/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereumetl/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/export_all_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/export_blocks_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/export_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/export_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/export_origin_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/export_receipts_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/export_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/export_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/export_traces_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereumetl/jobs/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/exporters/blocks_and_transactions_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/exporters/contracts_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/exporters/geth_traces_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/exporters/origin_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/exporters/receipts_and_logs_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/exporters/token_transfers_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/exporters/tokens_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/exporters/traces_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/extract_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/extract_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/extract_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/jobs/extract_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/json_rpc_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11649 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/mainnet_daofork_state_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)   673817 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/mainnet_genesis_alloc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereumetl/mappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/mappers/block_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/mappers/contract_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/mappers/geth_trace_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/mappers/origin_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/mappers/receipt_log_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/mappers/receipt_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/mappers/token_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/mappers/token_transfer_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/mappers/trace_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/mappers/transaction_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereumetl/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/misc/retriable_value_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/progress_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereumetl/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/providers/auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/providers/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/providers/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereumetl/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/service/eth_contract_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/service/eth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/service/eth_special_trace_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/service/eth_token_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/service/graph_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/service/origin_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/service/token_transfer_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/service/trace_id_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/service/trace_status_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/ethereumetl/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/streaming/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/streaming/eth_item_id_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/streaming/eth_item_timestamp_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/streaming/eth_streamer_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/streaming/item_exporter_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/streaming/postgres_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/thread_local_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/ethereumetl/web3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/tests/ethereumetl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/mock_batch_web3_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/mock_ipfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/mock_web3_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_blocks_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_origin_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_receipts_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/test_extract_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/job/test_extract_token_transfers_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/tests/ethereumetl/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70321 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/service/test_eth_contract_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/service/test_eth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/service/test_token_transfer_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/ethereumetl/test_progress_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:43:30.000000 ethereum-etl-2.4.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-11 12:43:28.000000 ethereum-etl-2.4.2/tests/resources/__init__.py
```

### Comparing `ethereum-etl-2.4.1/PKG-INFO` & `ethereum-etl-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethereum-etl
-Version: 2.4.1
+Version: 2.4.2
 Summary: Tools for exporting Ethereum blockchain data to CSV or JSON
 Home-page: https://github.com/blockchain-etl/ethereum-etl
 Author: Evgeny Medvedev
 Author-email: evge.medvedev@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/blockchain-etl/ethereum-etl/issues
 Project-URL: Chat, https://gitter.im/ethereum-etl/Lobby
```

### Comparing `ethereum-etl-2.4.1/README.md` & `ethereum-etl-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/atomic_counter.py` & `ethereum-etl-2.4.2/blockchainetl/atomic_counter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/csv_utils.py` & `ethereum-etl-2.4.2/blockchainetl/csv_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/exporters.py` & `ethereum-etl-2.4.2/blockchainetl/exporters.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/file_utils.py` & `ethereum-etl-2.4.2/blockchainetl/file_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/base_job.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/base_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/composite_item_exporter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/composite_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/console_item_exporter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/console_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/composite_item_converter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/composite_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/int_to_decimal_item_converter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/int_to_decimal_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/int_to_string_item_converter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/int_to_string_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/list_field_item_converter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/list_field_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/simple_item_converter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/simple_item_converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,17 +26,22 @@
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 
-
 class SimpleItemConverter:
 
+    def __init__(self, field_converters=None):
+        self.field_converters = field_converters
+
     def convert_item(self, item):
         return {
             key: self.convert_field(key, value) for key, value in item.items()
         }
 
     def convert_field(self, key, value):
-        return value
+        if self.field_converters is not None and key in self.field_converters:
+            return self.field_converters[key](value)
+        else:
+            return value
```

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/unix_timestamp_item_converter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/converters/unix_timestamp_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/gcs_item_exporter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/gcs_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/google_pubsub_item_exporter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/google_pubsub_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/in_memory_item_exporter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/in_memory_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/kafka_exporter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/kafka_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/kinesis_item_exporter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/kinesis_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/multi_item_exporter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/multi_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/postgres_item_exporter.py` & `ethereum-etl-2.4.2/blockchainetl/jobs/exporters/postgres_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/streaming/__init__.py` & `ethereum-etl-2.4.2/blockchainetl/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/streaming/postgres_utils.py` & `ethereum-etl-2.4.2/blockchainetl/streaming/postgres_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/blockchainetl/streaming/streamer.py` & `ethereum-etl-2.4.2/blockchainetl/streaming/streamer.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereum_etl.egg-info/PKG-INFO` & `ethereum-etl-2.4.2/ethereum_etl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethereum-etl
-Version: 2.4.1
+Version: 2.4.2
 Summary: Tools for exporting Ethereum blockchain data to CSV or JSON
 Home-page: https://github.com/blockchain-etl/ethereum-etl
 Author: Evgeny Medvedev
 Author-email: evge.medvedev@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/blockchain-etl/ethereum-etl/issues
 Project-URL: Chat, https://gitter.im/ethereum-etl/Lobby
```

### Comparing `ethereum-etl-2.4.1/ethereum_etl.egg-info/SOURCES.txt` & `ethereum-etl-2.4.2/ethereum_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/__init__.py` & `ethereum-etl-2.4.2/ethereumetl/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/__main__.py` & `ethereum-etl-2.4.2/ethereumetl/__main__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/atomic_counter.py` & `ethereum-etl-2.4.2/ethereumetl/atomic_counter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/__init__.py` & `ethereum-etl-2.4.2/ethereumetl/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from ethereumetl.cli.get_block_range_for_date import get_block_range_for_date
 from ethereumetl.cli.get_block_range_for_timestamps import get_block_range_for_timestamps
 from ethereumetl.cli.get_keccak_hash import get_keccak_hash
 from ethereumetl.cli.stream import stream
 
 
 @click.group()
-@click.version_option(version='2.4.1')
+@click.version_option(version='2.4.2')
 @click.pass_context
 def cli(ctx):
     pass
 
 
 # export
 cli.add_command(export_all, "export_all")
```

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/export_all.py` & `ethereum-etl-2.4.2/ethereumetl/cli/export_all.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/export_blocks_and_transactions.py` & `ethereum-etl-2.4.2/ethereumetl/cli/export_blocks_and_transactions.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/export_contracts.py` & `ethereum-etl-2.4.2/ethereumetl/cli/export_contracts.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/export_geth_traces.py` & `ethereum-etl-2.4.2/ethereumetl/cli/export_geth_traces.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/export_origin.py` & `ethereum-etl-2.4.2/ethereumetl/cli/export_origin.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/export_receipts_and_logs.py` & `ethereum-etl-2.4.2/ethereumetl/cli/export_receipts_and_logs.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/export_token_transfers.py` & `ethereum-etl-2.4.2/ethereumetl/cli/export_token_transfers.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/export_tokens.py` & `ethereum-etl-2.4.2/ethereumetl/cli/export_tokens.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/export_traces.py` & `ethereum-etl-2.4.2/ethereumetl/cli/export_traces.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/extract_contracts.py` & `ethereum-etl-2.4.2/ethereumetl/cli/extract_contracts.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/extract_csv_column.py` & `ethereum-etl-2.4.2/ethereumetl/cli/extract_csv_column.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/extract_field.py` & `ethereum-etl-2.4.2/ethereumetl/cli/extract_field.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/extract_geth_traces.py` & `ethereum-etl-2.4.2/ethereumetl/cli/extract_geth_traces.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/extract_token_transfers.py` & `ethereum-etl-2.4.2/ethereumetl/cli/extract_token_transfers.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/extract_tokens.py` & `ethereum-etl-2.4.2/ethereumetl/cli/extract_tokens.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/filter_items.py` & `ethereum-etl-2.4.2/ethereumetl/cli/filter_items.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/get_block_range_for_date.py` & `ethereum-etl-2.4.2/ethereumetl/cli/get_block_range_for_date.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/get_block_range_for_timestamps.py` & `ethereum-etl-2.4.2/ethereumetl/cli/get_block_range_for_timestamps.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/get_keccak_hash.py` & `ethereum-etl-2.4.2/ethereumetl/cli/get_keccak_hash.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/cli/stream.py` & `ethereum-etl-2.4.2/ethereumetl/cli/stream.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/csv_utils.py` & `ethereum-etl-2.4.2/ethereumetl/csv_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/domain/__init__.py` & `ethereum-etl-2.4.2/ethereumetl/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/domain/block.py` & `ethereum-etl-2.4.2/ethereumetl/domain/block.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/domain/contract.py` & `ethereum-etl-2.4.2/ethereumetl/domain/contract.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/domain/geth_trace.py` & `ethereum-etl-2.4.2/ethereumetl/domain/geth_trace.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/domain/origin.py` & `ethereum-etl-2.4.2/ethereumetl/domain/origin.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/domain/receipt.py` & `ethereum-etl-2.4.2/ethereumetl/domain/receipt.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/domain/receipt_log.py` & `ethereum-etl-2.4.2/ethereumetl/domain/receipt_log.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/domain/token.py` & `ethereum-etl-2.4.2/ethereumetl/domain/token.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/domain/token_transfer.py` & `ethereum-etl-2.4.2/ethereumetl/domain/token_transfer.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/domain/trace.py` & `ethereum-etl-2.4.2/ethereumetl/domain/trace.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/domain/transaction.py` & `ethereum-etl-2.4.2/ethereumetl/domain/transaction.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/erc20_abi.py` & `ethereum-etl-2.4.2/ethereumetl/erc20_abi.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/executors/__init__.py` & `ethereum-etl-2.4.2/ethereumetl/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/executors/batch_work_executor.py` & `ethereum-etl-2.4.2/ethereumetl/executors/batch_work_executor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/executors/bounded_executor.py` & `ethereum-etl-2.4.2/ethereumetl/executors/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/executors/fail_safe_executor.py` & `ethereum-etl-2.4.2/ethereumetl/executors/fail_safe_executor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/exporters.py` & `ethereum-etl-2.4.2/ethereumetl/exporters.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/ipfs/client.py` & `ethereum-etl-2.4.2/ethereumetl/ipfs/client.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/ipfs/origin.py` & `ethereum-etl-2.4.2/ethereumetl/ipfs/origin.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/__init__.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/export_all_common.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/export_all_common.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/export_blocks_job.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/export_blocks_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/export_contracts_job.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/export_contracts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/export_geth_traces_job.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/export_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/export_origin_job.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/export_origin_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/export_receipts_job.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/export_receipts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/export_token_transfers_job.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/export_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/export_tokens_job.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/export_tokens_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/export_traces_job.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/export_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/__init__.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/blocks_and_transactions_item_exporter.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/exporters/blocks_and_transactions_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/contracts_item_exporter.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/exporters/contracts_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/geth_traces_item_exporter.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/exporters/geth_traces_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/origin_exporter.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/exporters/origin_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/receipts_and_logs_item_exporter.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/exporters/receipts_and_logs_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/token_transfers_item_exporter.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/exporters/token_transfers_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/tokens_item_exporter.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/exporters/tokens_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/traces_item_exporter.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/exporters/traces_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/extract_contracts_job.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/extract_contracts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/extract_geth_traces_job.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/extract_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/extract_token_transfers_job.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/extract_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/jobs/extract_tokens_job.py` & `ethereum-etl-2.4.2/ethereumetl/jobs/extract_tokens_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/json_rpc_requests.py` & `ethereum-etl-2.4.2/ethereumetl/json_rpc_requests.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/mainnet_daofork_state_changes.py` & `ethereum-etl-2.4.2/ethereumetl/mainnet_daofork_state_changes.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/mainnet_genesis_alloc.py` & `ethereum-etl-2.4.2/ethereumetl/mainnet_genesis_alloc.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/mappers/__init__.py` & `ethereum-etl-2.4.2/ethereumetl/mappers/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/mappers/block_mapper.py` & `ethereum-etl-2.4.2/ethereumetl/mappers/block_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/mappers/contract_mapper.py` & `ethereum-etl-2.4.2/ethereumetl/mappers/contract_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/mappers/geth_trace_mapper.py` & `ethereum-etl-2.4.2/ethereumetl/mappers/geth_trace_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/mappers/origin_mapper.py` & `ethereum-etl-2.4.2/ethereumetl/mappers/origin_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/mappers/receipt_log_mapper.py` & `ethereum-etl-2.4.2/ethereumetl/mappers/receipt_log_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/mappers/receipt_mapper.py` & `ethereum-etl-2.4.2/ethereumetl/mappers/receipt_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/mappers/token_mapper.py` & `ethereum-etl-2.4.2/ethereumetl/mappers/token_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/mappers/token_transfer_mapper.py` & `ethereum-etl-2.4.2/ethereumetl/mappers/token_transfer_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/mappers/trace_mapper.py` & `ethereum-etl-2.4.2/ethereumetl/mappers/trace_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/mappers/transaction_mapper.py` & `ethereum-etl-2.4.2/ethereumetl/mappers/transaction_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/misc/__init__.py` & `ethereum-etl-2.4.2/ethereumetl/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/misc_utils.py` & `ethereum-etl-2.4.2/ethereumetl/misc_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/progress_logger.py` & `ethereum-etl-2.4.2/ethereumetl/progress_logger.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/providers/__init__.py` & `ethereum-etl-2.4.2/ethereumetl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/providers/auto.py` & `ethereum-etl-2.4.2/ethereumetl/providers/auto.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/providers/ipc.py` & `ethereum-etl-2.4.2/ethereumetl/providers/ipc.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/providers/rpc.py` & `ethereum-etl-2.4.2/ethereumetl/providers/rpc.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/service/__init__.py` & `ethereum-etl-2.4.2/ethereumetl/service/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/service/eth_contract_service.py` & `ethereum-etl-2.4.2/ethereumetl/service/eth_contract_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/service/eth_service.py` & `ethereum-etl-2.4.2/ethereumetl/service/eth_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/service/eth_special_trace_service.py` & `ethereum-etl-2.4.2/ethereumetl/service/eth_special_trace_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/service/eth_token_service.py` & `ethereum-etl-2.4.2/ethereumetl/service/eth_token_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/service/graph_operations.py` & `ethereum-etl-2.4.2/ethereumetl/service/graph_operations.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/service/origin_extractor.py` & `ethereum-etl-2.4.2/ethereumetl/service/origin_extractor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/service/token_transfer_extractor.py` & `ethereum-etl-2.4.2/ethereumetl/service/token_transfer_extractor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/service/trace_id_calculator.py` & `ethereum-etl-2.4.2/ethereumetl/service/trace_id_calculator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/service/trace_status_calculator.py` & `ethereum-etl-2.4.2/ethereumetl/service/trace_status_calculator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/streaming/__init__.py` & `ethereum-etl-2.4.2/ethereumetl/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/streaming/enrich.py` & `ethereum-etl-2.4.2/ethereumetl/streaming/enrich.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/streaming/eth_item_id_calculator.py` & `ethereum-etl-2.4.2/ethereumetl/streaming/eth_item_id_calculator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/streaming/eth_item_timestamp_calculator.py` & `ethereum-etl-2.4.2/ethereumetl/streaming/eth_item_timestamp_calculator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/streaming/eth_streamer_adapter.py` & `ethereum-etl-2.4.2/ethereumetl/streaming/eth_streamer_adapter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/streaming/item_exporter_creator.py` & `ethereum-etl-2.4.2/ethereumetl/streaming/item_exporter_creator.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,28 +58,36 @@
         )
     elif item_exporter_type == ItemExporterType.POSTGRES:
         from blockchainetl.jobs.exporters.postgres_item_exporter import PostgresItemExporter
         from blockchainetl.streaming.postgres_utils import create_insert_statement_for_table
         from blockchainetl.jobs.exporters.converters.unix_timestamp_item_converter import UnixTimestampItemConverter
         from blockchainetl.jobs.exporters.converters.int_to_decimal_item_converter import IntToDecimalItemConverter
         from blockchainetl.jobs.exporters.converters.list_field_item_converter import ListFieldItemConverter
+        from blockchainetl.jobs.exporters.converters.simple_item_converter import SimpleItemConverter
         from ethereumetl.streaming.postgres_tables import BLOCKS, TRANSACTIONS, LOGS, TOKEN_TRANSFERS, TRACES, TOKENS, CONTRACTS
 
+        def array_to_str(val):
+            return ','.join(val) if val is not None else None
+
         item_exporter = PostgresItemExporter(
             output, item_type_to_insert_stmt_mapping={
                 'block': create_insert_statement_for_table(BLOCKS),
                 'transaction': create_insert_statement_for_table(TRANSACTIONS),
                 'log': create_insert_statement_for_table(LOGS),
                 'token_transfer': create_insert_statement_for_table(TOKEN_TRANSFERS),
                 'trace': create_insert_statement_for_table(TRACES),
                 'token': create_insert_statement_for_table(TOKENS),
                 'contract': create_insert_statement_for_table(CONTRACTS),
             },
-            converters=[UnixTimestampItemConverter(), IntToDecimalItemConverter(),
-                        ListFieldItemConverter('topics', 'topic', fill=4)])
+            converters=[
+                UnixTimestampItemConverter(),
+                IntToDecimalItemConverter(),
+                ListFieldItemConverter('topics', 'topic', fill=4),
+                SimpleItemConverter(field_converters={'blob_versioned_hashes': array_to_str})
+            ])
     elif item_exporter_type == ItemExporterType.GCS:
         from blockchainetl.jobs.exporters.gcs_item_exporter import GcsItemExporter
         bucket, path = get_bucket_and_path_from_gcs_output(output)
         item_exporter = GcsItemExporter(bucket=bucket, path=path)
     elif item_exporter_type == ItemExporterType.CONSOLE:
         item_exporter = ConsoleItemExporter()
     elif item_exporter_type == ItemExporterType.KAFKA:
```

### Comparing `ethereum-etl-2.4.1/ethereumetl/streaming/postgres_tables.py` & `ethereum-etl-2.4.2/ethereumetl/streaming/postgres_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,17 @@
     Column('total_difficulty', Numeric(38)),
     Column('size', BigInteger),
     Column('extra_data', String),
     Column('gas_limit', BigInteger),
     Column('gas_used', BigInteger),
     Column('transaction_count', BigInteger),
     Column('base_fee_per_gas', BigInteger),
+    Column('withdrawals_root', String),
+    Column('blob_gas_used', BigInteger),
+    Column('excess_blob_gas', BigInteger),
 )
 
 TRANSACTIONS = Table(
     'transactions', metadata,
     Column('hash', String, primary_key=True),
     Column('nonce', BigInteger),
     Column('transaction_index', BigInteger),
@@ -74,14 +77,18 @@
     Column('max_priority_fee_per_gas', BigInteger),
     Column('transaction_type', BigInteger),
     Column('receipt_effective_gas_price', BigInteger),
     Column('receipt_l1_fee', BigInteger),
     Column('receipt_l1_gas_used', BigInteger),
     Column('receipt_l1_gas_price', BigInteger),
     Column('receipt_l1_fee_scalar', Float),
+    Column('max_fee_per_blob_gas', BigInteger),
+    Column('blob_versioned_hashes', String),
+    Column('receipt_blob_gas_price', BigInteger),
+    Column('receipt_blob_gas_used', BigInteger),
 )
 
 LOGS = Table(
     'logs', metadata,
     Column('log_index', BigInteger, primary_key=True),
     Column('transaction_hash', String, primary_key=True),
     Column('transaction_index', BigInteger),
```

### Comparing `ethereum-etl-2.4.1/ethereumetl/thread_local_proxy.py` & `ethereum-etl-2.4.2/ethereumetl/thread_local_proxy.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/utils.py` & `ethereum-etl-2.4.2/ethereumetl/utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/ethereumetl/web3_utils.py` & `ethereum-etl-2.4.2/ethereumetl/web3_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/setup.py` & `ethereum-etl-2.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 long_description = read('README.md') if os.path.isfile("README.md") else ""
 
 setup(
     name='ethereum-etl',
-    version='2.4.1',
+    version='2.4.2',
     author='Evgeny Medvedev',
     author_email='evge.medvedev@gmail.com',
     description='Tools for exporting Ethereum blockchain data to CSV or JSON',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blockchain-etl/ethereum-etl',
     packages=find_packages(exclude=['schemas', 'tests']),
```

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/__init__.py` & `ethereum-etl-2.4.2/tests/ethereumetl/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/__init__.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/helpers.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/helpers.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/mock_batch_web3_provider.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/mock_batch_web3_provider.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/mock_web3_provider.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/mock_web3_provider.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_blocks_job.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_blocks_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_contracts_job.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_contracts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_geth_traces_job.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_origin_job.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_origin_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_receipts_job.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_receipts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_token_transfers_job.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_tokens_job.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_tokens_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_traces_job.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/test_export_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/test_extract_geth_traces_job.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/test_extract_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/job/test_extract_token_transfers_job.py` & `ethereum-etl-2.4.2/tests/ethereumetl/job/test_extract_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/service/__init__.py` & `ethereum-etl-2.4.2/tests/ethereumetl/service/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/service/test_eth_contract_service.py` & `ethereum-etl-2.4.2/tests/ethereumetl/service/test_eth_contract_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/service/test_eth_service.py` & `ethereum-etl-2.4.2/tests/ethereumetl/service/test_eth_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/service/test_token_transfer_extractor.py` & `ethereum-etl-2.4.2/tests/ethereumetl/service/test_token_transfer_extractor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/ethereumetl/test_progress_logger.py` & `ethereum-etl-2.4.2/tests/ethereumetl/test_progress_logger.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.4.1/tests/resources/__init__.py` & `ethereum-etl-2.4.2/tests/resources/__init__.py`

 * *Files identical despite different names*

