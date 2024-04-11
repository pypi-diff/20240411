# Comparing `tmp/spai-2024.4.11.post3.tar.gz` & `tmp/spai-2024.4.11.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2024.4.11.post3.tar", max compression
+gzip compressed data, was "spai-2024.4.11.post4.tar", max compression
```

## Comparing `spai-2024.4.11.post3.tar` & `spai-2024.4.11.post4.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2024.4.11.post3/README.md
--rw-r--r--   0        0        0      527 2024-04-11 10:07:24.252764 spai-2024.4.11.post3/pyproject.toml
--rw-r--r--   0        0        0       29 2024-04-11 10:07:24.252764 spai-2024.4.11.post3/spai/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 10:07:14.320721 spai-2024.4.11.post3/spai/analytics/__init__.py
--rw-r--r--   0        0        0     4073 2024-03-28 15:02:41.834449 spai-2024.4.11.post3/spai/analytics/forest_monitoring.py
--rw-r--r--   0        0        0    12191 2024-04-11 10:07:11.468709 spai-2024.4.11.post3/spai/analytics/water_quality.py
--rw-r--r--   0        0        0       96 2024-02-13 11:22:06.401893 spai-2024.4.11.post3/spai/auth/__init__.py
--rw-r--r--   0        0        0     1210 2024-02-13 11:22:06.401893 spai-2024.4.11.post3/spai/auth/auth.py
--rw-r--r--   0        0        0       99 2024-02-13 11:22:06.401893 spai-2024.4.11.post3/spai/auth/is_logged.py
--rw-r--r--   0        0        0      161 2024-02-13 11:22:06.401893 spai-2024.4.11.post3/spai/auth/logout.py
--rw-r--r--   0        0        0     7202 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/cli.py
--rw-r--r--   0        0        0        0 2024-02-13 11:22:06.401893 spai-2024.4.11.post3/spai/commands/__init__.py
--rw-r--r--   0        0        0     1017 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/commands/auth.py
--rw-r--r--   0        0        0     1160 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/commands/list.py
--rw-r--r--   0        0        0       86 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/config/__init__.py
--rw-r--r--   0        0        0     3583 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/config/validate.py
--rw-r--r--   0        0        0     1324 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/config/vars.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2024.4.11.post3/spai/data/__init__.py
--rw-r--r--   0        0        0       49 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/data/indices/__init__.py
--rw-r--r--   0        0        0       54 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/data/indices/fwi/__init__.py
--rw-r--r--   0        0        0     3234 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/data/indices/fwi/fwi_nasa.py
--rw-r--r--   0        0        0      608 2024-04-11 09:16:29.113004 spai-2024.4.11.post3/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     3941 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/data/satellite/download.py
--rw-r--r--   0        0        0     6306 2024-04-11 08:49:55.311741 spai-2024.4.11.post3/spai/data/satellite/download_stac.py
--rw-r--r--   0        0        0      647 2023-10-30 11:07:40.852696 spai-2024.4.11.post3/spai/data/satellite/explore.py
--rw-r--r--   0        0        0      725 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py
--rw-r--r--   0        0        0      758 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py
--rw-r--r--   0        0        0      758 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py
--rw-r--r--   0        0        0      758 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHDEM30Downloader.py
--rw-r--r--   0        0        0     3587 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2584 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1264 2023-10-30 11:07:40.856696 spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      282 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0     2222 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/data/satellite/stac/STACDownloader.py
--rw-r--r--   0        0        0      208 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/data/satellite/stac/__init__.py
--rw-r--r--   0        0        0      461 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/data/satellite/stac/aws/AWSDEM30Downloader.py
--rw-r--r--   0        0        0      461 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/data/satellite/stac/aws/AWSDEM90Downloader.py
--rw-r--r--   0        0        0      876 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/data/satellite/stac/aws/AWSDEMDownloader.py
--rw-r--r--   0        0        0      392 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/data/satellite/stac/aws/AWSDownloader.py
--rw-r--r--   0        0        0     1951 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py
--rw-r--r--   0        0        0      233 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/data/satellite/stac/aws/__init__.py
--rw-r--r--   0        0        0      456 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/data/satellite/stac/decorators.py
--rw-r--r--   0        0        0      716 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/data/satellite/stac/pc/PCDownloader.py
--rw-r--r--   0        0        0      802 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/data/satellite/stac/pc/PCS1GRDDownloader.py
--rw-r--r--   0        0        0      120 2024-04-10 12:59:59.948165 spai-2024.4.11.post3/spai/data/satellite/stac/pc/__init__.py
--rw-r--r--   0        0        0     8905 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/data/satellite/utils.py
--rw-r--r--   0        0        0       84 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/data/vector/__init__.py
--rw-r--r--   0        0        0     5533 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/data/vector/openstreetmap.py
--rw-r--r--   0        0        0       71 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/errors/__init__.py
--rw-r--r--   0        0        0      308 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/errors/auth.py
--rw-r--r--   0        0        0      156 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/errors/mails.py
--rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2024.4.11.post3/spai/image/__init__.py
--rw-r--r--   0        0        0     1350 2023-10-30 11:07:40.856696 spai-2024.4.11.post3/spai/image/utils.py
--rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2024.4.11.post3/spai/image/xyz/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2024.4.11.post3/spai/image/xyz/cache.py
--rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2024.4.11.post3/spai/image/xyz/errors.py
--rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2024.4.11.post3/spai/image/xyz/get_image_tile.py
--rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2024.4.11.post3/spai/image/xyz/image_utils.py
--rw-r--r--   0        0        0       28 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/mails/__init__.py
--rw-r--r--   0        0        0     1334 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/mails/mimetypes.py
--rw-r--r--   0        0        0     2932 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/mails/send.py
--rw-r--r--   0        0        0     3305 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/models/Config.py
--rw-r--r--   0        0        0      984 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/models/StorageConfig.py
--rw-r--r--   0        0        0       27 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/models/__init__.py
--rw-r--r--   0        0        0      391 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/processing/__init__.py
--rw-r--r--   0        0        0      669 2024-03-28 15:02:41.834449 spai-2024.4.11.post3/spai/processing/autocategorize1D.py
--rw-r--r--   0        0        0      477 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/processing/colorize_raster.py
--rw-r--r--   0        0        0      932 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/processing/convert_array_to_vector.py
--rw-r--r--   0        0        0      291 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/processing/mask_raster.py
--rw-r--r--   0        0        0      682 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/processing/normalised_difference.py
--rw-r--r--   0        0        0     1239 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/processing/px_count.py
--rw-r--r--   0        0        0      107 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/processing/rasterio_mask.py
--rw-r--r--   0        0        0      266 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/processing/read_raster.py
--rw-r--r--   0        0        0      876 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/processing/save_table.py
--rw-r--r--   0        0        0      496 2024-03-28 15:02:41.834449 spai-2024.4.11.post3/spai/processing/utils.py
--rw-r--r--   0        0        0      475 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/project/__init__.py
--rw-r--r--   0        0        0      466 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/project/bck/GetLogs.py
--rw-r--r--   0        0        0     1018 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/project/bck/InstallReqs 2.py
--rw-r--r--   0        0        0     1018 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/project/bck/InstallReqs 3.py
--rw-r--r--   0        0        0      482 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/project/bck/RunService.py
--rw-r--r--   0        0        0      492 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/project/bck/ScheduleService.py
--rw-r--r--   0        0        0      510 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/project/bck/StopService.py
--rw-r--r--   0        0        0     1578 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/project/bck/main.py
--rw-r--r--   0        0        0      337 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/project/delete_project.py
--rw-r--r--   0        0        0     2060 2024-03-28 15:01:17.074615 spai-2024.4.11.post3/spai/project/deploy_folder.py
--rw-r--r--   0        0        0      408 2024-03-28 15:01:17.078615 spai-2024.4.11.post3/spai/project/deploy_template.py
--rw-r--r--   0        0        0     1203 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/project/download_template.py
--rw-r--r--   0        0        0      455 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/project/get_logs.py
--rw-r--r--   0        0        0      242 2024-02-13 11:22:06.405893 spai-2024.4.11.post3/spai/project/get_project_by_name.py
--rw-r--r--   0        0        0      172 2024-02-13 11:22:06.409893 spai-2024.4.11.post3/spai/project/get_projects.py
--rw-r--r--   0        0        0      344 2024-02-13 11:22:06.409893 spai-2024.4.11.post3/spai/project/get_service_by_name_type_project.py
--rw-r--r--   0        0        0     1616 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/project/get_services.py
--rw-r--r--   0        0        0      525 2024-02-21 09:43:40.417670 spai-2024.4.11.post3/spai/project/init_project.py
--rw-r--r--   0        0        0      726 2024-02-20 15:56:19.617848 spai-2024.4.11.post3/spai/project/install_requirements.py
--rw-r--r--   0        0        0     5617 2024-02-27 12:31:33.913016 spai-2024.4.11.post3/spai/project/project-template/README.md
--rw-r--r--   0        0        0      867 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/project/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0       36 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/project/project-template/apis/analytics/requirements.txt
--rw-r--r--   0        0        0     1800 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/project/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0       88 2024-03-13 09:12:15.507871 spai-2024.4.11.post3/spai/project/project-template/apis/xyz/requirements.txt
--rw-r--r--   0        0        0   748531 2024-03-13 09:12:15.511871 spai-2024.4.11.post3/spai/project/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0       39 2024-03-13 09:12:15.511871 spai-2024.4.11.post3/spai/project/project-template/notebooks/analytics/requirements.txt
--rw-r--r--   0        0        0     1602 2024-04-11 09:09:28.631609 spai-2024.4.11.post3/spai/project/project-template/scripts/analytics/main.py
--rw-r--r--   0        0        0       30 2024-03-13 09:12:15.511871 spai-2024.4.11.post3/spai/project/project-template/scripts/analytics/requirements.txt
--rw-r--r--   0        0        0     1076 2024-04-11 09:10:07.363737 spai-2024.4.11.post3/spai/project/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0       85 2024-04-11 09:09:55.963699 spai-2024.4.11.post3/spai/project/project-template/scripts/downloader/requirements.txt
--rw-r--r--   0        0        0      618 2024-03-13 09:12:15.511871 spai-2024.4.11.post3/spai/project/project-template/spai.config.yaml
--rw-r--r--   0        0        0     1523 2024-04-11 09:22:12.011397 spai-2024.4.11.post3/spai/project/project-template/uis/map/main.py
--rw-r--r--   0        0        0       23 2024-02-27 12:31:33.593015 spai-2024.4.11.post3/spai/project/project-template/uis/map/requirements.txt
--rw-r--r--   0        0        0     5242 2024-03-25 08:56:48.420217 spai-2024.4.11.post3/spai/project/run_local.py
--rw-r--r--   0        0        0      813 2024-03-13 09:12:15.511871 spai-2024.4.11.post3/spai/project/stop_service.py
--rw-r--r--   0        0        0       38 2024-02-13 11:22:06.413893 spai-2024.4.11.post3/spai/reports/__init__.py
--rw-r--r--   0        0        0     1328 2024-02-13 11:22:06.413893 spai-2024.4.11.post3/spai/reports/generate.py
--rw-r--r--   0        0        0     4709 2024-03-13 09:12:15.511871 spai-2024.4.11.post3/spai/repos/APIRepo.py
--rw-r--r--   0        0        0      997 2024-02-13 11:22:06.413893 spai-2024.4.11.post3/spai/repos/AuthRepo.py
--rw-r--r--   0        0        0      188 2024-02-13 11:22:06.413893 spai-2024.4.11.post3/spai/repos/MailsRepo.py
--rw-r--r--   0        0        0      200 2024-02-13 11:22:06.413893 spai-2024.4.11.post3/spai/repos/ReportsRepo.py
--rw-r--r--   0        0        0       60 2024-02-13 11:22:06.413893 spai-2024.4.11.post3/spai/repos/__init__.py
--rw-r--r--   0        0        0     2452 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     3716 2024-03-13 09:12:15.515871 spai-2024.4.11.post3/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     4527 2024-04-11 08:43:02.338399 spai-2024.4.11.post3/spai/storage/LocalStorage.py
--rw-r--r--   0        0        0     8449 2024-04-11 08:43:08.570420 spai-2024.4.11.post3/spai/storage/S3Storage.py
--rw-r--r--   0        0        0     1407 2024-03-13 09:12:15.515871 spai-2024.4.11.post3/spai/storage/Storage.py
--rw-r--r--   0        0        0     6077 2024-03-13 09:12:15.515871 spai-2024.4.11.post3/spai/storage/_S3Storage.py
--rw-r--r--   0        0        0      120 2024-03-13 09:12:15.515871 spai-2024.4.11.post3/spai/storage/__init__.py
--rw-r--r--   0        0        0      409 2024-03-13 09:12:15.515871 spai-2024.4.11.post3/spai/storage/create_s3.py
--rw-r--r--   0        0        0     1559 2024-04-10 12:59:59.948165 spai-2024.4.11.post3/spai/storage/decorators.py
--rw-r--r--   0        0        0      583 2024-03-13 09:12:15.515871 spai-2024.4.11.post3/spai/storage/minio.py
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 spai-2024.4.11.post3/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2024.4.11.post4/README.md
+-rw-r--r--   0        0        0      527 2024-04-11 14:49:19.952774 spai-2024.4.11.post4/pyproject.toml
+-rw-r--r--   0        0        0       29 2024-04-11 14:49:19.956774 spai-2024.4.11.post4/spai/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/analytics/__init__.py
+-rw-r--r--   0        0        0     5070 2024-04-11 14:45:20.895751 spai-2024.4.11.post4/spai/analytics/forest_monitoring.py
+-rw-r--r--   0        0        0    12191 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/analytics/water_quality.py
+-rw-r--r--   0        0        0       96 2024-02-13 11:22:06.401893 spai-2024.4.11.post4/spai/auth/__init__.py
+-rw-r--r--   0        0        0     1210 2024-02-13 11:22:06.401893 spai-2024.4.11.post4/spai/auth/auth.py
+-rw-r--r--   0        0        0       99 2024-02-13 11:22:06.401893 spai-2024.4.11.post4/spai/auth/is_logged.py
+-rw-r--r--   0        0        0      161 2024-02-13 11:22:06.401893 spai-2024.4.11.post4/spai/auth/logout.py
+-rw-r--r--   0        0        0     7202 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/cli.py
+-rw-r--r--   0        0        0        0 2024-02-13 11:22:06.401893 spai-2024.4.11.post4/spai/commands/__init__.py
+-rw-r--r--   0        0        0     1017 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/commands/auth.py
+-rw-r--r--   0        0        0     1160 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/commands/list.py
+-rw-r--r--   0        0        0       86 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/config/__init__.py
+-rw-r--r--   0        0        0     3583 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/config/validate.py
+-rw-r--r--   0        0        0     1324 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/config/vars.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2024.4.11.post4/spai/data/__init__.py
+-rw-r--r--   0        0        0       49 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/data/indices/__init__.py
+-rw-r--r--   0        0        0       54 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/data/indices/fwi/__init__.py
+-rw-r--r--   0        0        0     3234 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/data/indices/fwi/fwi_nasa.py
+-rw-r--r--   0        0        0      608 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     3941 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     6332 2024-04-11 13:22:00.598259 spai-2024.4.11.post4/spai/data/satellite/download_stac.py
+-rw-r--r--   0        0        0      647 2023-10-30 11:07:40.852696 spai-2024.4.11.post4/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0      725 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py
+-rw-r--r--   0        0        0      758 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py
+-rw-r--r--   0        0        0      758 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py
+-rw-r--r--   0        0        0      758 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHDEM30Downloader.py
+-rw-r--r--   0        0        0     3587 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2584 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1264 2023-10-30 11:07:40.856696 spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      282 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0     2222 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/stac/STACDownloader.py
+-rw-r--r--   0        0        0      208 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/stac/__init__.py
+-rw-r--r--   0        0        0      461 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/stac/aws/AWSDEM30Downloader.py
+-rw-r--r--   0        0        0      461 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/stac/aws/AWSDEM90Downloader.py
+-rw-r--r--   0        0        0      876 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/stac/aws/AWSDEMDownloader.py
+-rw-r--r--   0        0        0      392 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/stac/aws/AWSDownloader.py
+-rw-r--r--   0        0        0     1951 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py
+-rw-r--r--   0        0        0      233 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/stac/aws/__init__.py
+-rw-r--r--   0        0        0      456 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/stac/decorators.py
+-rw-r--r--   0        0        0      716 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/stac/pc/PCDownloader.py
+-rw-r--r--   0        0        0      802 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/stac/pc/PCS1GRDDownloader.py
+-rw-r--r--   0        0        0      120 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/stac/pc/__init__.py
+-rw-r--r--   0        0        0     8905 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/data/satellite/utils.py
+-rw-r--r--   0        0        0       84 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/data/vector/__init__.py
+-rw-r--r--   0        0        0     5533 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/data/vector/openstreetmap.py
+-rw-r--r--   0        0        0       71 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/errors/__init__.py
+-rw-r--r--   0        0        0      308 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/errors/auth.py
+-rw-r--r--   0        0        0      156 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/errors/mails.py
+-rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2024.4.11.post4/spai/image/__init__.py
+-rw-r--r--   0        0        0     1350 2023-10-30 11:07:40.856696 spai-2024.4.11.post4/spai/image/utils.py
+-rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2024.4.11.post4/spai/image/xyz/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2024.4.11.post4/spai/image/xyz/cache.py
+-rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2024.4.11.post4/spai/image/xyz/errors.py
+-rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2024.4.11.post4/spai/image/xyz/get_image_tile.py
+-rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2024.4.11.post4/spai/image/xyz/image_utils.py
+-rw-r--r--   0        0        0       28 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/mails/__init__.py
+-rw-r--r--   0        0        0     1334 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/mails/mimetypes.py
+-rw-r--r--   0        0        0     2932 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/mails/send.py
+-rw-r--r--   0        0        0     3305 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/models/Config.py
+-rw-r--r--   0        0        0      984 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/models/StorageConfig.py
+-rw-r--r--   0        0        0       27 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/models/__init__.py
+-rw-r--r--   0        0        0      391 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/processing/__init__.py
+-rw-r--r--   0        0        0      669 2024-03-28 15:02:41.834449 spai-2024.4.11.post4/spai/processing/autocategorize1D.py
+-rw-r--r--   0        0        0      477 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/processing/colorize_raster.py
+-rw-r--r--   0        0        0      932 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/processing/convert_array_to_vector.py
+-rw-r--r--   0        0        0      291 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/processing/mask_raster.py
+-rw-r--r--   0        0        0      682 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/processing/normalised_difference.py
+-rw-r--r--   0        0        0     1239 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/processing/px_count.py
+-rw-r--r--   0        0        0      107 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/processing/rasterio_mask.py
+-rw-r--r--   0        0        0      266 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/processing/read_raster.py
+-rw-r--r--   0        0        0      876 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/processing/save_table.py
+-rw-r--r--   0        0        0      496 2024-03-28 15:02:41.834449 spai-2024.4.11.post4/spai/processing/utils.py
+-rw-r--r--   0        0        0      475 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/project/__init__.py
+-rw-r--r--   0        0        0      466 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/project/bck/GetLogs.py
+-rw-r--r--   0        0        0     1018 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/project/bck/InstallReqs 2.py
+-rw-r--r--   0        0        0     1018 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/project/bck/InstallReqs 3.py
+-rw-r--r--   0        0        0      482 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/project/bck/RunService.py
+-rw-r--r--   0        0        0      492 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/project/bck/ScheduleService.py
+-rw-r--r--   0        0        0      510 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/project/bck/StopService.py
+-rw-r--r--   0        0        0     1578 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/project/bck/main.py
+-rw-r--r--   0        0        0      337 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/project/delete_project.py
+-rw-r--r--   0        0        0     2060 2024-03-28 15:01:17.074615 spai-2024.4.11.post4/spai/project/deploy_folder.py
+-rw-r--r--   0        0        0      408 2024-03-28 15:01:17.078615 spai-2024.4.11.post4/spai/project/deploy_template.py
+-rw-r--r--   0        0        0     1203 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/project/download_template.py
+-rw-r--r--   0        0        0      455 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/project/get_logs.py
+-rw-r--r--   0        0        0      242 2024-02-13 11:22:06.405893 spai-2024.4.11.post4/spai/project/get_project_by_name.py
+-rw-r--r--   0        0        0      172 2024-02-13 11:22:06.409893 spai-2024.4.11.post4/spai/project/get_projects.py
+-rw-r--r--   0        0        0      344 2024-02-13 11:22:06.409893 spai-2024.4.11.post4/spai/project/get_service_by_name_type_project.py
+-rw-r--r--   0        0        0     1616 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/project/get_services.py
+-rw-r--r--   0        0        0      525 2024-02-21 09:43:40.417670 spai-2024.4.11.post4/spai/project/init_project.py
+-rw-r--r--   0        0        0      726 2024-02-20 15:56:19.617848 spai-2024.4.11.post4/spai/project/install_requirements.py
+-rw-r--r--   0        0        0     5617 2024-02-27 12:31:33.913016 spai-2024.4.11.post4/spai/project/project-template/README.md
+-rw-r--r--   0        0        0      867 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/project/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0       36 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/project/project-template/apis/analytics/requirements.txt
+-rw-r--r--   0        0        0     1800 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/project/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0       88 2024-03-13 09:12:15.507871 spai-2024.4.11.post4/spai/project/project-template/apis/xyz/requirements.txt
+-rw-r--r--   0        0        0   748531 2024-03-13 09:12:15.511871 spai-2024.4.11.post4/spai/project/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0       39 2024-03-13 09:12:15.511871 spai-2024.4.11.post4/spai/project/project-template/notebooks/analytics/requirements.txt
+-rw-r--r--   0        0        0     1602 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/project/project-template/scripts/analytics/main.py
+-rw-r--r--   0        0        0       30 2024-03-13 09:12:15.511871 spai-2024.4.11.post4/spai/project/project-template/scripts/analytics/requirements.txt
+-rw-r--r--   0        0        0     1076 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/project/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0       85 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/project/project-template/scripts/downloader/requirements.txt
+-rw-r--r--   0        0        0      618 2024-03-13 09:12:15.511871 spai-2024.4.11.post4/spai/project/project-template/spai.config.yaml
+-rw-r--r--   0        0        0     1523 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/project/project-template/uis/map/main.py
+-rw-r--r--   0        0        0       23 2024-02-27 12:31:33.593015 spai-2024.4.11.post4/spai/project/project-template/uis/map/requirements.txt
+-rw-r--r--   0        0        0     5242 2024-03-25 08:56:48.420217 spai-2024.4.11.post4/spai/project/run_local.py
+-rw-r--r--   0        0        0      813 2024-03-13 09:12:15.511871 spai-2024.4.11.post4/spai/project/stop_service.py
+-rw-r--r--   0        0        0       38 2024-02-13 11:22:06.413893 spai-2024.4.11.post4/spai/reports/__init__.py
+-rw-r--r--   0        0        0     1328 2024-02-13 11:22:06.413893 spai-2024.4.11.post4/spai/reports/generate.py
+-rw-r--r--   0        0        0     4709 2024-03-13 09:12:15.511871 spai-2024.4.11.post4/spai/repos/APIRepo.py
+-rw-r--r--   0        0        0      997 2024-02-13 11:22:06.413893 spai-2024.4.11.post4/spai/repos/AuthRepo.py
+-rw-r--r--   0        0        0      188 2024-02-13 11:22:06.413893 spai-2024.4.11.post4/spai/repos/MailsRepo.py
+-rw-r--r--   0        0        0      200 2024-02-13 11:22:06.413893 spai-2024.4.11.post4/spai/repos/ReportsRepo.py
+-rw-r--r--   0        0        0       60 2024-02-13 11:22:06.413893 spai-2024.4.11.post4/spai/repos/__init__.py
+-rw-r--r--   0        0        0     2452 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     3716 2024-03-13 09:12:15.515871 spai-2024.4.11.post4/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     4527 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/storage/LocalStorage.py
+-rw-r--r--   0        0        0     8449 2024-04-11 11:16:27.098890 spai-2024.4.11.post4/spai/storage/S3Storage.py
+-rw-r--r--   0        0        0     1407 2024-03-13 09:12:15.515871 spai-2024.4.11.post4/spai/storage/Storage.py
+-rw-r--r--   0        0        0     6077 2024-03-13 09:12:15.515871 spai-2024.4.11.post4/spai/storage/_S3Storage.py
+-rw-r--r--   0        0        0      120 2024-03-13 09:12:15.515871 spai-2024.4.11.post4/spai/storage/__init__.py
+-rw-r--r--   0        0        0      409 2024-03-13 09:12:15.515871 spai-2024.4.11.post4/spai/storage/create_s3.py
+-rw-r--r--   0        0        0     1559 2024-04-11 11:16:27.102890 spai-2024.4.11.post4/spai/storage/decorators.py
+-rw-r--r--   0        0        0      583 2024-03-13 09:12:15.515871 spai-2024.4.11.post4/spai/storage/minio.py
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 spai-2024.4.11.post4/PKG-INFO
```

### Comparing `spai-2024.4.11.post3/pyproject.toml` & `spai-2024.4.11.post4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spai"
-version = "2024.04.11-3"
+version = "2024.04.11-4"
 description = ""
 authors = ["Juan Sensio <it@earthpulse.es>"]
 readme = "README.md"
 packages = [{include = "spai"}]
 
 [tool.poetry.scripts]
 spai = "spai.cli:app"
