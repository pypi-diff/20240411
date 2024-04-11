# Comparing `tmp/taxhub-1.9.3.tar.gz` & `tmp/taxhub-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taxhub-1.9.3.tar", last modified: Wed Jan 12 15:03:48 2022, max compression
+gzip compressed data, was "taxhub-1.9.4.tar", last modified: Tue Jan 25 10:19:39 2022, max compression
```

## Comparing `taxhub-1.9.3.tar` & `taxhub-1.9.4.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:03:48.103815 taxhub-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-01-12 15:03:39.000000 taxhub-1.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-01-12 15:03:39.000000 taxhub-1.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-01-12 15:03:48.103815 taxhub-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3095 2022-01-12 15:03:39.000000 taxhub-1.9.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-12 15:03:39.000000 taxhub-1.9.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:03:48.095815 taxhub-1.9.3/apptax/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4520 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/database.py
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/index.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:03:48.095815 taxhub-1.9.3/apptax/log/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/log/logmanager.py
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/log/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:03:48.095815 taxhub-1.9.3/apptax/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:03:48.099815 taxhub-1.9.3/apptax/migrations/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25942 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/data/taxonomie.sql
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/data/taxonomie_attributes_example.sql
--rw-r--r--   0 runner    (1001) docker     (121)     3530 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/data/taxonomie_bdc_statuts.sql
--rw-r--r--   0 runner    (1001) docker     (121)     4501 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/data/taxonomie_data.sql
--rw-r--r--   0 runner    (1001) docker     (121)     6062 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/data/taxonomie_materialized_views.sql
--rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/data/taxonomie_taxons_example.sql
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:03:48.099815 taxhub-1.9.3/apptax/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/versions/3fe8c07741be_taxhub_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/versions/4fb7e197d241_fix_v_bdc_status_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/versions/7540702c6407_cd_ref_utility_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/versions/8222017dc3f6_add_taxons_exemple_to_taxonomie.py
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/versions/98035939bc0d_find_all_taxons_parents.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/versions/9c2c0254aadc_create_taxonomie_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/versions/aa7533601e41_add_attributes_exemple_to_taxonomie.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/versions/c93cbb35cfe4_set_default_value_for_id_liste.py
--rw-r--r--   0 runner    (1001) docker     (121)    13419 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/versions/f61f95136ec3_insert_inpn_data_in_taxonomie_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1843 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/migrations/versions/fa5a90853c45_taxhub.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:03:48.099815 taxhub-1.9.3/apptax/taxonomie/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/taxonomie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9918 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/taxonomie/filemanager.py
--rw-r--r--   0 runner    (1001) docker     (121)    14358 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/taxonomie/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     7927 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/taxonomie/repositories.py
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/taxonomie/routesbdcstatuts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/taxonomie/routesbibattributs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9375 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/taxonomie/routesbiblistes.py
--rw-r--r--   0 runner    (1001) docker     (121)    10246 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/taxonomie/routesbibnoms.py
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/taxonomie/routesbibtypesmedia.py
--rw-r--r--   0 runner    (1001) docker     (121)    15453 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/taxonomie/routestaxref.py
--rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/taxonomie/routestmedias.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:03:48.099815 taxhub-1.9.3/apptax/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/utils/genericfunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/utils/routesconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     4034 2022-01-12 15:03:39.000000 taxhub-1.9.3/apptax/utils/utilssqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-01-12 15:03:39.000000 taxhub-1.9.3/requirements.in
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-12 15:03:48.103815 taxhub-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-01-12 15:03:39.000000 taxhub-1.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:03:48.103815 taxhub-1.9.3/taxhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-01-12 15:03:48.000000 taxhub-1.9.3/taxhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1977 2022-01-12 15:03:48.000000 taxhub-1.9.3/taxhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-12 15:03:48.000000 taxhub-1.9.3/taxhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-01-12 15:03:48.000000 taxhub-1.9.3/taxhub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-01-12 15:03:48.000000 taxhub-1.9.3/taxhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-12 15:03:48.000000 taxhub-1.9.3/taxhub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 10:19:39.150679 taxhub-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-01-25 10:19:27.000000 taxhub-1.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-01-25 10:19:27.000000 taxhub-1.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-01-25 10:19:39.150679 taxhub-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3095 2022-01-25 10:19:27.000000 taxhub-1.9.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-25 10:19:27.000000 taxhub-1.9.4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 10:19:39.142679 taxhub-1.9.4/apptax/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4555 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/index.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 10:19:39.142679 taxhub-1.9.4/apptax/log/
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/log/logmanager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/log/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 10:19:39.146679 taxhub-1.9.4/apptax/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 10:19:39.146679 taxhub-1.9.4/apptax/migrations/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25942 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/data/taxonomie.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      977 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/data/taxonomie_attributes_example.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     3530 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/data/taxonomie_bdc_statuts.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     4501 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/data/taxonomie_data.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     6062 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/data/taxonomie_materialized_views.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/data/taxonomie_taxons_example.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 10:19:39.146679 taxhub-1.9.4/apptax/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/versions/3fe8c07741be_taxhub_admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/versions/4fb7e197d241_fix_v_bdc_status_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/versions/7540702c6407_cd_ref_utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      921 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/versions/8222017dc3f6_add_taxons_exemple_to_taxonomie.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/versions/98035939bc0d_find_all_taxons_parents.py
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/versions/9c2c0254aadc_create_taxonomie_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      621 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/versions/aa7533601e41_add_attributes_exemple_to_taxonomie.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/versions/c93cbb35cfe4_set_default_value_for_id_liste.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13419 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/versions/f61f95136ec3_insert_inpn_data_in_taxonomie_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1843 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/migrations/versions/fa5a90853c45_taxhub.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 10:19:39.146679 taxhub-1.9.4/apptax/taxonomie/
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/taxonomie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9918 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/taxonomie/filemanager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14372 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/taxonomie/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7927 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/taxonomie/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/taxonomie/routesbdcstatuts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/taxonomie/routesbibattributs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9375 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/taxonomie/routesbiblistes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10246 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/taxonomie/routesbibnoms.py
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/taxonomie/routesbibtypesmedia.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15587 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/taxonomie/routestaxref.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/taxonomie/routestmedias.py
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 10:19:39.146679 taxhub-1.9.4/apptax/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      718 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/utils/genericfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/utils/routesconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4034 2022-01-25 10:19:27.000000 taxhub-1.9.4/apptax/utils/utilssqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-01-25 10:19:27.000000 taxhub-1.9.4/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-25 10:19:39.150679 taxhub-1.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-01-25 10:19:27.000000 taxhub-1.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 10:19:39.146679 taxhub-1.9.4/taxhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-01-25 10:19:39.000000 taxhub-1.9.4/taxhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-01-25 10:19:39.000000 taxhub-1.9.4/taxhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 10:19:39.000000 taxhub-1.9.4/taxhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-01-25 10:19:39.000000 taxhub-1.9.4/taxhub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-01-25 10:19:39.000000 taxhub-1.9.4/taxhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-25 10:19:39.000000 taxhub-1.9.4/taxhub.egg-info/top_level.txt
```

### Comparing `taxhub-1.9.3/LICENSE` & `taxhub-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/PKG-INFO` & `taxhub-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxhub
-Version: 1.9.3
+Version: 1.9.4
 Summary: Application web de gestion centralisée des taxons basée sur le référentiel TAXREF
 Home-page: https://github.com/PnX-SI/TaxHub
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
```

### Comparing `taxhub-1.9.3/README.rst` & `taxhub-1.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/app.py` & `taxhub-1.9.4/apptax/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     alembic_config.set_main_option('version_locations', ' '.join(version_locations))
     return alembic_config
 
 
 def create_app():
     app = Flask(__name__, template_folder='../templates', static_folder='../static')
 
