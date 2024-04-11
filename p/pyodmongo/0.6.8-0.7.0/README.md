# Comparing `tmp/pyodmongo-0.6.8.tar.gz` & `tmp/pyodmongo-0.7.0.tar.gz`

## Comparing `pyodmongo-0.6.8.tar` & `pyodmongo-0.7.0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/code_of_conduct.md
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/coverage.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/mkdocs.yml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyproject.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/requirements.txt
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.github/workflows/black_formatter.yml
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.github/workflows/publishing_docs_s3.yml
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.github/workflows/python_publish.yml
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.github/workflows/tests.yml
--rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    36227 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/assets/images/insomnia_request.png
--rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/assets/images/logo.png
--rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/assets/images/pyodmongo_Logo_BG_Dark.png
--rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/assets/images/pyodmongo_Logo_BG_White.png
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/aggregation.md
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/contributing.md
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/db_model.md
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/delete.md
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/fastapi.md
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/find.md
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/getting_started.md
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/index.md
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/indexes.md
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/query.md
--rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/save.md
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/aggregation.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/contributing.md
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/db_model.md
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/delete.md
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/fastapi.md
--rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/find.md
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/getting_started.md
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/index.md
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/indexes.md
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/query.md
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/save.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/stylesheets/extras.css
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/version.py
--rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/async_engine/engine.py
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/engine/engine.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/engine/utils.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/db_field_info.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/db_model.py
--rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/fields.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/id_model.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/paginate.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/query_operators.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/responses.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/queries/__init__.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/queries/comparison_operators.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/queries/logical_operators.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/queries/query_string.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/services/aggregate_stages.py
--rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/services/model_init.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/services/query_operators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/conftest.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_async_aggregate.py
--rw-r--r--   0        0        0    16778 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_async_crud_db.py
--rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_class.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_db_field_info.py
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_db_index.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_dict_empty.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_fastapi.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_model_init_functions.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_object_id.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_project_pipeline.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_pydantic_validators.py
--rw-r--r--   0        0        0     8675 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_queries.py
--rw-r--r--   0        0        0     9250 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_reference_pipeline.py
--rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_save_dict.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_sync_aggregate.py
--rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_sync_crud_db.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_version.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/LICENSE
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/code_of_conduct.md
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/coverage.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/mkdocs.yml
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyproject.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/requirements.txt
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.github/workflows/black_formatter.yml
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.github/workflows/publishing_docs_s3.yml
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.github/workflows/python_publish.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    94192 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/assets/images/insomnia_request.png
+-rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/assets/images/logo.png
+-rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/assets/images/pyodmongo_Logo_BG_Dark.png
+-rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/assets/images/pyodmongo_Logo_BG_White.png
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/aggregation.md
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/contributing.md
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/db_model.md
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/delete.md
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/fastapi.md
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/find.md
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/getting_started.md
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/index.md
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/indexes.md
+-rw-r--r--   0        0        0     7727 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/query.md
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/save.md
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/aggregation.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/contributing.md
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/db_model.md
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/delete.md
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/fastapi.md
+-rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/find.md
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/getting_started.md
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/index.md
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/indexes.md
+-rw-r--r--   0        0        0     7888 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/query.md
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/save.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/stylesheets/extras.css
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/version.py
+-rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/async_engine/engine.py
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/engine/engine.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/engine/utils.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/db_field_info.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/db_model.py
+-rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/fields.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/id_model.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/paginate.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/query_operators.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/responses.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/queries/__init__.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/queries/comparison_operators.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/queries/logical_operators.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/queries/query_string.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/queries/sort_operator.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/services/aggregate_stages.py
+-rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/services/model_init.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/services/query_operators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_async_aggregate.py
+-rw-r--r--   0        0        0    18182 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_async_crud_db.py
+-rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_class.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_db_field_info.py
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_db_index.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_dict_empty.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_fastapi.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_model_init_functions.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_object_id.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_project_pipeline.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_pydantic_validators.py
+-rw-r--r--   0        0        0     9990 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_queries.py
+-rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_reference_pipeline.py
+-rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_save_dict.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_sync_aggregate.py
+-rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_sync_crud_db.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_version.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/PKG-INFO
```

### Comparing `pyodmongo-0.6.8/code_of_conduct.md` & `pyodmongo-0.7.0/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/mkdocs.yml` & `pyodmongo-0.7.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/pyproject.py` & `pyodmongo-0.7.0/pyproject.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/requirements.txt` & `pyodmongo-0.7.0/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 isort==5.12.0
 Jinja2==3.1.2
 lazy-object-proxy==1.9.0
 Markdown==3.4.4
 MarkupSafe==2.1.3
 mccabe==0.7.0
 mergedeep==1.3.4
-mkdocs==1.5.2
-mkdocs-material==9.2.8
-mkdocs-material-extensions==1.1.1
+mkdocs==1.5.3
+mkdocs-material==9.5.17
+mkdocs-material-extensions==1.3.1
 mkdocs-static-i18n==1.0.3
 motor==3.3.2
 mypy-extensions==1.0.0
 packaging==23.1
 paginate==0.5.6
 pathspec==0.11.2
 Pillow==10.0.1
```

### Comparing `pyodmongo-0.6.8/.github/ISSUE_TEMPLATE/bug.yml` & `pyodmongo-0.7.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/.github/workflows/black_formatter.yml` & `pyodmongo-0.7.0/.github/workflows/black_formatter.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/.github/workflows/publishing_docs_s3.yml` & `pyodmongo-0.7.0/.github/workflows/publishing_docs_s3.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/.github/workflows/python_publish.yml` & `pyodmongo-0.7.0/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/.github/workflows/tests.yml` & `pyodmongo-0.7.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/assets/images/favicon.png` & `pyodmongo-0.7.0/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/assets/images/logo.png` & `pyodmongo-0.7.0/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/assets/images/pyodmongo_Logo_BG_Dark.png` & `pyodmongo-0.7.0/docs/assets/images/pyodmongo_Logo_BG_Dark.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/assets/images/pyodmongo_Logo_BG_White.png` & `pyodmongo-0.7.0/docs/assets/images/pyodmongo_Logo_BG_White.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/en/aggregation.md` & `pyodmongo-0.7.0/docs/en/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/en/contributing.md` & `pyodmongo-0.7.0/docs/en/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/en/db_model.md` & `pyodmongo-0.7.0/docs/en/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/en/delete.md` & `pyodmongo-0.7.0/docs/en/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/en/fastapi.md` & `pyodmongo-0.7.0/docs/en/fastapi.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,20 @@
     attr2: str
     attr3: int
     _collection: ClassVar = "my_model"
 
 
 @app.get("/", response_model=list[MyModel])
 async def get_route(request: Request):
