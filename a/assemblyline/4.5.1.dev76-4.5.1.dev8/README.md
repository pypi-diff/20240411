# Comparing `tmp/assemblyline-4.5.1.dev76.tar.gz` & `tmp/assemblyline-4.5.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyline-4.5.1.dev76.tar", last modified: Thu Apr 11 13:59:53 2024, max compression
+gzip compressed data, was "assemblyline-4.5.1.dev8.tar", last modified: Thu Feb 22 20:16:24 2024, max compression
```

## Comparing `assemblyline-4.5.1.dev76.tar` & `assemblyline-4.5.1.dev8.tar`

### file list

```diff
@@ -1,193 +1,191 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.881333 assemblyline-4.5.1.dev76/
--rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/LICENCE.md
--rw-r--r--   0 vsts      (1001) docker     (127)       47 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     2531 2024-04-11 13:59:53.881333 assemblyline-4.5.1.dev76/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1562 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.853333 assemblyline-4.5.1.dev76/assemblyline/
--rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-04-11 13:59:48.000000 assemblyline-4.5.1.dev76/assemblyline/VERSION
--rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.853333 assemblyline-4.5.1.dev76/assemblyline/cachestore/
--rw-r--r--   0 vsts      (1001) docker     (127)     3463 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/cachestore/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.865333 assemblyline-4.5.1.dev76/assemblyline/common/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7321 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/archiving.py
--rw-r--r--   0 vsts      (1001) docker     (127)  2243670 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/attack_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13368 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/backupmanager.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2369 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/common/banner.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16341 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/bundling.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5668 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/caching.py
--rw-r--r--   0 vsts      (1001) docker     (127)      903 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/chunk.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41768 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/classification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4950 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/classification.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     5811 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/cleanup_filestore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2132 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/codec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5031 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/common/comms.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2587 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5841 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/custom.magic
--rw-r--r--   0 vsts      (1001) docker     (127)    39467 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/custom.yara
--rw-r--r--   0 vsts      (1001) docker     (127)     2903 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/dict_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2550 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/digests.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2713 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/entropy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1903 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/common/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      584 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/file.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9003 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/forge.py
--rw-r--r--   0 vsts      (1001) docker     (127)   289190 2024-04-11 13:59:53.000000 assemblyline-4.5.1.dev76/assemblyline/common/frequency.c
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/common/frequency.pyx
--rw-r--r--   0 vsts      (1001) docker     (127)     6450 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/heuristics.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1398 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/hexdump.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23161 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/identify.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19801 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/identify_defaults.py
--rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/importing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4229 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/iprange.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5281 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/isotime.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4310 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      909 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/logformat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/lucene.lark
--rw-r--r--   0 vsts      (1001) docker     (127)     1105 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/common/memory_zip.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/metrics.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5230 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/net.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21606 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/net_static.py
--rw-r--r--   0 vsts      (1001) docker     (127)      231 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/common/null.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1515 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/path.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28598 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/postprocess.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4971 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/common/random_user.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3379 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/security.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/common/signaturing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7396 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/str_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12687 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/tag_safelist.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     3904 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/tagging.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1052 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/threading.py
--rw-r--r--   0 vsts      (1001) docker     (127)      640 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/uid.py
--rw-r--r--   0 vsts      (1001) docker     (127)       57 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/common/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.865333 assemblyline-4.5.1.dev76/assemblyline/datasource/
--rw-r--r--   0 vsts      (1001) docker     (127)      433 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/datasource/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2183 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/datasource/al.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1462 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/datasource/alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1093 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/datasource/common.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.865333 assemblyline-4.5.1.dev76/assemblyline/datastore/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/datastore/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2950 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/datastore/bulk.py
--rw-r--r--   0 vsts      (1001) docker     (127)    88839 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/datastore/collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      572 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/datastore/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    64390 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/datastore/helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15722 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/datastore/store.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.869333 assemblyline-4.5.1.dev76/assemblyline/datastore/support/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/datastore/support/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9424 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/datastore/support/build.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/datastore/support/schemas.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.869333 assemblyline-4.5.1.dev76/assemblyline/filestore/
--rw-r--r--   0 vsts      (1001) docker     (127)    10460 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/filestore/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.869333 assemblyline-4.5.1.dev76/assemblyline/filestore/transport/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/filestore/transport/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7891 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/filestore/transport/azure.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2720 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/filestore/transport/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9648 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/filestore/transport/ftp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3752 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/filestore/transport/http.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5429 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/filestore/transport/local.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6828 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/filestore/transport/s3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6558 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/filestore/transport/sftp.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.869333 assemblyline-4.5.1.dev76/assemblyline/odm/
--rw-r--r--   0 vsts      (1001) docker     (127)     1854 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    54612 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)      323 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/odm/common.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.873333 assemblyline-4.5.1.dev76/assemblyline/odm/messages/
--rw-r--r--   0 vsts      (1001) docker     (127)       75 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      596 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1505 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/alerter_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1532 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/archive_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/changes.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2476 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/dispatcher_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1299 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/dispatching.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1546 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/expiry_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/ingest_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      848 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/metrics.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1440 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/retrohunt_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/scaler_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1403 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/scaler_status_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1787 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/service_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1275 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/service_timing_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      959 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/shard_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2190 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/submission.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4109 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1116 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/messages/vacuum_heartbeat.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.877333 assemblyline-4.5.1.dev76/assemblyline/odm/models/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3071 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/actions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14239 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3932 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/badlist.py
--rw-r--r--   0 vsts      (1001) docker     (127)      281 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/cached_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)    74970 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/emptyresult.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2072 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/error.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5057 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      683 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/filescore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/heuristic.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.877333 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/
--rw-r--r--   0 vsts      (1001) docker     (127)       82 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.877333 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/filetypes/
--rw-r--r--   0 vsts      (1001) docker     (127)       61 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/filetypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24751 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/filetypes/pe.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5726 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/ontology.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.877333 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1843 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/antivirus.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13798 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/malware_config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3838 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/network.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2765 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/process.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2507 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/sandbox.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2961 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/signature.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3635 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/replay.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9421 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2683 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/retrohunt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3098 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/safelist.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10934 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/service.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8157 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/service_delta.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/signature.py
--rw-r--r--   0 vsts      (1001) docker     (127)      695 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/statistics.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8791 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/submission.py
--rw-r--r--   0 vsts      (1001) docker     (127)      843 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/submission_summary.py
--rw-r--r--   0 vsts      (1001) docker     (127)      638 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/submission_tree.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36489 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/tagging.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10462 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/user.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1255 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/user_favorites.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2508 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/user_settings.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1895 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/models/workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.881333 assemblyline-4.5.1.dev76/assemblyline/odm/random_data/
--rw-r--r--   0 vsts      (1001) docker     (127)    17983 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/random_data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2956 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/random_data/create_test_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25241 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/odm/random_data/sample_rules.yar
--rw-r--r--   0 vsts      (1001) docker     (127)     9244 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/odm/random_data/sample_suricata.rules
--rw-r--r--   0 vsts      (1001) docker     (127)    14862 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/odm/randomizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.881333 assemblyline-4.5.1.dev76/assemblyline/remote/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/remote/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.881333 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/
--rw-r--r--   0 vsts      (1001) docker     (127)     3448 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1661 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/cache.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1984 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/counters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4112 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/events.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7000 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/exporting_counter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6018 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/hash.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1442 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/lock.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.881333 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/queues/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/queues/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1793 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/queues/comms.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/queues/multi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2871 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/queues/named.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7394 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/queues/priority.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2902 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/set.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1926 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/user_quota_tracker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.881333 assemblyline-4.5.1.dev76/assemblyline/run/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/run/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53139 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/assemblyline/run/cli.py
--rw-r--r--   0 vsts      (1001) docker     (127)      645 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/run/pubsub_reader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3760 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/run/suricata_importer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4791 2024-04-11 13:59:26.000000 assemblyline-4.5.1.dev76/assemblyline/run/yara_importer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:53.853333 assemblyline-4.5.1.dev76/assemblyline.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2531 2024-04-11 13:59:53.000000 assemblyline-4.5.1.dev76/assemblyline.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     6292 2024-04-11 13:59:53.000000 assemblyline-4.5.1.dev76/assemblyline.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-11 13:59:53.000000 assemblyline-4.5.1.dev76/assemblyline.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      512 2024-04-11 13:59:53.000000 assemblyline-4.5.1.dev76/assemblyline.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-11 13:59:53.000000 assemblyline-4.5.1.dev76/assemblyline.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-11 13:59:53.881333 assemblyline-4.5.1.dev76/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     3845 2024-04-11 13:59:28.000000 assemblyline-4.5.1.dev76/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.760298 assemblyline-4.5.1.dev8/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/LICENCE.md
+-rw-r--r--   0 vsts      (1001) docker     (127)       47 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     2530 2024-02-22 20:16:24.760298 assemblyline-4.5.1.dev8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1562 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.732298 assemblyline-4.5.1.dev8/assemblyline/
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-02-22 20:16:21.000000 assemblyline-4.5.1.dev8/assemblyline/VERSION
+-rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.732298 assemblyline-4.5.1.dev8/assemblyline/cachestore/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3463 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/cachestore/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/common/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4138 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/archiving.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  2243670 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/attack_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13368 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/backupmanager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2369 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/banner.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16341 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/bundling.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5668 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/caching.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      903 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/chunk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41768 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/classification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4950 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/classification.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     5811 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/cleanup_filestore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2132 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/codec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5031 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/comms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2587 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5841 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/custom.magic
+-rw-r--r--   0 vsts      (1001) docker     (127)    39136 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/custom.yara
+-rw-r--r--   0 vsts      (1001) docker     (127)     2903 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/dict_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2550 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/digests.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2713 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/entropy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1903 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      584 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8581 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/forge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   288720 2024-02-22 20:16:24.000000 assemblyline-4.5.1.dev8/assemblyline/common/frequency.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/frequency.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)     6450 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/heuristics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1398 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/hexdump.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23161 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/identify.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19383 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/identify_defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/importing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4229 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/iprange.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5281 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/isotime.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4310 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      909 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/logformat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/lucene.lark
+-rw-r--r--   0 vsts      (1001) docker     (127)     1105 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/memory_zip.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5230 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/net.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21606 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/net_static.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      231 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/null.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1515 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/path.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28598 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/postprocess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4971 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/random_user.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3379 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/security.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/signaturing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7396 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/str_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12687 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/tag_safelist.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     3904 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1052 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/threading.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      640 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/uid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       57 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/datasource/
+-rw-r--r--   0 vsts      (1001) docker     (127)      433 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/datasource/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2183 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/datasource/al.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1462 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/datasource/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1093 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/datasource/common.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/datastore/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2950 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/bulk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    88221 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      572 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61668 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15722 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/store.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/datastore/support/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/support/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9424 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/support/build.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/support/schemas.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/filestore/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10460 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7891 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/azure.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2720 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9648 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/ftp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3752 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/http.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5429 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/local.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6828 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/s3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6558 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/sftp.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/odm/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1854 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    54611 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      323 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/odm/common.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.752298 assemblyline-4.5.1.dev8/assemblyline/odm/messages/
+-rw-r--r--   0 vsts      (1001) docker     (127)       75 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      596 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1505 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/alerter_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1532 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/archive_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/changes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2476 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/dispatcher_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1299 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/dispatching.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1546 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/expiry_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/ingest_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      848 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/scaler_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1403 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/scaler_status_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1787 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/service_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1275 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/service_timing_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2190 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/submission.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4109 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1116 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/vacuum_heartbeat.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.756298 assemblyline-4.5.1.dev8/assemblyline/odm/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3071 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/actions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13978 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3932 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/badlist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      281 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/cached_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    71484 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/emptyresult.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2072 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/error.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5057 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      683 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/filescore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/heuristic.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.756298 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/
+-rw-r--r--   0 vsts      (1001) docker     (127)       82 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.756298 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/filetypes/
+-rw-r--r--   0 vsts      (1001) docker     (127)       61 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/filetypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24751 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/filetypes/pe.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5726 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/ontology.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.756298 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1843 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/antivirus.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13798 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/malware_config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3838 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/network.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2765 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/process.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2507 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/sandbox.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2961 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/signature.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3635 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/replay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9421 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2683 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/retrohunt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3098 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/safelist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10968 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/service.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8161 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/service_delta.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/signature.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      695 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/statistics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8791 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/submission.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      843 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/submission_summary.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      638 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/submission_tree.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36489 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10371 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/user.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1255 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/user_favorites.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2508 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/user_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1895 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.756298 assemblyline-4.5.1.dev8/assemblyline/odm/random_data/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17934 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/random_data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2956 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/random_data/create_test_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25241 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/odm/random_data/sample_rules.yar
+-rw-r--r--   0 vsts      (1001) docker     (127)     9244 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/odm/random_data/sample_suricata.rules
+-rw-r--r--   0 vsts      (1001) docker     (127)    14862 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/randomizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.756298 assemblyline-4.5.1.dev8/assemblyline/remote/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/remote/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.760298 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3448 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1661 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1984 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/counters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4112 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7000 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/exporting_counter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6018 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/hash.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1442 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/lock.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.760298 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1793 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/comms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/multi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2871 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/named.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7394 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/priority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2902 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/set.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1926 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/user_quota_tracker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.760298 assemblyline-4.5.1.dev8/assemblyline/run/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/run/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53139 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/run/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      645 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/run/pubsub_reader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3760 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/run/suricata_importer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4791 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/run/yara_importer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.732298 assemblyline-4.5.1.dev8/assemblyline.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2530 2024-02-22 20:16:24.000000 assemblyline-4.5.1.dev8/assemblyline.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     6198 2024-02-22 20:16:24.000000 assemblyline-4.5.1.dev8/assemblyline.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-22 20:16:24.000000 assemblyline-4.5.1.dev8/assemblyline.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-02-22 20:16:24.000000 assemblyline-4.5.1.dev8/assemblyline.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-02-22 20:16:24.000000 assemblyline-4.5.1.dev8/assemblyline.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-02-22 20:16:24.760298 assemblyline-4.5.1.dev8/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     3812 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/setup.py
```

### Comparing `assemblyline-4.5.1.dev76/LICENCE.md` & `assemblyline-4.5.1.dev8/LICENCE.md`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/PKG-INFO` & `assemblyline-4.5.1.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline
-Version: 4.5.1.dev76
+Version: 4.5.1.dev8
 Summary: Assemblyline 4 - Automated malware analysis framework
 Home-page: https://github.com/CybercentreCanada/assemblyline-base
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-4.5.1.dev76/README.md` & `assemblyline-4.5.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/cachestore/__init__.py` & `assemblyline-4.5.1.dev8/assemblyline/cachestore/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/attack_map.py` & `assemblyline-4.5.1.dev8/assemblyline/common/attack_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/backupmanager.py` & `assemblyline-4.5.1.dev8/assemblyline/common/backupmanager.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/banner.py` & `assemblyline-4.5.1.dev8/assemblyline/common/banner.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/bundling.py` & `assemblyline-4.5.1.dev8/assemblyline/common/bundling.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/caching.py` & `assemblyline-4.5.1.dev8/assemblyline/common/caching.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/chunk.py` & `assemblyline-4.5.1.dev8/assemblyline/common/chunk.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/classification.py` & `assemblyline-4.5.1.dev8/assemblyline/common/classification.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/classification.yml` & `assemblyline-4.5.1.dev8/assemblyline/common/classification.yml`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/cleanup_filestore.py` & `assemblyline-4.5.1.dev8/assemblyline/common/cleanup_filestore.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/codec.py` & `assemblyline-4.5.1.dev8/assemblyline/common/codec.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/comms.py` & `assemblyline-4.5.1.dev8/assemblyline/common/comms.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/constants.py` & `assemblyline-4.5.1.dev8/assemblyline/common/constants.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/custom.magic` & `assemblyline-4.5.1.dev8/assemblyline/common/custom.magic`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/custom.yara` & `assemblyline-4.5.1.dev8/assemblyline/common/custom.yara`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         // Suported by https://github.com/CERT-Polska/karton-classifier/blob/4cf125296e3a0c1d6c1cb8c16f97d608054c7f19/karton/classifier/classifier.py#L659
         // Supported by https://github.com/CAPESandbox/sflock/blob/1e0ed7e18ddfe723c2d2603875ca26d63887c189/sflock/ident.py#L431
         $strong_js10 = /(^|;|\s)(var|let|const)[ \t]+\w+[ \t]*=/ ascii wide
         // If this is exactly in the sample, will trigger a second time because of strong_js10
         $strong_js11 = /(^|\n)window.location.href[ \t]*=/ ascii wide
 
         // Used in a lot of malware samples to fail silently
