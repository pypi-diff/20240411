# Comparing `tmp/swh.scrubber-2.3.0.tar.gz` & `tmp/swh.scrubber-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.scrubber-2.3.0.tar", last modified: Fri Feb  2 10:07:35 2024, max compression
+gzip compressed data, was "swh.scrubber-3.0.0.tar", last modified: Thu Apr 11 14:04:00 2024, max compression
```

## Comparing `swh.scrubber-2.3.0.tar` & `swh.scrubber-3.0.0.tar`

### file list

```diff
@@ -1,82 +1,87 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.932943 swh.scrubber-2.3.0/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      358 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      117 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1044 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4408 2024-02-02 10:07:35.932943 swh.scrubber-2.3.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2901 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/README.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       85 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.916943 swh.scrubber-2.3.0/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/docs/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2901 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.916943 swh.scrubber-2.3.0/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.916943 swh.scrubber-2.3.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      156 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      246 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      480 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1738 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       97 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)      175 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       71 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      261 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-02-02 10:07:35.932943 swh.scrubber-2.3.0/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.908943 swh.scrubber-2.3.0/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.920943 swh.scrubber-2.3.0/swh/scrubber/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      727 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18730 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    34883 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7601 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/fixer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5200 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/journal_checker.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3050 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/origin_locator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/py.typed
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.924943 swh.scrubber-2.3.0/swh/scrubber/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      201 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/sql/20-enums.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6059 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3098 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/sql/60-indexes.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.924943 swh.scrubber-2.3.0/swh/scrubber/sql/upgrades/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      942 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/sql/upgrades/2.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2338 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/sql/upgrades/3.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      989 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/sql/upgrades/4.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1567 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/sql/upgrades/5.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2524 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/sql/upgrades/6.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5124 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/sql/upgrades/7.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16191 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/storage_checker.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.928943 swh.scrubber-2.3.0/swh/scrubber/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3699 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.908943 swh.scrubber-2.3.0/swh/scrubber/tests/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.908943 swh.scrubber-2.3.0/swh/scrubber/tests/data/cli/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.928943 swh.scrubber-2.3.0/swh/scrubber/tests/data/cli/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9303 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/data/cli/sql/10-init-all.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4403 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/data/cli/sql/20-data.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.928943 swh.scrubber-2.3.0/swh/scrubber/tests/data/cli/sql/upgrades/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2524 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/data/cli/sql/upgrades/006.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5124 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/data/cli/sql/upgrades/007.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14849 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/storage_checker_tests.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    24833 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10591 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/test_db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9813 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/test_fixer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1053 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/test_init.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8000 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/test_journal_kafka.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8949 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/test_migration.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5137 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/test_origin_locator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1035 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/test_storage_cassandra.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      780 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/tests/test_storage_postgresql.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1729 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/swh/scrubber/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:07:35.928943 swh.scrubber-2.3.0/swh.scrubber.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4408 2024-02-02 10:07:35.000000 swh.scrubber-2.3.0/swh.scrubber.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1773 2024-02-02 10:07:35.000000 swh.scrubber-2.3.0/swh.scrubber.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-02-02 10:07:35.000000 swh.scrubber-2.3.0/swh.scrubber.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       54 2024-02-02 10:07:35.000000 swh.scrubber-2.3.0/swh.scrubber.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      214 2024-02-02 10:07:35.000000 swh.scrubber-2.3.0/swh.scrubber.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-02-02 10:07:35.000000 swh.scrubber-2.3.0/swh.scrubber.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1381 2024-02-02 10:07:28.000000 swh.scrubber-2.3.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.342583 swh.scrubber-3.0.0/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      358 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      117 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1487 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8697 2024-04-11 14:04:00.342583 swh.scrubber-3.0.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7148 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/README.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      121 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.326583 swh.scrubber-3.0.0/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/docs/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7148 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.326583 swh.scrubber-3.0.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.326583 swh.scrubber-3.0.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      156 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      246 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      480 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1738 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       78 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      261 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-04-11 14:04:00.342583 swh.scrubber-3.0.0/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.314583 swh.scrubber-3.0.0/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.330583 swh.scrubber-3.0.0/swh/scrubber/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      727 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4489 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/base_checker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24404 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    34854 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7601 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/fixer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4371 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/journal_checker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6837 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/objstorage_checker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3050 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/origin_locator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/py.typed
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.330583 swh.scrubber-3.0.0/swh/scrubber/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      201 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/sql/20-enums.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6059 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3098 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/sql/60-indexes.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.334583 swh.scrubber-3.0.0/swh/scrubber/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      942 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/sql/upgrades/2.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2338 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/sql/upgrades/3.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      989 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/sql/upgrades/4.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1567 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/sql/upgrades/5.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2524 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/sql/upgrades/6.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5124 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/sql/upgrades/7.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13767 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/storage_checker.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.338583 swh.scrubber-3.0.0/swh/scrubber/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4289 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.318583 swh.scrubber-3.0.0/swh/scrubber/tests/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.318583 swh.scrubber-3.0.0/swh/scrubber/tests/data/cli/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.338583 swh.scrubber-3.0.0/swh/scrubber/tests/data/cli/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9303 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/data/cli/sql/10-init-all.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4403 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/data/cli/sql/20-data.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.338583 swh.scrubber-3.0.0/swh/scrubber/tests/data/cli/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2524 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/data/cli/sql/upgrades/006.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5124 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/data/cli/sql/upgrades/007.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8100 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/objstorage_checker_tests.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14849 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/storage_checker_tests.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    34323 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11309 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/test_db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9813 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/test_fixer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1053 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6818 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/test_journal_kafka.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8949 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/test_migration.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      604 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/test_objstorage_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      563 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/test_objstorage_pathslicing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5137 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/test_origin_locator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1035 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/test_storage_cassandra.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      780 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/tests/test_storage_postgresql.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1729 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/swh/scrubber/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-11 14:04:00.338583 swh.scrubber-3.0.0/swh.scrubber.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8697 2024-04-11 14:04:00.000000 swh.scrubber-3.0.0/swh.scrubber.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1979 2024-04-11 14:04:00.000000 swh.scrubber-3.0.0/swh.scrubber.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-04-11 14:04:00.000000 swh.scrubber-3.0.0/swh.scrubber.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       54 2024-04-11 14:04:00.000000 swh.scrubber-3.0.0/swh.scrubber.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      241 2024-04-11 14:04:00.000000 swh.scrubber-3.0.0/swh.scrubber.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-04-11 14:04:00.000000 swh.scrubber-3.0.0/swh.scrubber.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1111 2024-04-11 14:03:55.000000 swh.scrubber-3.0.0/tox.ini
```

### Comparing `swh.scrubber-2.3.0/CODE_OF_CONDUCT.md` & `swh.scrubber-3.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/LICENSE` & `swh.scrubber-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/pyproject.toml` & `swh.scrubber-3.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/__init__.py` & `swh.scrubber-3.0.0/swh/scrubber/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/cli.py` & `swh.scrubber-3.0.0/swh/scrubber/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022-2023  The Software Heritage developers
+# Copyright (C) 2022-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import os
 from typing import Optional
 import warnings
@@ -10,43 +10,56 @@
 import click
 
 from swh.core.cli import CONTEXT_SETTINGS
 from swh.core.cli import swh as swh_cli_group
 from swh.model.swhids import ObjectType
 
 
+def _fix_sphinx_docstring():
+    """Remove \b markers used by click to prevent text rewrapping in docstring."""
+
+    def decorator(f):
+        if "SWH_DOC_BUILD" in os.environ:
+            f.__doc__ = f.__doc__.replace("\b", "")
+        return f
+
+    return decorator
+
+
 @swh_cli_group.group(name="scrubber", context_settings=CONTEXT_SETTINGS)
 @click.option(
     "--config-file",
     "-C",
     default=None,
     type=click.Path(
         exists=True,
         dir_okay=False,
     ),
     help="Configuration file.",
 )
 @click.pass_context
