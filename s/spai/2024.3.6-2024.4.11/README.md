# Comparing `tmp/spai-2024.3.6.tar.gz` & `tmp/spai-2024.4.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2024.3.6.tar", max compression
+gzip compressed data, was "spai-2024.4.11.tar", max compression
```

## Comparing `spai-2024.3.6.tar` & `spai-2024.4.11.tar`

### file list

```diff
@@ -1,119 +1,131 @@
--rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2024.3.6/README.md
--rw-r--r--   0        0        0      525 2024-03-06 15:54:23.315452 spai-2024.3.6/pyproject.toml
--rw-r--r--   0        0        0       27 2024-03-06 15:54:23.319452 spai-2024.3.6/spai/__init__.py
--rw-r--r--   0        0        0       96 2024-02-13 11:22:06.401893 spai-2024.3.6/spai/auth/__init__.py
--rw-r--r--   0        0        0     1210 2024-02-13 11:22:06.401893 spai-2024.3.6/spai/auth/auth.py
--rw-r--r--   0        0        0       99 2024-02-13 11:22:06.401893 spai-2024.3.6/spai/auth/is_logged.py
--rw-r--r--   0        0        0      161 2024-02-13 11:22:06.401893 spai-2024.3.6/spai/auth/logout.py
--rw-r--r--   0        0        0     7202 2024-03-06 15:37:54.446375 spai-2024.3.6/spai/cli.py
--rw-r--r--   0        0        0        0 2024-02-13 11:22:06.401893 spai-2024.3.6/spai/commands/__init__.py
--rw-r--r--   0        0        0     1017 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/commands/auth.py
--rw-r--r--   0        0        0     1160 2024-02-20 14:18:54.846405 spai-2024.3.6/spai/commands/list.py
--rw-r--r--   0        0        0       86 2024-03-06 14:18:56.276043 spai-2024.3.6/spai/config/__init__.py
--rw-r--r--   0        0        0     3583 2024-02-21 11:07:14.523625 spai-2024.3.6/spai/config/validate.py
--rw-r--r--   0        0        0     1324 2024-03-06 14:57:48.814599 spai-2024.3.6/spai/config/vars.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2024.3.6/spai/data/__init__.py
--rw-r--r--   0        0        0       49 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/data/indices/__init__.py
--rw-r--r--   0        0        0       54 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/data/indices/fwi/__init__.py
--rw-r--r--   0        0        0     3234 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/data/indices/fwi/fwi_nasa.py
--rw-r--r--   0        0        0      128 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     3941 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/data/satellite/download.py
--rw-r--r--   0        0        0      647 2023-10-30 11:07:40.852696 spai-2024.3.6/spai/data/satellite/explore.py
--rw-r--r--   0        0        0      725 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py
--rw-r--r--   0        0        0      758 2024-02-20 09:51:03.207114 spai-2024.3.6/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py
--rw-r--r--   0        0        0      758 2024-02-20 09:51:03.207114 spai-2024.3.6/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py
--rw-r--r--   0        0        0      758 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/data/satellite/sentinelhub/SHDEM30Downloader.py
--rw-r--r--   0        0        0     3587 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2584 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2024.3.6/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1264 2023-10-30 11:07:40.856696 spai-2024.3.6/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2024.3.6/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2024.3.6/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      282 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0     6275 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/data/satellite/utils.py
--rw-r--r--   0        0        0       84 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/data/vector/__init__.py
--rw-r--r--   0        0        0     5533 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/data/vector/openstreetmap.py
--rw-r--r--   0        0        0       71 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/errors/__init__.py
--rw-r--r--   0        0        0      308 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/errors/auth.py
--rw-r--r--   0        0        0      156 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/errors/mails.py
--rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2024.3.6/spai/image/__init__.py
--rw-r--r--   0        0        0     1350 2023-10-30 11:07:40.856696 spai-2024.3.6/spai/image/utils.py
--rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2024.3.6/spai/image/xyz/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2024.3.6/spai/image/xyz/cache.py
--rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2024.3.6/spai/image/xyz/errors.py
--rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2024.3.6/spai/image/xyz/get_image_tile.py
--rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2024.3.6/spai/image/xyz/image_utils.py
--rw-r--r--   0        0        0       28 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/mails/__init__.py
--rw-r--r--   0        0        0     1334 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/mails/mimetypes.py
--rw-r--r--   0        0        0     2932 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/mails/send.py
--rw-r--r--   0        0        0     3305 2024-02-20 15:56:27.665877 spai-2024.3.6/spai/models/Config.py
--rw-r--r--   0        0        0      984 2024-02-20 14:34:35.914586 spai-2024.3.6/spai/models/StorageConfig.py
--rw-r--r--   0        0        0       27 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/models/__init__.py
--rw-r--r--   0        0        0      391 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/processing/__init__.py
--rw-r--r--   0        0        0      461 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/processing/autocategorize1D.py
--rw-r--r--   0        0        0      477 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/processing/colorize_raster.py
--rw-r--r--   0        0        0      932 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/processing/convert_array_to_vector.py
--rw-r--r--   0        0        0      291 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/processing/mask_raster.py
--rw-r--r--   0        0        0      682 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/processing/normalised_difference.py
--rw-r--r--   0        0        0     1239 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/processing/px_count.py
--rw-r--r--   0        0        0      107 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/processing/rasterio_mask.py
--rw-r--r--   0        0        0      266 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/processing/read_raster.py
--rw-r--r--   0        0        0      876 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/processing/save_table.py
--rw-r--r--   0        0        0      475 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/project/__init__.py
--rw-r--r--   0        0        0      466 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/project/bck/GetLogs.py
--rw-r--r--   0        0        0     1018 2024-02-20 09:51:03.207114 spai-2024.3.6/spai/project/bck/InstallReqs 2.py
--rw-r--r--   0        0        0     1018 2024-02-20 09:51:03.207114 spai-2024.3.6/spai/project/bck/InstallReqs 3.py
--rw-r--r--   0        0        0      482 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/project/bck/RunService.py
--rw-r--r--   0        0        0      492 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/project/bck/ScheduleService.py
--rw-r--r--   0        0        0      510 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/project/bck/StopService.py
--rw-r--r--   0        0        0     1578 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/project/bck/main.py
--rw-r--r--   0        0        0      337 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/project/delete_project.py
--rw-r--r--   0        0        0     2061 2024-03-06 14:29:37.312605 spai-2024.3.6/spai/project/deploy_folder.py
--rw-r--r--   0        0        0      516 2024-03-06 14:19:55.532601 spai-2024.3.6/spai/project/deploy_template.py
--rw-r--r--   0        0        0     1203 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/project/download_template.py
--rw-r--r--   0        0        0      455 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/project/get_logs.py
--rw-r--r--   0        0        0      242 2024-02-13 11:22:06.405893 spai-2024.3.6/spai/project/get_project_by_name.py
--rw-r--r--   0        0        0      172 2024-02-13 11:22:06.409893 spai-2024.3.6/spai/project/get_projects.py
--rw-r--r--   0        0        0      344 2024-02-13 11:22:06.409893 spai-2024.3.6/spai/project/get_service_by_name_type_project.py
--rw-r--r--   0        0        0     1616 2024-03-05 14:14:16.187189 spai-2024.3.6/spai/project/get_services.py
--rw-r--r--   0        0        0      525 2024-02-21 09:43:40.417670 spai-2024.3.6/spai/project/init_project.py
--rw-r--r--   0        0        0      726 2024-02-20 15:56:19.617848 spai-2024.3.6/spai/project/install_requirements.py
--rw-r--r--   0        0        0     5617 2024-02-27 12:31:33.913016 spai-2024.3.6/spai/project/project-template/README.md
--rw-r--r--   0        0        0      867 2024-02-27 12:31:32.377011 spai-2024.3.6/spai/project/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0       36 2024-02-27 12:31:32.377011 spai-2024.3.6/spai/project/project-template/apis/analytics/requirements.txt
--rw-r--r--   0        0        0     1800 2024-02-27 12:31:32.381011 spai-2024.3.6/spai/project/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0       88 2024-02-27 12:31:32.381011 spai-2024.3.6/spai/project/project-template/apis/xyz/requirements.txt
--rw-r--r--   0        0        0   748531 2024-02-27 12:31:32.969013 spai-2024.3.6/spai/project/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0       39 2024-02-27 12:31:32.969013 spai-2024.3.6/spai/project/project-template/notebooks/analytics/requirements.txt
--rw-r--r--   0        0        0     1589 2024-02-27 12:31:33.281014 spai-2024.3.6/spai/project/project-template/scripts/analytics/main.py
--rw-r--r--   0        0        0       30 2024-02-27 12:31:33.281014 spai-2024.3.6/spai/project/project-template/scripts/analytics/requirements.txt
--rw-r--r--   0        0        0       53 2024-02-27 12:31:33.281014 spai-2024.3.6/spai/project/project-template/scripts/downloader/.env.example
--rw-r--r--   0        0        0     1093 2024-02-27 12:31:33.281014 spai-2024.3.6/spai/project/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0       64 2024-02-27 12:31:33.285014 spai-2024.3.6/spai/project/project-template/scripts/downloader/requirements.txt
--rw-r--r--   0        0        0      618 2024-02-27 12:46:15.703704 spai-2024.3.6/spai/project/project-template/spai.config.yaml
--rw-r--r--   0        0        0     1504 2024-02-27 12:31:33.593015 spai-2024.3.6/spai/project/project-template/uis/map/main.py
--rw-r--r--   0        0        0       23 2024-02-27 12:31:33.593015 spai-2024.3.6/spai/project/project-template/uis/map/requirements.txt
--rw-r--r--   0        0        0     5249 2024-03-06 15:37:59.114403 spai-2024.3.6/spai/project/run_local.py
--rw-r--r--   0        0        0      813 2024-02-20 14:02:02.358342 spai-2024.3.6/spai/project/stop_service.py
--rw-r--r--   0        0        0       90 2024-02-13 11:22:06.413893 spai-2024.3.6/spai/pulses/__init__.py
--rw-r--r--   0        0        0     4146 2024-02-13 11:22:06.413893 spai-2024.3.6/spai/pulses/forest_monitoring.py
--rw-r--r--   0        0        0     3160 2024-02-20 09:51:03.207114 spai-2024.3.6/spai/pulses/water_quality 2.py
--rw-r--r--   0        0        0    15958 2024-02-13 11:22:06.413893 spai-2024.3.6/spai/pulses/water_quality.py
--rw-r--r--   0        0        0       38 2024-02-13 11:22:06.413893 spai-2024.3.6/spai/reports/__init__.py
--rw-r--r--   0        0        0     1328 2024-02-13 11:22:06.413893 spai-2024.3.6/spai/reports/generate.py
--rw-r--r--   0        0        0     4709 2024-03-06 15:09:31.184505 spai-2024.3.6/spai/repos/APIRepo.py
--rw-r--r--   0        0        0      997 2024-02-13 11:22:06.413893 spai-2024.3.6/spai/repos/AuthRepo.py
--rw-r--r--   0        0        0      188 2024-02-13 11:22:06.413893 spai-2024.3.6/spai/repos/MailsRepo.py
--rw-r--r--   0        0        0      200 2024-02-13 11:22:06.413893 spai-2024.3.6/spai/repos/ReportsRepo.py
--rw-r--r--   0        0        0       60 2024-02-13 11:22:06.413893 spai-2024.3.6/spai/repos/__init__.py
--rw-r--r--   0        0        0     2260 2024-02-20 15:36:20.945363 spai-2024.3.6/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     3716 2024-02-21 15:37:15.557746 spai-2024.3.6/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     4309 2024-02-21 15:38:40.449966 spai-2024.3.6/spai/storage/LocalStorage.py
--rw-r--r--   0        0        0     7992 2024-02-21 16:15:58.783094 spai-2024.3.6/spai/storage/S3Storage.py
--rw-r--r--   0        0        0     1407 2024-02-21 15:58:16.878415 spai-2024.3.6/spai/storage/Storage.py
--rw-r--r--   0        0        0     6077 2024-02-21 15:41:15.474368 spai-2024.3.6/spai/storage/_S3Storage.py
--rw-r--r--   0        0        0      120 2024-02-20 10:14:34.063953 spai-2024.3.6/spai/storage/__init__.py
--rw-r--r--   0        0        0      409 2024-03-06 14:10:29.421374 spai-2024.3.6/spai/storage/create_s3.py
--rw-r--r--   0        0        0     1163 2024-02-20 15:50:27.760563 spai-2024.3.6/spai/storage/decorators.py
--rw-r--r--   0        0        0      583 2024-02-20 09:51:03.207114 spai-2024.3.6/spai/storage/minio.py
--rw-r--r--   0        0        0      938 1970-01-01 00:00:00.000000 spai-2024.3.6/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2024.4.11/README.md
+-rw-r--r--   0        0        0      525 2024-04-11 09:13:14.264357 spai-2024.4.11/pyproject.toml
+-rw-r--r--   0        0        0       27 2024-04-11 09:13:14.264357 spai-2024.4.11/spai/__init__.py
+-rw-r--r--   0        0        0       90 2024-03-28 09:40:21.297014 spai-2024.4.11/spai/analytics/__init__.py
+-rw-r--r--   0        0        0     4073 2024-03-28 15:02:41.834449 spai-2024.4.11/spai/analytics/forest_monitoring.py
+-rw-r--r--   0        0        0    12364 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/analytics/water_quality.py
+-rw-r--r--   0        0        0       96 2024-02-13 11:22:06.401893 spai-2024.4.11/spai/auth/__init__.py
+-rw-r--r--   0        0        0     1210 2024-02-13 11:22:06.401893 spai-2024.4.11/spai/auth/auth.py
+-rw-r--r--   0        0        0       99 2024-02-13 11:22:06.401893 spai-2024.4.11/spai/auth/is_logged.py
+-rw-r--r--   0        0        0      161 2024-02-13 11:22:06.401893 spai-2024.4.11/spai/auth/logout.py
+-rw-r--r--   0        0        0     7202 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/cli.py
+-rw-r--r--   0        0        0        0 2024-02-13 11:22:06.401893 spai-2024.4.11/spai/commands/__init__.py
+-rw-r--r--   0        0        0     1017 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/commands/auth.py
+-rw-r--r--   0        0        0     1160 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/commands/list.py
+-rw-r--r--   0        0        0       86 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/config/__init__.py
+-rw-r--r--   0        0        0     3583 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/config/validate.py
+-rw-r--r--   0        0        0     1324 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/config/vars.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2024.4.11/spai/data/__init__.py
+-rw-r--r--   0        0        0       49 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/data/indices/__init__.py
+-rw-r--r--   0        0        0       54 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/data/indices/fwi/__init__.py
+-rw-r--r--   0        0        0     3234 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/data/indices/fwi/fwi_nasa.py
+-rw-r--r--   0        0        0      604 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     3941 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     6306 2024-04-11 08:49:55.311741 spai-2024.4.11/spai/data/satellite/download_stac.py
+-rw-r--r--   0        0        0      647 2023-10-30 11:07:40.852696 spai-2024.4.11/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0      725 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py
+-rw-r--r--   0        0        0      758 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py
+-rw-r--r--   0        0        0      758 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py
+-rw-r--r--   0        0        0      758 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/data/satellite/sentinelhub/SHDEM30Downloader.py
+-rw-r--r--   0        0        0     3587 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2584 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2024.4.11/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1264 2023-10-30 11:07:40.856696 spai-2024.4.11/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2024.4.11/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2024.4.11/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      282 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0     2222 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/data/satellite/stac/STACDownloader.py
+-rw-r--r--   0        0        0      208 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/data/satellite/stac/__init__.py
+-rw-r--r--   0        0        0      461 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/data/satellite/stac/aws/AWSDEM30Downloader.py
+-rw-r--r--   0        0        0      461 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/data/satellite/stac/aws/AWSDEM90Downloader.py
+-rw-r--r--   0        0        0      876 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/data/satellite/stac/aws/AWSDEMDownloader.py
+-rw-r--r--   0        0        0      392 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/data/satellite/stac/aws/AWSDownloader.py
+-rw-r--r--   0        0        0     1951 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py
+-rw-r--r--   0        0        0      233 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/data/satellite/stac/aws/__init__.py
+-rw-r--r--   0        0        0      456 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/data/satellite/stac/decorators.py
+-rw-r--r--   0        0        0      716 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/data/satellite/stac/pc/PCDownloader.py
+-rw-r--r--   0        0        0      802 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/data/satellite/stac/pc/PCS1GRDDownloader.py
+-rw-r--r--   0        0        0      120 2024-04-10 12:59:59.948165 spai-2024.4.11/spai/data/satellite/stac/pc/__init__.py
+-rw-r--r--   0        0        0     8905 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/data/satellite/utils.py
+-rw-r--r--   0        0        0       84 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/data/vector/__init__.py
+-rw-r--r--   0        0        0     5533 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/data/vector/openstreetmap.py
+-rw-r--r--   0        0        0       71 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/errors/__init__.py
+-rw-r--r--   0        0        0      308 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/errors/auth.py
+-rw-r--r--   0        0        0      156 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/errors/mails.py
+-rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2024.4.11/spai/image/__init__.py
+-rw-r--r--   0        0        0     1350 2023-10-30 11:07:40.856696 spai-2024.4.11/spai/image/utils.py
+-rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2024.4.11/spai/image/xyz/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2024.4.11/spai/image/xyz/cache.py
+-rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2024.4.11/spai/image/xyz/errors.py
+-rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2024.4.11/spai/image/xyz/get_image_tile.py
+-rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2024.4.11/spai/image/xyz/image_utils.py
+-rw-r--r--   0        0        0       28 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/mails/__init__.py
+-rw-r--r--   0        0        0     1334 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/mails/mimetypes.py
+-rw-r--r--   0        0        0     2932 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/mails/send.py
+-rw-r--r--   0        0        0     3305 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/models/Config.py
+-rw-r--r--   0        0        0      984 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/models/StorageConfig.py
+-rw-r--r--   0        0        0       27 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/models/__init__.py
+-rw-r--r--   0        0        0      391 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/processing/__init__.py
+-rw-r--r--   0        0        0      669 2024-03-28 15:02:41.834449 spai-2024.4.11/spai/processing/autocategorize1D.py
+-rw-r--r--   0        0        0      477 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/processing/colorize_raster.py
+-rw-r--r--   0        0        0      932 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/processing/convert_array_to_vector.py
+-rw-r--r--   0        0        0      291 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/processing/mask_raster.py
+-rw-r--r--   0        0        0      682 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/processing/normalised_difference.py
+-rw-r--r--   0        0        0     1239 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/processing/px_count.py
+-rw-r--r--   0        0        0      107 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/processing/rasterio_mask.py
+-rw-r--r--   0        0        0      266 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/processing/read_raster.py
+-rw-r--r--   0        0        0      876 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/processing/save_table.py
+-rw-r--r--   0        0        0      496 2024-03-28 15:02:41.834449 spai-2024.4.11/spai/processing/utils.py
+-rw-r--r--   0        0        0      475 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/project/__init__.py
+-rw-r--r--   0        0        0      466 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/project/bck/GetLogs.py
+-rw-r--r--   0        0        0     1018 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/project/bck/InstallReqs 2.py
+-rw-r--r--   0        0        0     1018 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/project/bck/InstallReqs 3.py
+-rw-r--r--   0        0        0      482 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/project/bck/RunService.py
+-rw-r--r--   0        0        0      492 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/project/bck/ScheduleService.py
+-rw-r--r--   0        0        0      510 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/project/bck/StopService.py
+-rw-r--r--   0        0        0     1578 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/project/bck/main.py
+-rw-r--r--   0        0        0      337 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/project/delete_project.py
+-rw-r--r--   0        0        0     2060 2024-03-28 15:01:17.074615 spai-2024.4.11/spai/project/deploy_folder.py
+-rw-r--r--   0        0        0      408 2024-03-28 15:01:17.078615 spai-2024.4.11/spai/project/deploy_template.py
+-rw-r--r--   0        0        0     1203 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/project/download_template.py
+-rw-r--r--   0        0        0      455 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/project/get_logs.py
+-rw-r--r--   0        0        0      242 2024-02-13 11:22:06.405893 spai-2024.4.11/spai/project/get_project_by_name.py
+-rw-r--r--   0        0        0      172 2024-02-13 11:22:06.409893 spai-2024.4.11/spai/project/get_projects.py
+-rw-r--r--   0        0        0      344 2024-02-13 11:22:06.409893 spai-2024.4.11/spai/project/get_service_by_name_type_project.py
+-rw-r--r--   0        0        0     1616 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/project/get_services.py
+-rw-r--r--   0        0        0      525 2024-02-21 09:43:40.417670 spai-2024.4.11/spai/project/init_project.py
+-rw-r--r--   0        0        0      726 2024-02-20 15:56:19.617848 spai-2024.4.11/spai/project/install_requirements.py
+-rw-r--r--   0        0        0     5617 2024-02-27 12:31:33.913016 spai-2024.4.11/spai/project/project-template/README.md
+-rw-r--r--   0        0        0      867 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/project/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0       36 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/project/project-template/apis/analytics/requirements.txt
+-rw-r--r--   0        0        0     1800 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/project/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0       88 2024-03-13 09:12:15.507871 spai-2024.4.11/spai/project/project-template/apis/xyz/requirements.txt
+-rw-r--r--   0        0        0   748531 2024-03-13 09:12:15.511871 spai-2024.4.11/spai/project/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0       39 2024-03-13 09:12:15.511871 spai-2024.4.11/spai/project/project-template/notebooks/analytics/requirements.txt
+-rw-r--r--   0        0        0     1602 2024-04-11 09:09:28.631609 spai-2024.4.11/spai/project/project-template/scripts/analytics/main.py
+-rw-r--r--   0        0        0       30 2024-03-13 09:12:15.511871 spai-2024.4.11/spai/project/project-template/scripts/analytics/requirements.txt
+-rw-r--r--   0        0        0     1076 2024-04-11 09:10:07.363737 spai-2024.4.11/spai/project/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0       85 2024-04-11 09:09:55.963699 spai-2024.4.11/spai/project/project-template/scripts/downloader/requirements.txt
+-rw-r--r--   0        0        0      618 2024-03-13 09:12:15.511871 spai-2024.4.11/spai/project/project-template/spai.config.yaml
+-rw-r--r--   0        0        0     1504 2024-03-13 09:12:15.511871 spai-2024.4.11/spai/project/project-template/uis/map/main.py
+-rw-r--r--   0        0        0       23 2024-02-27 12:31:33.593015 spai-2024.4.11/spai/project/project-template/uis/map/requirements.txt
+-rw-r--r--   0        0        0     5242 2024-03-25 08:56:48.420217 spai-2024.4.11/spai/project/run_local.py
+-rw-r--r--   0        0        0      813 2024-03-13 09:12:15.511871 spai-2024.4.11/spai/project/stop_service.py
+-rw-r--r--   0        0        0       38 2024-02-13 11:22:06.413893 spai-2024.4.11/spai/reports/__init__.py
+-rw-r--r--   0        0        0     1328 2024-02-13 11:22:06.413893 spai-2024.4.11/spai/reports/generate.py
+-rw-r--r--   0        0        0     4709 2024-03-13 09:12:15.511871 spai-2024.4.11/spai/repos/APIRepo.py
+-rw-r--r--   0        0        0      997 2024-02-13 11:22:06.413893 spai-2024.4.11/spai/repos/AuthRepo.py
+-rw-r--r--   0        0        0      188 2024-02-13 11:22:06.413893 spai-2024.4.11/spai/repos/MailsRepo.py
+-rw-r--r--   0        0        0      200 2024-02-13 11:22:06.413893 spai-2024.4.11/spai/repos/ReportsRepo.py
+-rw-r--r--   0        0        0       60 2024-02-13 11:22:06.413893 spai-2024.4.11/spai/repos/__init__.py
+-rw-r--r--   0        0        0     2452 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     3716 2024-03-13 09:12:15.515871 spai-2024.4.11/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     4527 2024-04-11 08:43:02.338399 spai-2024.4.11/spai/storage/LocalStorage.py
+-rw-r--r--   0        0        0     8449 2024-04-11 08:43:08.570420 spai-2024.4.11/spai/storage/S3Storage.py
+-rw-r--r--   0        0        0     1407 2024-03-13 09:12:15.515871 spai-2024.4.11/spai/storage/Storage.py
+-rw-r--r--   0        0        0     6077 2024-03-13 09:12:15.515871 spai-2024.4.11/spai/storage/_S3Storage.py
+-rw-r--r--   0        0        0      120 2024-03-13 09:12:15.515871 spai-2024.4.11/spai/storage/__init__.py
+-rw-r--r--   0        0        0      409 2024-03-13 09:12:15.515871 spai-2024.4.11/spai/storage/create_s3.py
+-rw-r--r--   0        0        0     1559 2024-04-10 12:59:59.948165 spai-2024.4.11/spai/storage/decorators.py
+-rw-r--r--   0        0        0      583 2024-03-13 09:12:15.515871 spai-2024.4.11/spai/storage/minio.py
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 spai-2024.4.11/PKG-INFO
```

### Comparing `spai-2024.3.6/pyproject.toml` & `spai-2024.4.11/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spai"
-version = "2024.03.06"
+version = "2024.04.11"
 description = ""
 authors = ["Juan Sensio <it@earthpulse.es>"]
 readme = "README.md"
 packages = [{include = "spai"}]
 
 [tool.poetry.scripts]
 spai = "spai.cli:app"
