# Comparing `tmp/duplocloud-client-0.2.8.tar.gz` & `tmp/duplocloud-client-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duplocloud-client-0.2.8.tar", last modified: Fri Mar  8 23:23:43 2024, max compression
+gzip compressed data, was "duplocloud-client-0.2.9.tar", last modified: Wed Mar 13 17:17:31 2024, max compression
```

## Comparing `duplocloud-client-0.2.8.tar` & `duplocloud-client-0.2.9.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:23:43.209935 duplocloud-client-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:23:43.201935 duplocloud-client-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:23:43.205935 duplocloud-client-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/.github/workflows/image.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/.github/workflows/installer.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/.github/workflows/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-08 23:23:43.209935 duplocloud-client-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/docker-compose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/installer.spec
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 23:23:43.209935 duplocloud-client-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:23:43.201935 duplocloud-client-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:23:43.205935 duplocloud-client-0.2.8/src/duplo_resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/asg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/configmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/cronjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/ecs_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/ingress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/jit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplo_resource/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:23:43.209935 duplocloud-client-0.2.8/src/duplocloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplocloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplocloud/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplocloud/argtype.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplocloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplocloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplocloud/commander.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplocloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplocloud/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplocloud/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/duplocloud/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:23:43.209935 duplocloud-client-0.2.8/src/duplocloud_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-08 23:23:43.000000 duplocloud-client-0.2.8/src/duplocloud_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-08 23:23:43.000000 duplocloud-client-0.2.8/src/duplocloud_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 23:23:43.000000 duplocloud-client-0.2.8/src/duplocloud_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-08 23:23:43.000000 duplocloud-client-0.2.8/src/duplocloud_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-08 23:23:43.000000 duplocloud-client-0.2.8/src/duplocloud_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-08 23:23:43.000000 duplocloud-client-0.2.8/src/duplocloud_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:23:43.209935 duplocloud-client-0.2.8/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-03-08 23:23:08.000000 duplocloud-client-0.2.8/src/tests/test_commander.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:17:31.913120 duplocloud-client-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:17:31.901120 duplocloud-client-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:17:31.905120 duplocloud-client-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/.github/workflows/image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/.github/workflows/installer.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-13 17:17:31.913120 duplocloud-client-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/installer.spec
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 17:17:31.913120 duplocloud-client-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:17:31.901120 duplocloud-client-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:17:31.909119 duplocloud-client-0.2.9/src/duplo_resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/asg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/configmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/ecs_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/ingress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplo_resource/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:17:31.909119 duplocloud-client-0.2.9/src/duplocloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplocloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplocloud/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplocloud/argtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplocloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplocloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplocloud/commander.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplocloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplocloud/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplocloud/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/duplocloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:17:31.909119 duplocloud-client-0.2.9/src/duplocloud_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-13 17:17:31.000000 duplocloud-client-0.2.9/src/duplocloud_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-13 17:17:31.000000 duplocloud-client-0.2.9/src/duplocloud_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 17:17:31.000000 duplocloud-client-0.2.9/src/duplocloud_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-13 17:17:31.000000 duplocloud-client-0.2.9/src/duplocloud_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-13 17:17:31.000000 duplocloud-client-0.2.9/src/duplocloud_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-13 17:17:31.000000 duplocloud-client-0.2.9/src/duplocloud_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:17:31.909119 duplocloud-client-0.2.9/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-03-13 17:16:53.000000 duplocloud-client-0.2.9/src/tests/test_commander.py
```

### Comparing `duplocloud-client-0.2.8/.github/workflows/image.yml` & `duplocloud-client-0.2.9/.github/workflows/image.yml`

 * *Files 17% similar despite different names*

```diff
@@ -4,21 +4,29 @@
   workflow_dispatch: 
     inputs:
       push:
         description: Push the image to the registry
         required: true
         default: false
         type: boolean
+      tag:
+        description: The git tag to build on
+        required: true
+        type: string
   workflow_call: 
     inputs:
       push:
         description: Push the image to the registry
         required: false
         default: true
         type: boolean
+      tag:
+        description: The git tag to build on
+        required: true
+        type: string
     outputs:
       image:
         description: The URI of the image
         value: ${{ jobs.build_image.outputs.image }}
     secrets:
       DOCKER_USERNAME:
         description: Docker username
