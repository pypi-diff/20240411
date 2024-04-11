# Comparing `tmp/modelbest_sdk-0.1.2.tar.gz` & `tmp/modelbest_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelbest_sdk-0.1.2.tar", last modified: Tue Apr  9 08:09:40 2024, max compression
+gzip compressed data, was "modelbest_sdk-0.1.3.tar", last modified: Thu Apr 11 13:44:00 2024, max compression
```

## Comparing `modelbest_sdk-0.1.2.tar` & `modelbest_sdk-0.1.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.941722 modelbest_sdk-0.1.2/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       99 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.2/MANIFEST.in
--rw-r--r--   0 emr-user  (1000) emr-user  (1000)      984 2024-04-09 08:09:40.941722 modelbest_sdk-0.1.2/PKG-INFO
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      488 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/README.md
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.929721 modelbest_sdk-0.1.2/modelbest_sdk/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/modelbest_sdk/__init__.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.931722 modelbest_sdk-0.1.2/modelbest_sdk/dataset/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/__init__.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2606 2024-04-03 09:06:32.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/cache.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.931722 modelbest_sdk-0.1.2/modelbest_sdk/dataset/collater/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:33:51.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/collater/__init__.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4909 2024-04-09 08:07:57.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/collater/batched_dataset.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       53 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/collater/collater.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3241 2024-04-03 08:49:54.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/cuda_prefetcher.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     7949 2024-04-07 07:50:10.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/mbtable_iterable_dataset.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2667 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/range.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.931722 modelbest_sdk-0.1.2/modelbest_sdk/dataset/sampler/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:33:51.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/sampler/__init__.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       56 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/sampler/sampler.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3980 2024-04-07 07:47:05.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/sampler/weighted_dataset.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3531 2024-04-08 12:38:43.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/table_record_dataset.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.932722 modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:53:00.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/__init__.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1928 2024-04-08 08:15:10.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/base_doc.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     7606 2024-04-08 12:19:40.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2220 2024-04-03 09:25:49.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      896 2024-04-03 07:56:34.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/utils.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      464 2024-04-08 12:39:26.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/utils.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.932722 modelbest_sdk-0.1.2/modelbest_sdk/file_format/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/modelbest_sdk/file_format/__init__.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.932722 modelbest_sdk-0.1.2/modelbest_sdk/file_format/lib/
--rwxrwxr-x   0 emr-user  (1000) emr-user  (1000)  7114128 2024-03-26 09:17:44.000000 modelbest_sdk-0.1.2/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4768 2024-03-29 10:09:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/file_format/mbtable.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2895 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/modelbest_sdk/file_format/mbtable_builder.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4699 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.2/modelbest_sdk/file_format/mbtable_partition.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.940722 modelbest_sdk-0.1.2/modelbest_sdk/proto/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      405 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/breadcrumb.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3060 2024-04-02 07:22:05.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/chatdoc.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1136 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/const.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      830 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/context.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3846 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/data_base.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      631 2024-03-29 12:04:58.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/dataset_checkpoint.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      454 2024-04-03 08:15:57.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/dataset_context.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1806 2024-03-28 08:57:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/general_doc.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1624 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/general_servlet_rpc.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3408 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/linkinfo.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1501 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/mergeddoc.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      477 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/traindoc.thrift
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.930722 modelbest_sdk-0.1.2/modelbest_sdk.egg-info/
--rw-r--r--   0 emr-user  (1000) emr-user  (1000)      984 2024-04-09 08:09:40.000000 modelbest_sdk-0.1.2/modelbest_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1842 2024-04-09 08:09:40.000000 modelbest_sdk-0.1.2/modelbest_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        1 2024-04-09 08:09:40.000000 modelbest_sdk-0.1.2/modelbest_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       19 2024-04-09 08:09:40.000000 modelbest_sdk-0.1.2/modelbest_sdk.egg-info/top_level.txt
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       38 2024-04-09 08:09:40.941722 modelbest_sdk-0.1.2/setup.cfg
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      708 2024-04-09 08:09:34.000000 modelbest_sdk-0.1.2/setup.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.941722 modelbest_sdk-0.1.2/test/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-03-01 08:13:07.000000 modelbest_sdk-0.1.2/test/__init__.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1158 2024-04-03 09:13:40.000000 modelbest_sdk-0.1.2/test/dataset_context_test.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1209 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.2/test/generate_data.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4115 2024-04-08 12:42:07.000000 modelbest_sdk-0.1.2/test/test_base.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2289 2024-04-09 08:09:00.000000 modelbest_sdk-0.1.2/test/test_checkpoint.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2682 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/test/test_mbtable.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2248 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/test/test_mbtable_partition.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-11 13:44:00.742906 modelbest_sdk-0.1.3/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       99 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.3/MANIFEST.in
+-rw-r--r--   0 emr-user  (1000) emr-user  (1000)      984 2024-04-11 13:44:00.741906 modelbest_sdk-0.1.3/PKG-INFO
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      488 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.3/README.md
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-11 13:44:00.730906 modelbest_sdk-0.1.3/modelbest_sdk/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.3/modelbest_sdk/__init__.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-11 13:44:00.731906 modelbest_sdk-0.1.3/modelbest_sdk/dataset/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/__init__.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2606 2024-04-03 09:06:32.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/cache.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-11 13:44:00.732905 modelbest_sdk-0.1.3/modelbest_sdk/dataset/collater/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:33:51.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/collater/__init__.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4909 2024-04-09 08:07:57.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/collater/batched_dataset.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       53 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/collater/collater.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3241 2024-04-03 08:49:54.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/cuda_prefetcher.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)    11065 2024-04-11 13:41:22.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/mbtable_iterable_dataset.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2667 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/range.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-11 13:44:00.732905 modelbest_sdk-0.1.3/modelbest_sdk/dataset/sampler/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:33:51.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/sampler/__init__.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       56 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/sampler/sampler.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4034 2024-04-11 11:13:12.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/sampler/weighted_dataset.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3898 2024-04-11 13:26:10.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/table_record_dataset.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-11 13:44:00.733906 modelbest_sdk-0.1.3/modelbest_sdk/dataset/thrift_wrapper/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:53:00.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/thrift_wrapper/__init__.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1928 2024-04-08 08:15:10.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/thrift_wrapper/base_doc.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     7642 2024-04-11 12:43:34.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2220 2024-04-03 09:25:49.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      896 2024-04-03 07:56:34.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/thrift_wrapper/utils.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      464 2024-04-08 12:39:26.000000 modelbest_sdk-0.1.3/modelbest_sdk/dataset/utils.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-11 13:44:00.733906 modelbest_sdk-0.1.3/modelbest_sdk/file_format/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.3/modelbest_sdk/file_format/__init__.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-11 13:44:00.733906 modelbest_sdk-0.1.3/modelbest_sdk/file_format/lib/
+-rwxrwxr-x   0 emr-user  (1000) emr-user  (1000)  7114128 2024-03-26 09:17:44.000000 modelbest_sdk-0.1.3/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4760 2024-04-11 09:53:30.000000 modelbest_sdk-0.1.3/modelbest_sdk/file_format/mbtable.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2895 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.3/modelbest_sdk/file_format/mbtable_builder.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4699 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.3/modelbest_sdk/file_format/mbtable_partition.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-11 13:44:00.740906 modelbest_sdk-0.1.3/modelbest_sdk/proto/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      405 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.3/modelbest_sdk/proto/breadcrumb.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3060 2024-04-02 07:22:05.000000 modelbest_sdk-0.1.3/modelbest_sdk/proto/chatdoc.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1136 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.3/modelbest_sdk/proto/const.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      830 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.3/modelbest_sdk/proto/context.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3846 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.3/modelbest_sdk/proto/data_base.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      631 2024-03-29 12:04:58.000000 modelbest_sdk-0.1.3/modelbest_sdk/proto/dataset_checkpoint.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      454 2024-04-03 08:15:57.000000 modelbest_sdk-0.1.3/modelbest_sdk/proto/dataset_context.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1806 2024-03-28 08:57:29.000000 modelbest_sdk-0.1.3/modelbest_sdk/proto/general_doc.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1624 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.3/modelbest_sdk/proto/general_servlet_rpc.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3408 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.3/modelbest_sdk/proto/linkinfo.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1501 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.3/modelbest_sdk/proto/mergeddoc.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      477 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.3/modelbest_sdk/proto/traindoc.thrift
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-11 13:44:00.731906 modelbest_sdk-0.1.3/modelbest_sdk.egg-info/
+-rw-r--r--   0 emr-user  (1000) emr-user  (1000)      984 2024-04-11 13:44:00.000000 modelbest_sdk-0.1.3/modelbest_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1842 2024-04-11 13:44:00.000000 modelbest_sdk-0.1.3/modelbest_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        1 2024-04-11 13:44:00.000000 modelbest_sdk-0.1.3/modelbest_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       19 2024-04-11 13:44:00.000000 modelbest_sdk-0.1.3/modelbest_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       38 2024-04-11 13:44:00.742906 modelbest_sdk-0.1.3/setup.cfg
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      708 2024-04-11 13:43:58.000000 modelbest_sdk-0.1.3/setup.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-11 13:44:00.741906 modelbest_sdk-0.1.3/test/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-03-01 08:13:07.000000 modelbest_sdk-0.1.3/test/__init__.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1158 2024-04-03 09:13:40.000000 modelbest_sdk-0.1.3/test/dataset_context_test.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1209 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.3/test/generate_data.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4104 2024-04-11 13:09:33.000000 modelbest_sdk-0.1.3/test/test_base.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4660 2024-04-11 13:36:10.000000 modelbest_sdk-0.1.3/test/test_checkpoint.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2682 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.3/test/test_mbtable.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2248 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.3/test/test_mbtable_partition.py
```

### Comparing `modelbest_sdk-0.1.2/PKG-INFO` & `modelbest_sdk-0.1.3/modelbest_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: modelbest_sdk
-Version: 0.1.2
+Name: modelbest-sdk
+Version: 0.1.3
 Summary: Everything about modelbest data include data format mbtable, dataset, dataloader, and tools
 Home-page: https://codeup.aliyun.com/64ddb0a87f62ff9b3d23ca15/modelbest_sdk
 Author: HankyZhao
 Author-email: zhq980115@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/dataset/cache.py` & `modelbest_sdk-0.1.3/modelbest_sdk/dataset/cache.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/dataset/collater/batched_dataset.py` & `modelbest_sdk-0.1.3/modelbest_sdk/dataset/collater/batched_dataset.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/dataset/cuda_prefetcher.py` & `modelbest_sdk-0.1.3/modelbest_sdk/dataset/cuda_prefetcher.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/dataset/range.py` & `modelbest_sdk-0.1.3/modelbest_sdk/dataset/range.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/dataset/sampler/weighted_dataset.py` & `modelbest_sdk-0.1.3/modelbest_sdk/dataset/sampler/weighted_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import numpy as np
 import torch
 from modelbest_sdk.dataset.mbtable_iterable_dataset import MBTableIterableDataset
 # from modelbest_sdk.dataset.sampler.sampler import Sampler
 from modelbest_sdk.dataset.thrift_wrapper.dataset_checkpoint import *
 from modelbest_sdk.dataset.thrift_wrapper.dataset_context import DatasetContext
 