```

### Comparing `spai-2024.3.6/spai/auth/auth.py` & `spai-2024.4.11/spai/auth/auth.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/cli.py` & `spai-2024.4.11/spai/cli.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/commands/auth.py` & `spai-2024.4.11/spai/commands/auth.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/commands/list.py` & `spai-2024.4.11/spai/commands/list.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/config/validate.py` & `spai-2024.4.11/spai/config/validate.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/config/vars.py` & `spai-2024.4.11/spai/config/vars.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/data/indices/fwi/fwi_nasa.py` & `spai-2024.4.11/spai/data/indices/fwi/fwi_nasa.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/data/satellite/download.py` & `spai-2024.4.11/spai/data/satellite/download.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/data/satellite/explore.py` & `spai-2024.4.11/spai/data/satellite/explore.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py` & `spai-2024.4.11/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py` & `spai-2024.4.11/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py` & `spai-2024.4.11/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/data/satellite/sentinelhub/SHDEM30Downloader.py` & `spai-2024.4.11/spai/data/satellite/sentinelhub/SHDEM30Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2024.4.11/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2024.4.11/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2024.4.11/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2024.4.11/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/data/vector/openstreetmap.py` & `spai-2024.4.11/spai/data/vector/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/image/utils.py` & `spai-2024.4.11/spai/image/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/image/xyz/cache.py` & `spai-2024.4.11/spai/image/xyz/cache.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/image/xyz/errors.py` & `spai-2024.4.11/spai/image/xyz/errors.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/image/xyz/get_image_tile.py` & `spai-2024.4.11/spai/image/xyz/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/image/xyz/image_utils.py` & `spai-2024.4.11/spai/image/xyz/image_utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/mails/mimetypes.py` & `spai-2024.4.11/spai/mails/mimetypes.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/mails/send.py` & `spai-2024.4.11/spai/mails/send.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/models/Config.py` & `spai-2024.4.11/spai/models/Config.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/models/StorageConfig.py` & `spai-2024.4.11/spai/models/StorageConfig.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/processing/convert_array_to_vector.py` & `spai-2024.4.11/spai/processing/convert_array_to_vector.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/processing/normalised_difference.py` & `spai-2024.4.11/spai/processing/normalised_difference.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/processing/px_count.py` & `spai-2024.4.11/spai/processing/px_count.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/processing/save_table.py` & `spai-2024.4.11/spai/processing/save_table.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/bck/InstallReqs 2.py` & `spai-2024.4.11/spai/project/bck/InstallReqs 2.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/bck/InstallReqs 3.py` & `spai-2024.4.11/spai/project/bck/InstallReqs 3.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/bck/main.py` & `spai-2024.4.11/spai/project/bck/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/deploy_folder.py` & `spai-2024.4.11/spai/project/deploy_folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,11 +43,11 @@
     repo = APIRepo()
     data, error = repo.deploy_folder(user, zip_path, variables)
     # clean up
     shutil.rmtree(dst_path)
     if data:
         typer.echo(
             # f"Check status at {os.getenv('SPAI_UI_URL', 'https://spai.earthpulse.ai')}/dashboard/{data}"
-            f"Check status at {os.getenv('SPAI_UI_URL', 'https://spai-new.vercel.app')}/dashboard/{data['project_id']}"
+            f"Check status at {os.getenv('SPAI_UI_URL', 'https://spai.earthpulse.ai')}/dashboard/{data['project_id']}"
         )
         return
     raise Exception(f"Error: {error}")