```

### Comparing `spai-2024.4.11.post3/spai/analytics/forest_monitoring.py` & `spai-2024.4.11.post4/spai/analytics/forest_monitoring.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,82 +6,111 @@
 from ..processing import mask_raster
 from ..processing import autocategorize1D
 from ..processing import px_count
 from ..processing import colorize_raster
 from ..processing import save_table
 
 
-def forest_monitoring(image_name, aoi_mask, storage):
+def format_name(name, prefix, date):
+    return prefix + name.format(date=date)
+
+
+def forest_monitoring(
+    image_name,
+    aoi_mask,
+    storage,
+    prefix="",  # prefix for the raster names
+    names={},
+):
+    default_names = {  # names for the raster files
+        "ndvi": "ndvi_{date}.tif",
+        "ndvi_masked": "ndvi_masked_{date}.tif",
+        "ndvi_categorized": "ndvi_categorized_{date}.tif",
+        "vegetation": "vegetation_{date}.tif",
+        "vegetation_masked": "vegetation_masked_{date}.tif",
+        "vegetation_masked_rgb": "vegetation_masked_rgb_{date}.tif",
+        "quality_masked": "quality_masked_{date}.tif",
+        "quality_masked_rgb": "quality_masked_rgb_{date}.tif",
+    }
+    names = {**default_names, **names}
+
     # read_raster image
     ds, raster = read_raster(image_name, storage)
 