+logger = logging.getLogger(__name__)
+
 MAX_EPOCH = 2**31 - 1
 
 class WeightedDataset(torch.utils.data.IterableDataset):
     def __init__(
         self, 
         context: DatasetContext, 
         dataset_info_list: DatasetInfoList,
@@ -38,26 +40,26 @@
                 prefetch_chunk_cnt=prefetch_chunk_cnt,
                 chunk_size=chunk_size
             )
             self.datasets.append(dataset)
             weights.append(weight)
         weights = np.array(weights)
         self.dataset_weights = weights / weights.sum()
-        self.remain = len(self.datasets)
             
     def sample(self) -> int:
         choice = np.random.choice(len(self.dataset_weights), p=self.dataset_weights)
         return choice
     
     def __iter__(self):
         for dataset in self.datasets:
             self.datasets_iter.append(iter(dataset))
+        self.set_seed()
         while True:
             if all(d.exhausted for d in self.datasets):
-                print(f"All dataset exhaust on rank {self.context.rank}")
+                logger.warning(f"All dataset exhaust on rank {self.context.rank}")
                 break
             idx = self.sample()
             if self.datasets[idx].exhausted:
                 print(f"Dataset {idx} exhaust on rank {self.context.rank}")
                 continue
             chosen_iter = self.datasets_iter[idx]
             try:
@@ -66,17 +68,16 @@
                     continue
                 data['dataset_idx'] = idx
                 yield data
             except StopIteration:
                 continue
 
 
-    def set_seed():
-        # TODO: implement set_seed
-        pass
+    def set_seed(self):
+        np.random.seed(self.context.world_size + self.context.rank)
     
     def checkpoint(self):
         checkpoint_list = [dataset.checkpoint() for dataset in self.datasets]
         return DatasetCheckpointList(
             checkpoint_list=checkpoint_list,
             world_size=self.context.world_size,
             tp_size=self.context.tp_size
```

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/dataset/table_record_dataset.py` & `modelbest_sdk-0.1.3/modelbest_sdk/dataset/table_record_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         prefetch_chunk_cnt=20,
         chunk_size=1024,
         num_workers=1,
         prefetch_factor=20,
         cuda_prefetch=True
     ):
         self.context = context
+        self.context.num_workers = num_workers
         dataset_info_list = DatasetInfoList.load_from_file(context.dataset_config_path)
         
         self.weighted_dataset = WeightedDataset(
             context=context, 
             dataset_info_list=dataset_info_list,
             prefetch_chunk_cnt=prefetch_chunk_cnt,
             chunk_size=chunk_size
@@ -70,21 +71,27 @@
         self.weighted_dataset.update(dataset_entries)
     
     def save(self):
         path = os.path.join(self.context.dataset_checkpoint_path, f"dataset_ckpt_rank_{self.context.rank}.mbt")
         self.checkpoint().save_to_file(path)
         
     def resume(self):
+        # if dir empty, return
+        if not os.path.exists(self.context.dataset_checkpoint_path):
+            return
+        if os.listdir(self.context.dataset_checkpoint_path) == []:
+            return
         new_world_size = self.context.world_size
         first_rank_ckpt_path = os.path.join(self.context.dataset_checkpoint_path, f"dataset_ckpt_rank_0.mbt")
         cur_rank_ckpt_path = os.path.join(self.context.dataset_checkpoint_path, f"dataset_ckpt_rank_{self.context.rank}.mbt")
         old_world_size = DatasetCheckpointList.load_from_file(first_rank_ckpt_path).world_size
         if new_world_size == old_world_size:
             self.weighted_dataset.load_checkpoint(DatasetCheckpointList.load_from_file(cur_rank_ckpt_path))
         else:
+            print(f"Warning: world size changed from {old_world_size} to {new_world_size}, resuming from scratch")
             merged_ckpt = None
             for path in os.listdir(self.context.dataset_checkpoint_path):
                 abs_path = os.path.join(self.context.dataset_checkpoint_path, path)
                 if merged_ckpt is None:
                     merged_ckpt = DatasetCheckpointList.load_from_file(abs_path)
                 else:
                     merged_ckpt.merge(DatasetCheckpointList.load_from_file(abs_path))
```

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/base_doc.py` & `modelbest_sdk-0.1.3/modelbest_sdk/dataset/thrift_wrapper/base_doc.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py` & `modelbest_sdk-0.1.3/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import defaultdict
 import logging
 from typing import Dict, List, Set
 import thriftpy2
 from thriftpy2.utils import deserialize, serialize
 import os
 
 from modelbest_sdk.dataset.thrift_wrapper.utils import Utils
```

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py` & `modelbest_sdk-0.1.3/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/utils.py` & `modelbest_sdk-0.1.3/modelbest_sdk/dataset/thrift_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so` & `modelbest_sdk-0.1.3/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/file_format/mbtable.py` & `modelbest_sdk-0.1.3/modelbest_sdk/file_format/mbtable.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             retry += 1
             print('Failed to open mbtable, retrying in 5 second')
             import time
             import random
             time.sleep(random.randint(1, 5))
             self.handle = lib.MbTableOpen(self.path.encode('utf-8'))
         if not self.handle:
-            raise Exception('Failed to open mbtable after {} retries'.format(self.max_retry))
+            raise Exception(f'Failed to open mbtable after {self.max_retry} retries')
 
         return self.handle
 
     def read(self, index):
         '''
         only use this method if you seek few non-sequential records, otherwise use iterator
         '''
```

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/file_format/mbtable_builder.py` & `modelbest_sdk-0.1.3/modelbest_sdk/file_format/mbtable_builder.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/file_format/mbtable_partition.py` & `modelbest_sdk-0.1.3/modelbest_sdk/file_format/mbtable_partition.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/proto/chatdoc.thrift` & `modelbest_sdk-0.1.3/modelbest_sdk/proto/chatdoc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/proto/const.thrift` & `modelbest_sdk-0.1.3/modelbest_sdk/proto/const.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/proto/context.thrift` & `modelbest_sdk-0.1.3/modelbest_sdk/proto/context.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/proto/data_base.thrift` & `modelbest_sdk-0.1.3/modelbest_sdk/proto/data_base.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/proto/dataset_checkpoint.thrift` & `modelbest_sdk-0.1.3/modelbest_sdk/proto/dataset_checkpoint.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/proto/general_doc.thrift` & `modelbest_sdk-0.1.3/modelbest_sdk/proto/general_doc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/proto/general_servlet_rpc.thrift` & `modelbest_sdk-0.1.3/modelbest_sdk/proto/general_servlet_rpc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/proto/linkinfo.thrift` & `modelbest_sdk-0.1.3/modelbest_sdk/proto/linkinfo.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk/proto/mergeddoc.thrift` & `modelbest_sdk-0.1.3/modelbest_sdk/proto/mergeddoc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk.egg-info/PKG-INFO` & `modelbest_sdk-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: modelbest-sdk
-Version: 0.1.2
+Name: modelbest_sdk
+Version: 0.1.3
 Summary: Everything about modelbest data include data format mbtable, dataset, dataloader, and tools
 Home-page: https://codeup.aliyun.com/64ddb0a87f62ff9b3d23ca15/modelbest_sdk
 Author: HankyZhao
 Author-email: zhq980115@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `modelbest_sdk-0.1.2/modelbest_sdk.egg-info/SOURCES.txt` & `modelbest_sdk-0.1.3/modelbest_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/setup.py` & `modelbest_sdk-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modelbest_sdk',
-    version='0.1.2',
+    version='0.1.3',
     author='HankyZhao',
     author_email='zhq980115@gmail.com',
     description='Everything about modelbest data include data format mbtable, dataset, dataloader, and tools',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url='https://codeup.aliyun.com/64ddb0a87f62ff9b3d23ca15/modelbest_sdk',
     packages=find_packages(),
```

### Comparing `modelbest_sdk-0.1.2/test/dataset_context_test.py` & `modelbest_sdk-0.1.3/test/dataset_context_test.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/test/generate_data.py` & `modelbest_sdk-0.1.3/test/generate_data.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/test/test_base.py` & `modelbest_sdk-0.1.3/test/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         self.config_dir = os.path.join(cur_dir, "config")
         self.checkpoint_dir = os.path.join(cur_dir, "checkpoint")
         os.makedirs(self.data_dir, exist_ok=True)
         os.makedirs(self.config_dir, exist_ok=True)
         os.makedirs(self.checkpoint_dir, exist_ok=True)
         self.simple_dataset_config_path = os.path.join(self.config_dir , "simple_dataset_config.mbt")
         self.dist_dataset_config_path = os.path.join(self.config_dir , "dist_dataset_config.mbt")
-        self.simple_dataset_checkpoint_path = os.path.join(self.checkpoint_dir, "simple_dataset_checkpoint.mbt")
-        self.dist_dataset_checkpoint_path = os.path.join(self.checkpoint_dir, "dist_dataset_checkpoint.mbt")
+        self.simple_dataset_checkpoint_path = os.path.join(self.checkpoint_dir, "simple_dataset_checkpoint")
+        self.dist_dataset_checkpoint_path = os.path.join(self.checkpoint_dir, "dist_dataset_checkpoint")
         self.simple_dataset_context_path = os.path.join(self.config_dir, "simple_dataset_context.mbt")
         self.dist_dataset_context_path = os.path.join(self.config_dir, "dist_dataset_context.mbt")
 
         
         self.long_dataset_path = os.path.join(self.data_dir, "base_doc_long")
         self.short_dataset_path = os.path.join(self.data_dir, "base_doc_short")
         simple_dataset_info_list = DatasetInfoList([
@@ -50,18 +50,18 @@
         simple_dataset_context = DatasetContext(
             dataset_config_path=self.simple_dataset_config_path,
             dataset_checkpoint_path=self.simple_dataset_checkpoint_path,
         )
         dist_dataset_context = DatasetContext(
             rank=0,
             world_size=2,
-            num_workers=2,
+            num_workers=1,
             dataset_config_path=self.dist_dataset_config_path,
             dataset_checkpoint_path=self.dist_dataset_checkpoint_path,
-        )   
+        )
         simple_dataset_context.save_to_file(self.simple_dataset_context_path)
         dist_dataset_context.save_to_file(self.dist_dataset_context_path)
 
         os.makedirs(self.long_dataset_path, exist_ok=True)
         for i in range(2):
             builder = MbTableBuilder(os.path.join(self.long_dataset_path, f"part_{i}.mbt"))
             for j in range(10):
```

### Comparing `modelbest_sdk-0.1.2/test/test_mbtable.py` & `modelbest_sdk-0.1.3/test/test_mbtable.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.2/test/test_mbtable_partition.py` & `modelbest_sdk-0.1.3/test/test_mbtable_partition.py`

 * *Files identical despite different names*

