# Comparing `tmp/permit-2.3.0.tar.gz` & `tmp/permit-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-2.3.0.tar", last modified: Tue Jan 30 14:35:40 2024, max compression
+gzip compressed data, was "permit-2.4.0.tar", last modified: Thu Apr 11 18:30:39 2024, max compression
```

## Comparing `permit-2.3.0.tar` & `permit-2.4.0.tar`

### file list

```diff
@@ -1,66 +1,72 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-01-30 14:35:40.944983 permit-2.3.0/
--rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.3.0/LICENSE
--rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.3.0/MANIFEST.in
--rw-r--r--   0 asafc      (501) staff       (20)      478 2024-01-30 14:35:40.944790 permit-2.3.0/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.3.0/README.md
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-01-30 14:35:40.938112 permit-2.3.0/permit/
--rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.3.0/permit/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-01-30 14:35:40.942727 permit-2.3.0/permit/api/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.3.0/permit/api/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     5622 2024-01-10 05:48:29.000000 permit-2.3.0/permit/api/api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)    11982 2023-10-26 17:32:16.000000 permit-2.3.0/permit/api/base.py
--rw-r--r--   0 asafc      (501) staff       (20)     4020 2023-10-26 17:32:16.000000 permit-2.3.0/permit/api/condition_set_rules.py
--rw-r--r--   0 asafc      (501) staff       (20)     6218 2023-10-26 17:32:16.000000 permit-2.3.0/permit/api/condition_sets.py
--rw-r--r--   0 asafc      (501) staff       (20)     8347 2023-06-15 09:35:28.000000 permit-2.3.0/permit/api/context.py
--rw-r--r--   0 asafc      (501) staff       (20)     6493 2023-06-15 09:35:28.000000 permit-2.3.0/permit/api/deprecated.py
--rw-r--r--   0 asafc      (501) staff       (20)     2102 2023-10-26 17:32:16.000000 permit-2.3.0/permit/api/elements.py
--rw-r--r--   0 asafc      (501) staff       (20)     9818 2023-10-26 17:32:16.000000 permit-2.3.0/permit/api/environments.py
--rw-r--r--   0 asafc      (501) staff       (20)   160550 2024-01-30 14:35:31.000000 permit-2.3.0/permit/api/models.py
--rw-r--r--   0 asafc      (501) staff       (20)     5864 2023-10-26 17:32:16.000000 permit-2.3.0/permit/api/projects.py
--rw-r--r--   0 asafc      (501) staff       (20)     6510 2024-01-10 05:48:29.000000 permit-2.3.0/permit/api/relationship_tuples.py
--rw-r--r--   0 asafc      (501) staff       (20)     7176 2023-10-26 17:32:16.000000 permit-2.3.0/permit/api/resource_action_groups.py
--rw-r--r--   0 asafc      (501) staff       (20)     6842 2023-10-26 17:32:16.000000 permit-2.3.0/permit/api/resource_actions.py
--rw-r--r--   0 asafc      (501) staff       (20)     7148 2023-10-26 17:32:16.000000 permit-2.3.0/permit/api/resource_attributes.py
--rw-r--r--   0 asafc      (501) staff       (20)     9617 2024-01-30 14:35:31.000000 permit-2.3.0/permit/api/resource_instances.py
--rw-r--r--   0 asafc      (501) staff       (20)     5941 2023-10-26 17:32:16.000000 permit-2.3.0/permit/api/resource_relations.py
--rw-r--r--   0 asafc      (501) staff       (20)    12471 2023-10-26 17:32:16.000000 permit-2.3.0/permit/api/resource_roles.py
--rw-r--r--   0 asafc      (501) staff       (20)     6814 2023-10-26 17:32:16.000000 permit-2.3.0/permit/api/resources.py
--rw-r--r--   0 asafc      (501) staff       (20)     6265 2024-01-28 11:37:43.000000 permit-2.3.0/permit/api/role_assignments.py
--rw-r--r--   0 asafc      (501) staff       (20)     7541 2023-10-26 17:32:16.000000 permit-2.3.0/permit/api/roles.py
--rw-r--r--   0 asafc      (501) staff       (20)     7125 2024-01-10 05:48:29.000000 permit-2.3.0/permit/api/sync_api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     9843 2024-01-30 14:35:31.000000 permit-2.3.0/permit/api/tenants.py
--rw-r--r--   0 asafc      (501) staff       (20)    12949 2024-01-30 14:35:31.000000 permit-2.3.0/permit/api/users.py
--rw-r--r--   0 asafc      (501) staff       (20)     2193 2023-10-26 17:32:16.000000 permit-2.3.0/permit/config.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-01-30 14:35:40.943083 permit-2.3.0/permit/enforcement/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.3.0/permit/enforcement/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)    13219 2024-01-25 15:15:50.000000 permit-2.3.0/permit/enforcement/enforcer.py
--rw-r--r--   0 asafc      (501) staff       (20)      943 2023-10-26 17:32:16.000000 permit-2.3.0/permit/enforcement/interfaces.py
--rw-r--r--   0 asafc      (501) staff       (20)     3933 2024-01-30 14:35:31.000000 permit-2.3.0/permit/exceptions.py
--rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.3.0/permit/logger.py
--rw-r--r--   0 asafc      (501) staff       (20)     4545 2024-01-09 15:17:30.000000 permit-2.3.0/permit/permit.py
--rw-r--r--   0 asafc      (501) staff       (20)     3923 2024-01-09 15:17:30.000000 permit-2.3.0/permit/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-01-30 14:35:40.943649 permit-2.3.0/permit/utils/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.3.0/permit/utils/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.3.0/permit/utils/context.py
--rw-r--r--   0 asafc      (501) staff       (20)      625 2023-06-15 09:35:28.000000 permit-2.3.0/permit/utils/deprecation.py
--rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.3.0/permit/utils/dicts.py
--rw-r--r--   0 asafc      (501) staff       (20)       85 2023-10-26 17:32:16.000000 permit-2.3.0/permit/utils/pydantic_version.py
--rw-r--r--   0 asafc      (501) staff       (20)     1130 2023-06-15 09:35:28.000000 permit-2.3.0/permit/utils/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-01-30 14:35:40.938625 permit-2.3.0/permit.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)      478 2024-01-30 14:35:40.000000 permit-2.3.0/permit.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     1379 2024-01-30 14:35:40.000000 permit-2.3.0/permit.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2024-01-30 14:35:40.000000 permit-2.3.0/permit.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)      104 2024-01-30 14:35:40.000000 permit-2.3.0/permit.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       13 2024-01-30 14:35:40.000000 permit-2.3.0/permit.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)      104 2023-10-26 17:32:16.000000 permit-2.3.0/requirements.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2024-01-30 14:35:40.945031 permit-2.3.0/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)      793 2024-01-30 14:35:31.000000 permit-2.3.0/setup.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-01-30 14:35:40.944613 permit-2.3.0/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.3.0/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1894 2024-01-30 14:26:21.000000 permit-2.3.0/tests/conftest.py
--rw-r--r--   0 asafc      (501) staff       (20)    10459 2024-01-09 15:17:30.000000 permit-2.3.0/tests/test_abac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)      943 2024-01-25 15:15:50.000000 permit-2.3.0/tests/test_abac_pdp.py
--rw-r--r--   0 asafc      (501) staff       (20)     9931 2024-01-09 15:17:30.000000 permit-2.3.0/tests/test_rbac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)     9688 2024-01-09 15:17:30.000000 permit-2.3.0/tests/test_rbac_e2e_sync.py
--rw-r--r--   0 asafc      (501) staff       (20)    30220 2024-01-10 05:48:29.000000 permit-2.3.0/tests/test_rebac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)      358 2024-01-30 14:35:31.000000 permit-2.3.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.445193 permit-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 18:29:07.000000 permit-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 18:29:07.000000 permit-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-11 18:30:39.445193 permit-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-11 18:29:07.000000 permit-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.441193 permit-2.4.0/permit/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-11 18:29:07.000000 permit-2.4.0/permit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.445193 permit-2.4.0/permit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/condition_set_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/condition_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9818 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)   160550 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/relationship_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resource_action_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resource_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resource_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resource_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resource_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resource_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/role_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/sync_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-11 18:29:07.000000 permit-2.4.0/permit/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.445193 permit-2.4.0/permit/enforcement/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:29:07.000000 permit-2.4.0/permit/enforcement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-04-11 18:29:07.000000 permit-2.4.0/permit/enforcement/enforcer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-11 18:29:07.000000 permit-2.4.0/permit/enforcement/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-11 18:29:07.000000 permit-2.4.0/permit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-11 18:29:07.000000 permit-2.4.0/permit/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.445193 permit-2.4.0/permit/pdp_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:29:07.000000 permit-2.4.0/permit/pdp_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-11 18:29:07.000000 permit-2.4.0/permit/pdp_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-11 18:29:07.000000 permit-2.4.0/permit/pdp_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-11 18:29:07.000000 permit-2.4.0/permit/pdp_api/pdp_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-11 18:29:07.000000 permit-2.4.0/permit/pdp_api/role_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-11 18:29:07.000000 permit-2.4.0/permit/permit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-11 18:29:07.000000 permit-2.4.0/permit/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.445193 permit-2.4.0/permit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:29:07.000000 permit-2.4.0/permit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-11 18:29:07.000000 permit-2.4.0/permit/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-11 18:29:07.000000 permit-2.4.0/permit/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-11 18:29:07.000000 permit-2.4.0/permit/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-11 18:29:07.000000 permit-2.4.0/permit/utils/pydantic_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-11 18:29:07.000000 permit-2.4.0/permit/utils/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.441193 permit-2.4.0/permit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-11 18:30:39.000000 permit-2.4.0/permit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-11 18:30:39.000000 permit-2.4.0/permit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:30:39.000000 permit-2.4.0/permit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 18:30:39.000000 permit-2.4.0/permit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 18:30:39.000000 permit-2.4.0/permit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 18:29:07.000000 permit-2.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 18:30:39.445193 permit-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-11 18:30:37.000000 permit-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.445193 permit-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:29:07.000000 permit-2.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-11 18:29:07.000000 permit-2.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-04-11 18:29:07.000000 permit-2.4.0/tests/test_abac_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-11 18:29:07.000000 permit-2.4.0/tests/test_abac_pdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-04-11 18:29:07.000000 permit-2.4.0/tests/test_rbac_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-11 18:29:07.000000 permit-2.4.0/tests/test_rbac_e2e_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30220 2024-04-11 18:29:07.000000 permit-2.4.0/tests/test_rebac_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-11 18:29:07.000000 permit-2.4.0/tests/utils.py
```

### Comparing `permit-2.3.0/LICENSE` & `permit-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/api_client.py` & `permit-2.4.0/permit/api/api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/base.py` & `permit-2.4.0/permit/api/base.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/condition_set_rules.py` & `permit-2.4.0/permit/api/condition_set_rules.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/condition_sets.py` & `permit-2.4.0/permit/api/condition_sets.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/context.py` & `permit-2.4.0/permit/api/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/deprecated.py` & `permit-2.4.0/permit/api/deprecated.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/elements.py` & `permit-2.4.0/permit/api/elements.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/environments.py` & `permit-2.4.0/permit/api/environments.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/models.py` & `permit-2.4.0/permit/api/models.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/projects.py` & `permit-2.4.0/permit/api/projects.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/relationship_tuples.py` & `permit-2.4.0/permit/api/relationship_tuples.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/resource_action_groups.py` & `permit-2.4.0/permit/api/resource_action_groups.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/resource_actions.py` & `permit-2.4.0/permit/api/resource_actions.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/resource_attributes.py` & `permit-2.4.0/permit/api/resource_attributes.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/resource_instances.py` & `permit-2.4.0/permit/api/resource_instances.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/resource_relations.py` & `permit-2.4.0/permit/api/resource_relations.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/resource_roles.py` & `permit-2.4.0/permit/api/resource_roles.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/resources.py` & `permit-2.4.0/permit/api/resources.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/role_assignments.py` & `permit-2.4.0/permit/api/role_assignments.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/roles.py` & `permit-2.4.0/permit/api/roles.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/sync_api_client.py` & `permit-2.4.0/permit/api/sync_api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/tenants.py` & `permit-2.4.0/permit/api/tenants.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/api/users.py` & `permit-2.4.0/permit/api/users.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/config.py` & `permit-2.4.0/permit/config.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/enforcement/enforcer.py` & `permit-2.4.0/permit/enforcement/enforcer.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/enforcement/interfaces.py` & `permit-2.4.0/permit/enforcement/interfaces.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/exceptions.py` & `permit-2.4.0/permit/exceptions.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/permit.py` & `permit-2.4.0/permit/permit.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 from loguru import logger
 
 from .api.api_client import PermitApiClient
 from .api.elements import ElementsApi
 from .config import PermitConfig
 from .enforcement.enforcer import Action, CheckQuery, Enforcer, Resource, User
 from .logger import configure_logger