+    # esto no siempre va a funcionar... si el nombre de la imagen no sigue el formato
     date_and_tif = image_name.split("_")[-1]
     date = date_and_tif.split(".")[0]
 
     # calculate ndvi
     ndvi = normalised_difference(raster)
 
     # save_raster ndvi
-    raster_name_ndvi = f"ndvi_{date}.tif"
+    raster_name_ndvi = format_name(names["ndvi"], prefix, date)
     storage.create(ndvi, raster_name_ndvi, ds=ds)
 
     # read_geojson aoi_mask
     aoi_mask_gdf = gpd.GeoDataFrame.from_features(aoi_mask, crs=4326)
 
     # mask_raster ndvi with aoi_mask
     ndvi_masked, _ = mask_raster(raster_name_ndvi, aoi_mask_gdf, storage)
 
     # save_raster ndvi_masked
-    raster_name_ndvi_masked = f"ndvi_masked_{date}.tif"
+    raster_name_ndvi_masked = format_name(names["ndvi_masked"], prefix, date)
     storage.create(ndvi_masked, raster_name_ndvi_masked, ds=ds)
 
     # autocategorize1D ndvi
     ndvi_categorized = autocategorize1D(ndvi)
 
     # save_raster ndvi_categorized
-    raster_name_ndvi_categorized = f"ndvi_categorized_{date}.tif"
+    raster_name_ndvi_categorized = format_name(names["ndvi_categorized"], prefix, date)
     storage.create(ndvi_categorized, raster_name_ndvi_categorized, ds=ds)
 
     # apply_threshold to ndvi_categorized
     threshold = 3
     vegetation = ndvi_categorized >= threshold
     vegetation = vegetation.astype(np.uint8)
 
     # save_raster vegetation