+@_fix_sphinx_docstring()
 def scrubber_cli_group(ctx, config_file: Optional[str]) -> None:
     """main command group of the datastore scrubber
 
+    \b
     Expected config format::
-
+        \b
         scrubber:
             cls: postgresql
             db: "service=..."    # libpq DSN
-
+        \b
         # for storage checkers + origin locator only:
         storage:
             cls: postgresql     # cannot be remote for checkers, as they need direct
                                 # access to the pg DB
             db": "service=..."  # libpq DSN
             objstorage:
                 cls: memory
-
+        \b
         # for journal checkers only:
         journal:
             # see https://docs.softwareheritage.org/devel/apidoc/swh.journal.client.html
             # for the full list of options
             sasl.mechanism: SCRAM-SHA-512
             security.protocol: SASL_SSL
             sasl.username: ...
@@ -83,41 +96,38 @@
         warnings.warn(
             "the 'scrubber_db' configuration section has been renamed to 'scrubber'; "
             f"please update your configuration file {config_file}",
             DeprecationWarning,
         )
         conf["scrubber"] = conf.pop("scrubber_db")
 
-    if "scrubber" not in conf:
-        click.echo(
-            "WARNING: You must have a scrubber configured in your config file.\n"
-        )
-    else:
+    if "scrubber" in conf:
         ctx.obj["db"] = get_scrubber_db(**conf["scrubber"])
 
 
 @scrubber_cli_group.group(name="check")
 @click.pass_context
 def scrubber_check_cli_group(ctx):
     """group of commands which read from data stores and report errors."""
     pass
 
 
 @scrubber_check_cli_group.command(name="init")
-@click.argument("backend", type=click.Choice(["storage", "journal"]))
+@click.argument("backend", type=click.Choice(["storage", "journal", "objstorage"]))
 @click.option(
     "--object-type",
     type=click.Choice(
         # use a hardcoded list to prevent having to load the
         # replay module at cli loading time
         [
             "snapshot",
             "revision",
             "release",
             "directory",
+            "content",
             # TODO:
             # "raw_extrinsic_metadata",
             # "extid",
         ]
     ),
 )
 @click.option("--nb-partitions", default=4096, type=int)
@@ -135,19 +145,19 @@
     check_references: Optional[bool],
 ):
     """Initialise a scrubber check configuration for the datastore defined in the
     configuration file and given object_type.
 
     A checker configuration configuration consists simply in a set of:
 
-    - backend: the datastore type being scrubbed (storage or journal),
+    - backend: the datastore type being scrubbed (storage, objstorage or journal),
 
     - object-type: the type of object being checked,
 
-    - nb-pertitions: the number of partitions the hash space is divided
+    - nb-partitions: the number of partitions the hash space is divided
       in; must be a power of 2,
 
     - name: an unique name for easier reference,
 
     - check-hashes: flag (default to True) to select the hash validation step for
       this scrubbing configuration,
 
@@ -156,14 +166,16 @@
     """
     if not object_type or not name:
         raise click.ClickException(
             "Invalid parameters: you must provide the object type and configuration name"
         )
 
     conf = ctx.obj["config"]
+    if "db" not in ctx.obj:
+        ctx.fail("You must have a scrubber configured in your config file.")
     db = ctx.obj["db"]
 
     if backend == "storage":
         if check_references is None:
             check_references = True
         if "storage" not in conf:
             raise click.ClickException(
@@ -182,14 +194,31 @@
             raise click.ClickException(
                 "You must have a journal configured in your config file."
             )
         from .journal_checker import get_datastore as get_journal_datastore
 
         datastore = get_journal_datastore(journal_cfg=conf["journal"])
         db.datastore_get_or_add(datastore)
+        nb_partitions = 1
+    elif backend == "objstorage":
+        if check_references is None:
+            check_references = True
+        if object_type != "content":
+            raise click.ClickException(
+                "Object storage scrubber can only check content objects, "
+                f"not {object_type} ones."
+            )
+
+        if "objstorage" not in conf:
+            raise click.ClickException(
+                "You must have an object storage configured in your config file."
+            )
+        from .objstorage_checker import get_objstorage_datastore
+
+        datastore = get_objstorage_datastore(objstorage_config=conf["objstorage"])
     else:
         raise click.ClickException(f"Backend type {backend} is not supported")
 
     if db.config_get_by_name(name):
         raise click.ClickException(f"Configuration {name} already exists")
 
     assert check_references is not None
@@ -211,17 +240,18 @@
 @scrubber_check_cli_group.command(name="list")
 @click.pass_context
 def scrubber_check_list(
     ctx,
 ):
     """List the know configurations"""
     conf = ctx.obj["config"]
+    if "db" not in ctx.obj:
+        ctx.fail("You must have a scrubber configured in your config file.")
     if "storage" not in conf:
         ctx.fail("You must have a storage configured in your config file.")
-
     db = ctx.obj["db"]
 
     for id_, cfg in db.config_iter():
         ds = cfg.datastore
         if not ds:
             click.echo(
                 f"[{id_}] {cfg.name}: Invalid configuration entry; datastore not found"
@@ -262,14 +292,16 @@
     ctx, name: str, config_id: int, delay: Optional[str], reset: bool
 ):
     """List the stuck partitions for a given config"""
     import datetime
 
     from humanize import naturaldate, naturaldelta
 
+    if "db" not in ctx.obj:
+        ctx.fail("You must have a scrubber configured in your config file.")
     db = ctx.obj["db"]
     if name and config_id is None:
         config_id = db.config_get_by_name(name)
 
     if config_id is None:
         raise click.ClickException("A valid configuration name/id must be set")
 
@@ -318,14 +350,16 @@
 @click.pass_context
 def scrubber_check_running(ctx, name: str, config_id: int):
     """List partitions being checked for the check session <name>"""
     import datetime
 
     from humanize import naturaldate, naturaldelta
 
+    if "db" not in ctx.obj:
+        ctx.fail("You must have a scrubber configured in your config file.")
     db = ctx.obj["db"]
     if name and config_id is None:
         config_id = db.config_get_by_name(name)
 
     if config_id is None:
         raise click.ClickException("A valid configuration name/id must be set")
 
@@ -371,14 +405,16 @@
     """Display statistics for the check session <name>"""
     from dataclasses import asdict
     from json import dumps
     import textwrap
 
     from humanize import naturaldelta
 
+    if "db" not in ctx.obj:
+        ctx.fail("You must have a scrubber configured in your config file.")
     db = ctx.obj["db"]
     if name and config_id is None:
         config_id = db.config_get_by_name(name)
 
     if config_id is None:
         raise click.ClickException("A valid configuration name/id must be set")
 
@@ -420,32 +456,153 @@
         if cfg.check_hashes:
             click.echo(f"  corrupted objects: {stats['corrupt_object']}")
         if cfg.check_references:
             click.echo(f"  missing objects: {stats['missing_object']}")
             click.echo(f"  from references: {stats['missing_object_reference']}")
 
 
-@scrubber_check_cli_group.command(name="storage")
+@scrubber_check_cli_group.command(name="run")
+@click.argument(
+    "name",
+    type=str,
+    default=None,
+    required=False,  # can be given by config_id instead
+)
+@click.option(
+    "--config-id",
+    type=int,
+    default=None,
+    help="Config ID (is config name is not given as argument)",
+)
+@click.option(
+    "--use-journal",
+    is_flag=True,
+    default=False,
+    help=(
+        "Flag only relevant for running an object storage scrubber, "
+        "if set content ids are consumed from a kafka topic of SWH journal "
+        "instead of getting them from a storage"
+    ),
+)
+@click.option("--limit", default=0, type=int)
+@click.pass_context
+def scrubber_check_run(
+    ctx,
+    name: Optional[str],
+    config_id: Optional[int],
+    use_journal: bool,
+    limit: int,
+):
+    """Run the scrubber checker configured as `name` and reports corrupt
+    objects to the scrubber DB.
+
+    This runs a single thread; parallelism is achieved by running this command
+    multiple times.
+
+    This command references an existing scrubbing configuration (either by name
+    or by id); the configuration holds the object type, number of partitions
+    and the storage configuration this scrubbing session will check on.
+
+    """
+    if "db" not in ctx.obj:
+        ctx.fail("You must have a scrubber configured in your config file.")
+    db = ctx.obj["db"]
+    if name and config_id is None:
+        config_id = db.config_get_by_name(name)
+
+    if config_id is None:
+        ctx.fail("A valid configuration name/id must be given.")
+
+    from swh.scrubber.base_checker import BaseChecker
+
+    scrubber_cfg = db.config_get(config_id)
+    datastore = scrubber_cfg.datastore
+    conf = ctx.obj["config"]
+
+    assert config_id is not None
+    checker: BaseChecker
+
+    if datastore.package == "storage":
+        if "storage" not in conf:
+            ctx.fail("You must have a storage configured in your config file.")
+        from swh.storage import get_storage
+
+        from .storage_checker import StorageChecker
+
+        checker = StorageChecker(
+            db=db,
+            storage=get_storage(**conf["storage"]),
+            config_id=config_id,
+            limit=limit,
+        )
+    elif datastore.package == "objstorage":
+        if not use_journal and "storage" not in conf:
+            ctx.fail("You must have a storage configured in your config file.")
+        if use_journal and "journal" not in conf:
+            ctx.fail("You must have a journal configured in your config file.")
+        if "objstorage" not in conf:
+            ctx.fail("You must have an object storage configured in your config file.")
+        from swh.objstorage.factory import get_objstorage
+
+        if use_journal:
+            from .objstorage_checker import ObjectStorageCheckerFromJournal
+
+            checker = ObjectStorageCheckerFromJournal(
+                db=db,
+                journal_client_config=conf["journal"],
+                objstorage=get_objstorage(**conf["objstorage"]),
+                config_id=config_id,
+            )
+        else:
+            from swh.storage import get_storage
+
+            from .objstorage_checker import ObjectStorageCheckerFromStoragePartition
+
+            checker = ObjectStorageCheckerFromStoragePartition(
+                db=db,
+                storage=get_storage(**conf["storage"]),
+                objstorage=get_objstorage(**conf["objstorage"]),
+                config_id=config_id,
+                limit=limit,
+            )
+    elif datastore.package == "journal":
+        if "journal" not in conf:
+            ctx.fail("You must have a journal configured in your config file.")
+        from .journal_checker import JournalChecker
+
+        checker = JournalChecker(
+            db=db,
+            journal_client_config=conf["journal"],
+            config_id=config_id,
+        )
+    else:
+        ctx.fail(f"Unsupported scruber package {datastore.package}")
+
+    checker.run()
+
+
+@scrubber_check_cli_group.command(name="storage", deprecated=True, hidden=True)
 @click.argument(
     "name",
     type=str,
     default=None,
     required=False,  # can be given by config_id instead
 )
 @click.option(
     "--config-id",
     type=int,
+    default=None,
     help="Config ID (is config name is not given as argument)",
 )
 @click.option("--limit", default=0, type=int)
 @click.pass_context
 def scrubber_check_storage(
     ctx,
-    name: str,
-    config_id: int,
+    name: Optional[str],
+    config_id: Optional[int],
     limit: int,
 ):
     """Reads a swh-storage instance, and reports corrupt objects to the scrubber DB.
 
     This runs a single thread; parallelism is achieved by running this command
     multiple times.
 