-    app.config.from_pyfile("config.py")
+    app.config.from_pyfile(os.environ.get("TAXHUB_SETTINGS", "config.py"))
 
     # Patch suppression de static du paramètre UPLOAD_FOLDER
     # TODO changer le système de chargement de la conf pour avoir des valeurs par défaut
     if 'UPLOAD_FOLDER' in app.config:
         if app.config['UPLOAD_FOLDER'].startswith("static/"):
             app.config['UPLOAD_FOLDER'] = app.config['UPLOAD_FOLDER'][7:]
```

### Comparing `taxhub-1.9.3/apptax/log/logmanager.py` & `taxhub-1.9.4/apptax/log/logmanager.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/log/models.py` & `taxhub-1.9.4/apptax/log/models.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/data/taxonomie.sql` & `taxhub-1.9.4/apptax/migrations/data/taxonomie.sql`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/data/taxonomie_attributes_example.sql` & `taxhub-1.9.4/apptax/migrations/data/taxonomie_attributes_example.sql`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/data/taxonomie_bdc_statuts.sql` & `taxhub-1.9.4/apptax/migrations/data/taxonomie_bdc_statuts.sql`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/data/taxonomie_data.sql` & `taxhub-1.9.4/apptax/migrations/data/taxonomie_data.sql`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/data/taxonomie_materialized_views.sql` & `taxhub-1.9.4/apptax/migrations/data/taxonomie_materialized_views.sql`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/data/taxonomie_taxons_example.sql` & `taxhub-1.9.4/apptax/migrations/data/taxonomie_taxons_example.sql`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/env.py` & `taxhub-1.9.4/apptax/migrations/env.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/versions/3fe8c07741be_taxhub_admin.py` & `taxhub-1.9.4/apptax/migrations/versions/3fe8c07741be_taxhub_admin.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/versions/4fb7e197d241_fix_v_bdc_status_view.py` & `taxhub-1.9.4/apptax/migrations/versions/4fb7e197d241_fix_v_bdc_status_view.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/versions/7540702c6407_cd_ref_utility_functions.py` & `taxhub-1.9.4/apptax/migrations/versions/7540702c6407_cd_ref_utility_functions.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/versions/8222017dc3f6_add_taxons_exemple_to_taxonomie.py` & `taxhub-1.9.4/apptax/migrations/versions/8222017dc3f6_add_taxons_exemple_to_taxonomie.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/versions/98035939bc0d_find_all_taxons_parents.py` & `taxhub-1.9.4/apptax/migrations/versions/98035939bc0d_find_all_taxons_parents.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/versions/9c2c0254aadc_create_taxonomie_schema.py` & `taxhub-1.9.4/apptax/migrations/versions/9c2c0254aadc_create_taxonomie_schema.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/versions/aa7533601e41_add_attributes_exemple_to_taxonomie.py` & `taxhub-1.9.4/apptax/migrations/versions/aa7533601e41_add_attributes_exemple_to_taxonomie.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/versions/c93cbb35cfe4_set_default_value_for_id_liste.py` & `taxhub-1.9.4/apptax/migrations/versions/c93cbb35cfe4_set_default_value_for_id_liste.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/versions/f61f95136ec3_insert_inpn_data_in_taxonomie_schema.py` & `taxhub-1.9.4/apptax/migrations/versions/f61f95136ec3_insert_inpn_data_in_taxonomie_schema.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/migrations/versions/fa5a90853c45_taxhub.py` & `taxhub-1.9.4/apptax/migrations/versions/fa5a90853c45_taxhub.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/taxonomie/filemanager.py` & `taxhub-1.9.4/apptax/taxonomie/filemanager.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/taxonomie/models.py` & `taxhub-1.9.4/apptax/taxonomie/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,16 +215,17 @@
         return "<BibTypesMedia %r>" % self.nom_type_media
 
 
 @serializable
 class VMTaxrefListForautocomplete(db.Model):
     __tablename__ = "vm_taxref_list_forautocomplete"
     __table_args__ = {"schema": "taxonomie"}