```

### Comparing `spai-2024.3.6/spai/project/download_template.py` & `spai-2024.4.11/spai/project/download_template.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/get_services.py` & `spai-2024.4.11/spai/project/get_services.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/init_project.py` & `spai-2024.4.11/spai/project/init_project.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/install_requirements.py` & `spai-2024.4.11/spai/project/install_requirements.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/project-template/README.md` & `spai-2024.4.11/spai/project/project-template/README.md`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/project-template/apis/analytics/main.py` & `spai-2024.4.11/spai/project/project-template/apis/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/project-template/apis/xyz/main.py` & `spai-2024.4.11/spai/project/project-template/apis/xyz/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/project-template/notebooks/analytics/main.ipynb` & `spai-2024.4.11/spai/project/project-template/notebooks/analytics/main.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/project-template/scripts/analytics/main.py` & `spai-2024.4.11/spai/project/project-template/scripts/analytics/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from spai.storage import Storage
 import numpy as np
 import pandas as pd
 
+storage = Storage()["data"]
+
 
 def ndvi(image):
     ds = storage.read(image)
     red = ds.read(4).astype(np.float32)
     nir = ds.read(8)
     ndvi = (nir - red) / (nir + red + 1e-8)
     date = image.split("_")[1].split(".")[0]
@@ -17,16 +19,15 @@
     for i, cat in enumerate(cats[:-1]):
         data0[(data > cat) & (data <= cats[i + 1])] = i
     data0 = data0.astype(np.uint8)
     return data0
 
 
 # retrieve all images
-storage = Storage()["data"]
-images = storage.list("S2*")
+images = storage.list("sentinel-2-l2a*")
 print("Found the following images:", images)
 
 # compute ndvis
 
 for image in images:
     ndvi(image)
 images = storage.list("NDVI*")
```

