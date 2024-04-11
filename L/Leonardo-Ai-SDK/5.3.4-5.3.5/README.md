# Comparing `tmp/Leonardo-Ai-SDK-5.3.4.tar.gz` & `tmp/Leonardo-Ai-SDK-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Leonardo-Ai-SDK-5.3.4.tar", last modified: Tue Apr  9 00:03:11 2024, max compression
+gzip compressed data, was "Leonardo-Ai-SDK-5.3.5.tar", last modified: Thu Apr 11 05:38:45 2024, max compression
```

## Comparing `Leonardo-Ai-SDK-5.3.4.tar` & `Leonardo-Ai-SDK-5.3.5.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:03:11.035760 Leonardo-Ai-SDK-5.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-09 00:03:11.035760 Leonardo-Ai-SDK-5.3.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     9808 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:03:11.035760 Leonardo-Ai-SDK-5.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:03:11.019760 Leonardo-Ai-SDK-5.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:03:11.023759 Leonardo-Ai-SDK-5.3.4/src/Leonardo_Ai_SDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-09 00:03:10.000000 Leonardo-Ai-SDK-5.3.4/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-09 00:03:10.000000 Leonardo-Ai-SDK-5.3.4/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:03:10.000000 Leonardo-Ai-SDK-5.3.4/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 00:03:10.000000 Leonardo-Ai-SDK-5.3.4/src/Leonardo_Ai_SDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 00:03:10.000000 Leonardo-Ai-SDK-5.3.4/src/Leonardo_Ai_SDK.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:03:11.023759 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:03:11.023759 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17316 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/element.py
--rw-r--r--   0 runner    (1001) docker     (127)    44786 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/initimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    27064 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:03:11.027760 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:03:11.027760 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:03:11.031760 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/creategeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createlcmgeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createtexturegeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createvariationnobg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createvariationunzoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createvariationupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/deletedatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/deletegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/deletemodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/get3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getdatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getgenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getuserself.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getvariationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/listelements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/listplatformmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/performinpaintinglcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/performinstantrefine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/promptimprove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/promptrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/uploaddatasetimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/uploadinitimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/uploadmodelasset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:03:11.035760 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/controlnet_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/custom_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/lcm_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/model_asset_texture_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/sd_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/sd_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/strength.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/variation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:03:11.035760 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13748 2024-04-09 00:02:56.000000 Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/variation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.545252 Leonardo-Ai-SDK-5.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-11 05:38:45.541252 Leonardo-Ai-SDK-5.3.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9808 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 05:38:45.545252 Leonardo-Ai-SDK-5.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.529252 Leonardo-Ai-SDK-5.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.533252 Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-11 05:38:45.000000 Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-11 05:38:45.000000 Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 05:38:45.000000 Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-11 05:38:45.000000 Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 05:38:45.000000 Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.533252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.533252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17316 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44786 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/initimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27064 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.533252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.533252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.541252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15019 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/creategeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createlcmgeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createtexturegeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createvariationnobg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createvariationunzoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createvariationupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletedatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletemodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/get3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getdatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14923 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getgenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getuserself.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getvariationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/listelements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/listplatformmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/performinpaintinglcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/performinstantrefine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/promptimprove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/promptrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploaddatasetimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploadinitimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploadmodelasset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.541252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/controlnet_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/custom_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/lcm_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/model_asset_texture_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/sd_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/sd_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/strength.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/variation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.541252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13748 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/variation.py
```

### Comparing `Leonardo-Ai-SDK-5.3.4/LICENSE.md` & `Leonardo-Ai-SDK-5.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/PKG-INFO` & `Leonardo-Ai-SDK-5.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.3.4
+Version: 5.3.5
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.4 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.5 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) req =
 operations.CreateDatasetRequestBody( name='', ) res = s.dataset.create_dataset
```

### Comparing `Leonardo-Ai-SDK-5.3.4/README.md` & `Leonardo-Ai-SDK-5.3.5/README.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/setup.py` & `Leonardo-Ai-SDK-5.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='Leonardo-Ai-SDK',
-    version='5.3.4',
+    version='5.3.5',
     author='Leonardo-Ai',
     description='Leonardo AI Python Client SDK',
     url='https://github.com/Leonardo-Interactive/leonardo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `Leonardo-Ai-SDK-5.3.4/src/Leonardo_Ai_SDK.egg-info/PKG-INFO` & `Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.3.4