-    query = mount_query_filter(
+    query, sort = mount_query_filter(
         Model=MyModel,
         items=request.query_params._dict,
         initial_comparison_operators=[],
     )
-    return await engine.find_many(Model=MyModel, query=query)
+    return await engine.find_many(Model=MyModel, query=query, sort=sort)
 ```
 
 In the example above, we defined a FastAPI route `GET /` that accepts query parameters. The `mount_query_filter` function, designed for use with FastAPI `Request`, dynamically constructs a query based on the items in these parameters.
 
 ## The `mount_query_filter` Function
 
 The `mount_query_filter` function adapts perfectly to FastAPI. It dynamically builds a query based on the passed dictionary items, making it compatible with the `request.query_params._dict` attribute, which contains the route's query strings.
@@ -43,20 +43,21 @@
 
 The function returns a query with the `and` operator applied between all items in the passed dictionary.
 
 ## Example Usage
 
 ![Image title](./assets/images/insomnia_request.png)
 
-When you trigger the following route with query strings: `http://localhost:8000/?attr1_eq=value_1&attr2_in=%5B'value_2',%20'value_3'%5D&attr3_gte=10`, the `request.query_params._dict` will contain the following dictionary:
+When you trigger the following route with query strings: `http://localhost:8000/?attr1_eq=value_1&attr2_in=%5B'value_2',%20'value_3'%5D&attr3_gte=10&_sort=%5B%5B'attr1',%201%5D,%20%5B'attr2',%20-1%5D%5D`, the `request.query_params._dict` will contain the following dictionary:
 
 ```python
 {
     "attr1_eq": "value_1", 
     "attr2_in": "['value_2', 'value_3']", 
-    "attr3_gte": 10
+    "attr3_gte": 10,
+    "_sort": "[['attr1', 1], ['attr2', -1]]",
 }
 ```
 
 In this dictionary, keys must be attribute names followed by an underscore and a valid operator (e.g. 'attr1' + '_' + 'eq'). Valid operators are: `"eq", "gt", "gte", "in", "lt", "lte", "ne", "nin"`.
 
 By using the `mount_query_filter` function in combination with FastAPI's `Request`, you can enable powerful and dynamic query capabilities in your applications.
```

### Comparing `pyodmongo-0.6.8/docs/en/find.md` & `pyodmongo-0.7.0/docs/en/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/en/getting_started.md` & `pyodmongo-0.7.0/docs/en/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/en/index.md` & `pyodmongo-0.7.0/docs/en/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/en/indexes.md` & `pyodmongo-0.7.0/docs/en/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/en/save.md` & `pyodmongo-0.7.0/docs/en/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/pt-BR/aggregation.md` & `pyodmongo-0.7.0/docs/pt-BR/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/pt-BR/contributing.md` & `pyodmongo-0.7.0/docs/pt-BR/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/pt-BR/db_model.md` & `pyodmongo-0.7.0/docs/pt-BR/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/pt-BR/delete.md` & `pyodmongo-0.7.0/docs/pt-BR/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/pt-BR/fastapi.md` & `pyodmongo-0.7.0/docs/pt-BR/fastapi.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,20 @@
     attr2: str
     attr3: int
     _collection: ClassVar = "my_model"
 
 
 @app.get("/", response_model=list[MyModel])
 async def get_route(request: Request):
-    query = mount_query_filter(
+    query, sort = mount_query_filter(
         Model=MyModel,
         items=request.query_params._dict,
         initial_comparison_operators=[],
     )
-    return await engine.find_many(Model=MyModel, query=query)
+    return await engine.find_many(Model=MyModel, query=query, sort=sort)
 ```
 
 No exemplo acima, definimos uma rota FastAPI `GET /` que aceita parâmetros de consulta. A função `mount_query_filter`, projetada para uso com `Request` do FastAPI, constrói dinamicamente uma consulta com base nos itens desses parâmetros.
 
 ## A Função `mount_query_filter`
 
 A função `mount_query_filter` se adapta perfeitamente com o FastAPI. Ela constrói dinamicamente uma consulta com base nos itens do dicionário passado, tornando-a compatível com o atributo `request.query_params._dict`, que contém as query strings da rota.
@@ -43,20 +43,22 @@
 
 A função retorna uma consulta com o operador `and` aplicado entre todos os itens do dicionário passado.
 
 ## Exemplo de uso
 
 ![Image title](./assets/images/insomnia_request.png)
 
-Quando você aciona a seguinte rota com query strings: `http://localhost:8000/?attr1_eq=value_1&attr2_in=%5B'value_2',%20'value_3'%5D&attr3_gte=10`, o `request.query_params._dict` irá conter o seguinte dicionário:
+Quando você aciona a seguinte rota com query strings: `http://localhost:8000/?attr1_eq=value_1&attr2_in=%5B'value_2',%20'value_3'%5D&attr3_gte=10&_sort=%5B%5B'attr1',%201%5D,%20%5B'attr2',%20-1%5D%5D`, o `request.query_params._dict` irá conter o seguinte dicionário:
 
 ```python
 {
     "attr1_eq": "value_1", 
     "attr2_in": "['value_2', 'value_3']", 
-    "attr3_gte": 10
+    "attr3_gte": 10,
+    "_sort": "[['attr1', 1], ['attr2', -1]]",
 }
 ```
+```
 
 Neste dicionário, as chaves devem ser nomes de atributos seguidos por um sublinhado e um operador válido (por exemplo, 'attr1' + '_' + 'eq'). Os operadores válidos são: `"eq", "gt", "gte", "in", "lt", "lte", "ne", "nin"`.
 
 Ao utilizar a função `mount_query_filter` em combinação com `Request` do FastAPI, você pode habilitar recursos de consulta poderosos e dinâmicos em suas aplicações.
```

### Comparing `pyodmongo-0.6.8/docs/pt-BR/find.md` & `pyodmongo-0.7.0/docs/pt-BR/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/pt-BR/getting_started.md` & `pyodmongo-0.7.0/docs/pt-BR/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/pt-BR/index.md` & `pyodmongo-0.7.0/docs/pt-BR/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/pt-BR/indexes.md` & `pyodmongo-0.7.0/docs/pt-BR/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/docs/pt-BR/query.md` & `pyodmongo-0.7.0/docs/pt-BR/query.md`

 * *Files 22% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
 async def main():
     query = gte(Product.price, 5)
-    result: Product = await engine.find_one(Model=Product, query=query)
+    sort_oprator = sort((Product.name, 1), (Product.price, -1))
+    result: Product = await engine.find_one(Model=Product, query=query, sort=sort_oprator)
 
 asyncio.run(main())
 ```
 ///
 /// tab | Sync
 ```python hl_lines="16"
 from pyodmongo import DbEngine, DbModel
@@ -65,15 +66,16 @@
     name: str
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
 query = gte(Product.price, 5)
-result: Product = engine.find_one(Model=Product, query=query)
+sort_oprator = sort((Product.name, 1), (Product.price, -1))
+result: Product = engine.find_one(Model=Product, query=query, sort=sort_oprator)
 ```
 ///
 
 Neste exemplo, a consulta retornará todos os documentos da collection 'products' onde o campo price for igual ou superior a 5.
 
 ## Operadores lógicos
 
@@ -109,15 +111,16 @@
 
 
 async def main():
     query = and_(
         eq(Product.is_available, True),
         gte(Product.price, 5)
     )
-    result: Product = await engine.find_one(Model=Product, query=query)
+    sort_oprator = sort((Product.name, 1), (Product.price, -1))
+    result: Product = await engine.find_one(Model=Product, query=query, sort=sort_oprator)
 
 asyncio.run(main())
 ```
 ///
 /// tab | Sync
 ```python hl_lines="17"
 from pyodmongo import DbEngine, DbModel
@@ -136,16 +139,70 @@
     _collection: ClassVar = 'products'
 
 
 query = and_(
     eq(Product.is_available, True),
     gte(Product.price, 5)
 )
-result: Product = engine.find_one(Model=Product, query=query)
+sort_oprator = sort((Product.name, 1), (Product.price, -1))
+result: Product = engine.find_one(Model=Product, query=query, sort=sort_oprator)
 
 ```
 ///
 
 Neste exemplo a consulta retornará todos os documentos da collecion 'products' que `is_available` seja `True` e que tenham `price` maior ou igual a 5
 
 !!! tip
-    As entradas para estes Operadores Lógicos podem ser Operadores de Comparação ou mesmo outros Operadores Lógicos. Essa flexibilidade permite criar consultas complexas e aninhadas, permitindo expressar condições complexas de recuperação de dados com precisão.
+    As entradas para estes Operadores Lógicos podem ser Operadores de Comparação ou mesmo outros Operadores Lógicos. Essa flexibilidade permite criar consultas complexas e aninhadas, permitindo expressar condições complexas de recuperação de dados com precisão.
+
+    ## Sort
+
+/// tab | Async
+```python hl_lines="19"
+from pyodmongo import AsyncDbEngine, DbModel
+from pyodmongo.queries import ( eq, gt, gte, in_, lt, lte, ne, nin, text, 
+                                and_, or_, nor)
+from typing import ClassVar
+import asyncio
+
+engine = AsyncDbEngine(mongo_uri='mongodb://localhost:27017', db_name='my_db')
+
+
+class Product(DbModel):
+    name: str
+    price: float
+    is_available: bool
+    _collection: ClassVar = 'products'
+
+
+async def main():
+    query = gte(Product.price, 5)
+    sort_oprator = sort((Product.name, 1), (Product.price, -1))
+    result: Product = await engine.find_one(Model=Product, query=query, sort=sort_oprator)
+
+asyncio.run(main())
+```
+///
+/// tab | Sync
+```python hl_lines="17"
+from pyodmongo import DbEngine, DbModel
+from pyodmongo.queries import ( eq, gt, gte, in_, lt, lte, ne, nin, text, 
+                                and_, or_, nor)
+from typing import ClassVar
+
+engine = DbEngine(mongo_uri='mongodb://localhost:27017', db_name='my_db')
+
+
+class Product(DbModel):
+    name: str
+    price: float
+    is_available: bool
+    _collection: ClassVar = 'products'
+
+
+query = gte(Product.price, 5)
+sort_oprator = sort((Product.name, 1), (Product.price, -1))
+result: Product = engine.find_one(Model=Product, query=query, sort=sort_oprator)
+```
+///
+
+No exemplo fornecido, o `sort_operator` é definido usando a função `sort`, que aceita tuplas. Cada tupla contém dois elementos: o primeiro é o campo pelo qual você deseja ordenar e o segundo é a direção da ordenação, onde 1 indica ordem ascendente e -1 indica ordem descendente. No caso apresentado, o `sort_operator` ordena os resultados primeiro pelo campo name em ordem ascendente e, em seguida, pelo campo price em ordem descendente. Assim, os produtos são retornados em ordem alfabética pelo nome e, em caso de empate, em ordem decrescente pelo preço.
```

### Comparing `pyodmongo-0.6.8/docs/pt-BR/save.md` & `pyodmongo-0.7.0/docs/pt-BR/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/pyodmongo/async_engine/engine.py` & `pyodmongo-0.7.0/pyodmongo/async_engine/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from motor.motor_asyncio import AsyncIOMotorClient
 from pymongo.results import UpdateResult, DeleteResult
 from ..models.responses import SaveResponse, DeleteResponse
 from ..engine.utils import consolidate_dict, mount_base_pipeline
-from ..services.query_operators import query_dict
+from ..services.query_operators import query_dict, sort_dict
 from ..models.paginate import ResponsePaginate
-from ..models.query_operators import LogicalOperator, ComparisonOperator
+from ..models.query_operators import LogicalOperator, ComparisonOperator, SortOperator
 from ..models.db_model import DbModel
 from datetime import datetime
 from typing import TypeVar
 from bson import ObjectId
 from math import ceil
 from asyncio import gather
 
@@ -145,27 +145,37 @@
         return await gather(*save_calls)
 
     async def find_one(
         self,
         Model: type[Model],
         query: ComparisonOperator | LogicalOperator = None,
         raw_query: dict = None,
+        sort: SortOperator = None,
+        raw_sort: dict = None,
         populate: bool = False,
         as_dict: bool = False,
     ) -> type[Model]:
         if query and (
             type(query) != ComparisonOperator and type(query) != LogicalOperator
         ):
             raise TypeError(
                 'query argument must be a ComparisonOperator or LogicalOperator from pyodmongo.queries. If you really need to make a very specific query, use "raw_query" argument'
             )
+        if sort and (type(sort) != SortOperator):
+            raise TypeError(
+                'sort argument must be a SortOperator from pyodmongo.queries. If you really need to make a very specific sort, use "raw_sort" argument'
+            )
         raw_query = {} if not raw_query else raw_query
+        query = query_dict(query_operator=query, dct={}) if query else raw_query
+        raw_sort = {} if not raw_sort else raw_sort
+        sort = sort_dict(sort_operators=sort) if sort else raw_sort
         pipeline = mount_base_pipeline(
             Model=Model,
-            query=query_dict(query_operator=query, dct={}) if query else raw_query,
+            query=query,
+            sort=sort,
             populate=populate,
         )
         pipeline += [{"$limit": 1}]
         try:
             result = await self.__aggregate(
                 Model=Model, pipeline=pipeline, as_dict=as_dict
             )
@@ -174,31 +184,40 @@
             return None
 
     async def find_many(
         self,
         Model: type[Model],
         query: ComparisonOperator | LogicalOperator = None,
         raw_query: dict = None,
+        sort: SortOperator = None,
+        raw_sort: dict = None,
         populate: bool = False,
         as_dict: bool = False,
         paginate: bool = False,
         current_page: int = 1,
         docs_per_page: int = 1000,
     ):
         if query and (
             type(query) != ComparisonOperator and type(query) != LogicalOperator
         ):
             raise TypeError(
                 'query argument must be a ComparisonOperator or LogicalOperator from pyodmongo.queries. If you really need to make a very specific query, use "raw_query" argument'
             )
+        if sort and (type(sort) != SortOperator):
+            raise TypeError(
+                'sort argument must be a SortOperator from pyodmongo.queries. If you really need to make a very specific sort, use "raw_sort" argument'
+            )
         raw_query = {} if not raw_query else raw_query
         query = query_dict(query_operator=query, dct={}) if query else raw_query
+        raw_sort = {} if not raw_sort else raw_sort
+        sort = sort_dict(sort_operators=sort) if sort else raw_sort
         pipeline = mount_base_pipeline(
             Model=Model,
             query=query,
+            sort=sort,
             populate=populate,
         )
         if not paginate:
             return await self.__aggregate(
                 Model=Model, pipeline=pipeline, as_dict=as_dict
             )
         max_docs_per_page = 1000
```

### Comparing `pyodmongo-0.6.8/pyodmongo/engine/engine.py` & `pyodmongo-0.7.0/pyodmongo/engine/engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pymongo import MongoClient
 from pymongo.results import UpdateResult, DeleteResult
 from ..models.responses import SaveResponse, DeleteResponse
 from ..engine.utils import consolidate_dict, mount_base_pipeline
-from ..services.query_operators import query_dict
+from ..services.query_operators import query_dict, sort_dict
 from ..models.paginate import ResponsePaginate
-from ..models.query_operators import LogicalOperator, ComparisonOperator
+from ..models.query_operators import LogicalOperator, ComparisonOperator, SortOperator
 from ..models.db_model import DbModel
 from datetime import datetime
 from typing import TypeVar
 from bson import ObjectId
 from math import ceil
 
 
@@ -144,58 +144,77 @@
         return result
 
     def find_one(
         self,
         Model: type[Model],
         query: ComparisonOperator | LogicalOperator = None,
         raw_query: dict = None,
+        sort: SortOperator = None,
+        raw_sort: dict = None,
         populate: bool = False,
         as_dict: bool = False,
     ) -> type[Model]:
         if query and (
             type(query) != ComparisonOperator and type(query) != LogicalOperator
         ):
             raise TypeError(
                 'query argument must be a ComparisonOperator or LogicalOperator from pyodmongo.queries. If you really need to make a very specific query, use "raw_query" argument'
             )
+        if sort and (type(sort) != SortOperator):
+            raise TypeError(
+                'sort argument must be a SortOperator from pyodmongo.queries. If you really need to make a very specific sort, use "raw_sort" argument'
+            )
         raw_query = {} if not raw_query else raw_query
+        query = query_dict(query_operator=query, dct={}) if query else raw_query
+        raw_sort = {} if not raw_sort else raw_sort
+        sort = sort_dict(sort_operators=sort) if sort else raw_sort
         pipeline = mount_base_pipeline(
             Model=Model,
-            query=query_dict(query_operator=query, dct={}) if query else raw_query,
+            query=query,
+            sort=sort,
             populate=populate,
         )
         pipeline += [{"$limit": 1}]
         try:
             result = self.__aggregate(Model=Model, pipeline=pipeline, as_dict=as_dict)
             return result[0]
         except IndexError:
             return None
 
     def find_many(
         self,
         Model: type[Model],
         query: ComparisonOperator | LogicalOperator = None,
         raw_query: dict = None,
+        sort: SortOperator = None,
+        raw_sort: dict = None,
         populate: bool = False,
         as_dict: bool = False,
         paginate: bool = False,
         current_page: int = 1,
         docs_per_page: int = 1000,
     ):
         if query and (
             type(query) != ComparisonOperator and type(query) != LogicalOperator
         ):
             raise TypeError(
                 'query argument must be a ComparisonOperator or LogicalOperator from pyodmongo.queries. If you really need to make a very specific query, use "raw_query" argument'
             )
+        if sort and (type(sort) != SortOperator):
+            raise TypeError(
+                'sort argument must be a SortOperator from pyodmongo.queries. If you really need to make a very specific sort, use "raw_sort" argument'
+            )
         raw_query = {} if not raw_query else raw_query
         query = query_dict(query_operator=query, dct={}) if query else raw_query
+        raw_sort = {} if not raw_sort else raw_sort
+        sort = sort_dict(sort_operators=sort) if sort else raw_sort
         pipeline = mount_base_pipeline(
             Model=Model,
             query=query,
+            sort=sort,
             populate=populate,
         )
         if not paginate:
             return self.__aggregate(Model=Model, pipeline=pipeline, as_dict=as_dict)
         max_docs_per_page = 1000
         current_page = 1 if current_page <= 0 else current_page
         docs_per_page = (
```

### Comparing `pyodmongo-0.6.8/pyodmongo/engine/utils.py` & `pyodmongo-0.7.0/pyodmongo/engine/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,15 +44,16 @@
                 else:
                     dct[alias] = ObjectId(value) if ObjectId.is_valid(value) else value
             else:
                 dct[alias] = value
     return dct
 
 
-def mount_base_pipeline(Model, query, populate: bool = False):
+def mount_base_pipeline(Model, query: dict, sort: dict, populate: bool = False):
     match_stage = [{"$match": query}]
+    sort_stage = [{"$sort": sort}] if sort != {} else []
     model_stage = Model._pipeline
     reference_stage = Model._reference_pipeline
     if populate:
-        return match_stage + model_stage + reference_stage
+        return match_stage + model_stage + reference_stage + sort_stage
     else:
-        return match_stage + model_stage
+        return match_stage + model_stage + sort_stage
```

### Comparing `pyodmongo-0.6.8/pyodmongo/models/db_model.py` & `pyodmongo-0.7.0/pyodmongo/models/db_model.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/pyodmongo/models/fields.py` & `pyodmongo-0.7.0/pyodmongo/models/fields.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/pyodmongo/models/id_model.py` & `pyodmongo-0.7.0/pyodmongo/models/id_model.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/pyodmongo/queries/comparison_operators.py` & `pyodmongo-0.7.0/pyodmongo/queries/comparison_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/pyodmongo/queries/logical_operators.py` & `pyodmongo-0.7.0/pyodmongo/queries/logical_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/pyodmongo/queries/query_string.py` & `pyodmongo-0.7.0/pyodmongo/queries/query_string.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from ..models.db_model import DbModel
 from ..models.db_field_info import DbField
-from ..models.query_operators import LogicalOperator, ComparisonOperator
+from ..models.query_operators import LogicalOperator, ComparisonOperator, SortOperator
 from .comparison_operators import comparison_operator
+from .sort_operator import sort
 from .logical_operators import and_
 from typing import Type
 from datetime import datetime
 import re
 
 
 def is_inheritance_of_db_model(Model):
@@ -42,21 +43,27 @@
     Model: Type[DbModel],
     items: dict,
     initial_comparison_operators: list[ComparisonOperator],
 ) -> LogicalOperator:
     is_inheritance = is_inheritance_of_db_model(Model=Model)
     if not is_inheritance:
         raise TypeError("Model must be a DbModel")
+    sort_operators = None
     for key, value in items.items():
         value = value.strip()
         if value == "":
             continue
         split_result = key.strip().rsplit(sep="_", maxsplit=1)
         operator = f"${split_result[-1]}"
         if operator not in ["$eq", "$gt", "$gte", "$in", "$lt", "$lte", "$ne", "$nin"]:
+            if operator in ["$sort"]:
+                value = eval(value)
+                for v in value:
+                    v[0] = getattr(Model, v[0])
+                sort_operators = sort(*value)
             continue
         try:
             value = datetime.fromisoformat(value)
         except (TypeError, ValueError):
             try:
                 value = eval(value)
             except (NameError, SyntaxError):
@@ -70,9 +77,9 @@
             db_field_info: DbField = eval("Model." + field_name)
         except AttributeError:
             raise AttributeError(f"There's no field '{field_name}' in {Model.__name__}")
         initial_comparison_operators.append(
             comparison_operator(field=db_field_info, operator=operator, value=value)
         )
     if len(initial_comparison_operators) == 0:
-        return None
-    return and_(*initial_comparison_operators)
+        return None, sort_operators
+    return and_(*initial_comparison_operators), sort_operators
```

### Comparing `pyodmongo-0.6.8/pyodmongo/services/aggregate_stages.py` & `pyodmongo-0.7.0/pyodmongo/services/aggregate_stages.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/pyodmongo/services/model_init.py` & `pyodmongo-0.7.0/pyodmongo/services/model_init.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/pyodmongo/services/query_operators.py` & `pyodmongo-0.7.0/pyodmongo/services/query_operators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,28 @@
-from ..models.query_operators import ComparisonOperator, LogicalOperator
+from ..models.query_operators import ComparisonOperator, LogicalOperator, SortOperator
 
 
 def comparison_operator_dict(co: ComparisonOperator):
     return {co.path_str: {co.operator: co.value}}
 
 
-def query_dict(query_operator: ComparisonOperator | LogicalOperator, dct: dict):
+def query_dict(query_operator: ComparisonOperator | LogicalOperator, dct: dict) -> dict:
     if isinstance(query_operator, ComparisonOperator):
         return comparison_operator_dict(co=query_operator)
     dct[query_operator.operator] = []
     for operator in query_operator.operators:
         if isinstance(operator, ComparisonOperator):
             dct[query_operator.operator].append(comparison_operator_dict(co=operator))
         else:
             dct[query_operator.operator].append(
                 query_dict(query_operator=operator, dct={})
             )
     return dct
+
+
+def sort_dict(sort_operators: SortOperator) -> dict:
+    dct = {}
+    for operator in sort_operators.operators:
+        if operator[1] not in (1, -1):
+            raise ValueError("Only values 1 ascending and -1 descending are valid")
+        dct[operator[0].path_str] = operator[1]
+    return dct
```

### Comparing `pyodmongo-0.6.8/tests/test_async_aggregate.py` & `pyodmongo-0.7.0/tests/test_async_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/tests/test_async_crud_db.py` & `pyodmongo-0.7.0/tests/test_async_crud_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     DbModel,
     SaveResponse,
     DeleteResponse,
     ResponsePaginate,
     Id,
     Field,
 )
-from pyodmongo.queries import eq, gte, gt, mount_query_filter
+from pyodmongo.queries import eq, gte, gt, mount_query_filter, sort
 from pyodmongo.engine.utils import consolidate_dict
 from pydantic import ConfigDict, BaseModel
 from typing import ClassVar
 from bson import ObjectId
 from datetime import datetime
 import pytest
 import pytest_asyncio
@@ -304,15 +304,15 @@
     yield
     await db._db[MyModelRegex._collection].drop()
 
 
 @pytest.mark.asyncio
 async def test_find_regex(create_regex_collection):
     input_dict = {"attr_1_in": "['/^ind[uúû]stria/i']"}
-    query = mount_query_filter(
+    query, _ = mount_query_filter(
         Model=MyModelRegex, items=input_dict, initial_comparison_operators=[]
     )
     results = await db.find_many(Model=MyModelRegex, query=query)
     assert len(results) == 2
 
 
 class AsDict1(DbModel):
@@ -470,15 +470,15 @@
 @pytest.mark.asyncio
 async def test_find_nested_field_mount_query(drop_collections_a_b):
     obj_a = ClassA()
     await db.save(obj=obj_a)
     obj_b = ClassB(a=obj_a)
     await db.save(obj=obj_b)
     input_dict = {"a": obj_a.id}
-    query = mount_query_filter(
+    query, _ = mount_query_filter(
         Model=ClassB, items=input_dict, initial_comparison_operators=[]
     )
     result = await db.find_many(Model=ClassB, query=query, populate=True)
     assert result == [obj_b]
 
 
 class ClassOne(DbModel):
@@ -505,16 +505,16 @@
 
 
 @pytest_asyncio.fixture()
 async def drop_collections_one_three():
     await db._db[ClassOne._collection].drop()
     await db._db[ClassThree._collection].drop()
     yield
-    # await db._db[ClassOne._collection].drop()
-    # await db._db[ClassThree._collection].drop()
+    await db._db[ClassOne._collection].drop()
+    await db._db[ClassThree._collection].drop()
 
 
 @pytest.mark.asyncio
 async def test_nested_list_objects(drop_collections_one_three):
     obj_1 = ClassOne(attr_1="obj_1")
     obj_2 = ClassOne(attr_1="obj_2")
     obj_3 = ClassOne(attr_1="obj_3")
@@ -534,12 +534,55 @@
     obj_14 = ClassTwoB(
         attr_2_b="obj_14", class_two_a=obj_11, class_two_a_list=[obj_11, obj_12]
     )
     obj_15 = ClassThree(
         attr_3="obj_15", class_two_b=obj_13, class_two_b_list=[obj_13, obj_14]
     )
     await db.save(obj_15)
-    from pprint import pprint
 
     obj_found = await db.find_one(Model=ClassThree, populate=True)
     assert obj_found.id == obj_15.id
     assert obj_found.class_two_b.attr_2_b == "obj_13"
+
+
+class MySortClass(DbModel):
+    attr_1: str
+    attr_2: int
+    attr_3: datetime
+    _collection: ClassVar = "my_class_to_sort"
+
+
+@pytest_asyncio.fixture()
+async def drop_collection_for_test_sort():
+    await db._db[MySortClass._collection].drop()
+    yield
+    await db._db[MySortClass._collection].drop()
+
+
+@pytest.mark.asyncio
+async def test_sort_query(drop_collection_for_test_sort):
+    obj_list = [
+        MySortClass(
+            attr_1="Juliet", attr_2=100, attr_3=datetime(year=2023, month=1, day=20)
+        ),
+        MySortClass(
+            attr_1="Albert", attr_2=50, attr_3=datetime(year=2025, month=1, day=20)
+        ),
+        MySortClass(
+            attr_1="Zack", attr_2=30, attr_3=datetime(year=2020, month=1, day=20)
+        ),
+        MySortClass(
+            attr_1="Charlie", attr_2=150, attr_3=datetime(year=2027, month=1, day=20)
+        ),
+        MySortClass(
+            attr_1="Albert", attr_2=40, attr_3=datetime(year=2025, month=1, day=20)
+        ),
+    ]
+    await db.save_all(obj_list=obj_list)
+    sort_oprator = sort((MySortClass.attr_1, 1), (MySortClass.attr_2, 1))
+    result_many = await db.find_many(Model=MySortClass, sort=sort_oprator)
+    assert result_many[0] == obj_list[4]
+    assert result_many[1] == obj_list[1]
+
+    sort_oprator = sort((MySortClass.attr_3, 1))
+    result_one = await db.find_one(Model=MySortClass, sort=sort_oprator)
+    assert result_one == obj_list[2]
```

### Comparing `pyodmongo-0.6.8/tests/test_class.py` & `pyodmongo-0.7.0/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/tests/test_db_field_info.py` & `pyodmongo-0.7.0/tests/test_db_field_info.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/tests/test_db_index.py` & `pyodmongo-0.7.0/tests/test_db_index.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/tests/test_dict_empty.py` & `pyodmongo-0.7.0/tests/test_dict_empty.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/tests/test_fastapi.py` & `pyodmongo-0.7.0/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/tests/test_model_init_functions.py` & `pyodmongo-0.7.0/tests/test_model_init_functions.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/tests/test_object_id.py` & `pyodmongo-0.7.0/tests/test_object_id.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/tests/test_project_pipeline.py` & `pyodmongo-0.7.0/tests/test_project_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/tests/test_pydantic_validators.py` & `pyodmongo-0.7.0/tests/test_pydantic_validators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/tests/test_queries.py` & `pyodmongo-0.7.0/tests/test_queries.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,17 +12,18 @@
     lte,
     ne,
     nin,
     text,
     and_,
     or_,
     nor,
+    sort,
     mount_query_filter,
 )
-from pyodmongo.services.query_operators import query_dict
+from pyodmongo.services.query_operators import query_dict, sort_dict
 import pytest
 
 
 class Model1(DbModel):
     a: str = Field(alias="aAlias")
     b: str
     _collection: ClassVar = "model_1"
@@ -110,25 +111,25 @@
         ]
     }
 
 
 def test_mount_query_filter_with_invalid_field():
     dict_input = {"c_eq": "value1", "d_in": '["abc", "xyz"]', "vrau_eq": "ddsff"}
     with pytest.raises(AttributeError):