### Comparing `spai-2024.3.6/spai/project/project-template/scripts/downloader/main.py` & `spai-2024.4.11/spai/project/project-template/scripts/downloader/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-from datetime import datetime, timedelta
-from dotenv import load_dotenv
-
 from spai.storage import Storage
-from spai.data.satellite import explore_satellite_images, download_satellite_image
-
-load_dotenv()
+from spai.data.satellite import explore_satellite_imagery, download_satellite_imagery
 
 # explore available images
 print("Looking for images in the last month")
 bbox = (2.0052191, 41.38238988, 2.17002873, 41.48530451)  # Collserola
-images = explore_satellite_images(bbox, cloud_cover=10)
+images = explore_satellite_imagery(bbox, cloud_cover=10)
 if len(images) == 0:
     raise ValueError("No images found")
 
 # download images and save locally
 storage = Storage()
-sensor = "S2L2A"  # or 'S2L1C'
+sensor = "sentinel-2-l2a"
 existing_images = storage["data"].list(f"{sensor}*.tif")
 dates = [image.split("_")[1].split(".")[0] for image in existing_images]
 print("Found", len(images), f"image{'s' if len(images) > 1 else ''}")
+new_images = []
 for image in images:
     # check if image is already downloaded
-    date = image["date"].split("T")[0]
-    if date in dates:
+    date = image["datetime"].split("T")[0]
+    if date in dates or date in new_images:
         print("Image already downloaded:", date)
         continue