+from .pdp_api.pdp_api_client import PermitPdpApiClient
 from .utils.context import Context
 
 
 class Permit:
     def __init__(self, config: Optional[PermitConfig] = None, **options):
         self._config: PermitConfig = (
             config if config is not None else PermitConfig(**options)
         )
 
         configure_logger(self._config)
         self._enforcer = Enforcer(self._config)
         self._api = PermitApiClient(self._config)
         self._elements = ElementsApi(self._config)
-
+        self._pdp_api = PermitPdpApiClient(self._config)
         logger.debug(
             "Permit SDK initialized with config:\n${}",
             json.dumps(self._config.dict(exclude={"api_context"})),
         )
 
     @property
     def config(self):
@@ -60,14 +61,26 @@
         Usage example:
 
             permit = Permit(token="<YOUR_API_KEY>")
             await permit.elements.loginAs(user, tenant)
         """
         return self._elements
 
+    @property
+    def pdp_api(self) -> PermitPdpApiClient:
+        """
+        Access the Permit PDP API using this property.
+
+        Usage example:
+
+            permit = Permit(token="<YOUR_API_KEY>")
+            await permit.pdp_api.role_assignments.list()
+        """
+        return self._pdp_api
+
     async def bulk_check(
         self,
         checks: list[CheckQuery],
         context: Context = {},
     ) -> list[bool]:
         """
         Checks if a user is authorized to perform an action on a list of resources within the specified context.