-        $strong_js12 = /catch\s*\(\w*\)\s*\{/ ascii wide
+        $strong_js12 = /catch\s+\(\w*\)\s+\{/ ascii wide
 
         // Firefox browser specific method
         $strong_js13 = /user_pref\("[\w.]+",\s*[\w"']+\)/ ascii wide
 
         // Inspired by https://github.com/CAPESandbox/sflock/blob/1e0ed7e18ddfe723c2d2603875ca26d63887c189/sflock/ident.py#L431
         $strong_js14 = "alert(" ascii wide
         $strong_js15 = ".charAt(" ascii wide
@@ -365,35 +365,27 @@
 rule document_email_1 {
 
     meta:
         type = "document/email"
         score = 15
 
     strings:
-        // This is a common JavaScript key
         $rec = "From:"
         $subrec1 = "Bcc:"
-        // This is a common JavaScript key
         $subrec2 = "To:"
         $subrec3 = "Date:"
-        // This is a common JavaScript key
         $opt1 = "Subject:"
         $opt2 = "Received: from"
         $opt3 = "MIME-Version:"
         $opt4 = "Content-Type:"
 
     condition:
-        // This is a relatively* trusted mime for identifying JavaScript that could be mis-identified as emails
-        mime != "application/javascript"
-        and
-        (
-            all of ($rec*)
-            and 1 of ($subrec*)
-            and 1 of ($opt*)
-        )
+        all of ($rec*)
+        and 1 of ($subrec*)
+        and 1 of ($opt*)
 }
 
 rule document_email_2 {
 
     meta:
         type = "document/email"
         score = 10
@@ -914,15 +906,15 @@
         $cmd3 = /(^|\n|@|&)reg[ \t]+(delete|query|add|copy|save|load|unload|restore|compare|export|import|flags)[ \t]+/i
         $cmd4 = /(^|\n|@|&|^\s)start[ \t]+(\/(min|b|wait|belownormal|abovenormal|realtime|high|normal|low|shared|seperate|max|i)[ \t]+|"\w*"[ \t]+)+["']?([A-Z]:)?([\\|\/]?[\w.]+)+/i
         $cmd5 = /(^|\n)exit\s*$/i
         $cmd6 = /(^|\n|@|&)%comspec%/i
         $cmd7 = /(^|\n|@|&)timeout[ \t](\/\w+|[-]?\d{1,5})/i
         $rem1 = /(^|\n|@|&)\^?r\^?e\^?m\^?[ \t]\w+/i
         $rem2 = /(^|\n)::/
-        $set = /(^|\n|@|&)\^?s\^?e\^?t\^?[ \t]\^?\w+\^?=\^?%?\^?\w+/i
+        $set = /(^|\n|@|&)\^?s\^?e\^?t\^?[ \t]\^?\w+\^?=\^?\w+/i
         $exp = /setlocal[ \t](enableDelayedExpansion|disableDelayedExpansion)/i
 
     condition:
         (
             mime startswith "text"
             or uint16(0) == 0xFEFF  // little-endian utf-16 BOM at 0
         )
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/dict_utils.py` & `assemblyline-4.5.1.dev8/assemblyline/common/dict_utils.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/digests.py` & `assemblyline-4.5.1.dev8/assemblyline/common/digests.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/entropy.py` & `assemblyline-4.5.1.dev8/assemblyline/common/entropy.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/exceptions.py` & `assemblyline-4.5.1.dev8/assemblyline/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/file.py` & `assemblyline-4.5.1.dev8/assemblyline/common/file.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/forge.py` & `assemblyline-4.5.1.dev8/assemblyline/common/forge.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,19 @@
 import importlib
 import os
 import time
 import yaml
 
 from string import Template
 from typing import TYPE_CHECKING, Optional
-from hauntedhouse import Client
 
 from assemblyline.common.constants import service_queue_name
 from assemblyline.common.dict_utils import recursive_update
 from assemblyline.common.importing import load_module_by_path
 
-
 if TYPE_CHECKING:
     from assemblyline.odm.models.config import Config
 
 config_cache = {}
 classification_engines = {}
 
 
@@ -201,28 +199,14 @@
 
     if not tag_safelist_data:
         raise InvalidSafelist('Could not find any tag_safelist file to load.')
 
     return TagSafelister(tag_safelist_data, log=log)
 
 
-def get_hauntedhouse_client(config: Config) -> Optional[Client]:
-    if config.retrohunt.enabled:
-        ca_path = None
-        if config.retrohunt.tls_verify:
-            ca_path = '/etc/assemblyline/ssl/al_root-ca.crt'
-
-        return Client(
-            address=config.retrohunt.url,
-            api_key=config.retrohunt.api_key,
-            verify=ca_path
-        )
-    return None
-
-
 class CachedObject:
     """An object proxy that automatically refreshes its target periodically."""
 
     def __init__(self, factory, refresh=None, args=None, kwargs=None):
         """
         Args:
             factory: Factory that takes the arguments given in `args` and `kwargs` and produces the proxyed object.
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/frequency.c` & `assemblyline-4.5.1.dev8/assemblyline/common/frequency.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.10 */
+/* Generated by Cython 3.0.8 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "assemblyline.common.frequency",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x03000AF0
+#define CYTHON_HEX_VERSION 0x030008F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,16 +128,14 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-  #undef CYTHON_USE_FREELISTS
-  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -191,16 +189,14 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-  #undef CYTHON_USE_FREELISTS
-  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -254,83 +250,60 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-  #undef CYTHON_USE_FREELISTS
-  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
-  #ifndef CYTHON_USE_TYPE_SPECS
-    #define CYTHON_USE_TYPE_SPECS 0
-  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
-  #ifndef CYTHON_USE_PYLONG_INTERNALS
-    #define CYTHON_USE_PYLONG_INTERNALS 0
-  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
-  #undef CYTHON_FAST_GIL
-  #define CYTHON_FAST_GIL 0
-  #ifndef CYTHON_METH_FASTCALL
-    #define CYTHON_METH_FASTCALL 1
-  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #ifndef CYTHON_PEP487_INIT_SUBCLASS
-    #define CYTHON_PEP487_INIT_SUBCLASS 1
-  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
-  #ifndef CYTHON_USE_MODULE_STATE
-    #define CYTHON_USE_MODULE_STATE 0
-  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
-  #endif
-  #ifndef CYTHON_USE_FREELISTS
-    #define CYTHON_USE_FREELISTS 0
-  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -413,17 +386,14 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
-  #ifndef CYTHON_USE_FREELISTS
-    #define CYTHON_USE_FREELISTS 1
-  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -759,21 +729,16 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #if PY_VERSION_HEX >= 0x030d00A4
-  #  define __Pyx_PyCFunctionFast PyCFunctionFast
-  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
-  #else
-  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
-  #endif
+  #define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1117,15 +1082,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+#if PY_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1204,15 +1169,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1308,15 +1273,32 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
+{
+    const wchar_t *u_end = u;
+    while (*u_end++) ;
+    return (size_t)(u_end - u - 1);
+}
+#else
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
+{
+    const Py_UNICODE *u_end = u;
+    while (*u_end++) ;
+    return (size_t)(u_end - u - 1);
+}
+#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
+#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
+#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -5919,15 +5901,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/frequency.pyx` & `assemblyline-4.5.1.dev8/assemblyline/common/frequency.pyx`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/heuristics.py` & `assemblyline-4.5.1.dev8/assemblyline/common/heuristics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/hexdump.py` & `assemblyline-4.5.1.dev8/assemblyline/common/hexdump.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/identify.py` & `assemblyline-4.5.1.dev8/assemblyline/common/identify.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/identify_defaults.py` & `assemblyline-4.5.1.dev8/assemblyline/common/identify_defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,34 +123,31 @@
     {"al_type": "executable/linux/coff64", "regex": r"^64-bit XCOFF"},
     {"al_type": "executable/linux/ia/coff64", "regex": r"^Intel ia64 COFF"},
     {"al_type": "executable/linux/misp/ecoff", "regex": r"^MIPS[^\|]+ ECOFF"},
     {"al_type": "executable/linux/a.out", "regex": r"^a.out"},
     {"al_type": "executable/mach-o", "regex": r"^Mach-O"},
     {"al_type": "archive/7-zip", "regex": r"^7-zip archive data"},
     {"al_type": "archive/ace", "regex": r"^ACE archive data"},
-    {"al_type": "archive/asar", "regex": r"^Electron ASAR archive"},
     {"al_type": "archive/bzip2", "regex": r"^bzip2 compressed data"},
     {"al_type": "archive/cabinet", "regex": r"^installshield cab"},
     {"al_type": "archive/cabinet", "regex": r"^microsoft cabinet archive data"},
     {"al_type": "archive/cpio", "regex": r"cpio archive"},
     {"al_type": "archive/gzip", "regex": r"^gzip compressed data"},
     {"al_type": "archive/iso", "regex": r"ISO 9660"},
     {"al_type": "archive/lzma", "regex": r"^LZMA compressed data"},
     {"al_type": "archive/rar", "regex": r"^rar archive data"},
     {"al_type": "archive/tar", "regex": r"^(GNU|POSIX) tar archive"},
-    {"al_type": "archive/ar", "regex": r"^current ar archive"},
+    {"al_type": "archive/ar", "regex": r"ar archive"},
     {"al_type": "archive/vhd", "regex": r"^Microsoft Disk Image"},
     {"al_type": "archive/xz", "regex": r"^XZ compressed data"},
     {"al_type": "archive/zip", "regex": r"^zip archive data"},
     {"al_type": "archive/zstd", "regex": r"^Zstandard compressed data"},
     {"al_type": "archive/zpaq", "regex": r"^ZPAQ file"},
     {"al_type": "network/tcpdump", "regex": r"^(tcpdump|pcap)"},
     {"al_type": "document/pdf", "regex": r"^pdf document"},
-    {"al_type": "document/epub", "regex": r"^EPUB document"},
-    {"al_type": "document/mobi", "regex": r"^Mobipocket E-book"},
     {"al_type": "image/bmp", "regex": r"^pc bitmap"},
     {"al_type": "image/gif", "regex": r"^gif image data"},
     {"al_type": "image/jpg", "regex": r"^jpeg image data"},
     {"al_type": "image/png", "regex": r"^png image data"},
     {"al_type": "image/tiff", "regex": r"^TIFF image data"},
     {"al_type": "image/webp", "regex": r"Web/P image"},
     {"al_type": "document/installer/windows", "regex": r"(Installation Database|Windows Installer)"},
@@ -174,15 +171,14 @@
     {"al_type": "code/xml", "regex": r"xml"},
     {"al_type": "image/tim", "regex": r"TIM image"},
     {"al_type": "network/sff", "regex": r"Frame Format"},
     {"al_type": "shortcut/windows", "regex": r"^MS Windows shortcut"},
     {"al_type": "document/email", "regex": r"Mime entity text"},
     {"al_type": "document/email", "regex": r"MIME entity, ASCII text"},
     {"al_type": "metadata/sysmon/evt", "regex": r"MS Windows Vista Event Log"},
-    {"al_type": "metadata/sysmon/evt", "regex": r"MS Windows 10-11 Event Log"},
     {"al_type": "metadata/minidump", "regex": r"Mini DuMP crash report"},
     {"al_type": "image/emf", "regex": r"Windows Enhanced Metafile"},
     {"al_type": "resource/msvc", "regex": r"MSVC \.res"},
     {"al_type": "pgp/pubkey", "regex": r"^PGP public key"},
     {"al_type": "pgp/privkey", "regex": r"^PGP private key block"},
     {"al_type": "pgp/encrypted", "regex": r"^PGP RSA encrypted session key"},
     {"al_type": "pgp/message", "regex": r"^PGP message Public-Key Encrypted Session Key"},
@@ -258,16 +254,14 @@
     # But it is good enough to confirm that the type is at least text/plain.
     # A type of text/plain will then get sent to the yara identification stage.
     "text/x-java": "text/plain",
     # Batch
     "text/x-msdos-batch": "code/batch",
     # Registry file
     "text/x-ms-regedit": "text/windows/registry",
-    # Sysmon EVTX file
-    "metadata/sysmon/evt": "application/x-ms-evtx",
     # JSON file
     "application/json": "text/json",
 
     # Autorun files
     "application/x-setupscript": "code/autorun",
     # Bittorrent files
     "application/x-bittorrent": "application/torrent",
@@ -383,17 +377,14 @@
     "application/x-7z-compressed": "archive/7-zip",
     "application/x-bzip2": "archive/bzip2",
     "application/java-archive": "java/jar",
 
     # JAVA Class
     "application/x-java-applet": "java/class",
 
-    # EPUB
-    "application/epub+zip": "document/epub",
-
     # Packet capture
     "application/vnd.tcpdump.pcap": "network/tcpdump",
 
     "message/rfc822": "document/email",
     "text/calendar": "text/calendar",
     "application/x-mach-binary": "executable/mach-o",
     "application/x-iso9660-image": "archive/iso",
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/iprange.py` & `assemblyline-4.5.1.dev8/assemblyline/common/iprange.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/isotime.py` & `assemblyline-4.5.1.dev8/assemblyline/common/isotime.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/log.py` & `assemblyline-4.5.1.dev8/assemblyline/common/log.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/logformat.py` & `assemblyline-4.5.1.dev8/assemblyline/common/logformat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/lucene.lark` & `assemblyline-4.5.1.dev8/assemblyline/common/lucene.lark`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/memory_zip.py` & `assemblyline-4.5.1.dev8/assemblyline/common/memory_zip.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/metrics.py` & `assemblyline-4.5.1.dev8/assemblyline/common/metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/net.py` & `assemblyline-4.5.1.dev8/assemblyline/common/net.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/net_static.py` & `assemblyline-4.5.1.dev8/assemblyline/common/net_static.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/path.py` & `assemblyline-4.5.1.dev8/assemblyline/common/path.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/postprocess.py` & `assemblyline-4.5.1.dev8/assemblyline/common/postprocess.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/random_user.py` & `assemblyline-4.5.1.dev8/assemblyline/common/random_user.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/security.py` & `assemblyline-4.5.1.dev8/assemblyline/common/security.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/signaturing.py` & `assemblyline-4.5.1.dev8/assemblyline/common/signaturing.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/str_utils.py` & `assemblyline-4.5.1.dev8/assemblyline/common/str_utils.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/tag_safelist.yml` & `assemblyline-4.5.1.dev8/assemblyline/common/tag_safelist.yml`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/tagging.py` & `assemblyline-4.5.1.dev8/assemblyline/common/tagging.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/threading.py` & `assemblyline-4.5.1.dev8/assemblyline/common/threading.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/common/uid.py` & `assemblyline-4.5.1.dev8/assemblyline/common/uid.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/datasource/al.py` & `assemblyline-4.5.1.dev8/assemblyline/datasource/al.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/datasource/alert.py` & `assemblyline-4.5.1.dev8/assemblyline/datasource/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/datasource/common.py` & `assemblyline-4.5.1.dev8/assemblyline/datasource/common.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/datastore/bulk.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/bulk.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/datastore/collection.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -666,39 +666,28 @@
 
                 # Shrink/split the temporary index into the original index
                 logger.info(f"Perform shard fix operation from {temp_name.upper()} to {index.upper()}.")
                 self._safe_index_copy(method, temp_name, index, settings=settings)
 
                 # Make the original index the new alias
                 logger.info(f"Make {index.upper()} the current alias for {name.upper()} "
-                            f"but {temp_name.upper()} is not part of the alias anymore.")
-                actions = [
-                    {"add":  {"index": index, "alias": name, "is_write_index": True}},
-                    {"remove":  {"index": temp_name, "alias": name}}
-                ]
+                            f"and delete {temp_name.upper()}.")
+                actions = [{"add":  {"index": index, "alias": name}}, {
+                    "remove_index": {"index": temp_name}}]
                 self.with_retries(self.datastore.client.indices.update_aliases, actions=actions)
 
             # Restore writes
             logger.info("Restore datastore wide write operation on Elastic.")
             self.with_retries(self.datastore.client.indices.put_settings, index=name, settings=write_unblock_settings)
 
             # Restore normal routing and replicas
             logger.info(f"Restore original routing table for {name.upper()}.")
             self.with_retries(self.datastore.client.indices.put_settings, index=name,
                               settings=clone_finish_settings)
 
-            # Make 100% sure new fixed index is ready
-            logger.info(f"Waiting for {index.upper()} status to be GREEN.")
-            self._wait_for_status(index, 'green')
-
-            # Make sure the temporary index is deleted
-            if self.with_retries(self.datastore.client.indices.exists, index=temp_name):
-                logger.info(f"Delete extra {temp_name.upper()} index.")
-                self.with_retries(self.datastore.client.indices.delete, index=temp_name)
-
     def reindex(self, index_type=None):
         """
         This function triggers a reindex of the current index, this should almost never be used because:
             1. There is no crash recovery
             2. Even if the system is still accessible during that time the data is partially accessible
 
         :param index_type: Type of indices to target
@@ -1917,21 +1906,21 @@
                 'total': int(collapsed['inner_hits']['group']['hits']['total']['value']),
                 'items': [self._format_output(row, field_list, as_obj=as_obj)
                           for row in collapsed['inner_hits']['group']['hits']['hits']]
             } for collapsed in result['hits']['hits']]
         }
 
     @staticmethod
-    def _get_odm_type(ds_type: str):
+    def _get_odm_type(ds_type):
         try:
             return back_mapping[ds_type].__name__.lower()
         except KeyError:
             return ds_type.lower()
 
-    def fields(self) -> dict[str, dict[str, Any]]:
+    def fields(self):
         """
         This function should return all the fields in the index with their types
 
         :return:
         """
 
         def flatten_fields(props):
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/datastore/exceptions.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/exceptions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/datastore/helper.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 
 import concurrent.futures
 import elasticapm
 import json
 import os
 
 from datetime import datetime
-from typing import List, Union, Optional, Any, Tuple
+from typing import List, Union
 
 from assemblyline.common import forge
 from assemblyline.common.classification import InvalidClassification
 from assemblyline.common.dict_utils import flatten, recursive_update
 from assemblyline.common.isotime import now_as_iso
 from assemblyline.common.tagging import tag_dict_to_ai_list
 from assemblyline.common.uid import get_id_from_data
 from assemblyline.datastore.collection import ESCollection, log
 from assemblyline.datastore.exceptions import MultiKeyError, VersionConflictException
 from assemblyline.datastore.store import ESStore
 from assemblyline.filestore import FileStore
-from assemblyline.odm import DATEFORMAT, Model, Date
+from assemblyline.odm import DATEFORMAT, Model
 from assemblyline.odm.models.alert import Alert
 from assemblyline.odm.models.badlist import Badlist
 from assemblyline.odm.models.cached_file import CachedFile
 from assemblyline.odm.models.emptyresult import EmptyResult
 from assemblyline.odm.models.error import Error
 from assemblyline.odm.models.file import File
 from assemblyline.odm.models.filescore import FileScore
@@ -1401,71 +1401,7 @@
                 output.append(key)
                 processed_sha256.append(sha256)
 
             if len(processed_sha256) >= 10:
                 break
 
         return output
-
-
-class MetadataValidator:
-    """
-    Type mismatched metadata recived by ingestion can cause us to suffer
-    errors in ingester when it goes to save the submission.
-    
-    This class aims to limit those errors by offering limited validation
-    at the time of the API call, letting the user get a reasonable error instead.
-    """
-    def __init__(self, datastore: AssemblylineDatastore) -> None:
-        self.datastore = datastore
-        self.metadata = forge.CachedObject(self.get_metadata, refresh=60 * 20)
-
-    def get_metadata(self) -> dict[str, dict[str, Any]]:
-        """Fetch the type mapping for submission metadata."""
-        fields = self.datastore.submission.fields()
-        selected = {}
-        for key, value in fields.items():
-            prefix, _, key = key.partition('.')
-            if prefix == 'metadata':
-                selected[key] = value
-        return selected
-
-    def check_metadata(self, metadata: dict[str, Any]) -> Optional[Tuple[str, str]]:
-        """
-        Check if the type of every metedata field for obvious errors.
-
-        This isn't meant to be comprehensive, just to cover the types that most frequently
-        cause issues for us.
-
-        Return a tuple of (key name, error message) if any problems are detected.
-        """
-        for key, value in metadata.items():
-            try:
-                type_name = self.metadata[key]["type"]
-                if type_name == 'integer':
-                    try:
-                        number = int(value)
-                        if number < -(2 ** 31) or number > (2 ** 31 - 1):
-                            return (key, f'Metadata field {key} only supports signed 32 bit values')
-                    except ValueError:
-                        return (key, f'Metadata field {key} expected a number, received "{value}" instead')
-                elif type_name == 'date':
-                    try:
-                        int(value)
-                        return (key, f'Metadata field {key} expected a date, refusing to coerce a number')
-                    except Exception:
-                        pass
-                    try:
-                        value = Date().check(value)
-                        if value is None:
-                            raise ValueError()
-                        metadata[key] = value.strftime(DATEFORMAT)
-                    except Exception:
-                        return (key, f'Metadata field {key} expected a date, received "{value}" instead')
-                else:
-                    # Everything else seems fine so far
-                    pass
-            except KeyError:
-                pass
-
-        # No problems encountered
-        return None
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/datastore/store.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/store.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/datastore/support/build.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/support/build.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/datastore/support/schemas.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/support/schemas.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/filestore/__init__.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/filestore/transport/azure.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/azure.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/filestore/transport/base.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/base.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/filestore/transport/ftp.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/ftp.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/filestore/transport/http.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/http.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/filestore/transport/local.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/local.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/filestore/transport/s3.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/s3.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/filestore/transport/sftp.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/sftp.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/__init__.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/base.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # noinspection PyProtectedMember
     copy._deepcopy_dispatch[type(re.compile(''))] = lambda r, _: r
 
 BANNED_FIELDS = {"id", "__access_grp1__", "__access_lvl__", "__access_req__", "__access_grp2__"}
 DATEFORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
 FIELD_SANITIZER = re.compile("^[a-z][a-z0-9_]*$")
 FLATTENED_OBJECT_SANITIZER = re.compile("^[a-z][a-z0-9_.]*$")
-NOT_INDEXED_SANITIZER = re.compile("^[A-Za-z0-9_ -.]*$")
+NOT_INDEXED_SANITIZER = re.compile("^[A-Za-z0-9_ -]*$")
 UTC_TZ = tzutc()
 
 DOMAIN_REGEX = r"(?:(?:[A-Za-z0-9\u00a1-\U0010ffff][A-Za-z0-9\u00a1-\U0010ffff_-]{0,62})?" \
                r"[A-Za-z0-9\u00a1-\U0010ffff]\.)+(?:[Xx][Nn]--)?(?:[A-Za-z0-9\u00a1-\U0010ffff]{2,}\.?)"
 DOMAIN_ONLY_REGEX = f"^{DOMAIN_REGEX}$"
 DOMAIN_EXCLUDED_NORM_CHARS = './?@#'
 EMAIL_REGEX = f"^[a-zA-Z0-9!#$%&'*+/=?^_‘{{|}}~-]+(?:\\.[a-zA-Z0-9!#$%&'*+/=?^_‘{{|}}~-]+)*@({DOMAIN_REGEX})$"
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/alert.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/alerter_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/alerter_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/archive_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/archive_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/changes.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/changes.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/dispatcher_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/dispatcher_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/dispatching.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/dispatching.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/expiry_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/expiry_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/ingest_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/ingest_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/metrics.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/retrohunt_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/vacuum_heartbeat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from assemblyline import odm
 
-MSG_TYPES = {"RetrohuntHeartbeat"}
-LOADER_CLASS = "assemblyline.odm.messages.retrohunt_heartbeat.RetrohuntMessage"
+MSG_TYPES = {"VacuumHeartbeat"}
+LOADER_CLASS = "assemblyline.odm.messages.vacuum_heartbeat.VacuumMessage"
 
 
-@odm.model(description="Heartbeat Model for retrohunt")
+@odm.model(description="Vacuum Stats")
+class Metrics(odm.Model):
+    ingested = odm.Integer(description="Files ingested")
+    # protocol = odm.Mapping(odm.Integer())
+    safelist = odm.Integer(description="Files safelisted")
+    errors = odm.Integer()
+    skipped = odm.Integer()
+
+
+@odm.model(description="Heartbeat Model")
 class Heartbeat(odm.Model):
-    instances = odm.Integer(description="Number of retrohunt workers")
-    request_time = odm.Float(description="Time to load metrics")
-    pending_files = odm.integer(description="Files not yet available for searching")
-    ingested_last_minute = odm.integer(description="Files ingested in last minute")
-    worker_storage_available = odm.integer(description="Free storage for most depleted worker")
-    total_storage_available = odm.integer(description="Free storage across workers")
-    active_searches = odm.integer(description="Number of currently running searches")
-    last_minute_cpu = odm.Float(description="Last minute cpu load across all workers")
-    total_memory_used = odm.Float(description="Estimated current memory use across all workers")
+    # instances = odm.Integer(description="Number of instances")
+    metrics = odm.Compound(Metrics, description="Vacuum metrics")
+    # queues = odm.Compound(Metrics, description="Vacuum queues")
 
 
-@odm.model(description="Model of retrohunt heartbeat message")
-class RetrohuntMessage(odm.Model):
-    msg = odm.Compound(Heartbeat, description="Heartbeat message for retrohunt")
+@odm.model(description="Model of Vacuum Heartbeat Message")
+class VacuumMessage(odm.Model):
+    msg = odm.Compound(Heartbeat, description="Hearbeat message")
     msg_loader = odm.Enum(values={LOADER_CLASS}, default=LOADER_CLASS, description="Loader class for message")
-    msg_type = odm.Enum(values=MSG_TYPES, default="RetrohuntHeartbeat", description="Type of message")
+    msg_type = odm.Enum(values=MSG_TYPES, default="VacuumHeartbeat", description="Type of message")
     sender = odm.Keyword(description="Sender of message")
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/scaler_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/scaler_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/scaler_status_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/scaler_status_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/service_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/service_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/service_timing_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/service_timing_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/submission.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/submission.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/messages/task.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/task.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/actions.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/actions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/alert.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,24 +149,20 @@
 
 @odm.model(index=True, store=False, description="Model of Workflow Event")
 class Event(odm.Model):
     entity_type: str = odm.Enum(values=['user', 'workflow'], description="Type of entity associated to event")
     entity_id: str = odm.Keyword(description="ID of entity associated to event")
     entity_name: str = odm.Keyword(description="Name of entity")
     ts: str = odm.Date(default="NOW", description="Timestamp of event")
-    labels: List[str] = odm.sequence(odm.keyword(), default=[], description="Labels added during event")
-    labels_removed: List[str] = odm.sequence(odm.keyword(), default=[], description="Labels removed during event")
+    labels: List[str] = odm.Optional(odm.List(odm.Keyword()), description="Labels added during event")
     status: str = odm.Optional(odm.Enum(values=STATUSES), description="Status applied during event")
     priority: str = odm.Optional(odm.Enum(values=PRIORITIES), description="Priority applied during event")
 
     def __hash__(self) -> int:
-        data = self.as_primitives()
-        data['labels'] = tuple(sorted(self.labels))
-        data['labels_removed'] = tuple(sorted(self.labels_removed))
-        return hash(tuple(sorted(data.items())))
+        return hash(tuple(sorted(self.as_primitives().items())))
 
 
 @odm.model(index=True, store=True, description="Submission relations for an alert")
 class Relationship(odm.Model):
     child: str = odm.UUID()
     parent: Optional[str] = odm.optional(odm.UUID())
 
@@ -194,15 +190,15 @@
     submission_relations = odm.sequence(odm.compound(Relationship), description="Describes relationships "
                                         "between submissions used to build this alert")
     sid = odm.UUID(description="Submission ID related to this alert")
     status = odm.Optional(odm.Enum(values=STATUSES), description="Status applied to the alert")
     ts = odm.Date(description="File submission timestamp")
     type = odm.Keyword(description="Type of alert")
     verdict = odm.Compound(Verdict, default={}, description="Verdict Block")
-    events = odm.sequence(odm.compound(Event), default=[], description="An audit of events applied to alert")
+    events = odm.List(odm.Compound(Event), default=[], description="An audit of events applied to alert")
     workflows_completed = odm.Boolean(default=False, description="Have all workflows ran on this alert?")
 
     def update(self, other: Alert) -> None:
         """Update the current object given the content of a second alert."""
 
         # Make sure we are merging compatible alerts
         if self.alert_id != other.alert_id:
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/badlist.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/badlist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/config.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, List
 
 from assemblyline import odm
 from assemblyline.odm.models.service import EnvironmentVariable
 from assemblyline.odm.models.service_delta import DockerConfigDelta
 
 
-AUTO_PROPERTY_TYPE = ['access', 'classification', 'type', 'role', 'remove_role', 'group', 'multi_group']
+AUTO_PROPERTY_TYPE = ['access', 'classification', 'type', 'role', 'remove_role', 'group']
 DEFAULT_EMAIL_FIELDS = ['email', 'emails', 'extension_selectedEmailAddress', 'otherMails', 'preferred_username', 'upn']
 
 
 @odm.model(index=False, store=False, description="Password Requirement")
 class PasswordRequirement(odm.Model):
     lower: bool = odm.Boolean(description="Password must contain lowercase letters")
     number: bool = odm.Boolean(description="Password must contain numbers")
@@ -517,85 +517,23 @@
     'elasticsearch': DEFAULT_ES_METRICS,
     'export_interval': 5,
     'redis': DEFAULT_REDIS_NP,
 }
 
 
 @odm.model(index=False, store=False, description="Malware Archive Configuration")
-class ArchiverMetadata(odm.Model):
-    default = odm.Optional(odm.Keyword(description="Default value for the metadata"))
-    editable = odm.Boolean(default=False, description="Can the user provide a custom value")
-    values = odm.List(odm.Keyword(), default=[], description="List of possible values to pick from")
-
-
-EXEMPLE_ARCHIVER_METADATA = {
-    'rationale': {
-        'default': "File is malicious",
-        'editable': True,
-        'values': ["File is malicious", "File is interesting", "I just feel like keeping this..."]
-    }
-}
-
-
-@odm.model(index=False, store=False, description="Named Value")
-class NamedValue(odm.Model):
-    name = odm.Keyword(description="Name")
-    value = odm.Keyword(description="Value")
-
-
-@odm.model(index=False, store=False, description="Webhook Configuration")
-class Webhook(odm.Model):
-    password = odm.Optional(odm.Keyword(default=""), description="Password used to authenticate with source")
-    ca_cert = odm.Optional(odm.Keyword(default=""), description="CA cert for source")
-    ssl_ignore_errors = odm.Boolean(default=False, description="Ignore SSL errors when reaching out to source?")
-    proxy = odm.Optional(odm.Keyword(default=""), description="Proxy server for source")
-    method = odm.Keyword(default='POST', description="HTTP method used to access webhook")
-    uri = odm.Keyword(description="URI to source")
-    username = odm.Optional(odm.Keyword(default=""), description="Username used to authenticate with source")
-    headers = odm.List(odm.Compound(NamedValue), default=[], description="Headers")
-    retries = odm.Integer(default=3)
-
-
-DEFAULT_ARCHIVER_WEBHOOK = {
-    'password': None,
-    'ca_cert': None,
-    'ssl_ignore_errors': False,
-    'proxy': None,
-    'method': "POST",
-    'uri': "https://archiving-hook",
-    'username': None,
-    'headers': [],
-    'retries': 3
-}
-
-
-@odm.model(index=False, store=False, description="Malware Archive Configuration")
 class Archiver(odm.Model):
-    metadata: Dict = odm.Mapping(
-        odm.Compound(ArchiverMetadata),
-        description="Proxy configuration that is passed to Python Requests")
     minimum_required_services: List[str] = odm.List(
         odm.keyword(),
         default=[],
         description="List of minimum required service before archiving takes place")
-    webhook = odm.Optional(odm.Compound(Webhook), description="Webhook to call before triggering the archiving process")
-    use_metadata: bool = odm.Boolean(
-        default=False, description="Should the UI ask form metadata to be filed out when archiving")
-    use_webhook: bool = odm.Optional(odm.Boolean(
-        default=False,
-        description="Should the archiving go through the webhook prior to actually trigger the archiving function"))
 
 
 DEFAULT_ARCHIVER = {
-    'metadata': {},
-    'minimum_required_services': [],
-    'use_webhook': False,
-    'use_metadata': False,
-    'webhook': DEFAULT_ARCHIVER_WEBHOOK,
-
+    'minimum_required_services': []
 }
 
 
 @odm.model(index=False, store=False, description="Plumber Configuration")
 class Plumber(odm.Model):
     notification_queue_interval: int = odm.Integer(
         description="Interval at which the notification queue cleanup should run")
@@ -739,16 +677,14 @@
 
 
 @odm.model(index=False, store=False)
 class RegistryConfiguration(odm.Model):
     name: str = odm.Text(description="Name of container registry")
     proxies: Dict = odm.Optional(odm.Mapping(odm.Text()),
                                  description="Proxy configuration that is passed to Python Requests")
-    token_server: str = odm.Optional(odm.Text(),
-                                     description="Token server name to facilitate anonymous pull access")
 
 
 @odm.model(index=False, store=False)
 class Updater(odm.Model):
     job_dockerconfig: DockerConfigDelta = odm.Compound(
         DockerConfigDelta, description="Container configuration used for service registration/updates")
     registry_configs: List = odm.List(odm.Compound(RegistryConfiguration),
@@ -1082,112 +1018,94 @@
     options: Dict[str, str] = odm.Optional(odm.Mapping(odm.Any()),
                                            description="Other kwargs options directly passed to the API.")
 
 
 @odm.model(index=False, store=False, description="AI support configuration block")
 class AI(odm.Model):
     chat_url: str = odm.Keyword(description="URL to the AI API")
-    api_type: str = odm.Enum(values=['openai', 'cohere'], description="Type of chat API we are communicating with")
-    assistant: AIQueryParams = odm.Compound(AIQueryParams, description="Parameters used for Assamblyline Assistant")
     code: AIQueryParams = odm.Compound(AIQueryParams, description="Parameters used for code analysis")
     detailed_report: AIQueryParams = odm.Compound(AIQueryParams, description="Parameters used for detailed reports")
     executive_summary: AIQueryParams = odm.Compound(
         AIQueryParams, description="Parameters used for executive summaries")
     enabled: bool = odm.Boolean(description="Is AI support enabled?")
     headers: Dict[str, str] = odm.Optional(odm.Mapping(odm.Keyword()),
                                            description="Headers used by the _call_ai_backend method")
     model_name: str = odm.Keyword(description="Name of the model to be used for the AI analysis.")
     verify: bool = odm.Boolean(description="Should the SSL connection to the AI API be verified.")
     proxies: Dict[str, str] = odm.Optional(odm.Mapping(odm.Keyword()),
                                            description="Proxies used by the _call_ai_backend method")
 
 
-DEFAULT_AI_ASSISTANT = {
-    'system_message': """
-You are the Assemblyline AI Assistant, you are here to help users understand the results produced by Assemblyline.
-""",
-    'max_tokens': 1024,
-    'options': {
-        "frequency_penalty": 0,
-        "presence_penalty": 0,
-        "temperature": 0,
-        "top_p": 0
-    }
-}
-
-
 DEFAULT_AI_CODE = {
     'system_message': """
 You are an assistant that provides explanation of code snippets found in AssemblyLine,
 a malware detection and analysis tool. Start by providing a short summary of the intent behind the
 code and then follow with a detailed explanation of what the code is doing. Format your explanation
-using the Markdown syntax. Your answer must be written in plain $(LANG).
+using the Markdown syntax.
 
 User: print("Hello World!")
 Assistant:
 ## Summary
 The given code is printing "Hello World!" to the console.
 ## Details
 The code has only one line of code and prints a string to the console using the print() function.
 """,
     'max_tokens': 1024,
     'options': {
         "frequency_penalty": 0,
         "presence_penalty": 0,
-        "temperature": 0,
-        "top_p": 0
+        "temperature": 1,
+        "top_p": 1
     }
 }
 
 DEFAULT_AI_DETAILED_REPORT = {
     'system_message': """
 You are an assistant that summarizes the output of AssemblyLine, a malware detection and analysis tool.  Your role is
 to extract information of importance and discard what is not. Assemblyline uses a scoring mechanism where any scores
 below 0 is considered safe, scores between 0 and 300 are considered informational, scores between 300 and 700 are
 considered suspicious, scores between 700 and 1000 are considered highly-suspicious and scores with 1000 points and
 up are considered malicious.
 
-Once YAML has been submitted, the user expects a two-part result in plain $(LANG)..  The first part is a one or two
+Once YAML has been submitted, the user expects a two-part result in plain English.  The first part is a one or two
 paragraph executive summary which provides some highlights of the results, and the second part is a detailed description
 of the observations found in the report.  Format your answer using the Markdown syntax.
 """,
     'max_tokens': 2048,
     'options': {
         "frequency_penalty": 0,
         "presence_penalty": 0,
-        "temperature": 0,
-        "top_p": 0
+        "temperature": 1,
+        "top_p": 1
     }
 }
 
 DEFAULT_AI_EXECUTIVE_SUMMARY = {
     "system_message": """
 You are an assistant that summarizes the output of AssemblyLine, a malware detection and analysis tool. Your role
 is to extract information of importance and discard what is not.  Assemblyline uses a scoring mechanism where any scores
 below 0 is considered safe, scores between 0 and 300 are considered informational, scores between 300 and 700 are
 considered suspicious, scores between 700 and 1000 are considered highly-suspicious and scores with 1000 points and up
 are considered malicious.
 
 Once YAML has been submitted, the user expects a one or two paragraph executive summary of the output of AssemblyLine in
-plain $(LANG)..  Highlight important information using inline code block from the Markdown syntax.
+plain English.  Highlight important information using inline code block from the Markdown syntax.
 """,
     'max_tokens': 512,
     'options': {
         "frequency_penalty": 0,
         "presence_penalty": 0,
-        "temperature": 0,
-        "top_p": 0
+        "temperature": 1,
+        "top_p": 1
     }
 }
 
 
 DEFAULT_AI = {
     'chat_url': "https://api.openai.com/v1/chat/completions",
-    'api_type': "openai",
-    'assistant': DEFAULT_AI_ASSISTANT,
     'code': DEFAULT_AI_CODE,
     'detailed_report': DEFAULT_AI_DETAILED_REPORT,
     'executive_summary': DEFAULT_AI_EXECUTIVE_SUMMARY,
     'enabled': False,
     'headers': {
         "Content-Type": "application/json"
     },
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/error.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/error.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/file.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/file.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/filescore.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/filescore.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/heuristic.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/heuristic.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/filetypes/pe.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/filetypes/pe.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/ontology.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/antivirus.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/antivirus.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/malware_config.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/malware_config.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/network.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/network.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/process.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/process.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/sandbox.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/sandbox.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/ontology/results/signature.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/signature.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/replay.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/result.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/result.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/retrohunt.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/retrohunt.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/safelist.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/safelist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/service.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     'file': '',
     'custom': ''
 }
 
 
 @odm.model(index=False, store=False, description="Environment Variable Model")
 class EnvironmentVariable(odm.Model):
-    name: str = odm.keyword(description="Name of Environment Variable")
-    value: str = odm.keyword(description="Value of Environment Variable")
+    name: str = odm.Keyword(description="Name of Environment Variable")
+    value: str = odm.Keyword(description="Value of Environment Variable")
 
 
 @odm.model(index=False, store=False, description="Docker Container Configuration")
 class DockerConfig(odm.Model):
     allow_internet_access: bool = odm.Boolean(default=False, description="Does the container have internet-access?")
     command: Opt[list[str]] = odm.Optional(odm.List(odm.Keyword()),
                                            description="Command to run when container starts up.")
@@ -36,19 +36,19 @@
     image: str = odm.Keyword(description="Complete name of the Docker image with tag, may include registry")
     registry_username: Opt[str] = odm.Optional(odm.Keyword(default=""),
                                                description="The username to use when pulling the image")
     registry_password: Opt[str] = odm.Optional(odm.Keyword(default=""),
                                                description="The password or token to use when pulling the image")
     registry_type: str = odm.Enum(values=["docker", "harbor"], default='docker',
                                   description="The type of container registry")
+    operating_system: str = odm.Enum(values=['windows', 'linux'], default="linux", description="What operating system does this container run under?")
     ports: list[str] = odm.List(odm.Keyword(), default=[], description="What ports of container to expose?")
     ram_mb: int = odm.Integer(default=512, description="Container RAM limit")
     ram_mb_min: int = odm.Integer(default=256, description="Container RAM request")
     service_account = odm.optional(odm.keyword(description="Service account to use for pods in kubernetes"))
-    labels = odm.sequence(odm.compound(EnvironmentVariable), default=[], description="Additional container labels.")
 
 
 @ odm.model(index=False, store=False, description="Container's Persistent Volume Configuration")
 class PersistentVolume(odm.Model):
     mount_path = odm.Keyword(description="Path into the container to mount volume")
     capacity = odm.Keyword(description="The amount of storage allocated for volume")
     storage_class = odm.Keyword(description="Storage class used to create volume")
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/service_delta.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/service_delta.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     command = odm.Optional(odm.List(odm.Keyword()), description=REF_DOCKER_CONFIG)
     cpu_cores = odm.Optional(odm.Float(), description=REF_DOCKER_CONFIG)
     environment = odm.Optional(odm.List(odm.Compound(EnvironmentVariable)), description=REF_DOCKER_CONFIG)
     image = odm.Optional(odm.Keyword(), description=REF_DOCKER_CONFIG)
     registry_username = odm.Optional(odm.Keyword(default=""), description=REF_DOCKER_CONFIG)
     registry_password = odm.Optional(odm.Keyword(default=""), description=REF_DOCKER_CONFIG)
     registry_type = odm.Optional(odm.Enum(values=["docker", "harbor"]), description=REF_DOCKER_CONFIG)
+    operating_system = odm.Optional(odm.Enum(values=['windows', 'linux']), description=REF_DOCKER_CONFIG)
     ports = odm.Optional(odm.List(odm.Keyword()), description=REF_DOCKER_CONFIG)
     ram_mb = odm.Optional(odm.Integer(), description=REF_DOCKER_CONFIG)
     ram_mb_min = odm.Optional(odm.Integer(), description=REF_DOCKER_CONFIG)
     service_account = odm.optional(odm.keyword(description=REF_DOCKER_CONFIG))
-    labels = odm.Optional(odm.List(odm.Compound(EnvironmentVariable)), description=REF_DOCKER_CONFIG)
 
 
 @odm.model(index=False, store=False)
 class UpdateSourceDelta(odm.Model):
     name = odm.Optional(odm.Keyword(), description=REF_UPDATE_SOURCE)
     password = odm.Optional(odm.Keyword(default=""), description=REF_UPDATE_SOURCE)
     pattern = odm.Optional(odm.Keyword(default=""), description=REF_UPDATE_SOURCE)
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/signature.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/signature.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/statistics.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/statistics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/submission.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/submission.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/submission_summary.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/submission_summary.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/submission_tree.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/submission_tree.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/tagging.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/tagging.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/user.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     ("self_manage", 27),
     ("retrohunt_view", 28),
     ("retrohunt_run", 29),
     ("external_query", 30),
     ("badlist_view", 31),
     ("badlist_manage", 32),
     ("archive_comment", 33),
-    ("assistant_use", 34),
 ])
 
 
 SCOPES = {"r", "w", "rw", "c"}
 USER_TYPES = [
     TYPES.admin,               # Perform administartive task and has access to all roles
     TYPES.user,                # Normal user of the system
@@ -100,15 +99,14 @@
 
 USER_ROLES = USER_ROLES_BASIC.union({
     ROLES.administration,      # Perform administrative tasks
     ROLES.file_purge,          # Purge files from the filestore
     ROLES.replay_system,       # Manage status of file/submission/alerts during the replay process
     ROLES.signature_import,    # Import signatures in the system
     ROLES.signature_manage,    # Manage signatures sources in the system
-    ROLES.assistant_use,       # Use the Assemblyline Assistant
 })
 
 USER_TYPE_DEP = {
     TYPES.admin: USER_ROLES,
     TYPES.signature_importer: {
         ROLES.badlist_manage,
         ROLES.safelist_manage,
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/user_favorites.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/user_favorites.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/user_settings.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/user_settings.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/models/workflow.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/workflow.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/random_data/__init__.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/random_data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         pass
 
 
 def create_alerts(ds, alert_count=50, submission_list=None, log=None, workflows=[]):
     for _ in range(alert_count):
         a: Alert = random_model_obj(Alert)
         a.expiry_ts = now_as_iso(60 * 60 * 24 * 14)
-        a.label = list(set(a.label))
         if isinstance(submission_list, list):
             submission = random.choice(submission_list)
             a.file.sha256 = submission.files[0].sha256
             a.sid = submission.sid
 
         a.owner = random.choice(['admin', 'user', 'other', None])
         if workflows:
@@ -68,15 +67,15 @@
                     event.entity_type = 'workflow'
                     event.entity_name = wf.name
                     event.entity_id = wf.workflow_id
                 else:
                     # Overwrite with user information
                     event.entity_type = 'user'
                     event.entity_id = get_random_word()
-                event.labels = list(set([get_random_word() for _ in range(random.randint(0, 20))]))
+                event.labels = [get_random_word() for _ in range(random.randint(0, 20))]
                 event.status = random.choice(list(STATUSES) + [None])
                 event.priority = random.choice(list(PRIORITIES) + [None])
                 return event
             a.events = [generate_workflow_event(random.choice(workflows)) for _ in range(random.randint(0, 5))]
 
         # Clear sub-types
         for data_type in a.al.detailed.fields():
@@ -433,15 +432,14 @@
         sl['hashes']['sha256'] = "0" + get_random_hash(63)
         ds.safelist.save(sl['hashes']['sha256'], sl)
         if log:
             log.info(f"\t{sl['hashes']['sha256']}")
 
     ds.safelist.commit()
 
-
 def create_workflows(ds, count=20, log=None):
     workflows = []
     for _ in range(count):
         w_id = get_random_id()
         workflow = random_model_obj(Workflow)
         workflow.workflow_id = w_id
         ds.workflow.save(w_id, workflow)
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/random_data/create_test_data.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/random_data/create_test_data.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/random_data/sample_rules.yar` & `assemblyline-4.5.1.dev8/assemblyline/odm/random_data/sample_rules.yar`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/random_data/sample_suricata.rules` & `assemblyline-4.5.1.dev8/assemblyline/odm/random_data/sample_suricata.rules`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/odm/randomizer.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/randomizer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/__init__.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/cache.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/cache.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/counters.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/counters.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/events.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/events.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/exporting_counter.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/exporting_counter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/hash.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/hash.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/lock.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/lock.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/queues/comms.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/comms.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/queues/multi.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/multi.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/queues/named.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/named.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/queues/priority.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/priority.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/set.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/set.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/remote/datatypes/user_quota_tracker.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/user_quota_tracker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/run/cli.py` & `assemblyline-4.5.1.dev8/assemblyline/run/cli.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/run/pubsub_reader.py` & `assemblyline-4.5.1.dev8/assemblyline/run/pubsub_reader.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/run/suricata_importer.py` & `assemblyline-4.5.1.dev8/assemblyline/run/suricata_importer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline/run/yara_importer.py` & `assemblyline-4.5.1.dev8/assemblyline/run/yara_importer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev76/assemblyline.egg-info/PKG-INFO` & `assemblyline-4.5.1.dev8/assemblyline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline
-Version: 4.5.1.dev76
+Version: 4.5.1.dev8
 Summary: Assemblyline 4 - Automated malware analysis framework
 Home-page: https://github.com/CybercentreCanada/assemblyline-base
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-4.5.1.dev76/assemblyline.egg-info/SOURCES.txt` & `assemblyline-4.5.1.dev8/assemblyline.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,18 @@
 assemblyline/odm/messages/archive_heartbeat.py
 assemblyline/odm/messages/changes.py
 assemblyline/odm/messages/dispatcher_heartbeat.py
 assemblyline/odm/messages/dispatching.py
 assemblyline/odm/messages/expiry_heartbeat.py
 assemblyline/odm/messages/ingest_heartbeat.py
 assemblyline/odm/messages/metrics.py
-assemblyline/odm/messages/retrohunt_heartbeat.py
 assemblyline/odm/messages/scaler_heartbeat.py
 assemblyline/odm/messages/scaler_status_heartbeat.py
 assemblyline/odm/messages/service_heartbeat.py
 assemblyline/odm/messages/service_timing_heartbeat.py
-assemblyline/odm/messages/shard_heartbeat.py
 assemblyline/odm/messages/submission.py
 assemblyline/odm/messages/task.py
 assemblyline/odm/messages/vacuum_heartbeat.py
 assemblyline/odm/models/__init__.py
 assemblyline/odm/models/actions.py
 assemblyline/odm/models/alert.py
 assemblyline/odm/models/badlist.py
```

### Comparing `assemblyline-4.5.1.dev76/setup.py` & `assemblyline-4.5.1.dev8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,15 @@
         'notifications-python-client',
         # Blacklist a bad release of the azure library until a release newer than that comes out
         'azure-storage-blob!=12.4.0',
         'azure-identity',
         'msoffcrypto-tool',
         'chardet',
         'yara-python',
-        'python-tlsh',
-        'hauntedhouse==0.1.10',
+        'python-tlsh'
     ],
     extras_require={
         'test': [
             'pytest',
             'retrying',
             'pytest-mock',
             'pyftpdlib',
```