@@ -34,20 +42,22 @@
     runs-on: ubuntu-latest
     outputs:
       image: ${{ steps.build_image.outputs.uri }}
     steps:
 
     - name: Checkout code
       uses: actions/checkout@v4
+      with:
+        ref: ${{ inputs.tag }}
 
     - name: Build and Push Docker Image
       id: build_image
       uses: duplocloud/actions/build-image@main
       with:
-        platforms: linux/amd64 # ,linux/arm64 # makes it take longer
+        platforms: linux/amd64,linux/arm64 # makes it take longer
         push: ${{ inputs.push }}
         docker-username: ${{ secrets.DOCKER_USERNAME }}
         docker-password: ${{ secrets.DOCKER_PASSWORD }}
         build-args: >
           PY_VERSION=3.11
 
     - name: Docker Hub Description
```

### Comparing `duplocloud-client-0.2.8/.github/workflows/package.yml` & `duplocloud-client-0.2.9/.github/workflows/package.yml`

 * *Files 14% similar despite different names*

```diff
@@ -3,34 +3,44 @@
 on:
   workflow_dispatch: 
     inputs:
       push:
         description: Push the image to the registry
         default: false
         type: boolean
+      tag:
+        description: Tag to push
+        required: true
+        type: string
   workflow_call: 
     inputs:
       push:
         description: Push the image to the registry
         default: true
         type: boolean
+      tag:
+        description: Tag to push
+        required: true
+        type: string
     secrets:
       PYPI_API_TOKEN:
         description: PyPi token
         required: true
 
 jobs:
   package:
     name: Package
     runs-on: ubuntu-latest
     steps:
 
     # checkout code 
     - name: Checkout Code
       uses: actions/checkout@v4
+      with:
+        ref: ${{ inputs.tag }}
     
     # install python
     - name: Set up Python 3.11
       uses: actions/setup-python@v5
       with:
         python-version: "3.11"
         cache: pip
```

### Comparing `duplocloud-client-0.2.8/.github/workflows/release.yml` & `duplocloud-client-0.2.9/.github/workflows/release.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,50 @@
 name: Releaser
 
 on:
-  workflow_call:
   workflow_dispatch:
+    inputs:
+      push:
+        description: Should this push a new release? 
+        required: false
+        default: false
+        type: boolean
+      tag:
+        description: Tag to release
+        required: false
+        type: string
+  workflow_call:
+    inputs:
+      push:
+        description: Should this push a new release? 
+        required: false
+        default: false
+        type: boolean
+      tag:
+        description: Tag to release
+        required: false
+        type: string
 
 jobs:
   releaser:
     runs-on: ubuntu-latest
     steps:
 
     - name: Dist Dir
       id: dist_dir
       run: mkdir -p dist artifacts
 
     - name: Get Tag Name
       id: set_tag
+      env:
+        GIT_TAG: ${{ inputs.tag }}
       run: |