+Version: 5.3.5
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.4 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.5 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) req =
 operations.CreateDatasetRequestBody( name='', ) res = s.dataset.create_dataset
```

### Comparing `Leonardo-Ai-SDK-5.3.4/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt` & `Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/_hooks/sdkhooks.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/_hooks/types.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/dataset.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/dataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/element.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/element.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/generation.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/generation.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/initimage.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/initimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/model.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/model.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/errors/sdkerror.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/__init__.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createdataset.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createdataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/creategeneration.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/creategeneration.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreateGenerationRequestBody:
     r"""Query parameters to be provided in the request body as a JSON object"""
     UNSET='__SPEAKEASY_UNSET__'
     alchemy: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('alchemy'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
-    r"""Enable to use Alchemy."""
+    r"""Enable to use Alchemy. Note: The appropriate Alchemy version is selected for the specified model. For example, XL models will use Alchemy V2."""
     contrast_ratio: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contrastRatio'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Contrast Ratio to use with Alchemy. Must be a float between 0 and 1 inclusive."""
     control_net: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('controlNet'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable to use ControlNet. Requires an init image to be provided. Requires a model based on SD v1.5"""
     control_net_type: Optional[shared_controlnet_type.ControlnetType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('controlNetType'), 'exclude': lambda f: f is None }})
     r"""The type of ControlNet to use."""
     elements: Optional[List[shared_element_input.ElementInput]] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('elements'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
@@ -53,28 +53,26 @@
     r"""The ID of an Init Image to use in image2image."""
     init_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('init_strength'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""How strongly the generated images should reflect the original image in image2image. Must be a float between 0.1 and 0.9."""
     model_id: Optional[str] = dataclasses.field(default='6bef9f1b-29cb-40c7-b9df-32b51c1f67d3', metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modelId'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The model ID used for image generation. If not provided, uses sd_version to determine the version of Stable Diffusion to use. In-app, model IDs are under the Finetune Models menu. Click on the platform model or your custom model, then click View More. For platform models, you can also use the List Platform Models API."""
     negative_prompt: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('negative_prompt'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The negative prompt used for the image generation"""
-    nsfw: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nsfw'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
-    r"""Not Safe For Work Flag."""
     num_images: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_images'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The number of images to generate. Must be between 1 and 8. If either width or height is over 768, must be between 1 and 4."""
     num_inference_steps: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_inference_steps'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The number of inference steps to use for the generation. Must be between 30 and 60."""
     photo_real: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoReal'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable the photoReal feature. Requires enabling alchemy and unspecifying modelId (for photoRealVersion V1)."""
     photo_real_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoRealStrength'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Depth of field of photoReal. Must be 0.55 for low, 0.5 for medium, or 0.45 for high. Defaults to 0.55 if not specified."""
     photo_real_version: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoRealVersion'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The version of photoReal to use. Must be v1 or v2."""
     preset_style: Optional[shared_sd_generation_style.SdGenerationStyle] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presetStyle'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
-    r"""The style to generate images with. When photoReal is enabled, use CINEMATIC, CREATIVE, VIBRANT, or NONE. When alchemy is disabled, use LEONARDO or NONE. When alchemy is enabled, use ANIME, CREATIVE, DYNAMIC, ENVIRONMENT, GENERAL, ILLUSTRATION, PHOTOGRAPHY, RAYTRACED, RENDER_3D, SKETCH_BW, SKETCH_COLOR, or NONE."""
+    r"""The style to generate images with. When photoReal is enabled, refer to the Guide section for a full list. When alchemy is disabled, use LEONARDO or NONE. When alchemy is enabled, use ANIME, CREATIVE, DYNAMIC, ENVIRONMENT, GENERAL, ILLUSTRATION, PHOTOGRAPHY, RAYTRACED, RENDER_3D, SKETCH_BW, SKETCH_COLOR, or NONE."""
     prompt: Optional[str] = dataclasses.field(default='An oil painting of a cat', metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prompt'), 'exclude': lambda f: f is None }})
     r"""The prompt used to generate images"""
     prompt_magic: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagic'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable to use Prompt Magic."""
     prompt_magic_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicStrength'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Strength of prompt magic. Must be a float between 0.1 and 1.0"""
     prompt_magic_version: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicVersion'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
```

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createlcmgeneration.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createlcmgeneration.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     height: Optional[int] = dataclasses.field(default=512, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is CreateLCMGenerationRequestBody.UNSET }})
     r"""The output width of the image. Must be 512, 640 or 1024."""
     request_timestamp: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('requestTimestamp'), 'exclude': lambda f: f is None }})
     seed: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seed'), 'exclude': lambda f: f is CreateLCMGenerationRequestBody.UNSET }})
     steps: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('steps'), 'exclude': lambda f: f is CreateLCMGenerationRequestBody.UNSET }})
     r"""The number of steps to use for the generation. Must be between 4 and 16."""
     strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('strength'), 'exclude': lambda f: f is CreateLCMGenerationRequestBody.UNSET }})
-    r"""How strongly the generated images should reflect the original image supplied in imageDataUrl. Must be a float between 0.1 and 1."""
+    r"""Creativity strength of generation. Higher strength will deviate more from the original image supplied in imageDataUrl. Must be a float between 0.1 and 1."""
     style: Optional[shared_lcm_generation_style.LcmGenerationStyle] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('style'), 'exclude': lambda f: f is CreateLCMGenerationRequestBody.UNSET }})
     r"""The style to generate LCM images with."""
     width: Optional[int] = dataclasses.field(default=512, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is CreateLCMGenerationRequestBody.UNSET }})
     r"""The output width of the image. Must be 512, 640 or 1024."""
```

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createmodel.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createmodel.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createtexturegeneration.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createtexturegeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createvariationnobg.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createvariationnobg.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createvariationunzoom.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createvariationunzoom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/createvariationupscale.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createvariationupscale.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/delete3dmodelbyid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/delete3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/deletedatasetbyid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletedatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/deletegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/deleteinitimagebyid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deleteinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/deletemodelbyid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletemodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/get3dmodelbyid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/get3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getdatasetbyid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getdatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getgenerationbyid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getgenerationbyid.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     model_id: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modelId'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     negative_prompt: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('negativePrompt'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     photo_real: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoReal'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     r"""If photoReal feature was used."""
     photo_real_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoRealStrength'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     r"""Depth of field of photoReal used. 0.55 is low, 0.5 is medium, and 0.45 is high. Default is 0.55."""
     preset_style: Optional[shared_sd_generation_style.SdGenerationStyle] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presetStyle'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
-    r"""The style to generate images with. When photoReal is enabled, use CINEMATIC, CREATIVE, VIBRANT, or NONE. When alchemy is disabled, use LEONARDO or NONE. When alchemy is enabled, use ANIME, CREATIVE, DYNAMIC, ENVIRONMENT, GENERAL, ILLUSTRATION, PHOTOGRAPHY, RAYTRACED, RENDER_3D, SKETCH_BW, SKETCH_COLOR, or NONE."""
+    r"""The style to generate images with. When photoReal is enabled, refer to the Guide section for a full list. When alchemy is disabled, use LEONARDO or NONE. When alchemy is enabled, use ANIME, CREATIVE, DYNAMIC, ENVIRONMENT, GENERAL, ILLUSTRATION, PHOTOGRAPHY, RAYTRACED, RENDER_3D, SKETCH_BW, SKETCH_COLOR, or NONE."""
     prompt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prompt'), 'exclude': lambda f: f is None }})
     prompt_magic: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagic'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     r"""If prompt magic was used."""
     prompt_magic_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicStrength'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     r"""Strength of prompt magic used."""
     prompt_magic_version: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicVersion'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     r"""Version of prompt magic used."""
```

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     model_id: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modelId'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     negative_prompt: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('negativePrompt'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     photo_real: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoReal'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     r"""If photoReal feature was used."""
     photo_real_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoRealStrength'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     r"""Depth of field of photoReal used. 0.55 is low, 0.5 is medium, and 0.45 is high. Default is 0.55."""
     preset_style: Optional[shared_sd_generation_style.SdGenerationStyle] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presetStyle'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
-    r"""The style to generate images with. When photoReal is enabled, use CINEMATIC, CREATIVE, VIBRANT, or NONE. When alchemy is disabled, use LEONARDO or NONE. When alchemy is enabled, use ANIME, CREATIVE, DYNAMIC, ENVIRONMENT, GENERAL, ILLUSTRATION, PHOTOGRAPHY, RAYTRACED, RENDER_3D, SKETCH_BW, SKETCH_COLOR, or NONE."""
+    r"""The style to generate images with. When photoReal is enabled, refer to the Guide section for a full list. When alchemy is disabled, use LEONARDO or NONE. When alchemy is enabled, use ANIME, CREATIVE, DYNAMIC, ENVIRONMENT, GENERAL, ILLUSTRATION, PHOTOGRAPHY, RAYTRACED, RENDER_3D, SKETCH_BW, SKETCH_COLOR, or NONE."""
     prompt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prompt'), 'exclude': lambda f: f is None }})
     prompt_magic: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagic'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     r"""If prompt magic was used."""
     prompt_magic_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicStrength'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     r"""Strength of prompt magic used."""
     prompt_magic_version: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicVersion'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     r"""Version of prompt magic used."""
```

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getinitimagebyid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getmodelbyid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getuserself.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getuserself.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/getvariationbyid.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getvariationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/listelements.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/listelements.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/listplatformmodels.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/listplatformmodels.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     refine_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refineStrength'), 'exclude': lambda f: f is PerformAlchemyUpscaleLCMRequestBody.UNSET }})
     r"""Must be a float between 0.5 and 0.9."""
     request_timestamp: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('requestTimestamp'), 'exclude': lambda f: f is None }})
     seed: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seed'), 'exclude': lambda f: f is PerformAlchemyUpscaleLCMRequestBody.UNSET }})
     steps: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('steps'), 'exclude': lambda f: f is PerformAlchemyUpscaleLCMRequestBody.UNSET }})
     r"""The number of steps to use for the generation. Must be between 4 and 16."""
     strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('strength'), 'exclude': lambda f: f is PerformAlchemyUpscaleLCMRequestBody.UNSET }})