+    new_images.append(date)
     print("Downloading new image:", date)
-    path = download_satellite_image(storage["data"], bbox, date, sensor)
+    path = download_satellite_imagery(storage["data"], bbox, date, sensor)
     print("Image saved at", path)
```

### Comparing `spai-2024.3.6/spai/project/project-template/spai.config.yaml` & `spai-2024.4.11/spai/project/project-template/spai.config.yaml`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/project-template/uis/map/main.py` & `spai-2024.4.11/spai/project/project-template/uis/map/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/project/run_local.py` & `spai-2024.4.11/spai/project/run_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         typer.echo(f"Deploying apis...")
         for api in config.apis:
             typer.echo(f"Running api '{api.name}'...")
             p = Process(target=run_api, args=(api, dir, api.port, api.host))
             p.start()
             processes.append(p)
             # save api_urls in case UIs need them
-            api_urls[f"api.{api.name}"] = f"http://{api.host}:{api.port}"
+            api_urls[f"api.{api.name}"] = f"{api.host}:{api.port}"
     if config.uis:
         typer.echo(f"Deploying uis...")
         for ui in config.uis:
             typer.echo(f"Running ui '{ui.name}'...")
             p = Process(target=run_ui, args=(ui, dir, api_urls))
             p.start()
             processes.append(p)
```