```

### Comparing `permit-2.3.0/permit/sync.py` & `permit-2.4.0/permit/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/utils/context.py` & `permit-2.4.0/permit/utils/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/utils/deprecation.py` & `permit-2.4.0/permit/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit/utils/sync.py` & `permit-2.4.0/permit/utils/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/permit.egg-info/SOURCES.txt` & `permit-2.4.0/permit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 permit/api/roles.py
 permit/api/sync_api_client.py
 permit/api/tenants.py
 permit/api/users.py
 permit/enforcement/__init__.py
 permit/enforcement/enforcer.py
 permit/enforcement/interfaces.py
+permit/pdp_api/__init__.py
+permit/pdp_api/base.py
+permit/pdp_api/models.py
+permit/pdp_api/pdp_api_client.py
+permit/pdp_api/role_assignments.py
 permit/utils/__init__.py
 permit/utils/context.py
 permit/utils/deprecation.py
 permit/utils/dicts.py
 permit/utils/pydantic_version.py
 permit/utils/sync.py
 tests/__init__.py
```

### Comparing `permit-2.3.0/setup.py` & `permit-2.4.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,37 @@
+from pathlib import Path
+
 from setuptools import find_packages, setup
 
 
 def get_requirements(env=""):
     if env:
         env = "-{}".format(env)
     with open("requirements{}.txt".format(env)) as fp:
         return [x.strip() for x in fp.read().split("\n") if not x.startswith("#")]
 
 