-    r"""How strongly the generated images should reflect the original image supplied in imageDataUrl. Must be a float between 0.1 and 1."""
+    r"""Creativity strength of generation. Higher strength will deviate more from the original image supplied in imageDataUrl. Must be a float between 0.1 and 1."""
     style: Optional[shared_lcm_generation_style.LcmGenerationStyle] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('style'), 'exclude': lambda f: f is PerformAlchemyUpscaleLCMRequestBody.UNSET }})
     r"""The style to generate LCM images with."""
     width: Optional[int] = dataclasses.field(default=512, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is PerformAlchemyUpscaleLCMRequestBody.UNSET }})
     r"""The output width of the image. Must be 512, 640 or 1024."""
```

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/performinpaintinglcm.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/performinpaintinglcm.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     height: Optional[int] = dataclasses.field(default=512, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is PerformInpaintingLCMRequestBody.UNSET }})
     r"""The output width of the image. Must be 512, 640 or 1024."""
     request_timestamp: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('requestTimestamp'), 'exclude': lambda f: f is None }})
     seed: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seed'), 'exclude': lambda f: f is PerformInpaintingLCMRequestBody.UNSET }})
     steps: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('steps'), 'exclude': lambda f: f is PerformInpaintingLCMRequestBody.UNSET }})
     r"""The number of steps to use for the generation. Must be between 4 and 16."""
     strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('strength'), 'exclude': lambda f: f is PerformInpaintingLCMRequestBody.UNSET }})
-    r"""How strongly the generated images should reflect the original image supplied in imageDataUrl. Must be a float between 0.1 and 1."""
+    r"""Creativity strength of generation. Higher strength will deviate more from the original image supplied in imageDataUrl. Must be a float between 0.1 and 1."""
     style: Optional[shared_lcm_generation_style.LcmGenerationStyle] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('style'), 'exclude': lambda f: f is PerformInpaintingLCMRequestBody.UNSET }})
     r"""The style to generate LCM images with."""
     width: Optional[int] = dataclasses.field(default=512, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is PerformInpaintingLCMRequestBody.UNSET }})
     r"""The output width of the image. Must be 512, 640 or 1024."""
```

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/performinstantrefine.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/performinstantrefine.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     height: Optional[int] = dataclasses.field(default=512, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is PerformInstantRefineRequestBody.UNSET }})
     r"""The output width of the image. Must be 512, 640 or 1024."""
     request_timestamp: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('requestTimestamp'), 'exclude': lambda f: f is None }})
     seed: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seed'), 'exclude': lambda f: f is PerformInstantRefineRequestBody.UNSET }})
     steps: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('steps'), 'exclude': lambda f: f is PerformInstantRefineRequestBody.UNSET }})
     r"""The number of steps to use for the generation. Must be between 4 and 16."""
     strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('strength'), 'exclude': lambda f: f is PerformInstantRefineRequestBody.UNSET }})
