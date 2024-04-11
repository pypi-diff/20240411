# Comparing `tmp/dataloom-2.4.1.tar.gz` & `tmp/dataloom-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataloom-2.4.1.tar", last modified: Sat Mar  2 13:27:21 2024, max compression
+gzip compressed data, was "dataloom-2.4.2.tar", last modified: Thu Apr 11 15:13:14 2024, max compression
```

## Comparing `dataloom-2.4.1.tar` & `dataloom-2.4.2.tar`

### file list

```diff
@@ -1,115 +1,182 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.179101 dataloom-2.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.163101 dataloom-2.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:14.000000 dataloom-2.4.1/.github/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.163101 dataloom-2.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-02 13:27:14.000000 dataloom-2.4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-02 13:27:14.000000 dataloom-2.4.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-03-02 13:27:14.000000 dataloom-2.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11184 2024-03-02 13:27:14.000000 dataloom-2.4.1/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-02 13:27:14.000000 dataloom-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   122851 2024-03-02 13:27:21.179101 dataloom-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)   119957 2024-03-02 13:27:14.000000 dataloom-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.163101 dataloom-2.4.1/dataloom/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.163101 dataloom-2.4.1/dataloom/columns/
--rw-r--r--   0 runner    (1001) docker     (127)    26395 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/columns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.163101 dataloom-2.4.1/dataloom/conn/
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/conn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.163101 dataloom-2.4.1/dataloom/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.163101 dataloom-2.4.1/dataloom/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.163101 dataloom-2.4.1/dataloom/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/keys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.167101 dataloom-2.4.1/dataloom/loom/
--rw-r--r--   0 runner    (1001) docker     (127)    68320 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/loom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/loom/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/loom/insert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/loom/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/loom/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/loom/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/loom/qb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/loom/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/loom/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    18981 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/loom/subqueries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/loom/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.167101 dataloom-2.4.1/dataloom/model/
--rw-r--r--   0 runner    (1001) docker     (127)    28776 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.167101 dataloom-2.4.1/dataloom/statements/
--rw-r--r--   0 runner    (1001) docker     (127)    44903 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/statements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15610 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/statements/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.159101 dataloom-2.4.1/dataloom/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.171101 dataloom-2.4.1/dataloom/tests/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_aggregation_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_alter_tables_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_connection_options_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_connection_uri_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_create_tables_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)    16600 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_delete_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)    40798 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_eager_loading_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_experimental_decorators_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_insert_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_inspect_table_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_operators_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_qb_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)    24168 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_query_msql.py
--rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_update_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/mysql/test_utils_fns_mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.171101 dataloom-2.4.1/dataloom/tests/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_aggregation_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_alter_tables_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_connection_options_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_connection_uri_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_create_table_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)    16066 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_delete_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)    42342 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_eager_loading_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_experimental_decorators_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_insert_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_inspecting_table_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_operators_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_qb_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)    23817 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_query_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_update_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/postgres/test_utils_fns_pg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.175101 dataloom-2.4.1/dataloom/tests/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_aggregation_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_alter_tables_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_connection_options_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_connection_uri_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_create_table_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    15444 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_delete_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    39861 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_eager_loading_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_experimental_decorators_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_insert_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_inspect_table_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_operators_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_qb_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    23035 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_query_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_update_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/tests/sqlite3/test_utils_fns_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.175101 dataloom-2.4.1/dataloom/types/
--rw-r--r--   0 runner    (1001) docker     (127)    14829 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.175101 dataloom-2.4.1/dataloom/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/utils/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/utils/alter_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/utils/create_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/utils/loom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/utils/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom/utils/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:27:21.175101 dataloom-2.4.1/dataloom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)   122851 2024-03-02 13:27:21.000000 dataloom-2.4.1/dataloom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-03-02 13:27:21.000000 dataloom-2.4.1/dataloom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 13:27:21.000000 dataloom-2.4.1/dataloom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-02 13:27:21.000000 dataloom-2.4.1/dataloom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-02 13:27:21.000000 dataloom-2.4.1/dataloom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-03-02 13:27:14.000000 dataloom-2.4.1/dataloom.png
--rw-r--r--   0 runner    (1001) docker     (127)    90112 2024-03-02 13:27:14.000000 dataloom-2.4.1/hi.db
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-02 13:27:14.000000 dataloom-2.4.1/playground.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-02 13:27:14.000000 dataloom-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-02 13:27:14.000000 dataloom-2.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 13:27:21.179101 dataloom-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-02 13:27:14.000000 dataloom-2.4.1/todo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.413930 dataloom-2.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.389930 dataloom-2.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:04.000000 dataloom-2.4.2/.github/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.389930 dataloom-2.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-11 15:13:04.000000 dataloom-2.4.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-11 15:13:04.000000 dataloom-2.4.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-11 15:13:04.000000 dataloom-2.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-11 15:13:04.000000 dataloom-2.4.2/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.389930 dataloom-2.4.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 15:13:04.000000 dataloom-2.4.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11398 2024-04-11 15:13:04.000000 dataloom-2.4.2/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-11 15:13:04.000000 dataloom-2.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   123684 2024-04-11 15:13:14.413930 dataloom-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)   120790 2024-04-11 15:13:04.000000 dataloom-2.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.389930 dataloom-2.4.2/dataloom/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.393930 dataloom-2.4.2/dataloom/columns/
+-rw-r--r--   0 runner    (1001) docker     (127)    26395 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/columns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.393930 dataloom-2.4.2/dataloom/conn/
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/conn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.393930 dataloom-2.4.2/dataloom/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.393930 dataloom-2.4.2/dataloom/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.393930 dataloom-2.4.2/dataloom/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.393930 dataloom-2.4.2/dataloom/loom/
+-rw-r--r--   0 runner    (1001) docker     (127)    68320 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/loom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/loom/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/loom/insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/loom/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/loom/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/loom/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/loom/qb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/loom/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/loom/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18981 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/loom/subqueries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/loom/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.393930 dataloom-2.4.2/dataloom/model/
+-rw-r--r--   0 runner    (1001) docker     (127)    28776 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.393930 dataloom-2.4.2/dataloom/statements/
+-rw-r--r--   0 runner    (1001) docker     (127)    44903 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/statements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15610 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/statements/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.385930 dataloom-2.4.2/dataloom/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.397930 dataloom-2.4.2/dataloom/tests/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_aggregation_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_alter_tables_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_connection_options_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_connection_uri_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_create_tables_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16600 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_delete_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40798 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_eager_loading_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_experimental_decorators_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_insert_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_inspect_table_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_operators_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_qb_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24168 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_query_msql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_update_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/mysql/test_utils_fns_mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.401930 dataloom-2.4.2/dataloom/tests/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_aggregation_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_alter_tables_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_connection_options_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_connection_uri_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_create_table_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16066 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_delete_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42342 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_eager_loading_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_experimental_decorators_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_insert_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_inspecting_table_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_operators_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_qb_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23817 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_query_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_update_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/postgres/test_utils_fns_pg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.401930 dataloom-2.4.2/dataloom/tests/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_aggregation_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_alter_tables_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_connection_options_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_connection_uri_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_create_table_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15444 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_delete_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39861 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_eager_loading_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_experimental_decorators_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_insert_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_inspect_table_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_operators_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_qb_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23035 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_query_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_update_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/tests/sqlite3/test_utils_fns_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.401930 dataloom-2.4.2/dataloom/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    14829 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.405930 dataloom-2.4.2/dataloom/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/utils/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/utils/alter_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/utils/create_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/utils/loom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/utils/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom/utils/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.413930 dataloom-2.4.2/dataloom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)   123684 2024-04-11 15:13:14.000000 dataloom-2.4.2/dataloom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-11 15:13:14.000000 dataloom-2.4.2/dataloom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:13:14.000000 dataloom-2.4.2/dataloom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-11 15:13:14.000000 dataloom-2.4.2/dataloom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 15:13:14.000000 dataloom-2.4.2/dataloom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-11 15:13:04.000000 dataloom-2.4.2/dataloom.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.405930 dataloom-2.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.405930 dataloom-2.4.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.389930 dataloom-2.4.2/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.405930 dataloom-2.4.2/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/_static/css/index.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.405930 dataloom-2.4.2/docs/source/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.409930 dataloom-2.4.2/docs/source/api/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    16230 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/column.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/column_value.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/created_at.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/filter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/fk_column.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/group.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/having.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/include.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/loom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/order.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/pk_column.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/classes/updated_at.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/qb.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.409930 dataloom-2.4.2/docs/source/api/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/tables/connect_and_sync.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/tables/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/api/tables/sync.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.409930 dataloom-2.4.2/docs/source/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.409930 dataloom-2.4.2/docs/source/examples/associations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/associations/bi_directional.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/associations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/associations/n_to_n.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/associations/n_to_one.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/associations/one_to_n.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/associations/one_to_one.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/associations/self_relations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/data_aggregation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/filtering.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.409930 dataloom-2.4.2/docs/source/examples/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/operations/create.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/operations/delete.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/operations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13621 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/operations/read.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/operations/update.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/examples/ordering.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.409930 dataloom-2.4.2/docs/source/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/github/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/github/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:13:14.413930 dataloom-2.4.2/docs/source/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/utilities/avg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/utilities/count.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/utilities/decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/utilities/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/utilities/inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/utilities/max.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/utilities/min.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-11 15:13:04.000000 dataloom-2.4.2/docs/source/utilities/sum.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    90112 2024-04-11 15:13:04.000000 dataloom-2.4.2/hi.db
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 15:13:04.000000 dataloom-2.4.2/playground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-11 15:13:04.000000 dataloom-2.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-11 15:13:04.000000 dataloom-2.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:13:14.413930 dataloom-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-11 15:13:04.000000 dataloom-2.4.2/todo.txt
```

### Comparing `dataloom-2.4.1/.github/workflows/ci.yml` & `dataloom-2.4.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/.gitignore` & `dataloom-2.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/Changelog.md` & `dataloom-2.4.2/Changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 ===
+Dataloom **`2.4.2`**
+===
+
+### Release Notes - `dataloom`
+
+We have release the new `dataloom` Version `2.4.2` (`2024-04-11`)
+
+##### Changes
+
+- updated documentation
+- documentation available on Read the Docs.
+
+===
 Dataloom **`2.4.1`**
 ===
 
 ### Release Notes - `dataloom`
 
 We have release the new `dataloom` Version `2.4.1` (`2024-03-02`)
 
 ##### Changes
+
 - Updated documentation.
 
 ===
 Dataloom **`2.4.0`**
 ===
 
 ### Release Notes - `dataloom`
