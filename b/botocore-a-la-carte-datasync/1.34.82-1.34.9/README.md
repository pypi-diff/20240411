# Comparing `tmp/botocore-a-la-carte-datasync-1.34.82.tar.gz` & `tmp/botocore-a-la-carte-datasync-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-datasync-1.34.82.tar", last modified: Thu Apr 11 01:00:48 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-datasync-1.34.9.tar", last modified: Thu Dec 28 01:06:41 2023, max compression
```

## Comparing `botocore-a-la-carte-datasync-1.34.82.tar` & `botocore-a-la-carte-datasync-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:48.584771 botocore-a-la-carte-datasync-1.34.82/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-11 01:00:48.000000 botocore-a-la-carte-datasync-1.34.82/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-11 01:00:48.584771 botocore-a-la-carte-datasync-1.34.82/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:48.584771 botocore-a-la-carte-datasync-1.34.82/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:48.584771 botocore-a-la-carte-datasync-1.34.82/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:48.584771 botocore-a-la-carte-datasync-1.34.82/botocore/data/datasync/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:48.584771 botocore-a-la-carte-datasync-1.34.82/botocore/data/datasync/2018-11-09/
--rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-04-11 01:00:33.000000 botocore-a-la-carte-datasync-1.34.82/botocore/data/datasync/2018-11-09/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 01:00:33.000000 botocore-a-la-carte-datasync-1.34.82/botocore/data/datasync/2018-11-09/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-11 01:00:33.000000 botocore-a-la-carte-datasync-1.34.82/botocore/data/datasync/2018-11-09/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   254497 2024-04-11 01:00:33.000000 botocore-a-la-carte-datasync-1.34.82/botocore/data/datasync/2018-11-09/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:48.584771 botocore-a-la-carte-datasync-1.34.82/botocore_a_la_carte_datasync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-11 01:00:48.000000 botocore-a-la-carte-datasync-1.34.82/botocore_a_la_carte_datasync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-11 01:00:48.000000 botocore-a-la-carte-datasync-1.34.82/botocore_a_la_carte_datasync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:00:48.000000 botocore-a-la-carte-datasync-1.34.82/botocore_a_la_carte_datasync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 01:00:48.000000 botocore-a-la-carte-datasync-1.34.82/botocore_a_la_carte_datasync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 01:00:48.584771 botocore-a-la-carte-datasync-1.34.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-11 01:00:48.000000 botocore-a-la-carte-datasync-1.34.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:41.458277 botocore-a-la-carte-datasync-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:41.000000 botocore-a-la-carte-datasync-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2023-12-28 01:06:41.458277 botocore-a-la-carte-datasync-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:41.454277 botocore-a-la-carte-datasync-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:41.454277 botocore-a-la-carte-datasync-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:41.454277 botocore-a-la-carte-datasync-1.34.9/botocore/data/datasync/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:41.454277 botocore-a-la-carte-datasync-1.34.9/botocore/data/datasync/2018-11-09/
+-rw-r--r--   0 runner    (1001) docker     (127)    13734 2023-12-28 01:06:26.000000 botocore-a-la-carte-datasync-1.34.9/botocore/data/datasync/2018-11-09/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-datasync-1.34.9/botocore/data/datasync/2018-11-09/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-12-28 01:06:26.000000 botocore-a-la-carte-datasync-1.34.9/botocore/data/datasync/2018-11-09/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   244492 2023-12-28 01:06:26.000000 botocore-a-la-carte-datasync-1.34.9/botocore/data/datasync/2018-11-09/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:41.458277 botocore-a-la-carte-datasync-1.34.9/botocore_a_la_carte_datasync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2023-12-28 01:06:41.000000 botocore-a-la-carte-datasync-1.34.9/botocore_a_la_carte_datasync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2023-12-28 01:06:41.000000 botocore-a-la-carte-datasync-1.34.9/botocore_a_la_carte_datasync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:41.000000 botocore-a-la-carte-datasync-1.34.9/botocore_a_la_carte_datasync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:41.000000 botocore-a-la-carte-datasync-1.34.9/botocore_a_la_carte_datasync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:41.458277 botocore-a-la-carte-datasync-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-12-28 01:06:41.000000 botocore-a-la-carte-datasync-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-datasync-1.34.82/LICENSE.txt` & `botocore-a-la-carte-datasync-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-datasync-1.34.82/PKG-INFO` & `botocore-a-la-carte-datasync-1.34.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-datasync
-Version: 1.34.82
+Version: 1.34.9
 Summary: datasync data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-datasync-1.34.82/botocore/data/datasync/2018-11-09/endpoint-rule-set-1.json` & `botocore-a-la-carte-datasync-1.34.9/botocore/data/datasync/2018-11-09/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-datasync-1.34.82/botocore/data/datasync/2018-11-09/paginators-1.json` & `botocore-a-la-carte-datasync-1.34.9/botocore/data/datasync/2018-11-09/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-datasync-1.34.82/botocore/data/datasync/2018-11-09/service-2.json` & `botocore-a-la-carte-datasync-1.34.9/botocore/data/datasync/2018-11-09/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964075813772192%*

 * *Differences: {"'operations'": "{'CreateLocationAzureBlob': {'documentation': '<p>Creates an endpoint for a "*

 * *                 'Microsoft Azure Blob Storage container that DataSync can use as a transfer '*

 * *                 'source or destination.</p> <p>Before you begin, make sure you know <a '*

 * *                 'href="https://docs.aws.amazon.com/datasync/latest/userguide/creating-azure-blob-location.html#azure-blob-access">how '*

 * *                 'DataSync accesses Azure Blob Storage</a> and works with <a '*

 * *                […]*

```diff
@@ -80,15 +80,15 @@
             },
             "name": "CreateAgent",
             "output": {
                 "shape": "CreateAgentResponse"
             }
         },
         "CreateLocationAzureBlob": {
-            "documentation": "<p>Creates a transfer <i>location</i> for a Microsoft Azure Blob Storage container. DataSync can use this location as a transfer source or destination.</p> <p>Before you begin, make sure you know <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/creating-azure-blob-location.html#azure-blob-access\">how DataSync accesses Azure Blob Storage</a> and works with <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/creating-azure-blob-location.html#azure-blob-access-tiers\">access tiers</a> and <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/creating-azure-blob-location.html#blob-types\">blob types</a>. You also need a <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/creating-azure-blob-location.html#azure-blob-creating-agent\">DataSync agent</a> that can connect to your container.</p>",
+            "documentation": "<p>Creates an endpoint for a Microsoft Azure Blob Storage container that DataSync can use as a transfer source or destination.</p> <p>Before you begin, make sure you know <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/creating-azure-blob-location.html#azure-blob-access\">how DataSync accesses Azure Blob Storage</a> and works with <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/creating-azure-blob-location.html#azure-blob-access-tiers\">access tiers</a> and <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/creating-azure-blob-location.html#blob-types\">blob types</a>. You also need a <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/creating-azure-blob-location.html#azure-blob-creating-agent\">DataSync agent</a> that can connect to your container.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -102,15 +102,15 @@
             },
             "name": "CreateLocationAzureBlob",
             "output": {
                 "shape": "CreateLocationAzureBlobResponse"
             }
         },
         "CreateLocationEfs": {
-            "documentation": "<p>Creates a transfer <i>location</i> for an Amazon EFS file system. DataSync can use this location as a source or destination for transferring data.</p> <p>Before you begin, make sure that you understand how DataSync <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-efs-location.html#create-efs-location-access\">accesses Amazon EFS file systems</a>.</p>",
+            "documentation": "<p>Creates an endpoint for an Amazon EFS file system that DataSync can access for a transfer. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-efs-location.html\">Creating a location for Amazon EFS</a>.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -124,15 +124,15 @@
             },
             "name": "CreateLocationEfs",
             "output": {
                 "shape": "CreateLocationEfsResponse"
             }
         },
         "CreateLocationFsxLustre": {
-            "documentation": "<p>Creates a transfer <i>location</i> for an Amazon FSx for Lustre file system. DataSync can use this location as a source or destination for transferring data.</p> <p>Before you begin, make sure that you understand how DataSync <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-lustre-location.html#create-lustre-location-access\">accesses FSx for Lustre file systems</a>.</p>",
+            "documentation": "<p>Creates an endpoint for an Amazon FSx for Lustre file system.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -146,15 +146,15 @@
             },
             "name": "CreateLocationFsxLustre",
             "output": {
                 "shape": "CreateLocationFsxLustreResponse"
             }
         },
         "CreateLocationFsxOntap": {
-            "documentation": "<p>Creates a transfer <i>location</i> for an Amazon FSx for NetApp ONTAP file system. DataSync can use this location as a source or destination for transferring data.</p> <p>Before you begin, make sure that you understand how DataSync <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-ontap-location.html#create-ontap-location-access\">accesses FSx for ONTAP file systems</a>.</p>",
+            "documentation": "<p>Creates an endpoint for an Amazon FSx for NetApp ONTAP file system that DataSync can use for a data transfer.</p> <p>Before you begin, make sure that you understand how DataSync <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-ontap-location.html#create-ontap-location-access\">accesses an FSx for ONTAP file system</a>.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -168,15 +168,15 @@
             },
             "name": "CreateLocationFsxOntap",
             "output": {
                 "shape": "CreateLocationFsxOntapResponse"
             }
         },
         "CreateLocationFsxOpenZfs": {
-            "documentation": "<p>Creates a transfer <i>location</i> for an Amazon FSx for OpenZFS file system. DataSync can use this location as a source or destination for transferring data.</p> <p>Before you begin, make sure that you understand how DataSync <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-openzfs-location.html#create-openzfs-access\">accesses FSx for OpenZFS file systems</a>.</p> <note> <p>Request parameters related to <code>SMB</code> aren't supported with the <code>CreateLocationFsxOpenZfs</code> operation.</p> </note>",
+            "documentation": "<p>Creates an endpoint for an Amazon FSx for OpenZFS file system that DataSync can access for a transfer. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-openzfs-location.html\">Creating a location for FSx for OpenZFS</a>.</p> <note> <p>Request parameters related to <code>SMB</code> aren't supported with the <code>CreateLocationFsxOpenZfs</code> operation.</p> </note>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -190,15 +190,15 @@
             },
             "name": "CreateLocationFsxOpenZfs",
             "output": {
                 "shape": "CreateLocationFsxOpenZfsResponse"
             }
         },
         "CreateLocationFsxWindows": {
-            "documentation": "<p>Creates a transfer <i>location</i> for an Amazon FSx for Windows File Server file system. DataSync can use this location as a source or destination for transferring data.</p> <p>Before you begin, make sure that you understand how DataSync <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-fsx-location.html#create-fsx-location-access\">accesses FSx for Windows File Server file systems</a>.</p>",
+            "documentation": "<p>Creates an endpoint for an Amazon FSx for Windows File Server file system that DataSync can use for a data transfer.</p> <p>Before you begin, make sure that you understand how DataSync <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-fsx-location.html#create-fsx-location-access\">accesses an FSx for Windows File Server</a>.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -212,15 +212,15 @@
             },
             "name": "CreateLocationFsxWindows",
             "output": {
                 "shape": "CreateLocationFsxWindowsResponse"
             }
         },
         "CreateLocationHdfs": {
-            "documentation": "<p>Creates a transfer <i>location</i> for a Hadoop Distributed File System (HDFS). DataSync can use this location as a source or destination for transferring data.</p> <p>Before you begin, make sure that you understand how DataSync <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-hdfs-location.html#accessing-hdfs\">accesses HDFS clusters</a>.</p>",
+            "documentation": "<p>Creates an endpoint for a Hadoop Distributed File System (HDFS). </p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -234,15 +234,15 @@
             },
             "name": "CreateLocationHdfs",
             "output": {
                 "shape": "CreateLocationHdfsResponse"
             }
         },
         "CreateLocationNfs": {
-            "documentation": "<p>Creates a transfer <i>location</i> for a Network File System (NFS) file server. DataSync can use this location as a source or destination for transferring data.</p> <p>Before you begin, make sure that you understand how DataSync <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-nfs-location.html#accessing-nfs\">accesses NFS file servers</a>.</p> <note> <p>If you're copying data to or from an Snowcone device, you can also use <code>CreateLocationNfs</code> to create your transfer location. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/nfs-on-snowcone.html\">Configuring transfers with Snowcone</a>.</p> </note>",
+            "documentation": "<p>Creates an endpoint for a Network File System (NFS) file server that DataSync can use for a data transfer.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-nfs-location.html\">Configuring transfers to or from an NFS file server</a>.</p> <note> <p>If you're copying data to or from an Snowcone device, you can also use <code>CreateLocationNfs</code> to create your transfer location. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/nfs-on-snowcone.html\">Configuring transfers with Snowcone</a>.</p> </note>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -256,15 +256,15 @@
             },
             "name": "CreateLocationNfs",
             "output": {
                 "shape": "CreateLocationNfsResponse"
             }
         },
         "CreateLocationObjectStorage": {
-            "documentation": "<p>Creates a transfer <i>location</i> for an object storage system. DataSync can use this location as a source or destination for transferring data.</p> <p>Before you begin, make sure that you understand the <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-object-location.html#create-object-location-prerequisites\">prerequisites</a> for DataSync to work with object storage systems.</p>",
+            "documentation": "<p>Creates an endpoint for an object storage system that DataSync can access for a transfer. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-object-location.html\">Creating a location for object storage</a>.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -278,15 +278,15 @@
             },
             "name": "CreateLocationObjectStorage",
             "output": {
                 "shape": "CreateLocationObjectStorageResponse"
             }
         },
         "CreateLocationS3": {
-            "documentation": "<p>Creates a transfer <i>location</i> for an Amazon S3 bucket. DataSync can use this location as a source or destination for transferring data.</p> <important> <p>Before you begin, make sure that you read the following topics:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Storage class considerations with Amazon S3 locations</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#create-s3-location-s3-requests\">Evaluating S3 request costs when using DataSync</a> </p> </li> </ul> </important> <p> For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html\">Configuring transfers with Amazon S3</a>.</p>",
+            "documentation": "<p>A <i>location</i> is an endpoint for an Amazon S3 bucket. DataSync can use the location as a source or destination for copying data.</p> <important> <p>Before you create your location, make sure that you read the following sections:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Storage class considerations with Amazon S3 locations</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#create-s3-location-s3-requests\">Evaluating S3 request costs when using DataSync</a> </p> </li> </ul> </important> <p> For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-locations-cli.html#create-location-s3-cli\">Creating an Amazon S3 location</a>.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -300,15 +300,15 @@
             },
             "name": "CreateLocationS3",
             "output": {
                 "shape": "CreateLocationS3Response"
             }
         },
         "CreateLocationSmb": {
-            "documentation": "<p>Creates a transfer <i>location</i> for a Server Message Block (SMB) file server. DataSync can use this location as a source or destination for transferring data.</p> <p>Before you begin, make sure that you understand how DataSync <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-smb-location.html#configuring-smb\">accesses SMB file servers</a>.</p>",
+            "documentation": "<p>Creates an endpoint for a Server Message Block (SMB) file server that DataSync can use for a data transfer.</p> <p>Before you begin, make sure that you understand how DataSync <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-smb-location.html\">accesses an SMB file server</a>.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -366,15 +366,15 @@
             },
             "name": "DeleteAgent",
             "output": {
                 "shape": "DeleteAgentResponse"
             }
         },
         "DeleteLocation": {
-            "documentation": "<p>Deletes a transfer location resource from DataSync. </p>",
+            "documentation": "<p>Deletes the configuration of a location used by DataSync. </p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -388,15 +388,15 @@
             },
             "name": "DeleteLocation",
             "output": {
                 "shape": "DeleteLocationResponse"
             }
         },
         "DeleteTask": {
-            "documentation": "<p>Deletes a transfer task resource from DataSync.</p>",
+            "documentation": "<p>Deletes an DataSync transfer task.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -479,15 +479,15 @@
             },
             "name": "DescribeLocationAzureBlob",
             "output": {
                 "shape": "DescribeLocationAzureBlobResponse"
             }
         },
         "DescribeLocationEfs": {
-            "documentation": "<p>Provides details about how an DataSync transfer location for an Amazon EFS file system is configured.</p>",
+            "documentation": "<p>Returns metadata about your DataSync location for an Amazon EFS file system.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -501,15 +501,15 @@
             },
             "name": "DescribeLocationEfs",
             "output": {
                 "shape": "DescribeLocationEfsResponse"
             }
         },
         "DescribeLocationFsxLustre": {
-            "documentation": "<p>Provides details about how an DataSync transfer location for an Amazon FSx for Lustre file system is configured.</p>",
+            "documentation": "<p>Provides details about how an DataSync location for an Amazon FSx for Lustre file system is configured.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -523,15 +523,15 @@
             },
             "name": "DescribeLocationFsxLustre",
             "output": {
                 "shape": "DescribeLocationFsxLustreResponse"
             }
         },
         "DescribeLocationFsxOntap": {
-            "documentation": "<p>Provides details about how an DataSync transfer location for an Amazon FSx for NetApp ONTAP file system is configured.</p> <note> <p>If your location uses SMB, the <code>DescribeLocationFsxOntap</code> operation doesn't actually return a <code>Password</code>.</p> </note>",
+            "documentation": "<p>Provides details about how an DataSync location for an Amazon FSx for NetApp ONTAP file system is configured.</p> <note> <p>If your location uses SMB, the <code>DescribeLocationFsxOntap</code> operation doesn't actually return a <code>Password</code>.</p> </note>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -545,15 +545,15 @@
             },
             "name": "DescribeLocationFsxOntap",
             "output": {
                 "shape": "DescribeLocationFsxOntapResponse"
             }
         },
         "DescribeLocationFsxOpenZfs": {
-            "documentation": "<p>Provides details about how an DataSync transfer location for an Amazon FSx for OpenZFS file system is configured.</p> <note> <p>Response elements related to <code>SMB</code> aren't supported with the <code>DescribeLocationFsxOpenZfs</code> operation.</p> </note>",
+            "documentation": "<p>Provides details about how an DataSync location for an Amazon FSx for OpenZFS file system is configured.</p> <note> <p>Response elements related to <code>SMB</code> aren't supported with the <code>DescribeLocationFsxOpenZfs</code> operation.</p> </note>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -567,15 +567,15 @@
             },
             "name": "DescribeLocationFsxOpenZfs",
             "output": {
                 "shape": "DescribeLocationFsxOpenZfsResponse"
             }
         },
         "DescribeLocationFsxWindows": {
-            "documentation": "<p>Provides details about how an DataSync transfer location for an Amazon FSx for Windows File Server file system is configured.</p>",
+            "documentation": "<p>Returns metadata about an Amazon FSx for Windows File Server location, such as information about its path.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -589,15 +589,15 @@
             },
             "name": "DescribeLocationFsxWindows",
             "output": {
                 "shape": "DescribeLocationFsxWindowsResponse"
             }
         },
         "DescribeLocationHdfs": {
-            "documentation": "<p>Provides details about how an DataSync transfer location for a Hadoop Distributed File System (HDFS) is configured.</p>",
+            "documentation": "<p>Returns metadata, such as the authentication information about the Hadoop Distributed File System (HDFS) location. </p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -633,15 +633,15 @@
             },
             "name": "DescribeLocationNfs",
             "output": {
                 "shape": "DescribeLocationNfsResponse"
             }
         },
         "DescribeLocationObjectStorage": {
-            "documentation": "<p>Provides details about how an DataSync transfer location for an object storage system is configured.</p>",
+            "documentation": "<p>Returns metadata about your DataSync location for an object storage system.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -655,15 +655,15 @@
             },
             "name": "DescribeLocationObjectStorage",
             "output": {
                 "shape": "DescribeLocationObjectStorageResponse"
             }
         },
         "DescribeLocationS3": {
-            "documentation": "<p>Provides details about how an DataSync transfer location for an S3 bucket is configured.</p>",
+            "documentation": "<p>Returns metadata, such as bucket name, about an Amazon S3 bucket location.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -677,15 +677,15 @@
             },
             "name": "DescribeLocationS3",
             "output": {
                 "shape": "DescribeLocationS3Response"
             }
         },
         "DescribeLocationSmb": {
-            "documentation": "<p>Provides details about how an DataSync transfer location for a Server Message Block (SMB) file server is configured.</p>",
+            "documentation": "<p>Returns metadata, such as the path and user information about an SMB location.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -959,15 +959,15 @@
             },
             "name": "ListTagsForResource",
             "output": {
                 "shape": "ListTagsForResourceResponse"
             }
         },
         "ListTaskExecutions": {
-            "documentation": "<p>Returns a list of executions for an DataSync transfer task.</p>",
+            "documentation": "<p>Returns a list of executed tasks.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -1326,15 +1326,15 @@
             },
             "name": "UpdateStorageSystem",
             "output": {
                 "shape": "UpdateStorageSystemResponse"
             }
         },
         "UpdateTask": {
-            "documentation": "<p>Updates the configuration of an DataSync transfer task.</p>",
+            "documentation": "<p>Updates the configuration of a DataSync transfer task.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -1848,23 +1848,23 @@
                 }
             },
             "type": "structure"
         },
         "CreateLocationFsxWindowsRequest": {
             "members": {
                 "Domain": {
-                    "documentation": "<p>Specifies the name of the Microsoft Active Directory domain that the FSx for Windows File Server file system belongs to.</p> <p>If you have multiple Active Directory domains in your environment, configuring this parameter makes sure that DataSync connects to the right file system.</p>",
+                    "documentation": "<p>Specifies the name of the Windows domain that the FSx for Windows File Server belongs to.</p> <p>If you have multiple domains in your environment, configuring this parameter makes sure that DataSync connects to the right file server.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-fsx-location.html#create-fsx-windows-location-permissions\">required permissions</a> for FSx for Windows File Server locations.</p>",
                     "shape": "SmbDomain"
                 },
                 "FsxFilesystemArn": {
                     "documentation": "<p>Specifies the Amazon Resource Name (ARN) for the FSx for Windows File Server file system.</p>",
                     "shape": "FsxFilesystemArn"
                 },
                 "Password": {
-                    "documentation": "<p>Specifies the password of the user with the permissions to mount and access the files, folders, and file metadata in your FSx for Windows File Server file system.</p>",
+                    "documentation": "<p>Specifies the password of the user who has the permissions to access files and folders in the file system.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-fsx-location.html#create-fsx-windows-location-permissions\">required permissions</a> for FSx for Windows File Server locations.</p>",
                     "shape": "SmbPassword"
                 },
                 "SecurityGroupArns": {
                     "documentation": "<p>Specifies the ARNs of the security groups that provide access to your file system's preferred subnet.</p> <note> <p>If you choose a security group that doesn't allow connections from within itself, do one of the following:</p> <ul> <li> <p>Configure the security group to allow it to communicate within itself.</p> </li> <li> <p>Choose a different security group that can communicate with the mount target's security group.</p> </li> </ul> </note>",
                     "shape": "Ec2SecurityGroupArnList"
                 },
                 "Subdirectory": {
@@ -1872,15 +1872,15 @@
                     "shape": "FsxWindowsSubdirectory"
                 },
                 "Tags": {
                     "documentation": "<p>Specifies labels that help you categorize, filter, and search for your Amazon Web Services resources. We recommend creating at least a name tag for your location.</p>",
                     "shape": "InputTagList"
                 },
                 "User": {
-                    "documentation": "<p>Specifies the user with the permissions to mount and access the files, folders, and file metadata in your FSx for Windows File Server file system.</p> <p>For information about choosing a user with the right level of access for your transfer, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-fsx-location.html#create-fsx-windows-location-permissions\">required permissions</a> for FSx for Windows File Server locations.</p>",
+                    "documentation": "<p>Specifies the user who has the permissions to access files, folders, and metadata in your file system.</p> <p>For information about choosing a user with the right level of access for your transfer, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-fsx-location.html#create-fsx-windows-location-permissions\">required permissions</a> for FSx for Windows File Server locations.</p>",
                     "shape": "SmbUser"
                 }
             },
             "required": [
                 "FsxFilesystemArn",
                 "SecurityGroupArns",
                 "User",
@@ -2070,62 +2070,62 @@
             },
             "type": "structure"
         },
         "CreateLocationS3Request": {
             "documentation": "<p>CreateLocationS3Request</p>",
             "members": {
                 "AgentArns": {
-                    "documentation": "<p>(Amazon S3 on Outposts only) Specifies the Amazon Resource Name (ARN) of the DataSync agent on your Outpost.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/deploy-agents.html#outposts-agent\">Deploy your DataSync agent on Outposts</a>.</p>",
+                    "documentation": "<p>If you're using DataSync on an Amazon Web Services Outpost, specify the Amazon Resource Names (ARNs) of the DataSync agents deployed on your Outpost. For more information about launching a DataSync agent on an Amazon Web Services Outpost, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/deploy-agents.html#outposts-agent\">Deploy your DataSync agent on Outposts</a>.</p>",
                     "shape": "AgentArnList"
                 },
                 "S3BucketArn": {
-                    "documentation": "<p>Specifies the ARN of the S3 bucket that you want to use as a location. (When creating your DataSync task later, you specify whether this location is a transfer source or destination.) </p> <p>If your S3 bucket is located on an Outposts resource, you must specify an Amazon S3 access point. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/access-points.html\">Managing data access with Amazon S3 access points</a> in the <i>Amazon S3 User Guide</i>.</p>",
+                    "documentation": "<p>The ARN of the Amazon S3 bucket. If the bucket is on an Amazon Web Services Outpost, this must be an access point ARN.</p>",
                     "shape": "S3BucketArn"
                 },
                 "S3Config": {
                     "shape": "S3Config"
                 },
                 "S3StorageClass": {
-                    "documentation": "<p>Specifies the storage class that you want your objects to use when Amazon S3 is a transfer destination.</p> <p>For buckets in Amazon Web Services Regions, the storage class defaults to <code>STANDARD</code>. For buckets on Outposts, the storage class defaults to <code>OUTPOSTS</code>.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Storage class considerations with Amazon S3 transfers</a>.</p>",
+                    "documentation": "<p>The Amazon S3 storage class that you want to store your files in when this location is used as a task destination. For buckets in Amazon Web Services Regions, the storage class defaults to Standard. For buckets on Outposts, the storage class defaults to Amazon Web Services S3 Outposts.</p> <p>For more information about S3 storage classes, see <a href=\"http://aws.amazon.com/s3/storage-classes/\">Amazon S3 Storage Classes</a>. Some storage classes have behaviors that can affect your S3 storage cost. For detailed information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Considerations when working with S3 storage classes in DataSync</a>.</p>",
                     "shape": "S3StorageClass"
                 },
                 "Subdirectory": {
-                    "documentation": "<p>Specifies a prefix in the S3 bucket that DataSync reads from or writes to (depending on whether the bucket is a source or destination location).</p> <note> <p>DataSync can't transfer objects with a prefix that begins with a slash (<code>/</code>) or includes <code>//</code>, <code>/./</code>, or <code>/../</code> patterns. For example:</p> <ul> <li> <p> <code>/photos</code> </p> </li> <li> <p> <code>photos//2006/January</code> </p> </li> <li> <p> <code>photos/./2006/February</code> </p> </li> <li> <p> <code>photos/../2006/March</code> </p> </li> </ul> </note>",
+                    "documentation": "<p>A subdirectory in the Amazon S3 bucket. This subdirectory in Amazon S3 is used to read data from the S3 source location or write data to the S3 destination.</p>",
                     "shape": "S3Subdirectory"
                 },
                 "Tags": {
-                    "documentation": "<p>Specifies labels that help you categorize, filter, and search for your Amazon Web Services resources. We recommend creating at least a name tag for your transfer location.</p>",
+                    "documentation": "<p>The key-value pair that represents the tag that you want to add to the location. The value can be an empty string. We recommend using tags to name your resources.</p>",
                     "shape": "InputTagList"
                 }
             },
             "required": [
                 "S3BucketArn",
                 "S3Config"
             ],
             "type": "structure"
         },
         "CreateLocationS3Response": {
             "documentation": "<p>CreateLocationS3Response</p>",
             "members": {
                 "LocationArn": {
-                    "documentation": "<p>The ARN of the S3 location that you created.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the source Amazon S3 bucket location that is created.</p>",
                     "shape": "LocationArn"
                 }
             },
             "type": "structure"
         },
         "CreateLocationSmbRequest": {
             "documentation": "<p>CreateLocationSmbRequest</p>",
             "members": {
                 "AgentArns": {
                     "documentation": "<p>Specifies the DataSync agent (or agents) which you want to connect to your SMB file server. You specify an agent by using its Amazon Resource Name (ARN).</p>",
                     "shape": "AgentArnList"
                 },
                 "Domain": {
-                    "documentation": "<p>Specifies the name of the Active Directory domain that your SMB file server belongs to. </p> <p>If you have multiple Active Directory domains in your environment, configuring this parameter makes sure that DataSync connects to the right file server.</p>",
+                    "documentation": "<p>Specifies the Windows domain name that your SMB file server belongs to. </p> <p>If you have multiple domains in your environment, configuring this parameter makes sure that DataSync connects to the right file server.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-smb-location.html#configuring-smb-permissions\">required permissions</a> for SMB locations.</p>",
                     "shape": "SmbDomain"
                 },
                 "MountOptions": {
                     "documentation": "<p>Specifies the version of the SMB protocol that DataSync uses to access your SMB file server.</p>",
                     "shape": "SmbMountOptions"
                 },
                 "Password": {
@@ -2133,23 +2133,23 @@
                     "shape": "SmbPassword"
                 },
                 "ServerHostname": {
                     "documentation": "<p>Specifies the Domain Name Service (DNS) name or IP address of the SMB file server that your DataSync agent will mount.</p> <note> <p>You can't specify an IP version 6 (IPv6) address.</p> </note>",
                     "shape": "ServerHostname"
                 },
                 "Subdirectory": {
-                    "documentation": "<p>Specifies the name of the share exported by your SMB file server where DataSync will read or write data. You can include a subdirectory in the share path (for example, <code>/path/to/subdirectory</code>). Make sure that other SMB clients in your network can also mount this path.</p> <p>To copy all data in the subdirectory, DataSync must be able to mount the SMB share and access all of its data. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-smb-location.html#configuring-smb-permissions\">required permissions</a> for SMB locations.</p>",
+                    "documentation": "<p>Specifies the name of the share exported by your SMB file server where DataSync will read or write data. You can include a subdirectory in the share path (for example, <code>/path/to/subdirectory</code>). Make sure that other SMB clients in your network can also mount this path.</p> <p>To copy all data in the specified subdirectory, DataSync must be able to mount the SMB share and access all of its data. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-smb-location.html#configuring-smb-permissions\">required permissions</a> for SMB locations.</p>",
                     "shape": "SmbSubdirectory"
                 },
                 "Tags": {
                     "documentation": "<p>Specifies labels that help you categorize, filter, and search for your Amazon Web Services resources. We recommend creating at least a name tag for your location.</p>",
                     "shape": "InputTagList"
                 },
                 "User": {
-                    "documentation": "<p>Specifies the user that can mount and access the files, folders, and file metadata in your SMB file server.</p> <p>For information about choosing a user with the right level of access for your transfer, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-smb-location.html#configuring-smb-permissions\">required permissions</a> for SMB locations.</p>",
+                    "documentation": "<p>Specifies the user name that can mount your SMB file server and has permission to access the files and folders involved in your transfer.</p> <p>For information about choosing a user with the right level of access for your transfer, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-smb-location.html#configuring-smb-permissions\">required permissions</a> for SMB locations.</p>",
                     "shape": "SmbUser"
                 }
             },
             "required": [
                 "Subdirectory",
                 "ServerHostname",
                 "User",
@@ -2183,18 +2183,14 @@
                     "documentation": "<p>Specifies a list of filter rules that exclude specific data during your transfer. For more information and examples, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/filtering.html\">Filtering data transferred by DataSync</a>.</p>",
                     "shape": "FilterList"
                 },
                 "Includes": {
                     "documentation": "<p>Specifies a list of filter rules that include specific data during your transfer. For more information and examples, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/filtering.html\">Filtering data transferred by DataSync</a>.</p>",
                     "shape": "FilterList"
                 },
-                "ManifestConfig": {
-                    "documentation": "<p>Configures a manifest, which is a list of files or objects that you want DataSync to transfer. For more information and configuration examples, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/transferring-with-manifest.html\">Specifying what DataSync transfers by using a manifest</a>.</p> <p>When using this parameter, your caller identity (the role that you're using DataSync with) must have the <code>iam:PassRole</code> permission. The <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/security-iam-awsmanpol.html#security-iam-awsmanpol-awsdatasyncfullaccess\">AWSDataSyncFullAccess</a> policy includes this permission.</p>",
-                    "shape": "ManifestConfig"
-                },
                 "Name": {
                     "documentation": "<p>The name of a task. This value is a text reference that is used to identify the task in the console. </p>",
                     "shape": "TagValue"
                 },
                 "Options": {
                     "documentation": "<p>Specifies the configuration options for a task. Some options include preserving file or object metadata and verifying data integrity.</p> <p>You can also override these options before starting an individual run of a task (also known as a <i>task execution</i>). For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/API_StartTaskExecution.html\">StartTaskExecution</a>.</p>",
                     "shape": "Options"
@@ -2208,15 +2204,15 @@
                     "shape": "LocationArn"
                 },
                 "Tags": {
                     "documentation": "<p>Specifies the tags that you want to apply to the Amazon Resource Name (ARN) representing the task.</p> <p> <i>Tags</i> are key-value pairs that help you manage, filter, and search for your DataSync resources.</p>",
                     "shape": "InputTagList"
                 },
                 "TaskReportConfig": {
-                    "documentation": "<p>Specifies how you want to configure a task report, which provides detailed information about your DataSync transfer. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/task-reports.html\">Monitoring your DataSync transfers with task reports</a>.</p> <p>When using this parameter, your caller identity (the role that you're using DataSync with) must have the <code>iam:PassRole</code> permission. The <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/security-iam-awsmanpol.html#security-iam-awsmanpol-awsdatasyncfullaccess\">AWSDataSyncFullAccess</a> policy includes this permission.</p>",
+                    "documentation": "<p>Specifies how you want to configure a task report, which provides detailed information about for your DataSync transfer.</p>",
                     "shape": "TaskReportConfig"
                 }
             },
             "required": [
                 "SourceLocationArn",
                 "DestinationLocationArn"
             ],
@@ -2597,15 +2593,15 @@
                 }
             },
             "type": "structure"
         },
         "DescribeLocationFsxWindowsRequest": {
             "members": {
                 "LocationArn": {
-                    "documentation": "<p>Specifies the Amazon Resource Name (ARN) of the FSx for Windows File Server location.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the FSx for Windows File Server location to describe.</p>",
                     "shape": "LocationArn"
                 }
             },
             "required": [
                 "LocationArn"
             ],
             "type": "structure"
@@ -2613,52 +2609,52 @@
         "DescribeLocationFsxWindowsResponse": {
             "members": {
                 "CreationTime": {
                     "documentation": "<p>The time that the FSx for Windows File Server location was created.</p>",
                     "shape": "Time"
                 },
                 "Domain": {
-                    "documentation": "<p>The name of the Microsoft Active Directory domain that the FSx for Windows File Server file system belongs to.</p>",
+                    "documentation": "<p>The name of the Windows domain that the FSx for Windows File Server belongs to.</p>",
                     "shape": "SmbDomain"
                 },
                 "LocationArn": {
-                    "documentation": "<p>The ARN of the FSx for Windows File Server location.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the FSx for Windows File Server location that was described.</p>",
                     "shape": "LocationArn"
                 },
                 "LocationUri": {
-                    "documentation": "<p>The uniform resource identifier (URI) of the FSx for Windows File Server location.</p>",
+                    "documentation": "<p>The URL of the FSx for Windows File Server location that was described.</p>",
                     "shape": "LocationUri"
                 },
                 "SecurityGroupArns": {
-                    "documentation": "<p>The ARNs of the security groups that are configured for the FSx for Windows File Server file system.</p>",
+                    "documentation": "<p>The Amazon Resource Names (ARNs) of the security groups that are configured for the FSx for Windows File Server file system.</p>",
                     "shape": "Ec2SecurityGroupArnList"
                 },
                 "User": {
-                    "documentation": "<p>The user with the permissions to mount and access the FSx for Windows File Server file system.</p>",
+                    "documentation": "<p>The user who has the permissions to access files and folders in the FSx for Windows File Server file system.</p>",
                     "shape": "SmbUser"
                 }
             },
             "type": "structure"
         },
         "DescribeLocationHdfsRequest": {
             "members": {
                 "LocationArn": {
-                    "documentation": "<p>Specifies the Amazon Resource Name (ARN) of the HDFS location.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the HDFS cluster location to describe.</p>",
                     "shape": "LocationArn"
                 }
             },
             "required": [
                 "LocationArn"
             ],
             "type": "structure"
         },
         "DescribeLocationHdfsResponse": {
             "members": {
                 "AgentArns": {
-                    "documentation": "<p>The ARNs of the DataSync agents that can connect with your HDFS cluster.</p>",
+                    "documentation": "<p>The ARNs of the agents that are used to connect to the HDFS cluster. </p>",
                     "shape": "AgentArnList"
                 },
                 "AuthenticationType": {
                     "documentation": "<p>The type of authentication used to determine the identity of the user. </p>",
                     "shape": "HdfsAuthenticationType"
                 },
                 "BlockSize": {
@@ -2674,35 +2670,35 @@
                     "shape": "KerberosPrincipal"
                 },
                 "KmsKeyProviderUri": {
                     "documentation": "<p> The URI of the HDFS cluster's Key Management Server (KMS). </p>",
                     "shape": "KmsKeyProviderUri"
                 },
                 "LocationArn": {
-                    "documentation": "<p>The ARN of the HDFS location.</p>",
+                    "documentation": "<p>The ARN of the HDFS cluster location.</p>",
                     "shape": "LocationArn"
                 },
                 "LocationUri": {
-                    "documentation": "<p>The URI of the HDFS location.</p>",
+                    "documentation": "<p>The URI of the HDFS cluster location.</p>",
                     "shape": "LocationUri"
                 },
                 "NameNodes": {
-                    "documentation": "<p>The NameNode that manages the HDFS namespace. </p>",
+                    "documentation": "<p>The NameNode that manage the HDFS namespace. </p>",
                     "shape": "HdfsNameNodeList"
                 },
                 "QopConfiguration": {
-                    "documentation": "<p>The Quality of Protection (QOP) configuration, which specifies the Remote Procedure Call (RPC) and data transfer protection settings configured on the HDFS cluster. </p>",
+                    "documentation": "<p>The Quality of Protection (QOP) configuration specifies the Remote Procedure Call (RPC) and data transfer protection settings configured on the Hadoop Distributed File System (HDFS) cluster. </p>",
                     "shape": "QopConfiguration"
                 },
                 "ReplicationFactor": {
                     "documentation": "<p>The number of DataNodes to replicate the data to when writing to the HDFS cluster. </p>",
                     "shape": "HdfsReplicationFactor"
                 },
                 "SimpleUser": {
-                    "documentation": "<p>The user name to identify the client on the host operating system. This parameter is used if the <code>AuthenticationType</code> is defined as <code>SIMPLE</code>.</p>",
+                    "documentation": "<p>The user name used to identify the client on the host operating system. This parameter is used if the <code>AuthenticationType</code> is defined as <code>SIMPLE</code>.</p>",
                     "shape": "HdfsUser"
                 }
             },
             "type": "structure"
         },
         "DescribeLocationNfsRequest": {
             "documentation": "<p>DescribeLocationNfsRequest</p>",
@@ -2725,15 +2721,15 @@
                     "shape": "Time"
                 },
                 "LocationArn": {
                     "documentation": "<p>The ARN of the NFS location.</p>",
                     "shape": "LocationArn"
                 },
                 "LocationUri": {
-                    "documentation": "<p>The URI of the NFS location.</p>",
+                    "documentation": "<p>The URL of the NFS location.</p>",
                     "shape": "LocationUri"
                 },
                 "MountOptions": {
                     "documentation": "<p>The mount options that DataSync uses to mount your NFS file server.</p>",
                     "shape": "NfsMountOptions"
                 },
                 "OnPremConfig": {
@@ -2742,15 +2738,15 @@
             },
             "type": "structure"
         },
         "DescribeLocationObjectStorageRequest": {
             "documentation": "<p>DescribeLocationObjectStorageRequest</p>",
             "members": {
                 "LocationArn": {
-                    "documentation": "<p>Specifies the Amazon Resource Name (ARN) of the object storage system location.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the object storage system location that you want information about.</p>",
                     "shape": "LocationArn"
                 }
             },
             "required": [
                 "LocationArn"
             ],
             "type": "structure"
@@ -2759,27 +2755,27 @@
             "documentation": "<p>DescribeLocationObjectStorageResponse</p>",
             "members": {
                 "AccessKey": {
                     "documentation": "<p>The access key (for example, a user name) required to authenticate with the object storage system.</p>",
                     "shape": "ObjectStorageAccessKey"
                 },
                 "AgentArns": {
-                    "documentation": "<p>The ARNs of the DataSync agents that can connect with your object storage system.</p>",
+                    "documentation": "<p>The ARNs of the DataSync agents that can securely connect with your location.</p>",
                     "shape": "AgentArnList"
                 },
                 "CreationTime": {
                     "documentation": "<p>The time that the location was created.</p>",
                     "shape": "Time"
                 },
                 "LocationArn": {
                     "documentation": "<p>The ARN of the object storage system location.</p>",
                     "shape": "LocationArn"
                 },
                 "LocationUri": {
-                    "documentation": "<p>The URI of the object storage system location.</p>",
+                    "documentation": "<p>The URL of the object storage system location.</p>",
                     "shape": "LocationUri"
                 },
                 "ServerCertificate": {
                     "documentation": "<p>The self-signed certificate that DataSync uses to securely authenticate with your object storage system.</p>",
                     "shape": "ObjectStorageCertificate"
                 },
                 "ServerPort": {
@@ -2793,94 +2789,94 @@
             },
             "type": "structure"
         },
         "DescribeLocationS3Request": {
             "documentation": "<p>DescribeLocationS3Request</p>",
             "members": {
                 "LocationArn": {
-                    "documentation": "<p>Specifies the Amazon Resource Name (ARN) of the Amazon S3 location.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon S3 bucket location to describe.</p>",
                     "shape": "LocationArn"
                 }
             },
             "required": [
                 "LocationArn"
             ],
             "type": "structure"
         },
         "DescribeLocationS3Response": {
             "documentation": "<p>DescribeLocationS3Response</p>",
             "members": {
                 "AgentArns": {
-                    "documentation": "<p>The ARNs of the DataSync agents deployed on your Outpost when using working with Amazon S3 on Outposts.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/deploy-agents.html#outposts-agent\">Deploy your DataSync agent on Outposts</a>.</p>",
+                    "documentation": "<p>If you are using DataSync on an Amazon Web Services Outpost, the Amazon Resource Name (ARNs) of the EC2 agents deployed on your Outpost. For more information about launching a DataSync agent on an Amazon Web Services Outpost, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/deploy-agents.html#outposts-agent\">Deploy your DataSync agent on Outposts</a>.</p>",
                     "shape": "AgentArnList"
                 },
                 "CreationTime": {
-                    "documentation": "<p>The time that the Amazon S3 location was created.</p>",
+                    "documentation": "<p>The time that the Amazon S3 bucket location was created.</p>",
                     "shape": "Time"
                 },
                 "LocationArn": {
-                    "documentation": "<p>The ARN of the Amazon S3 location.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon S3 bucket or access point.</p>",
                     "shape": "LocationArn"
                 },
                 "LocationUri": {
                     "documentation": "<p>The URL of the Amazon S3 location that was described.</p>",
                     "shape": "LocationUri"
                 },
                 "S3Config": {
                     "shape": "S3Config"
                 },
                 "S3StorageClass": {
-                    "documentation": "<p>When Amazon S3 is a destination location, this is the storage class that you chose for your objects.</p> <p>Some storage classes have behaviors that can affect your Amazon S3 storage costs. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Storage class considerations with Amazon S3 transfers</a>.</p>",
+                    "documentation": "<p>The Amazon S3 storage class that you chose to store your files in when this location is used as a task destination. For more information about S3 storage classes, see <a href=\"http://aws.amazon.com/s3/storage-classes/\">Amazon S3 Storage Classes</a>. Some storage classes have behaviors that can affect your S3 storage cost. For detailed information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Considerations when working with S3 storage classes in DataSync</a>.</p>",
                     "shape": "S3StorageClass"
                 }
             },
             "type": "structure"
         },
         "DescribeLocationSmbRequest": {
             "documentation": "<p>DescribeLocationSmbRequest</p>",
             "members": {
                 "LocationArn": {
-                    "documentation": "<p>Specifies the Amazon Resource Name (ARN) of the SMB location that you want information about.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the SMB location to describe.</p>",
                     "shape": "LocationArn"
                 }
             },
             "required": [
                 "LocationArn"
             ],
             "type": "structure"
         },
         "DescribeLocationSmbResponse": {
             "documentation": "<p>DescribeLocationSmbResponse</p>",
             "members": {
                 "AgentArns": {
-                    "documentation": "<p>The ARNs of the DataSync agents that can connect with your SMB file server.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the source SMB file system location that is created.</p>",
                     "shape": "AgentArnList"
                 },
                 "CreationTime": {
                     "documentation": "<p>The time that the SMB location was created.</p>",
                     "shape": "Time"
                 },
                 "Domain": {
-                    "documentation": "<p>The name of the Microsoft Active Directory domain that the SMB file server belongs to.</p>",
+                    "documentation": "<p>The name of the Windows domain that the SMB server belongs to.</p>",
                     "shape": "SmbDomain"
                 },
                 "LocationArn": {
-                    "documentation": "<p>The ARN of the SMB location.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the SMB location that was described.</p>",
                     "shape": "LocationArn"
                 },
                 "LocationUri": {
-                    "documentation": "<p>The URI of the SMB location.</p>",
+                    "documentation": "<p>The URL of the source SMB location that was described.</p>",
                     "shape": "LocationUri"
                 },
                 "MountOptions": {
-                    "documentation": "<p>The protocol that DataSync use to access your SMB file.</p>",
+                    "documentation": "<p>The mount options that are available for DataSync to use to access an SMB location.</p>",
                     "shape": "SmbMountOptions"
                 },
                 "User": {
-                    "documentation": "<p>The user that can mount and access the files, folders, and file metadata in your SMB file server.</p>",
+                    "documentation": "<p>The user who can mount the share, has the permissions to access files and folders in the SMB share.</p>",
                     "shape": "SmbUser"
                 }
             },
             "type": "structure"
         },
         "DescribeStorageSystemRequest": {
             "members": {
@@ -3096,18 +3092,14 @@
                     "documentation": "<p>The number of files, objects, and directories that DataSync verified during your transfer.</p> <note> <p>When you configure your task to <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/configure-data-verification-options.html\">verify only the data that's transferred</a>, DataSync doesn't verify directories in some situations or files that fail to transfer.</p> </note>",
                     "shape": "long"
                 },
                 "Includes": {
                     "documentation": "<p>A list of filter rules that include specific data during your transfer. For more information and examples, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/filtering.html\">Filtering data transferred by DataSync</a>.</p>",
                     "shape": "FilterList"
                 },
-                "ManifestConfig": {
-                    "documentation": "<p>The configuration of the manifest that lists the files or objects to transfer. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/transferring-with-manifest.html\">Specifying what DataSync transfers by using a manifest</a>.</p>",
-                    "shape": "ManifestConfig"
-                },
                 "Options": {
                     "shape": "Options"
                 },
                 "ReportResult": {
                     "documentation": "<p>Indicates whether DataSync generated a complete <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/task-reports.html\">task report</a> for your transfer.</p>",
                     "shape": "ReportResult"
                 },
@@ -3124,15 +3116,15 @@
                     "shape": "TaskExecutionStatus"
                 },
                 "TaskExecutionArn": {
                     "documentation": "<p>The ARN of the task execution that you wanted information about. <code>TaskExecutionArn</code> is hierarchical and includes <code>TaskArn</code> for the task that was executed. </p> <p>For example, a <code>TaskExecution</code> value with the ARN <code>arn:aws:datasync:us-east-1:111222333444:task/task-0208075f79cedf4a2/execution/exec-08ef1e88ec491019b</code> executed the task with the ARN <code>arn:aws:datasync:us-east-1:111222333444:task/task-0208075f79cedf4a2</code>. </p>",
                     "shape": "TaskExecutionArn"
                 },
                 "TaskReportConfig": {
-                    "documentation": "<p>The configuration of your task report, which provides detailed information about for your DataSync transfer. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/task-reports.html\">Creating a task report</a>.</p>",
+                    "documentation": "<p>The configuration of your task report, which provides detailed information about for your DataSync transfer.</p>",
                     "shape": "TaskReportConfig"
                 }
             },
             "type": "structure"
         },
         "DescribeTaskRequest": {
             "documentation": "<p>DescribeTaskRequest</p>",
@@ -3182,18 +3174,14 @@
                     "documentation": "<p>A list of filter rules that exclude specific data during your transfer. For more information and examples, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/filtering.html\">Filtering data transferred by DataSync</a>.</p>",
                     "shape": "FilterList"
                 },
                 "Includes": {
                     "documentation": "<p>A list of filter rules that include specific data during your transfer. For more information and examples, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/filtering.html\">Filtering data transferred by DataSync</a>.</p>",
                     "shape": "FilterList"
                 },
-                "ManifestConfig": {
-                    "documentation": "<p>The configuration of the manifest that lists the files or objects to transfer. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/transferring-with-manifest.html\">Specifying what DataSync transfers by using a manifest</a>.</p>",
-                    "shape": "ManifestConfig"
-                },
                 "Name": {
                     "documentation": "<p>The name of the task that was described.</p>",
                     "shape": "TagValue"
                 },
                 "Options": {
                     "documentation": "<p>The configuration options that control the behavior of the <code>StartTaskExecution</code> operation. Some options include preserving file or object metadata and verifying data integrity.</p> <p>You can override these options for each task execution. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/API_StartTaskExecution.html\">StartTaskExecution</a>.</p>",
                     "shape": "Options"
@@ -3215,15 +3203,15 @@
                     "shape": "TaskStatus"
                 },
                 "TaskArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the task that was described.</p>",
                     "shape": "TaskArn"
                 },
                 "TaskReportConfig": {
-                    "documentation": "<p>The configuration of your task report, which provides detailed information about for your DataSync transfer. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/task-reports.html\">Creating a task report</a>.</p>",
+                    "documentation": "<p>The configuration of your task report. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/task-reports.html\">Creating a task report</a>.</p>",
                     "shape": "TaskReportConfig"
                 }
             },
             "type": "structure"
         },
         "DestinationNetworkInterfaceArns": {
             "member": {
@@ -3520,26 +3508,26 @@
             },
             "type": "structure"
         },
         "FsxProtocolSmb": {
             "documentation": "<p>Specifies the Server Message Block (SMB) protocol configuration that DataSync uses to access your Amazon FSx for NetApp ONTAP file system. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-ontap-location.html#create-ontap-location-access\">Accessing FSx for ONTAP file systems</a>.</p>",
             "members": {
                 "Domain": {
-                    "documentation": "<p>Specifies the fully qualified domain name (FQDN) of the Microsoft Active Directory that your storage virtual machine (SVM) belongs to.</p> <p>If you have multiple domains in your environment, configuring this setting makes sure that DataSync connects to the right SVM.</p>",
+                    "documentation": "<p>Specifies the fully qualified domain name (FQDN) of the Microsoft Active Directory that your storage virtual machine (SVM) belongs to.</p>",
                     "shape": "SmbDomain"
                 },
                 "MountOptions": {
                     "shape": "SmbMountOptions"
                 },
                 "Password": {
                     "documentation": "<p>Specifies the password of a user who has permission to access your SVM.</p>",
                     "shape": "SmbPassword"
                 },
                 "User": {
-                    "documentation": "<p>Specifies a user that can mount and access the files, folders, and metadata in your SVM.</p> <p>For information about choosing a user with the right level of access for your transfer, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-ontap-location.html#create-ontap-location-smb\">Using the SMB protocol</a>.</p>",
+                    "documentation": "<p>Specifies a user name that can mount the location and access the files, folders, and metadata that you need in the SVM.</p> <p>If you provide a user in your Active Directory, note the following:</p> <ul> <li> <p>If you're using Directory Service for Microsoft Active Directory, the user must be a member of the Amazon Web Services Delegated FSx Administrators group.</p> </li> <li> <p>If you're using a self-managed Active Directory, the user must be a member of either the Domain Admins group or a custom group that you specified for file system administration when you created your file system.</p> </li> </ul> <p>Make sure that the user has the permissions it needs to copy the data you want:</p> <ul> <li> <p> <code>SE_TCB_NAME</code>: Required to set object ownership and file metadata. With this privilege, you also can copy NTFS discretionary access lists (DACLs).</p> </li> <li> <p> <code>SE_SECURITY_NAME</code>: May be needed to copy NTFS system access control lists (SACLs). This operation specifically requires the Windows privilege, which is granted to members of the Domain Admins group. If you configure your task to copy SACLs, make sure that the user has the required privileges. For information about copying SACLs, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-task.html#configure-ownership-and-permissions\">Ownership and permissions-related options</a>.</p> </li> </ul>",
                     "shape": "SmbUser"
                 }
             },
             "required": [
                 "Password",
                 "User"
             ],
@@ -3924,37 +3912,37 @@
             },
             "type": "structure"
         },
         "ListTaskExecutionsRequest": {
             "documentation": "<p>ListTaskExecutions</p>",
             "members": {
                 "MaxResults": {
-                    "documentation": "<p>Specifies how many results you want in the response.</p>",
+                    "documentation": "<p>The maximum number of executed tasks to list.</p>",
                     "shape": "MaxResults"
                 },
                 "NextToken": {
-                    "documentation": "<p>Specifies an opaque string that indicates the position at which to begin the next list of results in the response.</p>",
+                    "documentation": "<p>An opaque string that indicates the position at which to begin the next list of the executed tasks.</p>",
                     "shape": "NextToken"
                 },
                 "TaskArn": {
-                    "documentation": "<p>Specifies the Amazon Resource Name (ARN) of the task that you want execution information about.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the task whose tasks you want to list.</p>",
                     "shape": "TaskArn"
                 }
             },
             "type": "structure"
         },
         "ListTaskExecutionsResponse": {
             "documentation": "<p>ListTaskExecutionsResponse</p>",
             "members": {
                 "NextToken": {
-                    "documentation": "<p>The opaque string that indicates the position to begin the next list of results in the response.</p>",
+                    "documentation": "<p>An opaque string that indicates the position at which to begin returning the next list of executed tasks.</p>",
                     "shape": "NextToken"
                 },
                 "TaskExecutions": {
-                    "documentation": "<p>A list of the task's executions.</p>",
+                    "documentation": "<p>A list of executed tasks.</p>",
                     "shape": "TaskExecutionList"
                 }
             },
             "type": "structure"
         },
         "ListTasksRequest": {
             "documentation": "<p>ListTasksRequest</p>",
@@ -4064,44 +4052,14 @@
             "enum": [
                 "OFF",
                 "BASIC",
                 "TRANSFER"
             ],
             "type": "string"
         },
-        "ManifestAction": {
-            "enum": [
-                "TRANSFER"
-            ],
-            "type": "string"
-        },
-        "ManifestConfig": {
-            "documentation": "<p>Configures a manifest, which is a list of files or objects that you want DataSync to transfer. For more information and configuration examples, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/transferring-with-manifest.html\">Specifying what DataSync transfers by using a manifest</a>.</p>",
-            "members": {
-                "Action": {
-                    "documentation": "<p>Specifies what DataSync uses the manifest for.</p>",
-                    "shape": "ManifestAction"
-                },
-                "Format": {
-                    "documentation": "<p>Specifies the file format of your manifest. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/transferring-with-manifest.html#transferring-with-manifest-create\">Creating a manifest</a>.</p>",
-                    "shape": "ManifestFormat"
-                },
-                "Source": {
-                    "documentation": "<p>Specifies the manifest that you want DataSync to use and where it's hosted.</p> <note> <p>You must specify this parameter if you're configuring a new manifest on or after February 7, 2024.</p> <p>If you don't, you'll get a 400 status code and <code>ValidationException</code> error stating that you're missing the IAM role for DataSync to access the S3 bucket where you're hosting your manifest. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/transferring-with-manifest.html#transferring-with-manifest-access\">Providing DataSync access to your manifest</a>.</p> </note>",
-                    "shape": "SourceManifestConfig"
-                }
-            },
-            "type": "structure"
-        },
-        "ManifestFormat": {
-            "enum": [
-                "CSV"
-            ],
-            "type": "string"
-        },
         "MaxP95Performance": {
             "documentation": "<p>The performance data that DataSync Discovery collects about an on-premises storage system resource.</p>",
             "members": {
                 "IopsOther": {
                     "documentation": "<p>Peak IOPS unrelated to read and write operations.</p>",
                     "shape": "NonNegativeDouble"
                 },
@@ -4494,71 +4452,71 @@
             ],
             "type": "string"
         },
         "Options": {
             "documentation": "<p>Indicates how your transfer task is configured. These options include how DataSync handles files, objects, and their associated metadata during your transfer. You also can specify how to verify data integrity, set bandwidth limits for your task, among other options.</p> <p>Each option has a default value. Unless you need to, you don't have to configure any of these options before starting your task.</p>",
             "members": {
                 "Atime": {
-                    "documentation": "<p>Specifies whether to preserve metadata indicating the last time a file was read or written to.</p> <note> <p>The behavior of <code>Atime</code> isn't fully standard across platforms, so DataSync can only do this on a best-effort basis.</p> </note> <ul> <li> <p> <code>BEST_EFFORT</code> (default) - DataSync attempts to preserve the original <code>Atime</code> attribute on all source files (that is, the version before the <code>PREPARING</code> phase of the task execution). This option is recommended.</p> </li> <li> <p> <code>NONE</code> - Ignores <code>Atime</code>.</p> </li> </ul> <note> <p>If <code>Atime</code> is set to <code>BEST_EFFORT</code>, <code>Mtime</code> must be set to <code>PRESERVE</code>. </p> <p>If <code>Atime</code> is set to <code>NONE</code>, <code>Mtime</code> must also be <code>NONE</code>. </p> </note>",
+                    "documentation": "<p>Specifies whether to preserve metadata indicating the last time a file was read or written to. If you set <code>Atime</code> to <code>BEST_EFFORT</code>, DataSync attempts to preserve the original <code>Atime</code> attribute on all source files (that is, the version before the <code>PREPARING</code> phase of the task execution).</p> <note> <p>The behavior of <code>Atime</code> isn't fully standard across platforms, so DataSync can only do this on a best-effort basis.</p> </note> <p>Default value: <code>BEST_EFFORT</code> </p> <p> <code>BEST_EFFORT</code>: Attempt to preserve the per-file <code>Atime</code> value (recommended).</p> <p> <code>NONE</code>: Ignore <code>Atime</code>.</p> <note> <p>If <code>Atime</code> is set to <code>BEST_EFFORT</code>, <code>Mtime</code> must be set to <code>PRESERVE</code>. </p> <p>If <code>Atime</code> is set to <code>NONE</code>, <code>Mtime</code> must also be <code>NONE</code>. </p> </note>",
                     "shape": "Atime"
                 },
                 "BytesPerSecond": {
                     "documentation": "<p>Limits the bandwidth used by a DataSync task. For example, if you want DataSync to use a maximum of 1 MB, set this value to <code>1048576</code> (<code>=1024*1024</code>).</p>",
                     "shape": "BytesPerSecond"
                 },
                 "Gid": {
-                    "documentation": "<p>Specifies the POSIX group ID (GID) of the file's owners.</p> <ul> <li> <p> <code>INT_VALUE</code> (default) - Preserves the integer value of user ID (UID) and GID, which is recommended.</p> </li> <li> <p> <code>NONE</code> - Ignores UID and GID.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/special-files.html#metadata-copied\">Metadata copied by DataSync</a>.</p>",
+                    "documentation": "<p>Specifies the POSIX group ID (GID) of the file's owners.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/special-files.html#metadata-copied\">Metadata copied by DataSync</a>.</p> <p>Default value: <code>INT_VALUE</code>. This preserves the integer value of the ID.</p> <p> <code>INT_VALUE</code>: Preserve the integer value of user ID (UID) and GID (recommended).</p> <p> <code>NONE</code>: Ignore UID and GID.</p>",
                     "shape": "Gid"
                 },
                 "LogLevel": {
-                    "documentation": "<p>Specifies the type of logs that DataSync publishes to a Amazon CloudWatch Logs log group. To specify the log group, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/API_CreateTask.html#DataSync-CreateTask-request-CloudWatchLogGroupArn\">CloudWatchLogGroupArn</a>.</p> <ul> <li> <p> <code>BASIC</code> - Publishes logs with only basic information (such as transfer errors).</p> </li> <li> <p> <code>TRANSFER</code> - Publishes logs for all files or objects that your DataSync task transfers and performs data-integrity checks on.</p> </li> <li> <p> <code>OFF</code> - No logs are published.</p> </li> </ul>",
+                    "documentation": "<p>Specifies the type of logs that DataSync publishes to a Amazon CloudWatch Logs log group. To specify the log group, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/API_CreateTask.html#DataSync-CreateTask-request-CloudWatchLogGroupArn\">CloudWatchLogGroupArn</a>.</p> <p>If you set <code>LogLevel</code> to <code>OFF</code>, no logs are published. <code>BASIC</code> publishes logs on errors for individual files transferred. <code>TRANSFER</code> publishes logs for every file or object that is transferred and integrity checked.</p>",
                     "shape": "LogLevel"
                 },
                 "Mtime": {
-                    "documentation": "<p>Specifies whether to preserve metadata indicating the last time that a file was written to before the <code>PREPARING</code> phase of your task execution. This option is required when you need to run the a task more than once.</p> <ul> <li> <p> <code>PRESERVE</code> (default) - Preserves original <code>Mtime</code>, which is recommended.</p> </li> <li> <p> <code>NONE</code> - Ignores <code>Mtime</code>.</p> </li> </ul> <note> <p>If <code>Mtime</code> is set to <code>PRESERVE</code>, <code>Atime</code> must be set to <code>BEST_EFFORT</code>.</p> <p>If <code>Mtime</code> is set to <code>NONE</code>, <code>Atime</code> must also be set to <code>NONE</code>. </p> </note>",
+                    "documentation": "<p>Specifies whether to preserve metadata indicating the last time that a file was written to before the <code>PREPARING</code> phase of your task execution. This option is required when you need to run the a task more than once.</p> <p>Default Value: <code>PRESERVE</code> </p> <p> <code>PRESERVE</code>: Preserve original <code>Mtime</code> (recommended)</p> <p> <code>NONE</code>: Ignore <code>Mtime</code>. </p> <note> <p>If <code>Mtime</code> is set to <code>PRESERVE</code>, <code>Atime</code> must be set to <code>BEST_EFFORT</code>.</p> <p>If <code>Mtime</code> is set to <code>NONE</code>, <code>Atime</code> must also be set to <code>NONE</code>. </p> </note>",
                     "shape": "Mtime"
                 },
                 "ObjectTags": {
-                    "documentation": "<p>Specifies whether you want DataSync to <code>PRESERVE</code> object tags (default behavior) when transferring between object storage systems. If you want your DataSync task to ignore object tags, specify the <code>NONE</code> value.</p>",
+                    "documentation": "<p>Specifies whether object tags are preserved when transferring between object storage systems. If you want your DataSync task to ignore object tags, specify the <code>NONE</code> value.</p> <p>Default Value: <code>PRESERVE</code> </p>",
                     "shape": "ObjectTags"
                 },
                 "OverwriteMode": {
-                    "documentation": "<p>Specifies whether DataSync should modify or preserve data at the destination location.</p> <ul> <li> <p> <code>ALWAYS</code> (default) - DataSync modifies data in the destination location when source data (including metadata) has changed.</p> <p>If DataSync overwrites objects, you might incur additional charges for certain Amazon S3 storage classes (for example, for retrieval or early deletion). For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Storage class considerations with Amazon S3 transfers</a>.</p> </li> <li> <p> <code>NEVER</code> - DataSync doesn't overwrite data in the destination location even if the source data has changed. You can use this option to protect against overwriting changes made to files or objects in the destination.</p> </li> </ul>",
+                    "documentation": "<p>Specifies whether data at the destination location should be overwritten or preserved. If set to <code>NEVER</code>, a destination file for example will not be replaced by a source file (even if the destination file differs from the source file). If you modify files in the destination and you sync the files, you can use this value to protect against overwriting those changes. </p> <p>Some storage classes have specific behaviors that can affect your Amazon S3 storage cost. For detailed information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Considerations when working with Amazon S3 storage classes in DataSync</a>.</p>",
                     "shape": "OverwriteMode"
                 },
                 "PosixPermissions": {
-                    "documentation": "<p>Specifies which users or groups can access a file for a specific purpose such as reading, writing, or execution of the file.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/special-files.html#metadata-copied\">Metadata copied by DataSync</a>.</p> <ul> <li> <p> <code>PRESERVE</code> (default) - Preserves POSIX-style permissions, which is recommended.</p> </li> <li> <p> <code>NONE</code> - Ignores POSIX-style permissions. </p> </li> </ul> <note> <p>DataSync can preserve extant permissions of a source location.</p> </note>",
+                    "documentation": "<p>Specifies which users or groups can access a file for a specific purpose such as reading, writing, or execution of the file.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/special-files.html#metadata-copied\">Metadata copied by DataSync</a>.</p> <p>Default value: <code>PRESERVE</code> </p> <p> <code>PRESERVE</code>: Preserve POSIX-style permissions (recommended).</p> <p> <code>NONE</code>: Ignore permissions. </p> <note> <p>DataSync can preserve extant permissions of a source location.</p> </note>",
                     "shape": "PosixPermissions"
                 },
                 "PreserveDeletedFiles": {
-                    "documentation": "<p>Specifies whether files in the destination location that don't exist in the source should be preserved. This option can affect your Amazon S3 storage cost. If your task deletes objects, you might incur minimum storage duration charges for certain storage classes. For detailed information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Considerations when working with Amazon S3 storage classes in DataSync</a>.</p> <ul> <li> <p> <code>PRESERVE</code> (default) - Ignores such destination files, which is recommended. </p> </li> <li> <p> <code>REMOVE</code> - Deletes destination files that aren\u2019t present in the source.</p> </li> </ul> <note> <p>If you set this parameter to <code>REMOVE</code>, you can't set <code>TransferMode</code> to <code>ALL</code>. When you transfer all data, DataSync doesn't scan your destination location and doesn't know what to delete.</p> </note>",
+                    "documentation": "<p>Specifies whether files in the destination location that don't exist in the source should be preserved. This option can affect your Amazon S3 storage cost. If your task deletes objects, you might incur minimum storage duration charges for certain storage classes. For detailed information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Considerations when working with Amazon S3 storage classes in DataSync</a>.</p> <p>Default value: <code>PRESERVE</code> </p> <p> <code>PRESERVE</code>: Ignore such destination files (recommended). </p> <p> <code>REMOVE</code>: Delete destination files that aren\u2019t present in the source.</p> <note> <p>If you set this parameter to <code>REMOVE</code>, you can't set <code>TransferMode</code> to <code>ALL</code>. When you transfer all data, DataSync doesn't scan your destination location and doesn't know what to delete.</p> </note>",
                     "shape": "PreserveDeletedFiles"
                 },
                 "PreserveDevices": {
-                    "documentation": "<p>Specifies whether DataSync should preserve the metadata of block and character devices in the source location and recreate the files with that device name and metadata on the destination. DataSync copies only the name and metadata of such devices.</p> <note> <p>DataSync can't copy the actual contents of these devices because they're nonterminal and don't return an end-of-file (EOF) marker.</p> </note> <ul> <li> <p> <code>NONE</code> (default) - Ignores special devices (recommended).</p> </li> <li> <p> <code>PRESERVE</code> - Preserves character and block device metadata. This option currently isn't supported for Amazon EFS.</p> </li> </ul>",
+                    "documentation": "<p>Specifies whether DataSync should preserve the metadata of block and character devices in the source location and recreate the files with that device name and metadata on the destination. DataSync copies only the name and metadata of such devices.</p> <note> <p>DataSync can't copy the actual contents of these devices because they're nonterminal and don't return an end-of-file (EOF) marker.</p> </note> <p>Default value: <code>NONE</code> </p> <p> <code>NONE</code>: Ignore special devices (recommended). </p> <p> <code>PRESERVE</code>: Preserve character and block device metadata. This option currently isn't supported for Amazon EFS. </p>",
                     "shape": "PreserveDevices"
                 },
                 "SecurityDescriptorCopyFlags": {
-                    "documentation": "<p>Specifies which components of the SMB security descriptor are copied from source to destination objects. </p> <p>This value is only used for transfers between SMB and Amazon FSx for Windows File Server locations or between two FSx for Windows File Server locations. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/special-files.html\">how DataSync handles metadata</a>.</p> <ul> <li> <p> <code>OWNER_DACL</code> (default) - For each copied object, DataSync copies the following metadata:</p> <ul> <li> <p>The object owner.</p> </li> <li> <p>NTFS discretionary access control lists (DACLs), which determine whether to grant access to an object.</p> <p>DataSync won't copy NTFS system access control lists (SACLs) with this option.</p> </li> </ul> </li> <li> <p> <code>OWNER_DACL_SACL</code> - For each copied object, DataSync copies the following metadata:</p> <ul> <li> <p>The object owner.</p> </li> <li> <p>NTFS discretionary access control lists (DACLs), which determine whether to grant access to an object.</p> </li> <li> <p>SACLs, which are used by administrators to log attempts to access a secured object.</p> <p>Copying SACLs requires granting additional permissions to the Windows user that DataSync uses to access your SMB location. For information about choosing a user with the right permissions, see required permissions for <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-smb-location.html#configuring-smb-permissions\">SMB</a>, <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-fsx-location.html#create-fsx-windows-location-permissions\">FSx for Windows File Server</a>, or <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-ontap-location.html#create-ontap-location-smb\">FSx for ONTAP</a> (depending on the type of location in your transfer).</p> </li> </ul> </li> <li> <p> <code>NONE</code> - None of the SMB security descriptor components are copied. Destination objects are owned by the user that was provided for accessing the destination location. DACLs and SACLs are set based on the destination server\u2019s configuration. </p> </li> </ul>",
+                    "documentation": "<p>Specifies which components of the SMB security descriptor are copied from source to destination objects. </p> <p>This value is only used for transfers between SMB and Amazon FSx for Windows File Server locations or between two FSx for Windows File Server locations. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/special-files.html\">how DataSync handles metadata</a>.</p> <p>Default value: <code>OWNER_DACL</code> </p> <p> <code>OWNER_DACL</code>: For each copied object, DataSync copies the following metadata:</p> <ul> <li> <p>The object owner.</p> </li> <li> <p>NTFS discretionary access control lists (DACLs), which determine whether to grant access to an object.</p> <p>DataSync won't copy NTFS system access control lists (SACLs) with this option.</p> </li> </ul> <p> <code>OWNER_DACL_SACL</code>: For each copied object, DataSync copies the following metadata:</p> <ul> <li> <p>The object owner.</p> </li> <li> <p>NTFS discretionary access control lists (DACLs), which determine whether to grant access to an object.</p> </li> <li> <p>SACLs, which are used by administrators to log attempts to access a secured object.</p> <p>Copying SACLs requires granting additional permissions to the Windows user that DataSync uses to access your SMB location. For information about choosing a user that ensures sufficient permissions to files, folders, and metadata, see <a href=\"create-smb-location.html#SMBuser\">user</a>.</p> </li> </ul> <p> <code>NONE</code>: None of the SMB security descriptor components are copied. Destination objects are owned by the user that was provided for accessing the destination location. DACLs and SACLs are set based on the destination server\u2019s configuration. </p>",
                     "shape": "SmbSecurityDescriptorCopyFlags"
                 },
                 "TaskQueueing": {
                     "documentation": "<p>Specifies whether your transfer tasks should be put into a queue during certain scenarios when <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/run-task.html#running-multiple-tasks\">running multiple tasks</a>. This is <code>ENABLED</code> by default.</p>",
                     "shape": "TaskQueueing"
                 },
                 "TransferMode": {
-                    "documentation": "<p>Determines whether DataSync transfers only the data and metadata that differ between the source and the destination location or transfers all the content from the source (without comparing what's in the destination).</p> <ul> <li> <p> <code>CHANGED</code> (default) - DataSync copies only data or metadata that is new or different content from the source location to the destination location.</p> </li> <li> <p> <code>ALL</code> - DataSync copies everything in the source to the destination without comparing differences between the locations.</p> </li> </ul>",
+                    "documentation": "<p>Determines whether DataSync transfers only the data and metadata that differ between the source and the destination location or transfers all the content from the source (without comparing what's in the destination).</p> <p> <code>CHANGED</code>: DataSync copies only data or metadata that is new or different content from the source location to the destination location.</p> <p> <code>ALL</code>: DataSync copies all source location content to the destination (without comparing what's in the destination).</p>",
                     "shape": "TransferMode"
                 },
                 "Uid": {
-                    "documentation": "<p>Specifies the POSIX user ID (UID) of the file's owner.</p> <ul> <li> <p> <code>INT_VALUE</code> (default) - Preserves the integer value of UID and group ID (GID), which is recommended.</p> </li> <li> <p> <code>NONE</code> - Ignores UID and GID. </p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/special-files.html#metadata-copied\">Metadata copied by DataSync</a>.</p>",
+                    "documentation": "<p>Specifies the POSIX user ID (UID) of the file's owner.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/special-files.html#metadata-copied\">Metadata copied by DataSync</a>.</p> <p>Default value: <code>INT_VALUE</code>. This preserves the integer value of the ID.</p> <p> <code>INT_VALUE</code>: Preserve the integer value of UID and group ID (GID) (recommended).</p> <p> <code>NONE</code>: Ignore UID and GID. </p>",
                     "shape": "Uid"
                 },
                 "VerifyMode": {
-                    "documentation": "<p>Specifies how and when DataSync checks the integrity of your data during a transfer.</p> <ul> <li> <p> <code>ONLY_FILES_TRANSFERRED</code> (recommended) - DataSync calculates the checksum of transferred files and metadata at the source location. At the end of the transfer, DataSync then compares this checksum to the checksum calculated on those files at the destination.</p> <p>We recommend this option when transferring to S3 Glacier Flexible Retrieval or S3 Glacier Deep Archive storage classes. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Storage class considerations with Amazon S3 locations</a>.</p> </li> <li> <p> <code>POINT_IN_TIME_CONSISTENT</code> (default) - At the end of the transfer, DataSync scans the entire source and destination to verify that both locations are fully synchronized.</p> <p>You can't use this option when transferring to S3 Glacier Flexible Retrieval or S3 Glacier Deep Archive storage classes. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Storage class considerations with Amazon S3 locations</a>.</p> </li> <li> <p> <code>NONE</code> - DataSync doesn't run additional verification at the end of the transfer. All data transmissions are still integrity-checked with checksum verification during the transfer.</p> </li> </ul>",
+                    "documentation": "<p>Specifies how and when DataSync checks the integrity of your data during a transfer. </p> <p>Default value: <code>POINT_IN_TIME_CONSISTENT</code> </p> <p> <code>ONLY_FILES_TRANSFERRED</code> (recommended): DataSync calculates the checksum of transferred files and metadata at the source location. At the end of the transfer, DataSync then compares this checksum to the checksum calculated on those files at the destination.</p> <p>We recommend this option when transferring to S3 Glacier Flexible Retrieval or S3 Glacier Deep Archive storage classes. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Storage class considerations with Amazon S3 locations</a>.</p> <p> <code>POINT_IN_TIME_CONSISTENT</code>: At the end of the transfer, DataSync scans the entire source and destination to verify that both locations are fully synchronized.</p> <p>You can't use this option when transferring to S3 Glacier Flexible Retrieval or S3 Glacier Deep Archive storage classes. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#using-storage-classes\">Storage class considerations with Amazon S3 locations</a>.</p> <p> <code>NONE</code>: DataSync doesn't run additional verification at the end of the transfer. All data transmissions are still integrity-checked with checksum verification during the transfer.</p>",
                     "shape": "VerifyMode"
                 }
             },
             "type": "structure"
         },
         "OutputTagList": {
             "max": 55,
@@ -4617,15 +4575,15 @@
             ],
             "type": "string"
         },
         "Platform": {
             "documentation": "<p>The platform-related details about the DataSync agent, such as the version number.</p>",
             "members": {
                 "Version": {
-                    "documentation": "<p>The version of the DataSync agent.</p> <important> <p>On December 7, 2023, we discontinued version 1 DataSync agents. Check the DataSync console to see if you have affected agents. If you do, <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/replacing-agent.html\">replace</a> those agents or <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/deleting-agent.html\">delete</a> them if they aren't in use. If you need more help, contact <a href=\"https://aws.amazon.com/contact-us/\">Amazon Web Services Support</a>.</p> </important>",
+                    "documentation": "<p>The version of the DataSync agent.</p> <important> <p>Beginning December 7, 2023, we will discontinue version 1 DataSync agents. Check the DataSync console to see if you have affected agents. If you do, <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/replacing-agent.html\">replace</a> those agents before then to avoid data transfer or storage discovery disruptions. If you need more help, contact <a href=\"https://aws.amazon.com/contact-us/\">Amazon Web Services Support</a>.</p> </important>",
                     "shape": "AgentVersion"
                 }
             },
             "type": "structure"
         },
         "PosixPermissions": {
             "enum": [
@@ -4776,15 +4734,15 @@
             },
             "type": "structure"
         },
         "ReportDestinationS3": {
             "documentation": "<p>Specifies the Amazon S3 bucket where DataSync uploads your <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/task-reports.html\">task report</a>.</p>",
             "members": {
                 "BucketAccessRoleArn": {
-                    "documentation": "<p>Specifies the Amazon Resource Name (ARN) of the IAM policy that allows DataSync to upload a task report to your S3 bucket. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/task-reports.html\">Allowing DataSync to upload a task report to an Amazon S3 bucket</a>.</p>",
+                    "documentation": "<p>Specifies the Amazon Resource Name (ARN) of the IAM policy that allows DataSync to upload a task report to your S3 bucket. For more information, see <a href=\"https://docs.aws.amazon.com/https:/docs.aws.amazon.com/datasync/latest/userguide/task-reports.html\">Allowing DataSync to upload a task report to an Amazon S3 bucket</a>.</p>",
                     "shape": "IamRoleArn"
                 },
                 "S3BucketArn": {
                     "documentation": "<p>Specifies the ARN of the S3 bucket where DataSync uploads your report.</p>",
                     "shape": "S3BucketArn"
                 },
                 "Subdirectory": {
@@ -4929,59 +4887,26 @@
         },
         "S3BucketArn": {
             "max": 156,
             "pattern": "^arn:(aws|aws-cn|aws-us-gov|aws-iso|aws-iso-b):(s3|s3-outposts):[a-z\\-0-9]*:[0-9]*:.*$",
             "type": "string"
         },
         "S3Config": {
-            "documentation": "<p>Specifies the Amazon Resource Name (ARN) of the Identity and Access Management (IAM) role that DataSync uses to access your S3 bucket.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-s3-location.html#create-s3-location-access\">Accessing S3 buckets</a>.</p>",
+            "documentation": "<p>The Amazon Resource Name (ARN) of the Identity and Access Management (IAM) role used to access an Amazon S3 bucket.</p> <p>For detailed information about using such a role, see Creating a Location for Amazon S3 in the <i>DataSync User Guide</i>.</p>",
             "members": {
                 "BucketAccessRoleArn": {
-                    "documentation": "<p>Specifies the ARN of the IAM role that DataSync uses to access your S3 bucket.</p>",
+                    "documentation": "<p>The ARN of the IAM role for accessing the S3 bucket. </p>",
                     "shape": "IamRoleArn"
                 }
             },
             "required": [
                 "BucketAccessRoleArn"
             ],
             "type": "structure"
         },
-        "S3ManifestConfig": {
-            "documentation": "<p>Specifies the S3 bucket where you're hosting the manifest that you want DataSync to use. For more information and configuration examples, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/transferring-with-manifest.html\">Specifying what DataSync transfers by using a manifest</a>.</p>",
-            "members": {
-                "BucketAccessRoleArn": {
-                    "documentation": "<p>Specifies the Identity and Access Management (IAM) role that allows DataSync to access your manifest. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/transferring-with-manifest.html#transferring-with-manifest-access\">Providing DataSync access to your manifest</a>.</p>",
-                    "shape": "IamRoleArn"
-                },
-                "ManifestObjectPath": {
-                    "documentation": "<p>Specifies the Amazon S3 object key of your manifest. This can include a prefix (for example, <code>prefix/my-manifest.csv</code>).</p>",
-                    "shape": "S3Subdirectory"
-                },
-                "ManifestObjectVersionId": {
-                    "documentation": "<p>Specifies the object version ID of the manifest that you want DataSync to use. If you don't set this, DataSync uses the latest version of the object.</p>",
-                    "shape": "S3ObjectVersionId"
-                },
-                "S3BucketArn": {
-                    "documentation": "<p>Specifies the Amazon Resource Name (ARN) of the S3 bucket where you're hosting your manifest.</p>",
-                    "shape": "S3BucketArn"
-                }
-            },
-            "required": [
-                "ManifestObjectPath",
-                "BucketAccessRoleArn",
-                "S3BucketArn"
-            ],
-            "type": "structure"
-        },
-        "S3ObjectVersionId": {
-            "max": 100,
-            "min": 1,
-            "pattern": "^.+$",
-            "type": "string"
-        },
         "S3StorageClass": {
             "enum": [
                 "STANDARD",
                 "STANDARD_IA",
                 "ONEZONE_IA",
                 "INTELLIGENT_TIERING",
                 "GLACIER",
@@ -5056,27 +4981,14 @@
                 "SMB2",
                 "SMB3",
                 "SMB1",
                 "SMB2_0"
             ],
             "type": "string"
         },
-        "SourceManifestConfig": {
-            "documentation": "<p>Specifies the manifest that you want DataSync to use and where it's hosted. For more information and configuration examples, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/transferring-with-manifest.html\">Specifying what DataSync transfers by using a manifest</a>.</p>",
-            "members": {
-                "S3": {
-                    "documentation": "<p>Specifies the S3 bucket where you're hosting your manifest.</p>",
-                    "shape": "S3ManifestConfig"
-                }
-            },
-            "required": [
-                "S3"
-            ],
-            "type": "structure"
-        },
         "SourceNetworkInterfaceArns": {
             "member": {
                 "shape": "NetworkInterfaceArn"
             },
             "type": "list"
         },
         "StartDiscoveryJobRequest": {
@@ -5122,31 +5034,27 @@
                     "documentation": "<p>Specifies a list of filter rules that determines which files to exclude from a task. The list contains a single filter string that consists of the patterns to exclude. The patterns are delimited by \"|\" (that is, a pipe), for example, <code>\"/folder1|/folder2\"</code>. </p>",
                     "shape": "FilterList"
                 },
                 "Includes": {
                     "documentation": "<p>Specifies a list of filter rules that determines which files to include when running a task. The pattern should contain a single filter string that consists of the patterns to include. The patterns are delimited by \"|\" (that is, a pipe), for example, <code>\"/folder1|/folder2\"</code>. </p>",
                     "shape": "FilterList"
                 },
-                "ManifestConfig": {
-                    "documentation": "<p>Configures a manifest, which is a list of files or objects that you want DataSync to transfer. For more information and configuration examples, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/transferring-with-manifest.html\">Specifying what DataSync transfers by using a manifest</a>.</p> <p>When using this parameter, your caller identity (the role that you're using DataSync with) must have the <code>iam:PassRole</code> permission. The <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/security-iam-awsmanpol.html#security-iam-awsmanpol-awsdatasyncfullaccess\">AWSDataSyncFullAccess</a> policy includes this permission.</p> <p>To remove a manifest configuration, specify this parameter with an empty value.</p>",
-                    "shape": "ManifestConfig"
-                },
                 "OverrideOptions": {
                     "shape": "Options"
                 },
                 "Tags": {
                     "documentation": "<p>Specifies the tags that you want to apply to the Amazon Resource Name (ARN) representing the task execution.</p> <p> <i>Tags</i> are key-value pairs that help you manage, filter, and search for your DataSync resources.</p>",
                     "shape": "InputTagList"
                 },
                 "TaskArn": {
                     "documentation": "<p>Specifies the Amazon Resource Name (ARN) of the task that you want to start.</p>",
                     "shape": "TaskArn"
                 },
                 "TaskReportConfig": {
-                    "documentation": "<p>Specifies how you want to configure a task report, which provides detailed information about your DataSync transfer. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/task-reports.html\">Monitoring your DataSync transfers with task reports</a>.</p> <p>When using this parameter, your caller identity (the role that you're using DataSync with) must have the <code>iam:PassRole</code> permission. The <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/security-iam-awsmanpol.html#security-iam-awsmanpol-awsdatasyncfullaccess\">AWSDataSyncFullAccess</a> policy includes this permission.</p> <p>To remove a task report configuration, specify this parameter as empty.</p>",
+                    "documentation": "<p>Specifies how you want to configure a task report, which provides detailed information about for your DataSync transfer.</p>",
                     "shape": "TaskReportConfig"
                 }
             },
             "required": [
                 "TaskArn"
             ],
             "type": "structure"
@@ -5292,22 +5200,22 @@
         "TaskExecutionList": {
             "member": {
                 "shape": "TaskExecutionListEntry"
             },
             "type": "list"
         },
         "TaskExecutionListEntry": {
-            "documentation": "<p>Represents a single entry in a list of DataSync task executions that's returned with the <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/API_ListTaskExecutions.html\">ListTaskExecutions</a> operation.</p>",
+            "documentation": "<p>Represents a single entry in a list of task executions. <code>TaskExecutionListEntry</code> returns an array that contains a list of specific invocations of a task when the <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/API_ListTaskExecutions.html\">ListTaskExecutions</a> operation is called.</p>",
             "members": {
                 "Status": {
-                    "documentation": "<p>The status of a task execution. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/understand-task-statuses.html#understand-task-execution-statuses\">Task execution statuses</a>.</p>",
+                    "documentation": "<p>The status of a task execution.</p>",
                     "shape": "TaskExecutionStatus"
                 },
                 "TaskExecutionArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of a task execution.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the task that was executed.</p>",
                     "shape": "TaskExecutionArn"
                 }
             },
             "type": "structure"
         },
         "TaskExecutionResultDetail": {
             "documentation": "<p>Describes the detailed result of a <code>TaskExecution</code> operation. This result includes the time in milliseconds spent in each phase, the status of the task execution, and the errors encountered.</p>",
@@ -5867,18 +5775,14 @@
                     "documentation": "<p>Specifies a list of filter rules that exclude specific data during your transfer. For more information and examples, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/filtering.html\">Filtering data transferred by DataSync</a>.</p>",
                     "shape": "FilterList"
                 },
                 "Includes": {
                     "documentation": "<p>Specifies a list of filter rules that include specific data during your transfer. For more information and examples, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/filtering.html\">Filtering data transferred by DataSync</a>.</p>",
                     "shape": "FilterList"
                 },
-                "ManifestConfig": {
-                    "documentation": "<p>Configures a manifest, which is a list of files or objects that you want DataSync to transfer. For more information and configuration examples, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/transferring-with-manifest.html\">Specifying what DataSync transfers by using a manifest</a>.</p> <p>When using this parameter, your caller identity (the IAM role that you're using DataSync with) must have the <code>iam:PassRole</code> permission. The <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/security-iam-awsmanpol.html#security-iam-awsmanpol-awsdatasyncfullaccess\">AWSDataSyncFullAccess</a> policy includes this permission.</p> <p>To remove a manifest configuration, specify this parameter as empty.</p>",
-                    "shape": "ManifestConfig"
-                },
                 "Name": {
                     "documentation": "<p>The name of the task to update.</p>",
                     "shape": "TagValue"
                 },
                 "Options": {
                     "shape": "Options"
                 },
@@ -5887,15 +5791,15 @@
                     "shape": "TaskSchedule"
                 },
                 "TaskArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the resource name of the task to update.</p>",
                     "shape": "TaskArn"
                 },
                 "TaskReportConfig": {
-                    "documentation": "<p>Specifies how you want to configure a task report, which provides detailed information about your DataSync transfer. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/task-reports.html\">Monitoring your DataSync transfers with task reports</a>.</p> <p>When using this parameter, your caller identity (the IAM role that you're using DataSync with) must have the <code>iam:PassRole</code> permission. The <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/security-iam-awsmanpol.html#security-iam-awsmanpol-awsdatasyncfullaccess\">AWSDataSyncFullAccess</a> policy includes this permission.</p> <p>To remove a task report configuration, specify this parameter as empty.</p>",
+                    "documentation": "<p>Specifies how you want to configure a task report, which provides detailed information about for your DataSync transfer.</p>",
                     "shape": "TaskReportConfig"
                 }
             },
             "required": [
                 "TaskArn"
             ],
             "type": "structure"
```

### Comparing `botocore-a-la-carte-datasync-1.34.82/botocore_a_la_carte_datasync.egg-info/PKG-INFO` & `botocore-a-la-carte-datasync-1.34.9/botocore_a_la_carte_datasync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-datasync
-Version: 1.34.82
+Version: 1.34.9
 Summary: datasync data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-datasync-1.34.82/setup.py` & `botocore-a-la-carte-datasync-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-datasync',
-    version="1.34.82",
+    version="1.34.9",
     description='datasync data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/datasync/*/*.json'],
```

