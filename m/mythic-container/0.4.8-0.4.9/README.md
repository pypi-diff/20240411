# Comparing `tmp/mythic_container-0.4.8.tar.gz` & `tmp/mythic_container-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic_container-0.4.8.tar", last modified: Tue Jan 23 20:49:48 2024, max compression
+gzip compressed data, was "mythic_container-0.4.9.tar", last modified: Wed Feb  7 02:58:03 2024, max compression
```

## Comparing `mythic_container-0.4.8.tar` & `mythic_container-0.4.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2024-01-23 20:49:48.426256 mythic_container-0.4.8/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.4.8/LICENSE.md
--rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2024-01-23 20:49:48.425708 mythic_container-0.4.8/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      993 2023-04-25 19:15:08.000000 mythic_container-0.4.8/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2024-01-23 20:49:48.375231 mythic_container-0.4.8/mythic_container/
--rw-r--r--   0 itsafeature   (501) staff       (20)    37526 2023-11-08 19:24:54.000000 mythic_container-0.4.8/mythic_container/C2ProfileBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    27829 2023-10-02 20:42:21.000000 mythic_container-0.4.8/mythic_container/LoggingBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    89266 2024-01-14 00:18:31.000000 mythic_container-0.4.8/mythic_container/MythicCommandBase.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2024-01-23 20:49:48.419908 mythic_container-0.4.8/mythic_container/MythicGoRPC/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2486 2024-01-22 16:30:33.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/callback_display_to_real_id.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1788 2023-12-11 21:00:48.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3123 2024-01-02 20:23:23.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_edge_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1788 2023-12-11 21:02:50.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7581 2023-05-09 13:37:04.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2273 2023-04-04 02:07:20.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3309 2023-04-26 14:57:11.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-04-01 06:52:13.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3169 2024-01-11 17:38:09.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4453 2023-04-13 18:13:16.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2370 2023-10-02 20:39:56.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     6013 2023-04-01 05:24:39.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1862 2023-10-02 20:39:56.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2425 2023-10-02 20:39:56.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1392 2023-10-02 20:39:56.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1403 2023-03-25 00:41:22.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2081 2023-10-02 20:39:56.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2031 2024-01-10 23:42:18.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_task_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2664 2023-10-02 20:39:56.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.4.8/mythic_container/MythicGoRPC/task_display_to_real_id.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.4.8/mythic_container/MythicRPC.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    23435 2024-01-10 22:45:59.000000 mythic_container-0.4.8/mythic_container/PayloadBuilder.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    17532 2023-10-02 20:39:56.000000 mythic_container-0.4.8/mythic_container/TranslationBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    13910 2023-05-08 15:16:26.000000 mythic_container-0.4.8/mythic_container/WebhookBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2963 2024-01-23 20:46:54.000000 mythic_container-0.4.8/mythic_container/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    49404 2024-01-23 20:46:24.000000 mythic_container-0.4.8/mythic_container/agent_utils.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    37389 2024-01-16 16:52:28.000000 mythic_container-0.4.8/mythic_container/c2_utils.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.4.8/mythic_container/config.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2024-01-23 20:49:48.424038 mythic_container-0.4.8/mythic_container/grpc/
--rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.4.8/mythic_container/grpc/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1768 2023-10-02 20:39:56.000000 mythic_container-0.4.8/mythic_container/grpc/pushC2GRPC_pb2.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2589 2023-10-02 20:39:56.000000 mythic_container-0.4.8/mythic_container/grpc/pushC2GRPC_pb2_grpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-10-02 16:59:34.000000 mythic_container-0.4.8/mythic_container/grpc/translationContainerGRPC_pb2.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-10-03 12:40:39.000000 mythic_container-0.4.8/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.4.8/mythic_container/logging.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4598 2023-10-02 20:39:56.000000 mythic_container-0.4.8/mythic_container/logging_utils.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)    31653 2024-01-10 22:14:52.000000 mythic_container-0.4.8/mythic_container/mythic_service.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    16178 2024-01-23 20:48:37.000000 mythic_container-0.4.8/mythic_container/rabbitmq.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.4.8/mythic_container/utils_mythic_file_transfer.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2821 2023-04-20 15:20:17.000000 mythic_container-0.4.8/mythic_container/webhook_utils.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2024-01-23 20:49:48.377190 mythic_container-0.4.8/mythic_container.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2024-01-23 20:49:48.000000 mythic_container-0.4.8/mythic_container.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)     4481 2024-01-23 20:49:48.000000 mythic_container-0.4.8/mythic_container.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2024-01-23 20:49:48.000000 mythic_container-0.4.8/mythic_container.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       95 2024-01-23 20:49:48.000000 mythic_container-0.4.8/mythic_container.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       17 2024-01-23 20:49:48.000000 mythic_container-0.4.8/mythic_container.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2024-01-23 20:49:48.426451 mythic_container-0.4.8/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1088 2024-01-23 20:46:50.000000 mythic_container-0.4.8/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2024-02-07 02:58:03.331842 mythic_container-0.4.9/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.4.9/LICENSE.md
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2024-02-07 02:58:03.331500 mythic_container-0.4.9/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      993 2023-04-25 19:15:08.000000 mythic_container-0.4.9/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2024-02-07 02:58:03.268040 mythic_container-0.4.9/mythic_container/
+-rw-r--r--   0 itsafeature   (501) staff       (20)    37526 2023-11-08 19:24:54.000000 mythic_container-0.4.9/mythic_container/C2ProfileBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    27953 2024-02-07 02:53:48.000000 mythic_container-0.4.9/mythic_container/LoggingBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    89266 2024-01-14 00:18:31.000000 mythic_container-0.4.9/mythic_container/MythicCommandBase.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2024-02-07 02:58:03.326257 mythic_container-0.4.9/mythic_container/MythicGoRPC/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2486 2024-01-22 16:30:33.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/callback_display_to_real_id.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1788 2023-12-11 21:00:48.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3123 2024-01-02 20:23:23.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_edge_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1788 2023-12-11 21:02:50.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7581 2023-05-09 13:37:04.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2273 2023-04-04 02:07:20.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3309 2023-04-26 14:57:11.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-04-01 06:52:13.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3169 2024-01-11 17:38:09.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4453 2023-04-13 18:13:16.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2370 2023-10-02 20:39:56.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     6013 2023-04-01 05:24:39.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1862 2023-10-02 20:39:56.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2425 2023-10-02 20:39:56.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1392 2023-10-02 20:39:56.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1403 2023-03-25 00:41:22.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2081 2023-10-02 20:39:56.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2031 2024-01-10 23:42:18.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2664 2023-10-02 20:39:56.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.4.9/mythic_container/MythicGoRPC/task_display_to_real_id.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.4.9/mythic_container/MythicRPC.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    23435 2024-01-10 22:45:59.000000 mythic_container-0.4.9/mythic_container/PayloadBuilder.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    17532 2023-10-02 20:39:56.000000 mythic_container-0.4.9/mythic_container/TranslationBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    13722 2024-02-07 02:56:42.000000 mythic_container-0.4.9/mythic_container/WebhookBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2963 2024-02-07 02:57:12.000000 mythic_container-0.4.9/mythic_container/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    49404 2024-01-30 00:35:40.000000 mythic_container-0.4.9/mythic_container/agent_utils.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    37389 2024-01-16 16:52:28.000000 mythic_container-0.4.9/mythic_container/c2_utils.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.4.9/mythic_container/config.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2024-02-07 02:58:03.330426 mythic_container-0.4.9/mythic_container/grpc/
+-rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.4.9/mythic_container/grpc/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1768 2023-10-02 20:39:56.000000 mythic_container-0.4.9/mythic_container/grpc/pushC2GRPC_pb2.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2589 2023-10-02 20:39:56.000000 mythic_container-0.4.9/mythic_container/grpc/pushC2GRPC_pb2_grpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-10-02 16:59:34.000000 mythic_container-0.4.9/mythic_container/grpc/translationContainerGRPC_pb2.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-10-03 12:40:39.000000 mythic_container-0.4.9/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.4.9/mythic_container/logging.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4598 2023-10-02 20:39:56.000000 mythic_container-0.4.9/mythic_container/logging_utils.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)    31653 2024-01-10 22:14:52.000000 mythic_container-0.4.9/mythic_container/mythic_service.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    16178 2024-01-23 20:48:37.000000 mythic_container-0.4.9/mythic_container/rabbitmq.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.4.9/mythic_container/utils_mythic_file_transfer.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2821 2023-04-20 15:20:17.000000 mythic_container-0.4.9/mythic_container/webhook_utils.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2024-02-07 02:58:03.270329 mythic_container-0.4.9/mythic_container.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2024-02-07 02:58:03.000000 mythic_container-0.4.9/mythic_container.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4481 2024-02-07 02:58:03.000000 mythic_container-0.4.9/mythic_container.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2024-02-07 02:58:03.000000 mythic_container-0.4.9/mythic_container.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       95 2024-02-07 02:58:03.000000 mythic_container-0.4.9/mythic_container.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       17 2024-02-07 02:58:03.000000 mythic_container-0.4.9/mythic_container.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2024-02-07 02:58:03.331983 mythic_container-0.4.9/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1088 2024-02-07 02:57:30.000000 mythic_container-0.4.9/setup.py
```

### Comparing `mythic_container-0.4.8/LICENSE.md` & `mythic_container-0.4.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/PKG-INFO` & `mythic_container-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic_container
-Version: 0.4.8
+Version: 0.4.9
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mythic_container-0.4.8/README.md` & `mythic_container-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/C2ProfileBase.py` & `mythic_container-0.4.9/mythic_container/C2ProfileBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/LoggingBase.py` & `mythic_container-0.4.9/mythic_container/LoggingBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -636,20 +636,22 @@
     def __init__(self,
                  operation_id: int = None,
                  operation_name: str = None,
                  username: str = None,
                  timestamp: str = None,
                  action: str = None,
                  data: dict = None,
+                 server_name: str = None,
                  **kwargs):
         self.OperationID = operation_id
         self.OperationName = operation_name
         self.OperatorUsername = username
         self.Timestamp = timestamp
         self.Action = action