-    raster_name_vegetation = f"vegetation_{date}.tif"
+    raster_name_vegetation = format_name(names["vegetation"], prefix, date)
     storage.create(vegetation, raster_name_vegetation, ds=ds)
 
     # mask_raster vegetation with aoi_mask
     vegetation_masked, _ = mask_raster(raster_name_vegetation, aoi_mask_gdf, storage)
 
     # save_raster vegetation_masked
-    raster_name_vegetation_masked = f"vegetation_masked_{date}.tif"
+    raster_name_vegetation_masked = format_name(
+        names["vegetation_masked"], prefix, date
+    )
     storage.create(vegetation_masked, raster_name_vegetation_masked, ds=ds)
 
     # colorize_raster vegetation_masked
     vegetation_masked_rgb = colorize_raster(vegetation_masked)
 
     # save_raster vegetation_masked_rgb
-    raster_name_vegetation_masked_rgb = f"vegetation_masked_rgb_{date}.tif"
+    raster_name_vegetation_masked_rgb = format_name(
+        names["vegetation_masked_rgb"], prefix, date
+    )
     storage.create(vegetation_masked_rgb, raster_name_vegetation_masked_rgb, ds=ds)
 
     # mask_raster ndvi_categorized with aoi_mask
     quality_mask, _ = mask_raster(raster_name_ndvi_categorized, aoi_mask_gdf, storage)
 
     # save_raster quality_mask