-    cd_nom = db.Column(db.Integer, primary_key=True)
-    search_name = db.Column(db.Unicode, primary_key=True)
+    gid = db.Column(db.Integer, primary_key=True)
+    cd_nom = db.Column(db.Integer)
+    search_name = db.Column(db.Unicode)
     cd_ref = db.Column(db.Integer)
     nom_valide = db.Column(db.Unicode)
     lb_nom = db.Column(db.Unicode)
     nom_vern = db.Column(db.Unicode)
     regne = db.Column(db.Unicode)
     group2_inpn = db.Column(db.Unicode)
```

### Comparing `taxhub-1.9.3/apptax/taxonomie/repositories.py` & `taxhub-1.9.4/apptax/taxonomie/repositories.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/taxonomie/routesbdcstatuts.py` & `taxhub-1.9.4/apptax/taxonomie/routesbdcstatuts.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/taxonomie/routesbibattributs.py` & `taxhub-1.9.4/apptax/taxonomie/routesbibattributs.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/taxonomie/routesbiblistes.py` & `taxhub-1.9.4/apptax/taxonomie/routesbiblistes.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/taxonomie/routesbibnoms.py` & `taxhub-1.9.4/apptax/taxonomie/routesbibnoms.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/taxonomie/routesbibtypesmedia.py` & `taxhub-1.9.4/apptax/taxonomie/routesbibtypesmedia.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/taxonomie/routestaxref.py` & `taxhub-1.9.4/apptax/taxonomie/routestaxref.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from warnings import warn
+
 from flask import abort, jsonify, Blueprint, request
 from sqlalchemy import distinct, desc, func, and_
 from sqlalchemy.orm.exc import NoResultFound
 
 
 from ..utils.utilssqlalchemy import json_resp, serializeQuery, serializeQueryOneResult