+def get_readme() -> str:
+    this_directory = Path(__file__).parent
+    long_description = (this_directory / "README.md").read_text()
+    return long_description
+
+
 setup(
     name="permit",
-    version="2.3.0",
+    version="2.4.0",
     packages=find_packages(),
     author="Asaf Cohen",
     author_email="asaf@permit.io",
     license="Apache 2.0",
     python_requires=">=3.8",
     description="Permit.io python sdk",
     install_requires=get_requirements(),
+    long_description=get_readme(),
+    long_description_content_type="text/markdown",
     classifiers=[
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
```

### Comparing `permit-2.3.0/tests/conftest.py` & `permit-2.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/tests/test_abac_e2e.py` & `permit-2.4.0/tests/test_abac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/tests/test_abac_pdp.py` & `permit-2.4.0/tests/test_abac_pdp.py`

 * *Files identical despite different names*

### Comparing `permit-2.3.0/tests/test_rbac_e2e.py` & `permit-2.4.0/tests/test_rbac_e2e_sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import time
 from typing import List
 
 import pytest
 from loguru import logger
 
-from permit import Permit, RoleAssignmentRead
+from permit import RoleAssignmentRead
 from permit.exceptions import PermitApiError, PermitConnectionError
+from permit.sync import Permit as SyncPermit
 
 from .utils import handle_api_error
 
 
 def print_break():
     print("\n\n ----------- \n\n")
 
 
-async def test_permission_check_e2e(permit: Permit):
+def test_permission_check_e2e(sync_permit: SyncPermit):
+    permit = sync_permit
     logger.info("initial setup of objects")
     try:
-        document = await permit.api.resources.create(
+        document = permit.api.resources.create(
             {
                 "key": "document",
                 "name": "Document",
                 "urn": "prn:gdrive:document",
                 "description": "google drive document",
                 "actions": {
                     "create": {},
@@ -48,24 +50,24 @@
         assert len(document.actions or {}) == 4
         assert (document.actions or {}).get("create") is not None
         assert (document.actions or {}).get("read") is not None
         assert (document.actions or {}).get("update") is not None
         assert (document.actions or {}).get("delete") is not None
 
         # verify list output
-        resources = await permit.api.resources.list()
+        resources = permit.api.resources.list()
         assert len(resources) == 1
         assert resources[0].id == document.id
         assert resources[0].key == document.key
         assert resources[0].name == document.name
         assert resources[0].description == document.description
         assert resources[0].urn == document.urn
 
         # create admin role
-        admin = await permit.api.roles.create(
+        admin = permit.api.roles.create(
             {
                 "key": "admin",
                 "name": "Admin",
                 "description": "an admin role",
                 "permissions": ["document:create", "document:read"],
             }
         )
@@ -75,15 +77,15 @@
         assert admin.name == "Admin"
         assert admin.description == "an admin role"
         assert admin.permissions is not None
         assert "document:create" in admin.permissions
         assert "document:read" in admin.permissions
 
         # create viewer role
-        viewer = await permit.api.roles.create(
+        viewer = permit.api.roles.create(
             {
                 "key": "viewer",
                 "name": "Viewer",
                 "description": "an viewer role",
             }
         )
 
@@ -91,39 +93,39 @@
         assert viewer.key == "viewer"
         assert viewer.name == "Viewer"
         assert viewer.description == "an viewer role"
         assert viewer.permissions is not None
         assert len(viewer.permissions) == 0
 
         # assign permissions to roles
-        assigned_viewer = await permit.api.roles.assign_permissions(
+        assigned_viewer = permit.api.roles.assign_permissions(
             "viewer", ["document:read"]
         )
 
         assert assigned_viewer.key == "viewer"
         assert len(assigned_viewer.permissions) == 1
         assert "document:read" in assigned_viewer.permissions
         assert "document:create" not in assigned_viewer.permissions
 
         # create a tenant
-        tenant = await permit.api.tenants.create(
+        tenant = permit.api.tenants.create(
             {
                 "key": "tesla",
                 "name": "Tesla Inc",
                 "description": "The car company",
             }
         )
 
         assert tenant.key == "tesla"
         assert tenant.name == "Tesla Inc"
         assert tenant.description == "The car company"
         assert tenant.attributes is None or len(tenant.attributes) == 0
 
         # create a user
-        user = await permit.api.users.sync(
+        user = permit.api.users.sync(
             {
                 "key": "auth0|elon",
                 "email": "elonmusk@tesla.com",
                 "first_name": "Elon",
                 "last_name": "Musk",
                 "attributes": {
                     "age": 50,
@@ -137,15 +139,15 @@
         assert user.first_name == "Elon"
         assert user.last_name == "Musk"
         assert len(user.attributes or {}) == 2
         assert user.attributes["age"] == 50
         assert user.attributes["favoriteColor"] == "red"
 
         # assign role to user in tenant
-        ra = await permit.api.users.assign_role(
+        ra = permit.api.users.assign_role(
             {
                 "user": "auth0|elon",
                 "role": "viewer",
                 "tenant": "tesla",
             }
         )
 
@@ -160,92 +162,87 @@
             "sleeping 2 seconds before permit.check() to make sure all writes propagated from cloud to PDP"
         )
         time.sleep(2)
 
         # positive permission check (will be True because elon is a viewer, and a viewer can read a document)
         logger.info("testing positive permission check")
         resource_attributes = {"secret": True}
-        assert await permit.check(
+        assert permit.check(
             "auth0|elon",
             "read",
             {"type": "document", "tenant": "tesla", "attributes": resource_attributes},
         )
 
         print_break()
 
         logger.info("testing positive permission check with complete user object")
-        assert await permit.check(
+        assert permit.check(
             user.dict(), "read", {"type": document.key, "tenant": tenant.key}
         )
 
         print_break()
 
         # negative permission check (will be False because a viewer cannot create a document)
         logger.info("testing negative permission check")
         assert (
-            await permit.check(
+            permit.check(
                 user.key, "create", {"type": document.key, "tenant": tenant.key}
             )
         ) == False
 
         print_break()
 
-        logger.info("testing bulk permission check")
-        assert (
-            await permit.bulk_check(
-                [
-                    {
-                        "user": "auth0|elon",
-                        "action": "read",
-                        "resource": {
-                            "type": "document",
-                            "tenant": "tesla",
-                            "attributes": resource_attributes,
-                        },
-                    },
-                    {
-                        "user": user.dict(),
-                        "action": "read",
-                        "resource": {"type": document.key, "tenant": tenant.key},
-                    },
-                    {
-                        "user": user.key,
-                        "action": "create",
-                        "resource": {"type": document.key, "tenant": tenant.key},
+        logger.info("testing permissions in bulk")
+        assert permit.bulk_check(
+            [
+                {
+                    "user": "auth0|elon",
+                    "action": "read",
+                    "resource": {
+                        "type": "document",
+                        "tenant": "tesla",
+                        "attributes": resource_attributes,
                     },
-                ],
-                {},
-            )
+                },
+                {
+                    "user": user.dict(),
+                    "action": "read",
+                    "resource": {"type": document.key, "tenant": tenant.key},
+                },
+                {
+                    "user": user.key,
+                    "action": "create",
+                    "resource": {"type": document.key, "tenant": tenant.key},
+                },
+            ]
         ) == [True, True, False]
 
-        print_break()
-
         logger.info("changing the user roles")
 
         # change the user role - assign admin role
-        await permit.api.users.assign_role(
+        permit.api.users.assign_role(
             {
                 "user": user.key,
                 "role": admin.key,
                 "tenant": tenant.key,
             }
         )
         # change the user role - remove viewer role
-        await permit.api.users.unassign_role(
+        permit.api.users.unassign_role(
             {
                 "user": user.key,
                 "role": viewer.key,
                 "tenant": tenant.key,
             }
         )
 
         # list user roles in all tenants
-        assigned_roles: List[
-            RoleAssignmentRead
-        ] = await permit.api.users.get_assigned_roles(user=user.key)
+        assigned_roles: List[RoleAssignmentRead] = permit.api.users.get_assigned_roles(
+            user=user.key
+        )
 
         assert len(assigned_roles) == 1
         assert assigned_roles[0].user_id == user.id
         assert assigned_roles[0].role_id == admin.id
         assert assigned_roles[0].tenant_id == tenant.id
 
         logger.info(
@@ -253,15 +250,15 @@
         )
         time.sleep(2)
 
         # run the same negative permission check again, this time it's True
         logger.info(
             "testing previously negative permission check, should now be positive"
         )
-        assert await permit.check(
+        assert permit.check(
             user.dict(), "create", {"type": document.key, "tenant": tenant.key}
         )
 
         print_break()
 
     except PermitApiError as error:
         handle_api_error(error, "Got API Error")
@@ -269,23 +266,23 @@
         raise
     except Exception as error:
         logger.error(f"Got error: {error}")
         pytest.fail(f"Got error: {error}")
     finally:
         # cleanup
         try:
-            await permit.api.resources.delete("document")
-            await permit.api.roles.delete("admin")
-            await permit.api.roles.delete("viewer")
-            await permit.api.tenants.delete("tesla")
-            await permit.api.users.delete("auth0|elon")
-            assert len(await permit.api.resources.list()) == 0
-            assert len(await permit.api.roles.list()) == 0
-            assert len(await permit.api.tenants.list()) == 1  # the default tenant
-            assert len((await permit.api.users.list()).data) == 0
+            permit.api.resources.delete("document")
+            permit.api.roles.delete("admin")
+            permit.api.roles.delete("viewer")
+            permit.api.tenants.delete("tesla")
+            permit.api.users.delete("auth0|elon")
+            assert len(permit.api.resources.list()) == 0
+            assert len(permit.api.roles.list()) == 0
+            assert len(permit.api.tenants.list()) == 1  # the default tenant
+            assert len((permit.api.users.list()).data) == 0
         except PermitApiError as error:
             handle_api_error(error, "Got API Error during cleanup")
         except PermitConnectionError as error:
             raise
         except Exception as error:
             logger.error(f"Got error during cleanup: {error}")
             pytest.fail(f"Got error during cleanup: {error}")
```

### Comparing `permit-2.3.0/tests/test_rbac_e2e_sync.py` & `permit-2.4.0/tests/test_rbac_e2e.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import time
 from typing import List
 
 import pytest
 from loguru import logger
 
-from permit import RoleAssignmentRead
+from permit import Permit, RoleAssignmentRead
 from permit.exceptions import PermitApiError, PermitConnectionError
-from permit.sync import Permit as SyncPermit
+from permit.pdp_api.models import RoleAssignment
 
 from .utils import handle_api_error
 
 
 def print_break():
     print("\n\n ----------- \n\n")
 
 
-def test_permission_check_e2e(sync_permit: SyncPermit):
-    permit = sync_permit
+async def test_permission_check_e2e(permit: Permit):
     logger.info("initial setup of objects")
     try:
-        document = permit.api.resources.create(
+        document = await permit.api.resources.create(
             {
                 "key": "document",
                 "name": "Document",
                 "urn": "prn:gdrive:document",
                 "description": "google drive document",
                 "actions": {
                     "create": {},
@@ -50,24 +49,24 @@
         assert len(document.actions or {}) == 4
         assert (document.actions or {}).get("create") is not None
         assert (document.actions or {}).get("read") is not None
         assert (document.actions or {}).get("update") is not None
         assert (document.actions or {}).get("delete") is not None
 
         # verify list output
-        resources = permit.api.resources.list()
+        resources = await permit.api.resources.list()
         assert len(resources) == 1
         assert resources[0].id == document.id
         assert resources[0].key == document.key
         assert resources[0].name == document.name
         assert resources[0].description == document.description
         assert resources[0].urn == document.urn
 
         # create admin role
-        admin = permit.api.roles.create(
+        admin = await permit.api.roles.create(
             {
                 "key": "admin",
                 "name": "Admin",
                 "description": "an admin role",
                 "permissions": ["document:create", "document:read"],
             }
         )
@@ -77,15 +76,15 @@
         assert admin.name == "Admin"
         assert admin.description == "an admin role"
         assert admin.permissions is not None
         assert "document:create" in admin.permissions
         assert "document:read" in admin.permissions
 
         # create viewer role
-        viewer = permit.api.roles.create(
+        viewer = await permit.api.roles.create(
             {
                 "key": "viewer",
                 "name": "Viewer",
                 "description": "an viewer role",
             }
         )
 
@@ -93,39 +92,39 @@
         assert viewer.key == "viewer"
         assert viewer.name == "Viewer"
         assert viewer.description == "an viewer role"
         assert viewer.permissions is not None
         assert len(viewer.permissions) == 0
 
         # assign permissions to roles
-        assigned_viewer = permit.api.roles.assign_permissions(
+        assigned_viewer = await permit.api.roles.assign_permissions(
             "viewer", ["document:read"]
         )
 
         assert assigned_viewer.key == "viewer"
         assert len(assigned_viewer.permissions) == 1
         assert "document:read" in assigned_viewer.permissions
         assert "document:create" not in assigned_viewer.permissions
 
         # create a tenant
-        tenant = permit.api.tenants.create(
+        tenant = await permit.api.tenants.create(
             {
                 "key": "tesla",
                 "name": "Tesla Inc",
                 "description": "The car company",
             }
         )
 
         assert tenant.key == "tesla"
         assert tenant.name == "Tesla Inc"
         assert tenant.description == "The car company"
         assert tenant.attributes is None or len(tenant.attributes) == 0
 
         # create a user
-        user = permit.api.users.sync(
+        user = await permit.api.users.sync(
             {
                 "key": "auth0|elon",
                 "email": "elonmusk@tesla.com",
                 "first_name": "Elon",
                 "last_name": "Musk",
                 "attributes": {
                     "age": 50,
@@ -139,15 +138,15 @@
         assert user.first_name == "Elon"
         assert user.last_name == "Musk"
         assert len(user.attributes or {}) == 2
         assert user.attributes["age"] == 50
         assert user.attributes["favoriteColor"] == "red"
 
         # assign role to user in tenant
-        ra = permit.api.users.assign_role(
+        ra = await permit.api.users.assign_role(
             {
                 "user": "auth0|elon",
                 "role": "viewer",
                 "tenant": "tesla",
             }
         )
 
@@ -162,87 +161,102 @@
             "sleeping 2 seconds before permit.check() to make sure all writes propagated from cloud to PDP"
         )
         time.sleep(2)
 
         # positive permission check (will be True because elon is a viewer, and a viewer can read a document)
         logger.info("testing positive permission check")
         resource_attributes = {"secret": True}
-        assert permit.check(
+        assert await permit.check(
             "auth0|elon",
             "read",
             {"type": "document", "tenant": "tesla", "attributes": resource_attributes},
         )
 
         print_break()
 
         logger.info("testing positive permission check with complete user object")
-        assert permit.check(
+        assert await permit.check(
             user.dict(), "read", {"type": document.key, "tenant": tenant.key}
         )
 
         print_break()
 
         # negative permission check (will be False because a viewer cannot create a document)
         logger.info("testing negative permission check")
         assert (
-            permit.check(
+            await permit.check(
                 user.key, "create", {"type": document.key, "tenant": tenant.key}
             )
         ) == False
 
         print_break()
 
-        logger.info("testing permissions in bulk")
-        assert permit.bulk_check(
-            [
-                {
-                    "user": "auth0|elon",
-                    "action": "read",
-                    "resource": {
-                        "type": "document",
-                        "tenant": "tesla",
-                        "attributes": resource_attributes,
+        logger.info("testing bulk permission check")
+        assert (
+            await permit.bulk_check(
+                [
+                    {
+                        "user": "auth0|elon",
+                        "action": "read",
+                        "resource": {
+                            "type": "document",
+                            "tenant": "tesla",
+                            "attributes": resource_attributes,
+                        },
                     },
-                },
-                {
-                    "user": user.dict(),
-                    "action": "read",
-                    "resource": {"type": document.key, "tenant": tenant.key},
-                },
-                {
-                    "user": user.key,
-                    "action": "create",
-                    "resource": {"type": document.key, "tenant": tenant.key},
-                },
-            ]
+                    {
+                        "user": user.dict(),
+                        "action": "read",
+                        "resource": {"type": document.key, "tenant": tenant.key},
+                    },
+                    {
+                        "user": user.key,
+                        "action": "create",
+                        "resource": {"type": document.key, "tenant": tenant.key},
+                    },
+                ],
+                {},
+            )
         ) == [True, True, False]
 
+        print_break()
+
+        logger.info("testing list role assignments")
+        assignments_returned: List[
+            RoleAssignment
+        ] = await permit.pdp_api.role_assignments.list()
+        assert len(assignments_returned) == 1
+        assert assignments_returned[0].user == user.key
+        assert assignments_returned[0].role == viewer.key
+        assert assignments_returned[0].tenant == tenant.key
+        print_break()
+
         logger.info("changing the user roles")
 
         # change the user role - assign admin role
-        permit.api.users.assign_role(
+        await permit.api.users.assign_role(
             {
                 "user": user.key,
                 "role": admin.key,
                 "tenant": tenant.key,
             }
         )
         # change the user role - remove viewer role
-        permit.api.users.unassign_role(
+        await permit.api.users.unassign_role(
             {
                 "user": user.key,
                 "role": viewer.key,
                 "tenant": tenant.key,
             }
         )
 
         # list user roles in all tenants
-        assigned_roles: List[RoleAssignmentRead] = permit.api.users.get_assigned_roles(
-            user=user.key
-        )
+        assigned_roles: List[
+            RoleAssignmentRead
+        ] = await permit.api.users.get_assigned_roles(user=user.key)
 
         assert len(assigned_roles) == 1
         assert assigned_roles[0].user_id == user.id
         assert assigned_roles[0].role_id == admin.id
         assert assigned_roles[0].tenant_id == tenant.id
 
         logger.info(
@@ -250,15 +264,15 @@
         )
         time.sleep(2)
 
         # run the same negative permission check again, this time it's True
         logger.info(
             "testing previously negative permission check, should now be positive"
         )
-        assert permit.check(
+        assert await permit.check(
             user.dict(), "create", {"type": document.key, "tenant": tenant.key}
         )
 
         print_break()
 
     except PermitApiError as error:
         handle_api_error(error, "Got API Error")
@@ -266,23 +280,23 @@
         raise
     except Exception as error:
         logger.error(f"Got error: {error}")
         pytest.fail(f"Got error: {error}")
     finally:
         # cleanup
         try:
-            permit.api.resources.delete("document")
-            permit.api.roles.delete("admin")
-            permit.api.roles.delete("viewer")
-            permit.api.tenants.delete("tesla")
-            permit.api.users.delete("auth0|elon")
-            assert len(permit.api.resources.list()) == 0
-            assert len(permit.api.roles.list()) == 0
-            assert len(permit.api.tenants.list()) == 1  # the default tenant
-            assert len((permit.api.users.list()).data) == 0
+            await permit.api.resources.delete("document")
+            await permit.api.roles.delete("admin")
+            await permit.api.roles.delete("viewer")
+            await permit.api.tenants.delete("tesla")
+            await permit.api.users.delete("auth0|elon")
+            assert len(await permit.api.resources.list()) == 0
+            assert len(await permit.api.roles.list()) == 0
+            assert len(await permit.api.tenants.list()) == 1  # the default tenant
+            assert len((await permit.api.users.list()).data) == 0
         except PermitApiError as error:
             handle_api_error(error, "Got API Error during cleanup")
         except PermitConnectionError as error:
             raise
         except Exception as error:
             logger.error(f"Got error during cleanup: {error}")
             pytest.fail(f"Got error during cleanup: {error}")
```

### Comparing `permit-2.3.0/tests/test_rebac_e2e.py` & `permit-2.4.0/tests/test_rebac_e2e.py`

 * *Files identical despite different names*