```

### Comparing `dataloom-2.4.1/LICENSE` & `dataloom-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/PKG-INFO` & `dataloom-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataloom
-Version: 2.4.1
+Version: 2.4.2
 Summary: dataloom stands as a bespoke Object-Relational Mapping (ORM) solution meticulously crafted to empower Python developers in efficiently managing diverse databases. Unlike conventional ORMs, Dataloom has been built from the ground up, providing native support for SQLite3, PostgreSQL, and MySQL. Navigate effortlessly between database engines while enjoying a tailored and performant ORM experience.
 Author-email: Crispen Gari <crispengari@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 crispengari
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -160,14 +160,15 @@
     - [Inserting](#inserting-3)
     - [Retrieving Records](#retrieving-records-3)
   - [6. `N-N` Relationship](#6-n-n-relationship)
     - [Inserting](#inserting-4)
     - [Retrieving Records](#retrieving-records-4)
 - [Query Builder.](#query-builder)
   - [Why Use Query Builder?](#why-use-query-builder)
+- [Documentation](#documentation)
 - [Contributing](#contributing)
 - [License](#license)
 
 ### Key Features:
 
 - **Lightweight**: `dataloom` is designed to be minimalistic and easy to use, ensuring a streamlined `ORM` experience without unnecessary complexities.
 
@@ -532,22 +533,23 @@
     __tablename__: Optional[TableColumn] = TableColumn(name="users")
     id = PrimaryKeyColumn(type="int", auto_increment=True)
     #...rest of your columns
 
 ```
 
 The following are the arguments that the `PrimaryKeyColumn` class accepts.
-| Argument | Description | Type | Default |
-| ---------------- | ------------------------------------------------------------------------------------------------------------------------ | --------------- | ------------- |
-| `type` | The datatype of your primary key. | `str` | `"int`" |
-| `length` | Optional to specify the length of the type. If passed as `N` with type `T`, it yields an SQL statement with type `T(N)`. | `int` \| `None` | `None` |
-| `auto_increment`| Optional to specify if the column will automatically increment or not. |`bool` |`False` |
-|`default` | Optional to specify the default value in a column. |`any` |`None` |
-|`nullable` | Optional to specify if the column will allow null values or not. |`bool` |`False` |
-|`unique` | Optional to specify if the column will contain unique values or not. |`bool` |`True` |
+
+| Argument         | Description                                                                                                              | Type            | Default |
+| ---------------- | ------------------------------------------------------------------------------------------------------------------------ | --------------- | ------- |
+| `type`           | The datatype of your primary key.                                                                                        | `str`           | `"int`" |
+| `length`         | Optional to specify the length of the type. If passed as `N` with type `T`, it yields an SQL statement with type `T(N)`. | `int` \| `None` | `None`  |
+| `auto_increment` | Optional to specify if the column will automatically increment or not.                                                   | `bool`          | `False` |
+| `default`        | Optional to specify the default value in a column.                                                                       | `any`           | `None`  |
+| `nullable`       | Optional to specify if the column will allow null values or not.                                                         | `bool`          | `False` |
+| `unique`         | Optional to specify if the column will contain unique values or not.                                                     | `bool`          | `True`  |
 
 #### `ForeignKeyColumn` Class
 
 This class is utilized when informing `dataloom` that a column has a relationship with a primary key in another table. Consider the following model definition of a `Post`:
 
 ```py
 class Post(Model):
@@ -750,15 +752,15 @@
     conn.close()
 ```
 
 Returns a `conn` and the list of `tablenames` that exist in the database. The method accepts the same arguments as the `sync` method.
 
 ### CRUD Operations with Dataloom
 
-In this section of the documentation, we will illustrate how to perform basic `CRUD` operations using `dataloom` on simple `Models`. Please note that in the following code snippets, I will be utilizing `sqlite_loom`. However, it's important to highlight that you can use any `loom` of your choice to follow along.
+In this section of the documentation, we will illustrate how to perform basic `CRUD` operations using `dataloom` on simple `Models`. Please note that in the following code snippets, I will be utilizing `sqlite_loom`, `mysql_loom`, `pg_loom` or `loom` interchangeably. However, it's important to highlight that you can use any `loom` of your choice to follow along.
 
 #### 1. Creating a Record
 
 To insert a single or multiple records in a database you make use of the following functions:
 
 1. `insert_one()`
 2. `insert_bulk()`
@@ -892,15 +894,15 @@
 | `filters`  | Collection of `Filter` or a `Filter` to apply to the query.                                | `list[Filter] \| Filter` | `None`  | `No`     |
 | `distinct` | Boolean telling dataloom to return distinct row values based on selected fields or not.    | `bool`                   | `False` | `No`     |
 
 > 👍 **Pro Tip**: The distinction between the `find_all()` and `find_many()` methods lies in the fact that `find_many()` enables you to apply specific filters, whereas `find_all()` retrieves all the documents within the specified model.
 
 ##### 3. `find_one()`
 
-Here is an example showing you how you can use `find_by_pk()` locate a single record in the database.
+Here is an example showing you how you can use `find_one()` locate a single record in the database.
 
 ```py
 user = mysql_loom.find_one(
     User,
     filters=[Filter(column="username", value="@miller")],
     select=["id", "username"],
 )
@@ -1086,16 +1088,19 @@
 To mitigate the potential risks associated with `delete_bulk()`, follow these guidelines:
 
 1. **Always Provide a Filter:**
 
    - When calling `delete_bulk()`, make sure to provide a filter to specify the subset of records to be deleted. This helps prevent unintentional deletions.
 
    ```python
-   # Example: Delete records where 'status' is 'inactive'
-   sqlite_loom.delete_bulk(filter={'status': 'inactive'})
+    # Example: Delete records where 'status' is 'inactive'
+    affected_rows = mysql_loom.delete_bulk(
+        instance=User,
+        filters=Filter(column="status",  value='inactive'),
+    )
    ```
 
 2. **Consider Usage When Necessary:**
 
 - When contemplating data deletion, it is advisable to consider more targeted methods before resorting to `delete_bulk()`. Prioritize the use of `delete_one()` or `delete_by_pk()` methods to remove specific records based on your needs. This ensures a more precise and controlled approach to data deletion.
 
 3. **Use limit and offsets options**
@@ -2526,14 +2531,18 @@
 
   ```python
   qb = loom.getQueryBuilder()
   result = qb.run("SELECT * FROM table1 INNER JOIN table2 ON table1.id = table2.table1_id;")
   print(result)
   ```
 
+### Documentation
+
+You can read the full documentation of dataloom on [readthedocs.io](https://dataloom-py.readthedocs.io/en/latest/)
+
 ### Contributing
 
 Contributions to `dataloom` are welcome! Feel free to submit bug reports, feature requests, or pull requests on [GitHub](https://github.com/CrispenGari/dataloom).
 
 ### License
 
 This project is licensed under the MIT License - see the [LICENSE](/LISENSE) file for details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dataloom Version: 2.4.1 Summary: dataloom stands as
+Metadata-Version: 2.1 Name: dataloom Version: 2.4.2 Summary: dataloom stands as
 a bespoke Object-Relational Mapping (ORM) solution meticulously crafted to
 empower Python developers in efficiently managing diverse databases. Unlike
 conventional ORMs, Dataloom has been built from the ground up, providing native
 support for SQLite3, PostgreSQL, and MySQL. Navigate effortlessly between
 database engines while enjoying a tailored and performant ORM experience.
 Author-email: Crispen Gari
 gmail.com> License: MIT License Copyright (c) 2024 crispengari Permission is
@@ -95,38 +95,39 @@
 [Inserting](#inserting-2) - [Retrieving Records](#retrieving-records-2) - [4.
 What about bidirectional queries?](#4-what-about-bidirectional-queries) - [1.
 Child to Parent](#1-child-to-parent) - [2. Parent to Child](#2-parent-to-child)
 - [5. `Self` Association](#5-self-association) - [Inserting](#inserting-3) -
 [Retrieving Records](#retrieving-records-3) - [6. `N-N` Relationship](#6-n-n-
 relationship) - [Inserting](#inserting-4) - [Retrieving Records](#retrieving-
 records-4) - [Query Builder.](#query-builder) - [Why Use Query Builder?](#why-
-use-query-builder) - [Contributing](#contributing) - [License](#license) ###
-Key Features: - **Lightweight**: `dataloom` is designed to be minimalistic and
-easy to use, ensuring a streamlined `ORM` experience without unnecessary
-complexities. - **Database Support**: `dataloom` supports popular relational
-databases such as `PostgreSQL`, `MySQL`, and `SQLite3`, making it suitable for
-a variety of projects. - **Simplified Querying**: The `ORM` simplifies the
-process of database querying, allowing developers to interact with the database
-using Python classes and methods rather than raw SQL queries. - **Intuitive
-Syntax**: `dataloom`'s syntax is intuitive and `Pythonic`, making it accessible
-for developers familiar with the Python language. - **Flexible Data Types**:
-The `ORM` seamlessly handles various data types, offering flexibility in
-designing database schemas. ### Installation To install `dataloom`, you just
-need to run the following command using `pip`: ```bash pip install dataloom ```
-### Python Version Compatibility `dataloom` supports **`Python`** version
-**`3.12`** and above. Ensure that you are using a compatible version of
-**`Python`** before installing or using `dataloom`. You can check your
-**`Python`** version by running: ```bash python --version ``` ### Usage In this
-section we are going to go through how you can use our `orm` package in your
-project. ### Connection To use Dataloom, you need to establish a connection
-with a specific database `dialect`. The available dialect options are `mysql`,
-`postgres`, and `sqlite`. #### `Postgres` The following is an example of how
-you can establish a connection with postgres database. ```python from dataloom
-import Loom # Create a Loom instance with PostgreSQL configuration pg_loom =
-Loom( dialect="postgres", database="hi", password="root", user="postgres",
+use-query-builder) - [Documentation](#documentation) - [Contributing]
+(#contributing) - [License](#license) ### Key Features: - **Lightweight**:
+`dataloom` is designed to be minimalistic and easy to use, ensuring a
+streamlined `ORM` experience without unnecessary complexities. - **Database
+Support**: `dataloom` supports popular relational databases such as
+`PostgreSQL`, `MySQL`, and `SQLite3`, making it suitable for a variety of
+projects. - **Simplified Querying**: The `ORM` simplifies the process of
+database querying, allowing developers to interact with the database using
+Python classes and methods rather than raw SQL queries. - **Intuitive Syntax**:
+`dataloom`'s syntax is intuitive and `Pythonic`, making it accessible for
+developers familiar with the Python language. - **Flexible Data Types**: The
+`ORM` seamlessly handles various data types, offering flexibility in designing
+database schemas. ### Installation To install `dataloom`, you just need to run
+the following command using `pip`: ```bash pip install dataloom ``` ### Python
+Version Compatibility `dataloom` supports **`Python`** version **`3.12`** and
+above. Ensure that you are using a compatible version of **`Python`** before
+installing or using `dataloom`. You can check your **`Python`** version by
+running: ```bash python --version ``` ### Usage In this section we are going to
+go through how you can use our `orm` package in your project. ### Connection To
+use Dataloom, you need to establish a connection with a specific database
+`dialect`. The available dialect options are `mysql`, `postgres`, and `sqlite`.
+#### `Postgres` The following is an example of how you can establish a
+connection with postgres database. ```python from dataloom import Loom # Create
+a Loom instance with PostgreSQL configuration pg_loom = Loom
+( dialect="postgres", database="hi", password="root", user="postgres",
 host="localhost", sql_logger="console", logs_filename="logs.sql", port=5432, )
 # Connect to the PostgreSQL database conn = pg_loom.connect() # Close the
 connection when the script completes if __name__ == "__main__": conn.close()
 ``` In `dataloom` you can use connection uris to establish a connection to the
 database in `postgres` as follows: ```py pg_loom = Loom( dialect="postgres",
 connection_uri = "postgressql://root:root@localhost:5432/hi", # ... ) ``` This
 will establish a connection with `postgres` with the database `hi`. ####
@@ -286,121 +287,120 @@
 `PrimaryKeyColumn` is required. Below is an example of creating an `id` column
 as a primary key in a table named `Post`: ```python class Post(Model):
 __tablename__: Optional[TableColumn] = TableColumn(name="users") id =
 PrimaryKeyColumn(type="int", auto_increment=True) #...rest of your columns ```
 The following are the arguments that the `PrimaryKeyColumn` class accepts. |
 Argument | Description | Type | Default | | ---------------- | ----------------
 -------------------------------------------------------------------------------
-------------------------- | --------------- | ------------- | | `type` | The
-datatype of your primary key. | `str` | `"int`" | | `length` | Optional to
-specify the length of the type. If passed as `N` with type `T`, it yields an
-SQL statement with type `T(N)`. | `int` \| `None` | `None` | |
-`auto_increment`| Optional to specify if the column will automatically
-increment or not. |`bool` |`False` | |`default` | Optional to specify the
-default value in a column. |`any` |`None` | |`nullable` | Optional to specify
-if the column will allow null values or not. |`bool` |`False` | |`unique` |
-Optional to specify if the column will contain unique values or not. |`bool`
-|`True` | #### `ForeignKeyColumn` Class This class is utilized when informing
-`dataloom` that a column has a relationship with a primary key in another
-table. Consider the following model definition of a `Post`: ```py class Post
-(Model): __tablename__: Optional[TableColumn] = TableColumn(name="posts") id =
-PrimaryKeyColumn(type="int", auto_increment=True, nullable=False, unique=True)
-completed = Column(type="boolean", default=False) title = Column
-(type="varchar", length=255, nullable=False) # timestamps createdAt =
-CreatedAtColumn() updatedAt = UpdatedAtColumn() # relations userId =
-ForeignKeyColumn( User, type="int", required=True, onDelete="CASCADE",
-onUpdate="CASCADE" ) ``` - `userId` is a foreign key in the table `posts`,
-indicating it has a relationship with a primary key in the `users` table. This
-column accepts the following arguments: | Argument | Description | Type |
-Default | | ---------- | ------------------------------------------------------
--------------------------------------------------------------- | --------------
--------------------------- | ----------- | | `table` | Required. This is the
-parent table that the current model references. In our example, this is
-referred to as `User`. It can be used as a string in self relations. |
-`Model`\| `str` | | | `type` | Optional. Specifies the data type of the foreign
-key. If not provided, dataloom can infer it from the parent table. | `str` \|
-`None` | `None` | | `required` | Optional. Indicates whether the foreign key is
-required or not. | `bool` | `False` | | `onDelete` | Optional. Specifies the
-action to be taken when the associated record in the parent table is deleted.
-|`"NO ACTION"`, `"SET NULL"`, `"CASCADE"` | `"NO ACTION"` | | `onUpdate` |
-Optional. Specifies the action to be taken when the associated record in the
-parent table is updated. | `"NO ACTION"`, `"SET NULL"`, `"CASCADE"`| `"NO
-ACTION"` | It is crucial to specify the actions for `onDelete` and `onUpdate`
-to ensure that `dataloom` manages your model's relationship actions
-appropriately. The available actions are: 1. `"NO ACTION"` - If you delete or
-update the parent table, no changes will occur in the child table. 2. `"SET
-NULL"` - If you delete or update the parent table, the corresponding value in
-the child table will be set to `null`. 3. `"CASCADE"` - If you delete or update
-the table, the same action will also be applied to the child table. ####
-`CreatedAtColumn` Class When a column is designated as `CreatedAtColumn`, its
-value will be automatically generated each time you create a new record in a
-database, serving as a timestamp. #### `UpdatedAtColumn` Class When a column is
-designated as `UpdatedAtColumn`, its value will be automatically generated each
-time you create a new record or update an existing record in a database table,
-acting as a timestamp. #### `Filter` Class This `Filter` class in `dataloom` is
-designed to facilitate the application of filters when executing queries and
-mutations. It allows users to specify conditions that must be met for the
-operation to affect certain rows in a database table. Below is an example
-demonstrating how this class can be used: ```python affected_rows =
-pg_loom.update_one( Post, values=[ ColumnValue(name="title", value="Hey"),
-ColumnValue(name="completed", value=True), ], filters=[ Filter(column="id",
-value=1, join_next_with="AND"), Filter(column="userId", value=1,
-join_next_with="AND"), ], ) ``` So from the above example we are applying
-filters while updating a `Post` here are the options that you can pass on that
-filter class: | Argument | Description | Type | Default | |--------------------
------|------------------------------------------------------------|------------
--------------------------------|------------------------| | `column` | The name
-of the column to apply the filter on | `String` | - | | `value` | The value to
-filter against | `Any` | - | | `operator` | The comparison operator to use for
-the filter | `'eq'`, `'neq'`. `'lt'`, `'gt'`, `'leq'`, `'geq'`, `'in'`,
-`'notIn'`, `'like'`, `'between'`, `'not'` | `'eq'` | | `join_next_with` | The
-logical operator to join this filter with the next one | `'AND'`, `'OR'` |
-`'AND'` | > ð**Pro Tip:** Note You can apply either a list of filters or a
-single filter when filtering records. #### `ColumnValue` Class Just like the
-`Filter` class, `dataloom` also provides a `ColumnValue` class. This class acts
-as a setter to update the values of columns in your database table. The
-following code snippet demonstrates how the `ColumnValue` class is used to
-update records in the database: ```py re = pg_loom.update_one( Post, values=
-[ ColumnValue(name="title", value="Hey"), ColumnValue(name="completed",
-value=True), ], filters=[ Filter(column="id", value=1, join_next_with="AND"),
-Filter(column="userId", value=1, join_next_with="AND"), ], ) ``` It accepts two
-arguments: `name` and `value`. name represents the column name, while value
-corresponds to the new value to be assigned to that column. | Argument |
-Description | Type | Default | | -------- | -----------------------------------
------------------------ | ----- | ------- | | `name` | The name of the column
-to be updated or inserted. | `str` | - | | `value` | The value to assign to the
-column during update or insert. | `Any` | - | #### `Order` Class The `Order`
-class enables us to specify the desired order in which documents should be
-returned. Below is an example illustrating its usage: ```py posts =
-pg_loom.find_all( Post, select=["id", "completed", "title", "createdAt"],
-limit=3, offset=0, order=[ Order(column="createdAt", order="ASC"), Order
-(column="id", order="DESC"), ] ) ``` > ð**Pro Tip:** Note when utilizing a
-list of orders, they are applied sequentially, one after the other: | Argument
-| Description | Type | Default | | -------- | ---------------------------------
----------------------------------------- | ------------------- | ------- | |
-`column` | The name of the column to order by. | `str` | - | | `order` | The
-order direction, either `"ASC"` (ascending) or `"DESC"` (descending). | `"ASC"`
-or `"DESC"` | `"ASC"` | #### `Include` Class The `Include` class facilitates
-eager loading for models with relationships. Below is a table detailing the
-parameters available for the `Include` class: | Argument | Description | Type |
-Default | Required | | ---------------- | -------------------------------------
------------------------------------------------------- | ------------------- |
--------- | -------- | | `model` | The model to be included when eagerly
-fetching records. | `Model` | - | Yes | | `junction_table` | The
-`junction_table` model that is used as a reference table in a many to many
-association. | `Model` | `None` | No | | `order` | The list of order
-specifications for sorting the included data. | `list[Order]` | `[]` | No | |
-`limit` | The maximum number of records to include. | `int \| None` | `0` | No
-| | `offset` | The number of records to skip before including. | `int \| None`
-| `0` | No | | `select` | The list of columns to include. | `list[str] \| None`
-| `None` | No | | `has` | The relationship type between the current model and
-the included model. | `INCLUDE_LITERAL` | `"many"` | No | | `include` | The
-extra included models. | `list[Include]` | `[]` | No | | `alias` | The alias
-name for the included model. Very important when mapping self relations. |
-`str` | `None` | No | #### `Group` Class This class is used for data
+------------------------- | --------------- | ------- | | `type` | The datatype
+of your primary key. | `str` | `"int`" | | `length` | Optional to specify the
+length of the type. If passed as `N` with type `T`, it yields an SQL statement
+with type `T(N)`. | `int` \| `None` | `None` | | `auto_increment` | Optional to
+specify if the column will automatically increment or not. | `bool` | `False` |
+| `default` | Optional to specify the default value in a column. | `any` |
+`None` | | `nullable` | Optional to specify if the column will allow null
+values or not. | `bool` | `False` | | `unique` | Optional to specify if the
+column will contain unique values or not. | `bool` | `True` | ####
+`ForeignKeyColumn` Class This class is utilized when informing `dataloom` that
+a column has a relationship with a primary key in another table. Consider the
+following model definition of a `Post`: ```py class Post(Model): __tablename__:
+Optional[TableColumn] = TableColumn(name="posts") id = PrimaryKeyColumn
+(type="int", auto_increment=True, nullable=False, unique=True) completed =
+Column(type="boolean", default=False) title = Column(type="varchar",
+length=255, nullable=False) # timestamps createdAt = CreatedAtColumn()
+updatedAt = UpdatedAtColumn() # relations userId = ForeignKeyColumn( User,
+type="int", required=True, onDelete="CASCADE", onUpdate="CASCADE" ) ``` -
+`userId` is a foreign key in the table `posts`, indicating it has a
+relationship with a primary key in the `users` table. This column accepts the
+following arguments: | Argument | Description | Type | Default | | ---------- |
+-------------------------------------------------------------------------------
+------------------------------------- | ---------------------------------------
+- | ----------- | | `table` | Required. This is the parent table that the
+current model references. In our example, this is referred to as `User`. It can
+be used as a string in self relations. | `Model`\| `str` | | | `type` |
+Optional. Specifies the data type of the foreign key. If not provided, dataloom
+can infer it from the parent table. | `str` \| `None` | `None` | | `required` |
+Optional. Indicates whether the foreign key is required or not. | `bool` |
+`False` | | `onDelete` | Optional. Specifies the action to be taken when the
+associated record in the parent table is deleted. |`"NO ACTION"`, `"SET NULL"`,
+`"CASCADE"` | `"NO ACTION"` | | `onUpdate` | Optional. Specifies the action to
+be taken when the associated record in the parent table is updated. | `"NO
+ACTION"`, `"SET NULL"`, `"CASCADE"`| `"NO ACTION"` | It is crucial to specify
+the actions for `onDelete` and `onUpdate` to ensure that `dataloom` manages
+your model's relationship actions appropriately. The available actions are: 1.
+`"NO ACTION"` - If you delete or update the parent table, no changes will occur
+in the child table. 2. `"SET NULL"` - If you delete or update the parent table,
+the corresponding value in the child table will be set to `null`. 3.
+`"CASCADE"` - If you delete or update the table, the same action will also be
+applied to the child table. #### `CreatedAtColumn` Class When a column is
+designated as `CreatedAtColumn`, its value will be automatically generated each
+time you create a new record in a database, serving as a timestamp. ####
+`UpdatedAtColumn` Class When a column is designated as `UpdatedAtColumn`, its
+value will be automatically generated each time you create a new record or
+update an existing record in a database table, acting as a timestamp. ####
+`Filter` Class This `Filter` class in `dataloom` is designed to facilitate the
+application of filters when executing queries and mutations. It allows users to
+specify conditions that must be met for the operation to affect certain rows in
+a database table. Below is an example demonstrating how this class can be used:
+```python affected_rows = pg_loom.update_one( Post, values=[ ColumnValue
+(name="title", value="Hey"), ColumnValue(name="completed", value=True), ],
+filters=[ Filter(column="id", value=1, join_next_with="AND"), Filter
+(column="userId", value=1, join_next_with="AND"), ], ) ``` So from the above
+example we are applying filters while updating a `Post` here are the options
+that you can pass on that filter class: | Argument | Description | Type |
+Default | |-------------------------|------------------------------------------
+------------------|-------------------------------------------|----------------
+--------| | `column` | The name of the column to apply the filter on | `String`
+| - | | `value` | The value to filter against | `Any` | - | | `operator` | The
+comparison operator to use for the filter | `'eq'`, `'neq'`. `'lt'`, `'gt'`,
+`'leq'`, `'geq'`, `'in'`, `'notIn'`, `'like'`, `'between'`, `'not'` | `'eq'` |
+| `join_next_with` | The logical operator to join this filter with the next one
+| `'AND'`, `'OR'` | `'AND'` | > ð**Pro Tip:** Note You can apply either a
+list of filters or a single filter when filtering records. #### `ColumnValue`
+Class Just like the `Filter` class, `dataloom` also provides a `ColumnValue`
+class. This class acts as a setter to update the values of columns in your
+database table. The following code snippet demonstrates how the `ColumnValue`
+class is used to update records in the database: ```py re = pg_loom.update_one
+( Post, values=[ ColumnValue(name="title", value="Hey"), ColumnValue
+(name="completed", value=True), ], filters=[ Filter(column="id", value=1,
+join_next_with="AND"), Filter(column="userId", value=1, join_next_with="AND"),
+], ) ``` It accepts two arguments: `name` and `value`. name represents the
+column name, while value corresponds to the new value to be assigned to that
+column. | Argument | Description | Type | Default | | -------- | --------------
+-------------------------------------------- | ----- | ------- | | `name` | The
+name of the column to be updated or inserted. | `str` | - | | `value` | The
+value to assign to the column during update or insert. | `Any` | - | ####
+`Order` Class The `Order` class enables us to specify the desired order in
+which documents should be returned. Below is an example illustrating its usage:
+```py posts = pg_loom.find_all( Post, select=["id", "completed", "title",
+"createdAt"], limit=3, offset=0, order=[ Order(column="createdAt",
+order="ASC"), Order(column="id", order="DESC"), ] ) ``` > ð**Pro Tip:** Note
+when utilizing a list of orders, they are applied sequentially, one after the
+other: | Argument | Description | Type | Default | | -------- | ---------------
+---------------------------------------------------------- | ------------------
+- | ------- | | `column` | The name of the column to order by. | `str` | - | |
+`order` | The order direction, either `"ASC"` (ascending) or `"DESC"`
+(descending). | `"ASC"` or `"DESC"` | `"ASC"` | #### `Include` Class The
+`Include` class facilitates eager loading for models with relationships. Below
+is a table detailing the parameters available for the `Include` class: |
+Argument | Description | Type | Default | Required | | ---------------- | -----
+-------------------------------------------------------------------------------
+------- | ------------------- | -------- | -------- | | `model` | The model to
+be included when eagerly fetching records. | `Model` | - | Yes | |
+`junction_table` | The `junction_table` model that is used as a reference table
+in a many to many association. | `Model` | `None` | No | | `order` | The list
+of order specifications for sorting the included data. | `list[Order]` | `[]` |
+No | | `limit` | The maximum number of records to include. | `int \| None` |
+`0` | No | | `offset` | The number of records to skip before including. | `int
+\| None` | `0` | No | | `select` | The list of columns to include. | `list[str]
+\| None` | `None` | No | | `has` | The relationship type between the current
+model and the included model. | `INCLUDE_LITERAL` | `"many"` | No | | `include`
+| The extra included models. | `list[Include]` | `[]` | No | | `alias` | The
+alias name for the included model. Very important when mapping self relations.
+| `str` | `None` | No | #### `Group` Class This class is used for data
 `aggregation` and grouping data in `dataloom`. Below is a table detailing the
 parameters available for the `Group` class: | Argument | Description | Type |
 Default | Required | | --------------------------- | --------------------------
 ----------------------------- | --------------------------------------------- |
 --------- | -------- | | `column` | The name of the column to group by. | `str`
 | | Yes | | `function` | The aggregation function to apply on the grouped data.
 | `"COUNT" \| "AVG" \| "SUM" \| "MIN" \| "MAX"` | `"COUNT"` | No | | `having` |
@@ -446,72 +446,73 @@
 logs.sql", logging=True ) conn, tables = sqlite_loom.connect_and_sync([Post,
 User], drop=True, force=True) print(tables) if __name__ == "__main__":
 conn.close() ``` Returns a `conn` and the list of `tablenames` that exist in
 the database. The method accepts the same arguments as the `sync` method. ###
 CRUD Operations with Dataloom In this section of the documentation, we will
 illustrate how to perform basic `CRUD` operations using `dataloom` on simple
 `Models`. Please note that in the following code snippets, I will be utilizing
-`sqlite_loom`. However, it's important to highlight that you can use any `loom`
-of your choice to follow along. #### 1. Creating a Record To insert a single or
-multiple records in a database you make use of the following functions: 1.
-`insert_one()` 2. `insert_bulk()` ##### 1. `insert_one()` The `insert_one`
-method allows you to save a single row in a specific table. Upon saving, it
-will return the primary key (`pk`) value of the inserted document. The
-following example shows how the `insert_one()` method works. ```python #
-Example: Creating a user record userId = pg_loom.insert_one( instance=User,
-values=ColumnValue(name="username", value="@miller") ) userId =
-pg_loom.insert_one( instance=User, values=[ ColumnValue(name="username",
-value="@miller"), ColumnValue(name="name", value="Jonh"), ], ) ``` This
-function takes in two arguments which are `instance` and `values`. Where values
-are the column values that you are inserting in a user table or a single column
-value. | Argument | Description | `Type` | `Required` | `Default` | | ---------
-- | ---------------------------------------------------------------------------
---------------------------------- | ------------------------------------ | ----
------- | --------- | | `instance` | The instance of the table where the row
-will be inserted. | `Model` | `Yes` | `None` | | `values` | The column values
-to be inserted into the table. It can be a single column value or a list of
-column values. | `list[ColumnValue]` or `ColumnValue` | `Yes` | `None` | #####
-2. `insert_bulk()`. The `insert_bulk` method facilitates the bulk insertion of
-records, as its name suggests. The following example illustrates how you can
-add `3` posts to the database table simultaneously. ```python # Example:
-Inserting multiple posts rows = pg_loom.insert_bulk( User, values=[
+`sqlite_loom`, `mysql_loom`, `pg_loom` or `loom` interchangeably. However, it's
+important to highlight that you can use any `loom` of your choice to follow
+along. #### 1. Creating a Record To insert a single or multiple records in a
+database you make use of the following functions: 1. `insert_one()` 2.
+`insert_bulk()` ##### 1. `insert_one()` The `insert_one` method allows you to
+save a single row in a specific table. Upon saving, it will return the primary
+key (`pk`) value of the inserted document. The following example shows how the
+`insert_one()` method works. ```python # Example: Creating a user record userId
+= pg_loom.insert_one( instance=User, values=ColumnValue(name="username",
+value="@miller") ) userId = pg_loom.insert_one( instance=User, values=
 [ ColumnValue(name="username", value="@miller"), ColumnValue(name="name",
-value="Jonh"), ], [ ColumnValue(name="username", value="@brown"), ColumnValue
-(name="name", value="Jonh"), ], [ ColumnValue(name="username", value="@blue"),
-ColumnValue(name="name", value="Jonh"), ], ], ) ``` The argument parameters for
-the `insert_bulk` methods are as follows. | Argument | Description | `Type` |
-`Required` | `Default` | | ---------- | ---------------------------------------
--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
------- | ------------------------------------------ | ---------- | --------- |
-| `instance` | The instance of the table where the row will be inserted. |
+value="Jonh"), ], ) ``` This function takes in two arguments which are
+`instance` and `values`. Where values are the column values that you are
+inserting in a user table or a single column value. | Argument | Description |
+`Type` | `Required` | `Default` | | ---------- | ------------------------------
+-----------------------------------------------------------------------------
+- | ------------------------------------ | ---------- | --------- | |
+`instance` | The instance of the table where the row will be inserted. |
 `Model` | `Yes` | `None` | | `values` | The column values to be inserted into
-the table. **It must be a list of list of column values with the same length,
-otherwise dataloom will fail to map the values correctly during the insert
-operation.** | `list[list[ColumnValue]]` or `ColumnValue` | `Yes` | `None` | >
-In contrast to the `insert_one` method, the `insert_bulk` method returns the
-row count of the inserted documents rather than the individual primary keys
-(`pks`) of those documents. #### 2. Reading records To retrieve documents or a
-document from the database, you can make use of the following functions: 1.
-`find_all()`: This function is used to retrieve all documents from the
-database. 2. `find_by_pk()`: This function is used to retrieve a document by
-its primary key (or ID). 3. `find_one()`: This function is used to retrieve a
-single document based on a specific condition. 4. `find_many()`: This function
-is used to retrieve multiple documents based on a specific condition. ##### 1.
-`find_all()` This method is used to retrieve all the records that are in the
-database table. Below are examples demonstrating how to do it: ```py users =
-pg_loom.find_all( instance=User, select=["id", "username"], limit=3, offset=0,
-order=[Order(column="id", order="DESC")], ) print(users) # ? [{'id': 1,
-'username': '@miller'}] ``` The `find_all()` method takes in the following
-arguments: | Argument | Description | Type | Default | Required | | ---------
-- | ---------------------------------------------------------------------------
---------------- | ------------------------ | ------- | -------- | | `instance`
-| The model class to retrieve documents from. | `Model` | `None` | `Yes` | |
-`select` | Collection or a string of fields to select from the documents. |
-`list[str]\|str` | `None` | `No` | | `limit` | Maximum number of documents to
+the table. It can be a single column value or a list of column values. | `list
+[ColumnValue]` or `ColumnValue` | `Yes` | `None` | ##### 2. `insert_bulk()`.
+The `insert_bulk` method facilitates the bulk insertion of records, as its name
+suggests. The following example illustrates how you can add `3` posts to the
+database table simultaneously. ```python # Example: Inserting multiple posts
+rows = pg_loom.insert_bulk( User, values=[ [ ColumnValue(name="username",
+value="@miller"), ColumnValue(name="name", value="Jonh"), ], [ ColumnValue
+(name="username", value="@brown"), ColumnValue(name="name", value="Jonh"), ],
+[ ColumnValue(name="username", value="@blue"), ColumnValue(name="name",
+value="Jonh"), ], ], ) ``` The argument parameters for the `insert_bulk`
+methods are as follows. | Argument | Description | `Type` | `Required` |
+`Default` | | ---------- | ----------------------------------------------------
+-------------------------------------------------------------------------------
+------------------------------------------------------------------------ | ----
+-------------------------------------- | ---------- | --------- | | `instance`
+| The instance of the table where the row will be inserted. | `Model` | `Yes` |
+`None` | | `values` | The column values to be inserted into the table. **It
+must be a list of list of column values with the same length, otherwise
+dataloom will fail to map the values correctly during the insert operation.** |
+`list[list[ColumnValue]]` or `ColumnValue` | `Yes` | `None` | > In contrast to
+the `insert_one` method, the `insert_bulk` method returns the row count of the
+inserted documents rather than the individual primary keys (`pks`) of those
+documents. #### 2. Reading records To retrieve documents or a document from the
+database, you can make use of the following functions: 1. `find_all()`: This
+function is used to retrieve all documents from the database. 2. `find_by_pk
+()`: This function is used to retrieve a document by its primary key (or ID).
+3. `find_one()`: This function is used to retrieve a single document based on a
+specific condition. 4. `find_many()`: This function is used to retrieve
+multiple documents based on a specific condition. ##### 1. `find_all()` This
+method is used to retrieve all the records that are in the database table.
+Below are examples demonstrating how to do it: ```py users = pg_loom.find_all
+( instance=User, select=["id", "username"], limit=3, offset=0, order=[Order
+(column="id", order="DESC")], ) print(users) # ? [{'id': 1, 'username':
+'@miller'}] ``` The `find_all()` method takes in the following arguments: |
+Argument | Description | Type | Default | Required | | ---------- | -----------
+------------------------------------------------------------------------------
+- | ------------------------ | ------- | -------- | | `instance` | The model
+class to retrieve documents from. | `Model` | `None` | `Yes` | | `select` |
+Collection or a string of fields to select from the documents. | `list
+[str]\|str` | `None` | `No` | | `limit` | Maximum number of documents to
 retrieve. | `int` | `None` | `No` | | `offset` | Number of documents to skip
 before retrieving. | `int` | `0` | `No` | | `order` | Collection of `Order` or
 a single `Order` to order the documents when querying. | `list[Order]\|Order` |
 `None` | `No` | | `include` | Collection or a `Include` of related models to
 eagerly load. | `list[Include]\|Include` | `None` | `No` | | `group` |
 Collection of `Group` which specifies how you want your data to be grouped
 during queries. | `list[Group]\|Group` | `None` | `No` | | `distinct` | Boolean
@@ -539,15 +540,15 @@
 Collection of `Filter` or a `Filter` to apply to the query. | `list[Filter] \|
 Filter` | `None` | `No` | | `distinct` | Boolean telling dataloom to return
 distinct row values based on selected fields or not. | `bool` | `False` | `No`
 | > ð **Pro Tip**: The distinction between the `find_all()` and `find_many
 ()` methods lies in the fact that `find_many()` enables you to apply specific
 filters, whereas `find_all()` retrieves all the documents within the specified
 model. ##### 3. `find_one()` Here is an example showing you how you can use
-`find_by_pk()` locate a single record in the database. ```py user =
+`find_one()` locate a single record in the database. ```py user =
 mysql_loom.find_one( User, filters=[Filter(column="username",
 value="@miller")], select=["id", "username"], ) print(user) # ? {'id': 1,
 'username': '@miller'} ``` This method take the following as arguments |
 Argument | Description | Type | Default | Required | | ---------- | -----------
 ------------------------------------------------------------------------------
 - | -------------------------------- | ------- | -------- | | `instance` | The
 model class to retrieve instances from. | `Model` | | `Yes` | | `filters` |
@@ -646,174 +647,175 @@
 `delete_bulk()` function, exercise caution as it can be aggressive. If the
 filter is not explicitly provided, there is a risk of mistakenly deleting all
 records in the table. ###### Guidelines for Safe Usage To mitigate the
 potential risks associated with `delete_bulk()`, follow these guidelines: 1.
 **Always Provide a Filter:** - When calling `delete_bulk()`, make sure to
 provide a filter to specify the subset of records to be deleted. This helps
 prevent unintentional deletions. ```python # Example: Delete records where
-'status' is 'inactive' sqlite_loom.delete_bulk(filter={'status': 'inactive'})
-``` 2. **Consider Usage When Necessary:** - When contemplating data deletion,
-it is advisable to consider more targeted methods before resorting to
-`delete_bulk()`. Prioritize the use of `delete_one()` or `delete_by_pk()`
-methods to remove specific records based on your needs. This ensures a more
-precise and controlled approach to data deletion. 3. **Use limit and offsets
-options** - You can consider using the `limit` and offset options during
-invocation of `delete_bulk` ```py affected_rows = mysql_loom.delete_bulk
+'status' is 'inactive' affected_rows = mysql_loom.delete_bulk( instance=User,
+filters=Filter(column="status", value='inactive'), ) ``` 2. **Consider Usage
+When Necessary:** - When contemplating data deletion, it is advisable to
+consider more targeted methods before resorting to `delete_bulk()`. Prioritize
+the use of `delete_one()` or `delete_by_pk()` methods to remove specific
+records based on your needs. This ensures a more precise and controlled
+approach to data deletion. 3. **Use limit and offsets options** - You can
+consider using the `limit` and offset options during invocation of
+`delete_bulk` ```py affected_rows = mysql_loom.delete_bulk( instance=Post,
+order=[Order(column="id", order="DESC"), Order(column="createdAt",
+order="ASC")], filters=[Filter(column="id", operator="gt", value=0)], offset=0,
+limit=10, ) ``` By following these guidelines, you can use the `delete_bulk()`
+function safely and minimize the risk of unintended data loss. Always exercise
+caution and adhere to best practices when performing bulk deletion operations.
+### Ordering In dataloom you can order documents in either `DESC` (descending)
+or `ASC` (ascending) order using the helper class `Order`. ```py posts =
+mysql_loom.find_all( instance=Post, order=[Order(column="id", order="DESC")], )
+``` You can apply multiple and these orders will ba applied in sequence of
+application here is an example: ```py posts = mysql_loom.find_all
 ( instance=Post, order=[Order(column="id", order="DESC"), Order
-(column="createdAt", order="ASC")], filters=[Filter(column="id", operator="gt",
-value=0)], offset=0, limit=10, ) ``` By following these guidelines, you can use
-the `delete_bulk()` function safely and minimize the risk of unintended data
-loss. Always exercise caution and adhere to best practices when performing bulk
-deletion operations. ### Ordering In dataloom you can order documents in either
-`DESC` (descending) or `ASC` (ascending) order using the helper class `Order`.
-```py posts = mysql_loom.find_all( instance=Post, order=[Order(column="id",
-order="DESC")], ) ``` You can apply multiple and these orders will ba applied
-in sequence of application here is an example: ```py posts =
-mysql_loom.find_all( instance=Post, order=[Order(column="id", order="DESC"),
-Order(column="createdAt", order="ASC")], ) ``` ### Filters There are different
-find of filters that you can use when filtering documents for mutations and
-queries. Filters are very important to use when updating and deleting documents
-as they give you control on which documents should be updated or deleted. When
-doing a mutation you can use a single or multiple filters. Bellow is an example
-that shows you how you can use a single filter in deleting a single record that
-has an `id` greater than `1` from the database. ```py res2 =
-mysql_loom.delete_one( instance=Post, offset=0, order=Order(column="id",
-order="DESC"), filters=Filter(column="id", value=1, operator="gt"), ) ``` Or
-you can use it as follows: ```py res2 = mysql_loom.delete_one( instance=Post,
-offset=0, order=[Order(column="id", order="DESC")], filters=[Filter
-(column="id", value=1, operator="gt")], ) ``` As you have noticed, you can join
-your filters together and they will be applied sequentially using the
-[`join_next_with`](#filter-class) which can be either `OR` or `AND` te default
-value is `AND`. Here is an of filter usage in sequential. ```py res2 =
-mysql_loom.delete_one( instance=Post, offset=0, order=[Order(column="id",
-order="DESC")], filters=[ Filter(column="id", value=1, operator="gt"), Filter
-(column="userId", value=1, operator="eq", join_next_with="OR"), Filter
-( column="title", value='"What are you doing general?"', operator="=",
-join_next_with="AND", ), ], ) ``` ##### Operators You can use the `operator` to
-match the values. Here is the table of description for these filters. |
-Operator | Explanation | Expect | | ----------- | -----------------------------
-------------------------------------------------------------------------------
-- | --------------------- | | `'eq'` | Indicates equality. It checks if the
-value is equal to the specified criteria. | Value == Criteria | | `'lt'` |
-Denotes less than. It checks if the value is less than the specified criteria.
-| Value < Criteria | | `'gt'` | Denotes greater than. It checks if the value is
-greater than the specified criteria. | Value > Criteria | | `'leq'` | Denotes
-less than or equal to. It checks if the value is less than or equal to the
-specified criteria. | Value <= Criteria | | `'geq'` | Denotes greater than or
-equal to. It checks if the value is greater than or equal to the specified
-criteria. | Value >= Criteria | | `'in'` | Checks if the value is included in a
-specified list of values. | Value in List | | `'notIn'` | Checks if the value
-is not included in a specified list of values. | Value not in List | | `'like'`
-| Performs a pattern matching operation. It checks if the value is similar to a
-specified pattern. | Value matches Pattern | | `'not'` | Indicates non-
-equality. It checks if the column value that does not equal to the specified
-criteria. | NOT id = Criteria | | `'neq'` | Indicates non-equality. It checks
-if the value is not equal to the specified criteria. | Value != Criteria | |
-`'between'` | It checks range values that matches a given range between the
-minimum and maximum. | id BETWEEN (min, max) | Let's talk about these filters
-in detail of code by example. Let's say you want to update a `Post` where the
-`id` matches `1` you can do it as follows: ```py res2 = mysql_loom.update_one
-( instance=Post, filters=Filter( column="id", value=1, operator="eq", ),
-values=[ColumnValue(name="title", value="Bob")], ) ``` What if you want to
-update a post where `id` is not equal to `1` you can do it as follows ```py
+(column="createdAt", order="ASC")], ) ``` ### Filters There are different find
+of filters that you can use when filtering documents for mutations and queries.
+Filters are very important to use when updating and deleting documents as they
+give you control on which documents should be updated or deleted. When doing a
+mutation you can use a single or multiple filters. Bellow is an example that
+shows you how you can use a single filter in deleting a single record that has
+an `id` greater than `1` from the database. ```py res2 = mysql_loom.delete_one
+( instance=Post, offset=0, order=Order(column="id", order="DESC"),
+filters=Filter(column="id", value=1, operator="gt"), ) ``` Or you can use it as
+follows: ```py res2 = mysql_loom.delete_one( instance=Post, offset=0, order=
+[Order(column="id", order="DESC")], filters=[Filter(column="id", value=1,
+operator="gt")], ) ``` As you have noticed, you can join your filters together
+and they will be applied sequentially using the [`join_next_with`](#filter-
+class) which can be either `OR` or `AND` te default value is `AND`. Here is an
+of filter usage in sequential. ```py res2 = mysql_loom.delete_one
+( instance=Post, offset=0, order=[Order(column="id", order="DESC")], filters=
+[ Filter(column="id", value=1, operator="gt"), Filter(column="userId", value=1,
+operator="eq", join_next_with="OR"), Filter( column="title", value='"What are
+you doing general?"', operator="=", join_next_with="AND", ), ], ) ``` #####
+Operators You can use the `operator` to match the values. Here is the table of
+description for these filters. | Operator | Explanation | Expect | | ----------
+- | ---------------------------------------------------------------------------
+--------------------------------- | --------------------- | | `'eq'` |
+Indicates equality. It checks if the value is equal to the specified criteria.
+| Value == Criteria | | `'lt'` | Denotes less than. It checks if the value is
+less than the specified criteria. | Value < Criteria | | `'gt'` | Denotes
+greater than. It checks if the value is greater than the specified criteria. |
+Value > Criteria | | `'leq'` | Denotes less than or equal to. It checks if the
+value is less than or equal to the specified criteria. | Value <= Criteria | |
+`'geq'` | Denotes greater than or equal to. It checks if the value is greater
+than or equal to the specified criteria. | Value >= Criteria | | `'in'` |
+Checks if the value is included in a specified list of values. | Value in List
+| | `'notIn'` | Checks if the value is not included in a specified list of
+values. | Value not in List | | `'like'` | Performs a pattern matching
+operation. It checks if the value is similar to a specified pattern. | Value
+matches Pattern | | `'not'` | Indicates non-equality. It checks if the column
+value that does not equal to the specified criteria. | NOT id = Criteria | |
+`'neq'` | Indicates non-equality. It checks if the value is not equal to the
+specified criteria. | Value != Criteria | | `'between'` | It checks range
+values that matches a given range between the minimum and maximum. | id BETWEEN
+(min, max) | Let's talk about these filters in detail of code by example. Let's
+say you want to update a `Post` where the `id` matches `1` you can do it as
+follows: ```py res2 = mysql_loom.update_one( instance=Post, filters=Filter
+( column="id", value=1, operator="eq", ), values=[ColumnValue(name="title",
+value="Bob")], ) ``` What if you want to update a post where `id` is not equal
+to `1` you can do it as follows ```py res2 = mysql_loom.update_bulk
+( instance=Post, filters=Filter( column="id", value=1, operator="neq", ),
+values=[ColumnValue(name="title", value="Bob")], ) ``` What if i want to update
+the records that have an `id` less than `3`? ```py res2 =
+mysql_loom.update_bulk( instance=Post, filters=Filter( column="id", value=3,
+operator="lt", ), values=[ColumnValue(name="title", value="Bob")], ) ``` What
+if i want to update the records that have an `id` less than or equal `3`? ```py
 res2 = mysql_loom.update_bulk( instance=Post, filters=Filter( column="id",
 value=1, operator="neq", ), values=[ColumnValue(name="title", value="Bob")], )
-``` What if i want to update the records that have an `id` less than `3`? ```py
-res2 = mysql_loom.update_bulk( instance=Post, filters=Filter( column="id",
-value=3, operator="lt", ), values=[ColumnValue(name="title", value="Bob")], )
-``` What if i want to update the records that have an `id` less than or equal
-`3`? ```py res2 = mysql_loom.update_bulk( instance=Post, filters=Filter
-( column="id", value=1, operator="neq", ), values=[ColumnValue(name="title",
-value="Bob")], ) ``` What if i want to update the records that have an `id`
-greater than `3`? ```py res = mysql_loom.update_bulk( instance=Post,
-filters=Filter( column="id", value=3, operator="gt", ), values=[ColumnValue
-(name="title", value="Bob")], ) ``` What if i want to update the records that
-have an `id` greater or equal to `3`? ```py res = mysql_loom.update_bulk
-( instance=Post, filters=Filter( column="id", value=3, operator="geq", ),
-values=[ColumnValue(name="title", value="Bob")], ) ``` You can use the `in` to
-update or query records that matches values in a specified `list` of values or
-`tuple`. Here is an example showing you how you can update records that does
-matches `id` in `[1, 2]`. ```py res = mysql_loom.update_bulk( instance=Post,
-filters=Filter( column="id", value=[1, 2], operator="in", ), values=
-[ColumnValue(name="title", value="Bob")], ) ``` You can use the `notIn` to
-update or query records that does not matches values in a specified `list` of
-values or `tuple`. Here is an example showing you how you can update records
-that does not matches `id` in `[1, 2]`. ```py res = mysql_loom.update_bulk
-( instance=Post, filters=Filter( column="id", value=[1, 2], operator="notIn",
-), values=[ColumnValue(name="title", value="Bob")], ) ``` You can use the
-`like` operator to match some patens in your query filters. Let's say we want
-to match a post that has the title ends with `general` we can use the `like`
-operator as follows ```py general = mysql_loom.find_one( instance=Post,
-filters=Filter( column="title", value="% general?", operator="like", ), select=
-["id", "title"], ) print(general) # ? {'id': 1, 'title': 'What are you doing
-general?'} ``` The following table show you some expression that you can use
-with this `like` operator. | Value | Description | | -------------- | ---------
+``` What if i want to update the records that have an `id` greater than `3`?
+```py res = mysql_loom.update_bulk( instance=Post, filters=Filter( column="id",
+value=3, operator="gt", ), values=[ColumnValue(name="title", value="Bob")], )
+``` What if i want to update the records that have an `id` greater or equal to
+`3`? ```py res = mysql_loom.update_bulk( instance=Post, filters=Filter
+( column="id", value=3, operator="geq", ), values=[ColumnValue(name="title",
+value="Bob")], ) ``` You can use the `in` to update or query records that
+matches values in a specified `list` of values or `tuple`. Here is an example
+showing you how you can update records that does matches `id` in `[1, 2]`.
+```py res = mysql_loom.update_bulk( instance=Post, filters=Filter( column="id",
+value=[1, 2], operator="in", ), values=[ColumnValue(name="title",
+value="Bob")], ) ``` You can use the `notIn` to update or query records that
+does not matches values in a specified `list` of values or `tuple`. Here is an
+example showing you how you can update records that does not matches `id` in `
+[1, 2]`. ```py res = mysql_loom.update_bulk( instance=Post, filters=Filter
+( column="id", value=[1, 2], operator="notIn", ), values=[ColumnValue
+(name="title", value="Bob")], ) ``` You can use the `like` operator to match
+some patens in your query filters. Let's say we want to match a post that has
+the title ends with `general` we can use the `like` operator as follows ```py
+general = mysql_loom.find_one( instance=Post, filters=Filter( column="title",
+value="% general?", operator="like", ), select=["id", "title"], ) print
+(general) # ? {'id': 1, 'title': 'What are you doing general?'} ``` The
+following table show you some expression that you can use with this `like`
+operator. | Value | Description | | -------------- | --------------------------
 -------------------------------------------------------------------------------
--------------------------------- | | `%pattern` | Finds values that end with
-the specified pattern. | | `pattern%` | Finds values that start with the
-specified pattern. | | `%pattern%` | Finds values that contain the specified
-pattern anywhere within the string. | | `_pattern` | Finds values that have any
-single character followed by the specified pattern. | | `pattern_` | Finds
-values that have the specified pattern followed by any single character. | | `
-[charlist]%` | Finds values that start with any character in the specified
-character list. | | `[!charlist]%` | Finds values that start with any character
-not in the specified character list. | | `_pattern_` | Finds values that have
-any single character followed by the specified pattern and then followed by any
-single character. | ### Data Aggregation With the [`Having`](#having-class) and
-the [`Group`](#group-class) classes you can perform some powerful powerful
-queries. In this section we are going to demonstrate an example of how we can
-do the aggregate queries. ```py posts = mysql_loom.find_many( Post,
-select="id", filters=Filter(column="id", operator="gt", value=1), group=Group
-( column="id", function="MAX", having=Having(column="id", operator="in", value=
-(2, 3, 4)), return_aggregation_column=True, ), ) ``` The following will be the
-output from the above query. ```shell [{'id': 2, 'MAX(`id`)': 2}, {'id': 3,
-'MAX(`id`)': 3}, {'id': 4, 'MAX(`id`)': 4}] ``` However you can remove the
-aggregation column from the above query by specifying the
-`return_aggregation_column` to be `False`: ```py posts = mysql_loom.find_many
-( Post, select="id", filters=Filter(column="id", operator="gt", value=1),
-group=Group( column="id", function="MAX", having=Having(column="id",
-operator="in", value=(2, 3, 4)), return_aggregation_column=False, ), ) print
-(posts) ``` This will output: ```shell [{'id': 2}, {'id': 3}, {'id': 4}] ```
-#### Aggregation Functions You can use the following aggregation functions that
-dataloom supports: | Aggregation Function | Description | | -------------------
-- | ------------------------------------------------ | | `"AVG"` | Computes the
-average of the values in the group. | | `"COUNT"` | Counts the number of items
-in the group. | | `"SUM"` | Computes the sum of the values in the group. | |
-`"MAX"` | Retrieves the maximum value in the group. | | `"MIN"` | Retrieves the
-minimum value in the group. | > ð **Pro Tip**: Note that data aggregation
-only works without `eager` loading and also works only with [`find_may()`](#2-
-find_many) and [`find_all()`](#1-find_all) in dataloom. ### Utilities Dataloom
-comes up with some utility functions that works on an instance of a model. This
-is very useful when debuging your tables to see how do they look like. These
-function include: #### 1. `inspect()` This function takes in a model as
-argument and inspect the model fields or columns. The following examples show
-how we can use this handy function in inspecting table names. ```py table =
-mysql_loom.inspect(instance=User, fields=["name", "type"], print_table=False)
-print(table) ``` The above snippet returns a list of dictionaries containing
-the column name and the arguments that were passed. ```shell [{'id': {'type':
-'int'}}, {'name': {'type': 'varchar'}}, {'tokenVersion': {'type': 'int'}},
-{'username': {'type': 'varchar'}}] ``` You can print table format these fields
-with their types as follows ```py mysql_loom.inspect(instance=User) ``` Output:
-```shell +--------------+---------+----------+---------+ | name | type |
-nullable | default | +--------------+---------+----------+---------+ | id | int
-| NO | None | | name | varchar | NO | Bob | | tokenVersion | int | YES | 0 | |
-username | varchar | YES | None | +--------------+---------+----------+--------
--+ ``` The `inspect` function take the following arguments. | Argument |
-Description | Type | Default | Required | | ------------- | -------------------
------------------------------------ | ----------- | ---------------------------
--------------- | -------- | | `instance` | The model instance to inspect. |
-`Model` | - | Yes | | `fields` | The list of fields to include in the
-inspection. | `list[str]` | `["name", "type", "nullable", "default"]` | No | |
-`print_table` | Flag indicating whether to print the inspection table. | `bool`
-| `True` | No | #### 2. `decorators` These modules contain several decorators
-that can prove useful when creating models. These decorators originate from
-`dataloom.decorators`, and at this stage, we are referring to them as
-"experimental." ##### `@initialize()` Let's examine a model named `Profile`,
-which appears as follows: ```py class Profile(Model): __tablename__: Optional
-[TableColumn] = TableColumn(name="profiles") id = PrimaryKeyColumn(type="int",
+--------------- | | `%pattern` | Finds values that end with the specified
+pattern. | | `pattern%` | Finds values that start with the specified pattern. |
+| `%pattern%` | Finds values that contain the specified pattern anywhere within
+the string. | | `_pattern` | Finds values that have any single character
+followed by the specified pattern. | | `pattern_` | Finds values that have the
+specified pattern followed by any single character. | | `[charlist]%` | Finds
+values that start with any character in the specified character list. | | `
+[!charlist]%` | Finds values that start with any character not in the specified
+character list. | | `_pattern_` | Finds values that have any single character
+followed by the specified pattern and then followed by any single character. |
+### Data Aggregation With the [`Having`](#having-class) and the [`Group`]
+(#group-class) classes you can perform some powerful powerful queries. In this
+section we are going to demonstrate an example of how we can do the aggregate
+queries. ```py posts = mysql_loom.find_many( Post, select="id", filters=Filter
+(column="id", operator="gt", value=1), group=Group( column="id",
+function="MAX", having=Having(column="id", operator="in", value=(2, 3, 4)),
+return_aggregation_column=True, ), ) ``` The following will be the output from
+the above query. ```shell [{'id': 2, 'MAX(`id`)': 2}, {'id': 3, 'MAX(`id`)':
+3}, {'id': 4, 'MAX(`id`)': 4}] ``` However you can remove the aggregation
+column from the above query by specifying the `return_aggregation_column` to be
+`False`: ```py posts = mysql_loom.find_many( Post, select="id", filters=Filter
+(column="id", operator="gt", value=1), group=Group( column="id",
+function="MAX", having=Having(column="id", operator="in", value=(2, 3, 4)),
+return_aggregation_column=False, ), ) print(posts) ``` This will output:
+```shell [{'id': 2}, {'id': 3}, {'id': 4}] ``` #### Aggregation Functions You
+can use the following aggregation functions that dataloom supports: |
+Aggregation Function | Description | | -------------------- | -----------------
+------------------------------- | | `"AVG"` | Computes the average of the
+values in the group. | | `"COUNT"` | Counts the number of items in the group. |
+| `"SUM"` | Computes the sum of the values in the group. | | `"MAX"` |
+Retrieves the maximum value in the group. | | `"MIN"` | Retrieves the minimum
+value in the group. | > ð **Pro Tip**: Note that data aggregation only works
+without `eager` loading and also works only with [`find_may()`](#2-find_many)
+and [`find_all()`](#1-find_all) in dataloom. ### Utilities Dataloom comes up
+with some utility functions that works on an instance of a model. This is very
+useful when debuging your tables to see how do they look like. These function
+include: #### 1. `inspect()` This function takes in a model as argument and
+inspect the model fields or columns. The following examples show how we can use
+this handy function in inspecting table names. ```py table = mysql_loom.inspect
+(instance=User, fields=["name", "type"], print_table=False) print(table) ```
+The above snippet returns a list of dictionaries containing the column name and
+the arguments that were passed. ```shell [{'id': {'type': 'int'}}, {'name':
+{'type': 'varchar'}}, {'tokenVersion': {'type': 'int'}}, {'username': {'type':
+'varchar'}}] ``` You can print table format these fields with their types as
+follows ```py mysql_loom.inspect(instance=User) ``` Output: ```shell +---------
+-----+---------+----------+---------+ | name | type | nullable | default | +---
+-----------+---------+----------+---------+ | id | int | NO | None | | name |
+varchar | NO | Bob | | tokenVersion | int | YES | 0 | | username | varchar |
+YES | None | +--------------+---------+----------+---------+ ``` The `inspect`
+function take the following arguments. | Argument | Description | Type |
+Default | Required | | ------------- | ----------------------------------------
+-------------- | ----------- | ----------------------------------------- | ----
+---- | | `instance` | The model instance to inspect. | `Model` | - | Yes | |
+`fields` | The list of fields to include in the inspection. | `list[str]` | `
+["name", "type", "nullable", "default"]` | No | | `print_table` | Flag
+indicating whether to print the inspection table. | `bool` | `True` | No | ####
+2. `decorators` These modules contain several decorators that can prove useful
+when creating models. These decorators originate from `dataloom.decorators`,
+and at this stage, we are referring to them as "experimental." #####
+`@initialize()` Let's examine a model named `Profile`, which appears as
+follows: ```py class Profile(Model): __tablename__: Optional[TableColumn] =
+TableColumn(name="profiles") id = PrimaryKeyColumn(type="int",
 auto_increment=True) avatar = Column(type="text", nullable=False) userId =
 ForeignKeyColumn( User, maps_to="1-1", type="int", required=True,
 onDelete="CASCADE", onUpdate="CASCADE", ) ``` This is simply a Python class
 that inherits from the top-level class `Model`. However, it lacks some useful
 `dunder` methods such as `__init__` and `__repr__`. In standard Python, we can
 achieve this functionality by using `dataclasses`. For example, we can modify
 our class as follows: ```py from dataclasses import dataclass @dataclass class
@@ -1357,11 +1359,13 @@
 don't want logging at all. | `int` | No | `1` | | `is_script` | Whether the SQL
 is a script. | `bool` | No | `False` | #### Why Use Query Builder? - The query
 builder empowers developers to seamlessly execute `SQL` queries directly. -
 While Dataloom primarily utilizes `subqueries` for eager data fetching on
 models, developers may prefer to employ JOIN operations, which are achievable
 through the `qb` object. ```python qb = loom.getQueryBuilder() result = qb.run
 ("SELECT * FROM table1 INNER JOIN table2 ON table1.id = table2.table1_id;")
-print(result) ``` ### Contributing Contributions to `dataloom` are welcome!
-Feel free to submit bug reports, feature requests, or pull requests on [GitHub]
-(https://github.com/CrispenGari/dataloom). ### License This project is licensed
-under the MIT License - see the [LICENSE](/LISENSE) file for details.
+print(result) ``` ### Documentation You can read the full documentation of
+dataloom on [readthedocs.io](https://dataloom-py.readthedocs.io/en/latest/) ###
+Contributing Contributions to `dataloom` are welcome! Feel free to submit bug
+reports, feature requests, or pull requests on [GitHub](https://github.com/
+CrispenGari/dataloom). ### License This project is licensed under the MIT
+License - see the [LICENSE](/LISENSE) file for details.
```

### Comparing `dataloom-2.4.1/README.md` & `dataloom-2.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     - [Inserting](#inserting-3)
     - [Retrieving Records](#retrieving-records-3)
   - [6. `N-N` Relationship](#6-n-n-relationship)
     - [Inserting](#inserting-4)
     - [Retrieving Records](#retrieving-records-4)
 - [Query Builder.](#query-builder)
   - [Why Use Query Builder?](#why-use-query-builder)
+- [Documentation](#documentation)
 - [Contributing](#contributing)
 - [License](#license)
 
 ### Key Features:
 
 - **Lightweight**: `dataloom` is designed to be minimalistic and easy to use, ensuring a streamlined `ORM` experience without unnecessary complexities.
 
@@ -481,22 +482,23 @@
     __tablename__: Optional[TableColumn] = TableColumn(name="users")
     id = PrimaryKeyColumn(type="int", auto_increment=True)
     #...rest of your columns
 
 ```
 
 The following are the arguments that the `PrimaryKeyColumn` class accepts.
-| Argument | Description | Type | Default |
-| ---------------- | ------------------------------------------------------------------------------------------------------------------------ | --------------- | ------------- |
-| `type` | The datatype of your primary key. | `str` | `"int`" |
-| `length` | Optional to specify the length of the type. If passed as `N` with type `T`, it yields an SQL statement with type `T(N)`. | `int` \| `None` | `None` |
-| `auto_increment`| Optional to specify if the column will automatically increment or not. |`bool` |`False` |
-|`default` | Optional to specify the default value in a column. |`any` |`None` |
-|`nullable` | Optional to specify if the column will allow null values or not. |`bool` |`False` |
-|`unique` | Optional to specify if the column will contain unique values or not. |`bool` |`True` |
+
+| Argument         | Description                                                                                                              | Type            | Default |
+| ---------------- | ------------------------------------------------------------------------------------------------------------------------ | --------------- | ------- |
+| `type`           | The datatype of your primary key.                                                                                        | `str`           | `"int`" |
+| `length`         | Optional to specify the length of the type. If passed as `N` with type `T`, it yields an SQL statement with type `T(N)`. | `int` \| `None` | `None`  |
+| `auto_increment` | Optional to specify if the column will automatically increment or not.                                                   | `bool`          | `False` |
+| `default`        | Optional to specify the default value in a column.                                                                       | `any`           | `None`  |
+| `nullable`       | Optional to specify if the column will allow null values or not.                                                         | `bool`          | `False` |
+| `unique`         | Optional to specify if the column will contain unique values or not.                                                     | `bool`          | `True`  |
 
 #### `ForeignKeyColumn` Class
 
 This class is utilized when informing `dataloom` that a column has a relationship with a primary key in another table. Consider the following model definition of a `Post`:
 
 ```py
 class Post(Model):
@@ -699,15 +701,15 @@
     conn.close()
 ```
 
 Returns a `conn` and the list of `tablenames` that exist in the database. The method accepts the same arguments as the `sync` method.
 
 ### CRUD Operations with Dataloom
 
-In this section of the documentation, we will illustrate how to perform basic `CRUD` operations using `dataloom` on simple `Models`. Please note that in the following code snippets, I will be utilizing `sqlite_loom`. However, it's important to highlight that you can use any `loom` of your choice to follow along.
+In this section of the documentation, we will illustrate how to perform basic `CRUD` operations using `dataloom` on simple `Models`. Please note that in the following code snippets, I will be utilizing `sqlite_loom`, `mysql_loom`, `pg_loom` or `loom` interchangeably. However, it's important to highlight that you can use any `loom` of your choice to follow along.
 
 #### 1. Creating a Record
 
 To insert a single or multiple records in a database you make use of the following functions:
 
 1. `insert_one()`
 2. `insert_bulk()`
@@ -841,15 +843,15 @@
 | `filters`  | Collection of `Filter` or a `Filter` to apply to the query.                                | `list[Filter] \| Filter` | `None`  | `No`     |
 | `distinct` | Boolean telling dataloom to return distinct row values based on selected fields or not.    | `bool`                   | `False` | `No`     |
 
 > 👍 **Pro Tip**: The distinction between the `find_all()` and `find_many()` methods lies in the fact that `find_many()` enables you to apply specific filters, whereas `find_all()` retrieves all the documents within the specified model.
 
 ##### 3. `find_one()`
 
-Here is an example showing you how you can use `find_by_pk()` locate a single record in the database.
+Here is an example showing you how you can use `find_one()` locate a single record in the database.
 
 ```py
 user = mysql_loom.find_one(
     User,
     filters=[Filter(column="username", value="@miller")],
     select=["id", "username"],
 )
@@ -1035,16 +1037,19 @@
 To mitigate the potential risks associated with `delete_bulk()`, follow these guidelines:
 
 1. **Always Provide a Filter:**
 
    - When calling `delete_bulk()`, make sure to provide a filter to specify the subset of records to be deleted. This helps prevent unintentional deletions.
 
    ```python
-   # Example: Delete records where 'status' is 'inactive'
-   sqlite_loom.delete_bulk(filter={'status': 'inactive'})
+    # Example: Delete records where 'status' is 'inactive'
+    affected_rows = mysql_loom.delete_bulk(
+        instance=User,
+        filters=Filter(column="status",  value='inactive'),
+    )
    ```
 
 2. **Consider Usage When Necessary:**
 
 - When contemplating data deletion, it is advisable to consider more targeted methods before resorting to `delete_bulk()`. Prioritize the use of `delete_one()` or `delete_by_pk()` methods to remove specific records based on your needs. This ensures a more precise and controlled approach to data deletion.
 
 3. **Use limit and offsets options**
@@ -2475,14 +2480,18 @@
 
   ```python
   qb = loom.getQueryBuilder()
   result = qb.run("SELECT * FROM table1 INNER JOIN table2 ON table1.id = table2.table1_id;")
   print(result)
   ```
 
+### Documentation
+
+You can read the full documentation of dataloom on [readthedocs.io](https://dataloom-py.readthedocs.io/en/latest/)
+
 ### Contributing
 
 Contributions to `dataloom` are welcome! Feel free to submit bug reports, feature requests, or pull requests on [GitHub](https://github.com/CrispenGari/dataloom).
 
 ### License
 
 This project is licensed under the MIT License - see the [LICENSE](/LISENSE) file for details.
```

#### html2text {}

```diff
@@ -59,38 +59,39 @@
 [Inserting](#inserting-2) - [Retrieving Records](#retrieving-records-2) - [4.
 What about bidirectional queries?](#4-what-about-bidirectional-queries) - [1.
 Child to Parent](#1-child-to-parent) - [2. Parent to Child](#2-parent-to-child)
 - [5. `Self` Association](#5-self-association) - [Inserting](#inserting-3) -
 [Retrieving Records](#retrieving-records-3) - [6. `N-N` Relationship](#6-n-n-
 relationship) - [Inserting](#inserting-4) - [Retrieving Records](#retrieving-
 records-4) - [Query Builder.](#query-builder) - [Why Use Query Builder?](#why-
-use-query-builder) - [Contributing](#contributing) - [License](#license) ###
-Key Features: - **Lightweight**: `dataloom` is designed to be minimalistic and
-easy to use, ensuring a streamlined `ORM` experience without unnecessary
-complexities. - **Database Support**: `dataloom` supports popular relational
-databases such as `PostgreSQL`, `MySQL`, and `SQLite3`, making it suitable for
-a variety of projects. - **Simplified Querying**: The `ORM` simplifies the
-process of database querying, allowing developers to interact with the database
-using Python classes and methods rather than raw SQL queries. - **Intuitive
-Syntax**: `dataloom`'s syntax is intuitive and `Pythonic`, making it accessible
-for developers familiar with the Python language. - **Flexible Data Types**:
-The `ORM` seamlessly handles various data types, offering flexibility in
-designing database schemas. ### Installation To install `dataloom`, you just
-need to run the following command using `pip`: ```bash pip install dataloom ```
-### Python Version Compatibility `dataloom` supports **`Python`** version
-**`3.12`** and above. Ensure that you are using a compatible version of
-**`Python`** before installing or using `dataloom`. You can check your
-**`Python`** version by running: ```bash python --version ``` ### Usage In this
-section we are going to go through how you can use our `orm` package in your
-project. ### Connection To use Dataloom, you need to establish a connection
-with a specific database `dialect`. The available dialect options are `mysql`,
-`postgres`, and `sqlite`. #### `Postgres` The following is an example of how
-you can establish a connection with postgres database. ```python from dataloom
-import Loom # Create a Loom instance with PostgreSQL configuration pg_loom =
-Loom( dialect="postgres", database="hi", password="root", user="postgres",
+use-query-builder) - [Documentation](#documentation) - [Contributing]
+(#contributing) - [License](#license) ### Key Features: - **Lightweight**:
+`dataloom` is designed to be minimalistic and easy to use, ensuring a
+streamlined `ORM` experience without unnecessary complexities. - **Database
+Support**: `dataloom` supports popular relational databases such as
+`PostgreSQL`, `MySQL`, and `SQLite3`, making it suitable for a variety of
+projects. - **Simplified Querying**: The `ORM` simplifies the process of
+database querying, allowing developers to interact with the database using
+Python classes and methods rather than raw SQL queries. - **Intuitive Syntax**:
+`dataloom`'s syntax is intuitive and `Pythonic`, making it accessible for
+developers familiar with the Python language. - **Flexible Data Types**: The
+`ORM` seamlessly handles various data types, offering flexibility in designing
+database schemas. ### Installation To install `dataloom`, you just need to run
+the following command using `pip`: ```bash pip install dataloom ``` ### Python
+Version Compatibility `dataloom` supports **`Python`** version **`3.12`** and
+above. Ensure that you are using a compatible version of **`Python`** before
+installing or using `dataloom`. You can check your **`Python`** version by
+running: ```bash python --version ``` ### Usage In this section we are going to
+go through how you can use our `orm` package in your project. ### Connection To
+use Dataloom, you need to establish a connection with a specific database
+`dialect`. The available dialect options are `mysql`, `postgres`, and `sqlite`.
+#### `Postgres` The following is an example of how you can establish a
+connection with postgres database. ```python from dataloom import Loom # Create
+a Loom instance with PostgreSQL configuration pg_loom = Loom
+( dialect="postgres", database="hi", password="root", user="postgres",
 host="localhost", sql_logger="console", logs_filename="logs.sql", port=5432, )
 # Connect to the PostgreSQL database conn = pg_loom.connect() # Close the
 connection when the script completes if __name__ == "__main__": conn.close()
 ``` In `dataloom` you can use connection uris to establish a connection to the
 database in `postgres` as follows: ```py pg_loom = Loom( dialect="postgres",
 connection_uri = "postgressql://root:root@localhost:5432/hi", # ... ) ``` This
 will establish a connection with `postgres` with the database `hi`. ####
@@ -250,121 +251,120 @@
 `PrimaryKeyColumn` is required. Below is an example of creating an `id` column
 as a primary key in a table named `Post`: ```python class Post(Model):
 __tablename__: Optional[TableColumn] = TableColumn(name="users") id =
 PrimaryKeyColumn(type="int", auto_increment=True) #...rest of your columns ```
 The following are the arguments that the `PrimaryKeyColumn` class accepts. |
 Argument | Description | Type | Default | | ---------------- | ----------------
 -------------------------------------------------------------------------------
-------------------------- | --------------- | ------------- | | `type` | The
-datatype of your primary key. | `str` | `"int`" | | `length` | Optional to
-specify the length of the type. If passed as `N` with type `T`, it yields an
-SQL statement with type `T(N)`. | `int` \| `None` | `None` | |
-`auto_increment`| Optional to specify if the column will automatically
-increment or not. |`bool` |`False` | |`default` | Optional to specify the
-default value in a column. |`any` |`None` | |`nullable` | Optional to specify
-if the column will allow null values or not. |`bool` |`False` | |`unique` |
-Optional to specify if the column will contain unique values or not. |`bool`
-|`True` | #### `ForeignKeyColumn` Class This class is utilized when informing
-`dataloom` that a column has a relationship with a primary key in another
-table. Consider the following model definition of a `Post`: ```py class Post
-(Model): __tablename__: Optional[TableColumn] = TableColumn(name="posts") id =
-PrimaryKeyColumn(type="int", auto_increment=True, nullable=False, unique=True)
-completed = Column(type="boolean", default=False) title = Column
-(type="varchar", length=255, nullable=False) # timestamps createdAt =
-CreatedAtColumn() updatedAt = UpdatedAtColumn() # relations userId =
-ForeignKeyColumn( User, type="int", required=True, onDelete="CASCADE",
-onUpdate="CASCADE" ) ``` - `userId` is a foreign key in the table `posts`,
-indicating it has a relationship with a primary key in the `users` table. This
-column accepts the following arguments: | Argument | Description | Type |
-Default | | ---------- | ------------------------------------------------------
--------------------------------------------------------------- | --------------
--------------------------- | ----------- | | `table` | Required. This is the
-parent table that the current model references. In our example, this is
-referred to as `User`. It can be used as a string in self relations. |
-`Model`\| `str` | | | `type` | Optional. Specifies the data type of the foreign
-key. If not provided, dataloom can infer it from the parent table. | `str` \|
-`None` | `None` | | `required` | Optional. Indicates whether the foreign key is
-required or not. | `bool` | `False` | | `onDelete` | Optional. Specifies the
-action to be taken when the associated record in the parent table is deleted.
-|`"NO ACTION"`, `"SET NULL"`, `"CASCADE"` | `"NO ACTION"` | | `onUpdate` |
-Optional. Specifies the action to be taken when the associated record in the
-parent table is updated. | `"NO ACTION"`, `"SET NULL"`, `"CASCADE"`| `"NO
-ACTION"` | It is crucial to specify the actions for `onDelete` and `onUpdate`
-to ensure that `dataloom` manages your model's relationship actions
-appropriately. The available actions are: 1. `"NO ACTION"` - If you delete or
-update the parent table, no changes will occur in the child table. 2. `"SET
-NULL"` - If you delete or update the parent table, the corresponding value in
-the child table will be set to `null`. 3. `"CASCADE"` - If you delete or update
-the table, the same action will also be applied to the child table. ####
-`CreatedAtColumn` Class When a column is designated as `CreatedAtColumn`, its
-value will be automatically generated each time you create a new record in a
-database, serving as a timestamp. #### `UpdatedAtColumn` Class When a column is
-designated as `UpdatedAtColumn`, its value will be automatically generated each
-time you create a new record or update an existing record in a database table,
-acting as a timestamp. #### `Filter` Class This `Filter` class in `dataloom` is
-designed to facilitate the application of filters when executing queries and
-mutations. It allows users to specify conditions that must be met for the
-operation to affect certain rows in a database table. Below is an example
-demonstrating how this class can be used: ```python affected_rows =
-pg_loom.update_one( Post, values=[ ColumnValue(name="title", value="Hey"),
-ColumnValue(name="completed", value=True), ], filters=[ Filter(column="id",
-value=1, join_next_with="AND"), Filter(column="userId", value=1,
-join_next_with="AND"), ], ) ``` So from the above example we are applying
-filters while updating a `Post` here are the options that you can pass on that
-filter class: | Argument | Description | Type | Default | |--------------------
------|------------------------------------------------------------|------------
--------------------------------|------------------------| | `column` | The name
-of the column to apply the filter on | `String` | - | | `value` | The value to
-filter against | `Any` | - | | `operator` | The comparison operator to use for
-the filter | `'eq'`, `'neq'`. `'lt'`, `'gt'`, `'leq'`, `'geq'`, `'in'`,
-`'notIn'`, `'like'`, `'between'`, `'not'` | `'eq'` | | `join_next_with` | The
-logical operator to join this filter with the next one | `'AND'`, `'OR'` |
-`'AND'` | > ð**Pro Tip:** Note You can apply either a list of filters or a
-single filter when filtering records. #### `ColumnValue` Class Just like the
-`Filter` class, `dataloom` also provides a `ColumnValue` class. This class acts
-as a setter to update the values of columns in your database table. The
-following code snippet demonstrates how the `ColumnValue` class is used to
-update records in the database: ```py re = pg_loom.update_one( Post, values=
-[ ColumnValue(name="title", value="Hey"), ColumnValue(name="completed",
-value=True), ], filters=[ Filter(column="id", value=1, join_next_with="AND"),
-Filter(column="userId", value=1, join_next_with="AND"), ], ) ``` It accepts two
-arguments: `name` and `value`. name represents the column name, while value
-corresponds to the new value to be assigned to that column. | Argument |
-Description | Type | Default | | -------- | -----------------------------------
------------------------ | ----- | ------- | | `name` | The name of the column
-to be updated or inserted. | `str` | - | | `value` | The value to assign to the
-column during update or insert. | `Any` | - | #### `Order` Class The `Order`
-class enables us to specify the desired order in which documents should be
-returned. Below is an example illustrating its usage: ```py posts =
-pg_loom.find_all( Post, select=["id", "completed", "title", "createdAt"],
-limit=3, offset=0, order=[ Order(column="createdAt", order="ASC"), Order
-(column="id", order="DESC"), ] ) ``` > ð**Pro Tip:** Note when utilizing a
-list of orders, they are applied sequentially, one after the other: | Argument
-| Description | Type | Default | | -------- | ---------------------------------
----------------------------------------- | ------------------- | ------- | |
-`column` | The name of the column to order by. | `str` | - | | `order` | The
-order direction, either `"ASC"` (ascending) or `"DESC"` (descending). | `"ASC"`
-or `"DESC"` | `"ASC"` | #### `Include` Class The `Include` class facilitates
-eager loading for models with relationships. Below is a table detailing the
-parameters available for the `Include` class: | Argument | Description | Type |
-Default | Required | | ---------------- | -------------------------------------
------------------------------------------------------- | ------------------- |
--------- | -------- | | `model` | The model to be included when eagerly
-fetching records. | `Model` | - | Yes | | `junction_table` | The
-`junction_table` model that is used as a reference table in a many to many
-association. | `Model` | `None` | No | | `order` | The list of order
-specifications for sorting the included data. | `list[Order]` | `[]` | No | |
-`limit` | The maximum number of records to include. | `int \| None` | `0` | No
-| | `offset` | The number of records to skip before including. | `int \| None`
-| `0` | No | | `select` | The list of columns to include. | `list[str] \| None`
-| `None` | No | | `has` | The relationship type between the current model and
-the included model. | `INCLUDE_LITERAL` | `"many"` | No | | `include` | The
-extra included models. | `list[Include]` | `[]` | No | | `alias` | The alias
-name for the included model. Very important when mapping self relations. |
-`str` | `None` | No | #### `Group` Class This class is used for data
+------------------------- | --------------- | ------- | | `type` | The datatype
+of your primary key. | `str` | `"int`" | | `length` | Optional to specify the
+length of the type. If passed as `N` with type `T`, it yields an SQL statement
+with type `T(N)`. | `int` \| `None` | `None` | | `auto_increment` | Optional to
+specify if the column will automatically increment or not. | `bool` | `False` |
+| `default` | Optional to specify the default value in a column. | `any` |
+`None` | | `nullable` | Optional to specify if the column will allow null
+values or not. | `bool` | `False` | | `unique` | Optional to specify if the
+column will contain unique values or not. | `bool` | `True` | ####
+`ForeignKeyColumn` Class This class is utilized when informing `dataloom` that
+a column has a relationship with a primary key in another table. Consider the
+following model definition of a `Post`: ```py class Post(Model): __tablename__:
+Optional[TableColumn] = TableColumn(name="posts") id = PrimaryKeyColumn
+(type="int", auto_increment=True, nullable=False, unique=True) completed =
+Column(type="boolean", default=False) title = Column(type="varchar",
+length=255, nullable=False) # timestamps createdAt = CreatedAtColumn()
+updatedAt = UpdatedAtColumn() # relations userId = ForeignKeyColumn( User,
+type="int", required=True, onDelete="CASCADE", onUpdate="CASCADE" ) ``` -
+`userId` is a foreign key in the table `posts`, indicating it has a
+relationship with a primary key in the `users` table. This column accepts the
+following arguments: | Argument | Description | Type | Default | | ---------- |
+-------------------------------------------------------------------------------
+------------------------------------- | ---------------------------------------
+- | ----------- | | `table` | Required. This is the parent table that the
+current model references. In our example, this is referred to as `User`. It can
+be used as a string in self relations. | `Model`\| `str` | | | `type` |
+Optional. Specifies the data type of the foreign key. If not provided, dataloom
+can infer it from the parent table. | `str` \| `None` | `None` | | `required` |
+Optional. Indicates whether the foreign key is required or not. | `bool` |
+`False` | | `onDelete` | Optional. Specifies the action to be taken when the
+associated record in the parent table is deleted. |`"NO ACTION"`, `"SET NULL"`,
+`"CASCADE"` | `"NO ACTION"` | | `onUpdate` | Optional. Specifies the action to
+be taken when the associated record in the parent table is updated. | `"NO
+ACTION"`, `"SET NULL"`, `"CASCADE"`| `"NO ACTION"` | It is crucial to specify
+the actions for `onDelete` and `onUpdate` to ensure that `dataloom` manages
+your model's relationship actions appropriately. The available actions are: 1.
+`"NO ACTION"` - If you delete or update the parent table, no changes will occur
+in the child table. 2. `"SET NULL"` - If you delete or update the parent table,
+the corresponding value in the child table will be set to `null`. 3.
+`"CASCADE"` - If you delete or update the table, the same action will also be
+applied to the child table. #### `CreatedAtColumn` Class When a column is
+designated as `CreatedAtColumn`, its value will be automatically generated each
+time you create a new record in a database, serving as a timestamp. ####
+`UpdatedAtColumn` Class When a column is designated as `UpdatedAtColumn`, its
+value will be automatically generated each time you create a new record or
+update an existing record in a database table, acting as a timestamp. ####
+`Filter` Class This `Filter` class in `dataloom` is designed to facilitate the
+application of filters when executing queries and mutations. It allows users to
+specify conditions that must be met for the operation to affect certain rows in
+a database table. Below is an example demonstrating how this class can be used:
+```python affected_rows = pg_loom.update_one( Post, values=[ ColumnValue
+(name="title", value="Hey"), ColumnValue(name="completed", value=True), ],
+filters=[ Filter(column="id", value=1, join_next_with="AND"), Filter
+(column="userId", value=1, join_next_with="AND"), ], ) ``` So from the above
+example we are applying filters while updating a `Post` here are the options
+that you can pass on that filter class: | Argument | Description | Type |
+Default | |-------------------------|------------------------------------------
+------------------|-------------------------------------------|----------------
+--------| | `column` | The name of the column to apply the filter on | `String`
+| - | | `value` | The value to filter against | `Any` | - | | `operator` | The
+comparison operator to use for the filter | `'eq'`, `'neq'`. `'lt'`, `'gt'`,
+`'leq'`, `'geq'`, `'in'`, `'notIn'`, `'like'`, `'between'`, `'not'` | `'eq'` |
+| `join_next_with` | The logical operator to join this filter with the next one
+| `'AND'`, `'OR'` | `'AND'` | > ð**Pro Tip:** Note You can apply either a
+list of filters or a single filter when filtering records. #### `ColumnValue`
+Class Just like the `Filter` class, `dataloom` also provides a `ColumnValue`
+class. This class acts as a setter to update the values of columns in your
+database table. The following code snippet demonstrates how the `ColumnValue`
+class is used to update records in the database: ```py re = pg_loom.update_one
+( Post, values=[ ColumnValue(name="title", value="Hey"), ColumnValue
+(name="completed", value=True), ], filters=[ Filter(column="id", value=1,
+join_next_with="AND"), Filter(column="userId", value=1, join_next_with="AND"),
+], ) ``` It accepts two arguments: `name` and `value`. name represents the
+column name, while value corresponds to the new value to be assigned to that
+column. | Argument | Description | Type | Default | | -------- | --------------
+-------------------------------------------- | ----- | ------- | | `name` | The
+name of the column to be updated or inserted. | `str` | - | | `value` | The
+value to assign to the column during update or insert. | `Any` | - | ####
+`Order` Class The `Order` class enables us to specify the desired order in
+which documents should be returned. Below is an example illustrating its usage:
+```py posts = pg_loom.find_all( Post, select=["id", "completed", "title",
+"createdAt"], limit=3, offset=0, order=[ Order(column="createdAt",
+order="ASC"), Order(column="id", order="DESC"), ] ) ``` > ð**Pro Tip:** Note
+when utilizing a list of orders, they are applied sequentially, one after the
+other: | Argument | Description | Type | Default | | -------- | ---------------
+---------------------------------------------------------- | ------------------
+- | ------- | | `column` | The name of the column to order by. | `str` | - | |
+`order` | The order direction, either `"ASC"` (ascending) or `"DESC"`
+(descending). | `"ASC"` or `"DESC"` | `"ASC"` | #### `Include` Class The
+`Include` class facilitates eager loading for models with relationships. Below
+is a table detailing the parameters available for the `Include` class: |
+Argument | Description | Type | Default | Required | | ---------------- | -----
+-------------------------------------------------------------------------------
+------- | ------------------- | -------- | -------- | | `model` | The model to
+be included when eagerly fetching records. | `Model` | - | Yes | |
+`junction_table` | The `junction_table` model that is used as a reference table
+in a many to many association. | `Model` | `None` | No | | `order` | The list
+of order specifications for sorting the included data. | `list[Order]` | `[]` |
+No | | `limit` | The maximum number of records to include. | `int \| None` |
+`0` | No | | `offset` | The number of records to skip before including. | `int
+\| None` | `0` | No | | `select` | The list of columns to include. | `list[str]
+\| None` | `None` | No | | `has` | The relationship type between the current
+model and the included model. | `INCLUDE_LITERAL` | `"many"` | No | | `include`
+| The extra included models. | `list[Include]` | `[]` | No | | `alias` | The
+alias name for the included model. Very important when mapping self relations.
+| `str` | `None` | No | #### `Group` Class This class is used for data
 `aggregation` and grouping data in `dataloom`. Below is a table detailing the
 parameters available for the `Group` class: | Argument | Description | Type |
 Default | Required | | --------------------------- | --------------------------
 ----------------------------- | --------------------------------------------- |
 --------- | -------- | | `column` | The name of the column to group by. | `str`
 | | Yes | | `function` | The aggregation function to apply on the grouped data.
 | `"COUNT" \| "AVG" \| "SUM" \| "MIN" \| "MAX"` | `"COUNT"` | No | | `having` |
@@ -410,72 +410,73 @@
 logs.sql", logging=True ) conn, tables = sqlite_loom.connect_and_sync([Post,
 User], drop=True, force=True) print(tables) if __name__ == "__main__":
 conn.close() ``` Returns a `conn` and the list of `tablenames` that exist in
 the database. The method accepts the same arguments as the `sync` method. ###
 CRUD Operations with Dataloom In this section of the documentation, we will
 illustrate how to perform basic `CRUD` operations using `dataloom` on simple
 `Models`. Please note that in the following code snippets, I will be utilizing
-`sqlite_loom`. However, it's important to highlight that you can use any `loom`
-of your choice to follow along. #### 1. Creating a Record To insert a single or
-multiple records in a database you make use of the following functions: 1.
-`insert_one()` 2. `insert_bulk()` ##### 1. `insert_one()` The `insert_one`
-method allows you to save a single row in a specific table. Upon saving, it
-will return the primary key (`pk`) value of the inserted document. The
-following example shows how the `insert_one()` method works. ```python #
-Example: Creating a user record userId = pg_loom.insert_one( instance=User,
-values=ColumnValue(name="username", value="@miller") ) userId =
-pg_loom.insert_one( instance=User, values=[ ColumnValue(name="username",
-value="@miller"), ColumnValue(name="name", value="Jonh"), ], ) ``` This
-function takes in two arguments which are `instance` and `values`. Where values
-are the column values that you are inserting in a user table or a single column
-value. | Argument | Description | `Type` | `Required` | `Default` | | ---------
-- | ---------------------------------------------------------------------------
---------------------------------- | ------------------------------------ | ----
------- | --------- | | `instance` | The instance of the table where the row
-will be inserted. | `Model` | `Yes` | `None` | | `values` | The column values
-to be inserted into the table. It can be a single column value or a list of
-column values. | `list[ColumnValue]` or `ColumnValue` | `Yes` | `None` | #####
-2. `insert_bulk()`. The `insert_bulk` method facilitates the bulk insertion of
-records, as its name suggests. The following example illustrates how you can
-add `3` posts to the database table simultaneously. ```python # Example:
-Inserting multiple posts rows = pg_loom.insert_bulk( User, values=[
+`sqlite_loom`, `mysql_loom`, `pg_loom` or `loom` interchangeably. However, it's
+important to highlight that you can use any `loom` of your choice to follow
+along. #### 1. Creating a Record To insert a single or multiple records in a
+database you make use of the following functions: 1. `insert_one()` 2.
+`insert_bulk()` ##### 1. `insert_one()` The `insert_one` method allows you to
+save a single row in a specific table. Upon saving, it will return the primary
+key (`pk`) value of the inserted document. The following example shows how the
+`insert_one()` method works. ```python # Example: Creating a user record userId
+= pg_loom.insert_one( instance=User, values=ColumnValue(name="username",
+value="@miller") ) userId = pg_loom.insert_one( instance=User, values=
 [ ColumnValue(name="username", value="@miller"), ColumnValue(name="name",
-value="Jonh"), ], [ ColumnValue(name="username", value="@brown"), ColumnValue
-(name="name", value="Jonh"), ], [ ColumnValue(name="username", value="@blue"),
-ColumnValue(name="name", value="Jonh"), ], ], ) ``` The argument parameters for
-the `insert_bulk` methods are as follows. | Argument | Description | `Type` |
-`Required` | `Default` | | ---------- | ---------------------------------------
--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
------- | ------------------------------------------ | ---------- | --------- |
-| `instance` | The instance of the table where the row will be inserted. |
+value="Jonh"), ], ) ``` This function takes in two arguments which are
+`instance` and `values`. Where values are the column values that you are
+inserting in a user table or a single column value. | Argument | Description |
+`Type` | `Required` | `Default` | | ---------- | ------------------------------
+-----------------------------------------------------------------------------
+- | ------------------------------------ | ---------- | --------- | |
+`instance` | The instance of the table where the row will be inserted. |
 `Model` | `Yes` | `None` | | `values` | The column values to be inserted into
-the table. **It must be a list of list of column values with the same length,
-otherwise dataloom will fail to map the values correctly during the insert
-operation.** | `list[list[ColumnValue]]` or `ColumnValue` | `Yes` | `None` | >
-In contrast to the `insert_one` method, the `insert_bulk` method returns the
-row count of the inserted documents rather than the individual primary keys
-(`pks`) of those documents. #### 2. Reading records To retrieve documents or a
-document from the database, you can make use of the following functions: 1.
-`find_all()`: This function is used to retrieve all documents from the
-database. 2. `find_by_pk()`: This function is used to retrieve a document by
-its primary key (or ID). 3. `find_one()`: This function is used to retrieve a
-single document based on a specific condition. 4. `find_many()`: This function
-is used to retrieve multiple documents based on a specific condition. ##### 1.
-`find_all()` This method is used to retrieve all the records that are in the
-database table. Below are examples demonstrating how to do it: ```py users =
-pg_loom.find_all( instance=User, select=["id", "username"], limit=3, offset=0,
-order=[Order(column="id", order="DESC")], ) print(users) # ? [{'id': 1,
-'username': '@miller'}] ``` The `find_all()` method takes in the following
-arguments: | Argument | Description | Type | Default | Required | | ---------
-- | ---------------------------------------------------------------------------
---------------- | ------------------------ | ------- | -------- | | `instance`
-| The model class to retrieve documents from. | `Model` | `None` | `Yes` | |
-`select` | Collection or a string of fields to select from the documents. |
-`list[str]\|str` | `None` | `No` | | `limit` | Maximum number of documents to
+the table. It can be a single column value or a list of column values. | `list
+[ColumnValue]` or `ColumnValue` | `Yes` | `None` | ##### 2. `insert_bulk()`.
+The `insert_bulk` method facilitates the bulk insertion of records, as its name
+suggests. The following example illustrates how you can add `3` posts to the
+database table simultaneously. ```python # Example: Inserting multiple posts
+rows = pg_loom.insert_bulk( User, values=[ [ ColumnValue(name="username",
+value="@miller"), ColumnValue(name="name", value="Jonh"), ], [ ColumnValue
+(name="username", value="@brown"), ColumnValue(name="name", value="Jonh"), ],
+[ ColumnValue(name="username", value="@blue"), ColumnValue(name="name",
+value="Jonh"), ], ], ) ``` The argument parameters for the `insert_bulk`
+methods are as follows. | Argument | Description | `Type` | `Required` |
+`Default` | | ---------- | ----------------------------------------------------
+-------------------------------------------------------------------------------
+------------------------------------------------------------------------ | ----
+-------------------------------------- | ---------- | --------- | | `instance`
+| The instance of the table where the row will be inserted. | `Model` | `Yes` |
+`None` | | `values` | The column values to be inserted into the table. **It
+must be a list of list of column values with the same length, otherwise
+dataloom will fail to map the values correctly during the insert operation.** |
+`list[list[ColumnValue]]` or `ColumnValue` | `Yes` | `None` | > In contrast to
+the `insert_one` method, the `insert_bulk` method returns the row count of the
+inserted documents rather than the individual primary keys (`pks`) of those
+documents. #### 2. Reading records To retrieve documents or a document from the
+database, you can make use of the following functions: 1. `find_all()`: This
+function is used to retrieve all documents from the database. 2. `find_by_pk
+()`: This function is used to retrieve a document by its primary key (or ID).
+3. `find_one()`: This function is used to retrieve a single document based on a
+specific condition. 4. `find_many()`: This function is used to retrieve
+multiple documents based on a specific condition. ##### 1. `find_all()` This
+method is used to retrieve all the records that are in the database table.
+Below are examples demonstrating how to do it: ```py users = pg_loom.find_all
+( instance=User, select=["id", "username"], limit=3, offset=0, order=[Order
+(column="id", order="DESC")], ) print(users) # ? [{'id': 1, 'username':
+'@miller'}] ``` The `find_all()` method takes in the following arguments: |
+Argument | Description | Type | Default | Required | | ---------- | -----------
+------------------------------------------------------------------------------
+- | ------------------------ | ------- | -------- | | `instance` | The model
+class to retrieve documents from. | `Model` | `None` | `Yes` | | `select` |
+Collection or a string of fields to select from the documents. | `list
+[str]\|str` | `None` | `No` | | `limit` | Maximum number of documents to
 retrieve. | `int` | `None` | `No` | | `offset` | Number of documents to skip
 before retrieving. | `int` | `0` | `No` | | `order` | Collection of `Order` or
 a single `Order` to order the documents when querying. | `list[Order]\|Order` |
 `None` | `No` | | `include` | Collection or a `Include` of related models to
 eagerly load. | `list[Include]\|Include` | `None` | `No` | | `group` |
 Collection of `Group` which specifies how you want your data to be grouped
 during queries. | `list[Group]\|Group` | `None` | `No` | | `distinct` | Boolean
@@ -503,15 +504,15 @@
 Collection of `Filter` or a `Filter` to apply to the query. | `list[Filter] \|
 Filter` | `None` | `No` | | `distinct` | Boolean telling dataloom to return
 distinct row values based on selected fields or not. | `bool` | `False` | `No`
 | > ð **Pro Tip**: The distinction between the `find_all()` and `find_many
 ()` methods lies in the fact that `find_many()` enables you to apply specific
 filters, whereas `find_all()` retrieves all the documents within the specified
 model. ##### 3. `find_one()` Here is an example showing you how you can use
-`find_by_pk()` locate a single record in the database. ```py user =
+`find_one()` locate a single record in the database. ```py user =
 mysql_loom.find_one( User, filters=[Filter(column="username",
 value="@miller")], select=["id", "username"], ) print(user) # ? {'id': 1,
 'username': '@miller'} ``` This method take the following as arguments |
 Argument | Description | Type | Default | Required | | ---------- | -----------
 ------------------------------------------------------------------------------
 - | -------------------------------- | ------- | -------- | | `instance` | The
 model class to retrieve instances from. | `Model` | | `Yes` | | `filters` |
@@ -610,174 +611,175 @@
 `delete_bulk()` function, exercise caution as it can be aggressive. If the
 filter is not explicitly provided, there is a risk of mistakenly deleting all
 records in the table. ###### Guidelines for Safe Usage To mitigate the
 potential risks associated with `delete_bulk()`, follow these guidelines: 1.
 **Always Provide a Filter:** - When calling `delete_bulk()`, make sure to
 provide a filter to specify the subset of records to be deleted. This helps
 prevent unintentional deletions. ```python # Example: Delete records where
-'status' is 'inactive' sqlite_loom.delete_bulk(filter={'status': 'inactive'})
-``` 2. **Consider Usage When Necessary:** - When contemplating data deletion,
-it is advisable to consider more targeted methods before resorting to
-`delete_bulk()`. Prioritize the use of `delete_one()` or `delete_by_pk()`
-methods to remove specific records based on your needs. This ensures a more
-precise and controlled approach to data deletion. 3. **Use limit and offsets
-options** - You can consider using the `limit` and offset options during
-invocation of `delete_bulk` ```py affected_rows = mysql_loom.delete_bulk
+'status' is 'inactive' affected_rows = mysql_loom.delete_bulk( instance=User,
+filters=Filter(column="status", value='inactive'), ) ``` 2. **Consider Usage
+When Necessary:** - When contemplating data deletion, it is advisable to
+consider more targeted methods before resorting to `delete_bulk()`. Prioritize
+the use of `delete_one()` or `delete_by_pk()` methods to remove specific
+records based on your needs. This ensures a more precise and controlled
+approach to data deletion. 3. **Use limit and offsets options** - You can
+consider using the `limit` and offset options during invocation of
+`delete_bulk` ```py affected_rows = mysql_loom.delete_bulk( instance=Post,
+order=[Order(column="id", order="DESC"), Order(column="createdAt",
+order="ASC")], filters=[Filter(column="id", operator="gt", value=0)], offset=0,
+limit=10, ) ``` By following these guidelines, you can use the `delete_bulk()`
+function safely and minimize the risk of unintended data loss. Always exercise
+caution and adhere to best practices when performing bulk deletion operations.
+### Ordering In dataloom you can order documents in either `DESC` (descending)
+or `ASC` (ascending) order using the helper class `Order`. ```py posts =
+mysql_loom.find_all( instance=Post, order=[Order(column="id", order="DESC")], )
+``` You can apply multiple and these orders will ba applied in sequence of
+application here is an example: ```py posts = mysql_loom.find_all
 ( instance=Post, order=[Order(column="id", order="DESC"), Order
-(column="createdAt", order="ASC")], filters=[Filter(column="id", operator="gt",
-value=0)], offset=0, limit=10, ) ``` By following these guidelines, you can use
-the `delete_bulk()` function safely and minimize the risk of unintended data
-loss. Always exercise caution and adhere to best practices when performing bulk
-deletion operations. ### Ordering In dataloom you can order documents in either
-`DESC` (descending) or `ASC` (ascending) order using the helper class `Order`.
-```py posts = mysql_loom.find_all( instance=Post, order=[Order(column="id",
-order="DESC")], ) ``` You can apply multiple and these orders will ba applied
-in sequence of application here is an example: ```py posts =
-mysql_loom.find_all( instance=Post, order=[Order(column="id", order="DESC"),
-Order(column="createdAt", order="ASC")], ) ``` ### Filters There are different
-find of filters that you can use when filtering documents for mutations and
-queries. Filters are very important to use when updating and deleting documents
-as they give you control on which documents should be updated or deleted. When
-doing a mutation you can use a single or multiple filters. Bellow is an example
-that shows you how you can use a single filter in deleting a single record that
-has an `id` greater than `1` from the database. ```py res2 =
-mysql_loom.delete_one( instance=Post, offset=0, order=Order(column="id",
-order="DESC"), filters=Filter(column="id", value=1, operator="gt"), ) ``` Or
-you can use it as follows: ```py res2 = mysql_loom.delete_one( instance=Post,
-offset=0, order=[Order(column="id", order="DESC")], filters=[Filter
-(column="id", value=1, operator="gt")], ) ``` As you have noticed, you can join
-your filters together and they will be applied sequentially using the
-[`join_next_with`](#filter-class) which can be either `OR` or `AND` te default
-value is `AND`. Here is an of filter usage in sequential. ```py res2 =
-mysql_loom.delete_one( instance=Post, offset=0, order=[Order(column="id",
-order="DESC")], filters=[ Filter(column="id", value=1, operator="gt"), Filter
-(column="userId", value=1, operator="eq", join_next_with="OR"), Filter
-( column="title", value='"What are you doing general?"', operator="=",
-join_next_with="AND", ), ], ) ``` ##### Operators You can use the `operator` to
-match the values. Here is the table of description for these filters. |
-Operator | Explanation | Expect | | ----------- | -----------------------------
-------------------------------------------------------------------------------
-- | --------------------- | | `'eq'` | Indicates equality. It checks if the
-value is equal to the specified criteria. | Value == Criteria | | `'lt'` |
-Denotes less than. It checks if the value is less than the specified criteria.
-| Value < Criteria | | `'gt'` | Denotes greater than. It checks if the value is
-greater than the specified criteria. | Value > Criteria | | `'leq'` | Denotes
-less than or equal to. It checks if the value is less than or equal to the
-specified criteria. | Value <= Criteria | | `'geq'` | Denotes greater than or
-equal to. It checks if the value is greater than or equal to the specified
-criteria. | Value >= Criteria | | `'in'` | Checks if the value is included in a
-specified list of values. | Value in List | | `'notIn'` | Checks if the value
-is not included in a specified list of values. | Value not in List | | `'like'`
-| Performs a pattern matching operation. It checks if the value is similar to a
-specified pattern. | Value matches Pattern | | `'not'` | Indicates non-
-equality. It checks if the column value that does not equal to the specified
-criteria. | NOT id = Criteria | | `'neq'` | Indicates non-equality. It checks
-if the value is not equal to the specified criteria. | Value != Criteria | |
-`'between'` | It checks range values that matches a given range between the
-minimum and maximum. | id BETWEEN (min, max) | Let's talk about these filters
-in detail of code by example. Let's say you want to update a `Post` where the
-`id` matches `1` you can do it as follows: ```py res2 = mysql_loom.update_one
-( instance=Post, filters=Filter( column="id", value=1, operator="eq", ),
-values=[ColumnValue(name="title", value="Bob")], ) ``` What if you want to
-update a post where `id` is not equal to `1` you can do it as follows ```py
+(column="createdAt", order="ASC")], ) ``` ### Filters There are different find
+of filters that you can use when filtering documents for mutations and queries.
+Filters are very important to use when updating and deleting documents as they
+give you control on which documents should be updated or deleted. When doing a
+mutation you can use a single or multiple filters. Bellow is an example that
+shows you how you can use a single filter in deleting a single record that has
+an `id` greater than `1` from the database. ```py res2 = mysql_loom.delete_one
+( instance=Post, offset=0, order=Order(column="id", order="DESC"),
+filters=Filter(column="id", value=1, operator="gt"), ) ``` Or you can use it as
+follows: ```py res2 = mysql_loom.delete_one( instance=Post, offset=0, order=
+[Order(column="id", order="DESC")], filters=[Filter(column="id", value=1,
+operator="gt")], ) ``` As you have noticed, you can join your filters together
+and they will be applied sequentially using the [`join_next_with`](#filter-
+class) which can be either `OR` or `AND` te default value is `AND`. Here is an
+of filter usage in sequential. ```py res2 = mysql_loom.delete_one
+( instance=Post, offset=0, order=[Order(column="id", order="DESC")], filters=
+[ Filter(column="id", value=1, operator="gt"), Filter(column="userId", value=1,
+operator="eq", join_next_with="OR"), Filter( column="title", value='"What are
+you doing general?"', operator="=", join_next_with="AND", ), ], ) ``` #####
+Operators You can use the `operator` to match the values. Here is the table of
+description for these filters. | Operator | Explanation | Expect | | ----------
+- | ---------------------------------------------------------------------------
+--------------------------------- | --------------------- | | `'eq'` |
+Indicates equality. It checks if the value is equal to the specified criteria.
+| Value == Criteria | | `'lt'` | Denotes less than. It checks if the value is
+less than the specified criteria. | Value < Criteria | | `'gt'` | Denotes
+greater than. It checks if the value is greater than the specified criteria. |
+Value > Criteria | | `'leq'` | Denotes less than or equal to. It checks if the
+value is less than or equal to the specified criteria. | Value <= Criteria | |
+`'geq'` | Denotes greater than or equal to. It checks if the value is greater
+than or equal to the specified criteria. | Value >= Criteria | | `'in'` |
+Checks if the value is included in a specified list of values. | Value in List
+| | `'notIn'` | Checks if the value is not included in a specified list of
+values. | Value not in List | | `'like'` | Performs a pattern matching
+operation. It checks if the value is similar to a specified pattern. | Value
+matches Pattern | | `'not'` | Indicates non-equality. It checks if the column
+value that does not equal to the specified criteria. | NOT id = Criteria | |
+`'neq'` | Indicates non-equality. It checks if the value is not equal to the
+specified criteria. | Value != Criteria | | `'between'` | It checks range
+values that matches a given range between the minimum and maximum. | id BETWEEN
+(min, max) | Let's talk about these filters in detail of code by example. Let's
+say you want to update a `Post` where the `id` matches `1` you can do it as
+follows: ```py res2 = mysql_loom.update_one( instance=Post, filters=Filter
+( column="id", value=1, operator="eq", ), values=[ColumnValue(name="title",
+value="Bob")], ) ``` What if you want to update a post where `id` is not equal
+to `1` you can do it as follows ```py res2 = mysql_loom.update_bulk
+( instance=Post, filters=Filter( column="id", value=1, operator="neq", ),
+values=[ColumnValue(name="title", value="Bob")], ) ``` What if i want to update
+the records that have an `id` less than `3`? ```py res2 =
+mysql_loom.update_bulk( instance=Post, filters=Filter( column="id", value=3,
+operator="lt", ), values=[ColumnValue(name="title", value="Bob")], ) ``` What
+if i want to update the records that have an `id` less than or equal `3`? ```py
 res2 = mysql_loom.update_bulk( instance=Post, filters=Filter( column="id",
 value=1, operator="neq", ), values=[ColumnValue(name="title", value="Bob")], )
-``` What if i want to update the records that have an `id` less than `3`? ```py
-res2 = mysql_loom.update_bulk( instance=Post, filters=Filter( column="id",
-value=3, operator="lt", ), values=[ColumnValue(name="title", value="Bob")], )
-``` What if i want to update the records that have an `id` less than or equal
-`3`? ```py res2 = mysql_loom.update_bulk( instance=Post, filters=Filter
-( column="id", value=1, operator="neq", ), values=[ColumnValue(name="title",
-value="Bob")], ) ``` What if i want to update the records that have an `id`
-greater than `3`? ```py res = mysql_loom.update_bulk( instance=Post,
-filters=Filter( column="id", value=3, operator="gt", ), values=[ColumnValue
-(name="title", value="Bob")], ) ``` What if i want to update the records that
-have an `id` greater or equal to `3`? ```py res = mysql_loom.update_bulk
-( instance=Post, filters=Filter( column="id", value=3, operator="geq", ),
-values=[ColumnValue(name="title", value="Bob")], ) ``` You can use the `in` to
-update or query records that matches values in a specified `list` of values or
-`tuple`. Here is an example showing you how you can update records that does
-matches `id` in `[1, 2]`. ```py res = mysql_loom.update_bulk( instance=Post,
-filters=Filter( column="id", value=[1, 2], operator="in", ), values=
-[ColumnValue(name="title", value="Bob")], ) ``` You can use the `notIn` to
-update or query records that does not matches values in a specified `list` of
-values or `tuple`. Here is an example showing you how you can update records
-that does not matches `id` in `[1, 2]`. ```py res = mysql_loom.update_bulk
-( instance=Post, filters=Filter( column="id", value=[1, 2], operator="notIn",
-), values=[ColumnValue(name="title", value="Bob")], ) ``` You can use the
-`like` operator to match some patens in your query filters. Let's say we want
-to match a post that has the title ends with `general` we can use the `like`
-operator as follows ```py general = mysql_loom.find_one( instance=Post,
-filters=Filter( column="title", value="% general?", operator="like", ), select=
-["id", "title"], ) print(general) # ? {'id': 1, 'title': 'What are you doing
-general?'} ``` The following table show you some expression that you can use
-with this `like` operator. | Value | Description | | -------------- | ---------
+``` What if i want to update the records that have an `id` greater than `3`?
+```py res = mysql_loom.update_bulk( instance=Post, filters=Filter( column="id",
+value=3, operator="gt", ), values=[ColumnValue(name="title", value="Bob")], )
+``` What if i want to update the records that have an `id` greater or equal to
+`3`? ```py res = mysql_loom.update_bulk( instance=Post, filters=Filter
+( column="id", value=3, operator="geq", ), values=[ColumnValue(name="title",
+value="Bob")], ) ``` You can use the `in` to update or query records that
+matches values in a specified `list` of values or `tuple`. Here is an example
+showing you how you can update records that does matches `id` in `[1, 2]`.
+```py res = mysql_loom.update_bulk( instance=Post, filters=Filter( column="id",
+value=[1, 2], operator="in", ), values=[ColumnValue(name="title",
+value="Bob")], ) ``` You can use the `notIn` to update or query records that
+does not matches values in a specified `list` of values or `tuple`. Here is an
+example showing you how you can update records that does not matches `id` in `
+[1, 2]`. ```py res = mysql_loom.update_bulk( instance=Post, filters=Filter
+( column="id", value=[1, 2], operator="notIn", ), values=[ColumnValue
+(name="title", value="Bob")], ) ``` You can use the `like` operator to match
+some patens in your query filters. Let's say we want to match a post that has
+the title ends with `general` we can use the `like` operator as follows ```py
+general = mysql_loom.find_one( instance=Post, filters=Filter( column="title",
+value="% general?", operator="like", ), select=["id", "title"], ) print
+(general) # ? {'id': 1, 'title': 'What are you doing general?'} ``` The
+following table show you some expression that you can use with this `like`
+operator. | Value | Description | | -------------- | --------------------------
 -------------------------------------------------------------------------------
--------------------------------- | | `%pattern` | Finds values that end with
-the specified pattern. | | `pattern%` | Finds values that start with the
-specified pattern. | | `%pattern%` | Finds values that contain the specified
-pattern anywhere within the string. | | `_pattern` | Finds values that have any
-single character followed by the specified pattern. | | `pattern_` | Finds
-values that have the specified pattern followed by any single character. | | `
-[charlist]%` | Finds values that start with any character in the specified
-character list. | | `[!charlist]%` | Finds values that start with any character
-not in the specified character list. | | `_pattern_` | Finds values that have
-any single character followed by the specified pattern and then followed by any
-single character. | ### Data Aggregation With the [`Having`](#having-class) and
-the [`Group`](#group-class) classes you can perform some powerful powerful
-queries. In this section we are going to demonstrate an example of how we can
-do the aggregate queries. ```py posts = mysql_loom.find_many( Post,
-select="id", filters=Filter(column="id", operator="gt", value=1), group=Group
-( column="id", function="MAX", having=Having(column="id", operator="in", value=
-(2, 3, 4)), return_aggregation_column=True, ), ) ``` The following will be the
-output from the above query. ```shell [{'id': 2, 'MAX(`id`)': 2}, {'id': 3,
-'MAX(`id`)': 3}, {'id': 4, 'MAX(`id`)': 4}] ``` However you can remove the
-aggregation column from the above query by specifying the
-`return_aggregation_column` to be `False`: ```py posts = mysql_loom.find_many
-( Post, select="id", filters=Filter(column="id", operator="gt", value=1),
-group=Group( column="id", function="MAX", having=Having(column="id",
-operator="in", value=(2, 3, 4)), return_aggregation_column=False, ), ) print
-(posts) ``` This will output: ```shell [{'id': 2}, {'id': 3}, {'id': 4}] ```
-#### Aggregation Functions You can use the following aggregation functions that
-dataloom supports: | Aggregation Function | Description | | -------------------
-- | ------------------------------------------------ | | `"AVG"` | Computes the
-average of the values in the group. | | `"COUNT"` | Counts the number of items
-in the group. | | `"SUM"` | Computes the sum of the values in the group. | |
-`"MAX"` | Retrieves the maximum value in the group. | | `"MIN"` | Retrieves the
-minimum value in the group. | > ð **Pro Tip**: Note that data aggregation
-only works without `eager` loading and also works only with [`find_may()`](#2-
-find_many) and [`find_all()`](#1-find_all) in dataloom. ### Utilities Dataloom
-comes up with some utility functions that works on an instance of a model. This
-is very useful when debuging your tables to see how do they look like. These
-function include: #### 1. `inspect()` This function takes in a model as
-argument and inspect the model fields or columns. The following examples show
-how we can use this handy function in inspecting table names. ```py table =
-mysql_loom.inspect(instance=User, fields=["name", "type"], print_table=False)
-print(table) ``` The above snippet returns a list of dictionaries containing
-the column name and the arguments that were passed. ```shell [{'id': {'type':
-'int'}}, {'name': {'type': 'varchar'}}, {'tokenVersion': {'type': 'int'}},
-{'username': {'type': 'varchar'}}] ``` You can print table format these fields
-with their types as follows ```py mysql_loom.inspect(instance=User) ``` Output:
-```shell +--------------+---------+----------+---------+ | name | type |
-nullable | default | +--------------+---------+----------+---------+ | id | int
-| NO | None | | name | varchar | NO | Bob | | tokenVersion | int | YES | 0 | |
-username | varchar | YES | None | +--------------+---------+----------+--------
--+ ``` The `inspect` function take the following arguments. | Argument |
-Description | Type | Default | Required | | ------------- | -------------------
------------------------------------ | ----------- | ---------------------------
--------------- | -------- | | `instance` | The model instance to inspect. |
-`Model` | - | Yes | | `fields` | The list of fields to include in the
-inspection. | `list[str]` | `["name", "type", "nullable", "default"]` | No | |
-`print_table` | Flag indicating whether to print the inspection table. | `bool`
-| `True` | No | #### 2. `decorators` These modules contain several decorators
-that can prove useful when creating models. These decorators originate from
-`dataloom.decorators`, and at this stage, we are referring to them as
-"experimental." ##### `@initialize()` Let's examine a model named `Profile`,
-which appears as follows: ```py class Profile(Model): __tablename__: Optional
-[TableColumn] = TableColumn(name="profiles") id = PrimaryKeyColumn(type="int",
+--------------- | | `%pattern` | Finds values that end with the specified
+pattern. | | `pattern%` | Finds values that start with the specified pattern. |
+| `%pattern%` | Finds values that contain the specified pattern anywhere within
+the string. | | `_pattern` | Finds values that have any single character
+followed by the specified pattern. | | `pattern_` | Finds values that have the
+specified pattern followed by any single character. | | `[charlist]%` | Finds
+values that start with any character in the specified character list. | | `
+[!charlist]%` | Finds values that start with any character not in the specified
+character list. | | `_pattern_` | Finds values that have any single character
+followed by the specified pattern and then followed by any single character. |
+### Data Aggregation With the [`Having`](#having-class) and the [`Group`]
+(#group-class) classes you can perform some powerful powerful queries. In this
+section we are going to demonstrate an example of how we can do the aggregate
+queries. ```py posts = mysql_loom.find_many( Post, select="id", filters=Filter
+(column="id", operator="gt", value=1), group=Group( column="id",
+function="MAX", having=Having(column="id", operator="in", value=(2, 3, 4)),
+return_aggregation_column=True, ), ) ``` The following will be the output from
+the above query. ```shell [{'id': 2, 'MAX(`id`)': 2}, {'id': 3, 'MAX(`id`)':
+3}, {'id': 4, 'MAX(`id`)': 4}] ``` However you can remove the aggregation
+column from the above query by specifying the `return_aggregation_column` to be
+`False`: ```py posts = mysql_loom.find_many( Post, select="id", filters=Filter
+(column="id", operator="gt", value=1), group=Group( column="id",
+function="MAX", having=Having(column="id", operator="in", value=(2, 3, 4)),
+return_aggregation_column=False, ), ) print(posts) ``` This will output:
+```shell [{'id': 2}, {'id': 3}, {'id': 4}] ``` #### Aggregation Functions You
+can use the following aggregation functions that dataloom supports: |
+Aggregation Function | Description | | -------------------- | -----------------
+------------------------------- | | `"AVG"` | Computes the average of the
+values in the group. | | `"COUNT"` | Counts the number of items in the group. |
+| `"SUM"` | Computes the sum of the values in the group. | | `"MAX"` |
+Retrieves the maximum value in the group. | | `"MIN"` | Retrieves the minimum
+value in the group. | > ð **Pro Tip**: Note that data aggregation only works
+without `eager` loading and also works only with [`find_may()`](#2-find_many)
+and [`find_all()`](#1-find_all) in dataloom. ### Utilities Dataloom comes up
+with some utility functions that works on an instance of a model. This is very
+useful when debuging your tables to see how do they look like. These function
+include: #### 1. `inspect()` This function takes in a model as argument and
+inspect the model fields or columns. The following examples show how we can use
+this handy function in inspecting table names. ```py table = mysql_loom.inspect
+(instance=User, fields=["name", "type"], print_table=False) print(table) ```
+The above snippet returns a list of dictionaries containing the column name and
+the arguments that were passed. ```shell [{'id': {'type': 'int'}}, {'name':
+{'type': 'varchar'}}, {'tokenVersion': {'type': 'int'}}, {'username': {'type':
+'varchar'}}] ``` You can print table format these fields with their types as
+follows ```py mysql_loom.inspect(instance=User) ``` Output: ```shell +---------
+-----+---------+----------+---------+ | name | type | nullable | default | +---
+-----------+---------+----------+---------+ | id | int | NO | None | | name |
+varchar | NO | Bob | | tokenVersion | int | YES | 0 | | username | varchar |
+YES | None | +--------------+---------+----------+---------+ ``` The `inspect`
+function take the following arguments. | Argument | Description | Type |
+Default | Required | | ------------- | ----------------------------------------
+-------------- | ----------- | ----------------------------------------- | ----
+---- | | `instance` | The model instance to inspect. | `Model` | - | Yes | |
+`fields` | The list of fields to include in the inspection. | `list[str]` | `
+["name", "type", "nullable", "default"]` | No | | `print_table` | Flag
+indicating whether to print the inspection table. | `bool` | `True` | No | ####
+2. `decorators` These modules contain several decorators that can prove useful
+when creating models. These decorators originate from `dataloom.decorators`,
+and at this stage, we are referring to them as "experimental." #####
+`@initialize()` Let's examine a model named `Profile`, which appears as
+follows: ```py class Profile(Model): __tablename__: Optional[TableColumn] =
+TableColumn(name="profiles") id = PrimaryKeyColumn(type="int",
 auto_increment=True) avatar = Column(type="text", nullable=False) userId =
 ForeignKeyColumn( User, maps_to="1-1", type="int", required=True,
 onDelete="CASCADE", onUpdate="CASCADE", ) ``` This is simply a Python class
 that inherits from the top-level class `Model`. However, it lacks some useful
 `dunder` methods such as `__init__` and `__repr__`. In standard Python, we can
 achieve this functionality by using `dataclasses`. For example, we can modify
 our class as follows: ```py from dataclasses import dataclass @dataclass class
@@ -1321,11 +1323,13 @@
 don't want logging at all. | `int` | No | `1` | | `is_script` | Whether the SQL
 is a script. | `bool` | No | `False` | #### Why Use Query Builder? - The query
 builder empowers developers to seamlessly execute `SQL` queries directly. -
 While Dataloom primarily utilizes `subqueries` for eager data fetching on
 models, developers may prefer to employ JOIN operations, which are achievable
 through the `qb` object. ```python qb = loom.getQueryBuilder() result = qb.run
 ("SELECT * FROM table1 INNER JOIN table2 ON table1.id = table2.table1_id;")
-print(result) ``` ### Contributing Contributions to `dataloom` are welcome!
-Feel free to submit bug reports, feature requests, or pull requests on [GitHub]
-(https://github.com/CrispenGari/dataloom). ### License This project is licensed
-under the MIT License - see the [LICENSE](/LISENSE) file for details.
+print(result) ``` ### Documentation You can read the full documentation of
+dataloom on [readthedocs.io](https://dataloom-py.readthedocs.io/en/latest/) ###
+Contributing Contributions to `dataloom` are welcome! Feel free to submit bug
+reports, feature requests, or pull requests on [GitHub](https://github.com/
+CrispenGari/dataloom). ### License This project is licensed under the MIT
+License - see the [LICENSE](/LISENSE) file for details.
```

### Comparing `dataloom-2.4.1/dataloom/__init__.py` & `dataloom-2.4.2/dataloom/__init__.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/columns/__init__.py` & `dataloom-2.4.2/dataloom/columns/__init__.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/conn/__init__.py` & `dataloom-2.4.2/dataloom/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/constants/__init__.py` & `dataloom-2.4.2/dataloom/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/decorators/__init__.py` & `dataloom-2.4.2/dataloom/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/exceptions/__init__.py` & `dataloom-2.4.2/dataloom/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/keys.py` & `dataloom-2.4.2/dataloom/keys.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/loom/__init__.py` & `dataloom-2.4.2/dataloom/loom/__init__.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/loom/delete.py` & `dataloom-2.4.2/dataloom/loom/delete.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/loom/insert.py` & `dataloom-2.4.2/dataloom/loom/insert.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/loom/inspect.py` & `dataloom-2.4.2/dataloom/loom/inspect.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/loom/interfaces.py` & `dataloom-2.4.2/dataloom/loom/interfaces.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/loom/math.py` & `dataloom-2.4.2/dataloom/loom/math.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/loom/qb.py` & `dataloom-2.4.2/dataloom/loom/qb.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/loom/query.py` & `dataloom-2.4.2/dataloom/loom/query.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/loom/sql.py` & `dataloom-2.4.2/dataloom/loom/sql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/loom/subqueries.py` & `dataloom-2.4.2/dataloom/loom/subqueries.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/loom/update.py` & `dataloom-2.4.2/dataloom/loom/update.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/model/__init__.py` & `dataloom-2.4.2/dataloom/model/__init__.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/statements/__init__.py` & `dataloom-2.4.2/dataloom/statements/__init__.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/statements/statements.py` & `dataloom-2.4.2/dataloom/statements/statements.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_aggregation_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_aggregation_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_alter_tables_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_alter_tables_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_connection_options_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_connection_options_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_connection_uri_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_connection_uri_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_create_tables_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_create_tables_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_delete_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_delete_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_eager_loading_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_eager_loading_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_experimental_decorators_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_experimental_decorators_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_insert_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_insert_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_inspect_table_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_inspect_table_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_operators_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_operators_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_qb_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_qb_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_query_msql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_query_msql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_update_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_update_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/mysql/test_utils_fns_mysql.py` & `dataloom-2.4.2/dataloom/tests/mysql/test_utils_fns_mysql.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_aggregation_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_aggregation_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_alter_tables_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_alter_tables_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_connection_options_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_connection_options_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_connection_uri_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_connection_uri_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_create_table_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_create_table_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_delete_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_delete_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_eager_loading_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_eager_loading_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_experimental_decorators_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_experimental_decorators_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_insert_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_insert_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_inspecting_table_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_inspecting_table_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_operators_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_operators_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_qb_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_qb_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_query_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_query_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_update_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_update_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/postgres/test_utils_fns_pg.py` & `dataloom-2.4.2/dataloom/tests/postgres/test_utils_fns_pg.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_aggregation_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_aggregation_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_alter_tables_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_alter_tables_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_connection_options_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_connection_options_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_connection_uri_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_connection_uri_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_create_table_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_create_table_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_delete_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_delete_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_eager_loading_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_eager_loading_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_experimental_decorators_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_experimental_decorators_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_insert_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_insert_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_inspect_table_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_inspect_table_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_operators_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_operators_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_qb_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_qb_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_query_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_query_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_update_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_update_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/tests/sqlite3/test_utils_fns_sqlite.py` & `dataloom-2.4.2/dataloom/tests/sqlite3/test_utils_fns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/types/__init__.py` & `dataloom-2.4.2/dataloom/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/utils/__init__.py` & `dataloom-2.4.2/dataloom/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/utils/aggregations.py` & `dataloom-2.4.2/dataloom/utils/aggregations.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/utils/alter_table.py` & `dataloom-2.4.2/dataloom/utils/alter_table.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/utils/create_table.py` & `dataloom-2.4.2/dataloom/utils/create_table.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/utils/logger.py` & `dataloom-2.4.2/dataloom/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/utils/table.py` & `dataloom-2.4.2/dataloom/utils/table.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom/utils/tables.py` & `dataloom-2.4.2/dataloom/utils/tables.py`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/dataloom.egg-info/PKG-INFO` & `dataloom-2.4.2/dataloom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataloom
-Version: 2.4.1
+Version: 2.4.2
 Summary: dataloom stands as a bespoke Object-Relational Mapping (ORM) solution meticulously crafted to empower Python developers in efficiently managing diverse databases. Unlike conventional ORMs, Dataloom has been built from the ground up, providing native support for SQLite3, PostgreSQL, and MySQL. Navigate effortlessly between database engines while enjoying a tailored and performant ORM experience.
 Author-email: Crispen Gari <crispengari@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 crispengari
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -160,14 +160,15 @@
     - [Inserting](#inserting-3)
     - [Retrieving Records](#retrieving-records-3)
   - [6. `N-N` Relationship](#6-n-n-relationship)
     - [Inserting](#inserting-4)
     - [Retrieving Records](#retrieving-records-4)
 - [Query Builder.](#query-builder)
   - [Why Use Query Builder?](#why-use-query-builder)
+- [Documentation](#documentation)
 - [Contributing](#contributing)
 - [License](#license)
 
 ### Key Features:
 
 - **Lightweight**: `dataloom` is designed to be minimalistic and easy to use, ensuring a streamlined `ORM` experience without unnecessary complexities.
 
@@ -532,22 +533,23 @@
     __tablename__: Optional[TableColumn] = TableColumn(name="users")
     id = PrimaryKeyColumn(type="int", auto_increment=True)
     #...rest of your columns
 
 ```
 
 The following are the arguments that the `PrimaryKeyColumn` class accepts.
-| Argument | Description | Type | Default |
-| ---------------- | ------------------------------------------------------------------------------------------------------------------------ | --------------- | ------------- |
-| `type` | The datatype of your primary key. | `str` | `"int`" |
-| `length` | Optional to specify the length of the type. If passed as `N` with type `T`, it yields an SQL statement with type `T(N)`. | `int` \| `None` | `None` |
-| `auto_increment`| Optional to specify if the column will automatically increment or not. |`bool` |`False` |
-|`default` | Optional to specify the default value in a column. |`any` |`None` |
-|`nullable` | Optional to specify if the column will allow null values or not. |`bool` |`False` |
-|`unique` | Optional to specify if the column will contain unique values or not. |`bool` |`True` |
+
+| Argument         | Description                                                                                                              | Type            | Default |
+| ---------------- | ------------------------------------------------------------------------------------------------------------------------ | --------------- | ------- |
+| `type`           | The datatype of your primary key.                                                                                        | `str`           | `"int`" |
+| `length`         | Optional to specify the length of the type. If passed as `N` with type `T`, it yields an SQL statement with type `T(N)`. | `int` \| `None` | `None`  |
+| `auto_increment` | Optional to specify if the column will automatically increment or not.                                                   | `bool`          | `False` |
+| `default`        | Optional to specify the default value in a column.                                                                       | `any`           | `None`  |
+| `nullable`       | Optional to specify if the column will allow null values or not.                                                         | `bool`          | `False` |
+| `unique`         | Optional to specify if the column will contain unique values or not.                                                     | `bool`          | `True`  |
 
 #### `ForeignKeyColumn` Class
 
 This class is utilized when informing `dataloom` that a column has a relationship with a primary key in another table. Consider the following model definition of a `Post`:
 
 ```py
 class Post(Model):
@@ -750,15 +752,15 @@
     conn.close()
 ```
 
 Returns a `conn` and the list of `tablenames` that exist in the database. The method accepts the same arguments as the `sync` method.
 
 ### CRUD Operations with Dataloom
 
-In this section of the documentation, we will illustrate how to perform basic `CRUD` operations using `dataloom` on simple `Models`. Please note that in the following code snippets, I will be utilizing `sqlite_loom`. However, it's important to highlight that you can use any `loom` of your choice to follow along.
+In this section of the documentation, we will illustrate how to perform basic `CRUD` operations using `dataloom` on simple `Models`. Please note that in the following code snippets, I will be utilizing `sqlite_loom`, `mysql_loom`, `pg_loom` or `loom` interchangeably. However, it's important to highlight that you can use any `loom` of your choice to follow along.
 
 #### 1. Creating a Record
 
 To insert a single or multiple records in a database you make use of the following functions:
 
 1. `insert_one()`
 2. `insert_bulk()`
@@ -892,15 +894,15 @@
 | `filters`  | Collection of `Filter` or a `Filter` to apply to the query.                                | `list[Filter] \| Filter` | `None`  | `No`     |
 | `distinct` | Boolean telling dataloom to return distinct row values based on selected fields or not.    | `bool`                   | `False` | `No`     |
 
 > 👍 **Pro Tip**: The distinction between the `find_all()` and `find_many()` methods lies in the fact that `find_many()` enables you to apply specific filters, whereas `find_all()` retrieves all the documents within the specified model.
 
 ##### 3. `find_one()`
 
-Here is an example showing you how you can use `find_by_pk()` locate a single record in the database.
+Here is an example showing you how you can use `find_one()` locate a single record in the database.
 
 ```py
 user = mysql_loom.find_one(
     User,
     filters=[Filter(column="username", value="@miller")],
     select=["id", "username"],
 )
@@ -1086,16 +1088,19 @@
 To mitigate the potential risks associated with `delete_bulk()`, follow these guidelines:
 
 1. **Always Provide a Filter:**
 
    - When calling `delete_bulk()`, make sure to provide a filter to specify the subset of records to be deleted. This helps prevent unintentional deletions.
 
    ```python
-   # Example: Delete records where 'status' is 'inactive'
-   sqlite_loom.delete_bulk(filter={'status': 'inactive'})
+    # Example: Delete records where 'status' is 'inactive'
+    affected_rows = mysql_loom.delete_bulk(
+        instance=User,
+        filters=Filter(column="status",  value='inactive'),
+    )
    ```
 
 2. **Consider Usage When Necessary:**
 
 - When contemplating data deletion, it is advisable to consider more targeted methods before resorting to `delete_bulk()`. Prioritize the use of `delete_one()` or `delete_by_pk()` methods to remove specific records based on your needs. This ensures a more precise and controlled approach to data deletion.
 
 3. **Use limit and offsets options**
@@ -2526,14 +2531,18 @@
 
   ```python
   qb = loom.getQueryBuilder()
   result = qb.run("SELECT * FROM table1 INNER JOIN table2 ON table1.id = table2.table1_id;")
   print(result)
   ```
 
+### Documentation
+
+You can read the full documentation of dataloom on [readthedocs.io](https://dataloom-py.readthedocs.io/en/latest/)
+
 ### Contributing
 
 Contributions to `dataloom` are welcome! Feel free to submit bug reports, feature requests, or pull requests on [GitHub](https://github.com/CrispenGari/dataloom).
 
 ### License
 
 This project is licensed under the MIT License - see the [LICENSE](/LISENSE) file for details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dataloom Version: 2.4.1 Summary: dataloom stands as
+Metadata-Version: 2.1 Name: dataloom Version: 2.4.2 Summary: dataloom stands as
 a bespoke Object-Relational Mapping (ORM) solution meticulously crafted to
 empower Python developers in efficiently managing diverse databases. Unlike
 conventional ORMs, Dataloom has been built from the ground up, providing native
 support for SQLite3, PostgreSQL, and MySQL. Navigate effortlessly between
 database engines while enjoying a tailored and performant ORM experience.
 Author-email: Crispen Gari
 gmail.com> License: MIT License Copyright (c) 2024 crispengari Permission is
@@ -95,38 +95,39 @@
 [Inserting](#inserting-2) - [Retrieving Records](#retrieving-records-2) - [4.
 What about bidirectional queries?](#4-what-about-bidirectional-queries) - [1.
 Child to Parent](#1-child-to-parent) - [2. Parent to Child](#2-parent-to-child)
 - [5. `Self` Association](#5-self-association) - [Inserting](#inserting-3) -
 [Retrieving Records](#retrieving-records-3) - [6. `N-N` Relationship](#6-n-n-
 relationship) - [Inserting](#inserting-4) - [Retrieving Records](#retrieving-
 records-4) - [Query Builder.](#query-builder) - [Why Use Query Builder?](#why-
-use-query-builder) - [Contributing](#contributing) - [License](#license) ###
-Key Features: - **Lightweight**: `dataloom` is designed to be minimalistic and
-easy to use, ensuring a streamlined `ORM` experience without unnecessary
-complexities. - **Database Support**: `dataloom` supports popular relational
-databases such as `PostgreSQL`, `MySQL`, and `SQLite3`, making it suitable for
-a variety of projects. - **Simplified Querying**: The `ORM` simplifies the
-process of database querying, allowing developers to interact with the database
-using Python classes and methods rather than raw SQL queries. - **Intuitive
-Syntax**: `dataloom`'s syntax is intuitive and `Pythonic`, making it accessible
-for developers familiar with the Python language. - **Flexible Data Types**:
-The `ORM` seamlessly handles various data types, offering flexibility in
-designing database schemas. ### Installation To install `dataloom`, you just
-need to run the following command using `pip`: ```bash pip install dataloom ```
-### Python Version Compatibility `dataloom` supports **`Python`** version
-**`3.12`** and above. Ensure that you are using a compatible version of
-**`Python`** before installing or using `dataloom`. You can check your
-**`Python`** version by running: ```bash python --version ``` ### Usage In this
-section we are going to go through how you can use our `orm` package in your
-project. ### Connection To use Dataloom, you need to establish a connection
-with a specific database `dialect`. The available dialect options are `mysql`,
-`postgres`, and `sqlite`. #### `Postgres` The following is an example of how
-you can establish a connection with postgres database. ```python from dataloom
-import Loom # Create a Loom instance with PostgreSQL configuration pg_loom =
-Loom( dialect="postgres", database="hi", password="root", user="postgres",
+use-query-builder) - [Documentation](#documentation) - [Contributing]
+(#contributing) - [License](#license) ### Key Features: - **Lightweight**:
+`dataloom` is designed to be minimalistic and easy to use, ensuring a
+streamlined `ORM` experience without unnecessary complexities. - **Database
+Support**: `dataloom` supports popular relational databases such as
+`PostgreSQL`, `MySQL`, and `SQLite3`, making it suitable for a variety of
+projects. - **Simplified Querying**: The `ORM` simplifies the process of
+database querying, allowing developers to interact with the database using
+Python classes and methods rather than raw SQL queries. - **Intuitive Syntax**:
+`dataloom`'s syntax is intuitive and `Pythonic`, making it accessible for
+developers familiar with the Python language. - **Flexible Data Types**: The
+`ORM` seamlessly handles various data types, offering flexibility in designing
+database schemas. ### Installation To install `dataloom`, you just need to run
+the following command using `pip`: ```bash pip install dataloom ``` ### Python
+Version Compatibility `dataloom` supports **`Python`** version **`3.12`** and
+above. Ensure that you are using a compatible version of **`Python`** before
+installing or using `dataloom`. You can check your **`Python`** version by
+running: ```bash python --version ``` ### Usage In this section we are going to
+go through how you can use our `orm` package in your project. ### Connection To
+use Dataloom, you need to establish a connection with a specific database
+`dialect`. The available dialect options are `mysql`, `postgres`, and `sqlite`.
+#### `Postgres` The following is an example of how you can establish a
+connection with postgres database. ```python from dataloom import Loom # Create
+a Loom instance with PostgreSQL configuration pg_loom = Loom
+( dialect="postgres", database="hi", password="root", user="postgres",
 host="localhost", sql_logger="console", logs_filename="logs.sql", port=5432, )
 # Connect to the PostgreSQL database conn = pg_loom.connect() # Close the
 connection when the script completes if __name__ == "__main__": conn.close()
 ``` In `dataloom` you can use connection uris to establish a connection to the
 database in `postgres` as follows: ```py pg_loom = Loom( dialect="postgres",
 connection_uri = "postgressql://root:root@localhost:5432/hi", # ... ) ``` This
 will establish a connection with `postgres` with the database `hi`. ####
@@ -286,121 +287,120 @@
 `PrimaryKeyColumn` is required. Below is an example of creating an `id` column
 as a primary key in a table named `Post`: ```python class Post(Model):
 __tablename__: Optional[TableColumn] = TableColumn(name="users") id =
 PrimaryKeyColumn(type="int", auto_increment=True) #...rest of your columns ```
 The following are the arguments that the `PrimaryKeyColumn` class accepts. |
 Argument | Description | Type | Default | | ---------------- | ----------------
 -------------------------------------------------------------------------------
-------------------------- | --------------- | ------------- | | `type` | The
-datatype of your primary key. | `str` | `"int`" | | `length` | Optional to
-specify the length of the type. If passed as `N` with type `T`, it yields an
-SQL statement with type `T(N)`. | `int` \| `None` | `None` | |
-`auto_increment`| Optional to specify if the column will automatically
-increment or not. |`bool` |`False` | |`default` | Optional to specify the
-default value in a column. |`any` |`None` | |`nullable` | Optional to specify
-if the column will allow null values or not. |`bool` |`False` | |`unique` |
-Optional to specify if the column will contain unique values or not. |`bool`
-|`True` | #### `ForeignKeyColumn` Class This class is utilized when informing
-`dataloom` that a column has a relationship with a primary key in another
-table. Consider the following model definition of a `Post`: ```py class Post
-(Model): __tablename__: Optional[TableColumn] = TableColumn(name="posts") id =
-PrimaryKeyColumn(type="int", auto_increment=True, nullable=False, unique=True)
-completed = Column(type="boolean", default=False) title = Column
-(type="varchar", length=255, nullable=False) # timestamps createdAt =
-CreatedAtColumn() updatedAt = UpdatedAtColumn() # relations userId =
-ForeignKeyColumn( User, type="int", required=True, onDelete="CASCADE",
-onUpdate="CASCADE" ) ``` - `userId` is a foreign key in the table `posts`,
-indicating it has a relationship with a primary key in the `users` table. This
-column accepts the following arguments: | Argument | Description | Type |
-Default | | ---------- | ------------------------------------------------------
--------------------------------------------------------------- | --------------
--------------------------- | ----------- | | `table` | Required. This is the
-parent table that the current model references. In our example, this is
-referred to as `User`. It can be used as a string in self relations. |
-`Model`\| `str` | | | `type` | Optional. Specifies the data type of the foreign
-key. If not provided, dataloom can infer it from the parent table. | `str` \|
-`None` | `None` | | `required` | Optional. Indicates whether the foreign key is
-required or not. | `bool` | `False` | | `onDelete` | Optional. Specifies the
-action to be taken when the associated record in the parent table is deleted.
-|`"NO ACTION"`, `"SET NULL"`, `"CASCADE"` | `"NO ACTION"` | | `onUpdate` |
-Optional. Specifies the action to be taken when the associated record in the
-parent table is updated. | `"NO ACTION"`, `"SET NULL"`, `"CASCADE"`| `"NO
-ACTION"` | It is crucial to specify the actions for `onDelete` and `onUpdate`
-to ensure that `dataloom` manages your model's relationship actions
-appropriately. The available actions are: 1. `"NO ACTION"` - If you delete or
-update the parent table, no changes will occur in the child table. 2. `"SET
-NULL"` - If you delete or update the parent table, the corresponding value in
-the child table will be set to `null`. 3. `"CASCADE"` - If you delete or update
-the table, the same action will also be applied to the child table. ####
-`CreatedAtColumn` Class When a column is designated as `CreatedAtColumn`, its
-value will be automatically generated each time you create a new record in a
-database, serving as a timestamp. #### `UpdatedAtColumn` Class When a column is
-designated as `UpdatedAtColumn`, its value will be automatically generated each
-time you create a new record or update an existing record in a database table,
-acting as a timestamp. #### `Filter` Class This `Filter` class in `dataloom` is
-designed to facilitate the application of filters when executing queries and
-mutations. It allows users to specify conditions that must be met for the
-operation to affect certain rows in a database table. Below is an example
-demonstrating how this class can be used: ```python affected_rows =
-pg_loom.update_one( Post, values=[ ColumnValue(name="title", value="Hey"),
-ColumnValue(name="completed", value=True), ], filters=[ Filter(column="id",
-value=1, join_next_with="AND"), Filter(column="userId", value=1,
-join_next_with="AND"), ], ) ``` So from the above example we are applying
-filters while updating a `Post` here are the options that you can pass on that
-filter class: | Argument | Description | Type | Default | |--------------------
------|------------------------------------------------------------|------------
--------------------------------|------------------------| | `column` | The name
-of the column to apply the filter on | `String` | - | | `value` | The value to
-filter against | `Any` | - | | `operator` | The comparison operator to use for
-the filter | `'eq'`, `'neq'`. `'lt'`, `'gt'`, `'leq'`, `'geq'`, `'in'`,
-`'notIn'`, `'like'`, `'between'`, `'not'` | `'eq'` | | `join_next_with` | The
-logical operator to join this filter with the next one | `'AND'`, `'OR'` |
-`'AND'` | > ð**Pro Tip:** Note You can apply either a list of filters or a
-single filter when filtering records. #### `ColumnValue` Class Just like the
-`Filter` class, `dataloom` also provides a `ColumnValue` class. This class acts
-as a setter to update the values of columns in your database table. The
-following code snippet demonstrates how the `ColumnValue` class is used to
-update records in the database: ```py re = pg_loom.update_one( Post, values=
-[ ColumnValue(name="title", value="Hey"), ColumnValue(name="completed",
-value=True), ], filters=[ Filter(column="id", value=1, join_next_with="AND"),
-Filter(column="userId", value=1, join_next_with="AND"), ], ) ``` It accepts two
-arguments: `name` and `value`. name represents the column name, while value
-corresponds to the new value to be assigned to that column. | Argument |
-Description | Type | Default | | -------- | -----------------------------------
------------------------ | ----- | ------- | | `name` | The name of the column
-to be updated or inserted. | `str` | - | | `value` | The value to assign to the
-column during update or insert. | `Any` | - | #### `Order` Class The `Order`
-class enables us to specify the desired order in which documents should be
-returned. Below is an example illustrating its usage: ```py posts =
-pg_loom.find_all( Post, select=["id", "completed", "title", "createdAt"],
-limit=3, offset=0, order=[ Order(column="createdAt", order="ASC"), Order
-(column="id", order="DESC"), ] ) ``` > ð**Pro Tip:** Note when utilizing a
-list of orders, they are applied sequentially, one after the other: | Argument
-| Description | Type | Default | | -------- | ---------------------------------
----------------------------------------- | ------------------- | ------- | |
-`column` | The name of the column to order by. | `str` | - | | `order` | The
-order direction, either `"ASC"` (ascending) or `"DESC"` (descending). | `"ASC"`
-or `"DESC"` | `"ASC"` | #### `Include` Class The `Include` class facilitates
-eager loading for models with relationships. Below is a table detailing the
-parameters available for the `Include` class: | Argument | Description | Type |
-Default | Required | | ---------------- | -------------------------------------
------------------------------------------------------- | ------------------- |
--------- | -------- | | `model` | The model to be included when eagerly
-fetching records. | `Model` | - | Yes | | `junction_table` | The
-`junction_table` model that is used as a reference table in a many to many
-association. | `Model` | `None` | No | | `order` | The list of order
-specifications for sorting the included data. | `list[Order]` | `[]` | No | |
-`limit` | The maximum number of records to include. | `int \| None` | `0` | No
-| | `offset` | The number of records to skip before including. | `int \| None`
-| `0` | No | | `select` | The list of columns to include. | `list[str] \| None`
-| `None` | No | | `has` | The relationship type between the current model and
-the included model. | `INCLUDE_LITERAL` | `"many"` | No | | `include` | The
-extra included models. | `list[Include]` | `[]` | No | | `alias` | The alias
-name for the included model. Very important when mapping self relations. |
-`str` | `None` | No | #### `Group` Class This class is used for data
+------------------------- | --------------- | ------- | | `type` | The datatype
+of your primary key. | `str` | `"int`" | | `length` | Optional to specify the
+length of the type. If passed as `N` with type `T`, it yields an SQL statement
+with type `T(N)`. | `int` \| `None` | `None` | | `auto_increment` | Optional to
+specify if the column will automatically increment or not. | `bool` | `False` |
+| `default` | Optional to specify the default value in a column. | `any` |
+`None` | | `nullable` | Optional to specify if the column will allow null
+values or not. | `bool` | `False` | | `unique` | Optional to specify if the
+column will contain unique values or not. | `bool` | `True` | ####
+`ForeignKeyColumn` Class This class is utilized when informing `dataloom` that
+a column has a relationship with a primary key in another table. Consider the
+following model definition of a `Post`: ```py class Post(Model): __tablename__:
+Optional[TableColumn] = TableColumn(name="posts") id = PrimaryKeyColumn
+(type="int", auto_increment=True, nullable=False, unique=True) completed =
+Column(type="boolean", default=False) title = Column(type="varchar",
+length=255, nullable=False) # timestamps createdAt = CreatedAtColumn()
+updatedAt = UpdatedAtColumn() # relations userId = ForeignKeyColumn( User,
+type="int", required=True, onDelete="CASCADE", onUpdate="CASCADE" ) ``` -
+`userId` is a foreign key in the table `posts`, indicating it has a
+relationship with a primary key in the `users` table. This column accepts the
+following arguments: | Argument | Description | Type | Default | | ---------- |
+-------------------------------------------------------------------------------
+------------------------------------- | ---------------------------------------
+- | ----------- | | `table` | Required. This is the parent table that the
+current model references. In our example, this is referred to as `User`. It can
+be used as a string in self relations. | `Model`\| `str` | | | `type` |
+Optional. Specifies the data type of the foreign key. If not provided, dataloom
+can infer it from the parent table. | `str` \| `None` | `None` | | `required` |
+Optional. Indicates whether the foreign key is required or not. | `bool` |
+`False` | | `onDelete` | Optional. Specifies the action to be taken when the
+associated record in the parent table is deleted. |`"NO ACTION"`, `"SET NULL"`,
+`"CASCADE"` | `"NO ACTION"` | | `onUpdate` | Optional. Specifies the action to
+be taken when the associated record in the parent table is updated. | `"NO
+ACTION"`, `"SET NULL"`, `"CASCADE"`| `"NO ACTION"` | It is crucial to specify
+the actions for `onDelete` and `onUpdate` to ensure that `dataloom` manages
+your model's relationship actions appropriately. The available actions are: 1.
+`"NO ACTION"` - If you delete or update the parent table, no changes will occur
+in the child table. 2. `"SET NULL"` - If you delete or update the parent table,
+the corresponding value in the child table will be set to `null`. 3.
+`"CASCADE"` - If you delete or update the table, the same action will also be
+applied to the child table. #### `CreatedAtColumn` Class When a column is
+designated as `CreatedAtColumn`, its value will be automatically generated each
+time you create a new record in a database, serving as a timestamp. ####
+`UpdatedAtColumn` Class When a column is designated as `UpdatedAtColumn`, its
+value will be automatically generated each time you create a new record or
+update an existing record in a database table, acting as a timestamp. ####
+`Filter` Class This `Filter` class in `dataloom` is designed to facilitate the
+application of filters when executing queries and mutations. It allows users to
+specify conditions that must be met for the operation to affect certain rows in
+a database table. Below is an example demonstrating how this class can be used:
+```python affected_rows = pg_loom.update_one( Post, values=[ ColumnValue
+(name="title", value="Hey"), ColumnValue(name="completed", value=True), ],
+filters=[ Filter(column="id", value=1, join_next_with="AND"), Filter
+(column="userId", value=1, join_next_with="AND"), ], ) ``` So from the above
+example we are applying filters while updating a `Post` here are the options
+that you can pass on that filter class: | Argument | Description | Type |
+Default | |-------------------------|------------------------------------------
+------------------|-------------------------------------------|----------------
+--------| | `column` | The name of the column to apply the filter on | `String`
+| - | | `value` | The value to filter against | `Any` | - | | `operator` | The
+comparison operator to use for the filter | `'eq'`, `'neq'`. `'lt'`, `'gt'`,
+`'leq'`, `'geq'`, `'in'`, `'notIn'`, `'like'`, `'between'`, `'not'` | `'eq'` |
+| `join_next_with` | The logical operator to join this filter with the next one
+| `'AND'`, `'OR'` | `'AND'` | > ð**Pro Tip:** Note You can apply either a
+list of filters or a single filter when filtering records. #### `ColumnValue`
+Class Just like the `Filter` class, `dataloom` also provides a `ColumnValue`
+class. This class acts as a setter to update the values of columns in your
+database table. The following code snippet demonstrates how the `ColumnValue`
+class is used to update records in the database: ```py re = pg_loom.update_one
+( Post, values=[ ColumnValue(name="title", value="Hey"), ColumnValue
+(name="completed", value=True), ], filters=[ Filter(column="id", value=1,
+join_next_with="AND"), Filter(column="userId", value=1, join_next_with="AND"),
+], ) ``` It accepts two arguments: `name` and `value`. name represents the
+column name, while value corresponds to the new value to be assigned to that
+column. | Argument | Description | Type | Default | | -------- | --------------
+-------------------------------------------- | ----- | ------- | | `name` | The
+name of the column to be updated or inserted. | `str` | - | | `value` | The
+value to assign to the column during update or insert. | `Any` | - | ####
+`Order` Class The `Order` class enables us to specify the desired order in
+which documents should be returned. Below is an example illustrating its usage:
+```py posts = pg_loom.find_all( Post, select=["id", "completed", "title",
+"createdAt"], limit=3, offset=0, order=[ Order(column="createdAt",
+order="ASC"), Order(column="id", order="DESC"), ] ) ``` > ð**Pro Tip:** Note
+when utilizing a list of orders, they are applied sequentially, one after the
+other: | Argument | Description | Type | Default | | -------- | ---------------
+---------------------------------------------------------- | ------------------
+- | ------- | | `column` | The name of the column to order by. | `str` | - | |
+`order` | The order direction, either `"ASC"` (ascending) or `"DESC"`
+(descending). | `"ASC"` or `"DESC"` | `"ASC"` | #### `Include` Class The
+`Include` class facilitates eager loading for models with relationships. Below
+is a table detailing the parameters available for the `Include` class: |
+Argument | Description | Type | Default | Required | | ---------------- | -----
+-------------------------------------------------------------------------------
+------- | ------------------- | -------- | -------- | | `model` | The model to
+be included when eagerly fetching records. | `Model` | - | Yes | |
+`junction_table` | The `junction_table` model that is used as a reference table
+in a many to many association. | `Model` | `None` | No | | `order` | The list
+of order specifications for sorting the included data. | `list[Order]` | `[]` |
+No | | `limit` | The maximum number of records to include. | `int \| None` |
+`0` | No | | `offset` | The number of records to skip before including. | `int
+\| None` | `0` | No | | `select` | The list of columns to include. | `list[str]
+\| None` | `None` | No | | `has` | The relationship type between the current
+model and the included model. | `INCLUDE_LITERAL` | `"many"` | No | | `include`
+| The extra included models. | `list[Include]` | `[]` | No | | `alias` | The
+alias name for the included model. Very important when mapping self relations.
+| `str` | `None` | No | #### `Group` Class This class is used for data
 `aggregation` and grouping data in `dataloom`. Below is a table detailing the
 parameters available for the `Group` class: | Argument | Description | Type |
 Default | Required | | --------------------------- | --------------------------
 ----------------------------- | --------------------------------------------- |
 --------- | -------- | | `column` | The name of the column to group by. | `str`
 | | Yes | | `function` | The aggregation function to apply on the grouped data.
 | `"COUNT" \| "AVG" \| "SUM" \| "MIN" \| "MAX"` | `"COUNT"` | No | | `having` |
@@ -446,72 +446,73 @@
 logs.sql", logging=True ) conn, tables = sqlite_loom.connect_and_sync([Post,
 User], drop=True, force=True) print(tables) if __name__ == "__main__":
 conn.close() ``` Returns a `conn` and the list of `tablenames` that exist in
 the database. The method accepts the same arguments as the `sync` method. ###
 CRUD Operations with Dataloom In this section of the documentation, we will
 illustrate how to perform basic `CRUD` operations using `dataloom` on simple
 `Models`. Please note that in the following code snippets, I will be utilizing
-`sqlite_loom`. However, it's important to highlight that you can use any `loom`
-of your choice to follow along. #### 1. Creating a Record To insert a single or
-multiple records in a database you make use of the following functions: 1.
-`insert_one()` 2. `insert_bulk()` ##### 1. `insert_one()` The `insert_one`
-method allows you to save a single row in a specific table. Upon saving, it
-will return the primary key (`pk`) value of the inserted document. The
-following example shows how the `insert_one()` method works. ```python #
-Example: Creating a user record userId = pg_loom.insert_one( instance=User,
-values=ColumnValue(name="username", value="@miller") ) userId =
-pg_loom.insert_one( instance=User, values=[ ColumnValue(name="username",
-value="@miller"), ColumnValue(name="name", value="Jonh"), ], ) ``` This
-function takes in two arguments which are `instance` and `values`. Where values
-are the column values that you are inserting in a user table or a single column
-value. | Argument | Description | `Type` | `Required` | `Default` | | ---------
-- | ---------------------------------------------------------------------------
---------------------------------- | ------------------------------------ | ----
------- | --------- | | `instance` | The instance of the table where the row
-will be inserted. | `Model` | `Yes` | `None` | | `values` | The column values
-to be inserted into the table. It can be a single column value or a list of
-column values. | `list[ColumnValue]` or `ColumnValue` | `Yes` | `None` | #####
-2. `insert_bulk()`. The `insert_bulk` method facilitates the bulk insertion of
-records, as its name suggests. The following example illustrates how you can
-add `3` posts to the database table simultaneously. ```python # Example:
-Inserting multiple posts rows = pg_loom.insert_bulk( User, values=[
+`sqlite_loom`, `mysql_loom`, `pg_loom` or `loom` interchangeably. However, it's
+important to highlight that you can use any `loom` of your choice to follow
+along. #### 1. Creating a Record To insert a single or multiple records in a
+database you make use of the following functions: 1. `insert_one()` 2.
+`insert_bulk()` ##### 1. `insert_one()` The `insert_one` method allows you to
+save a single row in a specific table. Upon saving, it will return the primary
+key (`pk`) value of the inserted document. The following example shows how the
+`insert_one()` method works. ```python # Example: Creating a user record userId
+= pg_loom.insert_one( instance=User, values=ColumnValue(name="username",
+value="@miller") ) userId = pg_loom.insert_one( instance=User, values=
 [ ColumnValue(name="username", value="@miller"), ColumnValue(name="name",
-value="Jonh"), ], [ ColumnValue(name="username", value="@brown"), ColumnValue
-(name="name", value="Jonh"), ], [ ColumnValue(name="username", value="@blue"),
-ColumnValue(name="name", value="Jonh"), ], ], ) ``` The argument parameters for
-the `insert_bulk` methods are as follows. | Argument | Description | `Type` |
-`Required` | `Default` | | ---------- | ---------------------------------------
--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
------- | ------------------------------------------ | ---------- | --------- |
-| `instance` | The instance of the table where the row will be inserted. |
+value="Jonh"), ], ) ``` This function takes in two arguments which are
+`instance` and `values`. Where values are the column values that you are
+inserting in a user table or a single column value. | Argument | Description |
+`Type` | `Required` | `Default` | | ---------- | ------------------------------
+-----------------------------------------------------------------------------
+- | ------------------------------------ | ---------- | --------- | |
+`instance` | The instance of the table where the row will be inserted. |
 `Model` | `Yes` | `None` | | `values` | The column values to be inserted into
-the table. **It must be a list of list of column values with the same length,
-otherwise dataloom will fail to map the values correctly during the insert
-operation.** | `list[list[ColumnValue]]` or `ColumnValue` | `Yes` | `None` | >
-In contrast to the `insert_one` method, the `insert_bulk` method returns the
-row count of the inserted documents rather than the individual primary keys
-(`pks`) of those documents. #### 2. Reading records To retrieve documents or a
-document from the database, you can make use of the following functions: 1.
-`find_all()`: This function is used to retrieve all documents from the
-database. 2. `find_by_pk()`: This function is used to retrieve a document by
-its primary key (or ID). 3. `find_one()`: This function is used to retrieve a
-single document based on a specific condition. 4. `find_many()`: This function
-is used to retrieve multiple documents based on a specific condition. ##### 1.
-`find_all()` This method is used to retrieve all the records that are in the
-database table. Below are examples demonstrating how to do it: ```py users =
-pg_loom.find_all( instance=User, select=["id", "username"], limit=3, offset=0,
-order=[Order(column="id", order="DESC")], ) print(users) # ? [{'id': 1,
-'username': '@miller'}] ``` The `find_all()` method takes in the following
-arguments: | Argument | Description | Type | Default | Required | | ---------
-- | ---------------------------------------------------------------------------
---------------- | ------------------------ | ------- | -------- | | `instance`
-| The model class to retrieve documents from. | `Model` | `None` | `Yes` | |
-`select` | Collection or a string of fields to select from the documents. |
-`list[str]\|str` | `None` | `No` | | `limit` | Maximum number of documents to
+the table. It can be a single column value or a list of column values. | `list
+[ColumnValue]` or `ColumnValue` | `Yes` | `None` | ##### 2. `insert_bulk()`.
+The `insert_bulk` method facilitates the bulk insertion of records, as its name
+suggests. The following example illustrates how you can add `3` posts to the
+database table simultaneously. ```python # Example: Inserting multiple posts
+rows = pg_loom.insert_bulk( User, values=[ [ ColumnValue(name="username",
+value="@miller"), ColumnValue(name="name", value="Jonh"), ], [ ColumnValue
+(name="username", value="@brown"), ColumnValue(name="name", value="Jonh"), ],
+[ ColumnValue(name="username", value="@blue"), ColumnValue(name="name",
+value="Jonh"), ], ], ) ``` The argument parameters for the `insert_bulk`
+methods are as follows. | Argument | Description | `Type` | `Required` |
+`Default` | | ---------- | ----------------------------------------------------
+-------------------------------------------------------------------------------
+------------------------------------------------------------------------ | ----
+-------------------------------------- | ---------- | --------- | | `instance`
+| The instance of the table where the row will be inserted. | `Model` | `Yes` |
+`None` | | `values` | The column values to be inserted into the table. **It
+must be a list of list of column values with the same length, otherwise
+dataloom will fail to map the values correctly during the insert operation.** |
+`list[list[ColumnValue]]` or `ColumnValue` | `Yes` | `None` | > In contrast to
+the `insert_one` method, the `insert_bulk` method returns the row count of the
+inserted documents rather than the individual primary keys (`pks`) of those
+documents. #### 2. Reading records To retrieve documents or a document from the
+database, you can make use of the following functions: 1. `find_all()`: This
+function is used to retrieve all documents from the database. 2. `find_by_pk
+()`: This function is used to retrieve a document by its primary key (or ID).
+3. `find_one()`: This function is used to retrieve a single document based on a
+specific condition. 4. `find_many()`: This function is used to retrieve
+multiple documents based on a specific condition. ##### 1. `find_all()` This
+method is used to retrieve all the records that are in the database table.
+Below are examples demonstrating how to do it: ```py users = pg_loom.find_all
+( instance=User, select=["id", "username"], limit=3, offset=0, order=[Order
+(column="id", order="DESC")], ) print(users) # ? [{'id': 1, 'username':
+'@miller'}] ``` The `find_all()` method takes in the following arguments: |
+Argument | Description | Type | Default | Required | | ---------- | -----------
+------------------------------------------------------------------------------
+- | ------------------------ | ------- | -------- | | `instance` | The model
+class to retrieve documents from. | `Model` | `None` | `Yes` | | `select` |
+Collection or a string of fields to select from the documents. | `list
+[str]\|str` | `None` | `No` | | `limit` | Maximum number of documents to
 retrieve. | `int` | `None` | `No` | | `offset` | Number of documents to skip
 before retrieving. | `int` | `0` | `No` | | `order` | Collection of `Order` or
 a single `Order` to order the documents when querying. | `list[Order]\|Order` |
 `None` | `No` | | `include` | Collection or a `Include` of related models to
 eagerly load. | `list[Include]\|Include` | `None` | `No` | | `group` |
 Collection of `Group` which specifies how you want your data to be grouped
 during queries. | `list[Group]\|Group` | `None` | `No` | | `distinct` | Boolean
@@ -539,15 +540,15 @@
 Collection of `Filter` or a `Filter` to apply to the query. | `list[Filter] \|
 Filter` | `None` | `No` | | `distinct` | Boolean telling dataloom to return
 distinct row values based on selected fields or not. | `bool` | `False` | `No`
 | > ð **Pro Tip**: The distinction between the `find_all()` and `find_many
 ()` methods lies in the fact that `find_many()` enables you to apply specific
 filters, whereas `find_all()` retrieves all the documents within the specified
 model. ##### 3. `find_one()` Here is an example showing you how you can use
-`find_by_pk()` locate a single record in the database. ```py user =
+`find_one()` locate a single record in the database. ```py user =
 mysql_loom.find_one( User, filters=[Filter(column="username",
 value="@miller")], select=["id", "username"], ) print(user) # ? {'id': 1,
 'username': '@miller'} ``` This method take the following as arguments |
 Argument | Description | Type | Default | Required | | ---------- | -----------
 ------------------------------------------------------------------------------
 - | -------------------------------- | ------- | -------- | | `instance` | The
 model class to retrieve instances from. | `Model` | | `Yes` | | `filters` |
@@ -646,174 +647,175 @@
 `delete_bulk()` function, exercise caution as it can be aggressive. If the
 filter is not explicitly provided, there is a risk of mistakenly deleting all
 records in the table. ###### Guidelines for Safe Usage To mitigate the
 potential risks associated with `delete_bulk()`, follow these guidelines: 1.
 **Always Provide a Filter:** - When calling `delete_bulk()`, make sure to
 provide a filter to specify the subset of records to be deleted. This helps
 prevent unintentional deletions. ```python # Example: Delete records where
-'status' is 'inactive' sqlite_loom.delete_bulk(filter={'status': 'inactive'})
-``` 2. **Consider Usage When Necessary:** - When contemplating data deletion,
-it is advisable to consider more targeted methods before resorting to
-`delete_bulk()`. Prioritize the use of `delete_one()` or `delete_by_pk()`
-methods to remove specific records based on your needs. This ensures a more
-precise and controlled approach to data deletion. 3. **Use limit and offsets
-options** - You can consider using the `limit` and offset options during
-invocation of `delete_bulk` ```py affected_rows = mysql_loom.delete_bulk
+'status' is 'inactive' affected_rows = mysql_loom.delete_bulk( instance=User,
+filters=Filter(column="status", value='inactive'), ) ``` 2. **Consider Usage
+When Necessary:** - When contemplating data deletion, it is advisable to
+consider more targeted methods before resorting to `delete_bulk()`. Prioritize
+the use of `delete_one()` or `delete_by_pk()` methods to remove specific
+records based on your needs. This ensures a more precise and controlled
+approach to data deletion. 3. **Use limit and offsets options** - You can
+consider using the `limit` and offset options during invocation of
+`delete_bulk` ```py affected_rows = mysql_loom.delete_bulk( instance=Post,
+order=[Order(column="id", order="DESC"), Order(column="createdAt",
+order="ASC")], filters=[Filter(column="id", operator="gt", value=0)], offset=0,
+limit=10, ) ``` By following these guidelines, you can use the `delete_bulk()`
+function safely and minimize the risk of unintended data loss. Always exercise
+caution and adhere to best practices when performing bulk deletion operations.
+### Ordering In dataloom you can order documents in either `DESC` (descending)
+or `ASC` (ascending) order using the helper class `Order`. ```py posts =
+mysql_loom.find_all( instance=Post, order=[Order(column="id", order="DESC")], )
+``` You can apply multiple and these orders will ba applied in sequence of
+application here is an example: ```py posts = mysql_loom.find_all
 ( instance=Post, order=[Order(column="id", order="DESC"), Order
-(column="createdAt", order="ASC")], filters=[Filter(column="id", operator="gt",
-value=0)], offset=0, limit=10, ) ``` By following these guidelines, you can use
-the `delete_bulk()` function safely and minimize the risk of unintended data
-loss. Always exercise caution and adhere to best practices when performing bulk
-deletion operations. ### Ordering In dataloom you can order documents in either
-`DESC` (descending) or `ASC` (ascending) order using the helper class `Order`.
-```py posts = mysql_loom.find_all( instance=Post, order=[Order(column="id",
-order="DESC")], ) ``` You can apply multiple and these orders will ba applied
-in sequence of application here is an example: ```py posts =
-mysql_loom.find_all( instance=Post, order=[Order(column="id", order="DESC"),
-Order(column="createdAt", order="ASC")], ) ``` ### Filters There are different
-find of filters that you can use when filtering documents for mutations and
-queries. Filters are very important to use when updating and deleting documents
-as they give you control on which documents should be updated or deleted. When
-doing a mutation you can use a single or multiple filters. Bellow is an example
-that shows you how you can use a single filter in deleting a single record that
-has an `id` greater than `1` from the database. ```py res2 =
-mysql_loom.delete_one( instance=Post, offset=0, order=Order(column="id",
-order="DESC"), filters=Filter(column="id", value=1, operator="gt"), ) ``` Or
-you can use it as follows: ```py res2 = mysql_loom.delete_one( instance=Post,
-offset=0, order=[Order(column="id", order="DESC")], filters=[Filter
-(column="id", value=1, operator="gt")], ) ``` As you have noticed, you can join
-your filters together and they will be applied sequentially using the
-[`join_next_with`](#filter-class) which can be either `OR` or `AND` te default
-value is `AND`. Here is an of filter usage in sequential. ```py res2 =
-mysql_loom.delete_one( instance=Post, offset=0, order=[Order(column="id",
-order="DESC")], filters=[ Filter(column="id", value=1, operator="gt"), Filter
-(column="userId", value=1, operator="eq", join_next_with="OR"), Filter
-( column="title", value='"What are you doing general?"', operator="=",
-join_next_with="AND", ), ], ) ``` ##### Operators You can use the `operator` to
-match the values. Here is the table of description for these filters. |
-Operator | Explanation | Expect | | ----------- | -----------------------------
-------------------------------------------------------------------------------
-- | --------------------- | | `'eq'` | Indicates equality. It checks if the
-value is equal to the specified criteria. | Value == Criteria | | `'lt'` |
-Denotes less than. It checks if the value is less than the specified criteria.
-| Value < Criteria | | `'gt'` | Denotes greater than. It checks if the value is
-greater than the specified criteria. | Value > Criteria | | `'leq'` | Denotes
-less than or equal to. It checks if the value is less than or equal to the
-specified criteria. | Value <= Criteria | | `'geq'` | Denotes greater than or
-equal to. It checks if the value is greater than or equal to the specified
-criteria. | Value >= Criteria | | `'in'` | Checks if the value is included in a
-specified list of values. | Value in List | | `'notIn'` | Checks if the value
-is not included in a specified list of values. | Value not in List | | `'like'`
-| Performs a pattern matching operation. It checks if the value is similar to a
-specified pattern. | Value matches Pattern | | `'not'` | Indicates non-
-equality. It checks if the column value that does not equal to the specified
-criteria. | NOT id = Criteria | | `'neq'` | Indicates non-equality. It checks
-if the value is not equal to the specified criteria. | Value != Criteria | |
-`'between'` | It checks range values that matches a given range between the
-minimum and maximum. | id BETWEEN (min, max) | Let's talk about these filters
-in detail of code by example. Let's say you want to update a `Post` where the
-`id` matches `1` you can do it as follows: ```py res2 = mysql_loom.update_one
-( instance=Post, filters=Filter( column="id", value=1, operator="eq", ),
-values=[ColumnValue(name="title", value="Bob")], ) ``` What if you want to
-update a post where `id` is not equal to `1` you can do it as follows ```py
+(column="createdAt", order="ASC")], ) ``` ### Filters There are different find
+of filters that you can use when filtering documents for mutations and queries.
+Filters are very important to use when updating and deleting documents as they
+give you control on which documents should be updated or deleted. When doing a
+mutation you can use a single or multiple filters. Bellow is an example that
+shows you how you can use a single filter in deleting a single record that has
+an `id` greater than `1` from the database. ```py res2 = mysql_loom.delete_one
+( instance=Post, offset=0, order=Order(column="id", order="DESC"),
+filters=Filter(column="id", value=1, operator="gt"), ) ``` Or you can use it as
+follows: ```py res2 = mysql_loom.delete_one( instance=Post, offset=0, order=
+[Order(column="id", order="DESC")], filters=[Filter(column="id", value=1,
+operator="gt")], ) ``` As you have noticed, you can join your filters together
+and they will be applied sequentially using the [`join_next_with`](#filter-
+class) which can be either `OR` or `AND` te default value is `AND`. Here is an
+of filter usage in sequential. ```py res2 = mysql_loom.delete_one
+( instance=Post, offset=0, order=[Order(column="id", order="DESC")], filters=
+[ Filter(column="id", value=1, operator="gt"), Filter(column="userId", value=1,
+operator="eq", join_next_with="OR"), Filter( column="title", value='"What are
+you doing general?"', operator="=", join_next_with="AND", ), ], ) ``` #####
+Operators You can use the `operator` to match the values. Here is the table of
+description for these filters. | Operator | Explanation | Expect | | ----------
+- | ---------------------------------------------------------------------------
+--------------------------------- | --------------------- | | `'eq'` |
+Indicates equality. It checks if the value is equal to the specified criteria.
+| Value == Criteria | | `'lt'` | Denotes less than. It checks if the value is
+less than the specified criteria. | Value < Criteria | | `'gt'` | Denotes
+greater than. It checks if the value is greater than the specified criteria. |
+Value > Criteria | | `'leq'` | Denotes less than or equal to. It checks if the
+value is less than or equal to the specified criteria. | Value <= Criteria | |
+`'geq'` | Denotes greater than or equal to. It checks if the value is greater
+than or equal to the specified criteria. | Value >= Criteria | | `'in'` |
+Checks if the value is included in a specified list of values. | Value in List
+| | `'notIn'` | Checks if the value is not included in a specified list of
+values. | Value not in List | | `'like'` | Performs a pattern matching
+operation. It checks if the value is similar to a specified pattern. | Value
+matches Pattern | | `'not'` | Indicates non-equality. It checks if the column
+value that does not equal to the specified criteria. | NOT id = Criteria | |
+`'neq'` | Indicates non-equality. It checks if the value is not equal to the
+specified criteria. | Value != Criteria | | `'between'` | It checks range
+values that matches a given range between the minimum and maximum. | id BETWEEN
+(min, max) | Let's talk about these filters in detail of code by example. Let's
+say you want to update a `Post` where the `id` matches `1` you can do it as
+follows: ```py res2 = mysql_loom.update_one( instance=Post, filters=Filter
+( column="id", value=1, operator="eq", ), values=[ColumnValue(name="title",
+value="Bob")], ) ``` What if you want to update a post where `id` is not equal
+to `1` you can do it as follows ```py res2 = mysql_loom.update_bulk
+( instance=Post, filters=Filter( column="id", value=1, operator="neq", ),
+values=[ColumnValue(name="title", value="Bob")], ) ``` What if i want to update
+the records that have an `id` less than `3`? ```py res2 =
+mysql_loom.update_bulk( instance=Post, filters=Filter( column="id", value=3,
+operator="lt", ), values=[ColumnValue(name="title", value="Bob")], ) ``` What
+if i want to update the records that have an `id` less than or equal `3`? ```py
 res2 = mysql_loom.update_bulk( instance=Post, filters=Filter( column="id",
 value=1, operator="neq", ), values=[ColumnValue(name="title", value="Bob")], )
-``` What if i want to update the records that have an `id` less than `3`? ```py
-res2 = mysql_loom.update_bulk( instance=Post, filters=Filter( column="id",
-value=3, operator="lt", ), values=[ColumnValue(name="title", value="Bob")], )
-``` What if i want to update the records that have an `id` less than or equal
-`3`? ```py res2 = mysql_loom.update_bulk( instance=Post, filters=Filter
-( column="id", value=1, operator="neq", ), values=[ColumnValue(name="title",
-value="Bob")], ) ``` What if i want to update the records that have an `id`
-greater than `3`? ```py res = mysql_loom.update_bulk( instance=Post,
-filters=Filter( column="id", value=3, operator="gt", ), values=[ColumnValue
-(name="title", value="Bob")], ) ``` What if i want to update the records that
-have an `id` greater or equal to `3`? ```py res = mysql_loom.update_bulk
-( instance=Post, filters=Filter( column="id", value=3, operator="geq", ),
-values=[ColumnValue(name="title", value="Bob")], ) ``` You can use the `in` to
-update or query records that matches values in a specified `list` of values or
-`tuple`. Here is an example showing you how you can update records that does
-matches `id` in `[1, 2]`. ```py res = mysql_loom.update_bulk( instance=Post,
-filters=Filter( column="id", value=[1, 2], operator="in", ), values=
-[ColumnValue(name="title", value="Bob")], ) ``` You can use the `notIn` to
-update or query records that does not matches values in a specified `list` of
-values or `tuple`. Here is an example showing you how you can update records
-that does not matches `id` in `[1, 2]`. ```py res = mysql_loom.update_bulk
-( instance=Post, filters=Filter( column="id", value=[1, 2], operator="notIn",
-), values=[ColumnValue(name="title", value="Bob")], ) ``` You can use the
-`like` operator to match some patens in your query filters. Let's say we want
-to match a post that has the title ends with `general` we can use the `like`
-operator as follows ```py general = mysql_loom.find_one( instance=Post,
-filters=Filter( column="title", value="% general?", operator="like", ), select=
-["id", "title"], ) print(general) # ? {'id': 1, 'title': 'What are you doing
-general?'} ``` The following table show you some expression that you can use
-with this `like` operator. | Value | Description | | -------------- | ---------
+``` What if i want to update the records that have an `id` greater than `3`?
+```py res = mysql_loom.update_bulk( instance=Post, filters=Filter( column="id",
+value=3, operator="gt", ), values=[ColumnValue(name="title", value="Bob")], )
+``` What if i want to update the records that have an `id` greater or equal to
+`3`? ```py res = mysql_loom.update_bulk( instance=Post, filters=Filter
+( column="id", value=3, operator="geq", ), values=[ColumnValue(name="title",
+value="Bob")], ) ``` You can use the `in` to update or query records that
+matches values in a specified `list` of values or `tuple`. Here is an example
+showing you how you can update records that does matches `id` in `[1, 2]`.
+```py res = mysql_loom.update_bulk( instance=Post, filters=Filter( column="id",
+value=[1, 2], operator="in", ), values=[ColumnValue(name="title",
+value="Bob")], ) ``` You can use the `notIn` to update or query records that
+does not matches values in a specified `list` of values or `tuple`. Here is an
+example showing you how you can update records that does not matches `id` in `
+[1, 2]`. ```py res = mysql_loom.update_bulk( instance=Post, filters=Filter
+( column="id", value=[1, 2], operator="notIn", ), values=[ColumnValue
+(name="title", value="Bob")], ) ``` You can use the `like` operator to match
+some patens in your query filters. Let's say we want to match a post that has
+the title ends with `general` we can use the `like` operator as follows ```py
+general = mysql_loom.find_one( instance=Post, filters=Filter( column="title",
+value="% general?", operator="like", ), select=["id", "title"], ) print
+(general) # ? {'id': 1, 'title': 'What are you doing general?'} ``` The
+following table show you some expression that you can use with this `like`
+operator. | Value | Description | | -------------- | --------------------------
 -------------------------------------------------------------------------------
--------------------------------- | | `%pattern` | Finds values that end with
-the specified pattern. | | `pattern%` | Finds values that start with the
-specified pattern. | | `%pattern%` | Finds values that contain the specified
-pattern anywhere within the string. | | `_pattern` | Finds values that have any
-single character followed by the specified pattern. | | `pattern_` | Finds
-values that have the specified pattern followed by any single character. | | `
-[charlist]%` | Finds values that start with any character in the specified
-character list. | | `[!charlist]%` | Finds values that start with any character
-not in the specified character list. | | `_pattern_` | Finds values that have
-any single character followed by the specified pattern and then followed by any
-single character. | ### Data Aggregation With the [`Having`](#having-class) and
-the [`Group`](#group-class) classes you can perform some powerful powerful
-queries. In this section we are going to demonstrate an example of how we can
-do the aggregate queries. ```py posts = mysql_loom.find_many( Post,
-select="id", filters=Filter(column="id", operator="gt", value=1), group=Group
-( column="id", function="MAX", having=Having(column="id", operator="in", value=
-(2, 3, 4)), return_aggregation_column=True, ), ) ``` The following will be the
-output from the above query. ```shell [{'id': 2, 'MAX(`id`)': 2}, {'id': 3,
-'MAX(`id`)': 3}, {'id': 4, 'MAX(`id`)': 4}] ``` However you can remove the
-aggregation column from the above query by specifying the
-`return_aggregation_column` to be `False`: ```py posts = mysql_loom.find_many
-( Post, select="id", filters=Filter(column="id", operator="gt", value=1),
-group=Group( column="id", function="MAX", having=Having(column="id",
-operator="in", value=(2, 3, 4)), return_aggregation_column=False, ), ) print
-(posts) ``` This will output: ```shell [{'id': 2}, {'id': 3}, {'id': 4}] ```
-#### Aggregation Functions You can use the following aggregation functions that
-dataloom supports: | Aggregation Function | Description | | -------------------
-- | ------------------------------------------------ | | `"AVG"` | Computes the
-average of the values in the group. | | `"COUNT"` | Counts the number of items
-in the group. | | `"SUM"` | Computes the sum of the values in the group. | |
-`"MAX"` | Retrieves the maximum value in the group. | | `"MIN"` | Retrieves the
-minimum value in the group. | > ð **Pro Tip**: Note that data aggregation
-only works without `eager` loading and also works only with [`find_may()`](#2-
-find_many) and [`find_all()`](#1-find_all) in dataloom. ### Utilities Dataloom
-comes up with some utility functions that works on an instance of a model. This
-is very useful when debuging your tables to see how do they look like. These
-function include: #### 1. `inspect()` This function takes in a model as
-argument and inspect the model fields or columns. The following examples show
-how we can use this handy function in inspecting table names. ```py table =
-mysql_loom.inspect(instance=User, fields=["name", "type"], print_table=False)
-print(table) ``` The above snippet returns a list of dictionaries containing
-the column name and the arguments that were passed. ```shell [{'id': {'type':
-'int'}}, {'name': {'type': 'varchar'}}, {'tokenVersion': {'type': 'int'}},
-{'username': {'type': 'varchar'}}] ``` You can print table format these fields
-with their types as follows ```py mysql_loom.inspect(instance=User) ``` Output:
-```shell +--------------+---------+----------+---------+ | name | type |
-nullable | default | +--------------+---------+----------+---------+ | id | int
-| NO | None | | name | varchar | NO | Bob | | tokenVersion | int | YES | 0 | |
-username | varchar | YES | None | +--------------+---------+----------+--------
--+ ``` The `inspect` function take the following arguments. | Argument |
-Description | Type | Default | Required | | ------------- | -------------------
------------------------------------ | ----------- | ---------------------------
--------------- | -------- | | `instance` | The model instance to inspect. |
-`Model` | - | Yes | | `fields` | The list of fields to include in the
-inspection. | `list[str]` | `["name", "type", "nullable", "default"]` | No | |
-`print_table` | Flag indicating whether to print the inspection table. | `bool`
-| `True` | No | #### 2. `decorators` These modules contain several decorators
-that can prove useful when creating models. These decorators originate from
-`dataloom.decorators`, and at this stage, we are referring to them as
-"experimental." ##### `@initialize()` Let's examine a model named `Profile`,
-which appears as follows: ```py class Profile(Model): __tablename__: Optional
-[TableColumn] = TableColumn(name="profiles") id = PrimaryKeyColumn(type="int",
+--------------- | | `%pattern` | Finds values that end with the specified
+pattern. | | `pattern%` | Finds values that start with the specified pattern. |
+| `%pattern%` | Finds values that contain the specified pattern anywhere within
+the string. | | `_pattern` | Finds values that have any single character
+followed by the specified pattern. | | `pattern_` | Finds values that have the
+specified pattern followed by any single character. | | `[charlist]%` | Finds
+values that start with any character in the specified character list. | | `
+[!charlist]%` | Finds values that start with any character not in the specified
+character list. | | `_pattern_` | Finds values that have any single character
+followed by the specified pattern and then followed by any single character. |
+### Data Aggregation With the [`Having`](#having-class) and the [`Group`]
+(#group-class) classes you can perform some powerful powerful queries. In this
+section we are going to demonstrate an example of how we can do the aggregate
+queries. ```py posts = mysql_loom.find_many( Post, select="id", filters=Filter
+(column="id", operator="gt", value=1), group=Group( column="id",
+function="MAX", having=Having(column="id", operator="in", value=(2, 3, 4)),
+return_aggregation_column=True, ), ) ``` The following will be the output from
+the above query. ```shell [{'id': 2, 'MAX(`id`)': 2}, {'id': 3, 'MAX(`id`)':
+3}, {'id': 4, 'MAX(`id`)': 4}] ``` However you can remove the aggregation
+column from the above query by specifying the `return_aggregation_column` to be
+`False`: ```py posts = mysql_loom.find_many( Post, select="id", filters=Filter
+(column="id", operator="gt", value=1), group=Group( column="id",
+function="MAX", having=Having(column="id", operator="in", value=(2, 3, 4)),
+return_aggregation_column=False, ), ) print(posts) ``` This will output:
+```shell [{'id': 2}, {'id': 3}, {'id': 4}] ``` #### Aggregation Functions You
+can use the following aggregation functions that dataloom supports: |
+Aggregation Function | Description | | -------------------- | -----------------
+------------------------------- | | `"AVG"` | Computes the average of the
+values in the group. | | `"COUNT"` | Counts the number of items in the group. |
+| `"SUM"` | Computes the sum of the values in the group. | | `"MAX"` |
+Retrieves the maximum value in the group. | | `"MIN"` | Retrieves the minimum
+value in the group. | > ð **Pro Tip**: Note that data aggregation only works
+without `eager` loading and also works only with [`find_may()`](#2-find_many)
+and [`find_all()`](#1-find_all) in dataloom. ### Utilities Dataloom comes up
+with some utility functions that works on an instance of a model. This is very
+useful when debuging your tables to see how do they look like. These function
+include: #### 1. `inspect()` This function takes in a model as argument and
+inspect the model fields or columns. The following examples show how we can use
+this handy function in inspecting table names. ```py table = mysql_loom.inspect
+(instance=User, fields=["name", "type"], print_table=False) print(table) ```
+The above snippet returns a list of dictionaries containing the column name and
+the arguments that were passed. ```shell [{'id': {'type': 'int'}}, {'name':
+{'type': 'varchar'}}, {'tokenVersion': {'type': 'int'}}, {'username': {'type':
+'varchar'}}] ``` You can print table format these fields with their types as
+follows ```py mysql_loom.inspect(instance=User) ``` Output: ```shell +---------
+-----+---------+----------+---------+ | name | type | nullable | default | +---
+-----------+---------+----------+---------+ | id | int | NO | None | | name |
+varchar | NO | Bob | | tokenVersion | int | YES | 0 | | username | varchar |
+YES | None | +--------------+---------+----------+---------+ ``` The `inspect`
+function take the following arguments. | Argument | Description | Type |
+Default | Required | | ------------- | ----------------------------------------
+-------------- | ----------- | ----------------------------------------- | ----
+---- | | `instance` | The model instance to inspect. | `Model` | - | Yes | |
+`fields` | The list of fields to include in the inspection. | `list[str]` | `
+["name", "type", "nullable", "default"]` | No | | `print_table` | Flag
+indicating whether to print the inspection table. | `bool` | `True` | No | ####
+2. `decorators` These modules contain several decorators that can prove useful
+when creating models. These decorators originate from `dataloom.decorators`,
+and at this stage, we are referring to them as "experimental." #####
+`@initialize()` Let's examine a model named `Profile`, which appears as
+follows: ```py class Profile(Model): __tablename__: Optional[TableColumn] =
+TableColumn(name="profiles") id = PrimaryKeyColumn(type="int",
 auto_increment=True) avatar = Column(type="text", nullable=False) userId =
 ForeignKeyColumn( User, maps_to="1-1", type="int", required=True,
 onDelete="CASCADE", onUpdate="CASCADE", ) ``` This is simply a Python class
 that inherits from the top-level class `Model`. However, it lacks some useful
 `dunder` methods such as `__init__` and `__repr__`. In standard Python, we can
 achieve this functionality by using `dataclasses`. For example, we can modify
 our class as follows: ```py from dataclasses import dataclass @dataclass class
@@ -1357,11 +1359,13 @@
 don't want logging at all. | `int` | No | `1` | | `is_script` | Whether the SQL
 is a script. | `bool` | No | `False` | #### Why Use Query Builder? - The query
 builder empowers developers to seamlessly execute `SQL` queries directly. -
 While Dataloom primarily utilizes `subqueries` for eager data fetching on
 models, developers may prefer to employ JOIN operations, which are achievable
 through the `qb` object. ```python qb = loom.getQueryBuilder() result = qb.run
 ("SELECT * FROM table1 INNER JOIN table2 ON table1.id = table2.table1_id;")
-print(result) ``` ### Contributing Contributions to `dataloom` are welcome!
-Feel free to submit bug reports, feature requests, or pull requests on [GitHub]
-(https://github.com/CrispenGari/dataloom). ### License This project is licensed
-under the MIT License - see the [LICENSE](/LISENSE) file for details.
+print(result) ``` ### Documentation You can read the full documentation of
+dataloom on [readthedocs.io](https://dataloom-py.readthedocs.io/en/latest/) ###
+Contributing Contributions to `dataloom` are welcome! Feel free to submit bug
+reports, feature requests, or pull requests on [GitHub](https://github.com/
+CrispenGari/dataloom). ### License This project is licensed under the MIT
+License - see the [LICENSE](/LISENSE) file for details.
```

### Comparing `dataloom-2.4.1/dataloom.png` & `dataloom-2.4.2/dataloom.png`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/hi.db` & `dataloom-2.4.2/hi.db`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/pyproject.toml` & `dataloom-2.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataloom"
-version = "2.4.1"
+version = "2.4.2"
 authors = [
     {name = "Crispen Gari", email = "crispengari@gmail.com"},
 ]
 description = "dataloom stands as a bespoke Object-Relational Mapping (ORM) solution meticulously crafted to empower Python developers in efficiently managing diverse databases. Unlike conventional ORMs, Dataloom has been built from the ground up, providing native support for SQLite3, PostgreSQL, and MySQL. Navigate effortlessly between database engines while enjoying a tailored and performant ORM experience."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.12"
```

### Comparing `dataloom-2.4.1/requirements.txt` & `dataloom-2.4.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `dataloom-2.4.1/todo.txt` & `dataloom-2.4.2/todo.txt`

 * *Files identical despite different names*