-from ..utils.genericfunctions import calculate_offset_page
 from .models import (
     Taxref,
     BibNoms,
     VMTaxrefListForautocomplete,
     BibTaxrefHabitats,
     BibTaxrefRangs,
     BibTaxrefStatus,
@@ -249,16 +250,15 @@
         q = q.join(BibNoms, BibNoms.cd_nom == Taxref.cd_nom)
     else:
         q = q.outerjoin(BibNoms, BibNoms.cd_nom == Taxref.cd_nom)
 
     # Traitement des parametres
     limit = parameters.get("limit", 20, int)
     page = parameters.get("page", 1, int)
-    offset = parameters.get("offset", 0, int)
-    (limit, offset, page) = calculate_offset_page(limit, offset, page)
+
 
     for param in parameters:
         if param in taxrefColumns and parameters[param] != "":
             col = getattr(taxrefColumns, param)
             q = q.filter(col == parameters[param])
         elif param == "is_ref" and parameters[param] == "true":
             q = q.filter(Taxref.cd_nom == Taxref.cd_ref)
@@ -280,17 +280,17 @@
         else:
             orderCol = None
         if "order" in parameters:
             if parameters["order"] == "desc":
                 orderCol = orderCol.desc()
         q = q.order_by(orderCol)
 
-    results = q.limit(limit).offset(offset).all()
+    results = q.paginate(page=page, per_page=limit, error_out=False)
     return {
-        "items": [dict(d.Taxref.as_dict(), **{"id_nom": d.id_nom}) for d in results],
+        "items": [dict(d.Taxref.as_dict(), **{"id_nom": d.id_nom}) for d in results.items],
         "total": nbResultsWithoutFilter,
         "total_filtered": nbResults,
         "limit": limit,
         "page": page
     }
 
 
@@ -376,23 +376,22 @@
         # S'il y a une id_liste elle à forcement la valeur -1
         #   c-a-d pas de liste
         if not id_liste:
             q = (
                 db.session.query(BibListes.id_liste)
                 .filter(BibListes.code_liste == code_liste)
             ).one()
-            print('LAAAAAA')
             id_liste = q[0]
     except NoResultFound:
         return (
             {
                 "success": False,
                 "message": "Code liste '{}' inexistant".format(code_liste)
             },
-            500,
+            400,
         )
 
     q = db.session.query(VMTaxrefListForautocomplete)
     if id_liste and id_liste != -1:
         q = q.join(
             BibNoms, BibNoms.cd_nom == VMTaxrefListForautocomplete.cd_nom
         ).join(CorNomListe,
@@ -409,37 +408,42 @@
                     VMTaxrefListForautocomplete.search_name, search_name
                 ).label("idx_trgm")
         )
         search_name = search_name.replace(" ", "%")
         q = q.filter(
             func.unaccent(VMTaxrefListForautocomplete.search_name).ilike(func.unaccent("%" + search_name + "%"))
         ).order_by(desc("idx_trgm"))