-        query = mount_query_filter(
+        query, _ = mount_query_filter(
             Model=Model2, items=dict_input, initial_comparison_operators=[]
         )
 
 
 def test_mount_query_filter():
     dict_input = {
         "id_eq": "64e8ef019af47dc6f91c5a48",
         "g_in": "['64e8ef019af47dc6f91c5a48', '64e8f1a5f1dae6703924546a']",
     }
-    query = mount_query_filter(
+    query, _ = mount_query_filter(
         Model=Model3, items=dict_input, initial_comparison_operators=[]
     )
     assert query_dict(query_operator=query, dct={}) == {
         "$and": [
             {"_id": {"$eq": ObjectId("64e8ef019af47dc6f91c5a48")}},
             {
                 "g": {
@@ -160,15 +161,15 @@
         "attr_1_eq": "Value1",
         "attr_2_eq": "Value2",
         "attr_3_eq": "Value3",
         "attr_4_eq": "Value4",
         "attr_4_in": "",
         "attr_4_er": "Value_error",
     }
-    query = mount_query_filter(
+    query, _ = mount_query_filter(
         Model=FourthModel, items=input_dict, initial_comparison_operators=[]
     )
     expected_query_dict = {
         "$and": [
             {"attr_1": {"$eq": "Value1"}},
             {"attr_2": {"$eq": "Value2"}},
             {"attr_3": {"$eq": "Value3"}},
@@ -196,41 +197,41 @@
     input_dict = {
         "attr_1_eq": "Value1",
         "attr_2_eq": "Value2",
         "attr_3_eq": "Value3",
         "attr_4_eq": "Value4",
     }
     with pytest.raises(TypeError, match="Model must be a DbModel"):
-        query = mount_query_filter(
+        query, _ = mount_query_filter(
             Model=FourthModel, items=input_dict, initial_comparison_operators=[]
         )
 
 
 def test_mount_query_filter_with_none_value():
     class MainModel(DbModel):
         attr_1: str = None
         _collection: ClassVar = "main_model"
 
     input_dict = {}
-    query = mount_query_filter(
+    query, _ = mount_query_filter(
         Model=MainModel, items=input_dict, initial_comparison_operators=[]
     )
     assert query is None
 
 
 def test_mount_query_filter_with_regex():
     import re
 
     class MyModel(DbModel):
         attr1: str
         attr2: str
 
     input_dict = {"attr1_in": "['/^agr[oóôõ]s/i', 123, 'abc']", "attr2_eq": "123"}
 
-    query = mount_query_filter(
+    query, _ = mount_query_filter(
         Model=MyModel, items=input_dict, initial_comparison_operators=[]
     )
     query_dct = query_dict(query_operator=query, dct={})
     assert query_dct == {
         "$and": [
             {"attr1": {"$in": [re.compile("^agr[oóôõ]s", re.IGNORECASE), 123, "abc"]}},
             {"attr2": {"$eq": 123}},
@@ -250,15 +251,15 @@
     input_dct = {
         "string_value_eq": "AString",
         "int_value_gt": "10",
         "float_value_lte": "50.6",
         "bool_value_eq": "True",
         "date_value_lte": "2024-06-01",
     }
-    query_dct = mount_query_filter(
+    query_dct, _ = mount_query_filter(
         Model=MyClass, items=input_dct, initial_comparison_operators=[]
     )
     assert query_dct.operators[0].value == "AString"
     assert type(query_dct.operators[0].value) is str
     assert query_dct.operators[1].value == 10
     assert type(query_dct.operators[1].value) is int
     assert query_dct.operators[2].value == 50.6
@@ -288,7 +289,58 @@
                 ]
             },
             {"aAlias": {"$eq": "string_to_find_1"}},
         ]
     }
     query_dct = query_dict(query_operator=query, dct={})
     assert query_dct == expected_dct
+
+
+def test_sort_operator():
+    class MyNestedClass(BaseModel):
+        n: int
+
+    class MyClass(DbModel):
+        a: str
+        b: int
+        c: int
+        nested: MyNestedClass
+
+    sort_operator = sort(
+        (MyClass.nested.n, -1), (MyClass.b, 1), (MyClass.c, -1), (MyClass.a, 1)
+    )
+    assert sort_dict(sort_operators=sort_operator) == {
+        "nested.n": -1,
+        "b": 1,
+        "c": -1,
+        "a": 1,
+    }
+
+    with pytest.raises(
+        ValueError, match="Only values 1 ascending and -1 descending are valid"
+    ):
+        sort_dict(sort_operators=sort((MyClass.a, 2)))
+
+
+def test_mount_query_string_with_sort():
+    class MyClass(DbModel):
+        attr_1: str
+        attr_2: str
+        attr_3: str
+
+    input_dict = {
+        "attr_1_eq": "attr 1",
+        "attr_2_in": "['value_1', 'value_2']",
+        "attr_3_gte": "10",
+        "_sort": "[['attr_1', 1], ['attr_2', -1]]",
+    }
+
+    query, sort_operator = mount_query_filter(
+        Model=MyClass, items=input_dict, initial_comparison_operators=[]
+    )
+
+    assert query == and_(
+        eq(MyClass.attr_1, "attr 1"),
+        in_(MyClass.attr_2, ["value_1", "value_2"]),
+        gte(MyClass.attr_3, 10),
+    )
+    assert sort_operator == sort((MyClass.attr_1, 1), (MyClass.attr_2, -1))
```

### Comparing `pyodmongo-0.6.8/tests/test_reference_pipeline.py` & `pyodmongo-0.7.0/tests/test_reference_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from pyodmongo import DbModel, Id, Field
 from pydantic import BaseModel
 from typing import ClassVar
-from pprint import pprint
 
 
 def test_single_class_project_pipeline():
     class A(DbModel):
         a1: str
         a2: str
         _collection: ClassVar = "a"
@@ -125,16 +124,14 @@
         _pipeline: ClassVar = ["manual pipeline here"]
 
     assert MyModel1._pipeline == []
     assert MyModel2._pipeline == ["manual pipeline here"]
 
 
 def test_recursive_reference_pipeline():
-    from pprint import pprint
-
     class Zero(DbModel):
         attr_0: str = "Zero"
         _collection: ClassVar = "col_0"
 
     class A(DbModel):
         attr_1: str = "One"
         zero_1: Zero | Id = Zero()
```

### Comparing `pyodmongo-0.6.8/tests/test_save_dict.py` & `pyodmongo-0.7.0/tests/test_save_dict.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/tests/test_sync_aggregate.py` & `pyodmongo-0.7.0/tests/test_sync_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/tests/test_sync_crud_db.py` & `pyodmongo-0.7.0/tests/test_sync_crud_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     DbModel,
     Id,
     SaveResponse,
     DeleteResponse,
     ResponsePaginate,
     Field,
 )
-from pyodmongo.queries import eq, gte, gt
+from pyodmongo.queries import eq, gte, gt, sort
 from pyodmongo.engine.utils import consolidate_dict
 from pydantic import ConfigDict
 from typing import ClassVar
 from bson import ObjectId
 from datetime import datetime
 import pytest
 
@@ -348,7 +348,50 @@
     obj_list = db.find_many(Model=AsDict2, as_dict=True, populate=True)
     assert len(obj_list) == 4
     assert type(obj_list) is list
     for dct in obj_list:
         assert type(dct) == dict
     obj_dict = db.find_one(Model=AsDict2, as_dict=True, populate=True)
     assert type(obj_dict) == dict
+
+
+class MySortClass(DbModel):
+    attr_1: str
+    attr_2: int
+    attr_3: datetime
+    _collection: ClassVar = "my_class_to_sort"
+
+
+@pytest.fixture()
+def drop_collection_for_test_sort():
+    db._db[MySortClass._collection].drop()
+    yield
+    db._db[MySortClass._collection].drop()
+
+
+def test_sort_query(drop_collection_for_test_sort):
+    obj_list = [
+        MySortClass(
+            attr_1="Juliet", attr_2=100, attr_3=datetime(year=2023, month=1, day=20)
+        ),
+        MySortClass(
+            attr_1="Albert", attr_2=50, attr_3=datetime(year=2025, month=1, day=20)
+        ),
+        MySortClass(
+            attr_1="Zack", attr_2=30, attr_3=datetime(year=2020, month=1, day=20)
+        ),
+        MySortClass(
+            attr_1="Charlie", attr_2=150, attr_3=datetime(year=2027, month=1, day=20)
+        ),
+        MySortClass(
+            attr_1="Albert", attr_2=40, attr_3=datetime(year=2025, month=1, day=20)
+        ),
+    ]
+    db.save_all(obj_list=obj_list)
+    sort_oprator = sort((MySortClass.attr_1, 1), (MySortClass.attr_2, 1))
+    result_many = db.find_many(Model=MySortClass, sort=sort_oprator)
+    assert result_many[0] == obj_list[4]
+    assert result_many[1] == obj_list[1]
+
+    sort_oprator = sort((MySortClass.attr_3, 1))
+    result_one = db.find_one(Model=MySortClass, sort=sort_oprator)
+    assert result_one == obj_list[2]
```

### Comparing `pyodmongo-0.6.8/.gitignore` & `pyodmongo-0.7.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -125,8 +125,9 @@
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 .vscode
 test.py
-coverage.json
+coverage.json
+.DS_Store
```

### Comparing `pyodmongo-0.6.8/LICENSE` & `pyodmongo-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/README.md` & `pyodmongo-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.8/pyproject.toml` & `pyodmongo-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyodmongo"
-version = "0.6.8"
+version = "0.7.0"
 license = "MIT"
 authors = [
   { name="Mauro André", email="eng.mauroandre@gmail.com" },
 ]
 description = "A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `pyodmongo-0.6.8/PKG-INFO` & `pyodmongo-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyodmongo
-Version: 0.6.8
+Version: 0.7.0
 Summary: A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic
 Project-URL: Homepage, https://github.com/mauro-andre/pyodmongo
 Project-URL: Documentation, https://pyodmongo.dev
 Author-email: Mauro André <eng.mauroandre@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