@@ -456,16 +613,18 @@
     All objects of type ``object_type`` are ordered, and split into the given
     number of partitions.
 
     Then, this process will check all partitions. The status of the ongoing
     check session is stored in the database, so the number of concurrent
     workers can be dynamically adjusted.
 
-    """  # noqa
+    """
     conf = ctx.obj["config"]
+    if "db" not in ctx.obj:
+        ctx.fail("You must have a scrubber configured in your config file.")
     if "storage" not in conf:
         ctx.fail("You must have a storage configured in your config file.")
     db = ctx.obj["db"]
 
     from swh.storage import get_storage
 
     from .storage_checker import StorageChecker
@@ -489,15 +648,15 @@
         config_id=config_id,
         limit=limit,
     )
 
     checker.run()
 
 
-@scrubber_check_cli_group.command(name="journal")
+@scrubber_check_cli_group.command(name="journal", deprecated=True, hidden=True)
 @click.argument(
     "name",
     type=str,
     default=None,
     required=False,  # can be given by config_id instead
 )
 @click.option(
@@ -506,14 +665,16 @@
     help="Config ID (is config name is not given as argument)",
 )
 @click.pass_context
 def scrubber_check_journal(ctx, name, config_id) -> None:
     """Reads a complete kafka journal, and reports corrupt objects to
     the scrubber DB."""
     conf = ctx.obj["config"]
+    if "db" not in ctx.obj:
+        ctx.fail("You must have a scrubber configured in your config file.")
     if "journal" not in conf:
         ctx.fail("You must have a journal configured in your config file.")
     db = ctx.obj["db"]
 
     if name and config_id is None:
         from .journal_checker import get_datastore as get_journal_datastore
 
@@ -527,15 +688,15 @@
     if config_id is None:
         raise click.ClickException("A valid configuration name/id must be set")
 
     from .journal_checker import JournalChecker
 
     checker = JournalChecker(
         db=ctx.obj["db"],
-        journal=conf["journal"],
+        journal_client_config=conf["journal"],
         config_id=config_id,
     )
 
     checker.run()
 
 
 @scrubber_cli_group.command(name="locate")
```

### Comparing `swh.scrubber-2.3.0/swh/scrubber/db.py` & `swh.scrubber-3.0.0/swh/scrubber/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -589,15 +589,15 @@
                 INNER JOIN check_config AS CC on (CC.id=CP.config_id)
                 WHERE CC.id=%s
                 """,
                 (config_id,),
             )
 
             for row in cur:
-                yield tuple(row)  # type: ignore[misc]
+                yield tuple(row)
 
     ####################################
     # Inventory of objects with issues
     ####################################
 
     def corrupt_object_add(
         self,
@@ -810,38 +810,37 @@
 
         Args:
             id: SWHID of the missing object (the hole)
             reference_id: SWHID of the object referencing the missing object
             datastore: representation of the swh-storage/swh-journal/... instance
               containing this hole
         """
-        if not reference_ids:
-            raise ValueError("reference_ids is empty")
         config_id = self.config_get_by_name(config.name)
         with self.transaction() as cur:
             cur.execute(
                 """
                 INSERT INTO missing_object (id, config_id)
                 VALUES (%s, %s)
                 ON CONFLICT DO NOTHING
                 """,
                 (str(id), config_id),
             )