+        q = q.order_by(
+            desc(VMTaxrefListForautocomplete.cd_nom == VMTaxrefListForautocomplete.cd_ref)
+        )
+    # if no search name no need to order by trigram or cd_nom=cdref - order by PK (use for mobile app)
+    else:
+        q = q.order_by(VMTaxrefListForautocomplete.gid)
 
     regne = request.args.get("regne")
     if regne:
         q = q.filter(VMTaxrefListForautocomplete.regne == regne)
 
     group2_inpn = request.args.get("group2_inpn")
     if group2_inpn:
         q = q.filter(VMTaxrefListForautocomplete.group2_inpn == group2_inpn)
 
-    q = q.order_by(
-        desc(VMTaxrefListForautocomplete.cd_nom == VMTaxrefListForautocomplete.cd_ref)
-    )
 
     limit = request.args.get("limit", 20, int)
     page = request.args.get("page", 1, int)
-    offset = request.args.get("offset", 0, int)
-    (limit, offset, page) = calculate_offset_page(limit, offset, page)
-    data = q.limit(limit).offset(offset).all()
+    if "offset" in request.args:
+        warn("offset is deprecated, please use page for pagination (start at 1)", DeprecationWarning)
+        page = (int(request.args["offset"]) / limit) + 1
+    data = q.paginate(page=page, per_page=limit, error_out=False)
 
     if search_name:
-        return [d[0].as_dict() for d in data]
+        return [d[0].as_dict() for d in data.items]
     else:
-        return [d.as_dict() for d in data]
+        return [d.as_dict() for d in data.items]
+
 
 
 @adresses.route("/bib_lr", methods=["GET"])
 @json_resp
 def get_bib_lr():
     data = db.session.query(BibTaxrefLR).all()
     formated_data = []
```

### Comparing `taxhub-1.9.3/apptax/taxonomie/routestmedias.py` & `taxhub-1.9.4/apptax/taxonomie/routestmedias.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/utils/genericfunctions.py` & `taxhub-1.9.4/apptax/utils/genericfunctions.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/utils/routesconfig.py` & `taxhub-1.9.4/apptax/utils/routesconfig.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/apptax/utils/utilssqlalchemy.py` & `taxhub-1.9.4/apptax/utils/utilssqlalchemy.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/setup.py` & `taxhub-1.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `taxhub-1.9.3/taxhub.egg-info/PKG-INFO` & `taxhub-1.9.4/taxhub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxhub
-Version: 1.9.3
+Version: 1.9.4
 Summary: Application web de gestion centralisée des taxons basée sur le référentiel TAXREF
 Home-page: https://github.com/PnX-SI/TaxHub
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
```

### Comparing `taxhub-1.9.3/taxhub.egg-info/SOURCES.txt` & `taxhub-1.9.4/taxhub.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 VERSION
 requirements.in
 setup.py
 apptax/__init__.py
 apptax/app.py
 apptax/database.py
 apptax/index.py
+apptax/test_config.py
 apptax/log/__init__.py
 apptax/log/logmanager.py
 apptax/log/models.py
 apptax/migrations/__init__.py
 apptax/migrations/env.py
 apptax/migrations/data/__init__.py
 apptax/migrations/data/taxonomie.sql
```

