# Comparing `tmp/opperai-0.2.6.tar.gz` & `tmp/opperai-0.3.0.tar.gz`

## Comparing `opperai-0.2.6.tar` & `opperai-0.3.0.tar`

### file list

```diff
@@ -1,53 +1,82 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.2.6/pytest.ini
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.2.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/__init__.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/_client.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/_http_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/functions/__init__.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/functions/_async_functions.py
--rw-r--r--   0        0        0     5724 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/functions/_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/functions/decorator/__init__.py
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/functions/decorator/_decorator.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/functions/decorator/_schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/indexes/__init__.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/indexes/_async_indexes.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/indexes/_indexes.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/spans/__init__.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/spans/_async_spans.py
--rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/spans/_decorator.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/spans/_spans.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/types/__init__.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/types/exceptions.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/types/indexes.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/types/spans.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/types/validators.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.2.6/src/opperai/utils/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/conftest.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/test_async_functions.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/test_async_indexes.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/test_async_spans.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/test_decorator.py
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/test_functions.py
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/test_indexes.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/test_spans.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/test_trace_decorator.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/test_types.py
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat[function0].yaml
--rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream[function0].yaml
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
--rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id[function0].yaml
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path[function0].yaml
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_get[function0].yaml
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id[function0].yaml
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path[function0].yaml
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function[function0].yaml
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.2.6/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.2.6/.gitignore
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 opperai-0.2.6/README.md
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 opperai-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 opperai-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.3.0/pytest.ini
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/__init__.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/_client.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/_http_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/functions/__init__.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/functions/_async_functions.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/functions/_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/functions/decorator/__init__.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/functions/decorator/_decorator.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/functions/decorator/_schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/indexes/__init__.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/indexes/_async_indexes.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/indexes/_indexes.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/spans/__init__.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/spans/_async_spans.py
+-rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/spans/_decorator.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/spans/_spans.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/types/__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/types/exceptions.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/types/indexes.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/types/spans.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/types/validators.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.3.0/src/opperai/utils/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/test_async_functions.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/test_async_indexes.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/test_async_spans.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/test_decorator.py
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/test_functions.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/test_indexes.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/test_spans.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/test_trace_decorator.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/test_types.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.3.0/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 opperai-0.3.0/README.md
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 opperai-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 opperai-0.3.0/PKG-INFO
```

### Comparing `opperai-0.2.6/.github/workflows/publish.yml` & `opperai-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `opperai-0.2.6/src/opperai/_client.py` & `opperai-0.3.0/src/opperai/_client.py`

 * *Files identical despite different names*

### Comparing `opperai-0.2.6/src/opperai/_http_clients.py` & `opperai-0.3.0/src/opperai/_http_clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import httpx
 from httpx_sse import aconnect_sse, connect_sse
 
 
 class _async_http_client:
     def __init__(self, api_key: str, api_url, timeout):
-        print(f"api_key: {api_key}")
         self.session = httpx.AsyncClient(
             base_url=api_url,
             headers={"X-OPPER-API-KEY": f"{api_key}"},
             timeout=httpx.Timeout(timeout),
         )
 
     async def do_request(self, method: str, path: str, **kwargs):
```

### Comparing `opperai-0.2.6/src/opperai/functions/_async_functions.py` & `opperai-0.3.0/src/opperai/functions/_async_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-from typing import Generator
+from typing import Generator, Optional
 
 from opperai._http_clients import _async_http_client
 from opperai.spans import get_current_span_id
 from opperai.types import (
     ChatPayload,
-    FunctionDescription,
+    Function,
     FunctionResponse,
     StreamingChunk,
     validate_id_xor_path,
 )
 from opperai.types.exceptions import APIError, RateLimitError
 
 
 class AsyncFunctions:
     def __init__(self, http_client: _async_http_client, default_model: str = None):
         self.http_client = http_client
         self.default_model = default_model
 
-    async def _create(self, function: FunctionDescription, **kwargs) -> int:
+    async def _create(self, function: Function, **kwargs) -> Function:
         if not function.model and self.default_model:
             function.model = self.default_model
         response = await self.http_client.do_request(
             "POST",
             "/api/v1/functions",
             json={**function.model_dump(), **kwargs},
         )
         if response.status_code != 200:
             raise APIError(
                 f"Failed to create function {function.path} with status {response.status_code}"
             )
 
-        return response.json()["id"]
+        return Function.model_validate(response.json())
 
-    async def update(self, function: FunctionDescription, **kwargs) -> int:
+    async def update(self, function: Function, **kwargs) -> Function:
         response = await self.http_client.do_request(
             "POST",
             f"/api/v1/functions/{function.id}",
             json={**function.model_dump(), **kwargs},
         )
         if response.status_code != 200:
             raise APIError(
                 f"Failed to update function {function.path} with status {response.status_code}"
             )
 
-        return response.json()["id"]
+        return Function.model_validate(response.json())
 
     @validate_id_xor_path
-    async def get(self, id: str = None, path: str = None) -> FunctionDescription:
+    async def get(self, id: str = None, path: str = None) -> Optional[Function]:
         if path is not None:
             if id is not None:
                 raise ValueError("Only one of id or path should be provided")
-            return await self.get_by_path(path)
+            return await self._get_by_path(path)
         elif id is not None:
-            return await self.get_by_id(id)
+            return await self._get_by_id(id)
         else:
             return None
 
-    async def get_by_path(self, function_path: str) -> FunctionDescription:
+    async def _get_by_path(self, function_path: str) -> Function:
         response = await self.http_client.do_request(
             "GET",
             f"/api/v1/functions/by_path/{function_path}",
         )
         if response.status_code == 404:
             return None
         if response.status_code != 200:
             raise APIError(
                 f"Failed to get function {function_path} with status {response.status_code}"
             )
 
-        return FunctionDescription(**response.json())
+        return Function.model_validate(response.json())
 
-    async def get_by_id(self, function_id: str) -> FunctionDescription:
+    async def _get_by_id(self, function_id: str) -> Function:
         response = await self.http_client.do_request(
             "GET",
             f"/api/v1/functions/{function_id}",
         )
         if response.status_code == 404:
             return None
         if response.status_code != 200:
             raise APIError(
                 f"Failed to get function {function_id} with status {response.status_code}"
             )
 
-        return FunctionDescription(**response.json())
+        return Function.model_validate(response.json())
 
     async def create(
-        self, function: FunctionDescription, update: bool = True, **kwargs
-    ) -> int:
-        fn = await self.get_by_path(function.path)
+        self, function: Function, update: bool = True, **kwargs
+    ) -> Function:
+        fn = await self.get(path=function.path)
         if fn is None:
             return await self._create(function, **kwargs)
         elif update:
             function.id = fn.id
             return await self.update(function, **kwargs)
-        return fn.id
+        return fn
 
     @validate_id_xor_path
     async def delete(self, id: str = None, path: str = None):
         if path is not None:
             try:
                 await self._delete_by_path(path)
             except APIError:
```

### Comparing `opperai-0.2.6/src/opperai/functions/_functions.py` & `opperai-0.3.0/src/opperai/functions/_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,126 +1,125 @@
-from typing import Generator
+from typing import Generator, Optional
 
 from opperai._http_clients import _http_client
 from opperai.spans import get_current_span_id
 from opperai.types import (
     ChatPayload,
-    FunctionDescription,
+    Function,
     FunctionResponse,
     StreamingChunk,
     validate_id_xor_path,
 )
 from opperai.types.exceptions import APIError, RateLimitError
 
 
 class Functions:
     def __init__(self, http_client: _http_client, default_model: str = None):
         self.http_client = http_client
         self.default_model = default_model
 
-    def _create(self, function: FunctionDescription, **kwargs) -> int:
+    def create(self, function: Function, update: bool = True, **kwargs) -> Function:
+        fn = self.get(path=function.path)
+        if fn is None:
+            return self._create(function, **kwargs)
+        elif update:
+            function.id = fn.id
+            return self.update(function, **kwargs)
+        else:
+            return fn
+
+    def _create(self, function: Function, **kwargs) -> Function:
         if not function.model and self.default_model:
             function.model = self.default_model
         response = self.http_client.do_request(
             "POST",
             "/api/v1/functions",
             json={**function.model_dump(), **kwargs},
         )
         if response.status_code != 200:
             raise APIError(
                 f"Failed to create function {function.path} with status {response.status_code}: {response.text}"
             )
 
-        return response.json()["id"]
+        return Function.model_validate(response.json())
 
-    def update(self, function: FunctionDescription, **kwargs) -> int:
+    def update(self, function: Function, **kwargs) -> Function:
         response = self.http_client.do_request(
             "POST",
             f"/api/v1/functions/{function.id}",
             json={**function.model_dump(), **kwargs},
         )
         if response.status_code != 200:
             raise APIError(
                 f"Failed to update function `{function.path}` with status {response.status_code}: {response.text}"
             )
 
-        return response.json()["id"]
+        return Function.model_validate(response.json())
 
     @validate_id_xor_path
-    def get(self, id: str = None, path: str = None) -> FunctionDescription:
+    def get(self, id: str = None, path: str = None) -> Optional[Function]:
         if path is not None:
             if id is not None:
                 raise ValueError("Only one of id or path should be provided")