### Comparing `spai-2024.3.6/spai/project/stop_service.py` & `spai-2024.4.11/spai/project/stop_service.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/pulses/forest_monitoring.py` & `spai-2024.4.11/spai/analytics/forest_monitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import numpy as np
 import geopandas as gpd
-import pandas as pd
-from datetime import datetime
 
 from ..processing import read_raster
 from ..processing import normalised_difference
 from ..processing import mask_raster
 from ..processing import autocategorize1D
 from ..processing import px_count
 from ..processing import colorize_raster
@@ -42,40 +40,36 @@
     # save_raster ndvi_categorized
     raster_name_ndvi_categorized = f"ndvi_categorized_{date}.tif"
     storage.create(ndvi_categorized, raster_name_ndvi_categorized, ds=ds)
 
     # apply_threshold to ndvi_categorized
     threshold = 3
     vegetation = ndvi_categorized >= threshold
-    vegetation = vegetation.astype(int)
+    vegetation = vegetation.astype(np.uint8)
 
     # save_raster vegetation
     raster_name_vegetation = f"vegetation_{date}.tif"
     storage.create(vegetation, raster_name_vegetation, ds=ds)
 
     # mask_raster vegetation with aoi_mask
-    vegetation_masked, _ = mask_raster(
-        raster_name_vegetation, aoi_mask_gdf, storage
-    )
+    vegetation_masked, _ = mask_raster(raster_name_vegetation, aoi_mask_gdf, storage)
 
     # save_raster vegetation_masked
     raster_name_vegetation_masked = f"vegetation_masked_{date}.tif"
     storage.create(vegetation_masked, raster_name_vegetation_masked, ds=ds)
 
     # colorize_raster vegetation_masked
     vegetation_masked_rgb = colorize_raster(vegetation_masked)
 
     # save_raster vegetation_masked_rgb
     raster_name_vegetation_masked_rgb = f"vegetation_masked_rgb_{date}.tif"
     storage.create(vegetation_masked_rgb, raster_name_vegetation_masked_rgb, ds=ds)
 
     # mask_raster ndvi_categorized with aoi_mask