+        self.ServerName = server_name
         if self.Action == mythic_container.LOG_TYPE_CALLBACK:
             self.Data = NewCallbackLoggingData(**data)
         elif self.Action == mythic_container.LOG_TYPE_FILE:
             self.Data = NewFileLoggingData(**data)
         elif self.Action == mythic_container.LOG_TYPE_KEYLOG:
             self.Data = NewKeylogLoggingData(**data)
         elif self.Action == mythic_container.LOG_TYPE_ARTIFACT:
@@ -670,14 +672,15 @@
     def to_json(self):
         return {
             "operation_id": self.OperationID,
             "operation_name": self.OperationName,
             "operator_username": self.OperatorUsername,
             "timestamp": self.Timestamp,
             "action": self.Action,
+            "server_name": self.ServerName,
             "data": self.Data.to_json()
         }
 
     def __str__(self):
         return json.dumps(self.to_json(), sort_keys=True, indent=2)
```

### Comparing `mythic_container-0.4.8/mythic_container/MythicCommandBase.py` & `mythic_container-0.4.9/mythic_container/MythicCommandBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/__init__.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/__init__.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/callback_display_to_real_id.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/callback_display_to_real_id.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_edge_search.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_edge_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_task_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicGoRPC/task_display_to_real_id.py` & `mythic_container-0.4.9/mythic_container/MythicGoRPC/task_display_to_real_id.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/MythicRPC.py` & `mythic_container-0.4.9/mythic_container/MythicRPC.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/PayloadBuilder.py` & `mythic_container-0.4.9/mythic_container/PayloadBuilder.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/TranslationBase.py` & `mythic_container-0.4.9/mythic_container/TranslationBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/WebhookBase.py` & `mythic_container-0.4.9/mythic_container/WebhookBase.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         ExtraInfo (str): Freeform additional text that can be set on the callback
         SleepInfo (str): Sleep information that can be stored as part of the callback (not implicitly set)
         DisplayID (int): The ID that the user sees when looking at the callback in Mythic's UI
         ID (int): The unique ID associated with this callback that can be used with RPC calls
         IntegrityLevel (int): The integrity level of this callback (mirrors Windows integrity levels with 0-5 range and 3+ is High integrity)
 
     """
+
     def __init__(self,
                  user: str = None,
                  host: str = None,
                  ips: str = None,
                  domain: str = None,
                  external_ip: str = None,
                  process_name: str = None,
@@ -94,14 +95,15 @@
     Attributes:
         TaskID (int): The ID of the task associated with this feedback (if provided) that can be used with RPC Calls
         Message (str): The feedback message
         FeedbackType (str): The type of feedback
         DisplayID (int): The display ID of the task that the user would see
 
     """