-            psycopg2.extras.execute_batch(
-                cur,
-                """
-                INSERT INTO missing_object_reference (missing_id, reference_id, config_id)
-                VALUES (%s, %s, %s)
-                ON CONFLICT DO NOTHING
-                """,
-                [
-                    (str(id), str(reference_id), config_id)
-                    for reference_id in reference_ids
-                ],
-            )
+            if reference_ids:
+                psycopg2.extras.execute_batch(
+                    cur,
+                    """
+                    INSERT INTO missing_object_reference (missing_id, reference_id, config_id)
+                    VALUES (%s, %s, %s)
+                    ON CONFLICT DO NOTHING
+                    """,
+                    [
+                        (str(id), str(reference_id), config_id)
+                        for reference_id in reference_ids
+                    ],
+                )
 
     def missing_object_iter(self) -> Iterator[MissingObject]:
         """Yields all records in the 'missing_object' table."""
         with self.transaction() as cur:
             cur.execute(
                 """
                 SELECT
```

### Comparing `swh.scrubber-2.3.0/swh/scrubber/fixer.py` & `swh.scrubber-3.0.0/swh/scrubber/fixer.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/journal_checker.py` & `swh.scrubber-3.0.0/swh/scrubber/journal_checker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# Copyright (C) 2021-2023  The Software Heritage developers
+# Copyright (C) 2021-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """Reads all objects in a swh-storage instance and recomputes their checksums."""
 
 import json
 import logging
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List
 
 import attr
 
-from swh.core.statsd import Statsd
 from swh.journal.client import get_journal_client
 from swh.journal.serializers import kafka_to_value
 from swh.model import model
 
-from .db import ConfigEntry, Datastore, ScrubberDb
+from .base_checker import BaseChecker
+from .db import Datastore, ScrubberDb
 
 logger = logging.getLogger(__name__)
 
 
 def get_datastore(journal_cfg) -> Datastore:
     if journal_cfg.get("cls") == "kafka":
         datastore = Datastore(
@@ -32,82 +32,53 @@
                     "group_id": journal_cfg["group_id"],
                     "prefix": journal_cfg["prefix"],
                 }
             ),
         )
     else:
         raise NotImplementedError(
-            f"JournalChecker(journal={journal_cfg!r}).datastore()"
+            f"JournalChecker(journal_client_config={journal_cfg!r}).datastore()"
         )
     return datastore
 
 
-class JournalChecker:
+class JournalChecker(BaseChecker):
     """Reads a chunk of a swh-storage database, recomputes checksums, and
     reports errors in a separate database."""
 
-    _config: Optional[ConfigEntry] = None
-    _datastore: Optional[Datastore] = None
-
-    def __init__(self, db: ScrubberDb, config_id: int, journal: Dict[str, Any]):
-        self.db = db
-        self.config_id = config_id
+    def __init__(
+        self, db: ScrubberDb, config_id: int, journal_client_config: Dict[str, Any]
+    ):
+        super().__init__(db=db, config_id=config_id)
 
         if self.config.check_references:
             raise ValueError(
-                "The journal checcker cannot check for references, please set "
+                "The journal checker cannot check for references, please set "
                 "the 'check_references' to False in the config entry %s.",
                 self.config_id,
             )
-        self.journal_client_config = journal.copy()
+        self.journal_client_config = journal_client_config.copy()
         if "object_types" in self.journal_client_config:
             raise ValueError(
                 "The journal_client configuration entry should not define the "
                 "object_types field; this is handled by the scrubber configuration entry"
             )
-        self.journal_client_config["object_types"] = [
-            self.config.object_type.name.lower()
-        ]
+        self.journal_client_config["object_types"] = [self.object_type.name.lower()]
         self.journal_client = get_journal_client(
             **self.journal_client_config,
             # Remove default deserializer; so process_kafka_values() gets the message
             # verbatim so it can archive it with as few modifications a possible.
             value_deserializer=lambda obj_type, msg: msg,
         )
-        self._statsd: Optional[Statsd] = None
-
-    @property
-    def config(self) -> ConfigEntry:
-        if self._config is None:
-            self._config = self.db.config_get(self.config_id)
-
-        assert self._config is not None
-        return self._config
-
-    @property
-    def datastore(self) -> Datastore:
-        """Returns a :class:`Datastore` instance representing the journal instance
-        being checked."""
-        return self.config.datastore
-
-    @property
-    def statsd(self) -> Statsd:
-        if self._statsd is None:
-            self._statsd = Statsd(
-                namespace="swh_scrubber",
-                constant_tags={
-                    "datastore_package": self.datastore.package,
-                    "datastore_cls": self.datastore.cls,
-                },
-            )
-        return self._statsd
 
-    def run(self):
+    def run(self) -> None:
         """Runs a journal client with the given configuration.
-        This method does not return, unless otherwise configured (with ``stop_on_eof``).
+
+        This method does not return, unless the client is configured with ``on_eof``
+        parameter equals to ``EofBehavior.STOP`` (``stop`` in YAML).
         """
         self.journal_client.process(self.process_kafka_messages)
 
     def process_kafka_messages(self, all_messages: Dict[str, List[bytes]]):
         for object_type, messages in all_messages.items():
             logger.debug("Processing %s %s", len(messages), object_type)
             cls = getattr(model, object_type.capitalize())
```

### Comparing `swh.scrubber-2.3.0/swh/scrubber/origin_locator.py` & `swh.scrubber-3.0.0/swh/scrubber/origin_locator.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/sql/30-schema.sql` & `swh.scrubber-3.0.0/swh/scrubber/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/sql/60-indexes.sql` & `swh.scrubber-3.0.0/swh/scrubber/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/sql/upgrades/2.sql` & `swh.scrubber-3.0.0/swh/scrubber/sql/upgrades/2.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/sql/upgrades/3.sql` & `swh.scrubber-3.0.0/swh/scrubber/sql/upgrades/3.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/sql/upgrades/4.sql` & `swh.scrubber-3.0.0/swh/scrubber/sql/upgrades/4.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/sql/upgrades/5.sql` & `swh.scrubber-3.0.0/swh/scrubber/sql/upgrades/5.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/sql/upgrades/6.sql` & `swh.scrubber-3.0.0/swh/scrubber/sql/upgrades/6.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/sql/upgrades/7.sql` & `swh.scrubber-3.0.0/swh/scrubber/sql/upgrades/7.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/storage_checker.py` & `swh.scrubber-3.0.0/swh/scrubber/storage_checker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-# Copyright (C) 2021-2023  The Software Heritage developers
+# Copyright (C) 2021-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """Reads all objects in a swh-storage instance and recomputes their checksums."""
 
 import collections
 import contextlib
-from itertools import count, islice
 import json
 import logging
 from typing import Iterable, Optional, Tuple, Union
 
-import psycopg2
-import tenacity
-
-from swh.core.statsd import Statsd
 from swh.journal.serializers import value_to_kafka
 from swh.model import swhids
 from swh.model.model import (
     Content,
     Directory,
     ObjectType,
     Release,
@@ -31,15 +26,16 @@
     directory_get_many_with_possibly_duplicated_entries,
 )
 from swh.storage.algos.snapshot import snapshot_get_all_branches
 from swh.storage.cassandra.storage import CassandraStorage
 from swh.storage.interface import StorageInterface
 from swh.storage.postgresql.storage import Storage as PostgresqlStorage
 
-from .db import ConfigEntry, Datastore, ScrubberDb
+from .base_checker import BasePartitionChecker
+from .db import Datastore, ScrubberDb
 
 logger = logging.getLogger(__name__)
 
 ScrubbableObject = Union[Revision, Release, Snapshot, Directory, Content]
 
 
 @contextlib.contextmanager
@@ -109,102 +105,25 @@
             ),
         )
     else:
         raise NotImplementedError(f"StorageChecker(storage={storage!r}).datastore()")
     return datastore
 
 
-class StorageChecker:
+class StorageChecker(BasePartitionChecker):
     """Reads a chunk of a swh-storage database, recomputes checksums, and
     reports errors in a separate database."""
 
     def __init__(
         self, db: ScrubberDb, config_id: int, storage: StorageInterface, limit: int = 0
     ):
-        self.db = db
+        super().__init__(db=db, config_id=config_id, limit=limit)
         self.storage = storage
-        self.config_id = config_id
-        self.limit = limit
-
-        self._config: Optional[ConfigEntry] = None
-        self._statsd: Optional[Statsd] = None
-
-    @property
-    def config(self) -> ConfigEntry:
-        if self._config is None:
-            self._config = self.db.config_get(self.config_id)
-
-        assert self._config is not None
-        return self._config
-
-    @property
-    def nb_partitions(self) -> int:
-        return self.config.nb_partitions
-
-    @property
-    def object_type(self) -> swhids.ObjectType:
-        return self.config.object_type
-
-    @property
-    def check_hashes(self) -> bool:
-        return self.config.check_hashes
-
-    @property
-    def check_references(self) -> bool:
-        return self.config.check_references
-
-    @property
-    def datastore(self) -> Datastore:
-        """Returns a :class:`Datastore` instance representing the swh-storage instance
-        being checked."""
-        return self.config.datastore
-
-    @property
-    def statsd(self) -> Statsd:
-        if self._statsd is None:
-            self._statsd = Statsd(
-                namespace="swh_scrubber",
-                constant_tags={
-                    "object_type": self.object_type,
-                    "nb_partitions": self.nb_partitions,
-                    "datastore_package": self.datastore.package,
-                    "datastore_cls": self.datastore.cls,
-                },
-            )
-        return self._statsd
-
-    def run(self) -> None:
-        """Runs on all objects of ``object_type`` in a partition between
-        ``start_partition_id`` (inclusive) and ``end_partition_id`` (exclusive)
-        """
-        counter: Iterable[int] = count()
-        if self.limit:
-            counter = islice(counter, 0, self.limit)
-        for i, partition_id in zip(
-            counter, self.db.checked_partition_iter_next(self.config_id)
-        ):
-            logger.debug(
-                "Processing %s partition %d/%d",
-                self.object_type,
-                partition_id,
-                self.nb_partitions,
-            )
-
-            self._check_partition(self.object_type, partition_id)
 
-            self.db.checked_partition_upsert(
-                self.config_id,
-                partition_id,
-            )
-
-    @tenacity.retry(
-        retry=tenacity.retry_if_exception_type(psycopg2.OperationalError),
-        wait=tenacity.wait_random_exponential(min=10, max=180),
-    )
-    def _check_partition(
+    def check_partition(
         self, object_type: swhids.ObjectType, partition_id: int
     ) -> None:
         page_token = None
         while True:
             if object_type in (swhids.ObjectType.RELEASE, swhids.ObjectType.REVISION):
                 method = getattr(
                     self.storage, f"{self.object_type.name.lower()}_get_partition"
```

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/conftest.py` & `swh.scrubber-3.0.0/swh/scrubber/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# Copyright (C) 2022  The Software Heritage developers
+# Copyright (C) 2022-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import datetime
 from functools import partial
 
 import attr
 import pytest
 from pytest_postgresql import factories
 
 from swh.core.db.db_utils import initialize_database_for_module
 from swh.journal.serializers import value_to_kafka
+from swh.journal.writer import get_journal_writer
 from swh.model.hashutil import hash_to_bytes
 from swh.model.model import Directory, DirectoryEntry
 from swh.model.swhids import ObjectType
 from swh.model.tests.swh_model_data import DIRECTORIES
 from swh.scrubber.db import ConfigEntry, CorruptObject, Datastore, ScrubberDb
 
 scrubber_postgresql_proc = factories.postgresql_proc(
@@ -106,7 +107,31 @@
 def corrupt_object(scrubber_db, config_entry):
     return CorruptObject(
         id=ORIGINAL_DIRECTORY.swhid(),
         config=config_entry,
         first_occurrence=datetime.datetime.now(tz=datetime.timezone.utc),
         object_=value_to_kafka(CORRUPT_DIRECTORY.to_dict()),
     )
+
+
+@pytest.fixture
+def journal_client_config(
+    kafka_server: str, kafka_prefix: str, kafka_consumer_group: str
+):
+    return dict(
+        cls="kafka",
+        brokers=kafka_server,
+        group_id=kafka_consumer_group,
+        prefix=kafka_prefix,
+        on_eof="stop",
+    )
+
+
+@pytest.fixture
+def journal_writer(kafka_server: str, kafka_prefix: str):
+    return get_journal_writer(
+        cls="kafka",
+        brokers=[kafka_server],
+        client_id="kafka_writer",
+        prefix=kafka_prefix,
+        anonymize=False,
+    )
```

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/data/cli/sql/10-init-all.sql` & `swh.scrubber-3.0.0/swh/scrubber/tests/data/cli/sql/10-init-all.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/data/cli/sql/20-data.sql` & `swh.scrubber-3.0.0/swh/scrubber/tests/data/cli/sql/20-data.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/data/cli/sql/upgrades/006.sql` & `swh.scrubber-3.0.0/swh/scrubber/tests/data/cli/sql/upgrades/006.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/data/cli/sql/upgrades/007.sql` & `swh.scrubber-3.0.0/swh/scrubber/tests/data/cli/sql/upgrades/007.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/storage_checker_tests.py` & `swh.scrubber-3.0.0/swh/scrubber/tests/storage_checker_tests.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/test_cli.py` & `swh.scrubber-3.0.0/swh/scrubber/tests/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2020-2022  The Software Heritage developers
+# Copyright (C) 2020-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import json
 import tempfile
 from unittest.mock import MagicMock, call
@@ -15,14 +15,15 @@
 from swh.scrubber.storage_checker import postgresql_storage_db
 
 
 def invoke(
     scrubber_db,
     args,
     storage=None,
+    objstorage=None,
     kafka_server=None,
     kafka_prefix=None,
     kafka_consumer_group=None,
 ):
     runner = CliRunner()
 
     config = {
@@ -32,27 +33,29 @@
     if storage:
         with postgresql_storage_db(storage) as db:
             config["storage"] = {
                 "cls": "postgresql",
                 "db": db.conn.dsn,
                 "objstorage": {"cls": "memory"},
             }
+    if objstorage:
+        config["objstorage"] = {"cls": "memory"}
 
     assert (
         (kafka_server is None)
         == (kafka_prefix is None)
         == (kafka_consumer_group is None)
     )
     if kafka_server:
         config["journal"] = dict(
             cls="kafka",
             brokers=kafka_server,
             group_id=kafka_consumer_group,
             prefix=kafka_prefix,
-            stop_on_eof=True,
+            on_eof="stop",
         )
 
     with tempfile.NamedTemporaryFile("a", suffix=".yml") as config_fd:
         yaml.dump(config, config_fd)
         config_fd.seek(0)
         args = ["-C" + config_fd.name] + list(args)
         result = runner.invoke(scrubber_cli_group, args, catch_exceptions=False)
@@ -88,36 +91,36 @@
     msg = "Usage: scrubber check [OPTIONS] COMMAND [ARGS]..."
     assert output[0] == msg
     assert "Commands:" in output
     commands = [cmd.split()[0] for cmd in output[output.index("Commands:") + 1 :]]
     # With older click version (e.g. 7.0-1), the text wrapping can be different,
     # resulting in some docstring text included in this command list, so check we find
     # the expected commands instead
-    for command in ["init", "journal", "list", "stalled", "storage"]:
+    for command in ["init", "list", "run", "stalled"]:
         assert command in commands
+    for command in ["storage", "journal"]:
+        assert command not in commands
 
-    # without a config file, --help should still work but with an extra message
+    # without a config file, --help should still work
     result = CliRunner().invoke(
         scrubber_cli_group, ["check", "--help"], catch_exceptions=False
     )
     output = result.output.splitlines(keepends=False)
-    msg = "WARNING: You must have a scrubber configured in your config file."
-    assert output[0] == msg
     msg = "Usage: scrubber check [OPTIONS] COMMAND [ARGS]..."
-    assert output[2] == msg
+    assert output[0] == msg
     assert "Commands:" in output
     commands = [cmd.split()[0] for cmd in output[output.index("Commands:") + 1 :]]
     # With older click version (e.g. 7.0-1), the text wrapping can be different,
     # resulting in some docstring text included in this command list, so check we find
     # the expected commands instead
-    for command in ["init", "journal", "list", "stalled", "storage"]:
+    for command in ["init", "list", "run", "stalled"]:
         assert command in commands
 
 
-def test_check_init(mocker, scrubber_db, swh_storage):
+def test_check_init_storage(mocker, scrubber_db, swh_storage):
     mocker.patch("swh.scrubber.get_scrubber_db", return_value=scrubber_db)
     result = invoke(
         scrubber_db,
         [
             "check",
             "init",
             "storage",
@@ -201,14 +204,83 @@
     assert result.exit_code == 0, result.output
 
     cfg_entry = scrubber_db.config_get(scrubber_db.config_get_by_name(name))
     assert cfg_entry.check_hashes is False
     assert cfg_entry.check_references is True
 
 
+def test_check_init_objstorage(mocker, scrubber_db, swh_storage, swh_objstorage):
+    config_name = "cfg1"
+    mocker.patch("swh.scrubber.get_scrubber_db", return_value=scrubber_db)
+    result = invoke(
+        scrubber_db,
+        [
+            "check",
+            "init",
+            "objstorage",
+            "--object-type",
+            "content",
+            "--nb-partitions",
+            "4",
+            "--name",
+            config_name,
+        ],
+        storage=swh_storage,
+        objstorage=swh_objstorage,
+    )
+    assert result.exit_code == 0, result.output
+    msg = f"Created configuration {config_name} [1] for checking content in memory objstorage"
+    assert result.output.strip() == msg
+
+    cfg_entry = scrubber_db.config_get(scrubber_db.config_get_by_name(config_name))
+    assert cfg_entry.check_hashes is True
+    assert cfg_entry.check_references is True
+
+    # error: config name already exists
+    result = invoke(
+        scrubber_db,
+        [
+            "check",
+            "init",
+            "objstorage",
+            "--object-type",
+            "content",
+            "--nb-partitions",
+            "8",
+            "--name",
+            config_name,
+        ],
+        storage=swh_storage,
+        objstorage=swh_objstorage,
+    )
+    assert result.exit_code == 1, result.output
+    msg = f"Error: Configuration {config_name} already exists"
+    assert result.output.strip() == msg
+
+    # error: missing objstorage config
+    result = invoke(
+        scrubber_db,
+        [
+            "check",
+            "init",
+            "objstorage",
+            "--object-type",
+            "content",
+            "--nb-partitions",
+            "8",
+            "--name",
+            config_name,
+        ],
+        storage=swh_storage,
+    )
+    assert result.exit_code == 1, result.output
+    msg = "Error: You must have an object storage configured in your config file."
+    assert result.output.strip() == msg
+
+
 def test_check_init_journal_flags(
     mocker, scrubber_db, kafka_server, kafka_prefix, kafka_consumer_group
 ):
     mocker.patch("swh.scrubber.get_scrubber_db", return_value=scrubber_db)
     arg_list = [
         "check",
         "init",
@@ -229,15 +301,22 @@
     assert result.exit_code == 0, result.output
 
     cfg_entry = scrubber_db.config_get(scrubber_db.config_get_by_name(name))
     assert cfg_entry.check_hashes is True
     assert cfg_entry.check_references is False
 
 
-def test_check_storage(mocker, scrubber_db, swh_storage):
+def test_check_run_ko(mocker, scrubber_db, swh_storage):
+    # using the config id instead of the config name
+    result = invoke(scrubber_db, ["check", "run"], storage=swh_storage)
+    assert result.exit_code == 2, result.output
+    assert "Error: A valid configuration name/id must be given." in result.output
+
+
+def test_check_run_storage(mocker, scrubber_db, swh_storage):
     storage_checker = MagicMock()
     StorageChecker = mocker.patch(
         "swh.scrubber.storage_checker.StorageChecker", return_value=storage_checker
     )
     get_scrubber_db = mocker.patch(
         "swh.scrubber.get_scrubber_db", return_value=scrubber_db
     )
@@ -256,40 +335,221 @@
         ],
         storage=swh_storage,
     )
     assert result.exit_code == 0, result.output
     msg = "Created configuration cfg1 [1] for checking snapshot in postgresql storage"
     assert result.output.strip() == msg
 
-    result = invoke(scrubber_db, ["check", "storage", "cfg1"], storage=swh_storage)
+    result = invoke(scrubber_db, ["check", "run", "cfg1"], storage=swh_storage)
     assert result.exit_code == 0, result.output
     assert result.output == ""
 
     get_scrubber_db.assert_called_with(cls="postgresql", db=scrubber_db.conn.dsn)
     StorageChecker.assert_called_once_with(
         db=scrubber_db,
         config_id=1,
         storage=StorageChecker.mock_calls[0][2]["storage"],
         limit=0,
     )
     assert storage_checker.method_calls == [call.run()]
 
     # using the config id instead of the config name
     result = invoke(
-        scrubber_db, ["check", "storage", "--config-id", "1"], storage=swh_storage
+        scrubber_db, ["check", "run", "--config-id", "1"], storage=swh_storage
     )
     assert result.exit_code == 0, result.output
     assert result.output == ""
 
 
-def test_check_storage_ko(mocker, scrubber_db, swh_storage):
+def test_check_run_objstorage_partition(
+    mocker, scrubber_db, swh_storage, swh_objstorage
+):
+    config_name = "cfg1"
+    objstorage_checker = MagicMock()
+    ObjectStorageCheckerFromStoragePartition = mocker.patch(
+        "swh.scrubber.objstorage_checker.ObjectStorageCheckerFromStoragePartition",
+        return_value=objstorage_checker,
+    )
+    get_scrubber_db = mocker.patch(
+        "swh.scrubber.get_scrubber_db", return_value=scrubber_db
+    )
+    result = invoke(
+        scrubber_db,
+        [
+            "check",
+            "init",
+            "objstorage",
+            "--object-type",
+            "content",
+            "--nb-partitions",
+            "4",
+            "--name",
+            config_name,
+        ],
+        storage=swh_storage,
+        objstorage=swh_objstorage,
+    )
+    assert result.exit_code == 0, result.output
+    msg = f"Created configuration {config_name} [1] for checking content in memory objstorage"
+    assert result.output.strip() == msg
+
+    result = invoke(
+        scrubber_db,
+        ["check", "run", config_name],
+        storage=swh_storage,
+        objstorage=swh_objstorage,
+    )
+    assert result.exit_code == 0, result.output
+    assert result.output == ""
+
+    get_scrubber_db.assert_called_with(cls="postgresql", db=scrubber_db.conn.dsn)
+    ObjectStorageCheckerFromStoragePartition.assert_called_once_with(
+        db=scrubber_db,
+        config_id=1,
+        storage=ObjectStorageCheckerFromStoragePartition.mock_calls[0][2]["storage"],
+        objstorage=ObjectStorageCheckerFromStoragePartition.mock_calls[0][2][
+            "objstorage"
+        ],
+        limit=0,
+    )
+    assert objstorage_checker.method_calls == [call.run()]
+
     # using the config id instead of the config name
-    result = invoke(scrubber_db, ["check", "storage"], storage=swh_storage)
-    assert result.exit_code == 1, result.output
-    assert result.output == "Error: A valid configuration name/id must be set\n"
+    result = invoke(
+        scrubber_db,
+        ["check", "run", "--config-id", "1"],
+        storage=swh_storage,
+        objstorage=swh_objstorage,
+    )
+    assert result.exit_code == 0, result.output
+    assert result.output == ""
+
+
+def test_check_run_objstorage_journal(
+    mocker,
+    scrubber_db,
+    kafka_server,
+    kafka_prefix,
+    kafka_consumer_group,
+    swh_objstorage,
+):
+    config_name = "cfg1"
+    journal_checker = MagicMock()
+    ObjectStorageCheckerFromJournal = mocker.patch(
+        "swh.scrubber.objstorage_checker.ObjectStorageCheckerFromJournal",
+        return_value=journal_checker,
+    )
+    get_scrubber_db = mocker.patch(
+        "swh.scrubber.get_scrubber_db", return_value=scrubber_db
+    )
+    result = invoke(
+        scrubber_db,
+        [
+            "check",
+            "init",
+            "objstorage",
+            "--object-type",
+            "content",
+            "--name",
+            config_name,
+        ],
+        kafka_server=kafka_server,
+        kafka_prefix=kafka_prefix,
+        kafka_consumer_group=kafka_consumer_group,
+        objstorage=swh_objstorage,
+    )
+    assert result.exit_code == 0, result.output
+    msg = f"Created configuration {config_name} [1] for checking content in memory objstorage"
+    assert result.output.strip() == msg
+
+    result = invoke(
+        scrubber_db,
+        ["check", "run", "--use-journal", config_name],
+        kafka_server=kafka_server,
+        kafka_prefix=kafka_prefix,
+        kafka_consumer_group=kafka_consumer_group,
+        objstorage=swh_objstorage,
+    )
+    assert result.exit_code == 0, result.output
+    assert result.output == ""
+
+    assert get_scrubber_db.call_count == 2
+    get_scrubber_db.assert_called_with(cls="postgresql", db=scrubber_db.conn.dsn)
+
+    ObjectStorageCheckerFromJournal.assert_called_once_with(
+        db=scrubber_db,
+        journal_client_config={
+            "brokers": kafka_server,
+            "cls": "kafka",
+            "group_id": kafka_consumer_group,
+            "prefix": kafka_prefix,
+            "on_eof": "stop",
+        },
+        config_id=1,
+        objstorage=ObjectStorageCheckerFromJournal.mock_calls[0][2]["objstorage"],
+    )
+    assert journal_checker.method_calls == [call.run()]
+
+
+def test_check_run_journal(
+    mocker, scrubber_db, kafka_server, kafka_prefix, kafka_consumer_group
+):
+    journal_checker = MagicMock()
+    JournalChecker = mocker.patch(
+        "swh.scrubber.journal_checker.JournalChecker", return_value=journal_checker
+    )
+    get_scrubber_db = mocker.patch(
+        "swh.scrubber.get_scrubber_db", return_value=scrubber_db
+    )
+    result = invoke(
+        scrubber_db,
+        [
+            "check",
+            "init",
+            "journal",
+            "--object-type",
+            "snapshot",
+            "--nb-partitions",
+            "4",
+            "--name",
+            "cfg1",
+        ],
+        kafka_server=kafka_server,
+        kafka_prefix=kafka_prefix,
+        kafka_consumer_group=kafka_consumer_group,
+    )
+    assert result.exit_code == 0, result.output
+    msg = "Created configuration cfg1 [1] for checking snapshot in kafka journal"
+    assert result.output.strip() == msg
+
+    result = invoke(
+        scrubber_db,
+        ["check", "run", "cfg1"],
+        kafka_server=kafka_server,
+        kafka_prefix=kafka_prefix,
+        kafka_consumer_group=kafka_consumer_group,
+    )
+    assert result.exit_code == 0, result.output
+    assert result.output == ""
+
+    assert get_scrubber_db.call_count == 2
+    get_scrubber_db.assert_called_with(cls="postgresql", db=scrubber_db.conn.dsn)
+
+    JournalChecker.assert_called_once_with(
+        db=scrubber_db,
+        journal_client_config={
+            "brokers": kafka_server,
+            "cls": "kafka",
+            "group_id": kafka_consumer_group,
+            "prefix": kafka_prefix,
+            "on_eof": "stop",
+        },
+        config_id=1,
+    )
+    assert journal_checker.method_calls == [call.run()]
 
 
 def test_check_list(mocker, scrubber_db, swh_storage):
     mocker.patch("swh.scrubber.get_scrubber_db", return_value=scrubber_db)
     result = invoke(scrubber_db, ["check", "list"], storage=swh_storage)
     assert result.exit_code == 0, result.output
     assert result.output == ""
@@ -638,14 +898,116 @@
 
     # for good measure, check the next few selected partitions, expected 0, 1 and 3
     assert next(scrubber_db.checked_partition_iter_next(1)) == 0
     assert next(scrubber_db.checked_partition_iter_next(1)) == 1
     assert next(scrubber_db.checked_partition_iter_next(1)) == 3
 
 
+def test_locate_origins(mocker, scrubber_db, swh_storage, naive_graph_client):
+    origin_locator = MagicMock()
+    OriginLocator = mocker.patch(
+        "swh.scrubber.origin_locator.OriginLocator", return_value=origin_locator
+    )
+    get_scrubber_db = mocker.patch(
+        "swh.scrubber.get_scrubber_db", return_value=scrubber_db
+    )
+    mocker.patch(
+        "swh.graph.http_client.RemoteGraphClient",
+        return_value=naive_graph_client,
+    )
+
+    result = invoke(scrubber_db, ["locate"], storage=swh_storage)
+    assert result.exit_code == 0, result.output
+    assert result.output == ""
+
+    get_scrubber_db.assert_called_once_with(cls="postgresql", db=scrubber_db.conn.dsn)
+    OriginLocator.assert_called_once_with(
+        db=scrubber_db,
+        storage=OriginLocator.mock_calls[0][2]["storage"],
+        graph=OriginLocator.mock_calls[0][2]["graph"],
+        start_object=CoreSWHID.from_string("swh:1:cnt:" + "00" * 20),
+        end_object=CoreSWHID.from_string("swh:1:snp:" + "ff" * 20),
+    )
+    assert origin_locator.method_calls == [call.run()]
+
+
+def test_fix_objects(mocker, scrubber_db):
+    fixer = MagicMock()
+    Fixer = mocker.patch("swh.scrubber.fixer.Fixer", return_value=fixer)
+    get_scrubber_db = mocker.patch(
+        "swh.scrubber.get_scrubber_db", return_value=scrubber_db
+    )
+    result = invoke(scrubber_db, ["fix"])
+    assert result.exit_code == 0, result.output
+    assert result.output == ""
+
+    get_scrubber_db.assert_called_once_with(cls="postgresql", db=scrubber_db.conn.dsn)
+    Fixer.assert_called_once_with(
+        db=scrubber_db,
+        start_object=CoreSWHID.from_string("swh:1:cnt:" + "00" * 20),
+        end_object=CoreSWHID.from_string("swh:1:snp:" + "ff" * 20),
+    )
+    assert fixer.method_calls == [call.run()]
+
+
+# deprecated commands
+def test_check_storage(mocker, scrubber_db, swh_storage):
+    storage_checker = MagicMock()
+    StorageChecker = mocker.patch(
+        "swh.scrubber.storage_checker.StorageChecker", return_value=storage_checker
+    )
+    get_scrubber_db = mocker.patch(
+        "swh.scrubber.get_scrubber_db", return_value=scrubber_db
+    )
+    result = invoke(
+        scrubber_db,
+        [
+            "check",
+            "init",
+            "storage",
+            "--object-type",
+            "snapshot",
+            "--nb-partitions",
+            "4",
+            "--name",
+            "cfg1",
+        ],
+        storage=swh_storage,
+    )
+    assert result.exit_code == 0, result.output
+    msg = "Created configuration cfg1 [1] for checking snapshot in postgresql storage"
+    assert result.output.strip() == msg
+
+    result = invoke(scrubber_db, ["check", "storage", "cfg1"], storage=swh_storage)
+    assert result.exit_code == 0, result.output
+    assert (
+        result.output.strip()
+        == "DeprecationWarning: The command 'storage' is deprecated."
+    )
+
+    get_scrubber_db.assert_called_with(cls="postgresql", db=scrubber_db.conn.dsn)
+    StorageChecker.assert_called_once_with(
+        db=scrubber_db,
+        config_id=1,
+        storage=StorageChecker.mock_calls[0][2]["storage"],
+        limit=0,
+    )
+    assert storage_checker.method_calls == [call.run()]
+
+    # using the config id instead of the config name
+    result = invoke(
+        scrubber_db, ["check", "storage", "--config-id", "1"], storage=swh_storage
+    )
+    assert result.exit_code == 0, result.output
+    assert (
+        result.output.strip()
+        == "DeprecationWarning: The command 'storage' is deprecated."
+    )
+
+
 def test_check_journal(
     mocker, scrubber_db, kafka_server, kafka_prefix, kafka_consumer_group
 ):
     journal_checker = MagicMock()
     JournalChecker = mocker.patch(
         "swh.scrubber.journal_checker.JournalChecker", return_value=journal_checker
     )
@@ -677,71 +1039,27 @@
         scrubber_db,
         ["check", "journal", "cfg1"],
         kafka_server=kafka_server,
         kafka_prefix=kafka_prefix,
         kafka_consumer_group=kafka_consumer_group,
     )
     assert result.exit_code == 0, result.output
-    assert result.output == ""
+    assert (
+        result.output.strip()
+        == "DeprecationWarning: The command 'journal' is deprecated."
+    )
 
     assert get_scrubber_db.call_count == 2
     get_scrubber_db.assert_called_with(cls="postgresql", db=scrubber_db.conn.dsn)
 
     JournalChecker.assert_called_once_with(
         db=scrubber_db,
-        journal={
+        journal_client_config={
             "brokers": kafka_server,
             "cls": "kafka",
             "group_id": kafka_consumer_group,
             "prefix": kafka_prefix,
-            "stop_on_eof": True,
+            "on_eof": "stop",
         },
         config_id=1,
     )
     assert journal_checker.method_calls == [call.run()]
-
-
-def test_locate_origins(mocker, scrubber_db, swh_storage, naive_graph_client):
-    origin_locator = MagicMock()
-    OriginLocator = mocker.patch(
-        "swh.scrubber.origin_locator.OriginLocator", return_value=origin_locator
-    )
-    get_scrubber_db = mocker.patch(
-        "swh.scrubber.get_scrubber_db", return_value=scrubber_db
-    )
-    mocker.patch(
-        "swh.graph.http_client.RemoteGraphClient",
-        return_value=naive_graph_client,
-    )
-
-    result = invoke(scrubber_db, ["locate"], storage=swh_storage)
-    assert result.exit_code == 0, result.output
-    assert result.output == ""
-
-    get_scrubber_db.assert_called_once_with(cls="postgresql", db=scrubber_db.conn.dsn)
-    OriginLocator.assert_called_once_with(
-        db=scrubber_db,
-        storage=OriginLocator.mock_calls[0][2]["storage"],
-        graph=OriginLocator.mock_calls[0][2]["graph"],
-        start_object=CoreSWHID.from_string("swh:1:cnt:" + "00" * 20),
-        end_object=CoreSWHID.from_string("swh:1:snp:" + "ff" * 20),
-    )
-    assert origin_locator.method_calls == [call.run()]
-
-
-def test_fix_objects(mocker, scrubber_db):
-    fixer = MagicMock()
-    Fixer = mocker.patch("swh.scrubber.fixer.Fixer", return_value=fixer)
-    get_scrubber_db = mocker.patch(
-        "swh.scrubber.get_scrubber_db", return_value=scrubber_db
-    )
-    result = invoke(scrubber_db, ["fix"])
-    assert result.exit_code == 0, result.output
-    assert result.output == ""
-
-    get_scrubber_db.assert_called_once_with(cls="postgresql", db=scrubber_db.conn.dsn)
-    Fixer.assert_called_once_with(
-        db=scrubber_db,
-        start_object=CoreSWHID.from_string("swh:1:cnt:" + "00" * 20),
-        end_object=CoreSWHID.from_string("swh:1:snp:" + "ff" * 20),
-    )
-    assert fixer.method_calls == [call.run()]
```

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/test_db.py` & `swh.scrubber-3.0.0/swh/scrubber/tests/test_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -193,14 +193,31 @@
     date = datetime.datetime.now(tz=datetime.timezone.utc)
     scrubber_db.checked_partition_upsert(config_snp, 0, date)
     scrubber_db.checked_partition_upsert(config_id, 2, date)
 
     assert next(snp_part_gen) == 3
     assert next(dir_part_gen) == 4
 
+    # iterate on all 64 possible partitions for the config config_id (5 of them
+    # are already affected, so 59 to go)
+    for i in range(59):
+        assert next(dir_part_gen) == (i + 5)
+    # we should be at the end of the partitions now...
+    with pytest.raises(StopIteration):
+        next(dir_part_gen)
+    # check we still do not get anything after 63 with a new iterator
+    assert list(scrubber_db.checked_partition_iter_next(config_id)) == []
+    # check the database is OK with that
+    with scrubber_db.transaction() as cur:
+        cur.execute(
+            "select max(partition_id) from checked_partition where config_id=%s",
+            (config_id,),
+        )
+        assert cur.fetchone() == (63,)
+
 
 def test_checked_partition_get_next_with_hole(
     datastore: Datastore, scrubber_db: ScrubberDb, config_id: int
 ):
     dir_part_gen = scrubber_db.checked_partition_iter_next(config_id)
 
     # fill the checked_partition table
```

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/test_fixer.py` & `swh.scrubber-3.0.0/swh/scrubber/tests/test_fixer.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/test_init.py` & `swh.scrubber-3.0.0/swh/scrubber/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/test_migration.py` & `swh.scrubber-3.0.0/swh/scrubber/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/test_origin_locator.py` & `swh.scrubber-3.0.0/swh/scrubber/tests/test_origin_locator.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/test_storage_cassandra.py` & `swh.scrubber-3.0.0/swh/scrubber/tests/test_storage_cassandra.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/tests/test_storage_postgresql.py` & `swh.scrubber-3.0.0/swh/scrubber/tests/test_storage_postgresql.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh/scrubber/utils.py` & `swh.scrubber-3.0.0/swh/scrubber/utils.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.3.0/swh.scrubber.egg-info/SOURCES.txt` & `swh.scrubber-3.0.0/swh.scrubber.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 swh.scrubber.egg-info/PKG-INFO
 swh.scrubber.egg-info/SOURCES.txt
 swh.scrubber.egg-info/dependency_links.txt
 swh.scrubber.egg-info/entry_points.txt
 swh.scrubber.egg-info/requires.txt
 swh.scrubber.egg-info/top_level.txt
 swh/scrubber/__init__.py
+swh/scrubber/base_checker.py
 swh/scrubber/cli.py
 swh/scrubber/db.py
 swh/scrubber/fixer.py
 swh/scrubber/journal_checker.py
+swh/scrubber/objstorage_checker.py
 swh/scrubber/origin_locator.py
 swh/scrubber/py.typed
 swh/scrubber/storage_checker.py
 swh/scrubber/utils.py
 swh/scrubber/sql/20-enums.sql
 swh/scrubber/sql/30-schema.sql
 swh/scrubber/sql/60-indexes.sql
@@ -47,21 +49,24 @@
 swh/scrubber/sql/upgrades/3.sql
 swh/scrubber/sql/upgrades/4.sql
 swh/scrubber/sql/upgrades/5.sql
 swh/scrubber/sql/upgrades/6.sql
 swh/scrubber/sql/upgrades/7.sql
 swh/scrubber/tests/__init__.py
 swh/scrubber/tests/conftest.py
+swh/scrubber/tests/objstorage_checker_tests.py
 swh/scrubber/tests/storage_checker_tests.py
 swh/scrubber/tests/test_cli.py
 swh/scrubber/tests/test_db.py
 swh/scrubber/tests/test_fixer.py
 swh/scrubber/tests/test_init.py
 swh/scrubber/tests/test_journal_kafka.py
 swh/scrubber/tests/test_migration.py
+swh/scrubber/tests/test_objstorage_memory.py
+swh/scrubber/tests/test_objstorage_pathslicing.py
 swh/scrubber/tests/test_origin_locator.py
 swh/scrubber/tests/test_storage_cassandra.py
 swh/scrubber/tests/test_storage_postgresql.py
 swh/scrubber/tests/data/cli/sql/10-init-all.sql
 swh/scrubber/tests/data/cli/sql/20-data.sql
 swh/scrubber/tests/data/cli/sql/upgrades/006.sql
 swh/scrubber/tests/data/cli/sql/upgrades/007.sql
```