-    r"""How strongly the generated images should reflect the original image supplied in imageDataUrl. Must be a float between 0.1 and 1."""
+    r"""Creativity strength of generation. Higher strength will deviate more from the original image supplied in imageDataUrl. Must be a float between 0.1 and 1."""
     style: Optional[shared_lcm_generation_style.LcmGenerationStyle] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('style'), 'exclude': lambda f: f is PerformInstantRefineRequestBody.UNSET }})
     r"""The style to generate LCM images with."""
     width: Optional[int] = dataclasses.field(default=512, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is PerformInstantRefineRequestBody.UNSET }})
     r"""The output width of the image. Must be 512, 640 or 1024."""
```

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/promptimprove.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/promptimprove.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/promptrandom.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/promptrandom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/uploaddatasetimage.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploaddatasetimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/uploadinitimage.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploadinitimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/operations/uploadmodelasset.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploadmodelasset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/__init__.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/custom_model_type.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/custom_model_type.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/element_input.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/element_input.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/lcm_generation_style.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/lcm_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/sd_generation_style.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/sd_generation_style.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,38 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
 class SdGenerationStyle(str, Enum):
-    r"""The style to generate images with. When photoReal is enabled, use CINEMATIC, CREATIVE, VIBRANT, or NONE. When alchemy is disabled, use LEONARDO or NONE. When alchemy is enabled, use ANIME, CREATIVE, DYNAMIC, ENVIRONMENT, GENERAL, ILLUSTRATION, PHOTOGRAPHY, RAYTRACED, RENDER_3D, SKETCH_BW, SKETCH_COLOR, or NONE."""
+    r"""The style to generate images with. When photoReal is enabled, refer to the Guide section for a full list. When alchemy is disabled, use LEONARDO or NONE. When alchemy is enabled, use ANIME, CREATIVE, DYNAMIC, ENVIRONMENT, GENERAL, ILLUSTRATION, PHOTOGRAPHY, RAYTRACED, RENDER_3D, SKETCH_BW, SKETCH_COLOR, or NONE."""
     ANIME = 'ANIME'
+    BOKEH = 'BOKEH'
     CINEMATIC = 'CINEMATIC'
+    CINEMATIC_CLOSEUP = 'CINEMATIC_CLOSEUP'
     CREATIVE = 'CREATIVE'
     DYNAMIC = 'DYNAMIC'
     ENVIRONMENT = 'ENVIRONMENT'
+    FASHION = 'FASHION'
+    FILM = 'FILM'
+    FOOD = 'FOOD'
     GENERAL = 'GENERAL'
+    HDR = 'HDR'
     ILLUSTRATION = 'ILLUSTRATION'
     LEONARDO = 'LEONARDO'
+    LONG_EXPOSURE = 'LONG_EXPOSURE'
+    MACRO = 'MACRO'
+    MINIMALISTIC = 'MINIMALISTIC'
+    MONOCHROME = 'MONOCHROME'
+    MOODY = 'MOODY'
     NONE = 'NONE'
+    NEUTRAL = 'NEUTRAL'
     PHOTOGRAPHY = 'PHOTOGRAPHY'
+    PORTRAIT = 'PORTRAIT'
     RAYTRACED = 'RAYTRACED'
     RENDER_3_D = 'RENDER_3D'
+    RETRO = 'RETRO'
     SKETCH_BW = 'SKETCH_BW'
     SKETCH_COLOR = 'SKETCH_COLOR'
+    STOCK_PHOTO = 'STOCK_PHOTO'
     VIBRANT = 'VIBRANT'
+    UNPROCESSED = 'UNPROCESSED'
```

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/models/shared/sd_versions.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/sd_versions.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/prompt.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/prompt.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/sdk.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/sdk.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/sdkconfiguration.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/sdkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = 'v1.0.0'
-    sdk_version: str = '5.3.4'
-    gen_version: str = '2.301.0'
-    user_agent: str = 'speakeasy-sdk/python 5.3.4 2.301.0 v1.0.0 Leonardo-Ai-SDK'
+    sdk_version: str = '5.3.5'
+    gen_version: str = '2.302.1'
+    user_agent: str = 'speakeasy-sdk/python 5.3.5 2.302.1 v1.0.0 Leonardo-Ai-SDK'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/user.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/user.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/utils/retries.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/utils/utils.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.4/src/leonardoaisdk/variation.py` & `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/variation.py`

 * *Files identical despite different names*