-            return self.get_by_path(path)
+            return self._get_by_path(path)
         elif id is not None:
-            return self.get_by_id(id)
+            return self._get_by_id(id)
         else:
             return None
 
-    def get_by_path(self, function_path: str) -> FunctionDescription:
+    def _get_by_path(self, function_path: str) -> Optional[Function]:
         response = self.http_client.do_request(
             "GET",
             f"/api/v1/functions/by_path/{function_path}",
         )
         if response.status_code == 404:
             return None
         if response.status_code != 200:
             raise APIError(
                 f"Failed to get function {function_path} with status {response.status_code}"
             )
 
-        return FunctionDescription(**response.json())
+        return Function.model_validate(response.json())
 
-    def get_by_id(self, function_id: str) -> FunctionDescription:
+    def _get_by_id(self, function_id: str) -> Optional[Function]:
         response = self.http_client.do_request(
             "GET",
             f"/api/v1/functions/{function_id}",
         )
         if response.status_code == 404:
             return None
         if response.status_code != 200:
             raise APIError(
                 f"Failed to get function {function_id} with status {response.status_code}"
             )
 
-        return FunctionDescription(**response.json())
-
-    def create(
-        self, function: FunctionDescription, update: bool = True, **kwargs
-    ) -> int:
-        fn = self.get(path=function.path)
-        if fn is None:
-            return self._create(function, **kwargs)
-        elif update:
-            function.id = fn.id
-            return self.update(function, **kwargs)
-        else:
-            return fn.id
+        return Function.model_validate(response.json())
 
     @validate_id_xor_path
-    def delete(self, id: str = None, path: str = None) -> None:
+    def delete(self, id: str = None, path: str = None) -> bool:
         if path is not None:
             try:
-                self._delete_by_path(path)
+                return self._delete_by_path(path)
             except APIError:
                 pass
         elif id is not None:
-            fn = self.get(id)
+            fn = self.get(id=id)
             if fn:
-                self._delete_by_path(fn.path)
+                return self._delete_by_path(fn.path)
 
-    def _delete_by_path(self, function_path: str) -> None:
+    def _delete_by_path(self, function_path: str) -> bool:
         response = self.http_client.do_request(
             "DELETE",
             f"/api/v1/functions/by_path/{function_path}",
         )
         if response.status_code != 200:
             raise APIError(
                 f"Failed to delete function {function_path} with status {response.status_code}"
             )
+        return True
 
     def chat(
         self, function_path, data: ChatPayload, stream=False, **kwargs
     ) -> [FunctionResponse, Generator[StreamingChunk, None, None]]:
         if data.parent_span_uuid is None:
             data.parent_span_uuid = get_current_span_id()
 
@@ -136,31 +135,33 @@
             raise RateLimitError("Rate limit error: please retry in a few seconds")
 
         if response.status_code != 200:
             raise APIError(
                 f"Failed to run function {function_path} with status {response.status_code}"
             )
 
-        return FunctionResponse(**response.json())
+        return FunctionResponse.model_validate(response.json())
 
     def _chat_stream(
         self, function_path, data: ChatPayload, **kwargs
     ) -> Generator[StreamingChunk, None, None]:
         serialized_data = data.model_dump()
         gen = self.http_client.stream(
             "POST",
             f"/v1/chat/{function_path}",
             json={**serialized_data, **kwargs},
             params={"stream": "True"},
         )
         for item in gen:
             yield StreamingChunk(**item)
 
-    def flush_cache(self, id: int) -> None:
+    def flush_cache(self, id: int) -> bool:
         response = self.http_client.do_request(
             "DELETE",
             f"/api/v1/functions/{id}/cache",
         )
         if response.status_code != 204:
             raise APIError(
                 f"Failed to flush cache for function with id={id} with status {response.status_code}"
             )
+
+        return True
```

### Comparing `opperai-0.2.6/src/opperai/functions/decorator/_decorator.py` & `opperai-0.3.0/src/opperai/functions/decorator/_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from functools import wraps
 from typing import List, get_args, get_origin, get_type_hints
 
 from pydantic import BaseModel
 
 from opperai import AsyncClient, Client
 from opperai.spans import _current_span_id
-from opperai.types import CacheConfiguration, ChatPayload, FunctionDescription, Message
+from opperai.types import CacheConfiguration, ChatPayload, Function, Message
 
 from ...utils import convert_function_call_to_json
 from ._schemas import get_output_schema
 
 _thread_local = threading.local()
 
 
@@ -59,15 +59,15 @@
                 sync_client = Client(api_key=client.api_key, api_url=client.api_url)
             elif isinstance(client, Client):
                 sync_client = client
             else:
                 sync_client = Client()
 
             use_few_shot = few_shot or os.environ.get("OPPER_USE_FEW_SHOT", False)