-        GIT_TAG=${GITHUB_REF#refs/*/}
+        if [ -z "$GIT_TAG" ]; then
+          GIT_TAG=${GITHUB_REF#refs/*/}
+        fi
         VERSION=$(echo $GIT_TAG | cut -d'v' -f2)
         NAME="duploctl-${GIT_TAG}"
         echo "GIT_TAG=${GIT_TAG}" >> $GITHUB_OUTPUT
         echo "VERSION=${VERSION}" >> $GITHUB_OUTPUT
         echo "NAME=${NAME}" >> $GITHUB_OUTPUT
     
     - name: Download Artifacts
@@ -33,21 +57,26 @@
     - name: Compress Artifacts
       shell: bash
       run: |
         for d in artifacts/*; do
           name=$(basename $d)
           dest="dist/${name}.tar.gz"
           tar -czvf "$dest" -C $d .
+          shasum -a 256 $dest >> dist/checksums.txt
         done
+        echo "Created Release Artifacts"
+        ls -l dist
 
     - name: Create Release
       id: release
       uses: softprops/action-gh-release@v1
-      if: startsWith(github.ref, 'refs/tags/')
+      if: inputs.push == true
       with:
+        name: ${{ steps.set_tag.outputs.GIT_TAG }}
+        tag_name: ${{ steps.set_tag.outputs.GIT_TAG }}
         files: |
           dist/*
         body: |
           duploctl ${{ steps.set_tag.outputs.GIT_TAG }} is out!. 
 
           PyPi: 
           [duplocloud-client](https://pypi.org/project/duplocloud-client/${{ steps.set_tag.outputs.VERSION }}/)
@@ -55,23 +84,23 @@
           pip install duplocloud-client==${{ steps.set_tag.outputs.VERSION }}
           ```
 
           Dockerhub:  
           [duplocloud/duploctl:${{ steps.set_tag.outputs.GIT_TAG }}](https://hub.docker.com/r/duplocloud/duploctl)
           ```sh
           docker pull duplocloud/duploctl:${{ steps.set_tag.outputs.GIT_TAG }}
-
-          Build: ${{ github.server_url }}/${{ github.repository }}/actions/runs/${{ github.run_id }}
-          
           ```
+          
+          Build: ${{ github.server_url }}/${{ github.repository }}/actions/runs/${{ github.run_id }}
         prerelease: false
 
     - name: Post to a Slack channel
       id: slack
       uses: slackapi/slack-github-action@v1.25.0
+      if: inputs.push == true
       env:
         SLACK_BOT_TOKEN: ${{ secrets.SLACK_BOT_TOKEN }}
       with:
         channel-id: ${{ vars.SLACK_CHANNEL_ID }}
         slack-message: |
           duploctl ${{ steps.set_tag.outputs.GIT_TAG }} is out! 
           ${{ steps.release.outputs.url }}
```

### Comparing `duplocloud-client-0.2.8/.github/workflows/test.yml` & `duplocloud-client-0.2.9/.github/workflows/test.yml`

 * *Files 9% similar despite different names*

```diff
@@ -2,36 +2,33 @@
 
 on:
   workflow_dispatch: {}
   workflow_call: {}
   pull_request:
     branches:
       - main
-  push: 
-    paths:
-      - 'src/**'
 
 jobs:
   test:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
         # was unable to biuld with: 3.7, 3.8, or 3.9
         python-version: ["3.10", "3.11", "3.12"]
 
     steps:
 
     # checkout code 
     - name: Checkout Code
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
     
     # install python
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         cache: 'pip'
     
     # install the project
     - name: Install dependencies
       run: |
```

### Comparing `duplocloud-client-0.2.8/CONTRIBUTING.md` & `duplocloud-client-0.2.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/Dockerfile` & `duplocloud-client-0.2.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/PKG-INFO` & `duplocloud-client-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplocloud-client
-Version: 0.2.8
+Version: 0.2.9
 Summary: Generic DuploClient for Python apps.
 Author-email: Kelly <kelly@duplocloud.net>
 Maintainer-email: Kelly <kelly@duplocloud.net>, Mick <mick@duplocloud.net>
 Keywords: duplocloud,duplo,duploctl,duplo-client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `duplocloud-client-0.2.8/README.md` & `duplocloud-client-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/pyproject.toml` & `duplocloud-client-0.2.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
 [project.entry-points."duplocloud.net"]
 infrastructure = "duplo_resource.infrastructure:DuploInfrastructure"
 tenant = "duplo_resource.tenant:DuploTenant"
 version = "duplo_resource.version:DuploVersion"
 service = "duplo_resource.service:DuploService"
 cronjob = "duplo_resource.cronjob:DuploCronJob"
+job = "duplo_resource.job:DuploJob"
 user = "duplo_resource.user:DuploUser"
 lambda = "duplo_resource.lambda:DuploLambda"
 jit = "duplo_resource.jit:DuploJit"
 system = "duplo_resource.system:DuploSystem"
 asg = "duplo_resource.asg:DuploAsg"
 secret = "duplo_resource.secret:DuploSecret"
 configmap = "duplo_resource.configmap:DuploConfigMap"
```

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/asg.py` & `duplocloud-client-0.2.9/src/duplo_resource/asg.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/configmap.py` & `duplocloud-client-0.2.9/src/duplo_resource/configmap.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/cronjob.py` & `duplocloud-client-0.2.9/src/duplo_resource/cronjob.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/ecs_service.py` & `duplocloud-client-0.2.9/src/duplo_resource/ecs_service.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/hosts.py` & `duplocloud-client-0.2.9/src/duplo_resource/hosts.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/infrastructure.py` & `duplocloud-client-0.2.9/src/duplo_resource/infrastructure.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/ingress.py` & `duplocloud-client-0.2.9/src/duplo_resource/ingress.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/jit.py` & `duplocloud-client-0.2.9/src/duplo_resource/jit.py`

 * *Files 13% similar despite different names*

```diff
@@ -116,39 +116,45 @@
     sts = self.aws(nocache=True)
     wb.open(sts["ConsoleUrl"], new=0, autoraise=True)
     return {
       "message": "Opening AWS console in browser"
     }
   
   def __k8s_exec_credential(self, creds):
+    cluster = {
+      "server": creds["ApiServer"],
+      "config": None
+    }
+    if creds["K8Provider"] == 0 and (ca := creds.get("CertificateAuthorityDataBase64", None)):
+      cluster["certificate-authority-data"] = ca
     return {
       "kind": "ExecCredential",
       "apiVersion": "client.authentication.k8s.io/v1beta1",
       "spec": {
-        "cluster": {
-          "server": creds["ApiServer"],
-          "certificate-authority-data": creds["CertificateAuthorityDataBase64"],
-          "config": None
-        },
+        "cluster": cluster,
         "interactive": False
       },
       "status": {
         "token": creds["Token"],
         "expirationTimestamp": self.duplo.expiration()
       }
     }
   
   def __cluster_config(self, config):
     """Build a kubeconfig cluster object"""
+    cluster = {
+      "server": config["ApiServer"]
+    }
+    if config["K8Provider"] == 0 and (ca := config.get("CertificateAuthorityDataBase64", None)):
+      cluster["certificate-authority-data"] = ca
+    elif config["K8Provider"] == 1:
+      cluster["insecure-skip-tls-verify"] = True
     return {
       "name": config["Name"],
-      "cluster": {
-        "server": config["ApiServer"],
-        "certificate-authority-data": config["CertificateAuthorityDataBase64"]
-      }
+      "cluster": cluster
     }
   
   def __user_config(self, config):
     """Build a kubeconfig user object"""
     cmd = self.duplo.build_command("jit", "k8s", "--plan", config["Name"])
     return {
       "name": config["Name"],
```

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/lambda.py` & `duplocloud-client-0.2.9/src/duplo_resource/lambda.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,20 +36,20 @@
     try:
       return [s for s in self.list() if s["FunctionName"] == name][0]
     except IndexError:
       raise DuploError(f"Lambda '{name}' not found", 404)
     
   @Command()
   def create(self, 
-             lambda_fx: args.BODY):
+             body: args.BODY):
     """Create a new tenant."""
     tenant_id = self.tenant["TenantId"]
-    self.duplo.post(f"subscriptions/{tenant_id}/CreateLambdaFunction", lambda_fx)
+    self.duplo.post(f"subscriptions/{tenant_id}/CreateLambdaFunction", body)
     return {
-      "message": f"Lambda {lambda_fx['FunctionName']} created"
+      "message": f"Lambda {body['FunctionName']} created"
     }
 
   @Command()
   def update_image(self, 
                    name: args.NAME, 
                    image: args.IMAGE):
     """Update the image of a lambda.
```

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/secret.py` & `duplocloud-client-0.2.9/src/duplo_resource/secret.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/service.py` & `duplocloud-client-0.2.9/src/duplo_resource/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,21 @@
 
     Args:
         name (str): The name of the service to update.
         replica (str): Number of replicas to set for service.
     """
     try:
       tenant_id = self.tenant["TenantId"]
+      service = self.find(name)
       data = {
+        "Name": name,
         "Replicas": replica,
-        "Name": name
+        "AllocationTags": service["Template"].get("AllocationTags", "")
       }
-      response = self.duplo.post(f"subscriptions/{tenant_id}/ReplicationControllerChangeAll", data)
+      response = self.duplo.post(f"subscriptions/{tenant_id}/ReplicationControllerChange", data)
       if response.json() is None:
         return {"message": f"Successfully updated replicas for service '{name}'"} 
     except IndexError:
       raise DuploError(f"Service '{name}' not found to set replica count.", 404)
   
   @Command()
   def update_image(self,
```

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/system.py` & `duplocloud-client-0.2.9/src/duplo_resource/system.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/tenant.py` & `duplocloud-client-0.2.9/src/duplo_resource/tenant.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     try:
       return [t for t in self.list() if t["AccountName"] == name][0]
     except IndexError:
       raise DuploError(f"Tenant '{name}' not found", 404)
   
   @Command()
   def create(self, 
-             tenant: args.BODY):
+             body: args.BODY):
     """Create a new tenant."""
-    self.duplo.post("admin/AddTenant", tenant)
+    self.duplo.post("admin/AddTenant", body)
     return {
-      "message": f"Tenant '{tenant['AccountName']}' created"
+      "message": f"Tenant '{body['AccountName']}' created"
     }
     
   @Command()
   def shutdown(self, 
                name: args.NAME, 
                schedule: args.SCHEDULE=None):
     """Expire a tenant."""
```

### Comparing `duplocloud-client-0.2.8/src/duplo_resource/user.py` & `duplocloud-client-0.2.9/src/duplo_resource/user.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplocloud/args.py` & `duplocloud-client-0.2.9/src/duplocloud/args.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplocloud/argtype.py` & `duplocloud-client-0.2.9/src/duplocloud/argtype.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplocloud/client.py` & `duplocloud-client-0.2.9/src/duplocloud/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,15 @@
 
     Args:
       name: The name to get the cache key for.
 
     Returns:
       The cache key as a string.
     """
-    h = self.host.split("://")[1]
+    h = self.host.split("://")[1].replace("/", "")
     parts = [h]
     if self.isadmin:
       parts.append("admin")
     parts.append(name)
     return ",".join(parts)
   
   def expiration(self, hours: int = 6):
```

### Comparing `duplocloud-client-0.2.8/src/duplocloud/commander.py` & `duplocloud-client-0.2.9/src/duplocloud/commander.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplocloud/formats.py` & `duplocloud-client-0.2.9/src/duplocloud/formats.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplocloud/resource.py` & `duplocloud-client-0.2.9/src/duplocloud/resource.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplocloud/server.py` & `duplocloud-client-0.2.9/src/duplocloud/server.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/duplocloud_client.egg-info/PKG-INFO` & `duplocloud-client-0.2.9/src/duplocloud_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplocloud-client
-Version: 0.2.8
+Version: 0.2.9
 Summary: Generic DuploClient for Python apps.
 Author-email: Kelly <kelly@duplocloud.net>
 Maintainer-email: Kelly <kelly@duplocloud.net>, Mick <mick@duplocloud.net>
 Keywords: duplocloud,duplo,duploctl,duplo-client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `duplocloud-client-0.2.8/src/duplocloud_client.egg-info/SOURCES.txt` & `duplocloud-client-0.2.9/src/duplocloud_client.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/duplo_resource/configmap.py
 src/duplo_resource/cronjob.py
 src/duplo_resource/ecs_service.py
 src/duplo_resource/hosts.py
 src/duplo_resource/infrastructure.py
 src/duplo_resource/ingress.py
 src/duplo_resource/jit.py
+src/duplo_resource/job.py
 src/duplo_resource/lambda.py
 src/duplo_resource/secret.py
 src/duplo_resource/service.py
 src/duplo_resource/system.py
 src/duplo_resource/tenant.py
 src/duplo_resource/user.py
 src/duplo_resource/version.py
```

### Comparing `duplocloud-client-0.2.8/src/duplocloud_client.egg-info/entry_points.txt` & `duplocloud-client-0.2.9/src/duplocloud_client.egg-info/entry_points.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 configmap = duplo_resource.configmap:DuploConfigMap
 cronjob = duplo_resource.cronjob:DuploCronJob
 ecs = duplo_resource.ecs_service:DuploEcsService
 hosts = duplo_resource.hosts:DuploHosts
 infrastructure = duplo_resource.infrastructure:DuploInfrastructure
 ingress = duplo_resource.ingress:DuploIngress
 jit = duplo_resource.jit:DuploJit
+job = duplo_resource.job:DuploJob
 lambda = duplo_resource.lambda:DuploLambda
 secret = duplo_resource.secret:DuploSecret
 service = duplo_resource.service:DuploService
 system = duplo_resource.system:DuploSystem
 tenant = duplo_resource.tenant:DuploTenant
 user = duplo_resource.user:DuploUser
 version = duplo_resource.version:DuploVersion
```

### Comparing `duplocloud-client-0.2.8/src/tests/test_client.py` & `duplocloud-client-0.2.9/src/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.2.8/src/tests/test_commander.py` & `duplocloud-client-0.2.9/src/tests/test_commander.py`

 * *Files identical despite different names*