-    quality_mask, _ = mask_raster(
-        raster_name_ndvi_categorized, aoi_mask_gdf, storage
-    )
+    quality_mask, _ = mask_raster(raster_name_ndvi_categorized, aoi_mask_gdf, storage)
 
     # save_raster quality_mask
     raster_name_quality_mask = f"quality_masked_{date}.tif"
     storage.create(quality_mask, raster_name_quality_mask, ds=ds)
 
     # colorize_raster quality_mask
     quality_mask_rgb = colorize_raster(
```

### Comparing `spai-2024.3.6/spai/pulses/water_quality.py` & `spai-2024.4.11/spai/analytics/water_quality.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 from ..processing import colorize_raster
 from ..processing import px_count
 from ..processing import save_table
 from ..processing import normalised_difference
 from ..processing import convert_array_to_vector
 
 
-def water_quality(image_name, aoi_mask, storage, desired_images=2, date=None):
+def water_quality(image_name, aoi_mask, storage, date=None):
     """
     This function calculates the water quality of a given image.
 
     It calculates the following layers:
         - Normalized Difference Water Index (NDWI) - ndwi_{date}.tif, ndwi_masked_{date}.tif, ndwi_categorized_{date}.tif
         - Normalized Difference Turbidity Index (NDTI) - ndti_{date}.tif, ndti_masked_{date}.tif, ndti_categorized_{date}.tif
         - Normalized Difference Chlorophyll Index (NDCI) - ndci_{date}.tif, ndci_masked_{date}.tif, ndci_categorized_{date}.tif
-        - Median Water Mask - median_water_mask_{date}.tif
+        - Water Mask - water_mask_{date}.tif
         - Dissolved Organic Carbon (DOC) - DOC_{date}.tif, DOC_masked_{date}.tif, DOC_categorized_{date}.tif
 
     It also calculates the following analytics:
         - Water Extent (in hectares and percentage) - table_water_extent.json
         - Water Turbidity (in hectares and percentage) - table_turbidity_Ha.json, table_turbidity_percent.json
         - Water Chlorophyll (in hectares and percentage) - table_chlorophyll_Ha.json, table_chlorophyll_percent.json
         - Water DOC (in hectares and percentage) - table_DOC_Ha.json, table_DOC_percent.json
@@ -39,16 +39,14 @@
     ----------
     image_name : str
         The name of the image to be processed.
     aoi_mask : dict
         The GeoJSON of the area of interest.
     storage : Storage
         The Storage object.
-    desired_images : int, optional
-        The number of images to be downloaded to determine the water body status, by default 2.
     date : str, optional
         The date of the image from which start downloading earlier images to determine the water body status,
         by default None, which uses the date given in the image name.
 
     Returns
     -------
     None
@@ -81,71 +79,66 @@
     ndci = normalised_difference(raster, [3, 2])
     ndci = equalize_hist(ndci)
 
     # save_raster ndci
     raster_name_ndci = f"ndci_{date}.tif"
     storage.create(ndci, raster_name_ndci, ds=ds)
 
-    # MEDIAN WATER MASK
-    # calculate median_water_mask
-    median_water_mask, stored_images, _ = compute_median_water_mask(
-        aoi_mask, desired_images, date, storage
-    )  # aoi_mask is needed for downloading
-
-    # save raster median_water_mask
-    raster_name_median_water_mask = f"median_water_mask_{date}.tif"
-    median_water_mask_path = storage.create(
-        median_water_mask, raster_name_median_water_mask, ds=ds
-    )
+    # Calculate water mask and smooth it
+    # threshold on 0
+    water_mask = ndwi >= 0.2
+    water_mask = median_filter(water_mask, size=(10, 5))
+
+    # save_raster water_mask
+    raster_name_water_mask = f"water_mask_{date}.tif"
+    storage.create(water_mask, raster_name_water_mask, ds=ds)
 
     # DOC
     # calculate doc
+    stored_images = storage.list("sentinel-2-l2a*.tif")
     doc_layers_array, doc_values_array, ds = compute_doc(stored_images, storage)
 
     # save_raster doc
     raster_name_doc = f"DOC_{date}.tif"
     storage.create(doc_layers_array[0], raster_name_doc, ds=ds)
 
     """ MASK LAYERS """
-    shp = convert_array_to_vector(median_water_mask, median_water_mask_path)
+    shp = convert_array_to_vector(water_mask, storage.get_path(raster_name_water_mask))
 
     # mask_raster ndwi with aoi_mask
     ndwi_masked, _ = mask_raster(raster_name_ndwi, shp, storage)
 
     # save_raster ndwi_masked
     raster_name_ndwi_masked = f"ndwi_masked_{date}.tif"
     storage.create(ndwi_masked, raster_name_ndwi_masked, ds=ds)
 
     # mask_raster ndti with aoi_mask
     ndti_masked, _ = mask_raster(raster_name_ndti, shp, storage)
-    ndti_masked[ndti_masked == False] = -9999  # convert false to nan
 
     # save_raster ndti_masked
     raster_name_ndti_masked = f"ndti_masked_{date}.tif"
     storage.create(ndti_masked, raster_name_ndti_masked, ds=ds)
 
     # mask_raster ndci with aoi_mask
     ndci_masked, _ = mask_raster(raster_name_ndci, shp, storage)
-    ndci_masked[ndci_masked == False] = -9999  # convert false to nan
 
     # save_raster ndci_masked
     raster_name_ndci_masked = f"ndci_masked_{date}.tif"
     storage.create(ndci_masked, raster_name_ndci_masked, ds=ds)
 
     # mask_raster doc with aoi_mask
     doc_masked, _ = mask_raster(raster_name_doc, shp, storage)
-    doc_masked[doc_masked == False] = -9999  # convert false to nan
 
     # save_raster doc_masked
     raster_name_doc_masked = f"DOC_masked_{date}.tif"
     storage.create(doc_masked, raster_name_doc_masked, ds=ds)
 
     """ ANALYTICS """
     # Water Extent
-    extent_has = np.divide(median_water_mask.sum(axis=(1, 2)).max(), 100)
+    extent_has = np.divide(water_mask.sum().max(), 100)
     update_extent_table(extent_has, date, storage)
 
     # Water Turbidity
     ndti_categories = np.digitize(ndti_masked, [-np.inf, -0.2, 0.4, np.inf])
     raster_name_ndti_categorized = f"ndti_categorized_{date}.tif"
     storage.create(ndti_categories, raster_name_ndti_categorized, ds=ds)
 
@@ -231,142 +224,58 @@
     mean_min_doc = np.mean([dict["min_doc"] for dict in doc_values_array])
     mean_std_doc = np.mean([dict["std_doc"] for dict in doc_values_array])
 
     # Categorize the doc values
     a = 1
     min_to_N0 = -np.inf
     N0_to_N1 = mean_mean_doc + 2 * mean_std_doc / a
-    N1_to_N2 = mean_mean_doc + 3 * mean_std_doc / a
-    N2_to_N3 = mean_mean_doc + 4 * mean_std_doc / a
+    N1_to_N3 = mean_mean_doc + 4 * mean_std_doc / a
     N3_to_max = np.inf
 
-    doc_categories = np.digitize(
-        doc_masked, [min_to_N0, N0_to_N1, N1_to_N2, N2_to_N3, N3_to_max]
-    )
+    doc_categories = np.digitize(doc_masked, [min_to_N0, N0_to_N1, N1_to_N3, N3_to_max])
     raster_name_doc_categorized = f"DOC_categorized_{date}.tif"
     storage.create(doc_categories, raster_name_doc_categorized, ds=ds)
 
-    doc_colorized = colorize_raster(
-        doc_categories, colors=["green", "yellow", "orange", "red"]
-    )
+    doc_colorized = colorize_raster(doc_categories, colors=["green", "yellow", "red"])
     raster_name_doc_colorized = f"DOC_categorized_rgb_{date}.tif"
     storage.create(doc_colorized, raster_name_doc_colorized, ds=ds)
 
-    doc_px_counted = px_count(doc_categories, [1, 2, 3, 4])
+    doc_px_counted = px_count(doc_categories, [1, 2, 3])
     doc_has = np.divide(
         doc_px_counted,
         100,
         out=np.zeros_like(doc_px_counted, dtype=np.float64),
         where=100 != 0,
     )
     # save_table DOC hectareas
     doc_table_name = "table_DOC_Ha.json"
-    doc_columns = ["N0 [Has]", "N1 [Has]", "N2 [Has]", "N3 [Has]", "Total [Has]"]
+    doc_columns = ["Good [Has]", "Careful [Has]", "Bad [Has]", "Total [Has]"]
     save_table(
         data=doc_has,
         columns=doc_columns,
         table_name=doc_table_name,
         date=date,
         storage=storage,
     )
     doc_percent = [
         np.divide(doc_has[i], doc_has[-1]) * 100 for i in range(len(doc_has) - 1)
     ]
     # save_table DOC percent
     doc_percent_table_name = "table_DOC_percent.json"
-    doc_percent_columns = ["N0 [%]", "N1 [%]", "N2 [%]", "N3 [%]"]
+    doc_percent_columns = ["Good [%]", "Careful [%]", "Bad [%]"]
+    print(doc_percent)
     save_table(
         data=doc_percent,
         columns=doc_percent_columns,
         table_name=doc_percent_table_name,
         date=date,
         storage=storage,
     )
 
 
-"""
-Methods for Layers: Median Water Mask
-"""
-
-
-def compute_median_water_mask(aoi_mask, desired_images, from_date_to_earlier, storage):
-    # Get the bbox from the aoi_mask
-    bbox = gpd.GeoDataFrame.from_features(aoi_mask["features"]).geometry[0]
-
-    stored_images = download_missing_images(
-        desired_images=desired_images,
-        from_date_to_earlier=from_date_to_earlier,
-        bbox=bbox,
-        storage=storage,
-    )
-    water_masks_array, ds = compute_water_masks(stored_images, storage)
-    median_water_mask = median_filter(water_masks_array, size=(7, 3, 3))
-    binary_median_water_mask = median_water_mask.astype(np.uint8)
-
-    # save_raster
-    median_raster_name = "median_water_mask.tif"
-    storage.create(median_water_mask, median_raster_name, ds=ds)
-    return binary_median_water_mask, stored_images, water_masks_array
-
-
-def download_missing_images(desired_images, from_date_to_earlier, bbox, storage):
-    # Convert the date string to a datetime object
-    date_obj = datetime.strptime(from_date_to_earlier, "%Y-%m-%d")
-    # Check how many images that begin with "S2L2A" are in storage
-    files = storage.list()
-    stored_images = []
-    for file in files:
-        # If the file is a Sentinel-2 image of a date equal or earlier than 'from_date_to_earlier' , add it to the list:
-        if file.startswith("S2L2A"):
-            image_date = datetime.strptime(file.split("_")[1].split(".")[0], "%Y-%m-%d")
-            if image_date <= date_obj and len(stored_images) < desired_images:
-                stored_images.append(file)
-    # If images are less than desired, download the missing ones
-    images_found = []
-    while len(stored_images) < desired_images:
-        time_interval = (
-            (date_obj - timedelta(days=10)).strftime("%Y-%m-%d"),
-            date_obj.strftime("%Y-%m-%d"),
-        )
-        images_found = explore_satellite_images(
-            bbox, time_interval=time_interval, cloud_cover=5
-        )
-        for image in images_found:
-            if f"S2L2A_{image['date'].split('T')[0]}.tif" not in stored_images:
-                path = download_satellite_image(
-                    storage, bbox, image["date"].split("T")[0]
-                )
-                stored_images.append(path)
-        date_obj -= timedelta(days=10)
-    return stored_images
-
-
-def compute_water_masks(stored_images, storage):
-    water_masks_array = []
-    for path in stored_images:
-        image_name = path.split("/")[-1]
-        date = image_name.split("_")[1].split(".")[0]
-        # read raster
-        ds, raster = read_raster(image_name, storage, bands=[3, 4, 5, 8])
-
-        # calculate ndwi
-        ndwi = normalised_difference(raster, [1, 4])
-
-        # apply thershold to calculate water-mask
-        threshold = 0
-        water_mask = ndwi >= threshold
-
-        # save_raster water_mask
-        raster_name_water_mask = f"water_mask_{date}.tif"
-        storage.create(water_mask, raster_name_water_mask, ds=ds)
-        water_masks_array.append(water_mask)
-
-    return water_masks_array, ds
-
-
 """ 
 Methods for Layers: DOC
 """
 
 
 def compute_doc(stored_images, storage):
     doc_layers_array = []
```

### Comparing `spai-2024.3.6/spai/reports/generate.py` & `spai-2024.4.11/spai/reports/generate.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/repos/APIRepo.py` & `spai-2024.4.11/spai/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/repos/AuthRepo.py` & `spai-2024.4.11/spai/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/storage/BaseStorage.py` & `spai-2024.4.11/spai/storage/BaseStorage.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,19 @@
             # if ext == "csv":
             #     return self.create_from_csv(data, name)
             # elif ext == "json":
             #     return self.create_from_json(data, name)
             # else:
             #     raise TypeError("Not a valid dataframe type")
         elif isinstance(data, dict):
+            print("hola")
             return self.create_from_dict(data, name)
+        elif hasattr(data, "variables") and hasattr(data, "coords"):
+            # Object is like a xr.Dataset
+            return self.create_from_xarray(data, name)
         else:
             raise TypeError("Not a valid type")
 
     def create_from_data(self, data, path):
         with open(path, "wb") as f:
             f.write(data.read())
         return path
```

### Comparing `spai-2024.3.6/spai/storage/CloudStorage.py` & `spai-2024.4.11/spai/storage/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/storage/LocalStorage.py` & `spai-2024.4.11/spai/storage/LocalStorage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 from glob import glob
 import numpy as np
 import pandas as pd
 import shutil
 import json
+from datetime import datetime
 
 from .BaseStorage import BaseStorage
-from .decorators import with_rio, with_geopandas, with_xarray
+from .decorators import with_rio, with_geopandas, with_xarray, with_rioxarray
 
 
 class LocalStorage(BaseStorage):
     def __init__(self, path="data"):
         super().__init__()
         self.path = path
         if not os.path.exists(self.path):
@@ -101,14 +102,20 @@
         return dst_path
 
     def create_from_zarr(self, data, name):
         dst_path = self.get_path(name)
         data.to_zarr(dst_path)
         return dst_path
 
+    @with_rioxarray
+    def create_from_xarray(self, rxr, data, name):
+        dst_path = self.get_path(name)
+        data.rio.to_raster(dst_path)
+        return dst_path
+
     def list(self, pattern="*"):
         paths = glob(os.path.join(self.path, pattern))
         # strip base path
         return [p.replace(self.path + "/", "") for p in paths]
 
     def read_from_array(self, name, path=None):
         if path is None:
```

### Comparing `spai-2024.3.6/spai/storage/S3Storage.py` & `spai-2024.4.11/spai/storage/S3Storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import pandas as pd
 import json
 import io
 from minio import Minio
 import fnmatch
 from io import BytesIO
 import numpy as np
+from os import remove
 
 from .BaseStorage import BaseStorage
-from .decorators import with_rio, with_geopandas
+from .decorators import with_rio, with_geopandas, with_rioxarray
 
 
 # Ver funciones en CloudStorage si las de aquí no acaban de funcionar...
 
 
 class S3Storage(BaseStorage):
     def __init__(self, url, access, secret, bucket, region=None):
@@ -101,14 +102,29 @@
                 bands = 1 if x.ndim < 3 else [i + 1 for i in range(x.shape[0])]
                 dest_ds.write(x, bands)
             self.client.put_object(
                 self.bucket, name, memfile, length=-1, part_size=10 * 1024 * 1024
             )
         return self.get_url(name)
 
+    @with_rioxarray
+    def create_from_xarray(self, rxr, data, name):
+        # TODO don't save to disk
+        content_type = "image/tiff"
+        tmp_path = f"/tmp/{name}"
+        data.rio.to_raster(tmp_path)
+        self.client.fput_object(
+            self.bucket,
+            name,
+            tmp_path,
+            content_type=content_type,
+        )
+        remove(tmp_path)
+        return self.get_url(name)
+
     def create_from_array(self, data, name):
         array_bytes = BytesIO()
         np.save(array_bytes, data)
         array_bytes.seek(0)
         self.client.put_object(
             self.bucket, name, array_bytes, len(array_bytes.getvalue())
         )
```

### Comparing `spai-2024.3.6/spai/storage/Storage.py` & `spai-2024.4.11/spai/storage/Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/storage/_S3Storage.py` & `spai-2024.4.11/spai/storage/_S3Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/spai/storage/decorators.py` & `spai-2024.4.11/spai/storage/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,7 +34,21 @@
             return func(self, gpd, *args, **kwargs)
         except ImportError:
             raise ImportError(
                 "The geopandas package is required for this function. Please install it with 'pip install geopandas' and try again."
             )
 
     return wrapper
+
+
+def with_rioxarray(func):
+    def wrapper(self, *args, **kwargs):
+        try:
+            import rioxarray as rxr
+
+            return func(self, rxr, *args, **kwargs)
+        except ImportError:
+            raise ImportError(
+                "The rioxarray package is required for this function. Please install it with 'pip install rioxarray' and try again."
+            )
+
+    return wrapper
```

### Comparing `spai-2024.3.6/spai/storage/minio.py` & `spai-2024.4.11/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2024.3.6/PKG-INFO` & `spai-2024.4.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spai
-Version: 2024.3.6
+Version: 2024.4.11
 Summary: 
 Author: Juan Sensio
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