+
     def __init__(self,
                  task_id: int = None,
                  display_id: int = None,
                  message: str = None,
                  feedback_type: str = None,
                  **kwargs):
         self.TaskID = task_id
@@ -126,14 +128,15 @@
 class NewStartupWebhookData:
     """The base definition for a notification that Mythic started
 
     Attributes:
         StartupMessage (str): The message that Mythic started
 
     """
+
     def __init__(self,
                  startup_message: str = None,
                  **kwargs):
         self.StartupMessage = startup_message
         for k, v in kwargs.items():
             logger.info(f"unknown kwarg {k} {v}")
 
@@ -153,14 +156,15 @@
         OperatorID (int): The unique ID of the operator that caused this message (if not Mythic)
         Message (str): The alert message
         Source (str): The source of the alert message
         Count (int): The number of times this entry has been seen
         Timestamp (str): When this alert was generated
 
     """
+
     def __init__(self,
                  operator_id: int = None,
                  message: str = None,
                  source: str = None,
                  count: int = None,
                  timestamp: str = None,
                  **kwargs):
@@ -208,20 +212,22 @@
                  operation_id: int = None,
                  operation_name: str = None,
                  operation_webhook: str = None,
                  operation_channel: str = None,
                  operator_username: str = None,
                  action: str = None,
                  data: dict = None,
+                 server_name: str = None,
                  **kwargs):
         self.OperationID = operation_id
         self.OperationName = operation_name
         self.OperationWebhook = operation_webhook
         self.OperationChannel = operation_channel
         self.OperatorUsername = operator_username
+        self.ServerName = server_name
         self.Action = action
         if self.Action == mythic_container.WEBHOOK_TYPE_NEW_CALLBACK:
             self.Data = NewCallbackWebhookData(**data)
         elif self.Action == mythic_container.WEBHOOK_TYPE_NEW_FEEDBACK:
             self.Data = NewFeedbackWebhookData(**data)
         elif self.Action == mythic_container.WEBHOOK_TYPE_NEW_STARTUP:
             self.Data = NewStartupWebhookData(**data)
@@ -238,14 +244,15 @@
         return {
             "operation_id": self.OperationID,
             "operation_name": self.OperationName,
             "operation_webhook": self.OperationWebhook,
             "operation_channel": self.OperationChannel,
             "operator_username": self.OperatorUsername,
             "action": self.Action,
+            "server_name": self.ServerName,
             "data": self.Data if isinstance(self.Data, dict) or self.Data is None else self.Data.to_json()
         }
 
     def __str__(self):
         return json.dumps(self.to_json(), sort_keys=True, indent=2)
 
 
@@ -317,21 +324,15 @@
         elif self.webhook_channel is not None:
             return self.webhook_channel
         else:
             logger.error(f"No webhook channel found")
             return ""
 
 
-async def sendWebhookMessage(contents: dict, url: str) -> str:
+async def sendWebhookMessage(contents: dict, url: str) -> (int, str):
     try:
         async with aiohttp.ClientSession() as session:
             async with session.post(url, json=contents, ssl=False) as resp:
-                if resp.status == 200:
-                    responseData = await resp.text()
-                    logger.debug(f"webhook response data: {responseData}")
-                    return responseData
-                else:
-                    logger.error(f"[-] Failed to send webhook message: {resp}")
-                    return f"[-] Failed to send webhook message: {resp}"
+                return resp.status, await resp.text()
     except Exception as e:
         logger.exception(f"[-] Failed to send webhook: {e}")
-        return f"[-] Failed to send webhook: {e}"
+        return 400, f"[-] Failed to send webhook: {e}"
```

### Comparing `mythic_container-0.4.8/mythic_container/__init__.py` & `mythic_container-0.4.9/mythic_container/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .rabbitmq import rabbitmqConnectionClass
 from .mythic_service import start_and_run_forever, test_command
 
-containerVersion = "v1.1.4"
+containerVersion = "v1.1.5"
 
-PyPi_version = "0.4.8"
+PyPi_version = "0.4.9"
 
 RabbitmqConnection = rabbitmqConnectionClass()
 
 MYTHIC_RPC_OTHER_SERVICES_RPC = "mythic_rpc_other_service_rpc"
 PAYLOAD_BUILD_C2_ROUTING_KEY = "payload_c2_build"
 # payload routes
 PT_SYNC_ROUTING_KEY = "pt_sync"
```

### Comparing `mythic_container-0.4.8/mythic_container/agent_utils.py` & `mythic_container-0.4.9/mythic_container/agent_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/c2_utils.py` & `mythic_container-0.4.9/mythic_container/c2_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/grpc/pushC2GRPC_pb2.py` & `mythic_container-0.4.9/mythic_container/grpc/pushC2GRPC_pb2.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/grpc/pushC2GRPC_pb2_grpc.py` & `mythic_container-0.4.9/mythic_container/grpc/pushC2GRPC_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/grpc/translationContainerGRPC_pb2.py` & `mythic_container-0.4.9/mythic_container/grpc/translationContainerGRPC_pb2.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py` & `mythic_container-0.4.9/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/logging.py` & `mythic_container-0.4.9/mythic_container/logging.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/logging_utils.py` & `mythic_container-0.4.9/mythic_container/logging_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/mythic_service.py` & `mythic_container-0.4.9/mythic_container/mythic_service.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/rabbitmq.py` & `mythic_container-0.4.9/mythic_container/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/utils_mythic_file_transfer.py` & `mythic_container-0.4.9/mythic_container/utils_mythic_file_transfer.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container/webhook_utils.py` & `mythic_container-0.4.9/mythic_container/webhook_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/mythic_container.egg-info/PKG-INFO` & `mythic_container-0.4.9/mythic_container.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic-container
-Version: 0.4.8
+Version: 0.4.9
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mythic_container-0.4.8/mythic_container.egg-info/SOURCES.txt` & `mythic_container-0.4.9/mythic_container.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mythic_container-0.4.8/setup.py` & `mythic_container-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic_container",
-    version="0.4.8",
+    version="0.4.9",
     description="Functionality for Mythic Services",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/customizing/payload-type-development",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