-            function = FunctionDescription(
+            function = Function(
                 path=func_path,
                 description=func.__doc__,
                 instructions=f"Operation: {func.__name__}\n\nOperation description: {func.__doc__}",
                 out_schema=get_output_schema(func),
                 few_shot=use_few_shot,
             )
             if use_few_shot:
```

### Comparing `opperai-0.2.6/src/opperai/functions/decorator/_schemas.py` & `opperai-0.3.0/src/opperai/functions/decorator/_schemas.py`

 * *Files identical despite different names*

### Comparing `opperai-0.2.6/src/opperai/indexes/_async_indexes.py` & `opperai-0.3.0/src/opperai/indexes/_indexes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,115 +1,147 @@
 from typing import List, Optional
 
-from opperai._http_clients import _async_http_client
+from opperai._http_clients import _http_client
 from opperai.types.exceptions import APIError
 from opperai.types.indexes import (
-    DocumentIn,
-    DocumentOut,
+    Document,
+    Document,
     Filter,
-    IndexOut,
-    IndexRetrieveResponse,
+    Index,
+    RetrievalResponse,
 )
+from pydantic import BaseModel
 
 
-class AsyncIndexes:
-    def __init__(self, http_client: _async_http_client):
+class RetrieveQuery(BaseModel):
+    q: str
+    k: int
+    filters: Optional[List[Filter]]
+
+
+class Indexes:
+    def __init__(self, http_client: _http_client):
         self.http_client = http_client
 
-    async def create(self, name: str) -> int:
-        response = await self.http_client.do_request(
+    def create(self, name: str) -> Index:
+        response = self.http_client.do_request(
             "POST",
             "/v1/indexes",
             json={"name": name},
         )
         if response.status_code != 200:
             raise APIError(f"Failed to create index with status {response.status_code}")
-        return response.json()["id"]
+        return Index.model_validate(response.json())
 
-    async def delete(self, index_id: int):
-        response = await self.http_client.do_request(
+    def delete(self, id: int) -> bool:
+        response = self.http_client.do_request(
             "DELETE",
-            f"/v1/indexes/{index_id}",
+            f"/v1/indexes/{id}",
         )
+        if response.status_code == 404:
+            return False
         if response.status_code != 200:
             raise APIError(f"Failed to delete index with status {response.status_code}")
-        return response.json()
+        return True
+
+    def get(self, id: int = None, name: str = None) -> Optional[Index]:
+        if id is None and name is None:
+            raise ValueError("Either id or name must be provided")
+        if id is not None and name is not None:
+            raise ValueError("Only one of id or name should be provided")
+
+        if id is not None:
+            return self._get_by_id(id)
+        if name is not None:
+            return self._get_by_name(name)
 
-    async def list(self):
-        response = await self.http_client.do_request(
+    def _get_by_id(self, id: int) -> Optional[Index]:
+        response = self.http_client.do_request(
             "GET",
-            "/v1/indexes",
+            f"/v1/indexes/{id}",
         )
+        if response.status_code == 404:
+            return None
         if response.status_code != 200:
-            raise APIError(f"Failed to list indexes with status {response.status_code}")
-        return [IndexOut.model_validate(item) for item in response.json()]
+            raise APIError(f"Failed to get index with status {response.status_code}")
+
+        return Index.model_validate(response.json())
 
-    async def get_by_name(self, name: str) -> IndexOut:
-        indexes = await self.list()
+    def _get_by_name(self, name: str) -> Optional[Index]:
+        indexes = self.list()
         for index in indexes:
             if index.name == name:
                 return index
         return None
 
-    async def upload_file(self, index_id: int, file_path: str, **kwargs):
+    def list(self) -> List[Index]:
+        response = self.http_client.do_request(
+            "GET",
+            "/v1/indexes",
+        )
+        if response.status_code != 200:
+            raise APIError(f"Failed to list indexes with status {response.status_code}")
+        return [Index.model_validate(item) for item in response.json()]
+
+    def upload_file(self, id: int, file_path: str, **kwargs):
         # Get upload URL
-        upload_url_response = await self.http_client.do_request(
+        upload_url_response = self.http_client.do_request(
             "GET",
-            f"/v1/indexes/{index_id}/upload_url",
+            f"/v1/indexes/{id}/upload_url",
             params={"filename": file_path.split("/")[-1]},
         )
         if upload_url_response.status_code != 200:
             raise APIError(
                 f"Failed to get upload URL with status {upload_url_response.status_code}"
             )
         upload_url_data = upload_url_response.json()
 
         # Upload file
         with open(file_path, "rb") as file:
             files = {"file": (file_path.split("/")[-1], file)}
-            upload_response = await self.http_client.do_request(
+            upload_response = self.http_client.do_request(
                 "POST",
                 upload_url_data["url"],
                 files=files,
                 data=upload_url_data["fields"],
             )
             if upload_response.status_code not in [200, 204]:
                 raise APIError(
                     f"Failed to upload file with status {upload_response.status_code}"
                 )
 
         # Register file
-        register_file_response = await self.http_client.do_request(
+        register_file_response = self.http_client.do_request(
             "POST",
-            f"/v1/indexes/{index_id}/register_file",
+            f"/v1/indexes/{id}/register_file",
             json={"uuid": upload_url_data["uuid"], **kwargs},
         )
         if register_file_response.status_code != 200:
             raise APIError(
                 f"Failed to register file with status {register_file_response.status_code}"
             )
 
         return register_file_response.json()
 
-    async def index(self, index_id: int, doc: DocumentIn) -> DocumentOut:
-        response = await self.http_client.do_request(
+    def index(self, id: int, doc: Document) -> Document:
+        response = self.http_client.do_request(
             "POST",
-            f"/v1/indexes/{index_id}/index",
+            f"/v1/indexes/{id}/index",
             json=doc.model_dump(),
         )
         if response.status_code != 200:
             raise APIError(f"Failed to add document with status {response.status_code}")
-        return DocumentOut.model_validate(response.json())
+        return Document.model_validate(response.json())
 
-    async def retrieve(
-        self, index_id: int, query: str, k: int, filters: Optional[List[Filter]] = None
-    ) -> List[IndexRetrieveResponse]:
-        response = await self.http_client.do_request(
+    def retrieve(
+        self, id: int, query: str, k: int, filters: Optional[List[Filter]] = None
+    ) -> List[RetrievalResponse]:
+        response = self.http_client.do_request(
             "POST",
-            f"/v1/indexes/{index_id}/query",
-            json={"q": query, "k": k, "filters": filters or []},
+            f"/v1/indexes/{id}/query",
+            json=RetrieveQuery(q=query, k=k, filters=filters).model_dump(),
         )
         if response.status_code != 200:
             raise APIError(
-                f"Failed to retrieve index {index_id} with status {response.status_code}"
+                f"Failed to retrieve index {id} with status {response.status_code}"
             )
-        return [IndexRetrieveResponse.model_validate(item) for item in response.json()]
+        return [RetrievalResponse.model_validate(item) for item in response.json()]
```

### Comparing `opperai-0.2.6/src/opperai/spans/_async_spans.py` & `opperai-0.3.0/src/opperai/spans/_async_spans.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,77 +1,80 @@
 import json
 from uuid import UUID
 
 from opperai._http_clients import _async_http_client
 from opperai.types.spans import Span, SpanFeedback
 from opperai.types.exceptions import APIError
 from opperai.utils import DateTimeEncoder
+from typing import Dict, Any
 
 
 class AsyncSpans:
     def __init__(self, http_client: _async_http_client):
         self.http_client = http_client
 
-    async def create(self, span: Span, **kwargs) -> str:
+    async def create(self, span: Span, **kwargs) -> Span:
         span_data = span.model_dump(exclude_none=True)
         json_payload = json.dumps(span_data, cls=DateTimeEncoder)
         response = await self.http_client.do_request(
             "POST",
             "/v1/spans",
-            data=json_payload,
+            content=json_payload,
         )
         if response.status_code != 200:
             raise APIError(
                 f"Failed to create span {span.name} with status {response.status_code}"
             )
 
-        return response.json()["uuid"]
+        return Span.model_validate(response.json())
 
-    async def update(self, span_uuid: UUID, **kwargs) -> str:
+    async def update(self, span_uuid: UUID, **kwargs) -> Span:
         span = Span(uuid=span_uuid, **kwargs)
         json_payload = json.dumps(
             span.model_dump(exclude_none=True), cls=DateTimeEncoder
         )
         response = await self.http_client.do_request(
             "PUT",
             f"/v1/spans/{span.uuid}",
-            data=json_payload,
+            content=json_payload,
         )
         if response.status_code != 200:
             raise APIError(
                 f"Failed to update span `{span.name}` with status {response.status_code}"
             )
 
-        return response.json()["uuid"]
+        return Span.model_validate(response.json())
 
     async def delete(self, span_uuid: UUID) -> bool:
         response = await self.http_client.do_request(
             "DELETE",
             f"/v1/spans/{span_uuid}",
         )
         if response.status_code != 204:
             raise APIError(
                 f"Failed to update span `{span_uuid}` with status {response.status_code}"
             )
 
         return True
 
-    async def save_example(self, uuid: str, **kwargs) -> str:
+    async def save_example(self, uuid: str, **kwargs) -> Dict[str, Any]:
         response = await self.http_client.do_request(
             "POST",
             f"/v1/spans/{uuid}/save_examples",
         )
         if response.status_code != 200:
             raise APIError(
                 f"Failed to save examples for span {uuid} with status {response.status_code}"
             )
 
-        return response.json()["uuid"]
+        return response.json()
 
-    async def save_feedback(self, uuid: str, feedback: SpanFeedback, **kwargs) -> str:
+    async def save_feedback(
+        self, uuid: str, feedback: SpanFeedback, **kwargs
+    ) -> Dict[str, Any]:
         response = await self.http_client.do_request(
             "POST",
             f"/v1/spans/{uuid}/feedbacks",
             json=feedback.model_dump(exclude_unset=True),
         )
         if response.status_code != 200:
             raise APIError(
```

### Comparing `opperai-0.2.6/src/opperai/spans/_decorator.py` & `opperai-0.3.0/src/opperai/spans/_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.2.6/src/opperai/spans/_spans.py` & `opperai-0.3.0/src/opperai/spans/_spans.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def create(self, span: Span, **kwargs) -> str:
         span_data = span.model_dump(exclude_none=True)
         json_payload = json.dumps(span_data, cls=DateTimeEncoder)
         response = self.http_client.do_request(
             "POST",
             "/v1/spans",
-            data=json_payload,
+            content=json_payload,
         )
         if response.status_code != 200:
             raise APIError(
                 f"Failed to create span {span.name} with status {response.status_code}"
             )
         return response.json()["uuid"]
 
@@ -31,15 +31,15 @@
         span = Span(uuid=span_uuid, **kwargs)
         json_payload = json.dumps(
             span.model_dump(exclude_none=True), cls=DateTimeEncoder
         )
         response = self.http_client.do_request(
             "PUT",
             f"/v1/spans/{span.uuid}",
-            data=json_payload,
+            content=json_payload,
         )
         if response.status_code != 200:
             raise APIError(
                 f"Failed to update span `{span.name}` with status {response.status_code}"
             )
 
         return response.json()["uuid"]
```

### Comparing `opperai-0.2.6/src/opperai/types/__init__.py` & `opperai-0.3.0/src/opperai/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,24 +48,24 @@
 
 class CacheConfiguration(BaseModel):
     exact_match_cache_ttl: Optional[int] = None
     semantic_cache_threshold: Optional[float] = None
     semantic_cache_ttl: Optional[int] = None
 
 
-class FunctionDescription(BaseModel):
+class Function(BaseModel):
     id: Optional[int] = None
     path: str = Field(
         ...,
         pattern=r"^[a-zA-Z0-9_]+(\/[a-zA-Z0-9_-]+)*$",
         description="Path should not contain characters that could break URLs.",
     )
     description: str
     input_schema: Optional[Dict[str, Any]] = None
     out_schema: Optional[Dict[str, Any]] = None
     instructions: str
     model: Optional[str] = None
-    index_ids: Optional[List[int]] = None
+    index_ids: Optional[List[int]] = []
     use_semantic_search: Optional[bool] = None
     few_shot: Optional[bool] = None
     few_shot_count: Optional[int] = None
     cache_configuration: Optional[CacheConfiguration] = None
```

### Comparing `opperai-0.2.6/src/opperai/types/indexes.py` & `opperai-0.3.0/src/opperai/types/indexes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 import datetime
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from pydantic import UUID4, BaseModel, Field
 
 
-class IndexRetrieveResponse(BaseModel):
+class RetrievalResponse(BaseModel):
     content: str
-    metadata: dict
+    metadata: Dict[str, Any]
 
 
-class DocumentIn(BaseModel):
-    id: Optional[str] = None
+class Document(BaseModel):
+    id: Optional[int] = None
+    uuid: Optional[UUID4] = None
     key: Optional[str] = None
-    content: str = Field(..., min_length=1)
-    metadata: dict = dict()
+    content: Optional[str] = Field(None, min_length=1)
+    metadata: Optional[Dict[str, Any]] = None
 
 
-class DocumentOut(BaseModel):
-    id: int
-    uuid: UUID4
-    key: str
-
-
-class IndexOut(BaseModel):
+class Index(BaseModel):
     id: int
     name: str
     created_at: datetime.datetime
 
 
 class Filter(BaseModel):
     key: str
```

### Comparing `opperai-0.2.6/src/opperai/types/spans.py` & `opperai-0.3.0/src/opperai/types/spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.2.6/src/opperai/types/validators.py` & `opperai-0.3.0/src/opperai/types/validators.py`

 * *Files identical despite different names*

### Comparing `opperai-0.2.6/src/opperai/utils/__init__.py` & `opperai-0.3.0/src/opperai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.2.6/tests/conftest.py` & `opperai-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opperai-0.2.6/tests/test_async_spans.py` & `opperai-0.3.0/tests/test_async_spans.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 from datetime import datetime
 import pytest
-from opperai.types.spans import Span
+from opperai.types.spans import Span, SpanFeedback
 from opperai import AsyncClient
+from contextlib import asynccontextmanager
+
+
+@asynccontextmanager
+async def span(desc: Span, _client: AsyncClient):
+    _span = await _client.spans.create(desc)
+    try:
+        yield _span
+    finally:
+        await _client.spans.delete(_span.uuid)
 
 
 @pytest.mark.asyncio(scope="module")
 async def test_async_crud(aclient: AsyncClient, vcr_cassette):
     root_uuid = "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"
     root_start_time = datetime(2021, 1, 1, 0, 0, 0, 0)
     root_end_time = datetime(2022, 1, 1, 0, 0, 0, 0)
@@ -45,7 +55,24 @@
         root_span.uuid,
         end_time=root_end_time,
         output="output",
     )
 
     assert await aclient.spans.delete(child_span.uuid)
     assert await aclient.spans.delete(root_span.uuid)
+
+
+@pytest.mark.asyncio(scope="module")
+async def test_save_feedback(aclient: AsyncClient, vcr_cassette):
+    async with span(
+        Span(
+            uuid="bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133",
+            project="project",
+            name="name",
+            input="input",
+            start_time=datetime(2021, 1, 1, 0, 0, 0, 0),
+        ),
+        aclient,
+    ) as _span:
+        await aclient.spans.save_feedback(
+            _span.uuid, SpanFeedback(dimension="dim", score=0.5, comment="comment")
+        )
```

### Comparing `opperai-0.2.6/tests/test_decorator.py` & `opperai-0.3.0/tests/test_decorator.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,34 @@
 from pydantic import BaseModel
 
 
 @patch("opperai._http_clients._http_client.do_request")
 def test_decorator(mock_do_request):
     mock_do_request.side_effect = [
         MagicMock(status_code=404),
-        MagicMock(status_code=200, json=lambda: {"id": 1}),
+        MagicMock(
+            status_code=200,
+            json=lambda: {
+                "id": 1,
+                "path": "path",
+                "description": "description",
+                "instructions": "instructions",
+            },
+        ),
         MagicMock(status_code=200, json=lambda: {"json_payload": "Hola"}),
         MagicMock(status_code=404),
-        MagicMock(status_code=200, json=lambda: {"id": 2}),
+        MagicMock(
+            status_code=200,
+            json=lambda: {
+                "id": 2,
+                "path": "path",
+                "description": "description",
+                "instructions": "instructions",
+            },
+        ),
         MagicMock(status_code=200, json=lambda: {"json_payload": ["Hola", "Bonjour"]}),
     ]
 
     @fn()
     def translate(text: str, target_language: str) -> str:
         """Translate text to a target language."""
 
@@ -32,18 +48,34 @@
     assert translate_list("Hello", ["es", "fr"]) == ["Hola", "Bonjour"]
 
 
 @patch("opperai._http_clients._http_client.do_request")
 def test_decorator_supply_model(mock_do_request):
     mock_do_request.side_effect = [
         MagicMock(status_code=404),
-        MagicMock(status_code=200, json=lambda: {"id": 1}),
+        MagicMock(
+            status_code=200,
+            json=lambda: {
+                "id": 1,
+                "path": "path",
+                "description": "description",
+                "instructions": "instructions",
+            },
+        ),
         MagicMock(status_code=200, json=lambda: {"json_payload": "Hola"}),
         MagicMock(status_code=404),
-        MagicMock(status_code=200, json=lambda: {"id": 2}),
+        MagicMock(
+            status_code=200,
+            json=lambda: {
+                "id": 2,
+                "path": "path",
+                "description": "description",
+                "instructions": "instructions",
+            },
+        ),
         MagicMock(status_code=200, json=lambda: {"json_payload": ["Hola", "Bonjour"]}),
     ]
 
     @fn(model="gpt-4-0125-preview")
     def translate(text: str, target_language: str) -> str:
         """Translate text to a target language."""
```

### Comparing `opperai-0.2.6/tests/test_spans.py` & `opperai-0.3.0/tests/test_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.2.6/tests/test_trace_decorator.py` & `opperai-0.3.0/tests/test_trace_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.2.6/tests/test_types.py` & `opperai-0.3.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat[function0].yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,126 +1,127 @@
 interactions:
 - request:
-    body: ''
+    body: '{"name": "test_retrieve_document"}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
+      content-length:
+      - '34'
+      content-type:
+      - application/json
       user-agent:
       - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_async_chat
+    method: POST
+    uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"id":257,"name":"test_retrieve_document","files":[],"created_at":"2024-04-11T16:25:34.538913Z"}'
     headers:
       content-length:
-      - '31'
+      - '96'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:25:33 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 200
+      message: OK
 - request:
-    body: '{"id": null, "path": "test/sdk/test_async_chat", "description": "Test function",
-      "input_schema": null, "out_schema": null, "instructions": "translate to french",
-      "model": null, "index_ids": null, "use_semantic_search": null, "few_shot": null,
-      "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
+      {"source": "test"}}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '295'
+      - '91'
       content-type:
       - application/json
       user-agent:
       - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/indexes/257/index
   response:
     body:
-      string: '{"id":42}'
+      string: '{"id":86,"uuid":"8320bd18-12da-4104-8f09-cfdb4b10e8e3","key":"8320bd18-12da-4104-8f09-cfdb4b10e8e3"}'
     headers:
       content-length:
-      - '9'
+      - '100'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:25:33 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"q": "Hello", "k": 1, "filters": null}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
+      content-length:
+      - '39'
+      content-type:
+      - application/json
       user-agent:
       - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/42
+    method: POST
+    uri: http://localhost:8000/v1/indexes/257/query
   response:
     body:
-      string: '{"id":42,"path":"test/sdk/test_async_chat","description":"Test function","input_schema":null,"dataset_uuid":"95a46013-feb0-43ce-b89d-0eb37e54f799","out_schema":null,"instructions":"translate
-        to french","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '[{"uuid":"060d77ca-09e7-4436-96cb-29ab17a8b160","content":"Hello","metadata":{"source":"test"},"document_id":null,"score":29.458036422729492,"source_uuids":["060d77ca-09e7-4436-96cb-29ab17a8b160"]}]'
     headers:
       content-length:
-      - '377'
+      - '198'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:25:33 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
+    body: ''
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
-      content-length:
-      - '78'
-      content-type:
-      - application/json
       user-agent:
       - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_async_chat
+    method: DELETE
+    uri: http://localhost:8000/v1/indexes/257
   response:
     body:
-      string: '{"event_id":"b63d9ae2-5427-4efc-97aa-e46d5dabc380","message":"Bonjour","json_payload":null,"error":null,"context":null,"cached":false}'
+      string: 'true'
     headers:
       content-length:
-      - '134'
+      - '4'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:25:33 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream[function0].yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -7,60 +7,61 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_async_chat_stream
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:23 GMT
+      - Thu, 11 Apr 2024 16:26:06 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_async_chat_stream", "description":
-      "Test function", "input_schema": null, "out_schema": null, "instructions": "translate
-      to french", "model": null, "index_ids": null, "use_semantic_search": null, "few_shot":
-      null, "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_create_function", "description": "Test
+      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
+      "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
+      "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '302'
+      - '291'
       content-type:
       - application/json
       user-agent:
       - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/api/v1/functions
   response:
     body:
-      string: '{"id":43}'
+      string: '{"id":52,"path":"test/sdk/test_create_function","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"5c2ded91-dd84-4161-ae5d-269130628be4","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '9'
+      - '392'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:23 GMT
+      - Thu, 11 Apr 2024 16:26:06 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -70,67 +71,54 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/43
+    uri: http://localhost:8000/api/v1/functions/52
   response:
     body:
-      string: '{"id":43,"path":"test/sdk/test_async_chat_stream","description":"Test
-        function","input_schema":null,"dataset_uuid":"03c4d2d1-beee-4a24-9e46-71932672c92c","out_schema":null,"instructions":"translate
-        to french","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"id":52,"path":"test/sdk/test_create_function","description":"Test
+        function","input_schema":null,"dataset_uuid":"5c2ded91-dd84-4161-ae5d-269130628be4","out_schema":null,"instructions":"Do
+        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
     headers:
       content-length:
-      - '384'
+      - '375'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:23 GMT
+      - Thu, 11 Apr 2024 16:26:06 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
+    body: ''
     headers:
       accept:
-      - text/event-stream
+      - '*/*'
       accept-encoding:
       - gzip, deflate
-      cache-control:
-      - no-store
       connection:
       - keep-alive
-      content-length:
-      - '78'
-      content-type:
-      - application/json
       user-agent:
       - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_async_chat_stream?stream=True
+    method: DELETE
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function
   response:
     body:
-      string: "data: {\"event_id\": \"b96b9ffa-d2cf-40a0-b8e0-07395b30f4bd\"}\r\n\r\ndata:
-        {\"delta\": \"Bonjour\"}\r\n\r\n"
+      string: '{"detail":"Function and associated generations deleted successfully"}'
     headers:
-      Transfer-Encoding:
-      - chunked
-      cache-control:
-      - no-cache
-      connection:
-      - keep-alive
+      content-length:
+      - '69'
       content-type:
-      - text/event-stream; charset=utf-8
+      - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:23 GMT
+      - Thu, 11 Apr 2024 16:26:06 GMT
       server:
       - uvicorn
-      x-accel-buffering:
-      - 'no'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,91 @@
 interactions:
 - request:
-    body: ''
+    body: '{"name": "test_get_by_name"}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
+      content-length:
+      - '28'
+      content-type:
+      - application/json
       user-agent:
       - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_function
+    method: POST
+    uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"id":253,"name":"test_get_by_name","files":[],"created_at":"2024-04-11T16:25:34.227196Z"}'
     headers:
       content-length:
-      - '31'
+      - '90'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:25:33 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 200
+      message: OK
 - request:
-    body: '{"id": null, "path": "test/sdk/test_function", "description": "Test function",
-      "input_schema": null, "out_schema": null, "instructions": "Do something", "model":
-      null, "index_ids": null, "use_semantic_search": null, "few_shot": null, "few_shot_count":
-      null, "cache_configuration": null}'
+    body: ''
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
+      user-agent:
+      - python-httpx/0.27.0
+    method: GET
+    uri: http://localhost:8000/v1/indexes
+  response:
+    body:
+      string: '[{"id":253,"org_id":1,"org_name":null,"name":"test_get_by_name","created_by":"Mattias
+        Lundell","created_at":"2024-04-11T16:25:34.227196Z","updated_at":"2024-04-11T16:25:34.227196Z","count":0}]'
+    headers:
       content-length:
-      - '286'
+      - '192'
       content-type:
       - application/json
+      date:
+      - Thu, 11 Apr 2024 16:25:33 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      accept-encoding:
+      - gzip, deflate
+      connection:
+      - keep-alive
       user-agent:
       - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/api/v1/functions
+    method: DELETE
+    uri: http://localhost:8000/v1/indexes/253
   response:
     body:
-      string: '{"id":35}'
+      string: 'true'
     headers:
       content-length:
-      - '9'
+      - '4'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:25:33 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -7,156 +7,173 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_with_cache_async
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:28 GMT
+      - Mon, 08 Apr 2024 13:34:13 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_create_function_with_cache_async",
-      "description": "Test function", "input_schema": null, "out_schema": null, "instructions":
-      "Do something", "model": null, "index_ids": null, "use_semantic_search": null,
-      "few_shot": null, "few_shot_count": null, "cache_configuration": {"exact_match_cache_ttl":
-      10, "semantic_cache_threshold": null, "semantic_cache_ttl": null}}'
+    body: '{"id": null, "path": "test/sdk/test_delete_function_by_path", "description":
+      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
+      something", "model": null, "index_ids": null, "use_semantic_search": null, "few_shot":
+      null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '397'
+      - '301'
       content-type:
       - application/json
       user-agent:
       - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/api/v1/functions
   response:
     body:
-      string: '{"id":44}'
+      string: '{"id":118}'
     headers:
       content-length:
-      - '9'
+      - '10'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:28 GMT
+      - Mon, 08 Apr 2024 13:34:13 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
+    body: ''
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
-      content-length:
-      - '78'
-      content-type:
-      - application/json
       user-agent:
       - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async
+    method: GET
+    uri: http://localhost:8000/api/v1/functions/118
   response:
     body:
-      string: '{"event_id":"0be17195-ad80-41f4-9980-2d1ad3dc7517","message":"Hello!
-        How can I assist you today? If you have any questions or need information
-        on a specific topic, feel free to ask!","json_payload":null,"error":null,"context":null,"cached":false}'
+      string: '{"id":118,"path":"test/sdk/test_delete_function_by_path","description":"Test
+        function","input_schema":null,"dataset_uuid":"98cf36c4-3b86-4952-abb8-dd418620b5c5","out_schema":null,"instructions":"Do
+        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
     headers:
       content-length:
-      - '246'
+      - '384'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:28 GMT
+      - Mon, 08 Apr 2024 13:34:13 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
+    body: ''
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
+      user-agent:
+      - python-httpx/0.27.0
+    method: DELETE
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
+  response:
+    body:
+      string: '{"detail":"Function and associated generations deleted successfully"}'
+    headers:
       content-length:
-      - '78'
+      - '69'
       content-type:
       - application/json
+      date:
+      - Mon, 08 Apr 2024 13:34:13 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      accept-encoding:
+      - gzip, deflate
+      connection:
+      - keep-alive
       user-agent:
       - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async
+    method: GET
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
   response:
     body:
-      string: '{"event_id":"787d613e-3d05-4f8f-8b6c-7cc78b1232ba","message":"Hello!
-        How can I assist you today? If you have any questions or need information
-        on a specific topic, feel free to ask!","json_payload":null,"error":null,"context":null,"cached":true}'
+      string: '{"detail":"Function not found"}'
     headers:
       content-length:
-      - '245'
+      - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:34 GMT
+      - Mon, 08 Apr 2024 13:34:13 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
-    method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_with_cache_async
+    method: GET
+    uri: http://localhost:8000/api/v1/functions/118
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: '{"detail":"Function not found"}'
     headers:
       content-length:
-      - '69'
+      - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:34 GMT
+      - Mon, 08 Apr 2024 13:34:13 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 version: 1
```

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -7,129 +7,120 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_with_cache_async_flush
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_id
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 19:30:28 GMT
+      - Mon, 08 Apr 2024 13:34:13 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_create_function_with_cache_async_flush",
-      "description": "Test function", "input_schema": null, "out_schema": null, "instructions":
-      "Do something", "model": null, "index_ids": null, "use_semantic_search": null,
-      "few_shot": null, "few_shot_count": null, "cache_configuration": {"exact_match_cache_ttl":
-      10, "semantic_cache_threshold": null, "semantic_cache_ttl": null}}'
+    body: '{"id": null, "path": "test/sdk/test_delete_function_by_id", "description":
+      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
+      something", "model": null, "index_ids": null, "use_semantic_search": null, "few_shot":
+      null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '403'
+      - '299'
       content-type:
       - application/json
       user-agent:
       - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/api/v1/functions
   response:
     body:
-      string: '{"id":50}'
+      string: '{"id":117}'
     headers:
       content-length:
-      - '9'
+      - '10'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 19:30:28 GMT
+      - Mon, 08 Apr 2024 13:34:13 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
+    body: ''
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
-      content-length:
-      - '78'
-      content-type:
-      - application/json
       user-agent:
       - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async_flush
+    method: GET
+    uri: http://localhost:8000/api/v1/functions/117
   response:
     body:
-      string: '{"event_id":"b74364d9-70c2-4597-997a-f1cb683d5078","message":"Hello!
-        How can I assist you today? If you have any questions or need information,
-        feel free to ask.","json_payload":null,"error":null,"context":null,"cached":false}'
+      string: '{"id":117,"path":"test/sdk/test_delete_function_by_id","description":"Test
+        function","input_schema":null,"dataset_uuid":"7984e90d-798e-4b1a-b54b-4701878c96d2","out_schema":null,"instructions":"Do
+        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
     headers:
       content-length:
-      - '226'
+      - '382'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 19:30:28 GMT
+      - Mon, 08 Apr 2024 13:34:13 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
+    body: ''
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
-      content-length:
-      - '78'
-      content-type:
-      - application/json
       user-agent:
       - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async_flush
+    method: GET
+    uri: http://localhost:8000/api/v1/functions/117
   response:
     body:
-      string: '{"event_id":"090dfc40-a839-43bb-a4c1-6de0a410ea4a","message":"Hello!
-        How can I assist you today? If you have any questions or need information,
-        feel free to ask.","json_payload":null,"error":null,"context":null,"cached":true}'
+      string: '{"id":117,"path":"test/sdk/test_delete_function_by_id","description":"Test
+        function","input_schema":null,"dataset_uuid":"7984e90d-798e-4b1a-b54b-4701878c96d2","out_schema":null,"instructions":"Do
+        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
     headers:
       content-length:
-      - '225'
+      - '382'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 19:30:30 GMT
+      - Mon, 08 Apr 2024 13:34:13 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -139,84 +130,80 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/50/cache
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_id
   response:
     body:
-      string: ''
+      string: '{"detail":"Function and associated generations deleted successfully"}'
     headers:
+      content-length:
+      - '69'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 19:30:30 GMT
+      - Mon, 08 Apr 2024 13:34:13 GMT
       server:
       - uvicorn
     status:
-      code: 204
-      message: No Content
+      code: 200
+      message: OK
 - request:
-    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
+    body: ''
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
-      content-length:
-      - '78'
-      content-type:
-      - application/json
       user-agent:
       - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async_flush
+    method: GET
+    uri: http://localhost:8000/api/v1/functions/117
   response:
     body:
-      string: '{"event_id":"508b2680-acdb-4fcf-880a-438f34f3455c","message":"Hello!
-        How can I assist you today? If you have any questions or need information,
-        feel free to ask.","json_payload":null,"error":null,"context":null,"cached":false}'
+      string: '{"detail":"Function not found"}'
     headers:
       content-length:
-      - '226'
+      - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 19:30:30 GMT
+      - Mon, 08 Apr 2024 13:34:13 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
-    method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_with_cache_async_flush
+    method: GET
+    uri: http://localhost:8000/api/v1/functions/117
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: '{"detail":"Function not found"}'
     headers:
       content-length:
-      - '69'
+      - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 19:30:34 GMT
+      - Mon, 08 Apr 2024 13:34:13 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 version: 1
```

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id[function0].yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -17,50 +17,51 @@
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:07 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_delete_function_by_id", "description":
       "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
-      something", "model": null, "index_ids": null, "use_semantic_search": null, "few_shot":
+      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
       null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '299'
+      - '297'
       content-type:
       - application/json
       user-agent:
       - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/api/v1/functions
   response:
     body:
-      string: '{"id":40}'
+      string: '{"id":56,"path":"test/sdk/test_delete_function_by_id","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"87e5ce5e-db28-4dc0-b860-045fd6ce9e7e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '9'
+      - '398'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -70,57 +71,27 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/40
+    uri: http://localhost:8000/api/v1/functions/56
   response:
     body:
-      string: '{"id":40,"path":"test/sdk/test_delete_function_by_id","description":"Test
-        function","input_schema":null,"dataset_uuid":"d00e9a7e-1666-499a-a61a-13221b858665","out_schema":null,"instructions":"Do
+      string: '{"id":56,"path":"test/sdk/test_delete_function_by_id","description":"Test
+        function","input_schema":null,"dataset_uuid":"87e5ce5e-db28-4dc0-b860-045fd6ce9e7e","out_schema":null,"instructions":"Do
         something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
     headers:
       content-length:
       - '381'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
-      server:
-      - uvicorn
-    status:
-      code: 200
-      message: OK
-- request:
-    body: ''
-    headers:
-      accept:
-      - '*/*'
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      user-agent:
-      - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/40
-  response:
-    body:
-      string: '{"id":40,"path":"test/sdk/test_delete_function_by_id","description":"Test
-        function","input_schema":null,"dataset_uuid":"d00e9a7e-1666-499a-a61a-13221b858665","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
-    headers:
-      content-length:
-      - '381'
-      content-type:
-      - application/json
-      date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -140,15 +111,15 @@
       string: '{"detail":"Function and associated generations deleted successfully"}'
     headers:
       content-length:
       - '69'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -158,24 +129,24 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/40
+    uri: http://localhost:8000/api/v1/functions/56
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:07 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 version: 1
```

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path[function0].yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -7,60 +7,61 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:23:54 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_delete_function_by_path", "description":
-      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
-      something", "model": null, "index_ids": null, "use_semantic_search": null, "few_shot":
-      null, "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_delete_function", "description": "Test
+      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
+      "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
+      "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '301'
+      - '291'
       content-type:
       - application/json
       user-agent:
       - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/api/v1/functions
   response:
     body:
-      string: '{"id":41}'
+      string: '{"id":47,"path":"test/sdk/test_delete_function","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"f3529aba-20a8-407b-9f68-b6eca214d9d6","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '9'
+      - '392'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:23:54 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -70,27 +71,27 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/41
+    uri: http://localhost:8000/api/v1/functions/47
   response:
     body:
-      string: '{"id":41,"path":"test/sdk/test_delete_function_by_path","description":"Test
-        function","input_schema":null,"dataset_uuid":"1d6a4d49-f0c8-4624-bb89-36ffb49ac201","out_schema":null,"instructions":"Do
+      string: '{"id":47,"path":"test/sdk/test_delete_function","description":"Test
+        function","input_schema":null,"dataset_uuid":"f3529aba-20a8-407b-9f68-b6eca214d9d6","out_schema":null,"instructions":"Do
         something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
     headers:
       content-length:
-      - '383'
+      - '375'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:23:54 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -100,25 +101,25 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function
   response:
     body:
       string: '{"detail":"Function and associated generations deleted successfully"}'
     headers:
       content-length:
       - '69'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:23:54 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -128,24 +129,24 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
+    uri: http://localhost:8000/api/v1/functions/47
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:23:54 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 version: 1
```

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_get[function0].yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -7,60 +7,61 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:07 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_get", "description": "Test function",
-      "input_schema": null, "out_schema": null, "instructions": "Do something", "model":
-      null, "index_ids": null, "use_semantic_search": null, "few_shot": null, "few_shot_count":
-      null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_delete_function_by_path", "description":
+      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
+      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
+      null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '281'
+      - '299'
       content-type:
       - application/json
       user-agent:
       - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/api/v1/functions
   response:
     body:
-      string: '{"id":38}'
+      string: '{"id":57,"path":"test/sdk/test_delete_function_by_path","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"3b2d8017-5f8a-40ec-8077-ce3ce9fcc3a7","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '9'
+      - '400'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -69,27 +70,26 @@
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/38
+    method: DELETE
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
   response:
     body:
-      string: '{"id":38,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"dataset_uuid":"7358b6c8-4536-4ba3-a26e-3acfa9db60af","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"detail":"Function and associated generations deleted successfully"}'
     headers:
       content-length:
-      - '363'
+      - '69'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -99,25 +99,24 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_delete_function_by_path
   response:
     body:
-      string: '{"id":38,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"dataset_uuid":"7358b6c8-4536-4ba3-a26e-3acfa9db60af","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"detail":"Function not found"}'
     headers:
       content-length:
-      - '363'
+      - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:07 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 version: 1
```

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id[function0].yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -7,60 +7,61 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get_by_id
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_async
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:23:54 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_get_by_id", "description": "Test function",
-      "input_schema": null, "out_schema": null, "instructions": "Do something", "model":
-      null, "index_ids": null, "use_semantic_search": null, "few_shot": null, "few_shot_count":
-      null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_create_function_async", "description":
+      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
+      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
+      null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '287'
+      - '297'
       content-type:
       - application/json
       user-agent:
       - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/api/v1/functions
   response:
     body:
-      string: '{"id":36}'
+      string: '{"id":42,"path":"test/sdk/test_create_function_async","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"8bb86025-9c91-4930-8f26-ac97cc7fb9a2","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '9'
+      - '398'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:23:54 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -70,25 +71,54 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/36
+    uri: http://localhost:8000/api/v1/functions/42
   response:
     body:
-      string: '{"id":36,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"dataset_uuid":"8b665798-95be-4977-82c5-e17d344067f3","out_schema":null,"instructions":"Do
+      string: '{"id":42,"path":"test/sdk/test_create_function_async","description":"Test
+        function","input_schema":null,"dataset_uuid":"8bb86025-9c91-4930-8f26-ac97cc7fb9a2","out_schema":null,"instructions":"Do
         something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
     headers:
       content-length:
-      - '369'
+      - '381'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:23:54 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      accept-encoding:
+      - gzip, deflate
+      connection:
+      - keep-alive
+      user-agent:
+      - python-httpx/0.27.0
+    method: DELETE
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_async
+  response:
+    body:
+      string: '{"detail":"Function and associated generations deleted successfully"}'
+    headers:
+      content-length:
+      - '69'
+      content-type:
+      - application/json
+      date:
+      - Thu, 11 Apr 2024 16:23:54 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path[function0].yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -7,60 +7,94 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get_by_path
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_async_chat
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:23:54 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_get_by_path", "description": "Test
-      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
-      "model": null, "index_ids": null, "use_semantic_search": null, "few_shot": null,
-      "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_async_chat", "description": "Translate
+      to French", "input_schema": null, "out_schema": null, "instructions": "Translate
+      to French", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
+      null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '289'
+      - '299'
       content-type:
       - application/json
       user-agent:
       - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/api/v1/functions
   response:
     body:
-      string: '{"id":37}'
+      string: '{"id":48,"path":"test/sdk/test_async_chat","description":"Translate
+        to French","input_schema":null,"out_schema":null,"instructions":"Translate
+        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"7223ad03-9f13-433d-a2c7-27052da2195d","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '9'
+      - '400'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:23:54 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
+    headers:
+      accept:
+      - '*/*'
+      accept-encoding:
+      - gzip, deflate
+      connection:
+      - keep-alive
+      content-length:
+      - '78'
+      content-type:
+      - application/json
+      user-agent:
+      - python-httpx/0.27.0
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_async_chat
+  response:
+    body:
+      string: '{"span_id":"84b5d901-47f0-4abd-8cf4-d5dc18800756","message":"Bonjour","json_payload":null,"error":null,"context":null,"cached":false}'
+    headers:
+      content-length:
+      - '133'
+      content-type:
+      - application/json
+      date:
+      - Thu, 11 Apr 2024 16:23:54 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -70,25 +104,54 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_get_by_path
+    uri: http://localhost:8000/api/v1/functions/48
+  response:
+    body:
+      string: '{"id":48,"path":"test/sdk/test_async_chat","description":"Translate
+        to French","input_schema":null,"dataset_uuid":"7223ad03-9f13-433d-a2c7-27052da2195d","out_schema":null,"instructions":"Translate
+        to French","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+    headers:
+      content-length:
+      - '383'
+      content-type:
+      - application/json
+      date:
+      - Thu, 11 Apr 2024 16:23:55 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      accept-encoding:
+      - gzip, deflate
+      connection:
+      - keep-alive
+      user-agent:
+      - python-httpx/0.27.0
+    method: DELETE
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_async_chat
   response:
     body:
-      string: '{"id":37,"path":"test/sdk/test_get_by_path","description":"Test function","input_schema":null,"dataset_uuid":"b72b4b20-b1e0-423e-9938-345d4a53397a","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"detail":"Function and associated generations deleted successfully"}'
     headers:
       content-length:
-      - '371'
+      - '69'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:23:55 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function[function0].yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -7,125 +7,130 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_update_function
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_with_cache
   response:
     body:
       string: '{"detail":"Function not found"}'
     headers:
       content-length:
       - '31'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:17 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_update_function", "description": "Test
-      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
-      "model": null, "index_ids": null, "use_semantic_search": null, "few_shot": null,
-      "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_create_function_with_cache", "description":
+      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
+      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
+      null, "few_shot_count": null, "cache_configuration": {"exact_match_cache_ttl":
+      10, "semantic_cache_threshold": null, "semantic_cache_ttl": null}}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '293'
+      - '389'
       content-type:
       - application/json
       user-agent:
       - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/api/v1/functions
   response:
     body:
-      string: '{"id":39}'
+      string: '{"id":60,"path":"test/sdk/test_create_function_with_cache","description":"Test
+        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"0492231a-3b8d-4fab-ad8e-19f8be5d8597","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '9'
+      - '403'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:17 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
+      content-length:
+      - '78'
+      content-type:
+      - application/json
       user-agent:
       - python-httpx/0.27.0
-    method: GET
-    uri: http://localhost:8000/api/v1/functions/39
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache
   response:
     body:
-      string: '{"id":39,"path":"test/sdk/test_update_function","description":"Test
-        function","input_schema":null,"dataset_uuid":"66f8c63e-483f-4751-a3c1-f1597ae4003d","out_schema":null,"instructions":"Do
-        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"span_id":"621f54fb-902c-4898-9cf2-c421b5129e26","message":"Hello!
+        How can I assist you today? If you have any questions or need information
+        on a particular topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '375'
+      - '247'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:17 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": 39, "path": "test/sdk/test_update_function", "description": "Test
-      function", "input_schema": null, "out_schema": null, "instructions": "Do something
-      else", "model": "azure/gpt4-eu", "index_ids": [], "use_semantic_search": false,
-      "few_shot": false, "few_shot_count": 2, "cache_configuration": null}'
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '304'
+      - '78'
       content-type:
       - application/json
       user-agent:
       - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions/39
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache
   response:
     body:
-      string: '{"id":39}'
+      string: '{"span_id":"b6d774b9-7cc6-4a01-8dd2-846d1fdd331a","message":"Hello!
+        How can I assist you today? If you have any questions or need information
+        on a particular topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":true}'
     headers:
       content-length:
-      - '9'
+      - '246'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -135,26 +140,54 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/39
+    uri: http://localhost:8000/api/v1/functions/60
+  response:
+    body:
+      string: '{"id":60,"path":"test/sdk/test_create_function_with_cache","description":"Test
+        function","input_schema":null,"dataset_uuid":"0492231a-3b8d-4fab-ad8e-19f8be5d8597","out_schema":null,"instructions":"Do
+        something","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":1,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+    headers:
+      content-length:
+      - '386'
+      content-type:
+      - application/json
+      date:
+      - Thu, 11 Apr 2024 16:26:21 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      accept-encoding:
+      - gzip, deflate
+      connection:
+      - keep-alive
+      user-agent:
+      - python-httpx/0.27.0
+    method: DELETE
+    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_with_cache
   response:
     body:
-      string: '{"id":39,"path":"test/sdk/test_update_function","description":"Test
-        function","input_schema":null,"dataset_uuid":"66f8c63e-483f-4751-a3c1-f1597ae4003d","out_schema":null,"instructions":"Do
-        something else","use_semantic_search":false,"few_shot":false,"few_shot_count":2,"revision":2,"org_id":1,"index_ids":[],"linked_functions_ids":[],"model":"azure/gpt4-eu","language_model_id":8}'
+      string: '{"detail":"Function and associated generations deleted successfully"}'
     headers:
       content-length:
-      - '380'
+      - '69'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:21 GMT
+      - Thu, 11 Apr 2024 16:26:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 interactions:
 - request:
-    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112", "project": "project",
+    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b", "project": "project",
       "name": "name", "input": "input", "start_time": "2021-01-01T00:00:00"}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
@@ -13,31 +13,31 @@
       - '141'
       user-agent:
       - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/spans
   response:
     body:
-      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
+      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Tue, 26 Mar 2024 14:57:14 GMT
+      - Thu, 11 Apr 2024 16:26:35 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12", "project": "project",
+    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c", "project": "project",
       "name": "name", "input": "input", "start_time": "2021-01-01T00:00:00", "parent_uuid":
-      "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
+      "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b"}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
@@ -45,84 +45,84 @@
       - '196'
       user-agent:
       - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/spans
   response:
     body:
-      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12"}'
+      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Tue, 26 Mar 2024 14:57:14 GMT
+      - Thu, 11 Apr 2024 16:26:35 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12", "output": "output", "end_time":
+    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c", "output": "output", "end_time":
       "2021-12-01T00:00:00"}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
       - '103'
       user-agent:
       - python-httpx/0.27.0
     method: PUT
-    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12
+    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c
   response:
     body:
-      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12"}'
+      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Tue, 26 Mar 2024 14:57:14 GMT
+      - Thu, 11 Apr 2024 16:26:35 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112", "output": "output", "end_time":
+    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b", "output": "output", "end_time":
       "2022-01-01T00:00:00"}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
       - '103'
       user-agent:
       - python-httpx/0.27.0
     method: PUT
-    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112
+    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b
   response:
     body:
-      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
+      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Tue, 26 Mar 2024 14:57:14 GMT
+      - Thu, 11 Apr 2024 16:26:35 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -132,23 +132,23 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12
+    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Tue, 26 Mar 2024 14:57:14 GMT
+      - Thu, 11 Apr 2024 16:26:35 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 - request:
     body: ''
@@ -158,22 +158,22 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112
+    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Tue, 26 Mar 2024 14:57:14 GMT
+      - Thu, 11 Apr 2024 16:26:35 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -7,129 +7,176 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: GET
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_with_cache_sync
+    uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '[]'
     headers:
       content-length:
-      - '31'
+      - '2'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:34 GMT
+      - Thu, 11 Apr 2024 16:26:34 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 200
+      message: OK
 - request:
-    body: '{"id": null, "path": "test/sdk/test_create_function_with_cache_sync", "description":
-      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
-      something", "model": null, "index_ids": null, "use_semantic_search": null, "few_shot":
-      null, "few_shot_count": null, "cache_configuration": {"exact_match_cache_ttl":
-      10, "semantic_cache_threshold": null, "semantic_cache_ttl": null}}'
+    body: '{"name": "test_list_indexes"}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '396'
+      - '29'
       content-type:
       - application/json
       user-agent:
       - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/api/v1/functions
+    uri: http://localhost:8000/v1/indexes
+  response:
+    body:
+      string: '{"id":263,"name":"test_list_indexes","files":[],"created_at":"2024-04-11T16:26:34.358515Z"}'
+    headers:
+      content-length:
+      - '91'
+      content-type:
+      - application/json
+      date:
+      - Thu, 11 Apr 2024 16:26:34 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      accept-encoding:
+      - gzip, deflate
+      connection:
+      - keep-alive
+      user-agent:
+      - python-httpx/0.27.0
+    method: GET
+    uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":45}'
+      string: '[{"id":263,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
+        Lundell","created_at":"2024-04-11T16:26:34.358515Z","updated_at":"2024-04-11T16:26:34.358515Z","count":0}]'
     headers:
       content-length:
-      - '9'
+      - '193'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:34 GMT
+      - Thu, 11 Apr 2024 16:26:34 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
+    body: '{"name": "test_list_indexes_2"}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '78'
+      - '31'
       content-type:
       - application/json
       user-agent:
       - python-httpx/0.27.0
     method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_sync
+    uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"event_id":"517d59e6-067e-4b08-aef9-72d2de0508e3","message":"Hello!
-        How can I assist you today? If you have any questions or need information
-        on a topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":false}'
+      string: '{"id":264,"name":"test_list_indexes_2","files":[],"created_at":"2024-04-11T16:26:34.376310Z"}'
     headers:
       content-length:
-      - '237'
+      - '93'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:34 GMT
+      - Thu, 11 Apr 2024 16:26:34 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
+    body: ''
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
+      user-agent:
+      - python-httpx/0.27.0
+    method: GET
+    uri: http://localhost:8000/v1/indexes
+  response:
+    body:
+      string: '[{"id":263,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
+        Lundell","created_at":"2024-04-11T16:26:34.358515Z","updated_at":"2024-04-11T16:26:34.358515Z","count":0},{"id":264,"org_id":1,"org_name":null,"name":"test_list_indexes_2","created_by":"Mattias
+        Lundell","created_at":"2024-04-11T16:26:34.376310Z","updated_at":"2024-04-11T16:26:34.376310Z","count":0}]'
+    headers:
       content-length:
-      - '78'
+      - '387'
       content-type:
       - application/json
+      date:
+      - Thu, 11 Apr 2024 16:26:34 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      accept-encoding:
+      - gzip, deflate
+      connection:
+      - keep-alive
       user-agent:
       - python-httpx/0.27.0
-    method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_sync
+    method: DELETE
+    uri: http://localhost:8000/v1/indexes/264
   response:
     body:
-      string: '{"event_id":"4762ff4b-e5ba-4819-a893-2d0eecd23bec","message":"Hello!
-        How can I assist you today? If you have any questions or need information
-        on a topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":true}'
+      string: 'true'
     headers:
       content-length:
-      - '236'
+      - '4'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:37 GMT
+      - Thu, 11 Apr 2024 16:26:34 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -139,24 +186,24 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/api/v1/functions/by_path/test/sdk/test_create_function_with_cache_sync
+    uri: http://localhost:8000/v1/indexes/263
   response:
     body:
-      string: '{"detail":"Function and associated generations deleted successfully"}'
+      string: 'true'
     headers:
       content-length:
-      - '69'
+      - '4'
       content-type:
       - application/json
       date:
-      - Wed, 27 Mar 2024 11:05:37 GMT
+      - Thu, 11 Apr 2024 16:26:34 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.2.6/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml` & `opperai-0.3.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 interactions:
 - request:
-    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b", "project": "project",
+    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112", "project": "project",
       "name": "name", "input": "input", "start_time": "2021-01-01T00:00:00"}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
@@ -13,31 +13,31 @@
       - '141'
       user-agent:
       - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/spans
   response:
     body:
-      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b"}'
+      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Tue, 26 Mar 2024 13:51:40 GMT
+      - Thu, 11 Apr 2024 16:26:06 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c", "project": "project",
+    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12", "project": "project",
       "name": "name", "input": "input", "start_time": "2021-01-01T00:00:00", "parent_uuid":
-      "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b"}'
+      "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
@@ -45,84 +45,84 @@
       - '196'
       user-agent:
       - python-httpx/0.27.0
     method: POST
     uri: http://localhost:8000/v1/spans
   response:
     body:
-      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c"}'
+      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Tue, 26 Mar 2024 13:51:40 GMT
+      - Thu, 11 Apr 2024 16:26:06 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c", "output": "output", "end_time":
+    body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12", "output": "output", "end_time":
       "2021-12-01T00:00:00"}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
       - '103'
       user-agent:
       - python-httpx/0.27.0
     method: PUT
-    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c
+    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12
   response:
     body:
-      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c"}'
+      string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Tue, 26 Mar 2024 13:51:40 GMT
+      - Thu, 11 Apr 2024 16:26:06 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b", "output": "output", "end_time":
+    body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112", "output": "output", "end_time":
       "2022-01-01T00:00:00"}'
     headers:
       accept:
       - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
       - '103'
       user-agent:
       - python-httpx/0.27.0
     method: PUT
-    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b
+    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112
   response:
     body:
-      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b"}'
+      string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Tue, 26 Mar 2024 13:51:40 GMT
+      - Thu, 11 Apr 2024 16:26:06 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -132,23 +132,23 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c3c4c3c
+    uri: http://localhost:8000/v1/spans/cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Tue, 26 Mar 2024 13:51:40 GMT
+      - Thu, 11 Apr 2024 16:26:06 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 - request:
     body: ''
@@ -158,22 +158,22 @@
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       user-agent:
       - python-httpx/0.27.0
     method: DELETE
-    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4b3b
+    uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Tue, 26 Mar 2024 13:51:40 GMT
+      - Thu, 11 Apr 2024 16:26:06 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.2.6/README.md` & `opperai-0.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -19,34 +19,97 @@
 print(translate("Hello","fr"))
 
 >>> "Bonjour"
 ```
 
 The `fn` decorator automatically creates an Opper function ready to be called like any other function in your code. They're no different than any other function!
 
-## Calling functions manually
+## Calling functions
 
 To call a function you created at [https://platform.opper.ai](https://platform.opper.ai) you can use the following code:
 
 
 ```python
 from opperai import Client
 from opperai.types import ChatPayload, Message
 
-# Use AsyncClient for async operations
 client = Client(api_key="your-api-key") 
 response = client.functions.chat("your-function-path", 
- ChatPayload(messages=[Message(role="user", content="hello")])
+  ChatPayload(messages=[Message(role="user", content="hello")])
 )
 
 print(response)
+```
+
+## Async function calling
+
+```python
+import asyncio
+from opperai import AsyncClient
+from opperai.types import ChatPayload, Message
+
+opper = AsyncClient(api_key="your-api-key")
+
+async def main():
+    message = ""
+    async for response in await opper.functions.chat(
+        "your-function-path",
+        ChatPayload(messages=[Message(role="user", content="Hello, world!")]),
+        stream=True,
+    ):
+        if response.delta is not None:
+            message += response.delta
+
+    print(message)
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+## Streaming responses
+
+```python
+from opperai import Client
+from opperai.types import ChatPayload, Message
 
+client = Client(api_key="op-xxxx")
+response = client.functions.chat(
+    "joch/test",
+    ChatPayload(
+        messages=[Message(role="user", content="tell me a story.")],
+    ),
+    stream=True,
+)
+for data in response:
+    print(data.delta, end="", flush=True)
 ```
 
-This more traditional API is better targeted for chat use cases.
+## Async streaming responses
+
+```python
+import asyncio
+from opperai import AsyncClient
+from opperai.types import ChatPayload, Message
+
+client = AsyncClient(api_key="your-api-key")
+
+async def main():
+    async for response in await client.functions.chat(
+        "your-function-path",
+        ChatPayload(
+            messages=[Message(role="user", content="tell me a story.")],
+        ),
+        stream=True,
+    ):
+        print(response.delta, end="", flush=True)
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
 
 ## Retrieval
 
 ```python
 client.indexes.retrieve(index_id=42, "Who is the president of the USA?", 3)
 
 ```
```

### Comparing `opperai-0.2.6/pyproject.toml` & `opperai-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "opperai"
-version = "0.2.6"
+version = "0.3.0"
 description = "Opper Python client"
 authors = [
   {name = "Opper", email = "opper@opper.ai"},
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `opperai-0.2.6/PKG-INFO` & `opperai-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.3
 Name: opperai
-Version: 0.2.6
+Version: 0.3.0
 Summary: Opper Python client
 Project-URL: Homepage, https://opper.ai
 Project-URL: Documentation, https://docs.opper.ai
 Project-URL: Platform, https://platform.opper.ai
 Author-email: Opper <opper@opper.ai>
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: httpx
 Requires-Dist: httpx-sse
 Requires-Dist: pydantic
 Provides-Extra: test
@@ -40,34 +41,97 @@
 print(translate("Hello","fr"))
 
 >>> "Bonjour"
 ```
 
 The `fn` decorator automatically creates an Opper function ready to be called like any other function in your code. They're no different than any other function!
 
-## Calling functions manually
+## Calling functions
 
 To call a function you created at [https://platform.opper.ai](https://platform.opper.ai) you can use the following code:
 
 
 ```python
 from opperai import Client
 from opperai.types import ChatPayload, Message
 
-# Use AsyncClient for async operations
 client = Client(api_key="your-api-key") 
 response = client.functions.chat("your-function-path", 
- ChatPayload(messages=[Message(role="user", content="hello")])
+  ChatPayload(messages=[Message(role="user", content="hello")])
 )
 
 print(response)
+```
+
+## Async function calling
+
+```python
+import asyncio
+from opperai import AsyncClient
+from opperai.types import ChatPayload, Message
+
+opper = AsyncClient(api_key="your-api-key")
+
+async def main():
+    message = ""
+    async for response in await opper.functions.chat(
+        "your-function-path",
+        ChatPayload(messages=[Message(role="user", content="Hello, world!")]),
+        stream=True,
+    ):
+        if response.delta is not None:
+            message += response.delta
+
+    print(message)
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+## Streaming responses
+
+```python
+from opperai import Client
+from opperai.types import ChatPayload, Message
 
+client = Client(api_key="op-xxxx")
+response = client.functions.chat(
+    "joch/test",
+    ChatPayload(
+        messages=[Message(role="user", content="tell me a story.")],
+    ),
+    stream=True,
+)
+for data in response:
+    print(data.delta, end="", flush=True)
 ```
 
-This more traditional API is better targeted for chat use cases.
+## Async streaming responses
+
+```python
+import asyncio
+from opperai import AsyncClient
+from opperai.types import ChatPayload, Message
+
+client = AsyncClient(api_key="your-api-key")
+
+async def main():
+    async for response in await client.functions.chat(
+        "your-function-path",
+        ChatPayload(
+            messages=[Message(role="user", content="tell me a story.")],
+        ),
+        stream=True,
+    ):
+        print(response.delta, end="", flush=True)
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
 
 ## Retrieval
 
 ```python
 client.indexes.retrieve(index_id=42, "Who is the president of the USA?", 3)
 
 ```
```