-    raster_name_quality_mask = f"quality_masked_{date}.tif"
+    raster_name_quality_mask = format_name(names["quality_masked"], prefix, date)
     storage.create(quality_mask, raster_name_quality_mask, ds=ds)
 
     # colorize_raster quality_mask
     quality_mask_rgb = colorize_raster(
         quality_mask, colors=["orangered", "yellow", "lawngreen", "darkgreen"]
     )
 
     # save_raster quality_mask_rgb
-    raster_name_quality_mask_rgb = f"quality_masked_rgb_{date}.tif"
+    raster_name_quality_mask_rgb = format_name(
+        names["quality_masked_rgb"], prefix, date
+    )
     storage.create(quality_mask_rgb, raster_name_quality_mask_rgb, ds=ds)
 
     # px_count vegetation_masked
     growth = px_count(vegetation_masked, values=[0, 1])
 
     # div growth
     growth_hectarias = np.divide(
```

### Comparing `spai-2024.4.11.post3/spai/analytics/water_quality.py` & `spai-2024.4.11.post4/spai/analytics/water_quality.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/auth/auth.py` & `spai-2024.4.11.post4/spai/auth/auth.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/cli.py` & `spai-2024.4.11.post4/spai/cli.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/commands/auth.py` & `spai-2024.4.11.post4/spai/commands/auth.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/commands/list.py` & `spai-2024.4.11.post4/spai/commands/list.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/config/validate.py` & `spai-2024.4.11.post4/spai/config/validate.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/config/vars.py` & `spai-2024.4.11.post4/spai/config/vars.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/indices/fwi/fwi_nasa.py` & `spai-2024.4.11.post4/spai/data/indices/fwi/fwi_nasa.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/__init__.py` & `spai-2024.4.11.post4/spai/data/satellite/__init__.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/download.py` & `spai-2024.4.11.post4/spai/data/satellite/download.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/download_stac.py` & `spai-2024.4.11.post4/spai/data/satellite/download_stac.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     collection : str, optional
         Satellite collection to download, by default "sentinel-2-l2a"
     clip : Optional[bool], optional
         Clip the data to the area of interest, by default False
     crs : Optional[str], optional
         Coordinate Reference System, by default "epsg:4326"
     kwargs : dict
-        Extra parameters to pass to the downloader, such as cloud_cover, vegetation_percentage an so on.   TODO
+        Extra parameters to pass to the downloader, such as bands, cloud_cover, vegetation_percentage an so on.   TODO
 
     Returns
     -------
     xarray.Dataset
         Satellite imagery data in memory.
     """
     gdf = create_aoi_geodataframe(aoi, crs)
@@ -79,15 +79,15 @@
     aoi: Any,
     date: Optional[List[Union[str, datetime]]] = None,
     collection: str = "sentinel-2-l2a",
     name: Optional[str] = None,
     clip: Optional[bool] = False,
     crs: Optional[str] = "epsg:4326",
     **kwargs,
-) -> None:
+) -> List[str]:
     """
     Download satellite imagery data from a given area of interest (aoi) and date to a given storage.
 
     Parameters
     ----------
     storage : Storage
         Storage object to save the data.
@@ -98,15 +98,15 @@
     collection : str, optional
         Satellite collection to download, by default "sentinel-2-l2a"
     clip : Optional[bool], optional
         Clip the data to the area of interest, by default False
     crs : Optional[str], optional
         Coordinate Reference System, by default "epsg:4326"
     kwargs : dict
-        Extra parameters to pass to the downloader, such as cloud_cover, vegetation_percentage an so on.   TODO
+        Extra parameters to pass to the downloader, such as bands, cloud_cover, vegetation_percentage an so on.   TODO
 
     Returns
     -------
     None
     """
     data = load_satellite_imagery(aoi, date, collection, clip, crs, **kwargs)
     if not data:
@@ -140,15 +140,15 @@
     date : Optional[List[Union[str, datetime]]], optional
         Date of the image, by default None. If None, the available images of the last month will be loaded.
     collection : str, optional
         Satellite collection to download, by default "sentinel-2-l2a"
     crs : Optional[str], optional
         Coordinate Reference System, by default "epsg:4326"
     kwargs : dict
-        Extra parameters to pass to the downloader, such as cloud_cover, vegetation_percentage an so on.   TODO
+        Extra parameters to pass to the downloader, such as bands, cloud_cover, vegetation_percentage an so on.   TODO
 
     Returns
     -------
     dict
         Information about the available images. If no image is found, it returns None. If any extra parameter is given, it will be added to the output.
     """
     gdf = create_aoi_geodataframe(aoi, crs)
```

### Comparing `spai-2024.4.11.post3/spai/data/satellite/explore.py` & `spai-2024.4.11.post4/spai/data/satellite/explore.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py` & `spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py` & `spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py` & `spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHDEM30Downloader.py` & `spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHDEM30Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2024.4.11.post4/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/stac/STACDownloader.py` & `spai-2024.4.11.post4/spai/data/satellite/stac/STACDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/stac/aws/AWSDEMDownloader.py` & `spai-2024.4.11.post4/spai/data/satellite/stac/aws/AWSDEMDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py` & `spai-2024.4.11.post4/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/stac/pc/PCDownloader.py` & `spai-2024.4.11.post4/spai/data/satellite/stac/pc/PCDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/stac/pc/PCS1GRDDownloader.py` & `spai-2024.4.11.post4/spai/data/satellite/stac/pc/PCS1GRDDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/satellite/utils.py` & `spai-2024.4.11.post4/spai/data/satellite/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/data/vector/openstreetmap.py` & `spai-2024.4.11.post4/spai/data/vector/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/image/utils.py` & `spai-2024.4.11.post4/spai/image/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/image/xyz/cache.py` & `spai-2024.4.11.post4/spai/image/xyz/cache.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/image/xyz/errors.py` & `spai-2024.4.11.post4/spai/image/xyz/errors.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/image/xyz/get_image_tile.py` & `spai-2024.4.11.post4/spai/image/xyz/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/image/xyz/image_utils.py` & `spai-2024.4.11.post4/spai/image/xyz/image_utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/mails/mimetypes.py` & `spai-2024.4.11.post4/spai/mails/mimetypes.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/mails/send.py` & `spai-2024.4.11.post4/spai/mails/send.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/models/Config.py` & `spai-2024.4.11.post4/spai/models/Config.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/models/StorageConfig.py` & `spai-2024.4.11.post4/spai/models/StorageConfig.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/processing/autocategorize1D.py` & `spai-2024.4.11.post4/spai/processing/autocategorize1D.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/processing/convert_array_to_vector.py` & `spai-2024.4.11.post4/spai/processing/convert_array_to_vector.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/processing/normalised_difference.py` & `spai-2024.4.11.post4/spai/processing/normalised_difference.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/processing/px_count.py` & `spai-2024.4.11.post4/spai/processing/px_count.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/processing/save_table.py` & `spai-2024.4.11.post4/spai/processing/save_table.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/bck/InstallReqs 2.py` & `spai-2024.4.11.post4/spai/project/bck/InstallReqs 2.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/bck/InstallReqs 3.py` & `spai-2024.4.11.post4/spai/project/bck/InstallReqs 3.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/bck/main.py` & `spai-2024.4.11.post4/spai/project/bck/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/deploy_folder.py` & `spai-2024.4.11.post4/spai/project/deploy_folder.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/download_template.py` & `spai-2024.4.11.post4/spai/project/download_template.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/get_services.py` & `spai-2024.4.11.post4/spai/project/get_services.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/init_project.py` & `spai-2024.4.11.post4/spai/project/init_project.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/install_requirements.py` & `spai-2024.4.11.post4/spai/project/install_requirements.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/project-template/README.md` & `spai-2024.4.11.post4/spai/project/project-template/README.md`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/project-template/apis/analytics/main.py` & `spai-2024.4.11.post4/spai/project/project-template/apis/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/project-template/apis/xyz/main.py` & `spai-2024.4.11.post4/spai/project/project-template/apis/xyz/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/project-template/notebooks/analytics/main.ipynb` & `spai-2024.4.11.post4/spai/project/project-template/notebooks/analytics/main.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/project-template/scripts/analytics/main.py` & `spai-2024.4.11.post4/spai/project/project-template/scripts/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/project-template/scripts/downloader/main.py` & `spai-2024.4.11.post4/spai/project/project-template/scripts/downloader/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/project-template/spai.config.yaml` & `spai-2024.4.11.post4/spai/project/project-template/spai.config.yaml`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/project-template/uis/map/main.py` & `spai-2024.4.11.post4/spai/project/project-template/uis/map/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/run_local.py` & `spai-2024.4.11.post4/spai/project/run_local.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/project/stop_service.py` & `spai-2024.4.11.post4/spai/project/stop_service.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/reports/generate.py` & `spai-2024.4.11.post4/spai/reports/generate.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/repos/APIRepo.py` & `spai-2024.4.11.post4/spai/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/repos/AuthRepo.py` & `spai-2024.4.11.post4/spai/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/storage/BaseStorage.py` & `spai-2024.4.11.post4/spai/storage/BaseStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/storage/CloudStorage.py` & `spai-2024.4.11.post4/spai/storage/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/storage/LocalStorage.py` & `spai-2024.4.11.post4/spai/storage/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/storage/S3Storage.py` & `spai-2024.4.11.post4/spai/storage/S3Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/storage/Storage.py` & `spai-2024.4.11.post4/spai/storage/Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/storage/_S3Storage.py` & `spai-2024.4.11.post4/spai/storage/_S3Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/storage/decorators.py` & `spai-2024.4.11.post4/spai/storage/decorators.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/spai/storage/minio.py` & `spai-2024.4.11.post4/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post3/PKG-INFO` & `spai-2024.4.11.post4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spai
-Version: 2024.4.11.post3
+Version: 2024.4.11.post4
 Summary: 
 Author: Juan Sensio
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

